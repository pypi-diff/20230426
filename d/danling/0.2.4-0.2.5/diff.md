# Comparing `tmp/danling-0.2.4.tar.gz` & `tmp/danling-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danling-0.2.4.tar", last modified: Sat Apr 15 07:40:42 2023, max compression
+gzip compressed data, was "danling-0.2.5.tar", last modified: Wed Apr 26 10:03:19 2023, max compression
```

## Comparing `danling-0.2.4.tar` & `danling-0.2.5.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.167348 danling-0.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.147348 danling-0.2.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-15 07:40:36.000000 danling-0.2.4/.github/merge_rules.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.147348 danling-0.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-15 07:40:36.000000 danling-0.2.4/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-15 07:40:36.000000 danling-0.2.4/.github/workflows/push.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-04-15 07:40:36.000000 danling-0.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-15 07:40:36.000000 danling-0.2.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.151348 danling-0.2.4/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-15 07:40:36.000000 danling-0.2.4/LICENSES/LICENSE.Apache2
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-15 07:40:36.000000 danling-0.2.4/LICENSES/LICENSE.BSD2
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-15 07:40:36.000000 danling-0.2.4/LICENSES/LICENSE.BSD3
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-15 07:40:36.000000 danling-0.2.4/LICENSES/LICENSE.BSD4
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-15 07:40:36.000000 danling-0.2.4/LICENSES/LICENSE.GPL2
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-15 07:40:36.000000 danling-0.2.4/LICENSES/LICENSE.GPL3
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-15 07:40:36.000000 danling-0.2.4/LICENSES/LICENSE.MIT
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-15 07:40:36.000000 danling-0.2.4/LICENSES/LICENSE.Unlicense
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-15 07:40:42.167348 danling-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-15 07:40:36.000000 danling-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-15 07:40:36.000000 danling-0.2.4/anaconda-project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.151348 danling-0.2.4/danling/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-15 07:40:36.000000 danling-0.2.4/danling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-15 07:40:41.000000 danling-0.2.4/danling/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.151348 danling-0.2.4/danling/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-15 07:40:36.000000 danling-0.2.4/danling/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-15 07:40:36.000000 danling-0.2.4/danling/metrics/average_meter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-15 07:40:36.000000 danling-0.2.4/danling/metrics/average_meters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.151348 danling-0.2.4/danling/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-15 07:40:36.000000 danling-0.2.4/danling/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.151348 danling-0.2.4/danling/modules/mlp/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-15 07:40:36.000000 danling-0.2.4/danling/modules/mlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-15 07:40:36.000000 danling-0.2.4/danling/modules/mlp/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-15 07:40:36.000000 danling-0.2.4/danling/modules/mlp/mlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.151348 danling-0.2.4/danling/modules/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-15 07:40:36.000000 danling-0.2.4/danling/modules/transformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.151348 danling-0.2.4/danling/modules/transformer/attention/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-15 07:40:36.000000 danling-0.2.4/danling/modules/transformer/attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-04-15 07:40:36.000000 danling-0.2.4/danling/modules/transformer/attention/multihead_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-04-15 07:40:36.000000 danling-0.2.4/danling/modules/transformer/attention/simple_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-04-15 07:40:36.000000 danling-0.2.4/danling/modules/transformer/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-04-15 07:40:36.000000 danling-0.2.4/danling/modules/transformer/encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.151348 danling-0.2.4/danling/modules/transformer/ffn/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-15 07:40:36.000000 danling-0.2.4/danling/modules/transformer/ffn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-15 07:40:36.000000 danling-0.2.4/danling/modules/transformer/ffn/fcn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.151348 danling-0.2.4/danling/modules/transformer/pos_embed/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-15 07:40:36.000000 danling-0.2.4/danling/modules/transformer/pos_embed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-04-15 07:40:36.000000 danling-0.2.4/danling/modules/transformer/pos_embed/pos_embed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.151348 danling-0.2.4/danling/optim/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-15 07:40:36.000000 danling-0.2.4/danling/optim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.151348 danling-0.2.4/danling/optim/lr_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-15 07:40:36.000000 danling-0.2.4/danling/optim/lr_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-04-15 07:40:36.000000 danling-0.2.4/danling/optim/lr_scheduler/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-04-15 07:40:36.000000 danling-0.2.4/danling/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.151348 danling-0.2.4/danling/runner/
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-04-15 07:40:36.000000 danling-0.2.4/danling/runner/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-15 07:40:36.000000 danling-0.2.4/danling/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-04-15 07:40:36.000000 danling-0.2.4/danling/runner/base_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    14755 2023-04-15 07:40:36.000000 danling-0.2.4/danling/runner/runner_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-04-15 07:40:36.000000 danling-0.2.4/danling/runner/runner_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-04-15 07:40:36.000000 danling-0.2.4/danling/runner/torch_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-15 07:40:36.000000 danling-0.2.4/danling/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.151348 danling-0.2.4/danling/tensors/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-15 07:40:36.000000 danling-0.2.4/danling/tensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21621 2023-04-15 07:40:36.000000 danling-0.2.4/danling/tensors/nested_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-15 07:40:36.000000 danling-0.2.4/danling/tensors/torch_func_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-15 07:40:36.000000 danling-0.2.4/danling/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.155348 danling-0.2.4/danling/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-15 07:40:36.000000 danling-0.2.4/danling/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-15 07:40:36.000000 danling-0.2.4/danling/utils/basex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-15 07:40:36.000000 danling-0.2.4/danling/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-04-15 07:40:36.000000 danling-0.2.4/danling/utils/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.151348 danling-0.2.4/danling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-15 07:40:42.000000 danling-0.2.4/danling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-15 07:40:42.000000 danling-0.2.4/danling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 07:40:42.000000 danling-0.2.4/danling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-15 07:40:42.000000 danling-0.2.4/danling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-15 07:40:42.000000 danling-0.2.4/danling.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.155348 danling-0.2.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-15 07:40:36.000000 danling-0.2.4/docs/CNAME
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.155348 danling-0.2.4/docs/blog/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-15 07:40:36.000000 danling-0.2.4/docs/blog/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-15 07:40:36.000000 danling-0.2.4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-15 07:40:36.000000 danling-0.2.4/docs/manifest.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.155348 danling-0.2.4/docs/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-15 07:40:36.000000 danling-0.2.4/docs/metrics/average_meter.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.155348 danling-0.2.4/docs/optim/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-15 07:40:36.000000 danling-0.2.4/docs/optim/lr_scheduler.md
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-15 07:40:36.000000 danling-0.2.4/docs/package.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-15 07:40:36.000000 danling-0.2.4/docs/registry.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.155348 danling-0.2.4/docs/runner/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-15 07:40:36.000000 danling-0.2.4/docs/runner/base_runner.md
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-15 07:40:36.000000 danling-0.2.4/docs/runner/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-15 07:40:36.000000 danling-0.2.4/docs/runner/runner_base.md
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-15 07:40:36.000000 danling-0.2.4/docs/runner/runner_state.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-15 07:40:36.000000 danling-0.2.4/docs/runner/torch_runner.md
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-15 07:40:36.000000 danling-0.2.4/docs/runner/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.155348 danling-0.2.4/docs/tensors/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-15 07:40:36.000000 danling-0.2.4/docs/tensors/nested_tensor.md
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-15 07:40:36.000000 danling-0.2.4/docs/tensors/pn_tensor.md
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-15 07:40:36.000000 danling-0.2.4/docs/tensors/torch_func_registry.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.155348 danling-0.2.4/docs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-15 07:40:36.000000 danling-0.2.4/docs/utils/basex.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-15 07:40:36.000000 danling-0.2.4/docs/utils/decorators.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-15 07:40:36.000000 danling-0.2.4/docs/utils/io.md
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-04-15 07:40:36.000000 danling-0.2.4/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.155348 danling-0.2.4/overrides/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.147348 danling-0.2.4/overrides/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.155348 danling-0.2.4/overrides/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-15 07:40:36.000000 danling-0.2.4/overrides/assets/css/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-15 07:40:36.000000 danling-0.2.4/overrides/assets/css/fonts.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.167348 danling-0.2.4/overrides/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   213368 2023-04-15 07:40:36.000000 danling-0.2.4/overrides/assets/fonts/CascadiaCodePL.woff2
--rw-r--r--   0 runner    (1001) docker     (123)  8530056 2023-04-15 07:40:37.000000 danling-0.2.4/overrides/assets/fonts/HYQiHei.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   118704 2023-04-15 07:40:37.000000 danling-0.2.4/overrides/assets/fonts/HelveticaNowDisplay.otf
--rw-r--r--   0 runner    (1001) docker     (123)   656232 2023-04-15 07:40:37.000000 danling-0.2.4/overrides/assets/fonts/HelveticaWorld.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.167348 danling-0.2.4/overrides/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-04-15 07:40:37.000000 danling-0.2.4/overrides/assets/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    21972 2023-04-15 07:40:37.000000 danling-0.2.4/overrides/assets/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.167348 danling-0.2.4/overrides/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-15 07:40:37.000000 danling-0.2.4/overrides/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-15 07:40:37.000000 danling-0.2.4/overrides/javascripts/shortcuts.js
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-15 07:40:37.000000 danling-0.2.4/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-15 07:40:37.000000 danling-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-15 07:40:37.000000 danling-0.2.4/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-15 07:40:37.000000 danling-0.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 07:40:42.167348 danling-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 07:40:37.000000 danling-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.167348 danling-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-04-15 07:40:37.000000 danling-0.2.4/tests/test_lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-04-15 07:40:37.000000 danling-0.2.4/tests/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.643284 danling-0.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.615284 danling-0.2.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-26 10:03:10.000000 danling-0.2.5/.github/merge_rules.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.615284 danling-0.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-26 10:03:10.000000 danling-0.2.5/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-26 10:03:10.000000 danling-0.2.5/.github/workflows/push.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-04-26 10:03:10.000000 danling-0.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-26 10:03:10.000000 danling-0.2.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.619284 danling-0.2.5/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 10:03:10.000000 danling-0.2.5/LICENSES/LICENSE.Apache2
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-26 10:03:10.000000 danling-0.2.5/LICENSES/LICENSE.BSD2
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-26 10:03:10.000000 danling-0.2.5/LICENSES/LICENSE.BSD3
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-26 10:03:10.000000 danling-0.2.5/LICENSES/LICENSE.BSD4
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-26 10:03:10.000000 danling-0.2.5/LICENSES/LICENSE.GPL2
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-26 10:03:10.000000 danling-0.2.5/LICENSES/LICENSE.GPL3
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-26 10:03:10.000000 danling-0.2.5/LICENSES/LICENSE.MIT
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-26 10:03:10.000000 danling-0.2.5/LICENSES/LICENSE.Unlicense
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-26 10:03:19.643284 danling-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-26 10:03:10.000000 danling-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-26 10:03:10.000000 danling-0.2.5/anaconda-project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.619284 danling-0.2.5/danling/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-26 10:03:10.000000 danling-0.2.5/danling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 10:03:18.000000 danling-0.2.5/danling/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.623284 danling-0.2.5/danling/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-26 10:03:10.000000 danling-0.2.5/danling/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-26 10:03:10.000000 danling-0.2.5/danling/metrics/average_meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-26 10:03:10.000000 danling-0.2.5/danling/metrics/average_meters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.623284 danling-0.2.5/danling/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-26 10:03:10.000000 danling-0.2.5/danling/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.623284 danling-0.2.5/danling/modules/mlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-26 10:03:10.000000 danling-0.2.5/danling/modules/mlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-26 10:03:10.000000 danling-0.2.5/danling/modules/mlp/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-26 10:03:10.000000 danling-0.2.5/danling/modules/mlp/mlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.623284 danling-0.2.5/danling/modules/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-26 10:03:10.000000 danling-0.2.5/danling/modules/transformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.627284 danling-0.2.5/danling/modules/transformer/attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-26 10:03:10.000000 danling-0.2.5/danling/modules/transformer/attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-04-26 10:03:10.000000 danling-0.2.5/danling/modules/transformer/attention/multihead_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-04-26 10:03:10.000000 danling-0.2.5/danling/modules/transformer/attention/simple_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-04-26 10:03:10.000000 danling-0.2.5/danling/modules/transformer/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-04-26 10:03:10.000000 danling-0.2.5/danling/modules/transformer/encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.627284 danling-0.2.5/danling/modules/transformer/ffn/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-26 10:03:10.000000 danling-0.2.5/danling/modules/transformer/ffn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-26 10:03:10.000000 danling-0.2.5/danling/modules/transformer/ffn/fcn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.627284 danling-0.2.5/danling/modules/transformer/pos_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-26 10:03:10.000000 danling-0.2.5/danling/modules/transformer/pos_embed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-04-26 10:03:10.000000 danling-0.2.5/danling/modules/transformer/pos_embed/pos_embed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.627284 danling-0.2.5/danling/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-26 10:03:10.000000 danling-0.2.5/danling/optim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.627284 danling-0.2.5/danling/optim/lr_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-26 10:03:10.000000 danling-0.2.5/danling/optim/lr_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-04-26 10:03:10.000000 danling-0.2.5/danling/optim/lr_scheduler/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-04-26 10:03:10.000000 danling-0.2.5/danling/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.631284 danling-0.2.5/danling/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-04-26 10:03:10.000000 danling-0.2.5/danling/runner/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-26 10:03:10.000000 danling-0.2.5/danling/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-04-26 10:03:10.000000 danling-0.2.5/danling/runner/base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14755 2023-04-26 10:03:10.000000 danling-0.2.5/danling/runner/runner_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-04-26 10:03:10.000000 danling-0.2.5/danling/runner/runner_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-04-26 10:03:10.000000 danling-0.2.5/danling/runner/torch_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-26 10:03:10.000000 danling-0.2.5/danling/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.631284 danling-0.2.5/danling/tensors/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-26 10:03:10.000000 danling-0.2.5/danling/tensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21621 2023-04-26 10:03:10.000000 danling-0.2.5/danling/tensors/nested_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-26 10:03:10.000000 danling-0.2.5/danling/tensors/torch_func_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-26 10:03:10.000000 danling-0.2.5/danling/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.631284 danling-0.2.5/danling/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-26 10:03:10.000000 danling-0.2.5/danling/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-26 10:03:10.000000 danling-0.2.5/danling/utils/basex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-26 10:03:10.000000 danling-0.2.5/danling/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-04-26 10:03:10.000000 danling-0.2.5/danling/utils/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.623284 danling-0.2.5/danling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-26 10:03:19.000000 danling-0.2.5/danling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-26 10:03:19.000000 danling-0.2.5/danling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 10:03:19.000000 danling-0.2.5/danling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-26 10:03:19.000000 danling-0.2.5/danling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 10:03:19.000000 danling-0.2.5/danling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.631284 danling-0.2.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-26 10:03:10.000000 danling-0.2.5/docs/CNAME
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.631284 danling-0.2.5/docs/blog/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 10:03:10.000000 danling-0.2.5/docs/blog/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-26 10:03:10.000000 danling-0.2.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-26 10:03:10.000000 danling-0.2.5/docs/manifest.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.631284 danling-0.2.5/docs/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-26 10:03:10.000000 danling-0.2.5/docs/metrics/average_meter.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.631284 danling-0.2.5/docs/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-26 10:03:10.000000 danling-0.2.5/docs/optim/lr_scheduler.md
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-26 10:03:10.000000 danling-0.2.5/docs/package.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-26 10:03:10.000000 danling-0.2.5/docs/registry.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.631284 danling-0.2.5/docs/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-26 10:03:10.000000 danling-0.2.5/docs/runner/base_runner.md
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-26 10:03:10.000000 danling-0.2.5/docs/runner/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-26 10:03:10.000000 danling-0.2.5/docs/runner/runner_base.md
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-26 10:03:10.000000 danling-0.2.5/docs/runner/runner_state.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-26 10:03:10.000000 danling-0.2.5/docs/runner/torch_runner.md
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-26 10:03:10.000000 danling-0.2.5/docs/runner/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.631284 danling-0.2.5/docs/tensors/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-26 10:03:10.000000 danling-0.2.5/docs/tensors/nested_tensor.md
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-26 10:03:10.000000 danling-0.2.5/docs/tensors/pn_tensor.md
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-26 10:03:10.000000 danling-0.2.5/docs/tensors/torch_func_registry.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.631284 danling-0.2.5/docs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-26 10:03:10.000000 danling-0.2.5/docs/utils/basex.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-26 10:03:10.000000 danling-0.2.5/docs/utils/decorators.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-26 10:03:10.000000 danling-0.2.5/docs/utils/io.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-04-26 10:03:10.000000 danling-0.2.5/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.631284 danling-0.2.5/overrides/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.615284 danling-0.2.5/overrides/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.631284 danling-0.2.5/overrides/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-26 10:03:10.000000 danling-0.2.5/overrides/assets/css/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-26 10:03:10.000000 danling-0.2.5/overrides/assets/css/fonts.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.643284 danling-0.2.5/overrides/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   213368 2023-04-26 10:03:10.000000 danling-0.2.5/overrides/assets/fonts/CascadiaCodePL.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)  8530056 2023-04-26 10:03:11.000000 danling-0.2.5/overrides/assets/fonts/HYQiHei.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   118704 2023-04-26 10:03:11.000000 danling-0.2.5/overrides/assets/fonts/HelveticaNowDisplay.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   656232 2023-04-26 10:03:11.000000 danling-0.2.5/overrides/assets/fonts/HelveticaWorld.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.643284 danling-0.2.5/overrides/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-04-26 10:03:11.000000 danling-0.2.5/overrides/assets/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    21972 2023-04-26 10:03:11.000000 danling-0.2.5/overrides/assets/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.643284 danling-0.2.5/overrides/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-26 10:03:11.000000 danling-0.2.5/overrides/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-26 10:03:11.000000 danling-0.2.5/overrides/javascripts/shortcuts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-26 10:03:11.000000 danling-0.2.5/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-26 10:03:11.000000 danling-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-26 10:03:11.000000 danling-0.2.5/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-26 10:03:11.000000 danling-0.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 10:03:19.643284 danling-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 10:03:11.000000 danling-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.643284 danling-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-04-26 10:03:11.000000 danling-0.2.5/tests/test_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-04-26 10:03:11.000000 danling-0.2.5/tests/test_runner.py
```

### Comparing `danling-0.2.4/.github/workflows/docs.yaml` & `danling-0.2.5/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/.github/workflows/push.yaml` & `danling-0.2.5/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/.gitignore` & `danling-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/LICENSES/LICENSE.Apache2` & `danling-0.2.5/LICENSES/LICENSE.Apache2`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/LICENSES/LICENSE.BSD2` & `danling-0.2.5/LICENSES/LICENSE.BSD2`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/LICENSES/LICENSE.BSD3` & `danling-0.2.5/LICENSES/LICENSE.BSD3`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/LICENSES/LICENSE.BSD4` & `danling-0.2.5/LICENSES/LICENSE.BSD4`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/LICENSES/LICENSE.GPL2` & `danling-0.2.5/LICENSES/LICENSE.GPL2`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/LICENSES/LICENSE.GPL3` & `danling-0.2.5/LICENSES/LICENSE.GPL3`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/LICENSES/LICENSE.MIT` & `danling-0.2.5/LICENSES/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/LICENSES/LICENSE.Unlicense` & `danling-0.2.5/LICENSES/LICENSE.Unlicense`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/PKG-INFO` & `danling-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danling
-Version: 0.2.4
+Version: 0.2.5
 Summary: Scaffold for experienced Machine Learning Researchers
 Author-email: Zhiyuan Chen <this@zyc.ai>
 Maintainer-email: Zhiyuan Chen <this@zyc.ai>
 License: Unlicense OR GPL-2.0-or-later OR MIT OR Apache-2.0 OR BSD-2-Clause OR BSD-3-Clause OR BSD-4-Clause
 Project-URL: homepage, https://danling.org
 Project-URL: repository, https://github.com/ZhiyuanChen/DanLing
 Project-URL: documentation, https://danling.org
```

