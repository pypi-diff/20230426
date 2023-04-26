# Comparing `tmp/pharmpy-core-0.93.2.tar.gz` & `tmp/pharmpy-core-0.94.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pharmpy-core-0.93.2.tar", last modified: Thu Apr 20 14:07:14 2023, max compression
+gzip compressed data, was "pharmpy-core-0.94.0.tar", last modified: Wed Apr 26 11:35:39 2023, max compression
```

## Comparing `pharmpy-core-0.93.2.tar` & `pharmpy-core-0.94.0.tar`

### file list

```diff
@@ -1,1182 +1,1182 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.425886 pharmpy-core-0.93.2/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    44506 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/LICENSE.LESSER
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    46471 2023-04-20 14:07:14.425886 pharmpy-core-0.93.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.297885 pharmpy-core-0.93.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    10512 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/NONMEM.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14367 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/Pharmpy_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/Pharmpy_logo_dark.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.297885 pharmpy-core-0.93.2/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/_ext/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/_ext/pharmpy_snippet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/allometry.rst
--rw-r--r--   0 runner    (1001) docker     (123)    24284 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/amd.rst
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/api_model.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/api_modeling.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/api_tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/api_workflows.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/bootstrap.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/cdd.rst
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/citation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/code_of_conduct.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/contributors.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/covsearch.rst
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/crossval.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/data.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/design.rst
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/developers.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10499 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/estmethod.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/frem.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/help_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/iivsearch.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.297885 pharmpy-core-0.93.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/images/Pharmpy_symbol.svg
--rw-r--r--   0 runner    (1001) docker     (123)   179150 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/images/tools.png
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/iovsearch.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/linearize.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/model.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/modelfit.rst
--rw-r--r--   0 runner    (1001) docker     (123)    28177 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/modeling.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16031 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/modelsearch.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/nonmem_plugin.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12416 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/pharmr_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/plots.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/projects.rst
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/psn_resmod.rst
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/psn_tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/qa.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/ruvsearch.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/scm.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/simeval.rst
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/user_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/docs/using_r.rst
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-20 14:07:14.425886 pharmpy-core-0.93.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3229 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.297885 pharmpy-core-0.93.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.297885 pharmpy-core-0.93.2/src/pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    80309 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.297885 pharmpy-core-0.93.2/src/pharmpy/deps/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/deps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/deps/altair.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/deps/rich.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/deps/scipy.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/deps/sympy_printing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.297885 pharmpy-core-0.93.2/src/pharmpy/internals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/code_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/df.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.297885 pharmpy-core-0.93.2/src/pharmpy/internals/ds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/ds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/ds/ordered_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.301885 pharmpy-core-0.93.2/src/pharmpy/internals/expr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/expr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/expr/assumptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/expr/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/expr/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/expr/leaves.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/expr/ode.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/expr/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/expr/subs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/expr/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/expr/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.301885 pharmpy-core-0.93.2/src/pharmpy/internals/fn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/fn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/fn/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/fn/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.301885 pharmpy-core-0.93.2/src/pharmpy/internals/fs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/fs/cwd.py
--rw-r--r--   0 runner    (1001) docker     (123)    19768 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/fs/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/fs/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/fs/tmp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.281884 pharmpy-core-0.93.2/src/pharmpy/internals/graph/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.301885 pharmpy-core-0.93.2/src/pharmpy/internals/graph/directed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/graph/directed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/graph/directed/connected_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/graph/directed/inverse.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/graph/directed/reachability.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/immutable.py
--rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.301885 pharmpy-core-0.93.2/src/pharmpy/internals/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/module/lazy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.305884 pharmpy-core-0.93.2/src/pharmpy/internals/parse/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15783 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/parse/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/parse/ignored.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/parse/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/parse/prettyprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/parse/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/parse/treeprint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.305884 pharmpy-core-0.93.2/src/pharmpy/internals/sequence/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/sequence/lcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.305884 pharmpy-core-0.93.2/src/pharmpy/internals/set/
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/set/partitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/set/subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/internals/unicode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.305884 pharmpy-core-0.93.2/src/pharmpy/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/model/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    28256 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/model/datainfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.305884 pharmpy-core-0.93.2/src/pharmpy/model/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/model/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/model/distributions/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)    18153 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/model/distributions/symbolic.py
--rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/model/estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16087 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/model/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    32839 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/model/random_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     8281 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/model/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    65698 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/model/statements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.309885 pharmpy-core-0.93.2/src/pharmpy/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/allometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/basic_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/block_rvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/blq.py
--rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/compartments.py
--rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/covariate_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)    49857 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    33875 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/estimation_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/eta_additions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7964 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/eta_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)    14677 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.313885 pharmpy-core-0.93.2/src/pharmpy/modeling/example_models/
--rw-r--r--   0 runner    (1001) docker     (123)    50310 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/example_models/moxo.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/example_models/moxo.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/example_models/pheno.cov
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/example_models/pheno.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/example_models/pheno.dta
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/example_models/pheno.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/example_models/pheno.lst
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/example_models/pheno.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/example_models/pheno.phi
--rw-r--r--   0 runner    (1001) docker     (123)    90151 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/example_models/pheno.tab
--rw-r--r--   0 runner    (1001) docker     (123)   298562 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/example_models/pheno_linear.dta
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/example_models/pheno_linear.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/example_models/pheno_linear.lst
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/example_models/pheno_linear.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/example_models/pheno_linear.phi
--rw-r--r--   0 runner    (1001) docker     (123)    45291 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/help_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/lrt.py
--rw-r--r--   0 runner    (1001) docker     (123)    19401 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/metabolite.py
--rw-r--r--   0 runner    (1001) docker     (123)    70935 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/odes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/parameter_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    15780 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/remove_iiv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/remove_iov.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)    25078 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/tmdd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/update_inits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/modeling/write_csv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.313885 pharmpy-core-0.93.2/src/pharmpy/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.313885 pharmpy-core-0.93.2/src/pharmpy/plugins/fcon/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/fcon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/fcon/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.313885 pharmpy-core-0.93.2/src/pharmpy/plugins/nlmixr/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nlmixr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nlmixr/error_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nlmixr/ini.py
--rw-r--r--   0 runner    (1001) docker     (123)    23568 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nlmixr/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nlmixr/model_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nlmixr/name_mangle.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nlmixr/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    10780 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nlmixr/sanity_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.313885 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21621 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/advan.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/detect.py
--rw-r--r--   0 runner    (1001) docker     (123)    14734 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/nmtran_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    28217 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.317885 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/abbreviated_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    25142 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/code_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/data_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/estimation_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/etas_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.317885 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/grammars/
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/grammars/abbreviated_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/grammars/code_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/grammars/data_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/grammars/definitions.lark
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/grammars/omega_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/grammars/option_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/grammars/problem_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/grammars/simulation_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/grammars/theta_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/model_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    17573 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/omega_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/option_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/problem_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/raw_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/record.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/simulation_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/sizes_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/subroutine_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/table_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/theta_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    20153 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/results_file.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7135 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    64128 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.317885 pharmpy-core-0.93.2/src/pharmpy/plugins/rxode/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/rxode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14079 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/rxode/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/plugins/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.317885 pharmpy-core-0.93.2/src/pharmpy/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/reporting/altairplot.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/reporting/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/reporting/custom.css
--rwxr-xr-x   0 runner    (1001) docker     (123)     5562 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/reporting/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.321885 pharmpy-core-0.93.2/src/pharmpy/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.321885 pharmpy-core-0.93.2/src/pharmpy/tools/allometry/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/allometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/allometry/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.321885 pharmpy-core-0.93.2/src/pharmpy/tools/amd/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/amd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/amd/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/amd/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    16039 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/amd/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.321885 pharmpy-core-0.93.2/src/pharmpy/tools/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/bootstrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/bootstrap/report.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/bootstrap/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/bootstrap/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.321885 pharmpy-core-0.93.2/src/pharmpy/tools/cdd/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/cdd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/cdd/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.321885 pharmpy-core-0.93.2/src/pharmpy/tools/covsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/covsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/covsearch/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    19893 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/covsearch/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.321885 pharmpy-core-0.93.2/src/pharmpy/tools/crossval/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/crossval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/crossval/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.321885 pharmpy-core-0.93.2/src/pharmpy/tools/estmethod/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/estmethod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/estmethod/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/estmethod/report.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/estmethod/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.321885 pharmpy-core-0.93.2/src/pharmpy/tools/evaldesign/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/evaldesign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/evaldesign/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.321885 pharmpy-core-0.93.2/src/pharmpy/tools/frem/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/frem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/frem/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/frem/report.rst
--rw-r--r--   0 runner    (1001) docker     (123)    38407 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/frem/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/frem/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.321885 pharmpy-core-0.93.2/src/pharmpy/tools/funcs/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/funcs/ml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.321885 pharmpy-core-0.93.2/src/pharmpy/tools/funcs/ml_models/
--rw-r--r--   0 runner    (1001) docker     (123)    91484 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/funcs/ml_models/infinds.tflite
--rw-r--r--   0 runner    (1001) docker     (123)    93596 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/funcs/ml_models/outliers.tflite
--rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/funcs/summarize_individuals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.325885 pharmpy-core-0.93.2/src/pharmpy/tools/iivsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/iivsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/iivsearch/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/iivsearch/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.325885 pharmpy-core-0.93.2/src/pharmpy/tools/iovsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/iovsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/iovsearch/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.325885 pharmpy-core-0.93.2/src/pharmpy/tools/linearize/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/linearize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/linearize/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/linearize/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.325885 pharmpy-core-0.93.2/src/pharmpy/tools/mfl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/mfl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.325885 pharmpy-core-0.93.2/src/pharmpy/tools/mfl/feature/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/mfl/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/mfl/feature/absorption.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/mfl/feature/covariate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/mfl/feature/elimination.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/mfl/feature/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/mfl/feature/lagtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/mfl/feature/peripherals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/mfl/feature/transits.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/mfl/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/mfl/grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/mfl/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/mfl/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/mfl/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.325885 pharmpy-core-0.93.2/src/pharmpy/tools/mfl/statement/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/mfl/statement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/mfl/statement/definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.325885 pharmpy-core-0.93.2/src/pharmpy/tools/mfl/statement/feature/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/mfl/statement/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/mfl/statement/feature/absorption.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/mfl/statement/feature/count_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/mfl/statement/feature/covariate.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/mfl/statement/feature/elimination.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/mfl/statement/feature/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/mfl/statement/feature/lagtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/mfl/statement/feature/peripherals.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/mfl/statement/feature/symbols.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/mfl/statement/feature/transits.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/mfl/statement/statement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/mfl/stringify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.325885 pharmpy-core-0.93.2/src/pharmpy/tools/modelfit/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/modelfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/modelfit/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/modelfit/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.329885 pharmpy-core-0.93.2/src/pharmpy/tools/modelsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/modelsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/modelsearch/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/modelsearch/tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/psn_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.329885 pharmpy-core-0.93.2/src/pharmpy/tools/qa/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/qa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18713 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/qa/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/rankfuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31937 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.329885 pharmpy-core-0.93.2/src/pharmpy/tools/ruvsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/ruvsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/ruvsearch/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    16608 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/ruvsearch/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.329885 pharmpy-core-0.93.2/src/pharmpy/tools/scm/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/scm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/scm/psn_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    27585 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/scm/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.329885 pharmpy-core-0.93.2/src/pharmpy/tools/simeval/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/simeval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/simeval/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.329885 pharmpy-core-0.93.2/src/pharmpy/tools/simfit/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/simfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/simfit/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/tools/wrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.329885 pharmpy-core-0.93.2/src/pharmpy/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/workflows/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/workflows/call.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/workflows/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.329885 pharmpy-core-0.93.2/src/pharmpy/workflows/dispatchers/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/workflows/dispatchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/workflows/dispatchers/local_dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/workflows/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/workflows/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.329885 pharmpy-core-0.93.2/src/pharmpy/workflows/model_database/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/workflows/model_database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/workflows/model_database/baseclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    12168 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/workflows/model_database/local_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/workflows/model_database/null_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/workflows/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/workflows/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.329885 pharmpy-core-0.93.2/src/pharmpy/workflows/tool_database/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/workflows/tool_database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/workflows/tool_database/baseclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/workflows/tool_database/local_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/workflows/tool_database/null_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/src/pharmpy/workflows/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.333885 pharmpy-core-0.93.2/src/pharmpy_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    46471 2023-04-20 14:07:14.000000 pharmpy-core-0.93.2/src/pharmpy_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    46649 2023-04-20 14:07:14.000000 pharmpy-core-0.93.2/src/pharmpy_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:07:14.000000 pharmpy-core-0.93.2/src/pharmpy_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-20 14:07:14.000000 pharmpy-core-0.93.2/src/pharmpy_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:02:02.000000 pharmpy-core-0.93.2/src/pharmpy_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-20 14:07:14.000000 pharmpy-core-0.93.2/src/pharmpy_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-20 14:07:14.000000 pharmpy-core-0.93.2/src/pharmpy_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.333885 pharmpy-core-0.93.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.333885 pharmpy-core-0.93.2/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/cli/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.333885 pharmpy-core-0.93.2/tests/config/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/config/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.333885 pharmpy-core-0.93.2/tests/deps/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/deps/test_deps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.333885 pharmpy-core-0.93.2/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/integration/test_allometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/integration/test_amd.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/integration/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/integration/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/integration/test_covsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/integration/test_estmethod.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/integration/test_evaldesign.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/integration/test_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/integration/test_iivsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/integration/test_iovsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/integration/test_modelsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/integration/test_resume.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/integration/test_ruvsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.333885 pharmpy-core-0.93.2/tests/internals/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.333885 pharmpy-core-0.93.2/tests/internals/fs/
--rw-r--r--   0 runner    (1001) docker     (123)    15348 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/internals/fs/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/internals/fs/test_tmp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.333885 pharmpy-core-0.93.2/tests/internals/module/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/internals/module/test_lazy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/internals/test_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/internals/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.333885 pharmpy-core-0.93.2/tests/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/model/test_datainfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/model/test_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/model/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/model/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    27417 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/model/test_random_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    12560 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/model/test_statements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.337885 pharmpy-core-0.93.2/tests/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14199 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/modeling/test_add_covariate_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/modeling/test_allometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/modeling/test_basic_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/modeling/test_block_rvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/modeling/test_blq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/modeling/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/modeling/test_compartments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/modeling/test_covariate_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/modeling/test_data_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16918 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/modeling/test_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    27448 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/modeling/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/modeling/test_estimation_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/modeling/test_eta_additions.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/modeling/test_eta_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/modeling/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)    20575 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/modeling/test_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/modeling/test_has_covariate_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/modeling/test_help_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/modeling/test_iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/modeling/test_lrt.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/modeling/test_metabolite.py
--rw-r--r--   0 runner    (1001) docker     (123)   100179 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/modeling/test_modeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/modeling/test_parameter_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/modeling/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/modeling/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/modeling/test_remove_covariate_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/modeling/test_results.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/modeling/test_tmdd.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/modeling/test_units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.341885 pharmpy-core-0.93.2/tests/nonmem/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/nonmem/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.341885 pharmpy-core-0.93.2/tests/nonmem/output/
--rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/nonmem/output/test_nonmem_results_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.341885 pharmpy-core-0.93.2/tests/nonmem/records/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/nonmem/records/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/nonmem/records/test_abbreviated.py
--rw-r--r--   0 runner    (1001) docker     (123)    28301 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/nonmem/records/test_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/nonmem/records/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/nonmem/records/test_estimation_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/nonmem/records/test_etas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/nonmem/records/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/nonmem/records/test_model_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    10795 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/nonmem/records/test_omega.py
--rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/nonmem/records/test_option_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/nonmem/records/test_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/nonmem/records/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/nonmem/records/test_sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/nonmem/records/test_subroutines.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/nonmem/records/test_theta.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/nonmem/test_advan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/nonmem/test_des.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/nonmem/test_fcon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/nonmem/test_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/nonmem/test_modelfit_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    35906 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/nonmem/test_nonmem_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/nonmem/test_nonmem_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/nonmem/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/nonmem/test_read.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.341885 pharmpy-core-0.93.2/tests/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/plugins/test_nlmixr.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/plugins/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.341885 pharmpy-core-0.93.2/tests/testdata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.341885 pharmpy-core-0.93.2/tests/testdata/frem/
--rw-r--r--   0 runner    (1001) docker     (123)    52275 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/frem/results.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.345885 pharmpy-core-0.93.2/tests/testdata/nonmem/
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/DDMODEL00000130
--rw-r--r--   0 runner    (1001) docker     (123)    59142 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/Simulated_CMS_colistin_PK_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.345885 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real.lst
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.349885 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.353885 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    22061 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21670 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21677 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    22067 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.ext
--rw-r--r--   0 runner    (1001) docker     (123)    22454 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.ext
--rw-r--r--   0 runner    (1001) docker     (123)    22067 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_10.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_4.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_5.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_6.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_7.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_8.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_9.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/skipped_individuals1.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.353885 pharmpy-core-0.93.2/tests/testdata/nonmem/errors/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/errors/control_stream_error.lst
--rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/errors/est_step_warning.lst
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/errors/estimate_near_boundary_warning.lst
--rw-r--r--   0 runner    (1001) docker     (123)    23702 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/errors/no_header_error.ext
--rw-r--r--   0 runner    (1001) docker     (123)    19648 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/errors/no_header_error.lst
--rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/errors/rounding_error.lst
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/errors/run_interrupted.ext
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/errors/run_interrupted.mod
--rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/errors/zero_gradient_error.lst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.353885 pharmpy-core-0.93.2/tests/testdata/nonmem/fcon/
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/fcon/FCON
--rw-r--r--   0 runner    (1001) docker     (123)    39432 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/fcon/FDATA
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/file.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.285884 pharmpy-core-0.93.2/tests/testdata/nonmem/frem/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.353885 pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno/
--rw-r--r--   0 runner    (1001) docker     (123)    22896 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno/frem_dataset.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno/model_3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    11250 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno/model_3.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno/model_3.mod
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno/model_3.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno/model_3_input.phi
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno/model_4.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno/model_4.ext
--rw-r--r--   0 runner    (1001) docker     (123)    26246 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno/model_4.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno/model_4.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno/model_4.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno/model_4_input.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.357885 pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno_cat/
--rw-r--r--   0 runner    (1001) docker     (123)    24625 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno_cat/frem_dataset.dta
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno_cat/model_4.cor
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno_cat/model_4.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno_cat/model_4.ext
--rw-r--r--   0 runner    (1001) docker     (123)    26183 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno_cat/model_4.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno_cat/model_4.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno_cat/model_4.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno_cat/model_4_input.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.285884 pharmpy-core-0.93.2/tests/testdata/nonmem/linearize/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.357885 pharmpy-core-0.93.2/tests/testdata/nonmem/linearize/linearize_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/linearize/linearize_dir1/command.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14234 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.lst
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.357885 pharmpy-core-0.93.2/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.lst
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.phi
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/minimal.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.285884 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.357885 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/covariance/
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.coi
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17620 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.lst
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.285884 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/multPROB/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.285884 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/multPROB/multEST/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.357885 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/
--rw-r--r--   0 runner    (1001) docker     (123)    14783 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.ext
--rw-r--r--   0 runner    (1001) docker     (123)    91887 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.lst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.285884 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.285884 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.361885 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/
--rw-r--r--   0 runner    (1001) docker     (123)    36515 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/anneal2_V7_30_beta.lst
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.ext
--rw-r--r--   0 runner    (1001) docker     (123)    16505 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.lst
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13947 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.phi
--rw-r--r--   0 runner    (1001) docker     (123)    59168 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/superid2_6_V7_30_beta.lst
--rw-r--r--   0 runner    (1001) docker     (123)    37889 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.cov
--rw-r--r--   0 runner    (1001) docker     (123)   115118 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.ext
--rw-r--r--   0 runner    (1001) docker     (123)    82511 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.lst
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.mod
--rw-r--r--   0 runner    (1001) docker     (123)    75841 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.361885 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.ext
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.lst
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.285884 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.365885 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/
--rw-r--r--   0 runner    (1001) docker     (123)    15883 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/UseCase7.lst
--rw-r--r--   0 runner    (1001) docker     (123)    18122 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/example6b_V7_30_beta.lst
--rw-r--r--   0 runner    (1001) docker     (123)    15469 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/hessian_error.lst
--rw-r--r--   0 runner    (1001) docker     (123)    26695 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/large_s_matrix_cov_fail.lst
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.ext
--rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.lst
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.mod
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17548 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.phi
--rw-r--r--   0 runner    (1001) docker     (123)    13203 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_fail_nonp.lst
--rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_nocov_nonp.lst
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.ext
--rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.mod
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/nm710_fail_negV.lst
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17299 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.lst
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.phi
--rw-r--r--   0 runner    (1001) docker     (123)    16143 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno_nonp.lst
--rw-r--r--   0 runner    (1001) docker     (123)    14090 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/phenocorr.lst
--rw-r--r--   0 runner    (1001) docker     (123)    54699 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/sparse_matrix_with_msfi.lst
--rw-r--r--   0 runner    (1001) docker     (123)    31702 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo.lst
--rw-r--r--   0 runner    (1001) docker     (123)    19741 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_nonp.lst
--rw-r--r--   0 runner    (1001) docker     (123)    31702 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_withcov.lst
--rw-r--r--   0 runner    (1001) docker     (123)    13140 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/warfarin_ddmore.lst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.365885 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/
--rw-r--r--   0 runner    (1001) docker     (123)   178666 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.ext
--rw-r--r--   0 runner    (1001) docker     (123)  1091059 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.res
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.365885 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/simfit/
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/simfit/sim-1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    38485 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/simfit/sim-1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/simfit/sim-1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    41718 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/simfit/sim-1.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.369885 pharmpy-core-0.93.2/tests/testdata/nonmem/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modeling/pheno_1transit.mod
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modeling/pheno_2transits.mod
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modeling/pheno_advan1.mod
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modeling/pheno_advan11.mod
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modeling/pheno_advan12.mod
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modeling/pheno_advan1_zero_order.mod
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modeling/pheno_advan2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modeling/pheno_advan2_seq.mod
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modeling/pheno_advan3.mod
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modeling/pheno_advan4.mod
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modeling/pheno_advan5_depot.mod
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modeling/pheno_advan5_nodepot.mod
--rw-r--r--   0 runner    (1001) docker     (123)    18812 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modeling/pheno_zero_order.csv
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/modeling/transit_indirect_reabsorption.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.373885 pharmpy-core-0.93.2/tests/testdata/nonmem/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/fviii6.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/fviii6.mod
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/fviii6.prn
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/mox1.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/mox1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/mox1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/mox1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/mox1.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/mox2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    90456 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/mox2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/mox2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/mox2.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/mox_2comp.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/mox_2comp.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21336 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/mox_2comp.lst
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/mox_2comp.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/mox_2comp.phi
--rw-r--r--   0 runner    (1001) docker     (123)   175384 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/mox_simulated_log.csv
--rw-r--r--   0 runner    (1001) docker     (123)   185992 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/mox_simulated_normal.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/mox_simulated_normal.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)   105888 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/moxo_simulated_amd.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/moxo_simulated_amd.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/mytab_mox2
--rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/pef.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/pef.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/pheno_advan3_trans1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/pheno_advan3_trans1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/pheno_advan3_trans1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/pheno_advan3_trans1.phi
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/pheno_dvid.csv
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/pheno_dvid.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/pheno_noifs.coi
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/pheno_noifs.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/pheno_noifs.cov
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/pheno_noifs.ext
--rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/pheno_noifs.lst
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/pheno_noifs.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/pheno_noifs.phi
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/pheno_trans1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/pheno_trans1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/pheno_trans1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/models/pheno_trans1.phi
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/pheno.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/pheno.dta
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/pheno.ext
--rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/pheno.lst
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/pheno.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/pheno.phi
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_abbr.mod
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_abbr_comments.mod
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_block.mod
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_clashing_symbols.mod
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_etas.mod
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_multivariate_piecewise.mod
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_nm750.mod
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_no_obs_1stID.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36053 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_rate.dta
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_real.coi
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_real.cor
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_real.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_real.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_real.lst
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_real.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_real.phi
--rw-r--r--   0 runner    (1001) docker     (123)    90151 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_real.tab
--rw-r--r--   0 runner    (1001) docker     (123)    22114 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_real.xml
--rw-r--r--   0 runner    (1001) docker     (123)   298562 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_real_linbase.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_real_linbase.ext
--rw-r--r--   0 runner    (1001) docker     (123)    28308 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_real_linbase.lst
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_real_linbase.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_real_linbase.phi
--rw-r--r--   0 runner    (1001) docker     (123)    17010 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_real_linbase.tab
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.377885 pharmpy-core-0.93.2/tests/testdata/nonmem/qa/
--rw-r--r--   0 runner    (1001) docker     (123)   370034 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/qa/add_etas_linbase.dta
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/qa/add_etas_linbase.ext
--rw-r--r--   0 runner    (1001) docker     (123)    16579 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/qa/add_etas_linbase.lst
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/qa/add_etas_linbase.mod
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/qa/boxcox.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14595 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/qa/boxcox.lst
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/qa/boxcox.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/qa/boxcox.phi
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/qa/cdd_results.json
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/qa/fullblock.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17210 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/qa/fullblock.lst
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/qa/fullblock.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/qa/fullblock.phi
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/qa/iov.ext
--rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/qa/iov.lst
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/qa/iov.mod
--rw-r--r--   0 runner    (1001) docker     (123)    24133 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/qa/iov.phi
--rw-r--r--   0 runner    (1001) docker     (123)   262826 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/qa/pheno_linbase.dta
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/qa/pheno_linbase.ext
--rw-r--r--   0 runner    (1001) docker     (123)    15014 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/qa/pheno_linbase.lst
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/qa/pheno_linbase.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/qa/pheno_linbase.phi
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/qa/resmod_results.json
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/qa/scm_results.json
--rw-r--r--   0 runner    (1001) docker     (123)   392990 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/qa/simeval_results.json
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/qa/tdist.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17544 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/qa/tdist.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/qa/tdist.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/qa/tdist.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.377885 pharmpy-core-0.93.2/tests/testdata/nonmem/ruvsearch/
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/ruvsearch/mox3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    13182 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/ruvsearch/mox3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/ruvsearch/mox3.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12417 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/ruvsearch/mox3.phi
--rw-r--r--   0 runner    (1001) docker     (123)   276902 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/ruvsearch/moxo_simulated_resmod.csv
--rw-r--r--   0 runner    (1001) docker     (123)   180553 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/ruvsearch/mytab
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.377885 pharmpy-core-0.93.2/tests/testdata/nonmem/scm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.381885 pharmpy-core-0.93.2/tests/testdata/nonmem/scm/backward_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/scm/backward_dir1/config_fake.scm
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/scm/backward_dir1/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/scm/backward_dir1/scmlog.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.381885 pharmpy-core-0.93.2/tests/testdata/nonmem/scm/gofofv_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/scm/gofofv_dir1/scmlog.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/scm/localmin.logf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.381885 pharmpy-core-0.93.2/tests/testdata/nonmem/scm/log_steps/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/scm/log_steps/backward_ofv_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/scm/log_steps/backward_pval_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/scm/log_steps/backward_pval_2.txt
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/scm/log_steps/forward_ofv_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/scm/log_steps/forward_pval_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/scm/log_steps/forward_pval_2.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/scm/log_steps/forward_pval_3.txt
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/scm/log_steps/forward_pval_4.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.381885 pharmpy-core-0.93.2/tests/testdata/nonmem/scm/mergeofv_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/scm/mergeofv_dir1/config_havebaserun.scm
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/scm/mergeofv_dir1/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    38957 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/scm/mergeofv_dir1/scmlog.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.381885 pharmpy-core-0.93.2/tests/testdata/nonmem/scm/mergeofv_dir2/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/scm/mergeofv_dir2/config_havebaserun.scm
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/scm/mergeofv_dir2/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20500 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/scm/mergeofv_dir2/scmlog.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/scm/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.381885 pharmpy-core-0.93.2/tests/testdata/nonmem/scm/onlyforward_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/scm/onlyforward_dir1/config_normal.scm
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/scm/onlyforward_dir1/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/scm/onlyforward_dir1/scmlog.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.381885 pharmpy-core-0.93.2/tests/testdata/nonmem/scm/scm_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/scm/scm_dir1/scmlog.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.381885 pharmpy-core-0.93.2/tests/testdata/nonmem/scm/scmplus_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/scm/scmplus_dir1/scmlog.txt
--rw-r--r--   0 runner    (1001) docker     (123)   108031 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/sdtab1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.385885 pharmpy-core-0.93.2/tests/testdata/nonmem/secondary_parameters/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/secondary_parameters/pheno.cov
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/secondary_parameters/pheno.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/secondary_parameters/pheno.ext
--rw-r--r--   0 runner    (1001) docker     (123)    16221 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/secondary_parameters/pheno.lst
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/secondary_parameters/pheno.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/secondary_parameters/pheno.phi
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/secondary_parameters/run1.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/secondary_parameters/run1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    16509 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/secondary_parameters/run1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/secondary_parameters/run1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/secondary_parameters/run1.phi
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/secondary_parameters/run2.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/secondary_parameters/run2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17071 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/secondary_parameters/run2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/secondary_parameters/run2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/nonmem/secondary_parameters/run2.phi
--rw-r--r--   0 runner    (1001) docker     (123)    16730 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/pheno_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.289884 pharmpy-core-0.93.2/tests/testdata/psn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.385885 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/command.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13424 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/est_data0.dta
--rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/est_data1.dta
--rw-r--r--   0 runner    (1001) docker     (123)    13336 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/est_data2.dta
--rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/est_data3.dta
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.389885 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model0.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model0.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model0.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model0.lst
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model0.mod
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model0.phi
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model1.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model1.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model1.phi
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model2.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model2.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model2.phi
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model3.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model3.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model3.phi
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/pred_model0.ext
--rw-r--r--   0 runner    (1001) docker     (123)    11625 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/pred_model0.lst
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/pred_model0.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/pred_model0.phi
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/pred_model1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/pred_model1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/pred_model1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/pred_model1.phi
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/pred_model2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/pred_model2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/pred_model2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/pred_model2.phi
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/pred_model3.cor
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/pred_model3.cov
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/pred_model3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    15116 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/pred_model3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/pred_model3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/pred_model3.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/pred_data0.dta
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/pred_data1.dta
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/pred_data2.dta
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/pred_data3.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/version_and_option_info.txt
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/xv_result.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.393885 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/command.txt
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/covariates_summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.393885 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/final_models/
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/final_models/model_4.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/final_models/model_4.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/final_models/model_4.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/final_models/model_4.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/final_models/model_4_input.phi
--rw-r--r--   0 runner    (1001) docker     (123)    19440 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/frem_dataset.dta
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/frem_results.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.397885 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/filter_data_model.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/filter_data_model.lst
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/filter_data_model.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/filter_data_model.phi
--rw-r--r--   0 runner    (1001) docker     (123)    93135 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/filtered_plus_type0.dta
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_1.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    16221 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_1.phi
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_1b.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_1b.phi
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_2.cor
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_2.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21654 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_2.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_2.phi
--rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_2_input.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_3.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_3.mod
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_3.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_3_input.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_3b.ext
--rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_3b.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_3b.mod
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_3b.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_3b_input.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/proposal_density.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/version_and_option_info.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.397885 pharmpy-core-0.93.2/tests/testdata/psn/qa_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/qa_dir1/command.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.397885 pharmpy-core-0.93.2/tests/testdata/psn/qa_dir1/linearize_run/
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/qa_dir1/linearize_run/results.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.397885 pharmpy-core-0.93.2/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.ext
--rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.phi
--rw-r--r--   0 runner    (1001) docker     (123)   137744 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/extra_table
--rw-r--r--   0 runner    (1001) docker     (123)   316422 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/qa_dir1/pheno_real_linbase.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/qa_dir1/pheno_real_linbase.ext
--rw-r--r--   0 runner    (1001) docker     (123)    13850 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/qa_dir1/pheno_real_linbase.lst
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/qa_dir1/pheno_real_linbase.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/qa_dir1/pheno_real_linbase.phi
--rw-r--r--   0 runner    (1001) docker     (123)    11536 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/qa_dir1/results_summary.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.397885 pharmpy-core-0.93.2/tests/testdata/psn/resmod_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/resmod_dir1/resmod_results.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.397885 pharmpy-core-0.93.2/tests/testdata/psn/resmod_dir2/
--rw-r--r--   0 runner    (1001) docker     (123)    11647 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/resmod_dir2/resmod_results.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.397885 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.405885 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/
--rw-r--r--   0 runner    (1001) docker     (123)    63331 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/orig_pred.dta
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/original.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/original.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/original.ext
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/original.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/original.phi
--rw-r--r--   0 runner    (1001) docker     (123)    54391 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/original_res_table.dta
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/pheno.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-1.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-2.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-3.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-3.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-4.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-4.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-4.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-4.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-5.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-5.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-5.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-5.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-6.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-6.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-6.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-6.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-7.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-7.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-7.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-7.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-8.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-8.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-8.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-8.phi
--rw-r--r--   0 runner    (1001) docker     (123)    73024 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim_res_table-1.dta
--rw-r--r--   0 runner    (1001) docker     (123)    73024 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim_res_table-2.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim_res_table-3.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim_res_table-4.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim_res_table-5.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim_res_table-6.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim_res_table-7.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim_res_table-8.dta
--rw-r--r--   0 runner    (1001) docker     (123)    21489 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/summary_cwres.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.409886 pharmpy-core-0.93.2/tests/testdata/results/
--rw-r--r--   0 runner    (1001) docker     (123)    24788 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/allometry_results.json
--rw-r--r--   0 runner    (1001) docker     (123)   263999 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/amd_results.json
--rw-r--r--   0 runner    (1001) docker     (123)   130598 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/bootstrap_results.json
--rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/cdd_results.json
--rw-r--r--   0 runner    (1001) docker     (123)  1360720 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/covsearch_results.json
--rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/estmethod_results.json
--rw-r--r--   0 runner    (1001) docker     (123)   205797 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/iivsearch_results.json
--rw-r--r--   0 runner    (1001) docker     (123)   197228 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/iovsearch_results.json
--rw-r--r--   0 runner    (1001) docker     (123)    12639 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/linearize_results.json
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)   105603 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/modelsearch_results.json
--rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/qa_results.json
--rw-r--r--   0 runner    (1001) docker     (123)    57352 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/ruvsearch_results.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.289884 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.409886 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.409886 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.409886 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/.datasets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.289884 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.409886 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/-7907770233072098756/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/-7907770233072098756/input_model.csv
--rw-r--r--   0 runner    (1001) docker     (123)   183701 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:03:18.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.409886 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/input_model/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.409886 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/results.json
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/input_model/input_model.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.413885 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.413885 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/results.json
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    91188 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.phi
--rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/mytab_mox1
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/nonmem.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stderr
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stdout
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.417885 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.417885 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/results.json
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    91119 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.phi
--rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/mytab_mox2
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/nonmem.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stderr
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stdout
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.417885 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.417885 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)    53630 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/results.json
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    91754 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.mod
--rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.phi
--rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/mytab_mox3
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/nonmem.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stderr
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stdout
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.417885 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.417885 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)    54979 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/results.json
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.ext
--rw-r--r--   0 runner    (1001) docker     (123)    91879 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.lst
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.mod
--rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.phi
--rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/mytab_mox4
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/nonmem.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stderr
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stdout
--rw-r--r--   0 runner    (1001) docker     (123)    47403 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/results.csv
--rw-r--r--   0 runner    (1001) docker     (123)   105597 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/results.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.425886 pharmpy-core-0.93.2/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/tools/test_allometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/tools/test_amd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/tools/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/tools/test_cdd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/tools/test_covsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/tools/test_crossval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/tools/test_estmethod.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/tools/test_exports.py
--rw-r--r--   0 runner    (1001) docker     (123)    27814 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/tools/test_frem.py
--rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/tools/test_iivsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/tools/test_iovsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/tools/test_linearize.py
--rw-r--r--   0 runner    (1001) docker     (123)    11786 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/tools/test_mfl.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/tools/test_ml.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/tools/test_modelfit.py
--rw-r--r--   0 runner    (1001) docker     (123)    10258 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/tools/test_modelsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/tools/test_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/tools/test_rankfuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16975 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/tools/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/tools/test_runtool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/tools/test_ruvsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)    19845 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/tools/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/tools/test_simeval.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/tools/test_start_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/tools/test_summarize_individuals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/tools/test_wrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:07:14.425886 pharmpy-core-0.93.2/tests/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/workflows/test_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/workflows/test_execute.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/workflows/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/workflows/test_model_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/workflows/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/workflows/test_tool_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tests/workflows/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-20 14:00:55.000000 pharmpy-core-0.93.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.576880 pharmpy-core-0.94.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    44894 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/LICENSE.LESSER
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    46809 2023-04-26 11:35:39.576880 pharmpy-core-0.94.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.324879 pharmpy-core-0.94.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    10512 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/NONMEM.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14367 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/Pharmpy_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/Pharmpy_logo_dark.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.328879 pharmpy-core-0.94.0/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/_ext/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/_ext/pharmpy_snippet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/allometry.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    24284 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/amd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/api_model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/api_modeling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/api_tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/api_workflows.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/bootstrap.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/cdd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/citation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/code_of_conduct.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/contributors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/covsearch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/crossval.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/design.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/developers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10499 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/estmethod.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/frem.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/help_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/iivsearch.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.328879 pharmpy-core-0.94.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/images/Pharmpy_symbol.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   179150 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/images/tools.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/iovsearch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/linearize.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/modelfit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    28177 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/modeling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16031 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/modelsearch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/nonmem_plugin.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12416 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/pharmr_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/plots.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/projects.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/psn_resmod.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/psn_tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/qa.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/ruvsearch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/scm.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/simeval.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/user_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/using_r.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-26 11:35:39.576880 pharmpy-core-0.94.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3180 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.328879 pharmpy-core-0.94.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.328879 pharmpy-core-0.94.0/src/pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80309 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.332879 pharmpy-core-0.94.0/src/pharmpy/deps/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/deps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/deps/altair.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/deps/rich.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/deps/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/deps/sympy_printing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.332879 pharmpy-core-0.94.0/src/pharmpy/internals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/code_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/df.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.332879 pharmpy-core-0.94.0/src/pharmpy/internals/ds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/ds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/ds/ordered_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.336879 pharmpy-core-0.94.0/src/pharmpy/internals/expr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/expr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/expr/assumptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/expr/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/expr/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/expr/leaves.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/expr/ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/expr/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/expr/subs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/expr/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/expr/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.336879 pharmpy-core-0.94.0/src/pharmpy/internals/fn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/fn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/fn/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/fn/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.336879 pharmpy-core-0.94.0/src/pharmpy/internals/fs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/fs/cwd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19768 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/fs/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/fs/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/fs/tmp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.284879 pharmpy-core-0.94.0/src/pharmpy/internals/graph/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.336879 pharmpy-core-0.94.0/src/pharmpy/internals/graph/directed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/graph/directed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/graph/directed/connected_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/graph/directed/inverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/graph/directed/reachability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/immutable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.340879 pharmpy-core-0.94.0/src/pharmpy/internals/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/module/lazy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.340879 pharmpy-core-0.94.0/src/pharmpy/internals/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15783 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/parse/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/parse/ignored.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/parse/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/parse/prettyprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/parse/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/parse/treeprint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.340879 pharmpy-core-0.94.0/src/pharmpy/internals/sequence/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/sequence/lcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.340879 pharmpy-core-0.94.0/src/pharmpy/internals/set/
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/set/partitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/set/subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/unicode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.344879 pharmpy-core-0.94.0/src/pharmpy/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/model/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28168 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/model/datainfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.344879 pharmpy-core-0.94.0/src/pharmpy/model/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/model/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/model/distributions/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18153 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/model/distributions/symbolic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/model/estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16087 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/model/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32839 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/model/random_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8281 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/model/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68113 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/model/statements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.356879 pharmpy-core-0.94.0/src/pharmpy/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/allometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/basic_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/block_rvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/blq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/compartments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/covariate_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49857 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33875 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/estimation_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/eta_additions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7964 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/eta_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14677 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.364879 pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/
+-rw-r--r--   0 runner    (1001) docker     (123)    50310 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/moxo.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/moxo.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno.cov
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno.datainfo
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    90151 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno.tab
+-rw-r--r--   0 runner    (1001) docker     (123)   298562 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno_linear.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno_linear.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno_linear.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno_linear.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno_linear.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    45291 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/help_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/lrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19401 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/metabolite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71026 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/odes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/parameter_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15780 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/remove_iiv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/remove_iov.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25078 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/tmdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/update_inits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/write_csv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.364879 pharmpy-core-0.94.0/src/pharmpy/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.364879 pharmpy-core-0.94.0/src/pharmpy/plugins/fcon/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/fcon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/fcon/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.364879 pharmpy-core-0.94.0/src/pharmpy/plugins/nlmixr/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nlmixr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nlmixr/error_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nlmixr/ini.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23381 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nlmixr/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14368 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nlmixr/model_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nlmixr/name_mangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nlmixr/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10780 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nlmixr/sanity_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.368879 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22478 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/advan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14734 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/nmtran_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28819 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.372879 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/abbreviated_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25142 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/code_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/data_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/estimation_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/etas_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.372879 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/grammars/
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/grammars/abbreviated_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/grammars/code_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/grammars/data_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/grammars/definitions.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/grammars/omega_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/grammars/option_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/grammars/problem_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/grammars/simulation_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/grammars/theta_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/model_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17573 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/omega_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/option_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/problem_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/raw_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/simulation_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/sizes_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/subroutine_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/table_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/theta_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20153 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/results_file.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7135 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64128 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.372879 pharmpy-core-0.94.0/src/pharmpy/plugins/rxode/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/rxode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14079 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/rxode/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.372879 pharmpy-core-0.94.0/src/pharmpy/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/reporting/altairplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/reporting/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/reporting/custom.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5562 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/reporting/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.376879 pharmpy-core-0.94.0/src/pharmpy/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.376879 pharmpy-core-0.94.0/src/pharmpy/tools/allometry/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/allometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/allometry/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.376879 pharmpy-core-0.94.0/src/pharmpy/tools/amd/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/amd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/amd/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/amd/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16039 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/amd/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.376879 pharmpy-core-0.94.0/src/pharmpy/tools/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/bootstrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/bootstrap/report.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/bootstrap/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/bootstrap/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.376879 pharmpy-core-0.94.0/src/pharmpy/tools/cdd/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/cdd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/cdd/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.376879 pharmpy-core-0.94.0/src/pharmpy/tools/covsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/covsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/covsearch/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19893 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/covsearch/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.380879 pharmpy-core-0.94.0/src/pharmpy/tools/crossval/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/crossval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/crossval/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.380879 pharmpy-core-0.94.0/src/pharmpy/tools/estmethod/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/estmethod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/estmethod/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/estmethod/report.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/estmethod/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.380879 pharmpy-core-0.94.0/src/pharmpy/tools/evaldesign/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/evaldesign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/evaldesign/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.380879 pharmpy-core-0.94.0/src/pharmpy/tools/frem/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/frem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/frem/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/frem/report.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    38407 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/frem/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/frem/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.380879 pharmpy-core-0.94.0/src/pharmpy/tools/funcs/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/funcs/ml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.380879 pharmpy-core-0.94.0/src/pharmpy/tools/funcs/ml_models/
+-rw-r--r--   0 runner    (1001) docker     (123)    91484 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/funcs/ml_models/infinds.tflite
+-rw-r--r--   0 runner    (1001) docker     (123)    93596 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/funcs/ml_models/outliers.tflite
+-rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/funcs/summarize_individuals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.384879 pharmpy-core-0.94.0/src/pharmpy/tools/iivsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/iivsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/iivsearch/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/iivsearch/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.384879 pharmpy-core-0.94.0/src/pharmpy/tools/iovsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/iovsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/iovsearch/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.384879 pharmpy-core-0.94.0/src/pharmpy/tools/linearize/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/linearize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/linearize/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/linearize/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.384879 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.388879 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/feature/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/feature/absorption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/feature/covariate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/feature/elimination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/feature/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/feature/lagtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/feature/peripherals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/feature/transits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.388879 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.392879 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/feature/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/feature/absorption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/feature/count_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/feature/covariate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/feature/elimination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/feature/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/feature/lagtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/feature/peripherals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/feature/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/feature/transits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/stringify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.392879 pharmpy-core-0.94.0/src/pharmpy/tools/modelfit/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/modelfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/modelfit/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/modelfit/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.392879 pharmpy-core-0.94.0/src/pharmpy/tools/modelsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/modelsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/modelsearch/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/modelsearch/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/psn_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.392879 pharmpy-core-0.94.0/src/pharmpy/tools/qa/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/qa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18713 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/qa/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/rankfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31937 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.392879 pharmpy-core-0.94.0/src/pharmpy/tools/ruvsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/ruvsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/ruvsearch/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16608 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/ruvsearch/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.396879 pharmpy-core-0.94.0/src/pharmpy/tools/scm/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/scm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/scm/psn_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27585 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/scm/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.396879 pharmpy-core-0.94.0/src/pharmpy/tools/simeval/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/simeval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/simeval/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.396879 pharmpy-core-0.94.0/src/pharmpy/tools/simfit/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/simfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/simfit/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/wrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.396879 pharmpy-core-0.94.0/src/pharmpy/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/call.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.400879 pharmpy-core-0.94.0/src/pharmpy/workflows/dispatchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/dispatchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/dispatchers/local_dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.400879 pharmpy-core-0.94.0/src/pharmpy/workflows/model_database/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/model_database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/model_database/baseclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12168 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/model_database/local_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/model_database/null_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.400879 pharmpy-core-0.94.0/src/pharmpy/workflows/tool_database/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/tool_database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/tool_database/baseclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/tool_database/local_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/tool_database/null_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.404879 pharmpy-core-0.94.0/src/pharmpy_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    46809 2023-04-26 11:35:39.000000 pharmpy-core-0.94.0/src/pharmpy_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    46649 2023-04-26 11:35:39.000000 pharmpy-core-0.94.0/src/pharmpy_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 11:35:39.000000 pharmpy-core-0.94.0/src/pharmpy_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-26 11:35:39.000000 pharmpy-core-0.94.0/src/pharmpy_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 11:29:03.000000 pharmpy-core-0.94.0/src/pharmpy_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-26 11:35:39.000000 pharmpy-core-0.94.0/src/pharmpy_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 11:35:39.000000 pharmpy-core-0.94.0/src/pharmpy_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.404879 pharmpy-core-0.94.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.404879 pharmpy-core-0.94.0/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/cli/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.404879 pharmpy-core-0.94.0/tests/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/config/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.404879 pharmpy-core-0.94.0/tests/deps/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/deps/test_deps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.408879 pharmpy-core-0.94.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/integration/test_allometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/integration/test_amd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/integration/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/integration/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/integration/test_covsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/integration/test_estmethod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/integration/test_evaldesign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/integration/test_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/integration/test_iivsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/integration/test_iovsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/integration/test_modelsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/integration/test_resume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/integration/test_ruvsearch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.408879 pharmpy-core-0.94.0/tests/internals/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.408879 pharmpy-core-0.94.0/tests/internals/fs/
+-rw-r--r--   0 runner    (1001) docker     (123)    15348 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/internals/fs/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/internals/fs/test_tmp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.408879 pharmpy-core-0.94.0/tests/internals/module/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/internals/module/test_lazy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/internals/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/internals/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.412879 pharmpy-core-0.94.0/tests/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/model/test_datainfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/model/test_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/model/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/model/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27417 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/model/test_random_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12560 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/model/test_statements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.416879 pharmpy-core-0.94.0/tests/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14199 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_add_covariate_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_allometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_basic_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_block_rvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_blq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_compartments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_covariate_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_data_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16918 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27448 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_estimation_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_eta_additions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_eta_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20575 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_has_covariate_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_help_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_lrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_metabolite.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100500 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_parameter_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_remove_covariate_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_tmdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.420879 pharmpy-core-0.94.0/tests/nonmem/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.420879 pharmpy-core-0.94.0/tests/nonmem/output/
+-rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/output/test_nonmem_results_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.424879 pharmpy-core-0.94.0/tests/nonmem/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/records/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/records/test_abbreviated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28301 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/records/test_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/records/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/records/test_estimation_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/records/test_etas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/records/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/records/test_model_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10795 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/records/test_omega.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/records/test_option_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/records/test_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/records/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/records/test_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/records/test_subroutines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/records/test_theta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/test_advan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/test_des.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/test_fcon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/test_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/test_modelfit_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35906 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/test_nonmem_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/test_nonmem_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/test_read.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.424879 pharmpy-core-0.94.0/tests/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/plugins/test_nlmixr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/plugins/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.424879 pharmpy-core-0.94.0/tests/testdata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.424879 pharmpy-core-0.94.0/tests/testdata/frem/
+-rw-r--r--   0 runner    (1001) docker     (123)    52275 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/frem/results.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.436879 pharmpy-core-0.94.0/tests/testdata/nonmem/
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/DDMODEL00000130
+-rw-r--r--   0 runner    (1001) docker     (123)    59142 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/Simulated_CMS_colistin_PK_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.436879 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.436879 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.448880 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    22061 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21670 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21677 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    22067 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    22454 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    22067 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_10.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_5.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_6.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_7.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_8.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_9.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/skipped_individuals1.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.452880 pharmpy-core-0.94.0/tests/testdata/nonmem/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/errors/control_stream_error.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/errors/est_step_warning.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/errors/estimate_near_boundary_warning.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    23702 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/errors/no_header_error.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    19648 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/errors/no_header_error.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/errors/rounding_error.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/errors/run_interrupted.ext
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/errors/run_interrupted.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/errors/zero_gradient_error.lst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.456879 pharmpy-core-0.94.0/tests/testdata/nonmem/fcon/
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/fcon/FCON
+-rw-r--r--   0 runner    (1001) docker     (123)    39432 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/fcon/FDATA
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/file.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.296879 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.456879 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/
+-rw-r--r--   0 runner    (1001) docker     (123)    22896 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/frem_dataset.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    11250 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_3_input.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_4.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_4.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    26246 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_4.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_4.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_4_input.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.460880 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno_cat/
+-rw-r--r--   0 runner    (1001) docker     (123)    24625 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno_cat/frem_dataset.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cor
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno_cat/model_4.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    26183 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno_cat/model_4.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno_cat/model_4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno_cat/model_4.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno_cat/model_4_input.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.296879 pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.460880 pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/command.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    14234 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.464880 pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/minimal.mod
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.296879 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.464880 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/covariance/
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.coi
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17620 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.mod
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.296879 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/multPROB/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.296879 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.464880 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/
+-rw-r--r--   0 runner    (1001) docker     (123)    14783 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    91887 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.lst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.296879 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.296879 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.468880 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/
+-rw-r--r--   0 runner    (1001) docker     (123)    36515 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/anneal2_V7_30_beta.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    16505 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    13947 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    59168 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/superid2_6_V7_30_beta.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    37889 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.cov
+-rw-r--r--   0 runner    (1001) docker     (123)   115118 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    82511 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    75841 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.468880 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.mod
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.296879 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.484880 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/
+-rw-r--r--   0 runner    (1001) docker     (123)    15883 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/UseCase7.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    18122 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/example6b_V7_30_beta.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    15469 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/hessian_error.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    26695 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/large_s_matrix_cov_fail.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17548 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    13203 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_fail_nonp.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_nocov_nonp.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/nm710_fail_negV.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17299 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    16143 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno_nonp.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    14090 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/phenocorr.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    54699 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/sparse_matrix_with_msfi.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    31702 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    19741 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_nonp.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    31702 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_withcov.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    13140 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/warfarin_ddmore.lst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.484880 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/
+-rw-r--r--   0 runner    (1001) docker     (123)   178666 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.ext
+-rw-r--r--   0 runner    (1001) docker     (123)  1091059 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.res
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.488880 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/simfit/
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    38485 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    41718 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.488880 pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_1transit.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_2transits.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan11.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan12.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan1_zero_order.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan2_seq.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan5_depot.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan5_nodepot.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    18812 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_zero_order.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/transit_indirect_reabsorption.mod
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.496880 pharmpy-core-0.94.0/tests/testdata/nonmem/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/fviii6.datainfo
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/fviii6.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/fviii6.prn
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox1.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    90456 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox_2comp.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox_2comp.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21336 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox_2comp.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox_2comp.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox_2comp.phi
+-rw-r--r--   0 runner    (1001) docker     (123)   175384 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox_simulated_log.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   185992 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox_simulated_normal.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox_simulated_normal.datainfo
+-rw-r--r--   0 runner    (1001) docker     (123)   105888 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/moxo_simulated_amd.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/moxo_simulated_amd.datainfo
+-rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mytab_mox2
+-rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pef.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pef.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_advan3_trans1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_advan3_trans1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_advan3_trans1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_advan3_trans1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_dvid.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_dvid.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_noifs.coi
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_noifs.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_noifs.cov
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_noifs.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_noifs.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_noifs.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_noifs.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_trans1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_trans1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_trans1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_trans1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno.datainfo
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno.dta
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_abbr.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_abbr_comments.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_block.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_clashing_symbols.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_etas.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_multivariate_piecewise.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_nm750.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_no_obs_1stID.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    36053 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_rate.dta
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.coi
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    90151 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.tab
+-rw-r--r--   0 runner    (1001) docker     (123)    22114 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   298562 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real_linbase.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real_linbase.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    28308 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real_linbase.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real_linbase.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real_linbase.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    17010 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real_linbase.tab
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.504880 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/
+-rw-r--r--   0 runner    (1001) docker     (123)   370034 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/add_etas_linbase.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/add_etas_linbase.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    16579 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/add_etas_linbase.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/add_etas_linbase.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/boxcox.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    14595 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/boxcox.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/boxcox.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/boxcox.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/cdd_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/fullblock.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17210 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/fullblock.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/fullblock.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/fullblock.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/iov.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/iov.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/iov.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    24133 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/iov.phi
+-rw-r--r--   0 runner    (1001) docker     (123)   262826 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/pheno_linbase.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/pheno_linbase.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    15014 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/pheno_linbase.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/pheno_linbase.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/pheno_linbase.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/resmod_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/scm_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)   392990 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/simeval_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/tdist.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17544 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/tdist.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/tdist.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/tdist.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.504880 pharmpy-core-0.94.0/tests/testdata/nonmem/ruvsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/ruvsearch/mox3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    13182 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/ruvsearch/mox3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/ruvsearch/mox3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    12417 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/ruvsearch/mox3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)   276902 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/ruvsearch/moxo_simulated_resmod.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   180553 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/ruvsearch/mytab
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.508880 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.508880 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/backward_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/backward_dir1/config_fake.scm
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/backward_dir1/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/backward_dir1/scmlog.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.508880 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/gofofv_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/gofofv_dir1/scmlog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/localmin.logf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.508880 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/log_steps/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/log_steps/backward_ofv_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/log_steps/backward_pval_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/log_steps/backward_pval_2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/log_steps/forward_ofv_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/log_steps/forward_pval_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/log_steps/forward_pval_2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/log_steps/forward_pval_3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/log_steps/forward_pval_4.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.508880 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/mergeofv_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/mergeofv_dir1/config_havebaserun.scm
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/mergeofv_dir1/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    38957 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/mergeofv_dir1/scmlog.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.508880 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/mergeofv_dir2/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/mergeofv_dir2/config_havebaserun.scm
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/mergeofv_dir2/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20500 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/mergeofv_dir2/scmlog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.508880 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/onlyforward_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/onlyforward_dir1/config_normal.scm
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/onlyforward_dir1/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/onlyforward_dir1/scmlog.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.508880 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/scm_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/scm_dir1/scmlog.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.512880 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/scmplus_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/scmplus_dir1/scmlog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   108031 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/sdtab1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.512880 pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/pheno.cov
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/pheno.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/pheno.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    16221 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/pheno.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/pheno.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/pheno.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run1.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    16509 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run2.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17071 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    16730 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/pheno_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.304879 pharmpy-core-0.94.0/tests/testdata/psn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.516880 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/command.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13424 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/est_data0.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/est_data1.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    13336 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/est_data2.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/est_data3.dta
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.524880 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model0.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model0.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model0.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model0.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    11625 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cov
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    15116 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/pred_data0.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/pred_data1.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/pred_data2.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/pred_data3.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/version_and_option_info.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/xv_result.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.524880 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/command.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/covariates_summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.528880 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/final_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/final_models/model_4.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/final_models/model_4.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/final_models/model_4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/final_models/model_4.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/final_models/model_4_input.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    19440 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/frem_dataset.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/frem_results.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.532880 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    93135 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/filtered_plus_type0.dta
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_1.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    16221 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_1b.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_1b.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_2.cor
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_2.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21654 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_2_input.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3_input.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3b.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3b.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3b.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3b.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3b_input.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/proposal_density.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/version_and_option_info.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.532880 pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/command.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.536880 pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/linearize_run/
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/linearize_run/results.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.536880 pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.phi
+-rw-r--r--   0 runner    (1001) docker     (123)   137744 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/extra_table
+-rw-r--r--   0 runner    (1001) docker     (123)   316422 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    13850 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    11536 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/results_summary.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.536880 pharmpy-core-0.94.0/tests/testdata/psn/resmod_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/resmod_dir1/resmod_results.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.536880 pharmpy-core-0.94.0/tests/testdata/psn/resmod_dir2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11647 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/resmod_dir2/resmod_results.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.536880 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.548880 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/
+-rw-r--r--   0 runner    (1001) docker     (123)    63331 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/orig_pred.dta
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/original.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/original.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/original.ext
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/original.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/original.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    54391 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/original_res_table.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/pheno.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-4.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-4.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-4.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-5.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-5.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-5.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-5.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-6.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-6.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-6.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-6.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-7.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-7.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-7.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-7.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-8.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-8.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-8.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-8.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    73024 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-1.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    73024 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-2.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-3.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-4.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-5.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-6.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-7.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-8.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    21489 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/summary_cwres.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.552880 pharmpy-core-0.94.0/tests/testdata/results/
+-rw-r--r--   0 runner    (1001) docker     (123)    24788 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/allometry_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)   263999 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/amd_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)   130598 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/bootstrap_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/cdd_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1360720 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/covsearch_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/estmethod_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)   205797 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/iivsearch_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)   197228 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/iovsearch_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12639 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/linearize_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)   105603 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/modelsearch_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/qa_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)    57352 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/ruvsearch_results.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.304879 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.552880 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.552880 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.556880 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.304879 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.556880 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/-7907770233072098756/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/-7907770233072098756/input_model.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   183701 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.datainfo
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:30:47.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.556880 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.556880 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/results.json
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/input_model.mod
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.556880 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.556880 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    91188 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/mytab_mox1
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/nonmem.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stderr
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stdout
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.560880 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.560880 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    91119 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/mytab_mox2
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/nonmem.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stderr
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stdout
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.564880 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.564880 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)    53630 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    91754 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/mytab_mox3
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/nonmem.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stderr
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stdout
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.564880 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.568880 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)    54979 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    91879 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/mytab_mox4
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/nonmem.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stderr
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stdout
+-rw-r--r--   0 runner    (1001) docker     (123)    47403 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/results.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   105597 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/results.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.572880 pharmpy-core-0.94.0/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_allometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_amd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_cdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_covsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_crossval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_estmethod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27814 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_frem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_iivsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_iovsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_linearize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11786 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_mfl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_modelfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10258 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_modelsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_rankfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16975 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_runtool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_ruvsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19845 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_simeval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_start_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_summarize_individuals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.576880 pharmpy-core-0.94.0/tests/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/workflows/test_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/workflows/test_execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/workflows/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/workflows/test_model_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/workflows/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/workflows/test_tool_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/workflows/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tox.ini
```

### Comparing `pharmpy-core-0.93.2/AUTHORS.rst` & `pharmpy-core-0.94.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/CHANGELOG.rst` & `pharmpy-core-0.94.0/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+0.94.0 (2023-04-26)
+-------------------
+
+New features
+============
+
+* Support parsing assignments other than DADT in $DES in NONMEM
+* Fix parsing of some complex ODE-systems in NONMEM
+
+Changes
+=======
+
+* Drop support for Python 3.8
+
+Bugfixes
+========
+
+* Fix bug causing BIC calculation to fail for models having first order absorption and lag_time after going into zero order absorption
+
 0.93.0 (2023-04-19)
 -------------------
 
 New features
 ============
 
 * Add function ``modeling.get_zero_order_inputs``
