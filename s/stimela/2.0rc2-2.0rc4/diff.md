# Comparing `tmp/stimela-2.0rc2.tar.gz` & `tmp/stimela-2.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stimela-2.0rc2.tar", max compression
+gzip compressed data, was "stimela-2.0rc4.tar", max compression
```

## Comparing `stimela-2.0rc2.tar` & `stimela-2.0rc4.tar`

### file list

```diff
@@ -1,152 +1,151 @@
--rw-r--r--   0        0        0    18047 2023-02-03 14:28:37.506645 stimela-2.0rc2/LICENSE
--rw-r--r--   0        0        0      642 2023-02-03 14:28:37.506645 stimela-2.0rc2/README.rst
--rw-r--r--   0        0        0     1086 2023-02-03 14:28:37.506645 stimela-2.0rc2/pyproject.toml
--rw-r--r--   0        0        0     1605 2023-02-03 14:28:37.506645 stimela-2.0rc2/scabha/__init__.py
--rw-r--r--   0        0        0     1622 2023-02-03 14:28:37.506645 stimela-2.0rc2/scabha/basetypes.py
--rw-r--r--   0        0        0      161 2023-02-03 14:28:37.506645 stimela-2.0rc2/scabha/cab_utils.py
--rw-r--r--   0        0        0    20610 2023-02-03 14:28:37.506645 stimela-2.0rc2/scabha/cargo.py
--rw-r--r--   0        0        0    11458 2023-02-03 14:28:37.506645 stimela-2.0rc2/scabha/configuratt/__init__.py
--rw-r--r--   0        0        0    10076 2023-02-03 14:28:37.506645 stimela-2.0rc2/scabha/configuratt/cache.py
--rw-r--r--   0        0        0      501 2023-02-03 14:28:37.506645 stimela-2.0rc2/scabha/configuratt/common.py
--rw-r--r--   0        0        0     9385 2023-02-03 14:28:37.506645 stimela-2.0rc2/scabha/configuratt/deps.py
--rw-r--r--   0        0        0    15499 2023-02-03 14:28:37.506645 stimela-2.0rc2/scabha/configuratt/resolvers.py
--rw-r--r--   0        0        0    19111 2023-02-03 14:28:37.506645 stimela-2.0rc2/scabha/evaluator.py
--rw-r--r--   0        0        0     2990 2023-02-03 14:28:37.506645 stimela-2.0rc2/scabha/exceptions.py
--rw-r--r--   0        0        0     3110 2023-02-03 14:28:37.510645 stimela-2.0rc2/scabha/logging_utils.py
--rw-r--r--   0        0        0      423 2023-02-03 14:28:37.510645 stimela-2.0rc2/scabha/proc_utils.py
--rw-r--r--   0        0        0     6402 2023-02-03 14:28:37.510645 stimela-2.0rc2/scabha/schema_utils.py
--rw-r--r--   0        0        0    20309 2023-02-03 14:28:37.510645 stimela-2.0rc2/scabha/substitutions.py
--rw-r--r--   0        0        0    12152 2023-02-03 14:28:37.510645 stimela-2.0rc2/scabha/validate.py
--rw-r--r--   0        0        0      662 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/__init__.py
--rw-r--r--   0        0        0     3565 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/backends/__init__.py
--rw-r--r--   0        0        0    10808 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/backends/docker.py
--rw-r--r--   0        0        0     4216 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/backends/flavours/__init__.py
--rw-r--r--   0        0        0      919 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/backends/flavours/binary.py
--rw-r--r--   0        0        0     3221 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/backends/flavours/casa.py
--rw-r--r--   0        0        0     8118 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/backends/flavours/python_flavours.py
--rw-r--r--   0        0        0      306 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/backends/kubernetes/__init__.py
--rw-r--r--   0        0        0    17289 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/backends/kubernetes/run_kube.py
--rw-r--r--   0        0        0       59 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/backends/native/__init__.py
--rw-r--r--   0        0        0     3396 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/backends/native/run_native.py
--rw-r--r--   0        0        0     7563 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/backends/podman.py
--rw-r--r--   0        0        0     4230 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/backends/singularity.py
--rw-r--r--   0        0        0      249 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/cargo/__init__.py
--rw-r--r--   0        0        0       56 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/cargo/base/21cmfast/Dockerfile
--rw-r--r--   0        0        0        0 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/cargo/base/__init__.py
--rw-r--r--   0        0        0       86 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/cargo/base/aegean/Dockerfile
--rw-r--r--   0        0        0      170 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/cargo/base/aimfast/Dockerfile
--rw-r--r--   0        0        0       57 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/cargo/base/aoflagger/Dockerfile
--rw-r--r--   0        0        0      180 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/cargo/base/astropy/Dockerfile
--rw-r--r--   0        0        0      538 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/cargo/base/base/Dockerfile
--rw-r--r--   0        0        0     1036 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/cargo/base/casa/Dockerfile
--rw-r--r--   0        0        0      987 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/cargo/base/casa/casa.yaml
--rw-r--r--   0        0        0        0 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/cargo/base/casa/casa.yml
--rw-r--r--   0        0        0      108 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/cargo/base/casarest/Dockerfile
--rw-r--r--   0        0        0      118 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/cargo/base/catdagger/Dockerfile
--rw-r--r--   0        0        0      993 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/cargo/base/chgcentre/Dockerfile
--rw-r--r--   0        0        0      266 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/cargo/base/codex-africanus/Dockerfile
--rw-r--r--   0        0        0      280 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/cargo/base/cubical/Dockerfile
--rw-r--r--   0        0        0      385 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/cargo/base/cubical_ddf/Dockerfile
--rw-r--r--   0        0        0       52 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/cargo/base/curl/Dockerfile
--rw-r--r--   0        0        0      420 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/cargo/base/ddfacet/Dockerfile
--rw-r--r--   0        0        0       98 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/cargo/base/eidos/Dockerfile
--rw-r--r--   0        0        0      490 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/cargo/base/group.template
--rw-r--r--   0        0        0      257 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/cargo/base/katdal/Dockerfile
--rw-r--r--   0        0        0      102 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/cargo/base/lofar/Dockerfile
--rw-r--r--   0        0        0      109 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/cargo/base/meqtrees/Dockerfile
--rw-r--r--   0        0        0      194 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/cargo/base/montage/Dockerfile
--rw-r--r--   0        0        0       51 2023-02-03 14:28:37.510645 stimela-2.0rc2/stimela/cargo/base/moresane/Dockerfile
--rw-r--r--   0        0        0      125 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/cargo/base/msutils/Dockerfile
--rw-r--r--   0        0        0      294 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/cargo/base/owlcat/Dockerfile
--rw-r--r--   0        0        0      979 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/cargo/base/passwd.template
--rw-r--r--   0        0        0      217 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/cargo/base/politsiyakat/Dockerfile
--rw-r--r--   0        0        0      103 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/cargo/base/pybdsf/Dockerfile
--rw-r--r--   0        0        0      116 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/cargo/base/pyddi/Dockerfile
--rw-r--r--   0        0        0      508 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/cargo/base/quartical/Dockerfile
--rw-r--r--   0        0        0      381 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/cargo/base/ragavi/Dockerfile
--rw-r--r--   0        0        0      352 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/cargo/base/rfimasker/Dockerfile
--rw-r--r--   0        0        0      285 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/cargo/base/rfinder/Dockerfile
--rw-r--r--   0        0        0       55 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/cargo/base/sagecal/Dockerfile
--rw-r--r--   0        0        0      231 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/cargo/base/shadems/Dockerfile
--rw-r--r--   0        0        0      266 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/cargo/base/shadems/Dockerfile.v040
--rw-r--r--   0        0        0      529 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/cargo/base/shadems/shadems.yaml
--rw-r--r--   0        0        0      236 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/cargo/base/sharpener/Dockerfile
--rw-r--r--   0        0        0      797 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/cargo/base/sofia/Dockerfile
--rw-r--r--   0        0        0      136 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/cargo/base/sourcery/Dockerfile
--rw-r--r--   0        0        0      189 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/cargo/base/sunblocker/Dockerfile
--rw-r--r--   0        0        0      193 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/cargo/base/tigger/Dockerfile
--rw-r--r--   0        0        0      678 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/cargo/base/tricolour/Dockerfile
--rw-r--r--   0        0        0      859 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/cargo/base/wsclean/Dockerfile
--rw-r--r--   0        0        0     1592 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/cargo/cab/casa_applycal.yaml
--rw-r--r--   0        0        0      614 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/cargo/cab/fitstool_stack.yaml
--rw-r--r--   0        0        0     5920 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/cargo/cab/shadems.yaml
--rw-r--r--   0        0        0      983 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/cargo/cab/simms.yaml
--rw-r--r--   0        0        0     2319 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/cargo/cab/tricolour.yaml
--rw-r--r--   0        0        0     1548 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/cargo/cab/wsclean.yaml
--rw-r--r--   0        0        0     2182 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/cargo/cab/wsclean_pol.yaml
--rw-r--r--   0        0        0     1197 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/cargo/lib/params/casa.yaml
--rw-r--r--   0        0        0     2559 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/cargo/lib/params/wsclean.yaml
--rw-r--r--   0        0        0        0 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/commands/__init__.py
--rw-r--r--   0        0        0     2249 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/commands/build.py
--rw-r--r--   0        0        0      832 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/commands/cabs.py
--rw-r--r--   0        0        0      896 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/commands/clean.py
--rw-r--r--   0        0        0      643 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/commands/containers.py
--rw-r--r--   0        0        0     5841 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/commands/help.py
--rw-r--r--   0        0        0     1681 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/commands/images.py
--rw-r--r--   0        0        0      371 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/commands/kill.py
--rw-r--r--   0        0        0      640 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/commands/ps.py
--rw-r--r--   0        0        0     1338 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/commands/pull.py
--rw-r--r--   0        0        0     1856 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/commands/push.py
--rw-r--r--   0        0        0    13131 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/commands/run.py
--rw-r--r--   0        0        0     2627 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/commands/save_config.py
--rw-r--r--   0        0        0    13171 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/config.py
--rw-r--r--   0        0        0     1761 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/exceptions.py
--rw-r--r--   0        0        0        0 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/kitchen/__init__.py
--rw-r--r--   0        0        0      533 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/kitchen/batch.py
--rw-r--r--   0        0        0    18688 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/kitchen/cab.py
--rw-r--r--   0        0        0    62522 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/kitchen/recipe.py
--rw-r--r--   0        0        0     1036 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/kitchen/runners.py
--rw-r--r--   0        0        0    26463 2023-02-03 14:28:37.514645 stimela-2.0rc2/stimela/kitchen/step.py
--rw-r--r--   0        0        0    11379 2023-02-03 14:28:37.518645 stimela-2.0rc2/stimela/kitchen/wranglers.py
--rw-r--r--   0        0        0     4820 2023-02-03 14:28:37.518645 stimela-2.0rc2/stimela/main.py
--rw-r--r--   0        0        0       29 2023-02-03 14:28:37.518645 stimela-2.0rc2/stimela/schedulers/__init__.py
--rw-r--r--   0        0        0     2274 2023-02-03 14:28:37.518645 stimela-2.0rc2/stimela/schedulers/slurm.py
--rw-r--r--   0        0        0    14999 2023-02-03 14:28:37.518645 stimela-2.0rc2/stimela/stimelogging.py
--rw-r--r--   0        0        0    10741 2023-02-03 14:28:37.518645 stimela-2.0rc2/stimela/task_stats.py
--rw-r--r--   0        0        0      254 2023-02-03 14:28:37.518645 stimela-2.0rc2/stimela/utils/__init__.py
--rw-r--r--   0        0        0     7314 2023-02-03 14:28:37.518645 stimela-2.0rc2/stimela/utils/xrun_asyncio.py
--rw-r--r--   0        0        0     9181 2023-02-03 14:28:37.518645 stimela-2.0rc2/stimela/utils/xrun_poll.py
--rw-r--r--   0        0        0        0 2023-02-03 14:28:37.518645 stimela-2.0rc2/tests/scabha_tests/__init__.py
--rw-r--r--   0        0        0     1965 2023-02-03 14:28:37.518645 stimela-2.0rc2/tests/scabha_tests/test_configuratt.py
--rw-r--r--   0        0        0      540 2023-02-03 14:28:37.518645 stimela-2.0rc2/tests/scabha_tests/test_dynschema.py
--rw-r--r--   0        0        0       70 2023-02-03 14:28:37.518645 stimela-2.0rc2/tests/scabha_tests/test_include.yaml
--rw-r--r--   0        0        0       46 2023-02-03 14:28:37.518645 stimela-2.0rc2/tests/scabha_tests/test_include2.yaml
--rw-r--r--   0        0        0       21 2023-02-03 14:28:37.518645 stimela-2.0rc2/tests/scabha_tests/test_nest_a.yml
--rw-r--r--   0        0        0       21 2023-02-03 14:28:37.518645 stimela-2.0rc2/tests/scabha_tests/test_nest_b.yml
--rw-r--r--   0        0        0       25 2023-02-03 14:28:37.518645 stimela-2.0rc2/tests/scabha_tests/test_nest_c.yml
--rw-r--r--   0        0        0     1659 2023-02-03 14:28:37.518645 stimela-2.0rc2/tests/scabha_tests/test_parsing.py
--rw-r--r--   0        0        0      658 2023-02-03 14:28:37.518645 stimela-2.0rc2/tests/scabha_tests/test_schema.py
--rw-r--r--   0        0        0       55 2023-02-03 14:28:37.518645 stimela-2.0rc2/tests/scabha_tests/test_schema.yaml
--rw-r--r--   0        0        0     5805 2023-02-03 14:28:37.518645 stimela-2.0rc2/tests/scabha_tests/test_substitutions.py
--rw-r--r--   0        0        0      924 2023-02-03 14:28:37.518645 stimela-2.0rc2/tests/scabha_tests/testconf.yaml
--rw-r--r--   0        0        0        0 2023-02-03 14:28:37.518645 stimela-2.0rc2/tests/stimela_tests/__init__.py
--rw-r--r--   0        0        0      240 2023-02-03 14:28:37.518645 stimela-2.0rc2/tests/stimela_tests/example_callable.py
--rw-r--r--   0        0        0      541 2023-02-03 14:28:37.518645 stimela-2.0rc2/tests/stimela_tests/example_dynschema.py
--rw-r--r--   0        0        0     1428 2023-02-03 14:28:37.518645 stimela-2.0rc2/tests/stimela_tests/test_aliasing.yml
--rw-r--r--   0        0        0      554 2023-02-03 14:28:37.518645 stimela-2.0rc2/tests/stimela_tests/test_callables.py
--rw-r--r--   0        0        0     2033 2023-02-03 14:28:37.518645 stimela-2.0rc2/tests/stimela_tests/test_callables.yml
--rw-r--r--   0        0        0      756 2023-02-03 14:28:37.518645 stimela-2.0rc2/tests/stimela_tests/test_casa.yml
--rw-r--r--   0        0        0      172 2023-02-03 14:28:37.518645 stimela-2.0rc2/tests/stimela_tests/test_dask_storage_options.yaml
--rw-r--r--   0        0        0     2228 2023-02-03 14:28:37.518645 stimela-2.0rc2/tests/stimela_tests/test_kube.yml
--rw-r--r--   0        0        0     2033 2023-02-03 14:28:37.518645 stimela-2.0rc2/tests/stimela_tests/test_loop_recipe.yml
--rw-r--r--   0        0        0     2154 2023-02-03 14:28:37.518645 stimela-2.0rc2/tests/stimela_tests/test_loop_recipe_slurm.yml
--rw-r--r--   0        0        0     4408 2023-02-03 14:28:37.518645 stimela-2.0rc2/tests/stimela_tests/test_nesting.yml
--rw-r--r--   0        0        0     3441 2023-02-03 14:28:37.518645 stimela-2.0rc2/tests/stimela_tests/test_recipe.py
--rw-r--r--   0        0        0     4023 2023-02-03 14:28:37.518645 stimela-2.0rc2/tests/stimela_tests/test_recipe.yml
--rw-r--r--   0        0        0     1390 2023-02-03 14:28:37.518645 stimela-2.0rc2/tests/stimela_tests/test_scatter.yml
--rw-r--r--   0        0        0     1882 2023-02-03 14:28:37.518645 stimela-2.0rc2/tests/stimela_tests/test_wranglers.py
--rw-r--r--   0        0        0      205 2023-02-03 14:28:37.518645 stimela-2.0rc2/tests/stimela_tests/test_wranglers.txt
--rw-r--r--   0        0        0     3010 2023-02-03 14:28:37.518645 stimela-2.0rc2/tests/stimela_tests/test_wranglers.yml
--rw-r--r--   0        0        0     1273 2023-02-03 14:28:37.518645 stimela-2.0rc2/tests/stimela_tests/test_xrun.yml
--rw-r--r--   0        0        0     3521 1970-01-01 00:00:00.000000 stimela-2.0rc2/setup.py
--rw-r--r--   0        0        0     1586 1970-01-01 00:00:00.000000 stimela-2.0rc2/PKG-INFO
+-rw-r--r--   0        0        0    18047 2023-03-28 14:27:45.913525 stimela-2.0rc4/LICENSE
+-rw-r--r--   0        0        0      642 2023-03-28 14:27:45.913525 stimela-2.0rc4/README.rst
+-rw-r--r--   0        0        0     1086 2023-03-28 14:27:45.913525 stimela-2.0rc4/pyproject.toml
+-rw-r--r--   0        0        0     1605 2023-03-28 14:27:45.913525 stimela-2.0rc4/scabha/__init__.py
+-rw-r--r--   0        0        0     1622 2023-03-28 14:27:45.913525 stimela-2.0rc4/scabha/basetypes.py
+-rw-r--r--   0        0        0      161 2023-03-28 14:27:45.913525 stimela-2.0rc4/scabha/cab_utils.py
+-rw-r--r--   0        0        0    20610 2023-03-28 14:27:45.917525 stimela-2.0rc4/scabha/cargo.py
+-rw-r--r--   0        0        0    11458 2023-03-28 14:27:45.917525 stimela-2.0rc4/scabha/configuratt/__init__.py
+-rw-r--r--   0        0        0    10076 2023-03-28 14:27:45.917525 stimela-2.0rc4/scabha/configuratt/cache.py
+-rw-r--r--   0        0        0      501 2023-03-28 14:27:45.917525 stimela-2.0rc4/scabha/configuratt/common.py
+-rw-r--r--   0        0        0     9385 2023-03-28 14:27:45.917525 stimela-2.0rc4/scabha/configuratt/deps.py
+-rw-r--r--   0        0        0    15499 2023-03-28 14:27:45.917525 stimela-2.0rc4/scabha/configuratt/resolvers.py
+-rw-r--r--   0        0        0    19111 2023-03-28 14:27:45.917525 stimela-2.0rc4/scabha/evaluator.py
+-rw-r--r--   0        0        0     2990 2023-03-28 14:27:45.917525 stimela-2.0rc4/scabha/exceptions.py
+-rw-r--r--   0        0        0     3110 2023-03-28 14:27:45.917525 stimela-2.0rc4/scabha/logging_utils.py
+-rw-r--r--   0        0        0      423 2023-03-28 14:27:45.917525 stimela-2.0rc4/scabha/proc_utils.py
+-rw-r--r--   0        0        0     6402 2023-03-28 14:27:45.917525 stimela-2.0rc4/scabha/schema_utils.py
+-rw-r--r--   0        0        0    20309 2023-03-28 14:27:45.917525 stimela-2.0rc4/scabha/substitutions.py
+-rw-r--r--   0        0        0    12152 2023-03-28 14:27:45.917525 stimela-2.0rc4/scabha/validate.py
+-rw-r--r--   0        0        0      662 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/__init__.py
+-rw-r--r--   0        0        0     3565 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/backends/__init__.py
+-rw-r--r--   0        0        0    10808 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/backends/docker.py
+-rw-r--r--   0        0        0     4216 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/backends/flavours/__init__.py
+-rw-r--r--   0        0        0      919 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/backends/flavours/binary.py
+-rw-r--r--   0        0        0     3221 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/backends/flavours/casa.py
+-rw-r--r--   0        0        0     8118 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/backends/flavours/python_flavours.py
+-rw-r--r--   0        0        0      306 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/backends/kubernetes/__init__.py
+-rw-r--r--   0        0        0    17289 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/backends/kubernetes/run_kube.py
+-rw-r--r--   0        0        0       59 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/backends/native/__init__.py
+-rw-r--r--   0        0        0     3396 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/backends/native/run_native.py
+-rw-r--r--   0        0        0     7563 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/backends/podman.py
+-rw-r--r--   0        0        0     4230 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/backends/singularity.py
+-rw-r--r--   0        0        0      249 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/__init__.py
+-rw-r--r--   0        0        0       56 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/21cmfast/Dockerfile
+-rw-r--r--   0        0        0        0 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/__init__.py
+-rw-r--r--   0        0        0       86 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/aegean/Dockerfile
+-rw-r--r--   0        0        0      170 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/aimfast/Dockerfile
+-rw-r--r--   0        0        0       57 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/aoflagger/Dockerfile
+-rw-r--r--   0        0        0      180 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/astropy/Dockerfile
+-rw-r--r--   0        0        0      538 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/base/Dockerfile
+-rw-r--r--   0        0        0     1036 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/casa/Dockerfile
+-rw-r--r--   0        0        0      987 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/casa/casa.yaml
+-rw-r--r--   0        0        0        0 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/casa/casa.yml
+-rw-r--r--   0        0        0      108 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/casarest/Dockerfile
+-rw-r--r--   0        0        0      118 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/catdagger/Dockerfile
+-rw-r--r--   0        0        0      993 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/chgcentre/Dockerfile
+-rw-r--r--   0        0        0      266 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/codex-africanus/Dockerfile
+-rw-r--r--   0        0        0      280 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/cubical/Dockerfile
+-rw-r--r--   0        0        0      385 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/cubical_ddf/Dockerfile
+-rw-r--r--   0        0        0       52 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/curl/Dockerfile
+-rw-r--r--   0        0        0      420 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/ddfacet/Dockerfile
+-rw-r--r--   0        0        0       98 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/eidos/Dockerfile
+-rw-r--r--   0        0        0      490 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/group.template
+-rw-r--r--   0        0        0      257 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/katdal/Dockerfile
+-rw-r--r--   0        0        0      102 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/lofar/Dockerfile
+-rw-r--r--   0        0        0      109 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/meqtrees/Dockerfile
+-rw-r--r--   0        0        0      194 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/montage/Dockerfile
+-rw-r--r--   0        0        0       51 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/moresane/Dockerfile
+-rw-r--r--   0        0        0      125 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/msutils/Dockerfile
+-rw-r--r--   0        0        0      294 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/owlcat/Dockerfile
+-rw-r--r--   0        0        0      979 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/passwd.template
+-rw-r--r--   0        0        0      217 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/politsiyakat/Dockerfile
+-rw-r--r--   0        0        0      103 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/pybdsf/Dockerfile
+-rw-r--r--   0        0        0      116 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/pyddi/Dockerfile
+-rw-r--r--   0        0        0      508 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/quartical/Dockerfile
+-rw-r--r--   0        0        0      381 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/ragavi/Dockerfile
+-rw-r--r--   0        0        0      352 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/rfimasker/Dockerfile
+-rw-r--r--   0        0        0      285 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/rfinder/Dockerfile
+-rw-r--r--   0        0        0       55 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/sagecal/Dockerfile
+-rw-r--r--   0        0        0      231 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/shadems/Dockerfile
+-rw-r--r--   0        0        0      266 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/shadems/Dockerfile.v040
+-rw-r--r--   0        0        0      529 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/shadems/shadems.yaml
+-rw-r--r--   0        0        0      236 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/sharpener/Dockerfile
+-rw-r--r--   0        0        0      797 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/sofia/Dockerfile
+-rw-r--r--   0        0        0      136 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/sourcery/Dockerfile
+-rw-r--r--   0        0        0      189 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/sunblocker/Dockerfile
+-rw-r--r--   0        0        0      193 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/tigger/Dockerfile
+-rw-r--r--   0        0        0      678 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/tricolour/Dockerfile
+-rw-r--r--   0        0        0      859 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/wsclean/Dockerfile
+-rw-r--r--   0        0        0     1592 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/cab/casa_applycal.yaml
+-rw-r--r--   0        0        0      614 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/cab/fitstool_stack.yaml
+-rw-r--r--   0        0        0     5920 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/cab/shadems.yaml
+-rw-r--r--   0        0        0      983 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/cab/simms.yaml
+-rw-r--r--   0        0        0     2319 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/cab/tricolour.yaml
+-rw-r--r--   0        0        0     1548 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/cab/wsclean.yaml
+-rw-r--r--   0        0        0     2182 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/cab/wsclean_pol.yaml
+-rw-r--r--   0        0        0     1197 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/lib/params/casa.yaml
+-rw-r--r--   0        0        0     2559 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/lib/params/wsclean.yaml
+-rw-r--r--   0        0        0        0 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/commands/__init__.py
+-rw-r--r--   0        0        0     2249 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/commands/build.py
+-rw-r--r--   0        0        0      832 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/commands/cabs.py
+-rw-r--r--   0        0        0      896 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/commands/clean.py
+-rw-r--r--   0        0        0      643 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/commands/containers.py
+-rw-r--r--   0        0        0     5847 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/commands/doc.py
+-rw-r--r--   0        0        0     1681 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/commands/images.py
+-rw-r--r--   0        0        0      371 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/commands/kill.py
+-rw-r--r--   0        0        0      640 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/commands/ps.py
+-rw-r--r--   0        0        0     1338 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/commands/pull.py
+-rw-r--r--   0        0        0     1856 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/commands/push.py
+-rw-r--r--   0        0        0    13131 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/commands/run.py
+-rw-r--r--   0        0        0     2627 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/commands/save_config.py
+-rw-r--r--   0        0        0    13171 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/config.py
+-rw-r--r--   0        0        0     1761 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/exceptions.py
+-rw-r--r--   0        0        0        0 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/kitchen/__init__.py
+-rw-r--r--   0        0        0      533 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/kitchen/batch.py
+-rw-r--r--   0        0        0    18688 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/kitchen/cab.py
+-rw-r--r--   0        0        0    62522 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/kitchen/recipe.py
+-rw-r--r--   0        0        0     1036 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/kitchen/runners.py
+-rw-r--r--   0        0        0    26463 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/kitchen/step.py
+-rw-r--r--   0        0        0    11379 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/kitchen/wranglers.py
+-rw-r--r--   0        0        0     4876 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/main.py
+-rw-r--r--   0        0        0       29 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/schedulers/__init__.py
+-rw-r--r--   0        0        0     2274 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/schedulers/slurm.py
+-rw-r--r--   0        0        0    14999 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/stimelogging.py
+-rw-r--r--   0        0        0    10741 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/task_stats.py
+-rw-r--r--   0        0        0      254 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/utils/__init__.py
+-rw-r--r--   0        0        0     7314 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/utils/xrun_asyncio.py
+-rw-r--r--   0        0        0     9181 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/utils/xrun_poll.py
+-rw-r--r--   0        0        0        0 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/scabha_tests/__init__.py
+-rw-r--r--   0        0        0     1965 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/scabha_tests/test_configuratt.py
+-rw-r--r--   0        0        0      540 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/scabha_tests/test_dynschema.py
+-rw-r--r--   0        0        0       70 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/scabha_tests/test_include.yaml
+-rw-r--r--   0        0        0       46 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/scabha_tests/test_include2.yaml
+-rw-r--r--   0        0        0       21 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/scabha_tests/test_nest_a.yml
+-rw-r--r--   0        0        0       21 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/scabha_tests/test_nest_b.yml
+-rw-r--r--   0        0        0       25 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/scabha_tests/test_nest_c.yml
+-rw-r--r--   0        0        0     1659 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/scabha_tests/test_parsing.py
+-rw-r--r--   0        0        0      658 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/scabha_tests/test_schema.py
+-rw-r--r--   0        0        0       55 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/scabha_tests/test_schema.yaml
+-rw-r--r--   0        0        0     5805 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/scabha_tests/test_substitutions.py
+-rw-r--r--   0        0        0      924 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/scabha_tests/testconf.yaml
+-rw-r--r--   0        0        0        0 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/__init__.py
+-rw-r--r--   0        0        0      240 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/example_callable.py
+-rw-r--r--   0        0        0      541 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/example_dynschema.py
+-rw-r--r--   0        0        0     1428 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/test_aliasing.yml
+-rw-r--r--   0        0        0      554 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/test_callables.py
+-rw-r--r--   0        0        0     2033 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/test_callables.yml
+-rw-r--r--   0        0        0      756 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/test_casa.yml
+-rw-r--r--   0        0        0      172 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/test_dask_storage_options.yaml
+-rw-r--r--   0        0        0     2228 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/test_kube.yml
+-rw-r--r--   0        0        0     2033 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/test_loop_recipe.yml
+-rw-r--r--   0        0        0     2154 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/test_loop_recipe_slurm.yml
+-rw-r--r--   0        0        0     4408 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/test_nesting.yml
+-rw-r--r--   0        0        0     3441 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/test_recipe.py
+-rw-r--r--   0        0        0     4023 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/test_recipe.yml
+-rw-r--r--   0        0        0     1390 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/test_scatter.yml
+-rw-r--r--   0        0        0     1882 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/test_wranglers.py
+-rw-r--r--   0        0        0      205 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/test_wranglers.txt
+-rw-r--r--   0        0        0     3010 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/test_wranglers.yml
+-rw-r--r--   0        0        0     1273 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/test_xrun.yml
+-rw-r--r--   0        0        0     1586 1970-01-01 00:00:00.000000 stimela-2.0rc4/PKG-INFO
```

### Comparing `stimela-2.0rc2/LICENSE` & `stimela-2.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/README.rst` & `stimela-2.0rc4/README.rst`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/pyproject.toml` & `stimela-2.0rc4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stimela"
-version = "2.0rc2"
+version = "2.0rc4"
 description = "Framework for system agnostic pipelines for radio interferometry arrays"
 authors = ["Sphesihle Makhathini <sphemakh@gmail.com>", "Oleg Smirnov and RATT <osmirnov@gmail.com>"]
 readme = "README.rst"
 license = "GNU GPL v2"
 include = [{ path = "tests" }]
 packages = [
     {include = "stimela"},
```

