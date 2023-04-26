# Comparing `tmp/pyrlprob-2.0.2.tar.gz` & `tmp/pyrlprob-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrlprob-2.0.2.tar", last modified: Fri Apr 21 21:40:33 2023, max compression
+gzip compressed data, was "pyrlprob-2.0.3.tar", last modified: Tue Apr 25 19:26:18 2023, max compression
```

## Comparing `pyrlprob-2.0.2.tar` & `pyrlprob-2.0.3.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-21 21:40:33.700507 pyrlprob-2.0.2/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1073 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/LICENSE.txt
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      301 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/MANIFEST.in
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     2322 2023-04-21 21:40:33.698510 pyrlprob-2.0.2/PKG-INFO
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1803 2023-03-08 19:07:40.000000 pyrlprob-2.0.2/README.md
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      103 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyproject.toml
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-21 21:40:33.462508 pyrlprob-2.0.2/pyrlprob/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      250 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/__init__.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1157 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/__main__.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)    15337 2023-04-21 21:39:44.000000 pyrlprob-2.0.2/pyrlprob/base_funs.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      661 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/commands.py
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-21 21:40:33.415509 pyrlprob-2.0.2/pyrlprob/include/
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-21 21:40:33.499506 pyrlprob-2.0.2/pyrlprob/include/pyrlprob/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     2938 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/include/pyrlprob/binding.cpp
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     5140 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/include/pyrlprob/mdp.h
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     3818 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/include/pyrlprob/mdp_vec.h
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     4114 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/include/pyrlprob/py_mdp.h
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     7448 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/mdp.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)    12688 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/problem.py
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-21 21:40:33.526506 pyrlprob-2.0.2/pyrlprob/tests/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      477 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/__init__.py
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-21 21:40:33.573509 pyrlprob-2.0.2/pyrlprob/tests/cpp_tests/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      210 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/cpp_tests/__init__.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      390 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/cpp_tests/binding.cpp
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     6849 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/cpp_tests/landing1d.cpp
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     2063 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/cpp_tests/landing1d.h
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1830 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/cpp_tests/landing1d.py
--rwx------   0 lorenzof (1001204911) domain users (1000000513)   463776 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/cpp_tests/landing1d_cpp.cpython-39-x86_64-linux-gnu.so
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      696 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/cpp_tests/landing1d_dyn.h
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1405 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/cpp_tests/rk4.h
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1282 2023-03-08 18:08:23.000000 pyrlprob-2.0.2/pyrlprob/tests/landing1d_cpp.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1574 2023-04-21 21:36:35.000000 pyrlprob-2.0.2/pyrlprob/tests/landing1d_load.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1266 2023-04-21 21:39:57.000000 pyrlprob-2.0.2/pyrlprob/tests/landing1d_py.yaml
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-21 21:40:33.590507 pyrlprob-2.0.2/pyrlprob/tests/py_tests/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      190 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/__init__.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     4713 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/landing1d.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      974 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/landing1d_dyn.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     6161 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/landing1d_gym.py
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-21 21:40:33.675507 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      428 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_A2C.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      691 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_DQN.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      331 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PG.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      560 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PPO.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1064 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_SAC.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      496 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_A2C.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      433 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_DQN.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      432 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PG.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      558 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PPO.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      713 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_SAC.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      520 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Landing1D_A2C.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      456 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PG.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      582 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PPO.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      732 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Landing1D_SAC.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      639 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Landing1D_TD3.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      497 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_A2C.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      432 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PG.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      558 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PPO.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      714 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_SAC.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      615 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_TD3.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     5273 2023-04-21 21:13:31.000000 pyrlprob-2.0.2/pyrlprob/tests/test_landing1d.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     2813 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/test_multiple_gym.py
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-21 21:40:33.692508 pyrlprob-2.0.2/pyrlprob/utils/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      546 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/utils/__init__.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     3183 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/utils/auxiliary.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     4709 2023-04-21 21:23:43.000000 pyrlprob-2.0.2/pyrlprob/utils/callbacks.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     3036 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/utils/plots.py
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-21 21:40:33.482508 pyrlprob-2.0.2/pyrlprob.egg-info/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     2322 2023-04-21 21:40:33.000000 pyrlprob-2.0.2/pyrlprob.egg-info/PKG-INFO
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     2454 2023-04-21 21:40:33.000000 pyrlprob-2.0.2/pyrlprob.egg-info/SOURCES.txt
--rw-------   0 lorenzof (1001204911) domain users (1000000513)        1 2023-04-21 21:40:33.000000 pyrlprob-2.0.2/pyrlprob.egg-info/dependency_links.txt
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      194 2023-04-21 21:40:33.000000 pyrlprob-2.0.2/pyrlprob.egg-info/requires.txt
--rw-------   0 lorenzof (1001204911) domain users (1000000513)        9 2023-04-21 21:40:33.000000 pyrlprob-2.0.2/pyrlprob.egg-info/top_level.txt
--rw-------   0 lorenzof (1001204911) domain users (1000000513)       38 2023-04-21 21:40:33.700512 pyrlprob-2.0.2/setup.cfg
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1242 2023-04-21 21:40:04.000000 pyrlprob-2.0.2/setup.py
+drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-25 19:26:18.626211 pyrlprob-2.0.3/
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     1073 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/LICENSE.txt
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      301 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/MANIFEST.in
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     2322 2023-04-25 19:26:18.625215 pyrlprob-2.0.3/PKG-INFO
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     1803 2023-03-08 19:07:40.000000 pyrlprob-2.0.3/README.md
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      103 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyproject.toml
+drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-25 19:26:18.343208 pyrlprob-2.0.3/pyrlprob/
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      250 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/__init__.py
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     1157 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/__main__.py
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)    15337 2023-04-21 21:39:44.000000 pyrlprob-2.0.3/pyrlprob/base_funs.py
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      661 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/commands.py
+drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-25 19:26:18.277208 pyrlprob-2.0.3/pyrlprob/include/
+drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-25 19:26:18.370209 pyrlprob-2.0.3/pyrlprob/include/pyrlprob/
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     2938 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/include/pyrlprob/binding.cpp
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     5140 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/include/pyrlprob/mdp.h
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     3818 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/include/pyrlprob/mdp_vec.h
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     4114 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/include/pyrlprob/py_mdp.h
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     7448 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/mdp.py
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)    12688 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/problem.py
+drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-25 19:26:18.447207 pyrlprob-2.0.3/pyrlprob/tests/
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      477 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/__init__.py
+drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-25 19:26:18.527209 pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      210 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/__init__.py
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      390 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/binding.cpp
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     6849 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/landing1d.cpp
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     2063 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/landing1d.h
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     1830 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/landing1d.py
+-rwx------   0 lorenzof (1001204911) domain users (1000000513)   463776 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/landing1d_cpp.cpython-39-x86_64-linux-gnu.so
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      696 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/landing1d_dyn.h
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     1405 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/rk4.h
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     1282 2023-03-08 18:08:23.000000 pyrlprob-2.0.3/pyrlprob/tests/landing1d_cpp.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     1574 2023-04-21 21:36:35.000000 pyrlprob-2.0.3/pyrlprob/tests/landing1d_load.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     1266 2023-04-21 21:39:57.000000 pyrlprob-2.0.3/pyrlprob/tests/landing1d_py.yaml
+drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-25 19:26:18.539206 pyrlprob-2.0.3/pyrlprob/tests/py_tests/
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      190 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/__init__.py
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     4713 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/landing1d.py
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      974 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/landing1d_dyn.py
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     6161 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/landing1d_gym.py
+drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-25 19:26:18.611210 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      428 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_A2C.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      691 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_DQN.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      331 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PG.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      560 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PPO.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     1064 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_SAC.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      496 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_A2C.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      433 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_DQN.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      432 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PG.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      558 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PPO.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      713 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_SAC.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      520 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_A2C.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      456 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PG.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      582 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PPO.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      732 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_SAC.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      639 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_TD3.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      497 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_A2C.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      432 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PG.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      558 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PPO.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      714 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_SAC.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      615 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_TD3.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     5273 2023-04-21 21:13:31.000000 pyrlprob-2.0.3/pyrlprob/tests/test_landing1d.py
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     2813 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/test_multiple_gym.py
+drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-25 19:26:18.623205 pyrlprob-2.0.3/pyrlprob/utils/
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      546 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/utils/__init__.py
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     3183 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/utils/auxiliary.py
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     4637 2023-04-25 19:25:53.000000 pyrlprob-2.0.3/pyrlprob/utils/callbacks.py
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     3036 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/utils/plots.py
+drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-25 19:26:18.357207 pyrlprob-2.0.3/pyrlprob.egg-info/
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     2322 2023-04-25 19:26:18.000000 pyrlprob-2.0.3/pyrlprob.egg-info/PKG-INFO
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     2454 2023-04-25 19:26:18.000000 pyrlprob-2.0.3/pyrlprob.egg-info/SOURCES.txt
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)        1 2023-04-25 19:26:18.000000 pyrlprob-2.0.3/pyrlprob.egg-info/dependency_links.txt
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      194 2023-04-25 19:26:18.000000 pyrlprob-2.0.3/pyrlprob.egg-info/requires.txt
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)        9 2023-04-25 19:26:18.000000 pyrlprob-2.0.3/pyrlprob.egg-info/top_level.txt
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)       38 2023-04-25 19:26:18.627209 pyrlprob-2.0.3/setup.cfg
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     1242 2023-04-25 19:25:59.000000 pyrlprob-2.0.3/setup.py
```

### Comparing `pyrlprob-2.0.2/LICENSE.txt` & `pyrlprob-2.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/PKG-INFO` & `pyrlprob-2.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrlprob
-Version: 2.0.2
+Version: 2.0.3
 Summary: Train Gym-derived environments in Python/C++ through Ray RLlib
 Home-page: https://github.com/LorenzoFederici/pyrlprob
 Author: Lorenzo Federici
 Author-email: federicilorenzo94@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyrlprob-2.0.2/README.md` & `pyrlprob-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/__main__.py` & `pyrlprob-2.0.3/pyrlprob/__main__.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/base_funs.py` & `pyrlprob-2.0.3/pyrlprob/base_funs.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/commands.py` & `pyrlprob-2.0.3/pyrlprob/commands.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/include/pyrlprob/binding.cpp` & `pyrlprob-2.0.3/pyrlprob/include/pyrlprob/binding.cpp`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/include/pyrlprob/mdp.h` & `pyrlprob-2.0.3/pyrlprob/include/pyrlprob/mdp.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/include/pyrlprob/mdp_vec.h` & `pyrlprob-2.0.3/pyrlprob/include/pyrlprob/mdp_vec.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/include/pyrlprob/py_mdp.h` & `pyrlprob-2.0.3/pyrlprob/include/pyrlprob/py_mdp.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/mdp.py` & `pyrlprob-2.0.3/pyrlprob/mdp.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/problem.py` & `pyrlprob-2.0.3/pyrlprob/problem.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/tests/cpp_tests/landing1d.cpp` & `pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/landing1d.cpp`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/tests/cpp_tests/landing1d.h` & `pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/landing1d.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/tests/cpp_tests/landing1d.py` & `pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/landing1d.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/tests/cpp_tests/landing1d_cpp.cpython-39-x86_64-linux-gnu.so` & `pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/landing1d_cpp.cpython-39-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/tests/cpp_tests/landing1d_dyn.h` & `pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/landing1d_dyn.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/tests/cpp_tests/rk4.h` & `pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/rk4.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/tests/landing1d_cpp.yaml` & `pyrlprob-2.0.3/pyrlprob/tests/landing1d_cpp.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/tests/landing1d_load.yaml` & `pyrlprob-2.0.3/pyrlprob/tests/landing1d_load.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/tests/landing1d_py.yaml` & `pyrlprob-2.0.3/pyrlprob/tests/landing1d_py.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/tests/py_tests/landing1d.py` & `pyrlprob-2.0.3/pyrlprob/tests/py_tests/landing1d.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/tests/py_tests/landing1d_dyn.py` & `pyrlprob-2.0.3/pyrlprob/tests/py_tests/landing1d_dyn.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/tests/py_tests/landing1d_gym.py` & `pyrlprob-2.0.3/pyrlprob/tests/py_tests/landing1d_gym.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_DQN.yaml` & `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_DQN.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PPO.yaml` & `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PPO.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_SAC.yaml` & `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_SAC.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PPO.yaml` & `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PPO.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_SAC.yaml` & `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_SAC.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Landing1D_A2C.yaml` & `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_A2C.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PPO.yaml` & `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PPO.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Landing1D_SAC.yaml` & `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_SAC.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Landing1D_TD3.yaml` & `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_TD3.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PPO.yaml` & `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PPO.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_SAC.yaml` & `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_SAC.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_TD3.yaml` & `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_TD3.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/tests/test_landing1d.py` & `pyrlprob-2.0.3/pyrlprob/tests/test_landing1d.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/tests/test_multiple_gym.py` & `pyrlprob-2.0.3/pyrlprob/tests/test_multiple_gym.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/utils/__init__.py` & `pyrlprob-2.0.3/pyrlprob/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/utils/auxiliary.py` & `pyrlprob-2.0.3/pyrlprob/utils/auxiliary.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob/utils/callbacks.py` & `pyrlprob-2.0.3/pyrlprob/utils/callbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,14 @@
         info = episode.last_info_for()
 
         if info is not None:
             if "episode_step_data" in info:
                 for key in info["episode_step_data"].keys():
                     episode.hist_data[key] = episode.user_data[key]
                     episode.hist_data[key + "_length"] = [len(episode.user_data[key])]