```

### Comparing `pharmpy-core-0.93.2/CODE_OF_CONDUCT.rst` & `pharmpy-core-0.94.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/LICENSE` & `pharmpy-core-0.94.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/LICENSE.LESSER` & `pharmpy-core-0.94.0/LICENSE.LESSER`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/MANIFEST.in` & `pharmpy-core-0.94.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/PKG-INFO` & `pharmpy-core-0.94.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pharmpy-core
-Version: 0.93.2
+Version: 0.94.0
 Summary: Pharmacometric modeling
 Home-page: https://pharmpy.github.io
 Author: Rikard Nordgren
 Author-email: rikard.nordgren@farmaci.uu.se
 License: GNU Lesser General Public License v3 (LGPLv3)
 Project-URL: Bug Tracker, https://github.com/pharmpy/pharmpy/issues
 Project-URL: Source Code, https://github.com/pharmpy/pharmpy
@@ -16,21 +16,20 @@
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Provides-Extra: nlmixr
 License-File: LICENSE
 License-File: LICENSE.LESSER
 License-File: AUTHORS.rst
 
 Pharmpy is a library and toolkit for pharmacometrics. It can be used as a regular Python package, in R
 via the `pharmr <https://github.com/pharmpy/pharmr>`_ package or via its built in command
@@ -41,14 +40,33 @@
 * A model abstraction as a foundation for higher level operations on models
 * Functions for manipulation of models, e.g. changing model components like elimination or absorption
 * Reading NONMEM models and results
 * Running models and complex workflows (with NONMEM or to some extent nlmixr)
 
 This is the `team behind Pharmpy <https://pharmpy.github.io/latest/contributors.html>`_
 