### Comparing `stimela-2.0rc2/scabha/__init__.py` & `stimela-2.0rc4/scabha/__init__.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/scabha/basetypes.py` & `stimela-2.0rc4/scabha/basetypes.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/scabha/cargo.py` & `stimela-2.0rc4/scabha/cargo.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     dtype: str = "str"
     # specifies that the value is implicitly set inside the step (i.e. not a free parameter). Typically used with filenames
     implicit: Any = None
     # optonal list of arbitrary tags, used to group parameters
     tags: List[str] = EmptyListDefault()
 
     # If True, parameter is required. None/False, not required.
-    # For outputs, required=False means invalid output will not be treated as an error.
+    # For outputs, required=False means missing output will not be treated as an error.
     # For aliases, False at recipe level will override the target setting, while the default of None won't.
     required: Optional[bool] = None
 
     # restrict value choices, i.e. making for an option-type parameter
     choices:  Optional[List[Any]] = ()
 
     # for List or Dict-type parameters, restict values of list elements or dict entries to a list of choices
```

### Comparing `stimela-2.0rc2/scabha/configuratt/__init__.py` & `stimela-2.0rc4/scabha/configuratt/__init__.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/scabha/configuratt/cache.py` & `stimela-2.0rc4/scabha/configuratt/cache.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/scabha/configuratt/deps.py` & `stimela-2.0rc4/scabha/configuratt/deps.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/scabha/configuratt/resolvers.py` & `stimela-2.0rc4/scabha/configuratt/resolvers.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/scabha/evaluator.py` & `stimela-2.0rc4/scabha/evaluator.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/scabha/exceptions.py` & `stimela-2.0rc4/scabha/exceptions.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/scabha/logging_utils.py` & `stimela-2.0rc4/scabha/logging_utils.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/scabha/schema_utils.py` & `stimela-2.0rc4/scabha/schema_utils.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/scabha/substitutions.py` & `stimela-2.0rc4/scabha/substitutions.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/scabha/validate.py` & `stimela-2.0rc4/scabha/validate.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/__init__.py` & `stimela-2.0rc4/stimela/__init__.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/backends/__init__.py` & `stimela-2.0rc4/stimela/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/backends/docker.py` & `stimela-2.0rc4/stimela/backends/docker.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/backends/flavours/__init__.py` & `stimela-2.0rc4/stimela/backends/flavours/__init__.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/backends/flavours/binary.py` & `stimela-2.0rc4/stimela/backends/flavours/binary.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/backends/flavours/casa.py` & `stimela-2.0rc4/stimela/backends/flavours/casa.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/backends/flavours/python_flavours.py` & `stimela-2.0rc4/stimela/backends/flavours/python_flavours.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/backends/kubernetes/run_kube.py` & `stimela-2.0rc4/stimela/backends/kubernetes/run_kube.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/backends/native/run_native.py` & `stimela-2.0rc4/stimela/backends/native/run_native.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/backends/podman.py` & `stimela-2.0rc4/stimela/backends/podman.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/backends/singularity.py` & `stimela-2.0rc4/stimela/backends/singularity.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/cargo/base/base/Dockerfile` & `stimela-2.0rc4/stimela/cargo/base/base/Dockerfile`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/cargo/base/casa/Dockerfile` & `stimela-2.0rc4/stimela/cargo/base/casa/Dockerfile`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/cargo/base/casa/casa.yaml` & `stimela-2.0rc4/stimela/cargo/base/casa/casa.yaml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/cargo/base/chgcentre/Dockerfile` & `stimela-2.0rc4/stimela/cargo/base/chgcentre/Dockerfile`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/cargo/base/passwd.template` & `stimela-2.0rc4/stimela/cargo/base/passwd.template`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/cargo/base/shadems/shadems.yaml` & `stimela-2.0rc4/stimela/cargo/base/shadems/shadems.yaml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/cargo/base/sofia/Dockerfile` & `stimela-2.0rc4/stimela/cargo/base/sofia/Dockerfile`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/cargo/base/tricolour/Dockerfile` & `stimela-2.0rc4/stimela/cargo/base/tricolour/Dockerfile`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/cargo/base/wsclean/Dockerfile` & `stimela-2.0rc4/stimela/cargo/base/wsclean/Dockerfile`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/cargo/cab/casa_applycal.yaml` & `stimela-2.0rc4/stimela/cargo/cab/casa_applycal.yaml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/cargo/cab/fitstool_stack.yaml` & `stimela-2.0rc4/stimela/cargo/cab/fitstool_stack.yaml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/cargo/cab/shadems.yaml` & `stimela-2.0rc4/stimela/cargo/cab/shadems.yaml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/cargo/cab/simms.yaml` & `stimela-2.0rc4/stimela/cargo/cab/simms.yaml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/cargo/cab/tricolour.yaml` & `stimela-2.0rc4/stimela/cargo/cab/tricolour.yaml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/cargo/cab/wsclean.yaml` & `stimela-2.0rc4/stimela/cargo/cab/wsclean.yaml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/cargo/cab/wsclean_pol.yaml` & `stimela-2.0rc4/stimela/cargo/cab/wsclean_pol.yaml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/cargo/lib/params/casa.yaml` & `stimela-2.0rc4/stimela/cargo/lib/params/casa.yaml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/cargo/lib/params/wsclean.yaml` & `stimela-2.0rc4/stimela/cargo/lib/params/wsclean.yaml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/commands/build.py` & `stimela-2.0rc4/stimela/commands/build.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/commands/cabs.py` & `stimela-2.0rc4/stimela/commands/cabs.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/commands/clean.py` & `stimela-2.0rc4/stimela/commands/clean.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/commands/containers.py` & `stimela-2.0rc4/stimela/commands/containers.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/commands/help.py` & `stimela-2.0rc4/stimela/commands/doc.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,33 +16,33 @@
 from stimela.kitchen.recipe import Recipe
 from stimela.kitchen.cab import Cab
 from stimela.config import ConfigExceptionTypes
 from stimela.exceptions import RecipeValidationError
 
 from .run import load_recipe_file
 
-@cli.command("help",
+@cli.command("doc",
     help="""
-    Print help on a cab or a recipe.
+    Print documentation on a cab or a recipe.
     """)
 @click.option("do_list", "-l", "--list", is_flag=True,
                 help="""Lists the available cabs and recipes, including custom-defined ones.""")
 @click.option("-I", "--implicit", is_flag=True,
                 help="""Increases level of detail to include implicit inputs/outputs.""")
 @click.option("-O", "--obscure", is_flag=True,
                 help="""Increases level of detail to include implicit and obscure inputs/outputs.""")
 @click.option("-A", "--all", is_flag=True,
                 help="""Increases level of detail to include all inputs/outputs.""")
 @click.option("-R", "--required", is_flag=True,
                 help="""Decreases level of detail to include required inputs/outputs only.""")
 @click.argument("items", nargs=-1, metavar="filename.yml|cab name|recipe name|...") 
-def help(items: List[str] = [], do_list=False, implicit=False, obscure=False, all=False, required=False):
+def doc(items: List[str] = [], do_list=False, implicit=False, obscure=False, all=False, required=False):
 
     log = logger()
-    top_tree = Tree(f"stimela help {' '.join(items)}", guide_style="dim")
+    top_tree = Tree(f"stimela doc {' '.join(items)}", guide_style="dim")
     found_something = False
     default_recipe = None
 
     if required:
         max_category = ParameterCategory.Required
     else:
         max_category = ParameterCategory.Optional
@@ -122,15 +122,15 @@
         if stimela.CONFIG.lib.recipes:
             subtree = top_tree.add("Recipes:")
             table = Table.grid("", "", padding=(0,2))
             for name, recipe in stimela.CONFIG.lib.recipes.items():
                 table.add_row(f"[bold]{name}[/bold]", recipe.info)
             subtree.add(table)
         elif not do_list and not found_something:
-            log.error(f"nothing particular to help on, perhaps specify a recipe name or a cab name, or use -l/--list")
+            log.error(f"nothing particular to document, please specify a recipe name or a cab name, or use -l/--list")
             sys.exit(2)
 
     if default_recipe and not found_something:
         recipe = load_recipe(name, stimela.CONFIG.lib.recipes[default_recipe])
         tree = top_tree.add(f"Recipe: [bold]{default_recipe}[/bold]")
         recipe.rich_help(tree, max_category=max_category)
```