-                    print("episode_step_data end callback: data added")
             if "episode_end_data" in info:
                 for key, item in info["episode_end_data"].items():
                     if isinstance(item, Iterable):
                         episode.hist_data[key] = [item[-1]]
                     else:
                         episode.hist_data[key] = [item]
             if "custom_metrics" in info:
```

### Comparing `pyrlprob-2.0.2/pyrlprob/utils/plots.py` & `pyrlprob-2.0.3/pyrlprob/utils/plots.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/pyrlprob.egg-info/PKG-INFO` & `pyrlprob-2.0.3/pyrlprob.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrlprob
-Version: 2.0.2
+Version: 2.0.3
 Summary: Train Gym-derived environments in Python/C++ through Ray RLlib
 Home-page: https://github.com/LorenzoFederici/pyrlprob
 Author: Lorenzo Federici
 Author-email: federicilorenzo94@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyrlprob-2.0.2/pyrlprob.egg-info/SOURCES.txt` & `pyrlprob-2.0.3/pyrlprob.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.2/setup.py` & `pyrlprob-2.0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(name='pyrlprob',
-    version='2.0.2',
+    version='2.0.3',
     author='Lorenzo Federici',
     author_email = 'federicilorenzo94@gmail.com',
     description = 'Train Gym-derived environments in Python/C++ through Ray RLlib',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/LorenzoFederici/pyrlprob',
     classifiers = [
```