+0.94.0 (2023-04-26)
+-------------------
+
+New features
+============
+
+* Support parsing assignments other than DADT in $DES in NONMEM
+* Fix parsing of some complex ODE-systems in NONMEM
+
+Changes
+=======
+
+* Drop support for Python 3.8
+
+Bugfixes
+========
+
+* Fix bug causing BIC calculation to fail for models having first order absorption and lag_time after going into zero order absorption
+
 0.93.0 (2023-04-19)
 -------------------
 
 New features
 ============
 
 * Add function ``modeling.get_zero_order_inputs``
```

### Comparing `pharmpy-core-0.93.2/README.rst` & `pharmpy-core-0.94.0/README.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/NONMEM.rst` & `pharmpy-core-0.94.0/docs/NONMEM.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/Pharmpy_logo.svg` & `pharmpy-core-0.94.0/docs/Pharmpy_logo.svg`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/Pharmpy_logo_dark.svg` & `pharmpy-core-0.94.0/docs/Pharmpy_logo_dark.svg`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/_ext/conversion.py` & `pharmpy-core-0.94.0/docs/_ext/conversion.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/_ext/pharmpy_snippet.py` & `pharmpy-core-0.94.0/docs/_ext/pharmpy_snippet.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/allometry.rst` & `pharmpy-core-0.94.0/docs/allometry.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/amd.rst` & `pharmpy-core-0.94.0/docs/amd.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/api.rst` & `pharmpy-core-0.94.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/bootstrap.rst` & `pharmpy-core-0.94.0/docs/bootstrap.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/cdd.rst` & `pharmpy-core-0.94.0/docs/cdd.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/cli.rst` & `pharmpy-core-0.94.0/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/conf.py` & `pharmpy-core-0.94.0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 source_suffix = '.rst'
 master_doc = 'index'
 project = 'Pharmpy'
 year = '2018-2023'
 authors = ['the Pharmpy development team']
 copyright = '{0}; {1}'.format(year, ', '.join(authors))
