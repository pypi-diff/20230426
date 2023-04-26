# Comparing `tmp/pymc-5.3.0.tar.gz` & `tmp/pymc-5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pymc-5.3.0.tar", last modified: Fri Apr 14 03:09:00 2023, max compression
+gzip compressed data, was "dist/pymc-5.3.1.tar", last modified: Wed Apr 26 17:34:50 2023, max compression
```

## Comparing `pymc-5.3.0.tar` & `pymc-5.3.1.tar`

### file list

```diff
@@ -1,133 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:09:00.000000 pymc-5.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-04-14 03:08:48.000000 pymc-5.3.0/ARCHITECTURE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-14 03:08:48.000000 pymc-5.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-14 03:08:48.000000 pymc-5.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    42347 2023-04-14 03:08:48.000000 pymc-5.3.0/GOVERNANCE.md
--rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-04-14 03:08:48.000000 pymc-5.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-14 03:08:48.000000 pymc-5.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-04-14 03:09:00.000000 pymc-5.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-04-14 03:08:48.000000 pymc-5.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    81106 2023-04-14 03:08:48.000000 pymc-5.3.0/RELEASE-NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:09:00.000000 pymc-5.3.0/pymc/
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-14 03:09:00.000000 pymc-5.3.0/pymc/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:09:00.000000 pymc-5.3.0/pymc/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21384 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/backends/arviz.py
--rw-r--r--   0 runner    (1001) docker     (123)    19523 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/backends/mcbackend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/backends/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/backends/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/blocking.py
--rw-r--r--   0 runner    (1001) docker     (123)    16472 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:09:00.000000 pymc-5.3.0/pymc/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/distributions/bound.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/distributions/censored.py
--rw-r--r--   0 runner    (1001) docker     (123)   115522 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/distributions/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)    51737 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/distributions/discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)    15229 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/distributions/dist_math.py
--rw-r--r--   0 runner    (1001) docker     (123)    39675 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/distributions/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    20940 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/distributions/mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)    89379 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/distributions/multivariate.py
--rw-r--r--   0 runner    (1001) docker     (123)    18230 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/distributions/shape_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12907 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/distributions/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    39568 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/distributions/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/distributions/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/distributions/truncated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/func_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:09:00.000000 pymc-5.3.0/pymc/gp/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/gp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32077 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/gp/cov.py
--rw-r--r--   0 runner    (1001) docker     (123)    49754 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/gp/gp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14494 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/gp/hsgp_approx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/gp/mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/gp/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11097 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/initial_point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:09:00.000000 pymc-5.3.0/pymc/logprob/
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/logprob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/logprob/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    14276 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/logprob/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/logprob/censoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/logprob/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/logprob/cumsum.py
--rw-r--r--   0 runner    (1001) docker     (123)    20564 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/logprob/mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/logprob/rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)    24280 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/logprob/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/logprob/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    34745 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/logprob/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/logprob/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15013 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    90137 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/model_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:09:00.000000 pymc-5.3.0/pymc/ode/
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/ode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9655 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/ode/ode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/ode/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:09:00.000000 pymc-5.3.0/pymc/plots/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/printing.py
--rw-r--r--   0 runner    (1001) docker     (123)    37227 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/pytensorf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:09:00.000000 pymc-5.3.0/pymc/sampling/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29781 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/sampling/forward.py
--rw-r--r--   0 runner    (1001) docker     (123)    25904 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/sampling/jax.py
--rw-r--r--   0 runner    (1001) docker     (123)    48752 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/sampling/mcmc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15597 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/sampling/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    15009 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/sampling/population.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/sampling_jax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:09:00.000000 pymc-5.3.0/pymc/smc/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/smc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24432 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/smc/kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)    14866 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/smc/sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:09:00.000000 pymc-5.3.0/pymc/stats/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/stats/convergence.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/stats/log_likelihood.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:09:00.000000 pymc-5.3.0/pymc/step_methods/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/step_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/step_methods/arraystep.py
--rw-r--r--   0 runner    (1001) docker     (123)    10623 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/step_methods/compound.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:09:00.000000 pymc-5.3.0/pymc/step_methods/hmc/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/step_methods/hmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/step_methods/hmc/base_hmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/step_methods/hmc/hmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/step_methods/hmc/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    17591 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/step_methods/hmc/nuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    27526 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/step_methods/hmc/quadpotential.py
--rw-r--r--   0 runner    (1001) docker     (123)    35693 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/step_methods/metropolis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/step_methods/slicer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/step_methods/step_sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)    36397 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:09:00.000000 pymc-5.3.0/pymc/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/tuning/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/tuning/starting.py
--rw-r--r--   0 runner    (1001) docker     (123)    16744 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:09:00.000000 pymc-5.3.0/pymc/variational/
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/variational/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13163 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/variational/approximations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/variational/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    28608 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/variational/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/variational/minibatch_rv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/variational/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    57336 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/variational/opvi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/variational/stein.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/variational/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    37930 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/variational/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/vartypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:09:00.000000 pymc-5.3.0/pymc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-04-14 03:08:59.000000 pymc-5.3.0/pymc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-14 03:08:59.000000 pymc-5.3.0/pymc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 03:08:59.000000 pymc-5.3.0/pymc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-14 03:08:59.000000 pymc-5.3.0/pymc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-14 03:08:59.000000 pymc-5.3.0/pymc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-14 03:08:48.000000 pymc-5.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-14 03:08:48.000000 pymc-5.3.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:09:00.000000 pymc-5.3.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      833 2023-04-14 03:08:48.000000 pymc-5.3.0/scripts/docker_container.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      181 2023-04-14 03:08:48.000000 pymc-5.3.0/scripts/test.sh
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-14 03:09:00.000000 pymc-5.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2698 2023-04-14 03:08:48.000000 pymc-5.3.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    81282 2023-04-14 03:08:48.000000 pymc-5.3.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:34:50.000000 pymc-5.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-04-26 17:34:28.000000 pymc-5.3.1/ARCHITECTURE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-26 17:34:28.000000 pymc-5.3.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-26 17:34:28.000000 pymc-5.3.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    42347 2023-04-26 17:34:28.000000 pymc-5.3.1/GOVERNANCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-04-26 17:34:28.000000 pymc-5.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-26 17:34:28.000000 pymc-5.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-04-26 17:34:50.000000 pymc-5.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-04-26 17:34:28.000000 pymc-5.3.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    81106 2023-04-26 17:34:28.000000 pymc-5.3.1/RELEASE-NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21384 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/backends/arviz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19523 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/backends/mcbackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/backends/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/backends/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/blocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16472 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/distributions/bound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/distributions/censored.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115522 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/distributions/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51737 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/distributions/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15229 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/distributions/dist_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39317 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/distributions/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20940 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/distributions/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89379 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/distributions/multivariate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18230 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/distributions/shape_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/distributions/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39568 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/distributions/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/distributions/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/distributions/truncated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/func_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc/gp/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/gp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32081 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/gp/cov.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49766 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/gp/gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14494 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/gp/hsgp_approx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/gp/mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/gp/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11097 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/initial_point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc/logprob/
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/logprob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/logprob/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14276 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/logprob/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/logprob/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/logprob/censoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/logprob/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/logprob/cumsum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20564 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/logprob/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/logprob/rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24280 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/logprob/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/logprob/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34442 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/logprob/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11557 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/logprob/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15013 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90135 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/model_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc/ode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/ode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9655 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/ode/ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/ode/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37227 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/pytensorf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc/sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29781 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/sampling/forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25904 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/sampling/jax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48752 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/sampling/mcmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15597 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/sampling/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15009 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/sampling/population.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/sampling_jax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc/smc/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/smc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24432 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/smc/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14866 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/smc/sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/stats/convergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/stats/log_likelihood.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc/step_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/step_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/step_methods/arraystep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10623 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/step_methods/compound.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc/step_methods/hmc/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/step_methods/hmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/step_methods/hmc/base_hmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/step_methods/hmc/hmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/step_methods/hmc/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17591 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/step_methods/hmc/nuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27526 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/step_methods/hmc/quadpotential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35731 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/step_methods/metropolis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/step_methods/slicer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/step_methods/step_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36397 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/tuning/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/tuning/starting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16744 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc/variational/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/variational/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13163 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/variational/approximations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/variational/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28608 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/variational/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/variational/minibatch_rv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/variational/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57336 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/variational/opvi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/variational/stein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/variational/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37930 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/variational/updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/vartypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-26 17:34:28.000000 pymc-5.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-26 17:34:28.000000 pymc-5.3.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:34:50.000000 pymc-5.3.1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      833 2023-04-26 17:34:28.000000 pymc-5.3.1/scripts/docker_container.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      181 2023-04-26 17:34:28.000000 pymc-5.3.1/scripts/test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-26 17:34:50.000000 pymc-5.3.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2698 2023-04-26 17:34:28.000000 pymc-5.3.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81282 2023-04-26 17:34:28.000000 pymc-5.3.1/versioneer.py
```

### Comparing `pymc-5.3.0/ARCHITECTURE.md` & `pymc-5.3.1/ARCHITECTURE.md`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/CODE_OF_CONDUCT.md` & `pymc-5.3.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/CONTRIBUTING.md` & `pymc-5.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/GOVERNANCE.md` & `pymc-5.3.1/GOVERNANCE.md`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/LICENSE` & `pymc-5.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/PKG-INFO` & `pymc-5.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc
-Version: 5.3.0
+Version: 5.3.1
 Summary: Probabilistic Programming in Python: Bayesian Modeling and Probabilistic Machine Learning with PyTensor
 Home-page: http://github.com/pymc-devs/pymc
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Description: .. image:: https://cdn.rawgit.com/pymc-devs/pymc/main/docs/logos/svg/PyMC_banner.svg
             :height: 100px
