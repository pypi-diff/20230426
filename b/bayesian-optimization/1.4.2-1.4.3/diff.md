# Comparing `tmp/bayesian-optimization-1.4.2.tar.gz` & `tmp/bayesian-optimization-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayesian-optimization-1.4.2.tar", last modified: Sun Dec  4 06:01:38 2022, max compression
+gzip compressed data, was "bayesian-optimization-1.4.3.tar", last modified: Tue Apr 25 21:55:32 2023, max compression
```

## Comparing `bayesian-optimization-1.4.2.tar` & `bayesian-optimization-1.4.3.tar`

### file list

```diff
@@ -1,22 +1,31 @@
-drwxrwxr-x   0 brendan   (1000) brendan   (1000)        0 2022-12-04 06:01:38.353732 bayesian-optimization-1.4.2/
--rw-rw-r--   0 brendan   (1000) brendan   (1000)     1089 2022-12-04 05:43:52.000000 bayesian-optimization-1.4.2/LICENSE
--rw-rw-r--   0 brendan   (1000) brendan   (1000)      392 2022-12-04 06:01:38.353732 bayesian-optimization-1.4.2/PKG-INFO
--rw-rw-r--   0 brendan   (1000) brendan   (1000)    15364 2022-12-04 05:43:52.000000 bayesian-optimization-1.4.2/README.md
-drwxrwxr-x   0 brendan   (1000) brendan   (1000)        0 2022-12-04 06:01:38.353732 bayesian-optimization-1.4.2/bayes_opt/
--rw-rw-r--   0 brendan   (1000) brendan   (1000)      436 2022-12-04 05:43:52.000000 bayesian-optimization-1.4.2/bayes_opt/__init__.py
--rw-rw-r--   0 brendan   (1000) brendan   (1000)    11759 2022-12-04 05:43:52.000000 bayesian-optimization-1.4.2/bayes_opt/bayesian_optimization.py
--rw-rw-r--   0 brendan   (1000) brendan   (1000)     5522 2022-12-04 05:43:52.000000 bayesian-optimization-1.4.2/bayes_opt/constraint.py
--rw-rw-r--   0 brendan   (1000) brendan   (1000)     4664 2022-12-04 05:43:52.000000 bayesian-optimization-1.4.2/bayes_opt/domain_reduction.py
--rw-rw-r--   0 brendan   (1000) brendan   (1000)      259 2022-12-04 05:43:52.000000 bayesian-optimization-1.4.2/bayes_opt/event.py
--rw-rw-r--   0 brendan   (1000) brendan   (1000)     5003 2022-12-04 05:43:52.000000 bayesian-optimization-1.4.2/bayes_opt/logger.py
--rw-rw-r--   0 brendan   (1000) brendan   (1000)     1289 2022-12-04 05:43:52.000000 bayesian-optimization-1.4.2/bayes_opt/observer.py
--rw-rw-r--   0 brendan   (1000) brendan   (1000)    11237 2022-12-04 05:43:52.000000 bayesian-optimization-1.4.2/bayes_opt/target_space.py
--rw-rw-r--   0 brendan   (1000) brendan   (1000)     8947 2022-12-04 05:43:52.000000 bayesian-optimization-1.4.2/bayes_opt/util.py
-drwxrwxr-x   0 brendan   (1000) brendan   (1000)        0 2022-12-04 06:01:38.353732 bayesian-optimization-1.4.2/bayesian_optimization.egg-info/
--rw-rw-r--   0 brendan   (1000) brendan   (1000)      392 2022-12-04 06:01:38.000000 bayesian-optimization-1.4.2/bayesian_optimization.egg-info/PKG-INFO
--rw-rw-r--   0 brendan   (1000) brendan   (1000)      466 2022-12-04 06:01:38.000000 bayesian-optimization-1.4.2/bayesian_optimization.egg-info/SOURCES.txt
--rw-rw-r--   0 brendan   (1000) brendan   (1000)        1 2022-12-04 06:01:38.000000 bayesian-optimization-1.4.2/bayesian_optimization.egg-info/dependency_links.txt
--rw-rw-r--   0 brendan   (1000) brendan   (1000)       63 2022-12-04 06:01:38.000000 bayesian-optimization-1.4.2/bayesian_optimization.egg-info/requires.txt
--rw-rw-r--   0 brendan   (1000) brendan   (1000)       10 2022-12-04 06:01:38.000000 bayesian-optimization-1.4.2/bayesian_optimization.egg-info/top_level.txt
--rw-rw-r--   0 brendan   (1000) brendan   (1000)       38 2022-12-04 06:01:38.353732 bayesian-optimization-1.4.2/setup.cfg
--rw-rw-r--   0 brendan   (1000) brendan   (1000)      663 2022-12-04 05:43:52.000000 bayesian-optimization-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 21:55:32.446584 bayesian-optimization-1.4.3/
+-rw-rw-rw-   0        0        0     1097 2023-04-25 21:47:05.000000 bayesian-optimization-1.4.3/LICENSE
+-rw-rw-rw-   0        0        0      404 2023-04-25 21:55:32.445587 bayesian-optimization-1.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0    15696 2023-04-25 21:47:05.000000 bayesian-optimization-1.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 21:55:32.420585 bayesian-optimization-1.4.3/bayes_opt/
+-rw-rw-rw-   0        0        0      452 2023-04-25 21:47:05.000000 bayesian-optimization-1.4.3/bayes_opt/__init__.py
+-rw-rw-rw-   0        0        0    11990 2023-04-25 21:47:05.000000 bayesian-optimization-1.4.3/bayes_opt/bayesian_optimization.py
+-rw-rw-rw-   0        0        0     5672 2023-04-25 21:47:05.000000 bayesian-optimization-1.4.3/bayes_opt/constraint.py
+-rw-rw-rw-   0        0        0     5862 2023-04-25 21:47:05.000000 bayesian-optimization-1.4.3/bayes_opt/domain_reduction.py
+-rw-rw-rw-   0        0        0      270 2023-04-25 21:47:05.000000 bayesian-optimization-1.4.3/bayes_opt/event.py
+-rw-rw-rw-   0        0        0     5166 2023-04-25 21:47:05.000000 bayesian-optimization-1.4.3/bayes_opt/logger.py
+-rw-rw-rw-   0        0        0     1337 2023-04-25 21:47:05.000000 bayesian-optimization-1.4.3/bayes_opt/observer.py
+-rw-rw-rw-   0        0        0    11583 2023-04-25 21:47:05.000000 bayesian-optimization-1.4.3/bayes_opt/target_space.py
+-rw-rw-rw-   0        0        0     9248 2023-04-25 21:47:05.000000 bayesian-optimization-1.4.3/bayes_opt/util.py
+drwxrwxrwx   0        0        0        0 2023-04-25 21:55:32.435584 bayesian-optimization-1.4.3/bayesian_optimization.egg-info/
+-rw-rw-rw-   0        0        0      404 2023-04-25 21:55:32.000000 bayesian-optimization-1.4.3/bayesian_optimization.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      670 2023-04-25 21:55:32.000000 bayesian-optimization-1.4.3/bayesian_optimization.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 21:55:32.000000 bayesian-optimization-1.4.3/bayesian_optimization.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-04-25 21:55:32.000000 bayesian-optimization-1.4.3/bayesian_optimization.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-25 21:55:32.000000 bayesian-optimization-1.4.3/bayesian_optimization.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 21:55:32.446584 bayesian-optimization-1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      686 2023-04-25 21:47:05.000000 bayesian-optimization-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 21:55:32.444085 bayesian-optimization-1.4.3/tests/
+-rw-rw-rw-   0        0        0     1806 2023-04-25 21:47:05.000000 bayesian-optimization-1.4.3/tests/test_acceptance.py
+-rw-rw-rw-   0        0        0    12900 2023-04-25 21:47:05.000000 bayesian-optimization-1.4.3/tests/test_bayesian_optimization.py
+-rw-rw-rw-   0        0        0     6057 2023-04-25 21:47:05.000000 bayesian-optimization-1.4.3/tests/test_constraint.py
+-rw-rw-rw-   0        0        0     3669 2023-04-25 21:47:05.000000 bayesian-optimization-1.4.3/tests/test_observer.py
+-rw-rw-rw-   0        0        0      815 2023-04-25 21:47:05.000000 bayesian-optimization-1.4.3/tests/test_queue.py
+-rw-rw-rw-   0        0        0     4617 2023-04-25 21:47:05.000000 bayesian-optimization-1.4.3/tests/test_seq_domain_red.py
+-rw-rw-rw-   0        0        0     6917 2023-04-25 21:47:05.000000 bayesian-optimization-1.4.3/tests/test_target_space.py
+-rw-rw-rw-   0        0        0     5299 2023-04-25 21:47:05.000000 bayesian-optimization-1.4.3/tests/test_util.py
```

### Comparing `bayesian-optimization-1.4.2/LICENSE` & `bayesian-optimization-1.4.3/LICENSE`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-The MIT License (MIT)
-
-Copyright (c) 2014 Fernando M. F. Nogueira
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+The MIT License (MIT)
+
+Copyright (c) 2014 Fernando M. F. Nogueira
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `bayesian-optimization-1.4.2/README.md` & `bayesian-optimization-1.4.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,331 +1,331 @@
-<div align="center">
-  <img src="https://github.com/fmfn/BayesianOptimization/blob/master/examples/func.png"><br><br>
-</div>
-
-# Bayesian Optimization
-
-![tests](https://github.com/fmfn/BayesianOptimization/actions/workflows/run_tests.yml/badge.svg)
-[![Codecov](https://codecov.io/github/fmfn/BayesianOptimization/badge.svg?branch=master&service=github)](https://codecov.io/github/fmfn/BayesianOptimization?branch=master)
-[![Pypi](https://img.shields.io/pypi/v/bayesian-optimization.svg)](https://pypi.python.org/pypi/bayesian-optimization)
-
-Pure Python implementation of bayesian global optimization with gaussian
-processes.
-
-* PyPI (pip):
-
-```console
-$ pip install bayesian-optimization
-```
-
-* Conda from conda-forge channel:
-
-```console
-$ conda install -c conda-forge bayesian-optimization
-```
-
-This is a constrained global optimization package built upon bayesian inference
-and gaussian process, that attempts to find the maximum value of an unknown
-function in as few iterations as possible. This technique is particularly
-suited for optimization of high cost functions, situations where the balance
-between exploration and exploitation is important.
-
-## Quick Start
-See below for a quick tour over the basics of the Bayesian Optimization package. More detailed information, other advanced features, and tips on usage/implementation can be found in the [examples](https://github.com/fmfn/BayesianOptimization/tree/master/examples) folder. I suggest that you:
-- Follow the
-[basic tour notebook](https://github.com/fmfn/BayesianOptimization/blob/master/examples/basic-tour.ipynb)
-to learn how to use the package's most important features.
-- Take a look at the
-[advanced tour notebook](https://github.com/fmfn/BayesianOptimization/blob/master/examples/advanced-tour.ipynb)
-to learn how to make the package more flexible, how to deal with categorical parameters, how to use observers, and more.
-- Check out this
-[notebook](https://github.com/fmfn/BayesianOptimization/blob/master/examples/visualization.ipynb)
-with a step by step visualization of how this method works.
-- To understand how to use bayesian optimization when additional constraints are present, see the
-[constrained optimization notebook](https://github.com/fmfn/BayesianOptimization/blob/master/examples/constraints.ipynb).
-- Explore this [notebook](https://github.com/fmfn/BayesianOptimization/blob/master/examples/exploitation_vs_exploration.ipynb)
-exemplifying the balance between exploration and exploitation and how to
-control it.
-- Go over this [script](https://github.com/fmfn/BayesianOptimization/blob/master/examples/sklearn_example.py)
-for examples of how to tune parameters of Machine Learning models using cross validation and bayesian optimization.
-- Explore the [domain reduction notebook](https://github.com/fmfn/BayesianOptimization/blob/master/examples/domain_reduction.ipynb) to learn more about how search can be sped up by dynamically changing parameters' bounds.
-- Finally, take a look at this [script](https://github.com/fmfn/BayesianOptimization/blob/master/examples/async_optimization.py)
-for ideas on how to implement bayesian optimization in a distributed fashion using this package.
-
-
-## How does it work?
-
-Bayesian optimization works by constructing a posterior distribution of functions (gaussian process) that best describes the function you want to optimize. As the number of observations grows, the posterior distribution improves, and the algorithm becomes more certain of which regions in parameter space are worth exploring and which are not, as seen in the picture below.
-
-![BayesianOptimization in action](./examples/bo_example.png)
-
-As you iterate over and over, the algorithm balances its needs of exploration and exploitation taking into account what it knows about the target function. At each step a Gaussian Process is fitted to the known samples (points previously explored), and the posterior distribution, combined with a exploration strategy (such as UCB (Upper Confidence Bound), or EI (Expected Improvement)), are used to determine the next point that should be explored (see the gif below).
-
-![BayesianOptimization in action](./examples/bayesian_optimization.gif)
-
-This process is designed to minimize the number of steps required to find a combination of parameters that are close to the optimal combination. To do so, this method uses a proxy optimization problem (finding the maximum of the acquisition function) that, albeit still a hard problem, is cheaper (in the computational sense) and common tools can be employed. Therefore Bayesian Optimization is most adequate for situations where sampling the function to be optimized is a very expensive endeavor. See the references for a proper discussion of this method.
-
-This project is under active development, if you find a bug, or anything that
-needs correction, please let me know.
-
-
-Basic tour of the Bayesian Optimization package
-===============================================
-
-## 1. Specifying the function to be optimized
-
-This is a function optimization package, therefore the first and most important ingredient is, of course, the function to be optimized.
-
-**DISCLAIMER:** We know exactly how the output of the function below depends on its parameter. Obviously this is just an example, and you shouldn't expect to know it in a real scenario. However, it should be clear that you don't need to. All you need in order to use this package (and more generally, this technique) is a function `f` that takes a known set of parameters and outputs a real number.
-
-
-```python
-def black_box_function(x, y):
-    """Function with unknown internals we wish to maximize.
-
-    This is just serving as an example, for all intents and
-    purposes think of the internals of this function, i.e.: the process
-    which generates its output values, as unknown.
-    """
-    return -x ** 2 - (y - 1) ** 2 + 1
-```
-
-## 2. Getting Started
-
-All we need to get started is to instantiate a `BayesianOptimization` object specifying a function to be optimized `f`, and its parameters with their corresponding bounds, `pbounds`. This is a constrained optimization technique, so you must specify the minimum and maximum values that can be probed for each parameter in order for it to work
-
-
-```python
-from bayes_opt import BayesianOptimization
-
-# Bounded region of parameter space
-pbounds = {'x': (2, 4), 'y': (-3, 3)}
-
-optimizer = BayesianOptimization(
-    f=black_box_function,
-    pbounds=pbounds,
-    random_state=1,
-)
-```
-
-The BayesianOptimization object will work out of the box without much tuning needed. The main method you should be aware of is `maximize`, which does exactly what you think it does.
-
-There are many parameters you can pass to maximize, nonetheless, the most important ones are:
-- `n_iter`: How many steps of bayesian optimization you want to perform. The more steps the more likely to find a good maximum you are.
-- `init_points`: How many steps of **random** exploration you want to perform. Random exploration can help by diversifying the exploration space.
-
-
-```python
-optimizer.maximize(
-    init_points=2,
-    n_iter=3,
-)
-```
-
-    |   iter    |  target   |     x     |     y     |
-    -------------------------------------------------
-    |  1        | -7.135    |  2.834    |  1.322    |
-    |  2        | -7.78     |  2.0      | -1.186    |
-    |  3        | -19.0     |  4.0      |  3.0      |
-    |  4        | -16.3     |  2.378    | -2.413    |
-    |  5        | -4.441    |  2.105    | -0.005822 |
-    =================================================
-
-
-The best combination of parameters and target value found can be accessed via the property `optimizer.max`.
-
-
-```python
-print(optimizer.max)
->>> {'target': -4.441293113411222, 'params': {'y': -0.005822117636089974, 'x': 2.104665051994087}}
-```
-
-
-While the list of all parameters probed and their corresponding target values is available via the property `optimizer.res`.
-
-
-```python
-for i, res in enumerate(optimizer.res):
-    print("Iteration {}: \n\t{}".format(i, res))
-
->>> Iteration 0:
->>>     {'target': -7.135455292718879, 'params': {'y': 1.3219469606529488, 'x': 2.8340440094051482}}
->>> Iteration 1:
->>>     {'target': -7.779531005607566, 'params': {'y': -1.1860045642089614, 'x': 2.0002287496346898}}
->>> Iteration 2:
->>>     {'target': -19.0, 'params': {'y': 3.0, 'x': 4.0}}
->>> Iteration 3:
->>>     {'target': -16.29839645063864, 'params': {'y': -2.412527795983739, 'x': 2.3776144540856503}}
->>> Iteration 4:
->>>     {'target': -4.441293113411222, 'params': {'y': -0.005822117636089974, 'x': 2.104665051994087}}
-```
-
-
-### 2.1 Changing bounds
-
-During the optimization process you may realize the bounds chosen for some parameters are not adequate. For these situations you can invoke the method `set_bounds` to alter them. You can pass any combination of **existing** parameters and their associated new bounds.
-
-
-```python
-optimizer.set_bounds(new_bounds={"x": (-2, 3)})
-
-optimizer.maximize(
-    init_points=0,
-    n_iter=5,
-)
-```
-
-    |   iter    |  target   |     x     |     y     |
-    -------------------------------------------------
-    |  6        | -5.145    |  2.115    | -0.2924   |
-    |  7        | -5.379    |  2.337    |  0.04124  |
-    |  8        | -3.581    |  1.874    | -0.03428  |
-    |  9        | -2.624    |  1.702    |  0.1472   |
-    |  10       | -1.762    |  1.442    |  0.1735   |
-    =================================================
-
-### 2.2 Sequential Domain Reduction
-
-Sometimes the initial boundaries specified for a problem are too wide, and adding points to improve the response surface in regions of the solution domain is extraneous. Other times the cost function is very expensive to compute, and minimizing the number of calls is extremely beneficial.
-
-When it's worthwhile to converge on an optimal point quickly rather than try to find the optimal point, contracting the domain around the current optimal value as the search progresses can speed up the search progress considerably. Using the `SequentialDomainReductionTransformer` the bounds of the problem can be panned and zoomed dynamically in an attempt to improve convergence.
-
-![sequential domain reduction](./examples/sdr.png)
-
-An example of using the `SequentialDomainReductionTransformer` is shown in the [domain reduction notebook](https://github.com/fmfn/BayesianOptimization/blob/master/examples/domain_reduction.ipynb). More information about this method can be found in the paper ["On the robustness of a simple domain reduction scheme for simulation‐based optimization"](http://www.truegrid.com/srsm_revised.pdf).
-
-## 3. Guiding the optimization
-
-It is often the case that we have an idea of regions of the parameter space where the maximum of our function might lie. For these situations the `BayesianOptimization` object allows the user to specify points to be probed. By default these will be explored lazily (`lazy=True`), meaning these points will be evaluated only the next time you call `maximize`. This probing process happens before the gaussian process takes over.
-
-Parameters can be passed as dictionaries or as an iterable.
-
-```python
-optimizer.probe(
-    params={"x": 0.5, "y": 0.7},
-    lazy=True,
-)
-
-optimizer.probe(
-    params=[-0.3, 0.1],
-    lazy=True,
-)
-
-# Will probe only the two points specified above
-optimizer.maximize(init_points=0, n_iter=0)
-```
-
-    |   iter    |  target   |     x     |     y     |
-    -------------------------------------------------
-    |  11       |  0.66     |  0.5      |  0.7      |
-    |  12       |  0.1      | -0.3      |  0.1      |
-    =================================================
-
-
-## 4. Saving, loading and restarting
-
-By default you can follow the progress of your optimization by setting `verbose>0` when instantiating the `BayesianOptimization` object. If you need more control over logging/alerting you will need to use an observer. For more information about observers checkout the advanced tour notebook. Here we will only see how to use the native `JSONLogger` object to save to and load progress from files.
-
-### 4.1 Saving progress
-
-
-```python
-from bayes_opt.logger import JSONLogger
-from bayes_opt.event import Events
-```
-
-The observer paradigm works by:
-1. Instantiating an observer object.
-2. Tying the observer object to a particular event fired by an optimizer.
-
-The `BayesianOptimization` object fires a number of internal events during optimization, in particular, everytime it probes the function and obtains a new parameter-target combination it will fire an `Events.OPTIMIZATION_STEP` event, which our logger will listen to.
-
-**Caveat:** The logger will not look back at previously probed points.
-
-
-```python
-logger = JSONLogger(path="./logs.json")
-optimizer.subscribe(Events.OPTIMIZATION_STEP, logger)
-
-# Results will be saved in ./logs.json
-optimizer.maximize(
-    init_points=2,
-    n_iter=3,
-)
-```
-
-By default the previous data in the json file is removed. If you want to keep working with the same logger, the `reset` paremeter in `JSONLogger` should be set to False.
-
-### 4.2 Loading progress
-
-Naturally, if you stored progress you will be able to load that onto a new instance of `BayesianOptimization`. The easiest way to do it is by invoking the `load_logs` function, from the `util` submodule.
-
-
-```python
-from bayes_opt.util import load_logs
-
-
-new_optimizer = BayesianOptimization(
-    f=black_box_function,
-    pbounds={"x": (-2, 2), "y": (-2, 2)},
-    verbose=2,
-    random_state=7,
-)
-
-# New optimizer is loaded with previously seen points
-load_logs(new_optimizer, logs=["./logs.json"]);
-```
-
-## Next Steps
-
-This introduction covered the most basic functionality of the package. Checkout the [basic-tour](https://github.com/fmfn/BayesianOptimization/blob/master/examples/basic-tour.ipynb) and [advanced-tour](https://github.com/fmfn/BayesianOptimization/blob/master/examples/advanced-tour.ipynb) notebooks in the example folder, where you will find detailed explanations and other more advanced functionality. Also, browse the examples folder for implementation tips and ideas.
-
-Installation
-============
-
-### Installation
-
-The latest release can be obtained by two ways:
-
-* With PyPI (pip):
-
-      pip install bayesian-optimization
-
-* With conda (from conda-forge channel):
-
-      conda install -c conda-forge bayesian-optimization
-
-The bleeding edge version can be installed with:
-
-    pip install git+https://github.com/fmfn/BayesianOptimization.git
-
-If you prefer, you can clone it and run the setup.py file. Use the following
-commands to get a copy from Github and install all dependencies:
-
-    git clone https://github.com/fmfn/BayesianOptimization.git
-    cd BayesianOptimization
-    python setup.py install
-
-Citation
-============
-
-If you used this package in your research and is interested in citing it here's how you do it:
-
-```
-@Misc{,
-    author = {Fernando Nogueira},
-    title = {{Bayesian Optimization}: Open source constrained global optimization tool for {Python}},
-    year = {2014--},
-    url = " https://github.com/fmfn/BayesianOptimization"
-}
-```
-
-# Dependencies
-* Numpy
-* Scipy
-* Scikit-learn
-
-# References:
-* http://papers.nips.cc/paper/4522-practical-bayesian-optimization-of-machine-learning-algorithms.pdf
-* http://arxiv.org/pdf/1012.2599v1.pdf
-* http://www.gaussianprocess.org/gpml/
-* https://www.youtube.com/watch?v=vz3D36VXefI&index=10&list=PLE6Wd9FR--EdyJ5lbFl8UuGjecvVw66F6
+<div align="center">
+  <img src="https://github.com/fmfn/BayesianOptimization/blob/master/examples/func.png"><br><br>
+</div>
+
+# Bayesian Optimization
+
+![tests](https://github.com/fmfn/BayesianOptimization/actions/workflows/run_tests.yml/badge.svg)
+[![Codecov](https://codecov.io/github/fmfn/BayesianOptimization/badge.svg?branch=master&service=github)](https://codecov.io/github/fmfn/BayesianOptimization?branch=master)
+[![Pypi](https://img.shields.io/pypi/v/bayesian-optimization.svg)](https://pypi.python.org/pypi/bayesian-optimization)
+
+Pure Python implementation of bayesian global optimization with gaussian
+processes.
+
+* PyPI (pip):
+
+```console
+$ pip install bayesian-optimization
+```
+
+* Conda from conda-forge channel:
+
+```console
+$ conda install -c conda-forge bayesian-optimization
+```
+
+This is a constrained global optimization package built upon bayesian inference
+and gaussian process, that attempts to find the maximum value of an unknown
+function in as few iterations as possible. This technique is particularly
+suited for optimization of high cost functions, situations where the balance
+between exploration and exploitation is important.
+
+## Quick Start
+See below for a quick tour over the basics of the Bayesian Optimization package. More detailed information, other advanced features, and tips on usage/implementation can be found in the [examples](https://github.com/fmfn/BayesianOptimization/tree/master/examples) folder. I suggest that you:
+- Follow the
+[basic tour notebook](https://github.com/fmfn/BayesianOptimization/blob/master/examples/basic-tour.ipynb)
+to learn how to use the package's most important features.
+- Take a look at the
+[advanced tour notebook](https://github.com/fmfn/BayesianOptimization/blob/master/examples/advanced-tour.ipynb)
+to learn how to make the package more flexible, how to deal with categorical parameters, how to use observers, and more.
+- Check out this
+[notebook](https://github.com/fmfn/BayesianOptimization/blob/master/examples/visualization.ipynb)
+with a step by step visualization of how this method works.
+- To understand how to use bayesian optimization when additional constraints are present, see the
+[constrained optimization notebook](https://github.com/fmfn/BayesianOptimization/blob/master/examples/constraints.ipynb).
+- Explore this [notebook](https://github.com/fmfn/BayesianOptimization/blob/master/examples/exploitation_vs_exploration.ipynb)
+exemplifying the balance between exploration and exploitation and how to
+control it.
+- Go over this [script](https://github.com/fmfn/BayesianOptimization/blob/master/examples/sklearn_example.py)
+for examples of how to tune parameters of Machine Learning models using cross validation and bayesian optimization.
+- Explore the [domain reduction notebook](https://github.com/fmfn/BayesianOptimization/blob/master/examples/domain_reduction.ipynb) to learn more about how search can be sped up by dynamically changing parameters' bounds.
+- Finally, take a look at this [script](https://github.com/fmfn/BayesianOptimization/blob/master/examples/async_optimization.py)
+for ideas on how to implement bayesian optimization in a distributed fashion using this package.
+
+
+## How does it work?
+
+Bayesian optimization works by constructing a posterior distribution of functions (gaussian process) that best describes the function you want to optimize. As the number of observations grows, the posterior distribution improves, and the algorithm becomes more certain of which regions in parameter space are worth exploring and which are not, as seen in the picture below.
+
+![BayesianOptimization in action](./examples/bo_example.png)
+
+As you iterate over and over, the algorithm balances its needs of exploration and exploitation taking into account what it knows about the target function. At each step a Gaussian Process is fitted to the known samples (points previously explored), and the posterior distribution, combined with a exploration strategy (such as UCB (Upper Confidence Bound), or EI (Expected Improvement)), are used to determine the next point that should be explored (see the gif below).
+
+![BayesianOptimization in action](./examples/bayesian_optimization.gif)
+
+This process is designed to minimize the number of steps required to find a combination of parameters that are close to the optimal combination. To do so, this method uses a proxy optimization problem (finding the maximum of the acquisition function) that, albeit still a hard problem, is cheaper (in the computational sense) and common tools can be employed. Therefore Bayesian Optimization is most adequate for situations where sampling the function to be optimized is a very expensive endeavor. See the references for a proper discussion of this method.
+
+This project is under active development, if you find a bug, or anything that
+needs correction, please let me know.
+
+
+Basic tour of the Bayesian Optimization package
+===============================================
+
+## 1. Specifying the function to be optimized
+
+This is a function optimization package, therefore the first and most important ingredient is, of course, the function to be optimized.
+
+**DISCLAIMER:** We know exactly how the output of the function below depends on its parameter. Obviously this is just an example, and you shouldn't expect to know it in a real scenario. However, it should be clear that you don't need to. All you need in order to use this package (and more generally, this technique) is a function `f` that takes a known set of parameters and outputs a real number.
+
+
+```python
+def black_box_function(x, y):
+    """Function with unknown internals we wish to maximize.
+
+    This is just serving as an example, for all intents and
+    purposes think of the internals of this function, i.e.: the process
+    which generates its output values, as unknown.
+    """
+    return -x ** 2 - (y - 1) ** 2 + 1
+```
+
+## 2. Getting Started
+
+All we need to get started is to instantiate a `BayesianOptimization` object specifying a function to be optimized `f`, and its parameters with their corresponding bounds, `pbounds`. This is a constrained optimization technique, so you must specify the minimum and maximum values that can be probed for each parameter in order for it to work
+
+
+```python
+from bayes_opt import BayesianOptimization
+
+# Bounded region of parameter space
+pbounds = {'x': (2, 4), 'y': (-3, 3)}
+
+optimizer = BayesianOptimization(
+    f=black_box_function,
+    pbounds=pbounds,
+    random_state=1,
+)
+```
+
+The BayesianOptimization object will work out of the box without much tuning needed. The main method you should be aware of is `maximize`, which does exactly what you think it does.
+
+There are many parameters you can pass to maximize, nonetheless, the most important ones are:
+- `n_iter`: How many steps of bayesian optimization you want to perform. The more steps the more likely to find a good maximum you are.
+- `init_points`: How many steps of **random** exploration you want to perform. Random exploration can help by diversifying the exploration space.
+
+
+```python
+optimizer.maximize(
+    init_points=2,
+    n_iter=3,
+)
+```
+
+    |   iter    |  target   |     x     |     y     |
+    -------------------------------------------------
+    |  1        | -7.135    |  2.834    |  1.322    |
+    |  2        | -7.78     |  2.0      | -1.186    |
+    |  3        | -19.0     |  4.0      |  3.0      |
+    |  4        | -16.3     |  2.378    | -2.413    |
+    |  5        | -4.441    |  2.105    | -0.005822 |
+    =================================================
+
+
+The best combination of parameters and target value found can be accessed via the property `optimizer.max`.
+
+
+```python
+print(optimizer.max)
+>>> {'target': -4.441293113411222, 'params': {'y': -0.005822117636089974, 'x': 2.104665051994087}}
+```
+
+
+While the list of all parameters probed and their corresponding target values is available via the property `optimizer.res`.
+
+
+```python
+for i, res in enumerate(optimizer.res):
+    print("Iteration {}: \n\t{}".format(i, res))
+
+>>> Iteration 0:
+>>>     {'target': -7.135455292718879, 'params': {'y': 1.3219469606529488, 'x': 2.8340440094051482}}
+>>> Iteration 1:
+>>>     {'target': -7.779531005607566, 'params': {'y': -1.1860045642089614, 'x': 2.0002287496346898}}
+>>> Iteration 2:
+>>>     {'target': -19.0, 'params': {'y': 3.0, 'x': 4.0}}
+>>> Iteration 3:
+>>>     {'target': -16.29839645063864, 'params': {'y': -2.412527795983739, 'x': 2.3776144540856503}}
+>>> Iteration 4:
+>>>     {'target': -4.441293113411222, 'params': {'y': -0.005822117636089974, 'x': 2.104665051994087}}
+```
+
+
+### 2.1 Changing bounds
+
+During the optimization process you may realize the bounds chosen for some parameters are not adequate. For these situations you can invoke the method `set_bounds` to alter them. You can pass any combination of **existing** parameters and their associated new bounds.
+
+
+```python
+optimizer.set_bounds(new_bounds={"x": (-2, 3)})
+
+optimizer.maximize(
+    init_points=0,
+    n_iter=5,
+)
+```
+
+    |   iter    |  target   |     x     |     y     |
+    -------------------------------------------------
+    |  6        | -5.145    |  2.115    | -0.2924   |
+    |  7        | -5.379    |  2.337    |  0.04124  |
+    |  8        | -3.581    |  1.874    | -0.03428  |
+    |  9        | -2.624    |  1.702    |  0.1472   |
+    |  10       | -1.762    |  1.442    |  0.1735   |
+    =================================================
+
+### 2.2 Sequential Domain Reduction
+
+Sometimes the initial boundaries specified for a problem are too wide, and adding points to improve the response surface in regions of the solution domain is extraneous. Other times the cost function is very expensive to compute, and minimizing the number of calls is extremely beneficial.
+
+When it's worthwhile to converge on an optimal point quickly rather than try to find the optimal point, contracting the domain around the current optimal value as the search progresses can speed up the search progress considerably. Using the `SequentialDomainReductionTransformer` the bounds of the problem can be panned and zoomed dynamically in an attempt to improve convergence.
+
+![sequential domain reduction](./examples/sdr.png)
+
+An example of using the `SequentialDomainReductionTransformer` is shown in the [domain reduction notebook](https://github.com/fmfn/BayesianOptimization/blob/master/examples/domain_reduction.ipynb). More information about this method can be found in the paper ["On the robustness of a simple domain reduction scheme for simulation‐based optimization"](http://www.truegrid.com/srsm_revised.pdf).
+
+## 3. Guiding the optimization
+
+It is often the case that we have an idea of regions of the parameter space where the maximum of our function might lie. For these situations the `BayesianOptimization` object allows the user to specify points to be probed. By default these will be explored lazily (`lazy=True`), meaning these points will be evaluated only the next time you call `maximize`. This probing process happens before the gaussian process takes over.
+
+Parameters can be passed as dictionaries or as an iterable.
+
+```python
+optimizer.probe(
+    params={"x": 0.5, "y": 0.7},
+    lazy=True,
+)
+
+optimizer.probe(
+    params=[-0.3, 0.1],
+    lazy=True,
+)
+
+# Will probe only the two points specified above
+optimizer.maximize(init_points=0, n_iter=0)
+```
+
+    |   iter    |  target   |     x     |     y     |
+    -------------------------------------------------
+    |  11       |  0.66     |  0.5      |  0.7      |
+    |  12       |  0.1      | -0.3      |  0.1      |
+    =================================================
+
+
+## 4. Saving, loading and restarting
+
+By default you can follow the progress of your optimization by setting `verbose>0` when instantiating the `BayesianOptimization` object. If you need more control over logging/alerting you will need to use an observer. For more information about observers checkout the advanced tour notebook. Here we will only see how to use the native `JSONLogger` object to save to and load progress from files.
+
+### 4.1 Saving progress
+
+
+```python
+from bayes_opt.logger import JSONLogger
+from bayes_opt.event import Events
+```
+
+The observer paradigm works by:
+1. Instantiating an observer object.
+2. Tying the observer object to a particular event fired by an optimizer.
+
+The `BayesianOptimization` object fires a number of internal events during optimization, in particular, everytime it probes the function and obtains a new parameter-target combination it will fire an `Events.OPTIMIZATION_STEP` event, which our logger will listen to.
+
+**Caveat:** The logger will not look back at previously probed points.
+
+
+```python
+logger = JSONLogger(path="./logs.json")
+optimizer.subscribe(Events.OPTIMIZATION_STEP, logger)
+
+# Results will be saved in ./logs.json
+optimizer.maximize(
+    init_points=2,
+    n_iter=3,
+)
+```
+
+By default the previous data in the json file is removed. If you want to keep working with the same logger, the `reset` paremeter in `JSONLogger` should be set to False.
+
+### 4.2 Loading progress
+
+Naturally, if you stored progress you will be able to load that onto a new instance of `BayesianOptimization`. The easiest way to do it is by invoking the `load_logs` function, from the `util` submodule.
+
+
+```python
+from bayes_opt.util import load_logs
+
+
+new_optimizer = BayesianOptimization(
+    f=black_box_function,
+    pbounds={"x": (-2, 2), "y": (-2, 2)},
+    verbose=2,
+    random_state=7,
+)
+
+# New optimizer is loaded with previously seen points
+load_logs(new_optimizer, logs=["./logs.json"]);
+```
+
+## Next Steps
+
+This introduction covered the most basic functionality of the package. Checkout the [basic-tour](https://github.com/fmfn/BayesianOptimization/blob/master/examples/basic-tour.ipynb) and [advanced-tour](https://github.com/fmfn/BayesianOptimization/blob/master/examples/advanced-tour.ipynb) notebooks in the example folder, where you will find detailed explanations and other more advanced functionality. Also, browse the examples folder for implementation tips and ideas.
+
+Installation
+============
+
+### Installation
+
+The latest release can be obtained by two ways:
+
+* With PyPI (pip):
+
+      pip install bayesian-optimization
+
+* With conda (from conda-forge channel):
+
+      conda install -c conda-forge bayesian-optimization
+
+The bleeding edge version can be installed with:
+
+    pip install git+https://github.com/fmfn/BayesianOptimization.git
+
+If you prefer, you can clone it and run the setup.py file. Use the following
+commands to get a copy from Github and install all dependencies:
+
+    git clone https://github.com/fmfn/BayesianOptimization.git
+    cd BayesianOptimization
+    python setup.py install
+
+Citation
+============
+
+If you used this package in your research and is interested in citing it here's how you do it:
+
+```
+@Misc{,
+    author = {Fernando Nogueira},
+    title = {{Bayesian Optimization}: Open source constrained global optimization tool for {Python}},
+    year = {2014--},
+    url = " https://github.com/fmfn/BayesianOptimization"
+}
+```
+
+# Dependencies
+* Numpy
+* Scipy
+* Scikit-learn
+ 
+# References:
+* http://papers.nips.cc/paper/4522-practical-bayesian-optimization-of-machine-learning-algorithms.pdf
+* http://arxiv.org/pdf/1012.2599v1.pdf
+* http://www.gaussianprocess.org/gpml/
+* https://www.youtube.com/watch?v=vz3D36VXefI&index=10&list=PLE6Wd9FR--EdyJ5lbFl8UuGjecvVw66F6
```

### Comparing `bayesian-optimization-1.4.2/bayes_opt/constraint.py` & `bayesian-optimization-1.4.3/bayes_opt/constraint.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,150 +1,150 @@
-import numpy as np
-from sklearn.gaussian_process.kernels import Matern
-from sklearn.gaussian_process import GaussianProcessRegressor
-from scipy.stats import norm
-
-
-class ConstraintModel():
-    """
-    This class takes the function to optimize as well as the parameters bounds
-    in order to find which values for the parameters yield the maximum value
-    using bayesian optimization.
-
-    Parameters
-    ----------
-    fun: function
-        Constraint function. If multiple constraints are handled, this should
-        return a numpy.ndarray of appropriate size.
-
-    lb: numeric or numpy.ndarray
-        Upper limit(s) for the constraints. The return value of `fun` should
-        have exactly this shape.
-
-    ub: numeric or numpy.ndarray
-        Upper limit(s) for the constraints. The return value of `fun` should
-        have exactly this shape.
-
-    random_state: int or numpy.random.RandomState, optional(default=None)
-        If the value is an integer, it is used as the seed for creating a
-        numpy.random.RandomState. Otherwise the random state provided is used.
-        When set to None, an unseeded random state is generated.
-
-    Note
-    ----
-    In case of multiple constraints, this model assumes conditional
-    independence. This means that for each constraint, the probability of
-    fulfillment is the cdf of a univariate Gaussian. The overall probability
-    is a simply the product of the individual probabilities.
-    """
-
-    def __init__(self, fun, lb, ub, random_state=None):
-        self.fun = fun
-
-        self._lb = np.atleast_1d(lb)        
-        self._ub = np.atleast_1d(ub)
-
-        if np.any(self._lb >= self._ub):
-            msg = "Lower bounds must be less than upper bounds."
-            raise ValueError(msg)
-
-        basis = lambda: GaussianProcessRegressor(
-            kernel=Matern(nu=2.5),
-            alpha=1e-6,
-            normalize_y=True,
-            n_restarts_optimizer=5,
-            random_state=random_state,
-        )
-        self._model = [basis() for _ in range(len(self._lb))]
-
-    @property
-    def lb(self):
-        return self._lb
-
-    @property
-    def ub(self):
-        return self._ub
-    
-    @property
-    def model(self):
-        return self._model
-
-    def eval(self, **kwargs):
-        """
-        Evaluates the constraint function.
-        """
-        try:
-            return self.fun(**kwargs)
-        except TypeError as e:
-            msg = (
-                "Encountered TypeError when evaluating constraint " +
-                "function. This could be because your constraint function " +
-                "doesn't use the same keyword arguments as the target " +
-                f"function. Original error message:\n\n{e}"
-                )
-            e.args = (msg,)
-            raise
-
-    def fit(self, X, Y):
-        """
-        Fits internal GaussianProcessRegressor's to the data.
-        """
-        if len(self._model) == 1:
-            self._model[0].fit(X, Y)
-        else:
-            for i, gp in enumerate(self._model):
-                gp.fit(X, Y[:, i])
-
-    def predict(self, X):
-        """
-        Returns the probability that the constraint is fulfilled at `X` based
-        on the internal Gaussian Process Regressors.
-
-        Note that this does not try to approximate the values of the constraint
-        function, but probability that the constraint function is fulfilled.
-        For the former, see `ConstraintModel.approx()`.
-        """
-        X_shape = X.shape
-        X = X.reshape((-1, self._model[0].n_features_in_))
-        if len(self._model) == 1:
-            y_mean, y_std = self._model[0].predict(X, return_std=True)
-
-            p_lower = (norm(loc=y_mean, scale=y_std).cdf(self._lb[0])
-                            if self._lb[0] != -np.inf else np.array([0]))
-            p_upper = (norm(loc=y_mean, scale=y_std).cdf(self._ub[0])
-                            if self._lb[0] != np.inf else np.array([1]))
-            result = p_upper - p_lower
-            return result.reshape(X_shape[:-1])
-        else:
-            result = np.ones(X.shape[0])
-            for j, gp in enumerate(self._model):
-                y_mean, y_std = gp.predict(X, return_std=True)
-                p_lower = (norm(loc=y_mean, scale=y_std).cdf(self._lb[j])
-                           if self._lb[j] != -np.inf else np.array([0]))
-                p_upper = (norm(loc=y_mean, scale=y_std).cdf(self._ub[j])
-                           if self._lb[j] != np.inf else np.array([1]))
-                result = result * (p_upper - p_lower)
-            return result.reshape(X_shape[:-1])
-
-    def approx(self, X):
-        """
-        Returns the approximation of the constraint function using the internal
-        Gaussian Process Regressors.
-        """
-        X_shape = X.shape
-        X = X.reshape((-1, self._model[0].n_features_in_))
-        if len(self._model) == 1:
-            return self._model[0].predict(X).reshape(X_shape[:-1])
-        else:
-            result = np.column_stack([gp.predict(X) for gp in self._model])
-            return result.reshape(X_shape[:-1] + (len(self._lb), ))
-
-    def allowed(self, constraint_values):
-        """
-        Checks whether `constraint_values` are below the specified limits.
-        """
-        if self._lb.size == 1:
-            return (np.less_equal(self._lb, constraint_values)
-                    & np.less_equal(constraint_values, self._ub))
-
-        return (np.all(constraint_values <= self._ub, axis=-1)
-                    & np.all(constraint_values >= self._lb, axis=-1))
+import numpy as np
+from sklearn.gaussian_process.kernels import Matern
+from sklearn.gaussian_process import GaussianProcessRegressor
+from scipy.stats import norm
+
+
+class ConstraintModel():
+    """
+    This class takes the function to optimize as well as the parameters bounds
+    in order to find which values for the parameters yield the maximum value
+    using bayesian optimization.
+
+    Parameters
+    ----------
+    fun: function
+        Constraint function. If multiple constraints are handled, this should
+        return a numpy.ndarray of appropriate size.
+
+    lb: numeric or numpy.ndarray
+        Upper limit(s) for the constraints. The return value of `fun` should
+        have exactly this shape.
+
+    ub: numeric or numpy.ndarray
+        Upper limit(s) for the constraints. The return value of `fun` should
+        have exactly this shape.
+
+    random_state: int or numpy.random.RandomState, optional(default=None)
+        If the value is an integer, it is used as the seed for creating a
+        numpy.random.RandomState. Otherwise the random state provided is used.
+        When set to None, an unseeded random state is generated.
+
+    Note
+    ----
+    In case of multiple constraints, this model assumes conditional
+    independence. This means that for each constraint, the probability of
+    fulfillment is the cdf of a univariate Gaussian. The overall probability
+    is a simply the product of the individual probabilities.
+    """
+
+    def __init__(self, fun, lb, ub, random_state=None):
+        self.fun = fun
+
+        self._lb = np.atleast_1d(lb)        
+        self._ub = np.atleast_1d(ub)
+
+        if np.any(self._lb >= self._ub):
+            msg = "Lower bounds must be less than upper bounds."
+            raise ValueError(msg)
+
+        basis = lambda: GaussianProcessRegressor(
+            kernel=Matern(nu=2.5),
+            alpha=1e-6,
+            normalize_y=True,
+            n_restarts_optimizer=5,
+            random_state=random_state,
+        )
+        self._model = [basis() for _ in range(len(self._lb))]
+
+    @property
+    def lb(self):
+        return self._lb
+
+    @property
+    def ub(self):
+        return self._ub
+    
+    @property
+    def model(self):
+        return self._model
+
+    def eval(self, **kwargs):
+        """
+        Evaluates the constraint function.
+        """
+        try:
+            return self.fun(**kwargs)
+        except TypeError as e:
+            msg = (
+                "Encountered TypeError when evaluating constraint " +
+                "function. This could be because your constraint function " +
+                "doesn't use the same keyword arguments as the target " +
+                f"function. Original error message:\n\n{e}"
+                )
+            e.args = (msg,)
+            raise
+
+    def fit(self, X, Y):
+        """
+        Fits internal GaussianProcessRegressor's to the data.
+        """
+        if len(self._model) == 1:
+            self._model[0].fit(X, Y)
+        else:
+            for i, gp in enumerate(self._model):
+                gp.fit(X, Y[:, i])
+
+    def predict(self, X):
+        """
+        Returns the probability that the constraint is fulfilled at `X` based
+        on the internal Gaussian Process Regressors.
+
+        Note that this does not try to approximate the values of the constraint
+        function, but probability that the constraint function is fulfilled.
+        For the former, see `ConstraintModel.approx()`.
+        """
+        X_shape = X.shape
+        X = X.reshape((-1, self._model[0].n_features_in_))
+        if len(self._model) == 1:
+            y_mean, y_std = self._model[0].predict(X, return_std=True)
+
+            p_lower = (norm(loc=y_mean, scale=y_std).cdf(self._lb[0])
+                            if self._lb[0] != -np.inf else np.array([0]))
+            p_upper = (norm(loc=y_mean, scale=y_std).cdf(self._ub[0])
+                            if self._lb[0] != np.inf else np.array([1]))
+            result = p_upper - p_lower
+            return result.reshape(X_shape[:-1])
+        else:
+            result = np.ones(X.shape[0])
+            for j, gp in enumerate(self._model):
+                y_mean, y_std = gp.predict(X, return_std=True)
+                p_lower = (norm(loc=y_mean, scale=y_std).cdf(self._lb[j])
+                           if self._lb[j] != -np.inf else np.array([0]))
+                p_upper = (norm(loc=y_mean, scale=y_std).cdf(self._ub[j])
+                           if self._lb[j] != np.inf else np.array([1]))
+                result = result * (p_upper - p_lower)
+            return result.reshape(X_shape[:-1])
+
+    def approx(self, X):
+        """
+        Returns the approximation of the constraint function using the internal
+        Gaussian Process Regressors.
+        """
+        X_shape = X.shape
+        X = X.reshape((-1, self._model[0].n_features_in_))
+        if len(self._model) == 1:
+            return self._model[0].predict(X).reshape(X_shape[:-1])
+        else:
+            result = np.column_stack([gp.predict(X) for gp in self._model])
+            return result.reshape(X_shape[:-1] + (len(self._lb), ))
+
+    def allowed(self, constraint_values):
+        """
+        Checks whether `constraint_values` are below the specified limits.
+        """
+        if self._lb.size == 1:
+            return (np.less_equal(self._lb, constraint_values)
+                    & np.less_equal(constraint_values, self._ub))
+
+        return (np.all(constraint_values <= self._ub, axis=-1)
+                    & np.all(constraint_values >= self._lb, axis=-1))
```

### Comparing `bayesian-optimization-1.4.2/bayes_opt/domain_reduction.py` & `bayesian-optimization-1.4.3/bayes_opt/domain_reduction.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,129 +1,148 @@
-from typing import Optional, Union, List
-
-import numpy as np
-from .target_space import TargetSpace
-
-
-class DomainTransformer():
-    '''The base transformer class'''
-
-    def __init__(self, **kwargs):
-        pass
-
-    def initialize(self, target_space: TargetSpace):
-        raise NotImplementedError
-
-    def transform(self, target_space: TargetSpace):
-        raise NotImplementedError
-
-
-class SequentialDomainReductionTransformer(DomainTransformer):
-    """
-    A sequential domain reduction transformer bassed on the work by Stander, N. and Craig, K:
-    "On the robustness of a simple domain reduction scheme for simulation‐based optimization"
-    """
-
-    def __init__(
-        self,
-        gamma_osc: float = 0.7,
-        gamma_pan: float = 1.0,
-        eta: float = 0.9,
-        minimum_window: Optional[Union[List[float], float]] = 0.0
-    ) -> None:
-        self.gamma_osc = gamma_osc
-        self.gamma_pan = gamma_pan
-        self.eta = eta
-        self.minimum_window_value = minimum_window
-
-    def initialize(self, target_space: TargetSpace) -> None:
-        """Initialize all of the parameters"""
-        self.original_bounds = np.copy(target_space.bounds)
-        self.bounds = [self.original_bounds]
-
-        # Set the minimum window to an array of length bounds
-        if isinstance(self.minimum_window_value, list) or isinstance(self.minimum_window_value, np.ndarray):
-            assert len(self.minimum_window_value) == len(target_space.bounds)
-            self.minimum_window = self.minimum_window_value
-        else:
-            self.minimum_window = [self.minimum_window_value] * len(target_space.bounds)
-
-        self.previous_optimal = np.mean(target_space.bounds, axis=1)
-        self.current_optimal = np.mean(target_space.bounds, axis=1)
-        self.r = target_space.bounds[:, 1] - target_space.bounds[:, 0]
-
-        self.previous_d = 2.0 * \
-            (self.current_optimal - self.previous_optimal) / self.r
-
-        self.current_d = 2.0 * (self.current_optimal -
-                                self.previous_optimal) / self.r
-
-        self.c = self.current_d * self.previous_d
-        self.c_hat = np.sqrt(np.abs(self.c)) * np.sign(self.c)
-
-        self.gamma = 0.5 * (self.gamma_pan * (1.0 + self.c_hat) +
-                            self.gamma_osc * (1.0 - self.c_hat))
-
-        self.contraction_rate = self.eta + \
-            np.abs(self.current_d) * (self.gamma - self.eta)
-
-        self.r = self.contraction_rate * self.r
-
-    def _update(self, target_space: TargetSpace) -> None:
-
-        # setting the previous
-        self.previous_optimal = self.current_optimal
-        self.previous_d = self.current_d
-
-        self.current_optimal = target_space.params[
-            np.argmax(target_space.target)
-        ]
-
-        self.current_d = 2.0 * (self.current_optimal -
-                                self.previous_optimal) / self.r
-
-        self.c = self.current_d * self.previous_d
-
-        self.c_hat = np.sqrt(np.abs(self.c)) * np.sign(self.c)
-
-        self.gamma = 0.5 * (self.gamma_pan * (1.0 + self.c_hat) +
-                            self.gamma_osc * (1.0 - self.c_hat))
-
-        self.contraction_rate = self.eta + \
-            np.abs(self.current_d) * (self.gamma - self.eta)
-
-        self.r = self.contraction_rate * self.r
-
-    def _trim(self, new_bounds: np.array, global_bounds: np.array) -> np.array:
-        for i, variable in enumerate(new_bounds):
-            if variable[0] < global_bounds[i, 0]:
-                variable[0] = global_bounds[i, 0]
-            if variable[1] > global_bounds[i, 1]:
-                variable[1] = global_bounds[i, 1]
-        for i, entry in enumerate(new_bounds):
-            if entry[0] > entry[1]:
-                new_bounds[i, 0] = entry[1]
-                new_bounds[i, 1] = entry[0]
-            window_width = abs(entry[0] - entry[1])
-            if window_width < self.minimum_window[i]:
-                new_bounds[i, 0] -= (self.minimum_window[i] - window_width) / 2.0
-                new_bounds[i, 1] += (self.minimum_window[i] - window_width) / 2.0
-
-        return new_bounds
-
-    def _create_bounds(self, parameters: dict, bounds: np.array) -> dict:
-        return {param: bounds[i, :] for i, param in enumerate(parameters)}
-
-    def transform(self, target_space: TargetSpace) -> dict:
-
-        self._update(target_space)
-
-        new_bounds = np.array(
-            [
-                self.current_optimal - 0.5 * self.r,
-                self.current_optimal + 0.5 * self.r
-            ]
-        ).T
-
-        self._trim(new_bounds, self.original_bounds)
-        self.bounds.append(new_bounds)
-        return self._create_bounds(target_space.keys, new_bounds)
+from typing import Optional, Union, List
+
+import numpy as np
+from .target_space import TargetSpace
+
+
+class DomainTransformer():
+    '''The base transformer class'''
+
+    def __init__(self, **kwargs):
+        pass
+
+    def initialize(self, target_space: TargetSpace):
+        raise NotImplementedError
+
+    def transform(self, target_space: TargetSpace):
+        raise NotImplementedError
+
+
+class SequentialDomainReductionTransformer(DomainTransformer):
+    """
+    A sequential domain reduction transformer bassed on the work by Stander, N. and Craig, K:
+    "On the robustness of a simple domain reduction scheme for simulation‐based optimization"
+    """
+
+    def __init__(
+        self,
+        gamma_osc: float = 0.7,
+        gamma_pan: float = 1.0,
+        eta: float = 0.9,
+        minimum_window: Optional[Union[List[float], float]] = 0.0
+    ) -> None:
+        self.gamma_osc = gamma_osc
+        self.gamma_pan = gamma_pan
+        self.eta = eta
+        self.minimum_window_value = minimum_window
+
+    def initialize(self, target_space: TargetSpace) -> None:
+        """Initialize all of the parameters"""
+        self.original_bounds = np.copy(target_space.bounds)
+        self.bounds = [self.original_bounds]
+
+        # Set the minimum window to an array of length bounds
+        if isinstance(self.minimum_window_value, list) or isinstance(self.minimum_window_value, np.ndarray):
+            assert len(self.minimum_window_value) == len(target_space.bounds)
+            self.minimum_window = self.minimum_window_value
+        else:
+            self.minimum_window = [self.minimum_window_value] * len(target_space.bounds)
+
+        self.previous_optimal = np.mean(target_space.bounds, axis=1)
+        self.current_optimal = np.mean(target_space.bounds, axis=1)
+        self.r = target_space.bounds[:, 1] - target_space.bounds[:, 0]
+
+        self.previous_d = 2.0 * \
+            (self.current_optimal - self.previous_optimal) / self.r
+
+        self.current_d = 2.0 * (self.current_optimal -
+                                self.previous_optimal) / self.r
+
+        self.c = self.current_d * self.previous_d
+        self.c_hat = np.sqrt(np.abs(self.c)) * np.sign(self.c)
+
+        self.gamma = 0.5 * (self.gamma_pan * (1.0 + self.c_hat) +
+                            self.gamma_osc * (1.0 - self.c_hat))
+
+        self.contraction_rate = self.eta + \
+            np.abs(self.current_d) * (self.gamma - self.eta)
+
+        self.r = self.contraction_rate * self.r
+
+        # check if the minimum window fits in the orignal bounds
+        self._window_bounds_compatiblity(self.original_bounds)
+
+    def _update(self, target_space: TargetSpace) -> None:
+
+        # setting the previous
+        self.previous_optimal = self.current_optimal
+        self.previous_d = self.current_d
+
+        self.current_optimal = target_space.params[
+            np.argmax(target_space.target)
+        ]
+
+        self.current_d = 2.0 * (self.current_optimal -
+                                self.previous_optimal) / self.r
+
+        self.c = self.current_d * self.previous_d
+
+        self.c_hat = np.sqrt(np.abs(self.c)) * np.sign(self.c)
+
+        self.gamma = 0.5 * (self.gamma_pan * (1.0 + self.c_hat) +
+                            self.gamma_osc * (1.0 - self.c_hat))
+
+        self.contraction_rate = self.eta + \
+            np.abs(self.current_d) * (self.gamma - self.eta)
+
+        self.r = self.contraction_rate * self.r
+
+    def _trim(self, new_bounds: np.array, global_bounds: np.array) -> np.array:
+        for i, variable in enumerate(new_bounds):
+            if variable[0] < global_bounds[i, 0]:
+                variable[0] = global_bounds[i, 0]
+            if variable[1] > global_bounds[i, 1]:
+                variable[1] = global_bounds[i, 1]
+        for i, entry in enumerate(new_bounds):
+            if entry[0] > entry[1]:
+                new_bounds[i, 0] = entry[1]
+                new_bounds[i, 1] = entry[0]
+            window_width = abs(entry[0] - entry[1])
+            if window_width < self.minimum_window[i]:
+                dw = (self.minimum_window[i] - window_width) / 2.0
+                left_expansion_space = abs(global_bounds[i, 0] - entry[0]) # should be non-positive
+                right_expansion_space = abs(global_bounds[i, 1] - entry[1]) # should be non-negative
+                # conservative
+                dw_l = min(dw, left_expansion_space)
+                dw_r = min(dw, right_expansion_space)
+                # this crawls towards the edge
+                ddw_r = dw_r + max(dw - dw_l, 0)
+                ddw_l = dw_l + max(dw - dw_r, 0)
+                new_bounds[i, 0] -= ddw_l
+                new_bounds[i, 1] += ddw_r
+        return new_bounds
+
+    def _window_bounds_compatiblity(self, global_bounds: np.array) -> bool:
+        """Checks if global bounds are compatible with the minimum window sizes."""
+        for i, entry in enumerate(global_bounds):
+            global_window_width = abs(entry[1] - entry[0])
+            if global_window_width < self.minimum_window[i]:
+                raise ValueError(
+                    "Global bounds are not compatible with the minimum window size.")
+
+    def _create_bounds(self, parameters: dict, bounds: np.array) -> dict:
+        return {param: bounds[i, :] for i, param in enumerate(parameters)}
+
+    def transform(self, target_space: TargetSpace) -> dict:
+
+        self._update(target_space)
+
+        new_bounds = np.array(
+            [
+                self.current_optimal - 0.5 * self.r,
+                self.current_optimal + 0.5 * self.r
+            ]
+        ).T
+
+        self._trim(new_bounds, self.original_bounds)
+        self.bounds.append(new_bounds)
+        return self._create_bounds(target_space.keys, new_bounds)
```

### Comparing `bayesian-optimization-1.4.2/bayes_opt/logger.py` & `bayesian-optimization-1.4.3/bayes_opt/logger.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,163 +1,163 @@
-from __future__ import print_function
-import os
-import json
-
-from .observer import _Tracker
-from .event import Events
-from .util import Colours
-
-def _get_default_logger(verbose, is_constrained):
-    return ScreenLogger(verbose=verbose, is_constrained=is_constrained)
-
-
-class ScreenLogger(_Tracker):
-    _default_cell_size = 9
-    _default_precision = 4
-
-    def __init__(self, verbose=2, is_constrained=False):
-        self._verbose = verbose
-        self._is_constrained = is_constrained
-        self._header_length = None
-        super(ScreenLogger, self).__init__()
-
-    @property
-    def verbose(self):
-        return self._verbose
-
-    @verbose.setter
-    def verbose(self, v):
-        self._verbose = v
-
-    @property
-    def is_constrained(self):
-        return self._is_constrained
-
-    def _format_number(self, x):
-        if isinstance(x, int):
-                s = "{x:<{s}}".format(
-                    x=x,
-                    s=self._default_cell_size,
-                )
-        else:
-            s = "{x:<{s}.{p}}".format(
-                x=x,
-                s=self._default_cell_size,
-                p=self._default_precision,
-            )
-
-        if len(s) > self._default_cell_size:
-            if "." in s:
-                return s[:self._default_cell_size]
-            else:
-                return s[:self._default_cell_size - 3] + "..."
-        return s
-
-    def _format_bool(self, x):
-        if 5 > self._default_cell_size:
-            if x == True:
-                x_ = 'T'
-            elif x == False:
-                x_ = 'F'
-        else:
-            x_ = str(x)
-        s = "{x:<{s}}".format(
-            x=x_,
-            s=self._default_cell_size,
-        )
-        return s
-
-    def _format_key(self, key):
-        s = "{key:^{s}}".format(
-            key=key,
-            s=self._default_cell_size
-        )
-        if len(s) > self._default_cell_size:
-            return s[:self._default_cell_size - 3] + "..."
-        return s
-
-    def _step(self, instance, colour=Colours.black):
-        res = instance.res[-1]
-        cells = []
-
-        cells.append(self._format_number(self._iterations + 1))
-        cells.append(self._format_number(res["target"]))
-        if self._is_constrained:
-            cells.append(self._format_bool(res["allowed"]))
-
-
-        for key in instance.space.keys:
-            cells.append(self._format_number(res["params"][key]))
-
-        return "| " + " | ".join(map(colour, cells)) + " |"
-
-    def _header(self, instance):
-        cells = []
-        cells.append(self._format_key("iter"))
-        cells.append(self._format_key("target"))
-
-        if self._is_constrained:
-            cells.append(self._format_key("allowed"))
-
-        for key in instance.space.keys:
-            cells.append(self._format_key(key))
-
-        line = "| " + " | ".join(cells) + " |"
-        self._header_length = len(line)
-        return line + "\n" + ("-" * self._header_length)
-
-    def _is_new_max(self, instance):
-        if instance.max["target"] is None:
-            # During constrained optimization, there might not be a maximum
-            # value since the optimizer might've not encountered any points
-            # that fulfill the constraints.
-            return False
-        if self._previous_max is None:
-            self._previous_max = instance.max["target"]
-        return instance.max["target"] > self._previous_max
-
-    def update(self, event, instance):
-        if event == Events.OPTIMIZATION_START:
-            line = self._header(instance) + "\n"
-        elif event == Events.OPTIMIZATION_STEP:
-            is_new_max = self._is_new_max(instance)
-            if self._verbose == 1 and not is_new_max:
-                line = ""
-            else:
-                colour = Colours.purple if is_new_max else Colours.black
-                line = self._step(instance, colour=colour) + "\n"
-        elif event == Events.OPTIMIZATION_END:
-            line = "=" * self._header_length + "\n"
-
-        if self._verbose:
-            print(line, end="")
-        self._update_tracker(event, instance)
-
-
-class JSONLogger(_Tracker):
-    def __init__(self, path, reset=True):
-        self._path = path if path[-5:] == ".json" else path + ".json"
-        if reset:
-            try:
-                os.remove(self._path)
-            except OSError:
-                pass
-        super(JSONLogger, self).__init__()
-
-    def update(self, event, instance):
-        if event == Events.OPTIMIZATION_STEP:
-            data = dict(instance.res[-1])
-
-            now, time_elapsed, time_delta = self._time_metrics()
-            data["datetime"] = {
-                "datetime": now,
-                "elapsed": time_elapsed,
-                "delta": time_delta,
-            }
-
-            if "allowed" in data: # fix: github.com/fmfn/BayesianOptimization/issues/361
-                data["allowed"] = bool(data["allowed"])
-
-            with open(self._path, "a") as f:
-                f.write(json.dumps(data) + "\n")
-
-        self._update_tracker(event, instance)
+from __future__ import print_function
+import os
+import json
+
+from .observer import _Tracker
+from .event import Events
+from .util import Colours
+
+def _get_default_logger(verbose, is_constrained):
+    return ScreenLogger(verbose=verbose, is_constrained=is_constrained)
+
+
+class ScreenLogger(_Tracker):
+    _default_cell_size = 9
+    _default_precision = 4
+
+    def __init__(self, verbose=2, is_constrained=False):
+        self._verbose = verbose
+        self._is_constrained = is_constrained
+        self._header_length = None
+        super(ScreenLogger, self).__init__()
+
+    @property
+    def verbose(self):
+        return self._verbose
+
+    @verbose.setter
+    def verbose(self, v):
+        self._verbose = v
+
+    @property
+    def is_constrained(self):
+        return self._is_constrained
+
+    def _format_number(self, x):
+        if isinstance(x, int):
+                s = "{x:<{s}}".format(
+                    x=x,
+                    s=self._default_cell_size,
+                )
+        else:
+            s = "{x:<{s}.{p}}".format(
+                x=x,
+                s=self._default_cell_size,
+                p=self._default_precision,
+            )
+
+        if len(s) > self._default_cell_size:
+            if "." in s:
+                return s[:self._default_cell_size]
+            else:
+                return s[:self._default_cell_size - 3] + "..."
+        return s
+
+    def _format_bool(self, x):
+        if 5 > self._default_cell_size:
+            if x == True:
+                x_ = 'T'
+            elif x == False:
+                x_ = 'F'
+        else:
+            x_ = str(x)
+        s = "{x:<{s}}".format(
+            x=x_,
+            s=self._default_cell_size,
+        )
+        return s
+
+    def _format_key(self, key):
+        s = "{key:^{s}}".format(
+            key=key,
+            s=self._default_cell_size
+        )
+        if len(s) > self._default_cell_size:
+            return s[:self._default_cell_size - 3] + "..."
+        return s
+
+    def _step(self, instance, colour=Colours.black):
+        res = instance.res[-1]
+        cells = []
+
+        cells.append(self._format_number(self._iterations + 1))
+        cells.append(self._format_number(res["target"]))
+        if self._is_constrained:
+            cells.append(self._format_bool(res["allowed"]))
+
+
+        for key in instance.space.keys:
+            cells.append(self._format_number(res["params"][key]))
+
+        return "| " + " | ".join(map(colour, cells)) + " |"
+
+    def _header(self, instance):
+        cells = []
+        cells.append(self._format_key("iter"))
+        cells.append(self._format_key("target"))
+
+        if self._is_constrained:
+            cells.append(self._format_key("allowed"))
+
+        for key in instance.space.keys:
+            cells.append(self._format_key(key))
+
+        line = "| " + " | ".join(cells) + " |"
+        self._header_length = len(line)
+        return line + "\n" + ("-" * self._header_length)
+
+    def _is_new_max(self, instance):
+        if instance.max["target"] is None:
+            # During constrained optimization, there might not be a maximum
+            # value since the optimizer might've not encountered any points
+            # that fulfill the constraints.
+            return False
+        if self._previous_max is None:
+            self._previous_max = instance.max["target"]
+        return instance.max["target"] > self._previous_max
+
+    def update(self, event, instance):
+        if event == Events.OPTIMIZATION_START:
+            line = self._header(instance) + "\n"
+        elif event == Events.OPTIMIZATION_STEP:
+            is_new_max = self._is_new_max(instance)
+            if self._verbose == 1 and not is_new_max:
+                line = ""
+            else:
+                colour = Colours.purple if is_new_max else Colours.black
+                line = self._step(instance, colour=colour) + "\n"
+        elif event == Events.OPTIMIZATION_END:
+            line = "=" * self._header_length + "\n"
+
+        if self._verbose:
+            print(line, end="")
+        self._update_tracker(event, instance)
+
+
+class JSONLogger(_Tracker):
+    def __init__(self, path, reset=True):
+        self._path = path if path[-5:] == ".json" else path + ".json"
+        if reset:
+            try:
+                os.remove(self._path)
+            except OSError:
+                pass
+        super(JSONLogger, self).__init__()
+
+    def update(self, event, instance):
+        if event == Events.OPTIMIZATION_STEP:
+            data = dict(instance.res[-1])
+
+            now, time_elapsed, time_delta = self._time_metrics()
+            data["datetime"] = {
+                "datetime": now,
+                "elapsed": time_elapsed,
+                "delta": time_delta,
+            }
+
+            if "allowed" in data: # fix: github.com/fmfn/BayesianOptimization/issues/361
+                data["allowed"] = bool(data["allowed"])
+
+            with open(self._path, "a") as f:
+                f.write(json.dumps(data) + "\n")
+
+        self._update_tracker(event, instance)
```

### Comparing `bayesian-optimization-1.4.2/bayes_opt/observer.py` & `bayesian-optimization-1.4.3/bayes_opt/observer.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-"""
-observers...
-"""
-from datetime import datetime
-from .event import Events
-
-
-class Observer:
-    def update(self, event, instance):
-        raise NotImplementedError
-
-
-class _Tracker(object):
-    def __init__(self):
-        self._iterations = 0
-
-        self._previous_max = None
-        self._previous_max_params = None
-
-        self._start_time = None
-        self._previous_time = None
-
-    def _update_tracker(self, event, instance):
-        if event == Events.OPTIMIZATION_STEP:
-            self._iterations += 1
-
-            current_max = instance.max
-            if (self._previous_max is None
-                    or current_max["target"] > self._previous_max):
-                self._previous_max = current_max["target"]
-                self._previous_max_params = current_max["params"]
-
-    def _time_metrics(self):
-        now = datetime.now()
-        if self._start_time is None:
-            self._start_time = now
-        if self._previous_time is None:
-            self._previous_time = now
-
-        time_elapsed = now - self._start_time
-        time_delta = now - self._previous_time
-
-        self._previous_time = now
-        return (
-            now.strftime("%Y-%m-%d %H:%M:%S"),
-            time_elapsed.total_seconds(),
-            time_delta.total_seconds()
-        )
+"""
+observers...
+"""
+from datetime import datetime
+from .event import Events
+
+
+class Observer:
+    def update(self, event, instance):
+        raise NotImplementedError
+
+
+class _Tracker(object):
+    def __init__(self):
+        self._iterations = 0
+
+        self._previous_max = None
+        self._previous_max_params = None
+
+        self._start_time = None
+        self._previous_time = None
+
+    def _update_tracker(self, event, instance):
+        if event == Events.OPTIMIZATION_STEP:
+            self._iterations += 1
+
+            current_max = instance.max
+            if (self._previous_max is None
+                    or current_max["target"] > self._previous_max):
+                self._previous_max = current_max["target"]
+                self._previous_max_params = current_max["params"]
+
+    def _time_metrics(self):
+        now = datetime.now()
+        if self._start_time is None:
+            self._start_time = now
+        if self._previous_time is None:
+            self._previous_time = now
+
+        time_elapsed = now - self._start_time
+        time_delta = now - self._previous_time
+
+        self._previous_time = now
+        return (
+            now.strftime("%Y-%m-%d %H:%M:%S"),
+            time_elapsed.total_seconds(),
+            time_delta.total_seconds()
+        )
```

### Comparing `bayesian-optimization-1.4.2/bayes_opt/util.py` & `bayesian-optimization-1.4.3/bayes_opt/util.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,301 +1,301 @@
-import warnings
-import numpy as np
-from scipy.stats import norm
-from scipy.optimize import minimize
-from colorama import just_fix_windows_console
-
-
-def acq_max(ac, gp, y_max, bounds, random_state, constraint=None, n_warmup=10000, n_iter=10):
-    """
-    A function to find the maximum of the acquisition function
-
-    It uses a combination of random sampling (cheap) and the 'L-BFGS-B'
-    optimization method. First by sampling `n_warmup` (1e5) points at random,
-    and then running L-BFGS-B from `n_iter` (250) random starting points.
-
-    Parameters
-    ----------
-    :param ac:
-        The acquisition function object that return its point-wise value.
-
-    :param gp:
-        A gaussian process fitted to the relevant data.
-
-    :param y_max:
-        The current maximum known value of the target function.
-
-    :param bounds:
-        The variables bounds to limit the search of the acq max.
-
-    :param random_state:
-        instance of np.RandomState random number generator
-
-    :param constraint:
-        A ConstraintModel.
-
-    :param n_warmup:
-        number of times to randomly sample the acquisition function
-
-    :param n_iter:
-        number of times to run scipy.minimize
-
-    Returns
-    -------
-    :return: x_max, The arg max of the acquisition function.
-    """
-
-    # Warm up with random points
-    x_tries = random_state.uniform(bounds[:, 0], bounds[:, 1],
-                                   size=(n_warmup, bounds.shape[0]))
-    ys = ac(x_tries, gp=gp, y_max=y_max)
-    x_max = x_tries[ys.argmax()]
-    max_acq = ys.max()
-
-    # Explore the parameter space more throughly
-    x_seeds = random_state.uniform(bounds[:, 0], bounds[:, 1],
-                                   size=(n_iter, bounds.shape[0]))
-
-    if constraint is not None:
-        def to_minimize(x):
-            target = -ac(x.reshape(1, -1), gp=gp, y_max=y_max)
-            p_constraint = constraint.predict(x.reshape(1, -1))
-
-            # TODO: This is not exactly how Gardner et al do it.
-            # Their way would require the result of the acquisition function
-            # to be strictly positive (or negative), which is not the case
-            # here. For a negative target value, we use Gardner's version. If
-            # the target is positive, we instead slightly rescale the target
-            # depending on the probability estimate to fulfill the constraint.
-            if target < 0:
-                return target * p_constraint
-            else:
-                return target / (0.5 + p_constraint)
-    else:
-        to_minimize = lambda x: -ac(x.reshape(1, -1), gp=gp, y_max=y_max)
-
-    for x_try in x_seeds:
-        # Find the minimum of minus the acquisition function
-        res = minimize(lambda x: to_minimize(x),
-                       x_try,
-                       bounds=bounds,
-                       method="L-BFGS-B")
-
-        # See if success
-        if not res.success:
-            continue
-
-        # Store it if better than previous minimum(maximum).
-        if max_acq is None or -np.squeeze(res.fun) >= max_acq:
-            x_max = res.x
-            max_acq = -np.squeeze(res.fun)
-
-    # Clip output to make sure it lies within the bounds. Due to floating
-    # point technicalities this is not always the case.
-    return np.clip(x_max, bounds[:, 0], bounds[:, 1])
-
-
-class UtilityFunction(object):
-    """
-    An object to compute the acquisition functions.
-
-    kind: {'ucb', 'ei', 'poi'}
-        * 'ucb' stands for the Upper Confidence Bounds method
-        * 'ei' is the Expected Improvement method
-        * 'poi' is the Probability Of Improvement criterion.
-
-    kappa: float, optional(default=2.576)
-            Parameter to indicate how closed are the next parameters sampled.
-            Higher value = favors spaces that are least explored.
-            Lower value = favors spaces where the regression function is
-            the highest.
-
-    kappa_decay: float, optional(default=1)
-        `kappa` is multiplied by this factor every iteration.
-
-    kappa_decay_delay: int, optional(default=0)
-        Number of iterations that must have passed before applying the
-        decay to `kappa`.
-
-    xi: float, optional(default=0.0)
-    """
-
-    def __init__(self, kind='ucb', kappa=2.576, xi=0, kappa_decay=1, kappa_decay_delay=0):
-
-        self.kappa = kappa
-        self._kappa_decay = kappa_decay
-        self._kappa_decay_delay = kappa_decay_delay
-
-        self.xi = xi
-
-        self._iters_counter = 0
-
-        if kind not in ['ucb', 'ei', 'poi']:
-            err = "The utility function " \
-                  "{} has not been implemented, " \
-                  "please choose one of ucb, ei, or poi.".format(kind)
-            raise NotImplementedError(err)
-        else:
-            self.kind = kind
-
-    def update_params(self):
-        self._iters_counter += 1
-
-        if self._kappa_decay < 1 and self._iters_counter > self._kappa_decay_delay:
-            self.kappa *= self._kappa_decay
-
-    def utility(self, x, gp, y_max):
-        if self.kind == 'ucb':
-            return self._ucb(x, gp, self.kappa)
-        if self.kind == 'ei':
-            return self._ei(x, gp, y_max, self.xi)
-        if self.kind == 'poi':
-            return self._poi(x, gp, y_max, self.xi)
-
-    @staticmethod
-    def _ucb(x, gp, kappa):
-        with warnings.catch_warnings():
-            warnings.simplefilter("ignore")
-            mean, std = gp.predict(x, return_std=True)
-
-        return mean + kappa * std
-
-    @staticmethod
-    def _ei(x, gp, y_max, xi):
-        with warnings.catch_warnings():
-            warnings.simplefilter("ignore")
-            mean, std = gp.predict(x, return_std=True)
-
-        a = (mean - y_max - xi)
-        z = a / std
-        return a * norm.cdf(z) + std * norm.pdf(z)
-
-    @staticmethod
-    def _poi(x, gp, y_max, xi):
-        with warnings.catch_warnings():
-            warnings.simplefilter("ignore")
-            mean, std = gp.predict(x, return_std=True)
-
-        z = (mean - y_max - xi)/std
-        return norm.cdf(z)
-
-
-class NotUniqueError(Exception):
-    """A point is non-unique."""
-    pass
-
-
-def load_logs(optimizer, logs):
-    """Load previous ...
-
-    """
-    import json
-
-    if isinstance(logs, str):
-        logs = [logs]
-
-    for log in logs:
-        with open(log, "r") as j:
-            while True:
-                try:
-                    iteration = next(j)
-                except StopIteration:
-                    break
-
-                iteration = json.loads(iteration)
-                try:
-                    optimizer.register(
-                        params=iteration["params"],
-                        target=iteration["target"],
-                        constraint_value=iteration["constraint"] if optimizer.is_constrained else None
-                    )
-                except NotUniqueError:
-                    continue
-
-    return optimizer
-
-
-def ensure_rng(random_state=None):
-    """
-    Creates a random number generator based on an optional seed.  This can be
-    an integer or another random state for a seeded rng, or None for an
-    unseeded rng.
-    """
-    if random_state is None:
-        random_state = np.random.RandomState()
-    elif isinstance(random_state, int):
-        random_state = np.random.RandomState(random_state)
-    else:
-        assert isinstance(random_state, np.random.RandomState)
-    return random_state
-
-
-class Colours:
-    """Print in nice colours."""
-
-    BLUE = '\033[94m'
-    BOLD = '\033[1m'
-    CYAN = '\033[96m'
-    DARKCYAN = '\033[36m'
-    END = '\033[0m'
-    GREEN = '\033[92m'
-    PURPLE = '\033[95m'
-    RED = '\033[91m'
-    UNDERLINE = '\033[4m'
-    YELLOW = '\033[93m'
-
-    @classmethod
-    def _wrap_colour(cls, s, colour):
-        return colour + s + cls.END
-
-    @classmethod
-    def black(cls, s):
-        """Wrap text in black."""
-        return cls._wrap_colour(s, cls.END)
-
-    @classmethod
-    def blue(cls, s):
-        """Wrap text in blue."""
-        return cls._wrap_colour(s, cls.BLUE)
-
-    @classmethod
-    def bold(cls, s):
-        """Wrap text in bold."""
-        return cls._wrap_colour(s, cls.BOLD)
-
-    @classmethod
-    def cyan(cls, s):
-        """Wrap text in cyan."""
-        return cls._wrap_colour(s, cls.CYAN)
-
-    @classmethod
-    def darkcyan(cls, s):
-        """Wrap text in darkcyan."""
-        return cls._wrap_colour(s, cls.DARKCYAN)
-
-    @classmethod
-    def green(cls, s):
-        """Wrap text in green."""
-        return cls._wrap_colour(s, cls.GREEN)
-
-    @classmethod
-    def purple(cls, s):
-        """Wrap text in purple."""
-        return cls._wrap_colour(s, cls.PURPLE)
-
-    @classmethod
-    def red(cls, s):
-        """Wrap text in red."""
-        return cls._wrap_colour(s, cls.RED)
-
-    @classmethod
-    def underline(cls, s):
-        """Wrap text in underline."""
-        return cls._wrap_colour(s, cls.UNDERLINE)
-
-    @classmethod
-    def yellow(cls, s):
-        """Wrap text in yellow."""
-        return cls._wrap_colour(s, cls.YELLOW)
-
-
-just_fix_windows_console()
+import warnings
+import numpy as np
+from scipy.stats import norm
+from scipy.optimize import minimize
+from colorama import just_fix_windows_console
+
+
+def acq_max(ac, gp, y_max, bounds, random_state, constraint=None, n_warmup=10000, n_iter=10):
+    """
+    A function to find the maximum of the acquisition function
+
+    It uses a combination of random sampling (cheap) and the 'L-BFGS-B'
+    optimization method. First by sampling `n_warmup` (1e5) points at random,
+    and then running L-BFGS-B from `n_iter` (250) random starting points.
+
+    Parameters
+    ----------
+    :param ac:
+        The acquisition function object that return its point-wise value.
+
+    :param gp:
+        A gaussian process fitted to the relevant data.
+
+    :param y_max:
+        The current maximum known value of the target function.
+
+    :param bounds:
+        The variables bounds to limit the search of the acq max.
+
+    :param random_state:
+        instance of np.RandomState random number generator
+
+    :param constraint:
+        A ConstraintModel.
+
+    :param n_warmup:
+        number of times to randomly sample the acquisition function
+
+    :param n_iter:
+        number of times to run scipy.minimize
+
+    Returns
+    -------
+    :return: x_max, The arg max of the acquisition function.
+    """
+
+    # Warm up with random points
+    x_tries = random_state.uniform(bounds[:, 0], bounds[:, 1],
+                                   size=(n_warmup, bounds.shape[0]))
+    ys = ac(x_tries, gp=gp, y_max=y_max)
+    x_max = x_tries[ys.argmax()]
+    max_acq = ys.max()
+
+    # Explore the parameter space more throughly
+    x_seeds = random_state.uniform(bounds[:, 0], bounds[:, 1],
+                                   size=(n_iter, bounds.shape[0]))
+
+    if constraint is not None:
+        def to_minimize(x):
+            target = -ac(x.reshape(1, -1), gp=gp, y_max=y_max)
+            p_constraint = constraint.predict(x.reshape(1, -1))
+
+            # TODO: This is not exactly how Gardner et al do it.
+            # Their way would require the result of the acquisition function
+            # to be strictly positive (or negative), which is not the case
+            # here. For a negative target value, we use Gardner's version. If
+            # the target is positive, we instead slightly rescale the target
+            # depending on the probability estimate to fulfill the constraint.
+            if target < 0:
+                return target * p_constraint
+            else:
+                return target / (0.5 + p_constraint)
+    else:
+        to_minimize = lambda x: -ac(x.reshape(1, -1), gp=gp, y_max=y_max)
+
+    for x_try in x_seeds:
+        # Find the minimum of minus the acquisition function
+        res = minimize(lambda x: to_minimize(x),
+                       x_try,
+                       bounds=bounds,
+                       method="L-BFGS-B")
+
+        # See if success
+        if not res.success:
+            continue
+
+        # Store it if better than previous minimum(maximum).
+        if max_acq is None or -np.squeeze(res.fun) >= max_acq:
+            x_max = res.x
+            max_acq = -np.squeeze(res.fun)
+
+    # Clip output to make sure it lies within the bounds. Due to floating
+    # point technicalities this is not always the case.
+    return np.clip(x_max, bounds[:, 0], bounds[:, 1])
+
+
+class UtilityFunction(object):
+    """
+    An object to compute the acquisition functions.
+
+    kind: {'ucb', 'ei', 'poi'}
+        * 'ucb' stands for the Upper Confidence Bounds method
+        * 'ei' is the Expected Improvement method
+        * 'poi' is the Probability Of Improvement criterion.
+
+    kappa: float, optional(default=2.576)
+            Parameter to indicate how closed are the next parameters sampled.
+            Higher value = favors spaces that are least explored.
+            Lower value = favors spaces where the regression function is
+            the highest.
+
+    kappa_decay: float, optional(default=1)
+        `kappa` is multiplied by this factor every iteration.
+
+    kappa_decay_delay: int, optional(default=0)
+        Number of iterations that must have passed before applying the
+        decay to `kappa`.
+
+    xi: float, optional(default=0.0)
+    """
+
+    def __init__(self, kind='ucb', kappa=2.576, xi=0, kappa_decay=1, kappa_decay_delay=0):
+
+        self.kappa = kappa
+        self._kappa_decay = kappa_decay
+        self._kappa_decay_delay = kappa_decay_delay
+
+        self.xi = xi
+
+        self._iters_counter = 0
+
+        if kind not in ['ucb', 'ei', 'poi']:
+            err = "The utility function " \
+                  "{} has not been implemented, " \
+                  "please choose one of ucb, ei, or poi.".format(kind)
+            raise NotImplementedError(err)
+        else:
+            self.kind = kind
+
+    def update_params(self):
+        self._iters_counter += 1
+
+        if self._kappa_decay < 1 and self._iters_counter > self._kappa_decay_delay:
+            self.kappa *= self._kappa_decay
+
+    def utility(self, x, gp, y_max):
+        if self.kind == 'ucb':
+            return self._ucb(x, gp, self.kappa)
+        if self.kind == 'ei':
+            return self._ei(x, gp, y_max, self.xi)
+        if self.kind == 'poi':
+            return self._poi(x, gp, y_max, self.xi)
+
+    @staticmethod
+    def _ucb(x, gp, kappa):
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            mean, std = gp.predict(x, return_std=True)
+
+        return mean + kappa * std
+
+    @staticmethod
+    def _ei(x, gp, y_max, xi):
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            mean, std = gp.predict(x, return_std=True)
+
+        a = (mean - y_max - xi)
+        z = a / std
+        return a * norm.cdf(z) + std * norm.pdf(z)
+
+    @staticmethod
+    def _poi(x, gp, y_max, xi):
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            mean, std = gp.predict(x, return_std=True)
+
+        z = (mean - y_max - xi)/std
+        return norm.cdf(z)
+
+
+class NotUniqueError(Exception):
+    """A point is non-unique."""
+    pass
+
+
+def load_logs(optimizer, logs):
+    """Load previous ...
+
+    """
+    import json
+
+    if isinstance(logs, str):
+        logs = [logs]
+
+    for log in logs:
+        with open(log, "r") as j:
+            while True:
+                try:
+                    iteration = next(j)
+                except StopIteration:
+                    break
+
+                iteration = json.loads(iteration)
+                try:
+                    optimizer.register(
+                        params=iteration["params"],
+                        target=iteration["target"],
+                        constraint_value=iteration["constraint"] if optimizer.is_constrained else None
+                    )
+                except NotUniqueError:
+                    continue
+
+    return optimizer
+
+
+def ensure_rng(random_state=None):
+    """
+    Creates a random number generator based on an optional seed.  This can be
+    an integer or another random state for a seeded rng, or None for an
+    unseeded rng.
+    """
+    if random_state is None:
+        random_state = np.random.RandomState()
+    elif isinstance(random_state, int):
+        random_state = np.random.RandomState(random_state)
+    else:
+        assert isinstance(random_state, np.random.RandomState)
+    return random_state
+
+
+class Colours:
+    """Print in nice colours."""
+
+    BLUE = '\033[94m'
+    BOLD = '\033[1m'
+    CYAN = '\033[96m'
+    DARKCYAN = '\033[36m'
+    END = '\033[0m'
+    GREEN = '\033[92m'
+    PURPLE = '\033[95m'
+    RED = '\033[91m'
+    UNDERLINE = '\033[4m'
+    YELLOW = '\033[93m'
+
+    @classmethod
+    def _wrap_colour(cls, s, colour):
+        return colour + s + cls.END
+
+    @classmethod
+    def black(cls, s):
+        """Wrap text in black."""
+        return cls._wrap_colour(s, cls.END)
+
+    @classmethod
+    def blue(cls, s):
+        """Wrap text in blue."""
+        return cls._wrap_colour(s, cls.BLUE)
+
+    @classmethod
+    def bold(cls, s):
+        """Wrap text in bold."""
+        return cls._wrap_colour(s, cls.BOLD)
+
+    @classmethod
+    def cyan(cls, s):
+        """Wrap text in cyan."""
+        return cls._wrap_colour(s, cls.CYAN)
+
+    @classmethod
+    def darkcyan(cls, s):
+        """Wrap text in darkcyan."""
+        return cls._wrap_colour(s, cls.DARKCYAN)
+
+    @classmethod
+    def green(cls, s):
+        """Wrap text in green."""
+        return cls._wrap_colour(s, cls.GREEN)
+
+    @classmethod
+    def purple(cls, s):
+        """Wrap text in purple."""
+        return cls._wrap_colour(s, cls.PURPLE)
+
+    @classmethod
+    def red(cls, s):
+        """Wrap text in red."""
+        return cls._wrap_colour(s, cls.RED)
+
+    @classmethod
+    def underline(cls, s):
+        """Wrap text in underline."""
+        return cls._wrap_colour(s, cls.UNDERLINE)
+
+    @classmethod
+    def yellow(cls, s):
+        """Wrap text in yellow."""
+        return cls._wrap_colour(s, cls.YELLOW)
+
+
+just_fix_windows_console()
```