-version = release = '0.93.2'
+version = release = '0.94.0'
 html_show_sourcelink = False
 
 pygments_style = 'trac'
 templates_path = ['.']
 
 html_static_path = ['.']
 html_theme = "pydata_sphinx_theme"
```

### Comparing `pharmpy-core-0.93.2/docs/configuration.rst` & `pharmpy-core-0.94.0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/contribute.rst` & `pharmpy-core-0.94.0/docs/contribute.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/covsearch.rst` & `pharmpy-core-0.94.0/docs/covsearch.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/crossval.rst` & `pharmpy-core-0.94.0/docs/crossval.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/custom.css` & `pharmpy-core-0.94.0/docs/custom.css`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/data.rst` & `pharmpy-core-0.94.0/docs/data.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/design.rst` & `pharmpy-core-0.94.0/docs/design.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/estmethod.rst` & `pharmpy-core-0.94.0/docs/estmethod.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/frem.rst` & `pharmpy-core-0.94.0/docs/frem.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/getting_started.rst` & `pharmpy-core-0.94.0/docs/getting_started.rst`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 Installation
 ------------
 
 .. note::
     If you plan to use Pharmpy in R, please follow the steps in :ref:`install_pharmr`.
 
 .. warning::
-    Pharmpy requires python 3.8 or later, and is currently tested on python 3.8, 3.9, and 3.10 on
+    Pharmpy requires python 3.9 or later, and is currently tested on python 3.9, 3.10 and 3.11 on
     Linux, MacOS and Windows.
 
 Install the latest stable version from PyPI with::
 
    pip install pharmpy-core
 
 To be able to use components using machine learning the tflite package is needed. It can be installed using::
```

### Comparing `pharmpy-core-0.93.2/docs/help_functions.py` & `pharmpy-core-0.94.0/docs/help_functions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/iivsearch.rst` & `pharmpy-core-0.94.0/docs/iivsearch.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/images/Pharmpy_symbol.svg` & `pharmpy-core-0.94.0/docs/images/Pharmpy_symbol.svg`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/images/tools.png` & `pharmpy-core-0.94.0/docs/images/tools.png`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/index.rst` & `pharmpy-core-0.94.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/iovsearch.rst` & `pharmpy-core-0.94.0/docs/iovsearch.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/license.rst` & `pharmpy-core-0.94.0/docs/license.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/linearize.rst` & `pharmpy-core-0.94.0/docs/linearize.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/model.rst` & `pharmpy-core-0.94.0/docs/model.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/modelfit.rst` & `pharmpy-core-0.94.0/docs/modelfit.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/modeling.rst` & `pharmpy-core-0.94.0/docs/modeling.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/modelsearch.rst` & `pharmpy-core-0.94.0/docs/modelsearch.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/nonmem_plugin.rst` & `pharmpy-core-0.94.0/docs/nonmem_plugin.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/pharmr_logo.svg` & `pharmpy-core-0.94.0/docs/pharmr_logo.svg`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/plots.rst` & `pharmpy-core-0.94.0/docs/plots.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/plugins.rst` & `pharmpy-core-0.94.0/docs/plugins.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/projects.rst` & `pharmpy-core-0.94.0/docs/projects.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/qa.rst` & `pharmpy-core-0.94.0/docs/qa.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/ruvsearch.rst` & `pharmpy-core-0.94.0/docs/ruvsearch.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/scm.rst` & `pharmpy-core-0.94.0/docs/scm.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/simeval.rst` & `pharmpy-core-0.94.0/docs/simeval.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/tools.rst` & `pharmpy-core-0.94.0/docs/tools.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/docs/using_r.rst` & `pharmpy-core-0.94.0/docs/using_r.rst`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 sets up Miniconda it can default to use Python 3.8. If you have any trouble installing Pharmpy or any of its
 dependencies, you can do the following to check the Python version in your reticulate environment:
 
 .. code-block:: r
 
     reticulate::py_discover_config()
 
-Make sure the Python version is >= 3.8. If it is not, you can run the following in R:
+Make sure the Python version is >= 3.9. If it is not, you can run the following in R:
 
 .. code-block:: r
 
     reticulate::conda_create('r-reticulate', python_version = '3.11')
 
 Restart the session and try installing Pharmpy again:
```

### Comparing `pharmpy-core-0.93.2/requirements.txt` & `pharmpy-core-0.94.0/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,49 +23,49 @@
 entrypoints==0.4
 executing==1.2.0
 fastjsonschema==2.16.3
 fsspec==2023.4.0
 HeapDict==1.0.1
 idna==3.4
 imagesize==1.4.1
-importlib_metadata==6.5.0
+importlib_metadata==6.6.0
 ipykernel==6.22.0
 ipython==8.12.0
 ipywidgets==8.0.6
 jedi==0.18.2
 Jinja2==3.1.2
 jsonschema==4.17.3
-jupyter-client==7.3.4
+jupyter-client==8.2.0
 jupyter-core==5.3.0
 jupyter-sphinx==0.4.0
 jupyterlab-pygments==0.2.2
 jupyterlab-widgets==3.0.7
 lark==1.1.5
 locket==1.0.0
 lxml==4.9.2
 MarkupSafe==2.1.2
 matplotlib-inline==0.1.6
 mistune==2.0.5
 mpmath==1.3.0
 msgpack==1.0.5
-nbclient==0.7.3
+nbclient==0.7.4
 nbconvert==7.3.1
 nbformat==5.8.0
 nest-asyncio==1.5.6
 networkx==3.1
 numexpr==2.8.4
-numpy==1.24.2
+numpy==1.24.3
 packaging==23.1
 pandas==1.5.3
 pandocfilters==1.5.0
 parso==0.8.3
 partd==1.4.0
 pexpect==4.8.0
 pickleshare==0.7.5
-platformdirs==3.2.0
+platformdirs==3.3.0
 prompt-toolkit==3.0.38
 psutil==5.9.5
 ptyprocess==0.7.0
 pure-eval==0.2.2
 Pygments==2.15.1
 pyreadr==0.4.7
 pyrsistent==0.19.3