```

### Comparing `pymc-5.3.0/README.rst` & `pymc-5.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/RELEASE-NOTES.md` & `pymc-5.3.1/RELEASE-NOTES.md`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/__init__.py` & `pymc-5.3.1/pymc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/backends/__init__.py` & `pymc-5.3.1/pymc/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/backends/arviz.py` & `pymc-5.3.1/pymc/backends/arviz.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/backends/base.py` & `pymc-5.3.1/pymc/backends/base.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/backends/mcbackend.py` & `pymc-5.3.1/pymc/backends/mcbackend.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/backends/ndarray.py` & `pymc-5.3.1/pymc/backends/ndarray.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/backends/report.py` & `pymc-5.3.1/pymc/backends/report.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/blocking.py` & `pymc-5.3.1/pymc/blocking.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/data.py` & `pymc-5.3.1/pymc/data.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/distributions/__init__.py` & `pymc-5.3.1/pymc/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/distributions/bound.py` & `pymc-5.3.1/pymc/distributions/bound.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/distributions/censored.py` & `pymc-5.3.1/pymc/distributions/censored.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/distributions/continuous.py` & `pymc-5.3.1/pymc/distributions/continuous.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/distributions/discrete.py` & `pymc-5.3.1/pymc/distributions/discrete.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/distributions/dist_math.py` & `pymc-5.3.1/pymc/distributions/dist_math.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/distributions/distribution.py` & `pymc-5.3.1/pymc/distributions/distribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -484,22 +484,22 @@
 
     rv_type = CustomDistRV
 
     @classmethod
     def dist(
         cls,
         *dist_params,
-        class_name: str,
         logp: Optional[Callable] = None,
         logcdf: Optional[Callable] = None,
         random: Optional[Callable] = None,
         moment: Optional[Callable] = None,
         ndim_supp: int = 0,
         ndims_params: Optional[Sequence[int]] = None,
         dtype: str = "floatX",
+        class_name: str = "CustomDist",
         **kwargs,
     ):
         dist_params = [as_tensor_variable(param) for param in dist_params]
 
         # Assume scalar ndims_params
         if ndims_params is None:
             ndims_params = [0] * len(dist_params)
@@ -519,44 +519,44 @@
             )
 
         if random is None:
             random = default_not_implemented(class_name, "random")
 
         return super().dist(
             dist_params,
-            class_name=class_name,
             logp=logp,
             logcdf=logcdf,
             random=random,
             moment=moment,
             ndim_supp=ndim_supp,
             ndims_params=ndims_params,
             dtype=dtype,
+            class_name=class_name,
             **kwargs,
         )
 
     @classmethod
     def rv_op(
         cls,
         *dist_params,
-        class_name: str,
         logp: Optional[Callable],
         logcdf: Optional[Callable],
         random: Optional[Callable],
         moment: Optional[Callable],
         ndim_supp: int,
         ndims_params: Optional[Sequence[int]],
         dtype: str,
+        class_name: str,
         **kwargs,
     ):
         rv_type = type(
-            f"CustomDistRV_{class_name}",
+            class_name,
             (CustomDistRV,),
             dict(
-                name=f"CustomDist_{class_name}",
+                name=class_name,
                 inplace=False,
                 ndim_supp=ndim_supp,
                 ndims_params=ndims_params,
                 dtype=dtype,
                 # Specific to CustomDist
                 _random_fn=random,
             ),
@@ -609,28 +609,23 @@
 class _CustomSymbolicDist(Distribution):
     rv_type = CustomSymbolicDistRV
 
     @classmethod
     def dist(
         cls,
         *dist_params,
-        class_name: str,
         dist: Callable,
         logp: Optional[Callable] = None,
         logcdf: Optional[Callable] = None,
         moment: Optional[Callable] = None,
         ndim_supp: int = 0,
         dtype: str = "floatX",
+        class_name: str = "CustomSymbolicDist",
         **kwargs,
     ):
-        warnings.warn(
-            "CustomDist with dist function is still experimental. Expect bugs!",
-            UserWarning,
-        )
-
         dist_params = [as_tensor_variable(param) for param in dist_params]
 
         if logcdf is None:
             logcdf = default_not_implemented(class_name, "logcdf")
 
         if moment is None:
             moment = functools.partial(
@@ -651,51 +646,53 @@
             **kwargs,
         )
 
     @classmethod
     def rv_op(
         cls,
         *dist_params,
-        class_name: str,
         dist: Callable,
         logp: Optional[Callable],
         logcdf: Optional[Callable],
         moment: Optional[Callable],
         size=None,
         ndim_supp: int,
+        class_name: str,
     ):
         size = normalize_size_param(size)
         dummy_size_param = size.type()
         dummy_dist_params = [dist_param.type() for dist_param in dist_params]
         with BlockModelAccess(
             error_msg_on_access="Model variables cannot be created in the dist function. Use the `.dist` API"
         ):
             dummy_rv = dist(*dummy_dist_params, dummy_size_param)
         dummy_params = [dummy_size_param] + dummy_dist_params
         dummy_updates_dict = collect_default_updates(dummy_params, (dummy_rv,))
 
         rv_type = type(
-            f"CustomSymbolicDistRV_{class_name}",
+            class_name,
             (CustomSymbolicDistRV,),
             # If logp is not provided, we try to infer it from the dist graph
             dict(
                 inline_logprob=logp is None,
             ),
         )
 
         # Dispatch custom methods
         if logp is not None:
 
             @_logprob.register(rv_type)
             def custom_dist_logp(op, values, size, *params, **kwargs):
                 return logp(values[0], *params[: len(dist_params)])
 
-        @_logcdf.register(rv_type)
-        def custom_dist_logcdf(op, value, size, *params, **kwargs):
-            return logcdf(value, *params[: len(dist_params)])
+        if logcdf is not None:
+
+            @_logcdf.register(rv_type)
+            def custom_dist_logcdf(op, value, size, *params, **kwargs):
+                return logcdf(value, *params[: len(dist_params)])
 
         @_moment.register(rv_type)
         def custom_dist_get_moment(op, rv, size, *params):
             return moment(rv, size, *params[: len(params)])
 
         @_change_dist_size.register(rv_type)
         def change_custom_symbolic_dist_size(op, rv, new_size, expand):
@@ -754,23 +751,14 @@
 
     Parameters
     ----------
     name : str
     dist_params : Tuple
         A sequence of the distribution's parameter. These will be converted into
         Pytensor tensor variables internally.
-    class_name : str
-        Name for the class which will wrap the CustomDist methods. When not specified,
-        it will be given the name of the model variable.
-
-        .. warning:: New CustomDists created with the same class_name will override the
-            methods dispatched onto the previous classes. If using CustomDists with
-            different methods across separate models, be sure to use distinct
-            class_names.
-
     dist: Optional[Callable]
         A callable that returns a PyTensor graph built from simpler PyMC distributions
         which represents the distribution. This can be used by PyMC to take random draws
         as well as to infer the logp of the distribution in some cases. In that case
         it's not necessary to implement ``random`` or ``logp`` functions.
 
         It must have the following signature: ``dist(*dist_params, size)``.
@@ -827,14 +815,17 @@
         parameters. If ``None``, it is assumed that all parameters are scalars, hence
         the number of dimensions of their support will be 0. This is not needed if an
         PyTensor dist function is provided.
     dtype : str
         The dtype of the distribution. All draws and observations passed into the
         distribution will be cast onto this dtype. This is not needed if an PyTensor
         dist function is provided, which should already return the right dtype!
+    class_name : str
+        Name for the class which will wrap the CustomDist methods. When not specified,
+        it will be given the name of the model variable.
     kwargs :
         Extra keyword arguments are passed to the parent's class ``__new__`` method.
 
 
     Examples
     --------
     Create a CustomDist that wraps a black-box logp function. This variable cannot be
@@ -975,44 +966,44 @@
                 " Previous versions allowed passing distribution parameters as"
                 " a dictionary in ``observed``, in the current version these "
                 "parameters are positional arguments."
             )
         dist_params = cls.parse_dist_params(dist_params)
         cls.check_valid_dist_random(dist, random, dist_params)
         if dist is not None:
+            kwargs.setdefault("class_name", f"CustomSymbolicDist_{name}")
             return _CustomSymbolicDist(
                 name,
                 *dist_params,
-                class_name=name,
                 dist=dist,
                 logp=logp,
                 logcdf=logcdf,
                 moment=moment,
                 ndim_supp=ndim_supp,
                 **kwargs,
             )
-        return _CustomDist(
-            name,
-            *dist_params,
-            class_name=name,
-            random=random,
-            logp=logp,
-            logcdf=logcdf,
-            moment=moment,
-            ndim_supp=ndim_supp,
-            ndims_params=ndims_params,
-            dtype=dtype,
-            **kwargs,
-        )
+        else:
+            kwargs.setdefault("class_name", f"CustomDist_{name}")
+            return _CustomDist(
+                name,
+                *dist_params,
+                random=random,
+                logp=logp,
+                logcdf=logcdf,
+                moment=moment,
+                ndim_supp=ndim_supp,
+                ndims_params=ndims_params,
+                dtype=dtype,
+                **kwargs,
+            )
 
     @classmethod
     def dist(
         cls,
         *dist_params,
-        class_name: str,
         dist: Optional[Callable] = None,
         random: Optional[Callable] = None,
         logp: Optional[Callable] = None,
         logcdf: Optional[Callable] = None,
         moment: Optional[Callable] = None,
         ndim_supp: int = 0,
         ndims_params: Optional[Sequence[int]] = None,
@@ -1020,26 +1011,24 @@
         **kwargs,
     ):
         dist_params = cls.parse_dist_params(dist_params)
         cls.check_valid_dist_random(dist, random, dist_params)
         if dist is not None:
             return _CustomSymbolicDist.dist(
                 *dist_params,
-                class_name=class_name,
                 dist=dist,
                 logp=logp,
                 logcdf=logcdf,
                 moment=moment,
                 ndim_supp=ndim_supp,
                 **kwargs,
             )
         else:
             return _CustomDist.dist(
                 *dist_params,
-                class_name=class_name,
                 random=random,
                 logp=logp,
                 logcdf=logcdf,
                 moment=moment,
                 ndim_supp=ndim_supp,
                 ndims_params=ndims_params,
                 dtype=dtype,
```