### Comparing `stimela-2.0rc2/stimela/commands/images.py` & `stimela-2.0rc4/stimela/commands/images.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/commands/ps.py` & `stimela-2.0rc4/stimela/commands/ps.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/commands/pull.py` & `stimela-2.0rc4/stimela/commands/pull.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/commands/push.py` & `stimela-2.0rc4/stimela/commands/push.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/commands/run.py` & `stimela-2.0rc4/stimela/commands/run.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/commands/save_config.py` & `stimela-2.0rc4/stimela/commands/save_config.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/config.py` & `stimela-2.0rc4/stimela/config.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/exceptions.py` & `stimela-2.0rc4/stimela/exceptions.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/kitchen/batch.py` & `stimela-2.0rc4/stimela/kitchen/batch.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/kitchen/cab.py` & `stimela-2.0rc4/stimela/kitchen/cab.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/kitchen/recipe.py` & `stimela-2.0rc4/stimela/kitchen/recipe.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/kitchen/runners.py` & `stimela-2.0rc4/stimela/kitchen/runners.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/kitchen/step.py` & `stimela-2.0rc4/stimela/kitchen/step.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/kitchen/wranglers.py` & `stimela-2.0rc4/stimela/kitchen/wranglers.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/main.py` & `stimela-2.0rc4/stimela/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,28 +12,29 @@
 UID = stimela.UID
 GID = stimela.GID
 LOG_HOME = stimela.LOG_HOME
 LOG_FILE = stimela.LOG_FILE
 
 log = None
 