@@ -77,28 +77,28 @@
 pyzmq==25.0.2
 rich==13.3.4
 scipy==1.10.1
 six==1.16.0
 snowballstemmer==2.2.0
 sortedcontainers==2.4.0
 soupsieve==2.4.1
-Sphinx==6.1.3
+Sphinx==6.2.1
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
 sphinxcontrib.applehelp==1.0.4
 stack-data==0.6.2
 symengine==0.10.0
 sympy==1.11.1
 tblib==1.7.0
 tinycss2==1.2.1
 toolz==0.12.0
-tornado==6.3
+tornado==6.3.1
 traitlets==5.9.0
 urllib3==1.26.15
 wcwidth==0.2.6
 webencodings==0.5.1
 widgetsnbextension==4.0.7
 zict==3.0.0
 zipp==3.15.0
```

### Comparing `pharmpy-core-0.93.2/setup.cfg` & `pharmpy-core-0.94.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/setup.py` & `pharmpy-core-0.94.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     txt = re.compile(pat, re.MULTILINE | re.DOTALL).findall(text_str)
     txt = [dedent(block).strip() for block in txt]
     return '\n\n'.join(txt)
 
 
 setup(
     name='pharmpy-core',
-    version='0.93.2',
+    version='0.94.0',
     license='GNU Lesser General Public License v3 (LGPLv3)',
     description='Pharmacometric modeling',
     long_description='%s\n\n%s'
     % (strip_refs(longdesc(read('README.rst'))), strip_refs(read('CHANGELOG.rst'))),
     author='Rikard Nordgren',
     author_email='rikard.nordgren@farmaci.uu.se',
     url='https://pharmpy.github.io',
@@ -42,27 +42,26 @@
         "Source Code": 'https://github.com/pharmpy/pharmpy',
     },
     packages=find_packages('src'),
     package_dir={'': 'src'},
     py_modules=[splitext(basename(path))[0] for path in glob('src/*.py')],
     include_package_data=True,
     zip_safe=False,