### Comparing `pymc-5.3.0/pymc/distributions/mixture.py` & `pymc-5.3.1/pymc/distributions/mixture.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/distributions/multivariate.py` & `pymc-5.3.1/pymc/distributions/multivariate.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/distributions/shape_utils.py` & `pymc-5.3.1/pymc/distributions/shape_utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/distributions/simulator.py` & `pymc-5.3.1/pymc/distributions/simulator.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,23 +82,14 @@
         Parameters used by the Simulator random function. Each parameter can be passed
         by order after fn, for example ``param1, param2, ..., paramN``. params can also
         be passed with keyword argument "params".
     params : list of TensorVariable
         Keyword form of ''unnamed_params''.
         One of unnamed_params or params must be provided.
         If passed both unnamed_params and params, an error is raised.
-    class_name : str
-        Name for the RandomVariable class which will wrap the Simulator methods.
-        When not specified, it will be given the name of the variable.
-
-        .. warning:: New Simulators created with the same class_name will override the
-            methods dispatched onto the previous classes. If using Simulators with
-            different methods across separate models, be sure to use distinct
-            class_names.
-
     distance : PyTensor_Op, callable or str, default "gaussian"
         Distance function. Available options are ``"gaussian"``, ``"laplace"``,
         ``"kullback_leibler"`` or a user defined function (or PyTensor_Op) that takes
         ``epsilon``, the summary statistics of observed_data and the summary statistics
         of simulated_data as input.
 
         ``gaussian``: :math:`-0.5 \left(\left(\frac{xo - xs}{\epsilon}\right)^2\right)`