+_command_aliases = dict(exec="run", help="doc")
+
 class RunExecGroup(click.Group):
     """ Makes the run and exec commands point to the same thing
 
     Args:
         click (_type_): _description_
     """
     def get_command(self, ctx, cmd_name):
         rv = click.Group.get_command(self, ctx, cmd_name)
         if rv is not None:
             return rv
 
-        alias = "exec"
-        if cmd_name == alias :  
-            return click.Group.get_command(self, ctx, "run")
+        if cmd_name in _command_aliases:  
+            return click.Group.get_command(self, ctx, _command_aliases[cmd_name])
         ctx.fail("Uknown command or alias")
 
     def resolve_command(self, ctx, args):
         # always return the full command name
         _, cmd, args = super().resolve_command(ctx, args)
         return cmd.name, cmd, args
 
@@ -117,11 +118,11 @@
     # dump dependencies
     filename = os.path.join(stimelogging.get_logfile_dir(log) or '.', "stimela.config.deps")
     log.info(f"saving config dependencies to {filename}")
     config.CONFIG_DEPS.save(filename)
 
 
 # import commands
-from stimela.commands import run, images, build, push, save_config, help
+from stimela.commands import doc, run, images, build, push, save_config
 
 ## the ones not listed above haven't been converted to click yet. They are:
 # cabs, clean, containers, kill, ps, pull