-    python_requires='>=3.8',
+    python_requires='>=3.9',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
         'Operating System :: POSIX',
         'Operating System :: MacOS',
         'Operating System :: Unix',
         'Operating System :: Microsoft :: Windows',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Topic :: Scientific/Engineering',
     ],
     keywords=[
```

### Comparing `pharmpy-core-0.93.2/src/pharmpy/cli.py` & `pharmpy-core-0.94.0/src/pharmpy/cli.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/config.py` & `pharmpy-core-0.94.0/src/pharmpy/config.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/deps/__init__.py` & `pharmpy-core-0.94.0/src/pharmpy/deps/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/deps/altair.py` & `pharmpy-core-0.94.0/src/pharmpy/deps/altair.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/internals/df.py` & `pharmpy-core-0.94.0/src/pharmpy/internals/df.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/internals/ds/ordered_set.py` & `pharmpy-core-0.94.0/src/pharmpy/internals/ds/ordered_set.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/internals/expr/eval.py` & `pharmpy-core-0.94.0/src/pharmpy/internals/expr/eval.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/internals/expr/funcs.py` & `pharmpy-core-0.94.0/src/pharmpy/internals/expr/funcs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/internals/expr/leaves.py` & `pharmpy-core-0.94.0/src/pharmpy/internals/expr/leaves.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/internals/expr/ode.py` & `pharmpy-core-0.94.0/src/pharmpy/internals/expr/ode.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/internals/expr/subs.py` & `pharmpy-core-0.94.0/src/pharmpy/internals/expr/subs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/internals/expr/tree.py` & `pharmpy-core-0.94.0/src/pharmpy/internals/expr/tree.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/internals/expr/units.py` & `pharmpy-core-0.94.0/src/pharmpy/internals/expr/units.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/internals/fn/signature.py` & `pharmpy-core-0.94.0/src/pharmpy/internals/fn/signature.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/internals/fn/type.py` & `pharmpy-core-0.94.0/src/pharmpy/internals/fn/type.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 from collections.abc import Collection, Container, Iterable, Iterator, Sequence, Sized
 from inspect import signature
-from typing import Any
-from typing import Container as TypingContainer  # NOTE needed for Python 3.8
-from typing import Iterable as TypingIterable  # NOTE needed for Python 3.8
-from typing import List, Literal, Optional, Tuple, Type, Union, get_args, get_origin, get_type_hints
+from typing import (
+    Any,
+    List,
+    Literal,
+    Optional,
+    Tuple,
+    Type,
+    Union,
+    get_args,
+    get_origin,
+    get_type_hints,
+)
 
 
 def with_runtime_arguments_type_check(fn):
     sig = signature(fn)
     parameters = sig.parameters.values()
     type_hints = None
 
@@ -162,17 +170,17 @@
             return False
 
     if origin is Collection:
         t = get_args(typing)
         return (
             _match(Sized, value)
             and _match(
-                TypingContainer[t] if t else Container,  # pyright: ignore [reportGeneralTypeIssues]
+                Container[t] if t else Container,  # pyright: ignore [reportGeneralTypeIssues]
                 value,
             )
             and _match(
-                TypingIterable[t] if t else Iterable,  # pyright: ignore [reportGeneralTypeIssues]
+                Iterable[t] if t else Iterable,  # pyright: ignore [reportGeneralTypeIssues]
                 value,
             )
         )
 
     raise NotImplementedError(origin)
```

### Comparing `pharmpy-core-0.93.2/src/pharmpy/internals/fs/lock.py` & `pharmpy-core-0.94.0/src/pharmpy/internals/fs/lock.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/internals/fs/path.py` & `pharmpy-core-0.94.0/src/pharmpy/internals/fs/path.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/internals/fs/tmp.py` & `pharmpy-core-0.94.0/src/pharmpy/internals/fs/tmp.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,23 +7,17 @@
 
 # NOTE This is copied from the Python 3.10 implementation to expose the
 # ignore_cleanup_errors flag and patch PermissionError handling for Windows
 # lock files. Here is the original source link:
 #
 # https://github.com/python/cpython/blob/b494f5935c92951e75597bfe1c8b1f3112fec270/Lib/tempfile.py#L778-L848
 #
-# We had to remove the definition
-# __class_getitem__ = classmethod(_types.GenericAlias)
-# introduced in Python 3.9 because we do not use it and having a correct
-# implementation for Python 3.8 would be non-trivial. This definition can be
-# reintroduced if needed once we drop support for Python 3.8.
-#
 # The whole thing can be replaced by `from tempfile import TemporaryDirectory`
 # once Python fixes their implementation AND once we drop support for Python
-# 3.8 and Python 3.9.
+# Python 3.9.
 class TemporaryDirectory:
     """Create and return a temporary directory.  This has the same
     behavior as mkdtemp but can be used as a context manager.  For
     example:
 
         with TemporaryDirectory() as tmpdir:
             ...
```

### Comparing `pharmpy-core-0.93.2/src/pharmpy/internals/graph/directed/connected_components.py` & `pharmpy-core-0.94.0/src/pharmpy/internals/graph/directed/connected_components.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/internals/immutable.py` & `pharmpy-core-0.94.0/src/pharmpy/internals/immutable.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,10 +26,9 @@
 
     if kwargs or not isinstance(arg, MappingProxyType):
         return MappingProxyType(dict(arg, **kwargs))
 
     # NOTE MappingProxyType[K, V] is both a Mapping[K, V] and an Iterable[K].
     # Pyright tries to idenfiy Iterable[Tuple[K, V]] to an input of type
     # MappingProxyType[Tuple[K, V], Any] which is unfortunately not what we
-    # want. We also cannot cast to MappingProxyType[K, V] because Python 3.8
-    # does not define that.
+    # want.
     return cast(MappingProxyType, arg)
```

### Comparing `pharmpy-core-0.93.2/src/pharmpy/internals/math.py` & `pharmpy-core-0.94.0/src/pharmpy/internals/math.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/internals/module/lazy.py` & `pharmpy-core-0.94.0/src/pharmpy/internals/module/lazy.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/internals/parse/generic.py` & `pharmpy-core-0.94.0/src/pharmpy/internals/parse/generic.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/internals/parse/ignored.py` & `pharmpy-core-0.94.0/src/pharmpy/internals/parse/ignored.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/internals/parse/missing.py` & `pharmpy-core-0.94.0/src/pharmpy/internals/parse/missing.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/internals/parse/prettyprint.py` & `pharmpy-core-0.94.0/src/pharmpy/internals/parse/prettyprint.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/internals/parse/tree.py` & `pharmpy-core-0.94.0/src/pharmpy/internals/parse/tree.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/internals/parse/treeprint.py` & `pharmpy-core-0.94.0/src/pharmpy/internals/parse/treeprint.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/internals/sequence/lcs.py` & `pharmpy-core-0.94.0/src/pharmpy/internals/sequence/lcs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/internals/set/partitions.py` & `pharmpy-core-0.94.0/src/pharmpy/internals/set/partitions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/internals/set/subsets.py` & `pharmpy-core-0.94.0/src/pharmpy/internals/set/subsets.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/internals/unicode.py` & `pharmpy-core-0.94.0/src/pharmpy/internals/unicode.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/model/__init__.py` & `pharmpy-core-0.94.0/src/pharmpy/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/model/data.py` & `pharmpy-core-0.94.0/src/pharmpy/model/data.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/model/datainfo.py` & `pharmpy-core-0.94.0/src/pharmpy/model/datainfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """DataInfo is a companion to the dataset. It contains metadata of the dataset
 """
 from __future__ import annotations
 
 import json
 from collections.abc import Sequence
 from pathlib import Path
-from typing import Optional
-from typing import Sequence as TypingSequence
-from typing import Tuple, Union, cast, overload
+from typing import Optional, Tuple, Union, cast, overload
 
 from pharmpy.deps import pandas as pd
 from pharmpy.deps import sympy
 from pharmpy.internals.expr.units import parse as parse_units
 from pharmpy.internals.fs.path import path_absolute, path_relative_to
 from pharmpy.internals.immutable import Immutable
 
@@ -467,28 +465,28 @@
         Path to dataset file
     separator : str
         Character or regexp separator for dataset
     """
 
     def __init__(
         self,
-        columns: Optional[Union[TypingSequence[ColumnInfo], TypingSequence[str]]] = (),
+        columns: Optional[Union[Sequence[ColumnInfo], Sequence[str]]] = (),
         path: Optional[Union[str, Path]] = None,
         separator: str = ',',
         force_absolute_path: bool = True,
     ):
         self._columns = columns
         self._path = path
         self._separator = separator
         self._force_absolute_path = force_absolute_path
 
     @classmethod
     def create(
         cls,
-        columns: Optional[Union[TypingSequence[ColumnInfo], TypingSequence[str]]] = None,
+        columns: Optional[Union[Sequence[ColumnInfo], Sequence[str]]] = None,
         path: Optional[Union[str, Path]] = None,
         separator: str = ',',
         force_absolute_path: bool = True,
     ):
         if columns is None:
             columns: Tuple[ColumnInfo, ...] = ()
         elif len(columns) > 0 and isinstance(columns[0], str):
```

### Comparing `pharmpy-core-0.93.2/src/pharmpy/model/distributions/numeric.py` & `pharmpy-core-0.94.0/src/pharmpy/model/distributions/numeric.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/model/distributions/symbolic.py` & `pharmpy-core-0.94.0/src/pharmpy/model/distributions/symbolic.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/model/estimation.py` & `pharmpy-core-0.94.0/src/pharmpy/model/estimation.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/model/model.py` & `pharmpy-core-0.94.0/src/pharmpy/model/model.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/model/parameters.py` & `pharmpy-core-0.94.0/src/pharmpy/model/parameters.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/model/random_variables.py` & `pharmpy-core-0.94.0/src/pharmpy/model/random_variables.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/model/results.py` & `pharmpy-core-0.94.0/src/pharmpy/model/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/model/statements.py` & `pharmpy-core-0.94.0/src/pharmpy/model/statements.py`

 * *Files 2% similar despite different names*

```diff
@@ -416,35 +416,74 @@
         concentrations.add(A)
         name = names[A.func]
         comp = Compartment.create(name)
         cb.add_compartment(comp)
         compartments[name] = comp
 
     neweqs = list(eqs)  # Remaining flows
+
     for eq in eqs:
+        checked_terms = set()
         for comp_func in concentrations.intersection(free_images(eq.rhs)):
             dep = eq.rhs.as_independent(comp_func, as_Add=True)[1]
-            terms = sympy.Add.make_args(dep)
+            terms = sympy.Add.make_args(dep.expand())
             for term in terms:
-                if _is_positive(term):
-                    from_comp = compartments[names[comp_func.func]]
-                    to_comp = compartments[names[eq.lhs.args[0].func]]
-                    cb.add_flow(from_comp, to_comp, term / comp_func)
-                    for i, neweq in enumerate(neweqs):
-                        if neweq.lhs.args[0].name == eq.lhs.args[0].name:
-                            neweqs[i] = sympy.Eq(neweq.lhs, sympy.expand(neweq.rhs - term))
-                        elif neweq.lhs.args[0].name == comp_func.name:
-                            neweqs[i] = sympy.Eq(neweq.lhs, sympy.expand(neweq.rhs + term))
-
+                if term not in checked_terms:
+                    checked_terms.add(term)
+                    from_comp = None
+                    to_comp = None
+                    if len(concentrations.intersection(free_images(term))) >= 2:
+                        # This means second order absorption -> find matching term
+                        # to determine flow
+                        if _is_positive(term):
+                            for second_comp in concentrations.intersection(free_images(term)):
+                                for eq_2 in eqs:
+                                    if eq_2.lhs.args[0].name == second_comp.name:
+                                        if -term in sympy.Add.make_args(eq_2.rhs.expand()):
+                                            from_comp = compartments[names[second_comp.func]]
+                                            to_comp = compartments[names[eq.lhs.args[0].func]]
+                    else:
+                        # Find matching term to determine if flow is between
+                        # compartments or not
+                        if _is_positive(term):
+                            for eq_2 in eqs:
+                                if -term in sympy.Add.make_args(eq_2.rhs.expand()):
+                                    from_comp = compartments[names[eq_2.lhs.args[0].func]]
+                                    to_comp = compartments[names[eq.lhs.args[0].func]]
+
+                    if from_comp is not None and to_comp is not None:
+                        # FIXME : get current flow from builder instead?
+                        cs = CompartmentalSystem(cb)
+                        current_flow = cs.get_flow(from_comp, to_comp)
+
+                        if isinstance(current_flow, sympy.core.numbers.Zero):
+                            cb.add_flow(from_comp, to_comp, term / comp_func)
+                        else:
+                            new_flow = term / comp_func + current_flow
+                            cb.add_flow(from_comp, to_comp, new_flow)
+
+                        for i, neweq in enumerate(neweqs):
+                            if neweq.lhs.args[0].name == eq.lhs.args[0].name:
+                                neweqs[i] = sympy.Eq(neweq.lhs, sympy.expand(neweq.rhs - term))
+                            elif neweq.lhs.args[0].name == comp_func.name:
+                                neweqs[i] = sympy.Eq(neweq.lhs, sympy.expand(neweq.rhs + term))
     for eq in neweqs:
         if eq.rhs != 0:
+            i = sympy.Add(0)
+            o = sympy.Add(0)
+            for term in sympy.Add.make_args(eq.rhs):
+                if _is_positive(term):
+                    i = i + term
+                else:
+                    o = o + term
+
             comp_func = eq.lhs.args[0]
             from_comp = compartments[names[comp_func.func]]
-            cb.add_flow(from_comp, output, -eq.rhs / comp_func)
-
+            cb.add_flow(from_comp, output, -o / comp_func)
+            cb.set_input(from_comp, i)
     cs = CompartmentalSystem(cb)
     return cs
 
 
 class CompartmentalSystem(ODESystem):
     """System of ODEs descibed as a compartmental system
 
@@ -1026,23 +1065,28 @@
             a = list(x)
             if output in a:
                 a.remove(output)
             a = sorted(a, key=lambda x: x.name)
             return iter(a)
 
         nodes = list(nx.bfs_tree(self._g, dosecmt, sort_neighbors=sortfunc))
-
         remaining = set(self._g.nodes) - {output} - set(nodes)
-        if remaining:  # Disjoint graph
-            # Start with the one compartment having a zero order input (target for TMDD)
-            for comp in remaining:
-                if comp.input != 0:
-                    break
+        while remaining:  # Disjoint graph
+            comp = sorted(remaining, key=lambda x: x.name)[0]
+            # Start with a compartment having a zero order input
+            for c in remaining:
+                if comp is None and c.input != 0:
+                    comp = c
             ordered_remaining = list(nx.bfs_tree(self._g, comp, sort_neighbors=sortfunc))
-            nodes += ordered_remaining
+            cleaned_ordered_remaining = []
+            for c in ordered_remaining:
+                if c not in set(nodes):
+                    cleaned_ordered_remaining.append(c)
+            nodes += cleaned_ordered_remaining
+            remaining = set(self._g.nodes) - {output} - set(nodes)
         return nodes
 
     @property
     def zero_order_inputs(self):
         """Vector of all zero order inputs to each compartment
 
         Example
```

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/__init__.py` & `pharmpy-core-0.94.0/src/pharmpy/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/allometry.py` & `pharmpy-core-0.94.0/src/pharmpy/modeling/allometry.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/basic_models.py` & `pharmpy-core-0.94.0/src/pharmpy/modeling/basic_models.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/block_rvs.py` & `pharmpy-core-0.94.0/src/pharmpy/modeling/block_rvs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/blq.py` & `pharmpy-core-0.94.0/src/pharmpy/modeling/blq.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/common.py` & `pharmpy-core-0.94.0/src/pharmpy/modeling/common.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/compartments.py` & `pharmpy-core-0.94.0/src/pharmpy/modeling/compartments.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/covariate_effect.py` & `pharmpy-core-0.94.0/src/pharmpy/modeling/covariate_effect.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/data.py` & `pharmpy-core-0.94.0/src/pharmpy/modeling/data.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/error.py` & `pharmpy-core-0.94.0/src/pharmpy/modeling/error.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/estimation.py` & `pharmpy-core-0.94.0/src/pharmpy/modeling/estimation.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/estimation_steps.py` & `pharmpy-core-0.94.0/src/pharmpy/modeling/estimation_steps.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/eta_additions.py` & `pharmpy-core-0.94.0/src/pharmpy/modeling/eta_additions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/eta_transformations.py` & `pharmpy-core-0.94.0/src/pharmpy/modeling/eta_transformations.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/evaluation.py` & `pharmpy-core-0.94.0/src/pharmpy/modeling/evaluation.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/example_models/moxo.csv` & `pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/moxo.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/example_models/moxo.mod` & `pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/moxo.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/example_models/pheno.cov` & `pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/example_models/pheno.datainfo` & `pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/example_models/pheno.dta` & `pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/example_models/pheno.ext` & `pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/example_models/pheno.lst` & `pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/example_models/pheno.mod` & `pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/example_models/pheno.phi` & `pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/example_models/pheno.tab` & `pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno.tab`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/example_models/pheno_linear.dta` & `pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno_linear.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/example_models/pheno_linear.ext` & `pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno_linear.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/example_models/pheno_linear.lst` & `pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno_linear.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/example_models/pheno_linear.mod` & `pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno_linear.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/example_models/pheno_linear.phi` & `pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno_linear.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/expressions.py` & `pharmpy-core-0.94.0/src/pharmpy/modeling/expressions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/help_functions.py` & `pharmpy-core-0.94.0/src/pharmpy/modeling/help_functions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/iterators.py` & `pharmpy-core-0.94.0/src/pharmpy/modeling/iterators.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/lrt.py` & `pharmpy-core-0.94.0/src/pharmpy/modeling/lrt.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/math.py` & `pharmpy-core-0.94.0/src/pharmpy/modeling/math.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/metabolite.py` & `pharmpy-core-0.94.0/src/pharmpy/modeling/metabolite.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/odes.py` & `pharmpy-core-0.94.0/src/pharmpy/modeling/odes.py`

 * *Files 0% similar despite different names*

```diff
@@ -963,19 +963,19 @@
     lag_time = dose_comp.lag_time
     if depot:
         to_comp, _ = odes.get_compartment_outflows(depot)[0]
         ka = odes.get_flow(depot, odes.central_compartment)
         assert ka is not None
         cb = CompartmentalSystemBuilder(odes)
         cb.remove_compartment(depot)
-        cb.set_dose(to_comp, dose)
+        to_comp = cb.set_dose(to_comp, dose)
+        to_comp = cb.set_lag_time(to_comp, depot.lag_time)
+        cb.set_bioavailability(to_comp, depot.bioavailability)
         statements = statements.before_odes + CompartmentalSystem(cb) + statements.after_odes
         symbols = ka.free_symbols
-    else:
-        to_comp = dose_comp  #
 
     new_statements = statements.remove_symbol_definitions(symbols, statements.ode_system)
     mat_idx = statements.find_assignment_index('MAT')
     if mat_idx is not None:
         mat_assign = statements[mat_idx]
         new_statements = new_statements[0:mat_idx] + mat_assign + new_statements[mat_idx:]
```

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/parameter_sampling.py` & `pharmpy-core-0.94.0/src/pharmpy/modeling/parameter_sampling.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/parameters.py` & `pharmpy-core-0.94.0/src/pharmpy/modeling/parameters.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/plots.py` & `pharmpy-core-0.94.0/src/pharmpy/modeling/plots.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/remove_iiv.py` & `pharmpy-core-0.94.0/src/pharmpy/modeling/remove_iiv.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/remove_iov.py` & `pharmpy-core-0.94.0/src/pharmpy/modeling/remove_iov.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/results.py` & `pharmpy-core-0.94.0/src/pharmpy/modeling/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/tmdd.py` & `pharmpy-core-0.94.0/src/pharmpy/modeling/tmdd.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/units.py` & `pharmpy-core-0.94.0/src/pharmpy/modeling/units.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/update_inits.py` & `pharmpy-core-0.94.0/src/pharmpy/modeling/update_inits.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/modeling/write_csv.py` & `pharmpy-core-0.94.0/src/pharmpy/modeling/write_csv.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/fcon/model.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/fcon/model.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nlmixr/__init__.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nlmixr/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nlmixr/error_model.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nlmixr/error_model.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nlmixr/ini.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nlmixr/ini.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nlmixr/model.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nlmixr/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,21 +52,16 @@
         A model converted to nlmixr format.
 
     """
 
     if isinstance(model, Model):
         return model
 
-    if model.internals.control_stream.get_records("DES"):
-        des = model.internals.control_stream.get_records("DES")[0]
-    else:
-        des = None
-
     nlmixr_model = Model(
-        internals=NLMIXRModelInternals(DES=des),
+        internals=NLMIXRModelInternals(),
         parameters=model.parameters,
         random_variables=model.random_variables,
         statements=model.statements,
         dependent_variables=model.dependent_variables,
         estimation_steps=model.estimation_steps,
         filename_extension='.R',
         datainfo=model.datainfo,
@@ -277,15 +272,14 @@
     return temp_model
 
 
 @dataclass
 class NLMIXRModelInternals:
     src: Optional[str] = None
     path: Optional[Path] = None
-    DES: Optional = None
 
 
 class Model(pharmpy.model.Model):
     def __init__(self, **kwargs):
         super().__init__(
             **kwargs,
         )
```

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nlmixr/model_block.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nlmixr/model_block.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,22 +262,14 @@
         A pharmpy model object to add ODEs to.
     cg : CodeGenerator
         Codegenerator object holding the code to be added to.
     """
     amounts = [am.name for am in list(model.statements.ode_system.amounts)]
     printer = ExpressionPrinter(amounts)
 
-    des = model.internals.DES
-    statements = []
-    if des:
-        pattern = re.compile(r"DADT\(\d*\)")
-        for s in des.statements:
-            if not pattern.match(s.symbol.name):
-                statements.append(s)
-        add_statements(model, cg, statements)
     for eq in model.statements.ode_system.eqs:
         # Should remove piecewise from these equations in nlmixr
         if eq.atoms(sympy.Piecewise):
             lhs = remove_piecewise(printer.doprint(eq.lhs))
             rhs = remove_piecewise(printer.doprint(eq.rhs))
 
             cg.add(f'{lhs} = {rhs}')
```

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nlmixr/sanity_checks.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nlmixr/sanity_checks.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/__init__.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/advan.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/advan.py`

 * *Files 3% similar despite different names*

```diff
@@ -321,14 +321,41 @@
         odes = CompartmentalSystem(cb)
         return odes, ass, None
     else:
         return None
     return CompartmentalSystem(cb), ass, comp_map
 
 
+def des_assign_statements(
+    control_stream: NMTranControlStream,
+    des=None,
+):
+    if des:
+        rec_model = control_stream.get_records('MODEL')[0]
+
+        subs_dict, comp_names = {}, {}
+        comps = [c for c, _ in rec_model.compartments()]
+        func_to_name = {}
+        t = sympy.Symbol('t')
+        for i, c in enumerate(comps, 1):
+            a = sympy.Function(f'A_{c}')
+            subs_dict[f'DADT({i})'] = sympy.Derivative(a(t))
+            subs_dict[f'DADT ({i})'] = sympy.Derivative(a(t))
+            subs_dict[f'A({i})'] = str(a)
+            comp_names[f'A({i})'] = a
+            func_to_name[a] = c
+
+        sset = des.statements.subs(subs_dict)
+
+        statements = [sympy.Eq(s.symbol, s.expression) for s in sset if s.symbol.is_Symbol]
+        if len(statements) == 0:
+            statements = None
+        return statements
+
+
 def _f_link_assignment(control_stream: NMTranControlStream, compartment: Compartment, compno: int):
     f = sympy.Symbol('F')
     try:
         fexpr = compartment.amount
     except AttributeError:
         fexpr = compartment
     pkrec = control_stream.get_records('PK')[0]
```

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/config.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/config.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/dataset.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/dataset.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/model.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/model.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/nmtran_parser.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/nmtran_parser.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/parsing.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/parsing.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     Parameter,
     Parameters,
     RandomVariables,
     Statements,
 )
 from pharmpy.plugins.nonmem.table import NONMEMTableFile, PhiTable
 
-from .advan import _compartmental_model
+from .advan import _compartmental_model, des_assign_statements
 from .dataset import read_nonmem_dataset
 from .nmtran_parser import NMTranControlStream
 
 
 def parse_thetas(control_stream):
     names = []
     bounds = []
@@ -229,26 +229,37 @@
 
     des = control_stream.get_des_record()
     error = control_stream.get_error_record()
     comp_map = None
 
     if error:
         sub = control_stream.get_records('SUBROUTINES')[0]
+        des_assign = des_assign_statements(control_stream, des)
+        if des_assign is not None:
+            for s in des_assign:
+                statements += Assignment(s.lhs, s.rhs)
         comp = _compartmental_model(di, dataset, control_stream, sub.advan, sub.trans, des)
         trans_amounts = {}
         if comp is None:
             statements += ODESystem()
             # FIXME: Dummy link statement
             statements += Assignment(sympy.Symbol('F'), sympy.Symbol('F'))
         else:
             cm, link, comp_map = comp
             statements += [cm, link]
-            for i, amount in enumerate(cm.amounts, start=1):
-                trans_amounts[sympy.Symbol(f"A({i})")] = amount
-                trans_amounts[sympy.Symbol(f"A_0({i})")] = sympy.Function(amount.name)(0)
+            if des:
+                rec_model = control_stream.get_records('MODEL')[0]
+                comps = [c for c, _ in rec_model.compartments()]
+                for i, c in enumerate(comps, 1):
+                    trans_amounts[sympy.Symbol(f"A({i})")] = f'A_{c}'
+                    trans_amounts[sympy.Symbol(f"A_0({i})")] = sympy.Function(f'A_{c}')(0)
+            else:
+                for i, amount in enumerate(cm.amounts, start=1):
+                    trans_amounts[sympy.Symbol(f"A({i})")] = amount
+                    trans_amounts[sympy.Symbol(f"A_0({i})")] = sympy.Function(amount.name)(0)
         statements += error.statements
         if trans_amounts:
             statements = statements.subs(trans_amounts)
 
     return statements, comp_map
```

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/abbreviated_record.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/abbreviated_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/code_record.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/code_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/data_record.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/data_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/factory.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/factory.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/grammars/abbreviated_record.lark` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/grammars/abbreviated_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/grammars/code_record.lark` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/grammars/code_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/grammars/data_record.lark` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/grammars/data_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/grammars/omega_record.lark` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/grammars/omega_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/grammars/simulation_record.lark` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/grammars/simulation_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/grammars/theta_record.lark` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/grammars/theta_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/model_record.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/model_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/omega_record.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/omega_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/option_record.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/option_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/parsers.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/parsers.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/problem_record.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/problem_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/record.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/sizes_record.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/sizes_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/subroutine_record.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/subroutine_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/table_record.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/table_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/records/theta_record.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/theta_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/results.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/results_file.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/results_file.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/run.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/run.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/table.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/table.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/nonmem/update.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/update.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/rxode/__init__.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/rxode/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/rxode/model.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/rxode/model.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/plugins/utils.py` & `pharmpy-core-0.94.0/src/pharmpy/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/reporting/altairplot.py` & `pharmpy-core-0.94.0/src/pharmpy/reporting/altairplot.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/reporting/custom.css` & `pharmpy-core-0.94.0/src/pharmpy/reporting/custom.css`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/reporting/reporting.py` & `pharmpy-core-0.94.0/src/pharmpy/reporting/reporting.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/results.py` & `pharmpy-core-0.94.0/src/pharmpy/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/__init__.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/allometry/tool.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/allometry/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/amd/funcs.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/amd/funcs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/amd/run.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/amd/run.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/bootstrap/report.rst` & `pharmpy-core-0.94.0/src/pharmpy/tools/bootstrap/report.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/bootstrap/results.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/bootstrap/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/bootstrap/tool.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/bootstrap/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/cdd/results.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/cdd/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/common.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/common.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/covsearch/tool.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/covsearch/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/crossval/results.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/crossval/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/estmethod/algorithms.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/estmethod/algorithms.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/estmethod/report.rst` & `pharmpy-core-0.94.0/src/pharmpy/tools/estmethod/report.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/estmethod/tool.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/estmethod/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/evaldesign/tool.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/evaldesign/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/frem/models.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/frem/models.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/frem/results.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/frem/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/frem/tool.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/frem/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/funcs/ml.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/funcs/ml.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/funcs/ml_models/infinds.tflite` & `pharmpy-core-0.94.0/src/pharmpy/tools/funcs/ml_models/infinds.tflite`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/funcs/ml_models/outliers.tflite` & `pharmpy-core-0.94.0/src/pharmpy/tools/funcs/ml_models/outliers.tflite`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/funcs/summarize_individuals.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/funcs/summarize_individuals.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/iivsearch/algorithms.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/iivsearch/algorithms.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/iivsearch/tool.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/iivsearch/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/iovsearch/tool.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/iovsearch/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/linearize/results.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/linearize/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/linearize/tool.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/linearize/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/mfl/feature/absorption.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/mfl/feature/absorption.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/mfl/feature/covariate.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/mfl/feature/covariate.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/mfl/feature/elimination.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/mfl/feature/elimination.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/mfl/feature/peripherals.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/mfl/feature/peripherals.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/mfl/feature/transits.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/mfl/feature/transits.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/mfl/filter.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/mfl/filter.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/mfl/grammar.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/mfl/grammar.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/mfl/helpers.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/mfl/helpers.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/mfl/interpreter.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/mfl/interpreter.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/mfl/parse.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/mfl/parse.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/mfl/statement/definition.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/definition.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/mfl/statement/feature/absorption.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/feature/absorption.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/mfl/statement/feature/count_interpreter.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/feature/count_interpreter.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/mfl/statement/feature/covariate.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/feature/covariate.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/mfl/statement/feature/elimination.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/feature/elimination.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/mfl/statement/feature/transits.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/feature/transits.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/mfl/stringify.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/mfl/stringify.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/modelfit/__init__.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/modelfit/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/modelfit/results.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/modelfit/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/modelfit/tool.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/modelfit/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/modelsearch/algorithms.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/modelsearch/algorithms.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/modelsearch/tool.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/modelsearch/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/psn_helpers.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/psn_helpers.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/qa/results.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/qa/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/rankfuncs.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/rankfuncs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/run.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/run.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/ruvsearch/results.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/ruvsearch/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/ruvsearch/tool.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/ruvsearch/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/scm/psn_wrapper.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/scm/psn_wrapper.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/scm/results.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/scm/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/simeval/results.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/simeval/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/simfit/results.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/simfit/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/tools/wrap.py` & `pharmpy-core-0.94.0/src/pharmpy/tools/wrap.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/visualization.py` & `pharmpy-core-0.94.0/src/pharmpy/visualization.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/workflows/__init__.py` & `pharmpy-core-0.94.0/src/pharmpy/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/workflows/args.py` & `pharmpy-core-0.94.0/src/pharmpy/workflows/args.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/workflows/call.py` & `pharmpy-core-0.94.0/src/pharmpy/workflows/call.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/workflows/dispatchers/local_dask.py` & `pharmpy-core-0.94.0/src/pharmpy/workflows/dispatchers/local_dask.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/workflows/execute.py` & `pharmpy-core-0.94.0/src/pharmpy/workflows/execute.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/workflows/log.py` & `pharmpy-core-0.94.0/src/pharmpy/workflows/log.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/workflows/model_database/baseclass.py` & `pharmpy-core-0.94.0/src/pharmpy/workflows/model_database/baseclass.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/workflows/model_database/local_directory.py` & `pharmpy-core-0.94.0/src/pharmpy/workflows/model_database/local_directory.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/workflows/model_database/null_database.py` & `pharmpy-core-0.94.0/src/pharmpy/workflows/model_database/null_database.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/workflows/optimize.py` & `pharmpy-core-0.94.0/src/pharmpy/workflows/optimize.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/workflows/tool_database/baseclass.py` & `pharmpy-core-0.94.0/src/pharmpy/workflows/tool_database/baseclass.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/workflows/tool_database/local_directory.py` & `pharmpy-core-0.94.0/src/pharmpy/workflows/tool_database/local_directory.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/workflows/tool_database/null_database.py` & `pharmpy-core-0.94.0/src/pharmpy/workflows/tool_database/null_database.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy/workflows/workflow.py` & `pharmpy-core-0.94.0/src/pharmpy/workflows/workflow.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/src/pharmpy_core.egg-info/PKG-INFO` & `pharmpy-core-0.94.0/src/pharmpy_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pharmpy-core
-Version: 0.93.2
+Version: 0.94.0
 Summary: Pharmacometric modeling
 Home-page: https://pharmpy.github.io
 Author: Rikard Nordgren
 Author-email: rikard.nordgren@farmaci.uu.se
 License: GNU Lesser General Public License v3 (LGPLv3)
 Project-URL: Bug Tracker, https://github.com/pharmpy/pharmpy/issues
 Project-URL: Source Code, https://github.com/pharmpy/pharmpy
@@ -16,21 +16,20 @@
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Provides-Extra: nlmixr
 License-File: LICENSE
 License-File: LICENSE.LESSER
 License-File: AUTHORS.rst
 
 Pharmpy is a library and toolkit for pharmacometrics. It can be used as a regular Python package, in R
 via the `pharmr <https://github.com/pharmpy/pharmr>`_ package or via its built in command
@@ -41,14 +40,33 @@
 * A model abstraction as a foundation for higher level operations on models
 * Functions for manipulation of models, e.g. changing model components like elimination or absorption
 * Reading NONMEM models and results
 * Running models and complex workflows (with NONMEM or to some extent nlmixr)
 
 This is the `team behind Pharmpy <https://pharmpy.github.io/latest/contributors.html>`_
 
+0.94.0 (2023-04-26)
+-------------------
+
+New features
+============
+
+* Support parsing assignments other than DADT in $DES in NONMEM
+* Fix parsing of some complex ODE-systems in NONMEM
+
+Changes
+=======
+
+* Drop support for Python 3.8
+
+Bugfixes
+========
+
+* Fix bug causing BIC calculation to fail for models having first order absorption and lag_time after going into zero order absorption
+
 0.93.0 (2023-04-19)
 -------------------
 
 New features
 ============
 
 * Add function ``modeling.get_zero_order_inputs``
```

### Comparing `pharmpy-core-0.93.2/src/pharmpy_core.egg-info/SOURCES.txt` & `pharmpy-core-0.94.0/src/pharmpy_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/cli/test_cli.py` & `pharmpy-core-0.94.0/tests/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/conftest.py` & `pharmpy-core-0.94.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/integration/conftest.py` & `pharmpy-core-0.94.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/integration/test_allometry.py` & `pharmpy-core-0.94.0/tests/integration/test_allometry.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/integration/test_amd.py` & `pharmpy-core-0.94.0/tests/integration/test_amd.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/integration/test_bootstrap.py` & `pharmpy-core-0.94.0/tests/integration/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/integration/test_common.py` & `pharmpy-core-0.94.0/tests/integration/test_common.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/integration/test_covsearch.py` & `pharmpy-core-0.94.0/tests/integration/test_covsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/integration/test_estmethod.py` & `pharmpy-core-0.94.0/tests/integration/test_estmethod.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/integration/test_evaldesign.py` & `pharmpy-core-0.94.0/tests/integration/test_evaldesign.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/integration/test_fit.py` & `pharmpy-core-0.94.0/tests/integration/test_fit.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/integration/test_iivsearch.py` & `pharmpy-core-0.94.0/tests/integration/test_iivsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/integration/test_iovsearch.py` & `pharmpy-core-0.94.0/tests/integration/test_iovsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/integration/test_modelsearch.py` & `pharmpy-core-0.94.0/tests/integration/test_modelsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/integration/test_resume.py` & `pharmpy-core-0.94.0/tests/integration/test_resume.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/integration/test_ruvsearch.py` & `pharmpy-core-0.94.0/tests/integration/test_ruvsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/internals/fs/test_lock.py` & `pharmpy-core-0.94.0/tests/internals/fs/test_lock.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/internals/module/test_lazy.py` & `pharmpy-core-0.94.0/tests/internals/module/test_lazy.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/internals/test_math.py` & `pharmpy-core-0.94.0/tests/internals/test_math.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/internals/test_parse.py` & `pharmpy-core-0.94.0/tests/internals/test_parse.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/model/test_datainfo.py` & `pharmpy-core-0.94.0/tests/model/test_datainfo.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/model/test_estimation.py` & `pharmpy-core-0.94.0/tests/model/test_estimation.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/model/test_model.py` & `pharmpy-core-0.94.0/tests/model/test_model.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/model/test_parameter.py` & `pharmpy-core-0.94.0/tests/model/test_parameter.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/model/test_random_variables.py` & `pharmpy-core-0.94.0/tests/model/test_random_variables.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/model/test_statements.py` & `pharmpy-core-0.94.0/tests/model/test_statements.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/modeling/test_add_covariate_effect.py` & `pharmpy-core-0.94.0/tests/modeling/test_add_covariate_effect.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/modeling/test_allometry.py` & `pharmpy-core-0.94.0/tests/modeling/test_allometry.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/modeling/test_block_rvs.py` & `pharmpy-core-0.94.0/tests/modeling/test_block_rvs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/modeling/test_blq.py` & `pharmpy-core-0.94.0/tests/modeling/test_blq.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/modeling/test_common.py` & `pharmpy-core-0.94.0/tests/modeling/test_common.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/modeling/test_covariate_effect.py` & `pharmpy-core-0.94.0/tests/modeling/test_covariate_effect.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/modeling/test_data_funcs.py` & `pharmpy-core-0.94.0/tests/modeling/test_data_funcs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/modeling/test_distribution.py` & `pharmpy-core-0.94.0/tests/modeling/test_distribution.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/modeling/test_error.py` & `pharmpy-core-0.94.0/tests/modeling/test_error.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/modeling/test_estimation_steps.py` & `pharmpy-core-0.94.0/tests/modeling/test_estimation_steps.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/modeling/test_eta_additions.py` & `pharmpy-core-0.94.0/tests/modeling/test_eta_additions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/modeling/test_eta_transformations.py` & `pharmpy-core-0.94.0/tests/modeling/test_eta_transformations.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/modeling/test_evaluate.py` & `pharmpy-core-0.94.0/tests/modeling/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/modeling/test_expressions.py` & `pharmpy-core-0.94.0/tests/modeling/test_expressions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/modeling/test_has_covariate_effect.py` & `pharmpy-core-0.94.0/tests/modeling/test_has_covariate_effect.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/modeling/test_help_functions.py` & `pharmpy-core-0.94.0/tests/modeling/test_help_functions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/modeling/test_iterators.py` & `pharmpy-core-0.94.0/tests/modeling/test_iterators.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/modeling/test_lrt.py` & `pharmpy-core-0.94.0/tests/modeling/test_lrt.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/modeling/test_modeling.py` & `pharmpy-core-0.94.0/tests/modeling/test_modeling.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     add_iov,
     add_lag_time,
     add_peripheral_compartment,
     add_pk_iiv,
     create_joint_distribution,
     fix_parameters_to,
     get_initial_conditions,
+    get_lag_times,
     get_zero_order_inputs,
     has_first_order_elimination,
     has_linear_odes,
     has_linear_odes_with_real_eigenvalues,
     has_michaelis_menten_elimination,
     has_mixed_mm_fo_elimination,
     has_odes,
@@ -1414,14 +1415,22 @@
 $COVARIANCE UNCONDITIONAL
 $TABLE ID TIME DV AMT WGT APGR IPRED PRED RES TAD CWRES NPDE NOAPPEND
        NOPRINT ONEHEADER FILE=sdtab1
 '''
     assert model.model_code == correct
 
 
+def test_lagtime_then_zoabs(load_example_model_for_test):
+    model = load_example_model_for_test("pheno")
+    model = set_first_order_absorption(model)
+    model = add_lag_time(model)
+    model = set_zero_order_absorption(model)
+    assert get_lag_times(model) == {'CENTRAL': sympy.Symbol('ALAG1')}
+
+
 def test_seq_to_ZO(load_model_for_test, testdata):
     model = load_model_for_test(testdata / 'nonmem' / 'modeling' / 'pheno_advan2_seq.mod')
     model = set_zero_order_absorption(model)
     correct = '''$PROBLEM PHENOBARB SIMPLE MODEL
 $DATA pheno_zero_order.csv IGNORE=@
 $INPUT ID TIME AMT RATE WGT APGR DV FA1 FA2
 $SUBROUTINE ADVAN1 TRANS2
```

### Comparing `pharmpy-core-0.93.2/tests/modeling/test_parameter_sampling.py` & `pharmpy-core-0.94.0/tests/modeling/test_parameter_sampling.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/modeling/test_parameters.py` & `pharmpy-core-0.94.0/tests/modeling/test_parameters.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/modeling/test_plots.py` & `pharmpy-core-0.94.0/tests/modeling/test_plots.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/modeling/test_remove_covariate_effect.py` & `pharmpy-core-0.94.0/tests/modeling/test_remove_covariate_effect.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/modeling/test_results.py` & `pharmpy-core-0.94.0/tests/modeling/test_results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/nonmem/output/test_nonmem_results_file.py` & `pharmpy-core-0.94.0/tests/nonmem/output/test_nonmem_results_file.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/nonmem/records/test_abbreviated.py` & `pharmpy-core-0.94.0/tests/nonmem/records/test_abbreviated.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/nonmem/records/test_code.py` & `pharmpy-core-0.94.0/tests/nonmem/records/test_code.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/nonmem/records/test_data.py` & `pharmpy-core-0.94.0/tests/nonmem/records/test_data.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/nonmem/records/test_estimation_record.py` & `pharmpy-core-0.94.0/tests/nonmem/records/test_estimation_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/nonmem/records/test_factory.py` & `pharmpy-core-0.94.0/tests/nonmem/records/test_factory.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/nonmem/records/test_model_record.py` & `pharmpy-core-0.94.0/tests/nonmem/records/test_model_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/nonmem/records/test_omega.py` & `pharmpy-core-0.94.0/tests/nonmem/records/test_omega.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/nonmem/records/test_option_record.py` & `pharmpy-core-0.94.0/tests/nonmem/records/test_option_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/nonmem/records/test_problem.py` & `pharmpy-core-0.94.0/tests/nonmem/records/test_problem.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/nonmem/records/test_sizes.py` & `pharmpy-core-0.94.0/tests/nonmem/records/test_sizes.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/nonmem/records/test_theta.py` & `pharmpy-core-0.94.0/tests/nonmem/records/test_theta.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/nonmem/test_advan.py` & `pharmpy-core-0.94.0/tests/nonmem/test_advan.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/nonmem/test_des.py` & `pharmpy-core-0.94.0/tests/nonmem/test_des.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/nonmem/test_input.py` & `pharmpy-core-0.94.0/tests/nonmem/test_input.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/nonmem/test_modelfit_results.py` & `pharmpy-core-0.94.0/tests/nonmem/test_modelfit_results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/nonmem/test_nonmem_model.py` & `pharmpy-core-0.94.0/tests/nonmem/test_nonmem_model.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/nonmem/test_nonmem_table.py` & `pharmpy-core-0.94.0/tests/nonmem/test_nonmem_table.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/nonmem/test_parser.py` & `pharmpy-core-0.94.0/tests/nonmem/test_parser.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/nonmem/test_read.py` & `pharmpy-core-0.94.0/tests/nonmem/test_read.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/frem/results.json` & `pharmpy-core-0.94.0/tests/testdata/frem/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/DDMODEL00000130` & `pharmpy-core-0.94.0/tests/testdata/nonmem/DDMODEL00000130`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/Simulated_CMS_colistin_PK_data.csv` & `pharmpy-core-0.94.0/tests/testdata/nonmem/Simulated_CMS_colistin_PK_data.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real.cov` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real.phi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.cov` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.cov` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.cov` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.cov` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.cov` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.cov` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.cov` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.cov` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.cov` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.cov` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_1.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_10.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_10.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_2.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_3.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_4.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_5.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_5.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_6.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_6.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_7.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_7.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_8.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_8.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_9.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_9.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/cdd/pheno_real_bin10/meta.yaml` & `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/errors/control_stream_error.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/errors/control_stream_error.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/errors/est_step_warning.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/errors/est_step_warning.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/errors/estimate_near_boundary_warning.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/errors/estimate_near_boundary_warning.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/errors/no_header_error.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/errors/no_header_error.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/errors/no_header_error.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/errors/no_header_error.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/errors/rounding_error.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/errors/rounding_error.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/errors/run_interrupted.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/errors/run_interrupted.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/errors/zero_gradient_error.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/errors/zero_gradient_error.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/fcon/FCON` & `pharmpy-core-0.94.0/tests/testdata/nonmem/fcon/FCON`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/fcon/FDATA` & `pharmpy-core-0.94.0/tests/testdata/nonmem/fcon/FDATA`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno/frem_dataset.dta` & `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/frem_dataset.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno/model_3.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno/model_3.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno/model_3.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno/model_3.phi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno/model_3_input.phi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_3_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno/model_4.cov` & `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_4.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno/model_4.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno/model_4.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno/model_4.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno/model_4.phi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_4.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno/model_4_input.phi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_4_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno_cat/frem_dataset.dta` & `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno_cat/frem_dataset.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno_cat/model_4.cor` & `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno_cat/model_4.cov` & `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno_cat/model_4.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno_cat/model_4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno_cat/model_4.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno_cat/model_4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno_cat/model_4.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno_cat/model_4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno_cat/model_4.phi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno_cat/model_4.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/frem/pheno_cat/model_4_input.phi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno_cat/model_4_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.phi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.phi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.coi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.coi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/anneal2_V7_30_beta.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/anneal2_V7_30_beta.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.dta` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.phi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/superid2_6_V7_30_beta.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/superid2_6_V7_30_beta.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.cov` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.phi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/UseCase7.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/UseCase7.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/example6b_V7_30_beta.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/example6b_V7_30_beta.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/hessian_error.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/hessian_error.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/large_s_matrix_cov_fail.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/large_s_matrix_cov_fail.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.cov` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.phi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_fail_nonp.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_fail_nonp.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_nocov_nonp.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_nocov_nonp.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/nm710_fail_negV.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/nm710_fail_negV.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.dta` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.phi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno_nonp.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno_nonp.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/phenocorr.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/phenocorr.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/sparse_matrix_with_msfi.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/sparse_matrix_with_msfi.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_nonp.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_nonp.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_withcov.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_withcov.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/warfarin_ddmore.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/warfarin_ddmore.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.res` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.res`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/simfit/sim-1.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/simfit/sim-1.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/simfit/sim-1.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modelfit_results/simfit/sim-1.phi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modeling/pheno_1transit.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_1transit.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modeling/pheno_2transits.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_2transits.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modeling/pheno_advan1.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modeling/pheno_advan11.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan11.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modeling/pheno_advan12.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan12.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modeling/pheno_advan1_zero_order.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan1_zero_order.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modeling/pheno_advan2.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modeling/pheno_advan2_seq.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan2_seq.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modeling/pheno_advan3.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modeling/pheno_advan4.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modeling/pheno_advan5_depot.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan5_depot.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modeling/pheno_advan5_nodepot.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan5_nodepot.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modeling/pheno_zero_order.csv` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_zero_order.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/modeling/transit_indirect_reabsorption.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/transit_indirect_reabsorption.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/fviii6.datainfo` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/fviii6.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/fviii6.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/fviii6.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/mox1.cov` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox1.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/mox1.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/mox1.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/mox1.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/mox1.phi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/mox2.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/mox2.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/mox2.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/mox2.phi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/mox_2comp.cov` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox_2comp.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/mox_2comp.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox_2comp.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/mox_2comp.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox_2comp.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/mox_2comp.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox_2comp.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/mox_2comp.phi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox_2comp.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/mox_simulated_log.csv` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox_simulated_log.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/mox_simulated_normal.csv` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox_simulated_normal.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/mox_simulated_normal.datainfo` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox_simulated_normal.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/moxo_simulated_amd.csv` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/moxo_simulated_amd.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/moxo_simulated_amd.datainfo` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/moxo_simulated_amd.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/mytab_mox2` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mytab_mox2`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/pef.csv` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/pef.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/pheno_advan3_trans1.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_advan3_trans1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/pheno_advan3_trans1.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_advan3_trans1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/pheno_advan3_trans1.phi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_advan3_trans1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/pheno_dvid.csv` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_dvid.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/pheno_dvid.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_dvid.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/pheno_noifs.coi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_noifs.coi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/pheno_noifs.cor` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_noifs.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/pheno_noifs.cov` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_noifs.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/pheno_noifs.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_noifs.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/pheno_noifs.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_noifs.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/pheno_noifs.phi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_noifs.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/pheno_trans1.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_trans1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/pheno_trans1.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_trans1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/models/pheno_trans1.phi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_trans1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/pheno.datainfo` & `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/pheno.dta` & `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/pheno.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/pheno.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/pheno.phi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_block.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_block.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_etas.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_etas.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_multivariate_piecewise.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_multivariate_piecewise.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_no_obs_1stID.dta` & `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_no_obs_1stID.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_rate.dta` & `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_rate.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_real.coi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.coi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_real.cor` & `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_real.cov` & `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_real.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_real.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_real.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_real.phi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_real.tab` & `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.tab`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_real.xml` & `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.xml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_real_linbase.dta` & `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real_linbase.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_real_linbase.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real_linbase.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_real_linbase.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real_linbase.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_real_linbase.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real_linbase.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_real_linbase.phi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real_linbase.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/pheno_real_linbase.tab` & `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real_linbase.tab`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/qa/add_etas_linbase.dta` & `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/add_etas_linbase.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/qa/add_etas_linbase.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/add_etas_linbase.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/qa/add_etas_linbase.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/add_etas_linbase.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/qa/add_etas_linbase.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/add_etas_linbase.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/qa/boxcox.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/boxcox.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/qa/boxcox.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/boxcox.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/qa/boxcox.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/boxcox.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/qa/boxcox.phi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/boxcox.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/qa/cdd_results.json` & `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/cdd_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/qa/fullblock.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/fullblock.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/qa/fullblock.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/fullblock.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/qa/fullblock.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/fullblock.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/qa/fullblock.phi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/fullblock.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/qa/iov.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/iov.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/qa/iov.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/iov.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/qa/iov.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/iov.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/qa/iov.phi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/iov.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/qa/pheno_linbase.dta` & `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/pheno_linbase.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/qa/pheno_linbase.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/pheno_linbase.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/qa/pheno_linbase.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/pheno_linbase.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/qa/pheno_linbase.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/pheno_linbase.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/qa/pheno_linbase.phi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/pheno_linbase.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/qa/resmod_results.json` & `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/resmod_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/qa/scm_results.json` & `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/scm_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/qa/simeval_results.json` & `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/simeval_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/qa/tdist.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/tdist.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/qa/tdist.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/tdist.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/qa/tdist.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/tdist.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/qa/tdist.phi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/tdist.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/ruvsearch/mox3.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/ruvsearch/mox3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/ruvsearch/mox3.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/ruvsearch/mox3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/ruvsearch/mox3.mod` & `pharmpy-core-0.94.0/tests/testdata/nonmem/ruvsearch/mox3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/ruvsearch/mox3.phi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/ruvsearch/mox3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/ruvsearch/moxo_simulated_resmod.csv` & `pharmpy-core-0.94.0/tests/testdata/nonmem/ruvsearch/moxo_simulated_resmod.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/ruvsearch/mytab` & `pharmpy-core-0.94.0/tests/testdata/nonmem/ruvsearch/mytab`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/scm/backward_dir1/meta.yaml` & `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/backward_dir1/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/scm/backward_dir1/scmlog.txt` & `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/backward_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/scm/gofofv_dir1/scmlog.txt` & `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/gofofv_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/scm/localmin.logf` & `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/localmin.logf`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/scm/log_steps/backward_ofv_1.txt` & `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/log_steps/backward_ofv_1.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/scm/log_steps/forward_ofv_1.txt` & `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/log_steps/forward_ofv_1.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/scm/log_steps/forward_pval_1.txt` & `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/log_steps/forward_pval_1.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/scm/log_steps/forward_pval_2.txt` & `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/log_steps/forward_pval_2.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/scm/log_steps/forward_pval_3.txt` & `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/log_steps/forward_pval_3.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/scm/mergeofv_dir1/meta.yaml` & `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/mergeofv_dir1/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/scm/mergeofv_dir1/scmlog.txt` & `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/mergeofv_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/scm/mergeofv_dir2/meta.yaml` & `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/mergeofv_dir2/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/scm/mergeofv_dir2/scmlog.txt` & `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/mergeofv_dir2/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/scm/meta.yaml` & `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/scm/onlyforward_dir1/meta.yaml` & `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/onlyforward_dir1/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/scm/onlyforward_dir1/scmlog.txt` & `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/onlyforward_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/scm/scm_dir1/scmlog.txt` & `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/scm_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/scm/scmplus_dir1/scmlog.txt` & `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/scmplus_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/sdtab1` & `pharmpy-core-0.94.0/tests/testdata/nonmem/sdtab1`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/secondary_parameters/pheno.cov` & `pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/pheno.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/secondary_parameters/pheno.dta` & `pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/pheno.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/secondary_parameters/pheno.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/pheno.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/secondary_parameters/pheno.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/pheno.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/secondary_parameters/pheno.phi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/pheno.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/secondary_parameters/run1.cov` & `pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run1.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/secondary_parameters/run1.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/secondary_parameters/run1.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/secondary_parameters/run1.phi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/secondary_parameters/run2.cov` & `pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run2.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/secondary_parameters/run2.ext` & `pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/secondary_parameters/run2.lst` & `pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/nonmem/secondary_parameters/run2.phi` & `pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/pheno_data.csv` & `pharmpy-core-0.94.0/tests/testdata/pheno_data.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/est_data0.dta` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/est_data0.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/est_data1.dta` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/est_data1.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/est_data2.dta` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/est_data2.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/est_data3.dta` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/est_data3.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model0.cor` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model0.cov` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model0.ext` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model0.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model0.lst` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model0.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model0.phi` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model0.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model1.cor` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model1.cov` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model1.ext` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model1.lst` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model1.phi` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model2.cor` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model2.cov` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model2.ext` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model2.lst` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model2.phi` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model3.cor` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model3.cov` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model3.ext` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model3.lst` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/est_model3.phi` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/pred_model0.ext` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/pred_model0.lst` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/pred_model0.phi` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/pred_model1.ext` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/pred_model1.lst` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/pred_model1.phi` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/pred_model2.ext` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/pred_model2.lst` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/pred_model2.phi` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/pred_model3.cor` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/pred_model3.cov` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/pred_model3.ext` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/pred_model3.lst` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/m1/pred_model3.phi` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/meta.yaml` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/pred_data0.dta` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/pred_data0.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/pred_data1.dta` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/pred_data1.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/pred_data2.dta` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/pred_data2.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/pred_data3.dta` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/pred_data3.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/crossval_dir1/version_and_option_info.txt` & `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/version_and_option_info.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/final_models/model_4.ext` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/final_models/model_4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/final_models/model_4.lst` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/final_models/model_4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/final_models/model_4.mod` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/final_models/model_4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/final_models/model_4.phi` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/final_models/model_4.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/final_models/model_4_input.phi` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/final_models/model_4_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/frem_dataset.dta` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/frem_dataset.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/frem_results.csv` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/frem_results.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/filter_data_model.ext` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/filter_data_model.lst` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/filter_data_model.mod` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/filter_data_model.phi` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/filtered_plus_type0.dta` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/filtered_plus_type0.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_1.cov` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_1.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_1.ext` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_1.lst` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_1.phi` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_1b.phi` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_1b.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_2.cor` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_2.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_2.cov` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_2.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_2.ext` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_2.lst` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_2.mod` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_2.phi` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_2_input.phi` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_2_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_3.ext` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_3.lst` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_3.mod` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_3.phi` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_3_input.phi` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_3b.ext` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3b.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_3b.lst` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3b.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_3b.mod` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3b.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_3b.phi` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3b.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/m1/model_3b_input.phi` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3b_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/meta.yaml` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/proposal_density.cov` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/proposal_density.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/frem_dir1/version_and_option_info.txt` & `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/version_and_option_info.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/qa_dir1/linearize_run/results.json` & `pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/linearize_run/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.ext` & `pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.lst` & `pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.mod` & `pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.phi` & `pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/extra_table` & `pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/extra_table`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/qa_dir1/pheno_real_linbase.dta` & `pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/qa_dir1/pheno_real_linbase.ext` & `pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/qa_dir1/pheno_real_linbase.lst` & `pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/qa_dir1/pheno_real_linbase.mod` & `pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/qa_dir1/pheno_real_linbase.phi` & `pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/qa_dir1/results_summary.yaml` & `pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/results_summary.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/resmod_dir1/resmod_results.csv` & `pharmpy-core-0.94.0/tests/testdata/psn/resmod_dir1/resmod_results.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/resmod_dir2/resmod_results.csv` & `pharmpy-core-0.94.0/tests/testdata/psn/resmod_dir2/resmod_results.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/orig_pred.dta` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/orig_pred.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/original.cor` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/original.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/original.cov` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/original.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/original.ext` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/original.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/original.mod` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/original.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/original.phi` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/original.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/original_res_table.dta` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/original_res_table.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/pheno.dta` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/pheno.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-1.ext` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-1.lst` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-1.phi` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-2.ext` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-2.lst` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-2.phi` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-3.ext` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-3.lst` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-3.phi` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-4.ext` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-4.lst` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-4.phi` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-4.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-5.ext` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-5.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-5.lst` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-5.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-5.phi` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-5.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-6.ext` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-6.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-6.lst` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-6.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-6.phi` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-6.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-7.ext` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-7.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-7.lst` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-7.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-7.phi` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-7.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-8.ext` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-8.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-8.lst` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-8.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim-8.phi` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-8.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim_res_table-1.dta` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-1.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim_res_table-2.dta` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-2.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim_res_table-3.dta` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-3.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim_res_table-4.dta` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-4.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim_res_table-5.dta` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-5.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim_res_table-6.dta` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-6.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim_res_table-7.dta` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-7.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/m1/sim_res_table-8.dta` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-8.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/psn/simeval_dir1/summary_cwres.csv` & `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/summary_cwres.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/allometry_results.json` & `pharmpy-core-0.94.0/tests/testdata/results/allometry_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/amd_results.json` & `pharmpy-core-0.94.0/tests/testdata/results/amd_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/bootstrap_results.json` & `pharmpy-core-0.94.0/tests/testdata/results/bootstrap_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/cdd_results.json` & `pharmpy-core-0.94.0/tests/testdata/results/cdd_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/covsearch_results.json` & `pharmpy-core-0.94.0/tests/testdata/results/covsearch_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/estmethod_results.json` & `pharmpy-core-0.94.0/tests/testdata/results/estmethod_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/iivsearch_results.json` & `pharmpy-core-0.94.0/tests/testdata/results/iivsearch_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/iovsearch_results.json` & `pharmpy-core-0.94.0/tests/testdata/results/iovsearch_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/linearize_results.json` & `pharmpy-core-0.94.0/tests/testdata/results/linearize_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/metadata.json` & `pharmpy-core-0.94.0/tests/testdata/results/metadata.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/modelsearch_results.json` & `pharmpy-core-0.94.0/tests/testdata/results/modelsearch_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/qa_results.json` & `pharmpy-core-0.94.0/tests/testdata/results/qa_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/ruvsearch_results.json` & `pharmpy-core-0.94.0/tests/testdata/results/ruvsearch_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/metadata.json` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/metadata.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.csv` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.datainfo` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/results.json` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/input_model/input_model.mod` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/input_model.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/results.json` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.ext` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.lst` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.mod` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.phi` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/mytab_mox1` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/mytab_mox1`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stdout` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stdout`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/results.json` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.ext` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.lst` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.mod` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.phi` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/mytab_mox2` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/mytab_mox2`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stdout` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stdout`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/results.json` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.ext` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.lst` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.mod` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.phi` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/mytab_mox3` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/mytab_mox3`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stdout` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stdout`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/results.json` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.ext` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.lst` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.mod` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.phi` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/mytab_mox4` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/mytab_mox4`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stdout` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stdout`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/results.csv` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/results.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/testdata/results/tool_databases/modelsearch/results.json` & `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/tools/test_allometry.py` & `pharmpy-core-0.94.0/tests/tools/test_allometry.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/tools/test_amd.py` & `pharmpy-core-0.94.0/tests/tools/test_amd.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/tools/test_bootstrap.py` & `pharmpy-core-0.94.0/tests/tools/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/tools/test_cdd.py` & `pharmpy-core-0.94.0/tests/tools/test_cdd.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/tools/test_covsearch.py` & `pharmpy-core-0.94.0/tests/tools/test_covsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/tools/test_estmethod.py` & `pharmpy-core-0.94.0/tests/tools/test_estmethod.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/tools/test_exports.py` & `pharmpy-core-0.94.0/tests/tools/test_exports.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/tools/test_frem.py` & `pharmpy-core-0.94.0/tests/tools/test_frem.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/tools/test_iivsearch.py` & `pharmpy-core-0.94.0/tests/tools/test_iivsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/tools/test_iovsearch.py` & `pharmpy-core-0.94.0/tests/tools/test_iovsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/tools/test_linearize.py` & `pharmpy-core-0.94.0/tests/tools/test_linearize.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/tools/test_mfl.py` & `pharmpy-core-0.94.0/tests/tools/test_mfl.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/tools/test_ml.py` & `pharmpy-core-0.94.0/tests/tools/test_ml.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/tools/test_modelfit.py` & `pharmpy-core-0.94.0/tests/tools/test_modelfit.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/tools/test_modelsearch.py` & `pharmpy-core-0.94.0/tests/tools/test_modelsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/tools/test_qa.py` & `pharmpy-core-0.94.0/tests/tools/test_qa.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/tools/test_rankfuncs.py` & `pharmpy-core-0.94.0/tests/tools/test_rankfuncs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/tools/test_run.py` & `pharmpy-core-0.94.0/tests/tools/test_run.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/tools/test_runtool.py` & `pharmpy-core-0.94.0/tests/tools/test_runtool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/tools/test_ruvsearch.py` & `pharmpy-core-0.94.0/tests/tools/test_ruvsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/tools/test_scm.py` & `pharmpy-core-0.94.0/tests/tools/test_scm.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/tools/test_start_model.py` & `pharmpy-core-0.94.0/tests/tools/test_start_model.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/tools/test_summarize_individuals.py` & `pharmpy-core-0.94.0/tests/tools/test_summarize_individuals.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/tools/test_wrap.py` & `pharmpy-core-0.94.0/tests/tools/test_wrap.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/workflows/test_call.py` & `pharmpy-core-0.94.0/tests/workflows/test_call.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/workflows/test_execute.py` & `pharmpy-core-0.94.0/tests/workflows/test_execute.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/workflows/test_model_database.py` & `pharmpy-core-0.94.0/tests/workflows/test_model_database.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tests/workflows/test_workflow.py` & `pharmpy-core-0.94.0/tests/workflows/test_workflow.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.93.2/tox.ini` & `pharmpy-core-0.94.0/tox.ini`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ; a generative tox configuration, see: https://tox.readthedocs.io/en/latest/config.html#generative-envlist
 ;
 [tox]
 skip_missing_interpreters=True
 envlist =
-    {py38-,py39-,py310-,py311-,}{doctest,unit,integration}{-cover,}
-    {py38-,py39-,py310-,py311-,}{lint,format,report,docs-build,docs-test,docs-lint},
+    {py39-,py310-,py311-,}{doctest,unit,integration}{-cover,}
+    {py39-,py310-,py311-,}{lint,format,report,docs-build,docs-test,docs-lint},
     clean,
     spell,
     licenses,
     plain
 
 [testenv]
 skip_install = true
@@ -41,50 +41,50 @@
     debug: pdbpp
 
 [flags]
 cover = --cov --cov-report=term-missing --cov-report=term:skip-covered --cov-report xml:.coverage.xml
 profile = --profile-svg
 debug = --pdb
 
-[testenv:{py38,py39,py310,py311,py38-unit,py39-unit,py310-unit,py311-unit,unit}{-cover,}{-profile,}{-debug,}]
+[testenv:{py39,py310,py311,py39-unit,py310-unit,py311-unit,unit}{-cover,}{-profile,}{-debug,}]
 skip_install = false
 deps =
     -rrequirements.txt
     {[base]deps}
 commands = pytest -n auto -vv \
     profile: {[flags]profile} \
     cover: {[flags]cover} \
     debug: {[flags]debug} \
     {posargs:tests}
 
-[testenv:{py38-,py39-,py310-,py311-,}doctest{-cover,}]
+[testenv:{py39-,py310-,py311-,}doctest{-cover,}]
 skip_install = false
 deps =
     -rrequirements.txt
     {[base]deps}
 commands = pytest -W ignore::UserWarning -n auto -vv \
     profile: {[flags]profile} \
     cover: {[flags]cover} \
     debug: {[flags]debug} \
     --doctest-modules {posargs:src}
 
-[testenv:{py38-,py39-,py310-,py311-,}integration{-cover,}{-profile,}{-debug,}]
+[testenv:{py39-,py310-,py311-,}integration{-cover,}{-profile,}{-debug,}]
 skip_install = false
 deps =
     -rrequirements.txt
     {[base]deps}
 setenv =
     PHARMPYNOCONFIGFILE=0
 commands = pytest -vv \
     profile: {[flags]profile} \
     cover: {[flags]cover} \
     debug: {[flags]debug} \
     {posargs:tests/integration}
 
-[testenv:{py38-,py39-,py310-,py311-,}plain]
+[testenv:{py39-,py310-,py311-,}plain]
 setenv =
     PHARMPYNOCONFIGFILE=0
 skip_install = false
 deps =
     -rrequirements.txt
 commands = {posargs}
 
@@ -95,29 +95,29 @@
 commands =
     sphinx-build -j auto -b spelling docs dist/docs
 deps =
     -r{toxinidir}/docs/requirements.txt
     sphinxcontrib-spelling
     pyenchant
 
-[testenv:{py38-,py39-,py310-,py311-,}docs-{build,test}]
+[testenv:{py39-,py310-,py311-,}docs-{build,test}]
 skip_install = false
 deps =
     -rrequirements.txt
     -r{toxinidir}/docs/requirements.txt
 commands =
     pip install ipykernel==5.5.5  # Unable to build docs with newer version
     pip install sphinx>=5.1.1
     pip install sphinx-tabs>=3.4.1
     build: rm -rf docs/api
     build: sphinx-build {posargs:-E} -j auto -b html docs dist/docs
     build: sphinx-build -j auto -b linkcheck docs dist/docs
     test: sphinx-build {posargs:-E} -j auto -b doctest docs dist/docs
 
-[testenv:{py38-,py39-,py310-,py311-,}{lint,format}]
+[testenv:{py39-,py310-,py311-,}{lint,format}]
 deps =
     docutils
     check-manifest >= 0.45
     flake8
     readme-renderer
     pygments
     isort >= 5.0.0
@@ -133,23 +133,23 @@
     src tests setup.py
     flake8 src tests setup.py
     isort \
     lint: --check --diff \
     src tests setup.py
     bash scripts/lint_deps_imports.sh
 
-[testenv:{py38-,py39-,py310-,py311-,}{type-check}]
+[testenv:{py39-,py310-,py311-,}{type-check}]
 deps =
     -rrequirements.txt
     pytest>5.3.5
     pyright
 commands =
     pyright {posargs:src/pharmpy}
 
-[testenv:{py38-,py39-,py310-,py311-,}report]
+[testenv:{py39-,py310-,py311-,}report]
 deps = coverage
 commands =
     coverage report
     coverage html
 
 [testenv:clean]
 commands = coverage erase
@@ -159,14 +159,14 @@
 skip_install = false
 deps =
     -rrequirements.txt
     pip-licenses
 commands =
     pip-licenses
 
-[testenv:{py38-,py39-,py310-,py311-,}docs-lint]
+[testenv:{py39-,py310-,py311-,}docs-lint]
 skip_install = false
 deps =
     darglint
 commands =
     darglint --docstring-style numpy -z long src/pharmpy/modeling
     python scripts/lint_type_hints.py
```