@@ -119,14 +110,16 @@
         an array of the same size of the output of ``sum_stat``.
     ndim_supp : int, default 0
         Number of dimensions of the SimulatorRV (0 for scalar, 1 for vector, etc.)
     ndims_params : list of int, optional
         Number of minimum dimensions of each parameter of the RV. For example,
         if the Simulator accepts two scalar inputs, it should be ``[0, 0]``.
         Default to list of 0 with length equal to the number of parameters.
+    class_name : str, optional
+        Suffix name for the RandomVariable class which will wrap the Simulator methods.
 
     Examples
     --------
     .. code-block:: python
 
         def simulator_fn(rng, loc, scale, size):
             return rng.normal(loc, scale, size=size)
@@ -145,30 +138,30 @@
         `link <https://ieeexplore.ieee.org/document/4595271>`__
 
     """
 
     rv_type = SimulatorRV
 
     def __new__(cls, name, *args, **kwargs):
-        kwargs.setdefault("class_name", name)
+        kwargs.setdefault("class_name", f"Simulator_{name}")
         return super().__new__(cls, name, *args, **kwargs)
 
     @classmethod
     def dist(  # type: ignore
         cls,
         fn,
         *unnamed_params,
         params=None,
-        class_name: str,
         distance="gaussian",
         sum_stat="identity",
         epsilon=1,
         ndim_supp=0,
         ndims_params=None,
         dtype="floatX",
+        class_name: str = "Simulator",
         **kwargs,
     ):
         if not isinstance(distance, Op):
             if distance == "gaussian":
                 distance = gaussian
             elif distance == "laplace":
                 distance = laplace
@@ -209,44 +202,44 @@
 
         # Assume scalar ndims_params
         if ndims_params is None:
             ndims_params = [0] * len(params)
 
         return super().dist(
             params,
-            class_name=class_name,
             fn=fn,
             ndim_supp=ndim_supp,
             ndims_params=ndims_params,
             dtype=dtype,
             distance=distance,
             sum_stat=sum_stat,
             epsilon=epsilon,
+            class_name=class_name,
             **kwargs,
         )
 
     @classmethod
     def rv_op(
         cls,
         *params,
-        class_name,
         fn,
         ndim_supp,
         ndims_params,
         dtype,
         distance,
         sum_stat,
         epsilon,
+        class_name,
         **kwargs,
     ):
         sim_op = type(
-            f"Simulator_{class_name}",
+            class_name,
             (SimulatorRV,),
             dict(
-                name=f"Simulator_{class_name}",
+                name=class_name,
                 ndim_supp=ndim_supp,
                 ndims_params=ndims_params,
                 dtype=dtype,
                 inplace=False,
                 fn=fn,
                 _distance=distance,
                 _sum_stat=sum_stat,
```

### Comparing `pymc-5.3.0/pymc/distributions/timeseries.py` & `pymc-5.3.1/pymc/distributions/timeseries.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/distributions/transforms.py` & `pymc-5.3.1/pymc/distributions/transforms.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/distributions/truncated.py` & `pymc-5.3.1/pymc/distributions/truncated.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/exceptions.py` & `pymc-5.3.1/pymc/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/func_utils.py` & `pymc-5.3.1/pymc/func_utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/gp/__init__.py` & `pymc-5.3.1/pymc/gp/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/gp/cov.py` & `pymc-5.3.1/pymc/gp/cov.py`

 * *Files 0% similar despite different names*

```diff
@@ -382,15 +382,15 @@
     def full(self, X, Xs=None):
         if Xs is None:
             return pt.alloc(self.c, X.shape[0], X.shape[0])
         else:
             return pt.alloc(self.c, X.shape[0], Xs.shape[0])
 
 
-class WhiteNoise(Covariance):
+class WhiteNoise(BaseCovariance):
     r"""
     White noise covariance function.
 
     .. math::
 
        k(x, x') = \sigma^2 \mathrm{I}
     """
```

### Comparing `pymc-5.3.0/pymc/gp/gp.py` & `pymc-5.3.1/pymc/gp/gp.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import numpy as np
 import pytensor.tensor as pt
 
 from pytensor.tensor.nlinalg import eigh
 
 import pymc as pm
 
-from pymc.gp.cov import Constant, Covariance
+from pymc.gp.cov import BaseCovariance, Constant
 from pymc.gp.mean import Zero
 from pymc.gp.util import (
     JITTER_DEFAULT,
     cholesky,
     conditioned_vars,
     replace_with_values,
     solve_lower,
@@ -479,15 +479,15 @@
             Deprecated. Whether to set `y` as an `observed` variable in the `model`.
         **kwargs
             Extra keyword arguments that are passed to :class:`~pymc.MvNormal` distribution
             constructor.
         """
         sigma = _handle_sigma_noise_parameters(sigma=sigma, noise=noise)
 
-        noise_func = sigma if isinstance(sigma, Covariance) else pm.gp.cov.WhiteNoise(sigma)
+        noise_func = sigma if isinstance(sigma, BaseCovariance) else pm.gp.cov.WhiteNoise(sigma)
         mu, cov = self._build_marginal_likelihood(X=X, noise_func=noise_func, jitter=jitter)
         self.X = X
         self.y = y
         self.sigma = noise_func
         if is_observed:
             return pm.MvNormal(name, mu=mu, cov=cov, observed=y, **kwargs)
         else:
@@ -511,15 +511,15 @@
 
         if "noise" in given:
             warnings.warn(_noise_deprecation_warning, FutureWarning)
             given["sigma"] = given["noise"]
 
         if all(val in given for val in ["X", "y", "sigma"]):
             X, y, sigma = given["X"], given["y"], given["sigma"]
-            noise_func = sigma if isinstance(sigma, Covariance) else pm.gp.cov.WhiteNoise(sigma)
+            noise_func = sigma if isinstance(sigma, BaseCovariance) else pm.gp.cov.WhiteNoise(sigma)
         else:
             X, y, noise_func = self.X, self.y, self.sigma
         return X, y, noise_func, cov_total, mean_total
 
     def _build_conditional(
         self, Xnew, pred_noise, diag, X, y, noise_func, cov_total, mean_total, jitter
     ):
```

### Comparing `pymc-5.3.0/pymc/gp/hsgp_approx.py` & `pymc-5.3.1/pymc/gp/hsgp_approx.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/gp/mean.py` & `pymc-5.3.1/pymc/gp/mean.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/gp/util.py` & `pymc-5.3.1/pymc/gp/util.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/initial_point.py` & `pymc-5.3.1/pymc/initial_point.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/logprob/__init__.py` & `pymc-5.3.1/pymc/logprob/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 #   OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #   SOFTWARE.
 
 from pymc.logprob.basic import factorized_joint_logprob, icdf, joint_logp, logcdf, logp
 
 # isort: off
 # Add rewrites to the DBs
+import pymc.logprob.binary
 import pymc.logprob.censoring
 import pymc.logprob.cumsum
 import pymc.logprob.checks
 import pymc.logprob.mixture
 import pymc.logprob.scan
 import pymc.logprob.tensor
 import pymc.logprob.transforms
```

### Comparing `pymc-5.3.0/pymc/logprob/abstract.py` & `pymc-5.3.1/pymc/logprob/abstract.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/logprob/basic.py` & `pymc-5.3.1/pymc/logprob/basic.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/logprob/censoring.py` & `pymc-5.3.1/pymc/logprob/censoring.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/logprob/checks.py` & `pymc-5.3.1/pymc/logprob/checks.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/logprob/cumsum.py` & `pymc-5.3.1/pymc/logprob/cumsum.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/logprob/mixture.py` & `pymc-5.3.1/pymc/logprob/mixture.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/logprob/rewriting.py` & `pymc-5.3.1/pymc/logprob/rewriting.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/logprob/scan.py` & `pymc-5.3.1/pymc/logprob/scan.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/logprob/tensor.py` & `pymc-5.3.1/pymc/logprob/tensor.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/logprob/transforms.py` & `pymc-5.3.1/pymc/logprob/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     _icdf_helper,
     _logcdf,
     _logcdf_helper,
     _logprob,
     _logprob_helper,
 )
 from pymc.logprob.rewriting import PreserveRVMappings, measurable_ir_rewrites_db