### Comparing `danling-0.2.4/README.md` & `danling-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/anaconda-project.yml` & `danling-0.2.5/anaconda-project.yml`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/danling/__init__.py` & `danling-0.2.5/danling/__init__.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/danling/metrics/average_meter.py` & `danling-0.2.5/danling/metrics/average_meter.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/danling/metrics/average_meters.py` & `danling-0.2.5/danling/metrics/average_meters.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/danling/modules/__init__.py` & `danling-0.2.5/danling/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/danling/modules/mlp/dense.py` & `danling-0.2.5/danling/modules/mlp/dense.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/danling/modules/mlp/mlp.py` & `danling-0.2.5/danling/modules/mlp/mlp.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/danling/modules/transformer/__init__.py` & `danling-0.2.5/danling/modules/transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/danling/modules/transformer/attention/multihead_attention.py` & `danling-0.2.5/danling/modules/transformer/attention/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/danling/modules/transformer/attention/simple_attention.py` & `danling-0.2.5/danling/modules/transformer/attention/simple_attention.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/danling/modules/transformer/decoder.py` & `danling-0.2.5/danling/modules/transformer/decoder.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/danling/modules/transformer/encoder.py` & `danling-0.2.5/danling/modules/transformer/encoder.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/danling/modules/transformer/ffn/fcn.py` & `danling-0.2.5/danling/modules/transformer/ffn/fcn.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/danling/modules/transformer/pos_embed/pos_embed.py` & `danling-0.2.5/danling/modules/transformer/pos_embed/pos_embed.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/danling/optim/lr_scheduler/lr_scheduler.py` & `danling-0.2.5/danling/optim/lr_scheduler/lr_scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from torch.optim import Optimizer, lr_scheduler
 
 
 class LRScheduler(lr_scheduler._LRScheduler):  # pylint: disable=W0212
     r"""
     General learning rate scheduler.
 
-    PyTorch LRScheduler is hard to entend.
+    PyTorch LRScheduler is hard to extend.
     This class is a wrapper of PyTorch LRScheduler, which provides a more general interface.
     You only needs to add a new method which calculates a learning rate ratio (range from 0 to 1)
     with total progress (range from 0 to 1), and everything else will be done automatically.
 
     Moreover, this class has warmup and cooldown built-in.
     By default, the first 5% and last 20% of training steps will be warmup and cooldown respectively.
     You can alternate by passing `warmup_steps` and `cooldown_steps`, or disable them by setting them to 0.
@@ -104,15 +104,15 @@
         self.strategy = strategy
         self.method = method
         self.warmup_steps = warmup_steps
         self.cooldown_steps = cooldown_steps
         self.cooldown_steps_begin = self.steps - self.cooldown_steps
         super().__init__(optimizer, last_epoch)
 
-    def get_lr(self) -> List[float]:
+    def get_lr(self) -> List[float]:  # type: ignore
         step_count = self._step_count  # type: ignore
         if step_count > self.steps + 1 or step_count < 1:
             warn(f"Step count {step_count} is out of range [1, {self.steps + 1}]", RuntimeWarning)
         progress = np.clip(step_count / self.steps, 0.0, 1.0)
         warmup_ratio = step_count / self.warmup_steps if self.warmup_steps > 0 else 1.0
         cooldown_ratio = (
             1 - (step_count - self.cooldown_steps_begin) / self.cooldown_steps if self.cooldown_steps > 0 else 1.0
```

### Comparing `danling-0.2.4/danling/registry.py` & `danling-0.2.5/danling/registry.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/danling/runner/README.md` & `danling-0.2.5/danling/runner/README.md`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/danling/runner/base_runner.py` & `danling-0.2.5/danling/runner/base_runner.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/danling/runner/runner_base.py` & `danling-0.2.5/danling/runner/runner_base.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/danling/runner/runner_state.py` & `danling-0.2.5/danling/runner/runner_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from chanfig import NestedDict
 
 try:
     from git.exc import InvalidGitRepositoryError
     from git.repo import Repo
 except ImportError:
     warn("gitpython not installed, git hash will not be available")
-    Repo = None
+    Repo = None  # type: ignore
 
 from danling.utils import base62
 
 PathStr = Union[os.PathLike, str, bytes]
 File = Union[PathStr, IO]
 
 DEFAULT_EXPERIMENT_NAME = "DanLing"
```

### Comparing `danling-0.2.4/danling/runner/torch_runner.py` & `danling-0.2.5/danling/runner/torch_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,19 +27,20 @@
 
     # pylint: disable=R0902
 
     accelerator: Accelerator = None  # type: ignore
     accelerate: Mapping[str, Any]
 
     def __init__(self, *args, **kwargs) -> None:
-        self.accelerate = {}
+        if "accelerate" not in self:
+            self.accelerate = {}
         if len(args) == 1 and isinstance(args[0], dict):
-            self.accelerate.update(args[0].pop("accelerate", {}))
+            self.accelerate.update(args[0].pop("accelerate", {}))  # type: ignore
         if "accelerate" in kwargs:
-            self.accelerate.update(kwargs.pop("accelerate"))
+            self.accelerate.update(kwargs.pop("accelerate"))  # type: ignore
         super().__init__(*args, **kwargs)
 
     def init_distributed(self) -> None:
         r"""
         Set up distributed training.
 
         Initialise process group and set up DDP variables.