```

### Comparing `stimela-2.0rc2/stimela/schedulers/slurm.py` & `stimela-2.0rc4/stimela/schedulers/slurm.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/stimelogging.py` & `stimela-2.0rc4/stimela/stimelogging.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/task_stats.py` & `stimela-2.0rc4/stimela/task_stats.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/utils/xrun_asyncio.py` & `stimela-2.0rc4/stimela/utils/xrun_asyncio.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/stimela/utils/xrun_poll.py` & `stimela-2.0rc4/stimela/utils/xrun_poll.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/tests/scabha_tests/test_configuratt.py` & `stimela-2.0rc4/tests/scabha_tests/test_configuratt.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/tests/scabha_tests/test_dynschema.py` & `stimela-2.0rc4/tests/scabha_tests/test_dynschema.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/tests/scabha_tests/test_parsing.py` & `stimela-2.0rc4/tests/scabha_tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/tests/scabha_tests/test_schema.py` & `stimela-2.0rc4/tests/scabha_tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/tests/scabha_tests/test_substitutions.py` & `stimela-2.0rc4/tests/scabha_tests/test_substitutions.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/tests/scabha_tests/testconf.yaml` & `stimela-2.0rc4/tests/scabha_tests/testconf.yaml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/tests/stimela_tests/example_dynschema.py` & `stimela-2.0rc4/tests/stimela_tests/example_dynschema.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/tests/stimela_tests/test_aliasing.yml` & `stimela-2.0rc4/tests/stimela_tests/test_aliasing.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/tests/stimela_tests/test_callables.py` & `stimela-2.0rc4/tests/stimela_tests/test_callables.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/tests/stimela_tests/test_callables.yml` & `stimela-2.0rc4/tests/stimela_tests/test_callables.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/tests/stimela_tests/test_casa.yml` & `stimela-2.0rc4/tests/stimela_tests/test_casa.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/tests/stimela_tests/test_kube.yml` & `stimela-2.0rc4/tests/stimela_tests/test_kube.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/tests/stimela_tests/test_loop_recipe.yml` & `stimela-2.0rc4/tests/stimela_tests/test_loop_recipe.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/tests/stimela_tests/test_loop_recipe_slurm.yml` & `stimela-2.0rc4/tests/stimela_tests/test_loop_recipe_slurm.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/tests/stimela_tests/test_nesting.yml` & `stimela-2.0rc4/tests/stimela_tests/test_nesting.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/tests/stimela_tests/test_recipe.py` & `stimela-2.0rc4/tests/stimela_tests/test_recipe.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/tests/stimela_tests/test_recipe.yml` & `stimela-2.0rc4/tests/stimela_tests/test_recipe.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/tests/stimela_tests/test_scatter.yml` & `stimela-2.0rc4/tests/stimela_tests/test_scatter.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/tests/stimela_tests/test_wranglers.py` & `stimela-2.0rc4/tests/stimela_tests/test_wranglers.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/tests/stimela_tests/test_wranglers.yml` & `stimela-2.0rc4/tests/stimela_tests/test_wranglers.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/tests/stimela_tests/test_xrun.yml` & `stimela-2.0rc4/tests/stimela_tests/test_xrun.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc2/PKG-INFO` & `stimela-2.0rc4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stimela
-Version: 2.0rc2
+Version: 2.0rc4
 Summary: Framework for system agnostic pipelines for radio interferometry arrays
 License: GNU GPL v2
 Author: Sphesihle Makhathini
 Author-email: sphemakh@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