-from pymc.logprob.utils import ignore_logprob, walk_model
+from pymc.logprob.utils import check_potential_measurability, ignore_logprob
 
 
 class TransformedVariable(Op):
     """A no-op that identifies a transform and its un-transformed input."""
 
     view_map = {0: [0]}
 
@@ -569,27 +569,16 @@
     # Do not apply rewrite to discrete variables
     if measurable_input.type.dtype.startswith("int"):
         return None
 
     # Check that other inputs are not potentially measurable, in which case this rewrite
     # would be invalid
     other_inputs = tuple(inp for inp in node.inputs if inp is not measurable_input)
-    if any(
-        ancestor_node
-        for ancestor_node in walk_model(
-            other_inputs,
-            walk_past_rvs=False,
-            stop_at_vars=set(rv_map_feature.rv_values),
-        )
-        if (
-            ancestor_node.owner
-            and isinstance(ancestor_node.owner.op, MeasurableVariable)
-            and ancestor_node not in rv_map_feature.rv_values
-        )
-    ):
+
+    if not check_potential_measurability(other_inputs, rv_map_feature):
         return None
 
     # Make base_measure outputs unmeasurable
     # This seems to be the only thing preventing nested rewrites from being erased
     measurable_input = ignore_logprob(measurable_input)
 
     scalar_op = node.op.scalar_op