```

### Comparing `danling-0.2.4/danling/runner/utils.py` & `danling-0.2.5/danling/runner/utils.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/danling/tensors/nested_tensor.py` & `danling-0.2.5/danling/tensors/nested_tensor.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/danling/tensors/torch_func_registry.py` & `danling-0.2.5/danling/tensors/torch_func_registry.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/danling/utils/basex.py` & `danling-0.2.5/danling/utils/basex.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/danling/utils/decorators.py` & `danling-0.2.5/danling/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/danling/utils/io.py` & `danling-0.2.5/danling/utils/io.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/danling.egg-info/PKG-INFO` & `danling-0.2.5/danling.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danling
-Version: 0.2.4
+Version: 0.2.5
 Summary: Scaffold for experienced Machine Learning Researchers
 Author-email: Zhiyuan Chen <this@zyc.ai>
 Maintainer-email: Zhiyuan Chen <this@zyc.ai>
 License: Unlicense OR GPL-2.0-or-later OR MIT OR Apache-2.0 OR BSD-2-Clause OR BSD-3-Clause OR BSD-4-Clause
 Project-URL: homepage, https://danling.org
 Project-URL: repository, https://github.com/ZhiyuanChen/DanLing
 Project-URL: documentation, https://danling.org
```

### Comparing `danling-0.2.4/danling.egg-info/SOURCES.txt` & `danling-0.2.5/danling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/mkdocs.yml` & `danling-0.2.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/overrides/assets/fonts/CascadiaCodePL.woff2` & `danling-0.2.5/overrides/assets/fonts/CascadiaCodePL.woff2`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/overrides/assets/fonts/HYQiHei.ttf` & `danling-0.2.5/overrides/assets/fonts/HYQiHei.ttf`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/overrides/assets/fonts/HelveticaNowDisplay.otf` & `danling-0.2.5/overrides/assets/fonts/HelveticaNowDisplay.otf`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/overrides/assets/fonts/HelveticaWorld.ttf` & `danling-0.2.5/overrides/assets/fonts/HelveticaWorld.ttf`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/overrides/assets/images/favicon.ico` & `danling-0.2.5/overrides/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/overrides/assets/images/logo.png` & `danling-0.2.5/overrides/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/overrides/main.html` & `danling-0.2.5/overrides/main.html`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/pyproject.toml` & `danling-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/tests/test_lr_scheduler.py` & `danling-0.2.5/tests/test_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.4/tests/test_runner.py` & `danling-0.2.5/tests/test_runner.py`

 * *Files identical despite different names*