```

### Comparing `pymc-5.3.0/pymc/logprob/utils.py` & `pymc-5.3.1/pymc/logprob/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,14 +206,32 @@
 def indices_from_subtensor(idx_list, indices):
     """Compute a useable index tuple from the inputs of a ``*Subtensor**`` ``Op``."""
     return tuple(
         tuple(convert_indices(list(indices), idx) for idx in idx_list) if idx_list else indices
     )
 
 
+def check_potential_measurability(inputs: Tuple[TensorVariable], rv_map_feature):
+    if any(
+        ancestor_node
+        for ancestor_node in walk_model(
+            inputs,
+            walk_past_rvs=False,
+            stop_at_vars=set(rv_map_feature.rv_values),
+        )
+        if (
+            ancestor_node.owner
+            and isinstance(ancestor_node.owner.op, MeasurableVariable)
+            and ancestor_node not in rv_map_feature.rv_values
+        )
+    ):
+        return None
+    return True
+
+
 class ParameterValueError(ValueError):
     """Exception for invalid parameters values in logprob graphs"""
 
 
 class CheckParameterValue(CheckAndRaise):
     """Implements a parameter value check in a logprob graph.
```

### Comparing `pymc-5.3.0/pymc/math.py` & `pymc-5.3.1/pymc/math.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/model.py` & `pymc-5.3.1/pymc/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1151,15 +1151,15 @@
             initval = rv_var.type.filter(initval)
 
         self.rvs_to_initial_values[rv_var] = initval
 
     def set_data(
         self,
         name: str,
-        values: Dict[str, Optional[Sequence]],
+        values: Union[Sequence, np.ndarray],
         coords: Optional[Dict[str, Sequence]] = None,
     ):
         """Changes the values of a data variable in the model.
 
         In contrast to pm.MutableData().set_value, this method can also
         update the corresponding coordinates.
```

### Comparing `pymc-5.3.0/pymc/model_graph.py` & `pymc-5.3.1/pymc/model_graph.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/ode/__init__.py` & `pymc-5.3.1/pymc/ode/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/ode/ode.py` & `pymc-5.3.1/pymc/ode/ode.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/ode/utils.py` & `pymc-5.3.1/pymc/ode/utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/plots/__init__.py` & `pymc-5.3.1/pymc/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/printing.py` & `pymc-5.3.1/pymc/printing.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/pytensorf.py` & `pymc-5.3.1/pymc/pytensorf.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/sampling/__init__.py` & `pymc-5.3.1/pymc/sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/sampling/forward.py` & `pymc-5.3.1/pymc/sampling/forward.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/sampling/jax.py` & `pymc-5.3.1/pymc/sampling/jax.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/sampling/mcmc.py` & `pymc-5.3.1/pymc/sampling/mcmc.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/sampling/parallel.py` & `pymc-5.3.1/pymc/sampling/parallel.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/sampling/population.py` & `pymc-5.3.1/pymc/sampling/population.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/sampling_jax.py` & `pymc-5.3.1/pymc/sampling_jax.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/smc/__init__.py` & `pymc-5.3.1/pymc/smc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/smc/kernels.py` & `pymc-5.3.1/pymc/smc/kernels.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/smc/sampling.py` & `pymc-5.3.1/pymc/smc/sampling.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/stats/__init__.py` & `pymc-5.3.1/pymc/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/stats/convergence.py` & `pymc-5.3.1/pymc/stats/convergence.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/stats/log_likelihood.py` & `pymc-5.3.1/pymc/stats/log_likelihood.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/step_methods/__init__.py` & `pymc-5.3.1/pymc/step_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/step_methods/arraystep.py` & `pymc-5.3.1/pymc/step_methods/arraystep.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/step_methods/compound.py` & `pymc-5.3.1/pymc/step_methods/compound.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/step_methods/hmc/__init__.py` & `pymc-5.3.1/pymc/step_methods/hmc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/step_methods/hmc/base_hmc.py` & `pymc-5.3.1/pymc/step_methods/hmc/base_hmc.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/step_methods/hmc/hmc.py` & `pymc-5.3.1/pymc/step_methods/hmc/hmc.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/step_methods/hmc/integration.py` & `pymc-5.3.1/pymc/step_methods/hmc/integration.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/step_methods/hmc/nuts.py` & `pymc-5.3.1/pymc/step_methods/hmc/nuts.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/step_methods/hmc/quadpotential.py` & `pymc-5.3.1/pymc/step_methods/hmc/quadpotential.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/step_methods/metropolis.py` & `pymc-5.3.1/pymc/step_methods/metropolis.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,22 +253,23 @@
             else:
                 delta[self.discrete] = np.round(delta[self.discrete], 0)
                 q = q0d + delta
         else:
             q = floatX(q0d + delta)
 
         if self.elemwise_update:
+            q0d = q0d.copy()
             q_temp = q0d.copy()
             # Shuffle order of updates (probably we don't need to do this in every step)
             np.random.shuffle(self.enum_dims)
             for i in self.enum_dims:
                 q_temp[i] = q[i]
                 accept_rate_i = self.delta_logp(q_temp, q0d)
                 q_temp_, accepted_i = metrop_select(accept_rate_i, q_temp, q0d)
-                q_temp[i] = q_temp_[i]
+                q_temp[i] = q0d[i] = q_temp_[i]
                 self.accept_rate_iter[i] = accept_rate_i
                 self.accepted_iter[i] = accepted_i
                 self.accepted_sum[i] += accepted_i
             q = q_temp
         else:
             accept_rate = self.delta_logp(q, q0d)
             q, accepted = metrop_select(accept_rate, q, q0d)
```

### Comparing `pymc-5.3.0/pymc/step_methods/slicer.py` & `pymc-5.3.1/pymc/step_methods/slicer.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/step_methods/step_sizes.py` & `pymc-5.3.1/pymc/step_methods/step_sizes.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/testing.py` & `pymc-5.3.1/pymc/testing.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/tuning/__init__.py` & `pymc-5.3.1/pymc/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/tuning/scaling.py` & `pymc-5.3.1/pymc/tuning/scaling.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/tuning/starting.py` & `pymc-5.3.1/pymc/tuning/starting.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/util.py` & `pymc-5.3.1/pymc/util.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/variational/__init__.py` & `pymc-5.3.1/pymc/variational/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/variational/approximations.py` & `pymc-5.3.1/pymc/variational/approximations.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/variational/callbacks.py` & `pymc-5.3.1/pymc/variational/callbacks.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/variational/inference.py` & `pymc-5.3.1/pymc/variational/inference.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/variational/minibatch_rv.py` & `pymc-5.3.1/pymc/variational/minibatch_rv.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/variational/operators.py` & `pymc-5.3.1/pymc/variational/operators.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/variational/opvi.py` & `pymc-5.3.1/pymc/variational/opvi.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/variational/stein.py` & `pymc-5.3.1/pymc/variational/stein.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/variational/test_functions.py` & `pymc-5.3.1/pymc/variational/test_functions.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/variational/updates.py` & `pymc-5.3.1/pymc/variational/updates.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc/vartypes.py` & `pymc-5.3.1/pymc/vartypes.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/pymc.egg-info/PKG-INFO` & `pymc-5.3.1/pymc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc
-Version: 5.3.0
+Version: 5.3.1
 Summary: Probabilistic Programming in Python: Bayesian Modeling and Probabilistic Machine Learning with PyTensor
 Home-page: http://github.com/pymc-devs/pymc
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Description: .. image:: https://cdn.rawgit.com/pymc-devs/pymc/main/docs/logos/svg/PyMC_banner.svg
             :height: 100px
```

### Comparing `pymc-5.3.0/pymc.egg-info/SOURCES.txt` & `pymc-5.3.1/pymc.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 pymc/gp/gp.py
 pymc/gp/hsgp_approx.py
 pymc/gp/mean.py
 pymc/gp/util.py
 pymc/logprob/__init__.py
 pymc/logprob/abstract.py
 pymc/logprob/basic.py
+pymc/logprob/binary.py
 pymc/logprob/censoring.py
 pymc/logprob/checks.py
 pymc/logprob/cumsum.py
 pymc/logprob/mixture.py
 pymc/logprob/rewriting.py
 pymc/logprob/scan.py
 pymc/logprob/tensor.py
```

### Comparing `pymc-5.3.0/scripts/docker_container.sh` & `pymc-5.3.1/scripts/docker_container.sh`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/setup.py` & `pymc-5.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.0/versioneer.py` & `pymc-5.3.1/versioneer.py`

 * *Files identical despite different names*

