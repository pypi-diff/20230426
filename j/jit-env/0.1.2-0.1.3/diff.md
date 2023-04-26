# Comparing `tmp/jit_env-0.1.2.tar.gz` & `tmp/jit_env-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jit_env-0.1.2.tar", last modified: Sun Apr 23 09:51:22 2023, max compression
+gzip compressed data, was "dist/jit_env-0.1.3.tar", last modified: Tue Apr 25 14:22:23 2023, max compression
```

## Comparing `jit_env-0.1.2.tar` & `jit_env-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-23 09:51:22.969188 jit_env-0.1.2/
--rwxrwxrwx   0 joery     (1000) joery     (1000)     1062 2023-04-07 11:59:34.000000 jit_env-0.1.2/LICENSE
--rwxrwxrwx   0 joery     (1000) joery     (1000)       29 2023-04-10 08:18:00.000000 jit_env-0.1.2/MANIFEST.in
--rwxrwxrwx   0 joery     (1000) joery     (1000)     5523 2023-04-23 09:51:22.962867 jit_env-0.1.2/PKG-INFO
--rwxrwxrwx   0 joery     (1000) joery     (1000)     4739 2023-04-23 09:50:06.000000 jit_env-0.1.2/README.md
-drwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-23 09:51:22.676900 jit_env-0.1.2/jit_env/
--rwxrwxrwx   0 joery     (1000) joery     (1000)     1057 2023-04-07 09:34:23.000000 jit_env-0.1.2/jit_env/__init__.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)     4215 2023-04-11 07:18:45.000000 jit_env-0.1.2/jit_env/_compat_test.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)    14702 2023-04-15 05:34:34.000000 jit_env-0.1.2/jit_env/_core.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)     9289 2023-04-11 07:13:02.000000 jit_env-0.1.2/jit_env/_core_test.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)    16484 2023-04-10 12:51:38.000000 jit_env-0.1.2/jit_env/_specs_test.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)    13301 2023-04-15 05:34:34.000000 jit_env-0.1.2/jit_env/_wrappers_test.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)     4532 2023-04-11 07:17:00.000000 jit_env-0.1.2/jit_env/compat.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-13 07:54:10.000000 jit_env-0.1.2/jit_env/py.typed
--rwxrwxrwx   0 joery     (1000) joery     (1000)    23230 2023-04-10 13:11:26.000000 jit_env-0.1.2/jit_env/specs.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)      304 2023-04-23 09:50:06.000000 jit_env-0.1.2/jit_env/version.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)    14216 2023-04-13 07:54:10.000000 jit_env-0.1.2/jit_env/wrappers.py
-drwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-23 09:51:22.902842 jit_env-0.1.2/jit_env.egg-info/
--rwxrwxrwx   0 joery     (1000) joery     (1000)     5523 2023-04-23 09:51:20.000000 jit_env-0.1.2/jit_env.egg-info/PKG-INFO
--rwxrwxrwx   0 joery     (1000) joery     (1000)      453 2023-04-23 09:51:20.000000 jit_env-0.1.2/jit_env.egg-info/SOURCES.txt
--rwxrwxrwx   0 joery     (1000) joery     (1000)        1 2023-04-23 09:51:20.000000 jit_env-0.1.2/jit_env.egg-info/dependency_links.txt
--rwxrwxrwx   0 joery     (1000) joery     (1000)      157 2023-04-23 09:51:20.000000 jit_env-0.1.2/jit_env.egg-info/requires.txt
--rwxrwxrwx   0 joery     (1000) joery     (1000)        8 2023-04-23 09:51:20.000000 jit_env-0.1.2/jit_env.egg-info/top_level.txt
--rwxrwxrwx   0 joery     (1000) joery     (1000)       44 2023-04-08 05:46:44.000000 jit_env-0.1.2/requirements.txt
--rwxrwxrwx   0 joery     (1000) joery     (1000)      115 2023-04-10 08:18:00.000000 jit_env-0.1.2/requirements_dev.txt
--rwxrwxrwx   0 joery     (1000) joery     (1000)       38 2023-04-23 09:51:22.972656 jit_env-0.1.2/setup.cfg
--rwxrwxrwx   0 joery     (1000) joery     (1000)     1835 2023-04-13 07:54:10.000000 jit_env-0.1.2/setup.py
+drwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-25 14:22:22.708681 jit_env-0.1.3/
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     1062 2023-04-07 11:59:34.000000 jit_env-0.1.3/LICENSE
+-rwxrwxrwx   0 joery     (1000) joery     (1000)       29 2023-04-10 08:18:00.000000 jit_env-0.1.3/MANIFEST.in
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     5523 2023-04-25 14:22:22.701198 jit_env-0.1.3/PKG-INFO
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     4739 2023-04-25 14:21:51.000000 jit_env-0.1.3/README.md
+drwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-25 14:22:22.591823 jit_env-0.1.3/jit_env/
+-rwxrwxrwx   0 joery     (1000) joery     (1000)      772 2023-04-25 14:18:00.000000 jit_env-0.1.3/jit_env/__init__.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     4215 2023-04-11 07:18:45.000000 jit_env-0.1.3/jit_env/_compat_test.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)    14702 2023-04-15 05:34:34.000000 jit_env-0.1.3/jit_env/_core.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     9289 2023-04-11 07:13:02.000000 jit_env-0.1.3/jit_env/_core_test.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)    16484 2023-04-10 12:51:38.000000 jit_env-0.1.3/jit_env/_specs_test.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)    15327 2023-04-25 14:18:00.000000 jit_env-0.1.3/jit_env/_wrappers_test.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     4532 2023-04-11 07:17:00.000000 jit_env-0.1.3/jit_env/compat.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-13 07:54:10.000000 jit_env-0.1.3/jit_env/py.typed
+-rwxrwxrwx   0 joery     (1000) joery     (1000)    23230 2023-04-10 13:11:26.000000 jit_env-0.1.3/jit_env/specs.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)      304 2023-04-25 14:21:51.000000 jit_env-0.1.3/jit_env/version.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)    14574 2023-04-25 14:18:00.000000 jit_env-0.1.3/jit_env/wrappers.py
+drwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-25 14:22:22.685574 jit_env-0.1.3/jit_env.egg-info/
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     5523 2023-04-25 14:22:21.000000 jit_env-0.1.3/jit_env.egg-info/PKG-INFO
+-rwxrwxrwx   0 joery     (1000) joery     (1000)      453 2023-04-25 14:22:21.000000 jit_env-0.1.3/jit_env.egg-info/SOURCES.txt
+-rwxrwxrwx   0 joery     (1000) joery     (1000)        1 2023-04-25 14:22:21.000000 jit_env-0.1.3/jit_env.egg-info/dependency_links.txt
+-rwxrwxrwx   0 joery     (1000) joery     (1000)      157 2023-04-25 14:22:21.000000 jit_env-0.1.3/jit_env.egg-info/requires.txt
+-rwxrwxrwx   0 joery     (1000) joery     (1000)        8 2023-04-25 14:22:21.000000 jit_env-0.1.3/jit_env.egg-info/top_level.txt
+-rwxrwxrwx   0 joery     (1000) joery     (1000)       44 2023-04-08 05:46:44.000000 jit_env-0.1.3/requirements.txt
+-rwxrwxrwx   0 joery     (1000) joery     (1000)      115 2023-04-10 08:18:00.000000 jit_env-0.1.3/requirements_dev.txt
+-rwxrwxrwx   0 joery     (1000) joery     (1000)       38 2023-04-25 14:22:22.709193 jit_env-0.1.3/setup.cfg
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     1835 2023-04-13 07:54:10.000000 jit_env-0.1.3/setup.py
```

### Comparing `jit_env-0.1.2/LICENSE` & `jit_env-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jit_env-0.1.2/PKG-INFO` & `jit_env-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jit_env
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Jax interface for Reinforcement Learning environments.
 Home-page: https://github.com/joeryjoery/jit_env
 Author: Joery A. de Vries
 Author-email: J.A.deVries@tudelft.nl
 License: MIT
 Keywords: reinforcement-learning python machine learning jax
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 ![Run Tox Tests](https://github.com/joeryjoery/jit_env/actions/workflows/tests.yml/badge.svg)
 ![Python Version](https://img.shields.io/badge/Python-3.9%20%7C%203.10%20%7C%203.11-blue)
-![Package Version](https://img.shields.io/badge/jit__env-0.1.2-blue)
+![Package Version](https://img.shields.io/badge/jit__env-0.1.3-blue)
 # `jit_env`: A Jax Compatible RL Environment API
 `jit_env` is a library that aims to adhere closely to the `dm_env` interface
 while allowing for `jax` transformations inside Environment implementations
 and defining clear type annotations.
 
 Like `dm_env` our API consists of the main components:
```

### Comparing `jit_env-0.1.2/README.md` & `jit_env-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ![Run Tox Tests](https://github.com/joeryjoery/jit_env/actions/workflows/tests.yml/badge.svg)
 ![Python Version](https://img.shields.io/badge/Python-3.9%20%7C%203.10%20%7C%203.11-blue)
-![Package Version](https://img.shields.io/badge/jit__env-0.1.2-blue)
+![Package Version](https://img.shields.io/badge/jit__env-0.1.3-blue)
 # `jit_env`: A Jax Compatible RL Environment API
 `jit_env` is a library that aims to adhere closely to the `dm_env` interface
 while allowing for `jax` transformations inside Environment implementations
 and defining clear type annotations.
 
 Like `dm_env` our API consists of the main components:
```

### Comparing `jit_env-0.1.2/jit_env/__init__.py` & `jit_env-0.1.3/jit_env/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 """Define main module/ API hierarchy.
 
 Private attributes (starting with '_') should not be accessed lest thou would
 risketh the consequences of internal API changes.
 """
-from typing import Union as _Alias_Union
-from typing_extensions import TypeAlias as _TypeAlias
-
 from jit_env.version import __version__, __version_info__
 
 from jit_env import _core
+from jit_env._core import (
+    Action as Action,
+    State as State,
+    Observation as Observation
+)
 
 from jit_env import specs
 from jit_env import wrappers
 from jit_env import compat
 
 Environment = _core.Environment
 Wrapper = _core.Wrapper
 StepType = _core.StepType
 TimeStep = _core.TimeStep
 
-# Type Annotations/ Alias defined as a type Union to distinguish Variables
-# from an Alias: https://github.com/python/mypy/issues/3494
-Action: _TypeAlias = _Alias_Union[_core.Action]
-State: _TypeAlias = _Alias_Union[_core.State]
-Observation: _TypeAlias = _Alias_Union[_core.Observation]
-
 # Helper functions for creating TimeStep namedtuples with default settings.
 restart = _core.restart
 termination = _core.termination
 transition = _core.transition
 truncation = _core.truncation
```

### Comparing `jit_env-0.1.2/jit_env/_compat_test.py` & `jit_env-0.1.3/jit_env/_compat_test.py`

 * *Files identical despite different names*

### Comparing `jit_env-0.1.2/jit_env/_core.py` & `jit_env-0.1.3/jit_env/_core.py`

 * *Files identical despite different names*

### Comparing `jit_env-0.1.2/jit_env/_core_test.py` & `jit_env-0.1.3/jit_env/_core_test.py`

 * *Files identical despite different names*

### Comparing `jit_env-0.1.2/jit_env/_specs_test.py` & `jit_env-0.1.3/jit_env/_specs_test.py`

 * *Files identical despite different names*

### Comparing `jit_env-0.1.2/jit_env/_wrappers_test.py` & `jit_env-0.1.3/jit_env/_wrappers_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-import chex
+from dataclasses import replace
+
 import pytest
 
+import chex
+
 import jax
 from jax import numpy as jnp
 
 import jit_env
 from jit_env import wrappers, specs
 
 
@@ -59,22 +62,25 @@
     assert dummy_env.unwrapped is dummy_env
 
     assert wrapped.env is dummy_env
     assert doubly_wrapped.env is wrapped
 
 
 @pytest.mark.usefixtures('dummy_env')
-def test_jit(dummy_env: jit_env.Environment):
+def test_jit(
+        dummy_env: jit_env.Environment[
+            jit_env.State, jax.Array, jit_env.Observation
+        ]
+):
     jitted = wrappers.Jit(dummy_env)
 
-    # Reset logic
-
     # For type checker
     jit_state: jit_env.State
 
+    # Reset logic
     state, step = dummy_env.reset(jax.random.PRNGKey(0))
     jit_state, jit_step = jitted.reset(jax.random.PRNGKey(0))
 
     chex.assert_trees_all_equal(state, jit_state, ignore_nones=True)
     chex.assert_trees_all_equal(step, jit_step, ignore_nones=True)
     chex.assert_trees_all_equal_shapes_and_dtypes(
         state, jit_state, ignore_nones=True
@@ -94,14 +100,57 @@
     )
     chex.assert_trees_all_equal_shapes_and_dtypes(
         (step,), (jit_step,), ignore_nones=True
     )
 
 
 @pytest.mark.usefixtures('dummy_env')
+def test_stopgrad(dummy_env: jit_env.Environment):
+    class ScaleRewardWrapper(jit_env.Wrapper):
+
+        def step(
+                self,
+                s: jit_env.State,
+                a: jit_env.Action
+        ) -> tuple[jit_env.State, jit_env.TimeStep]:
+            s, t = super().step(s, a)
+            # y = constant * x + x
+            # dy/dx = constant + 1
+            t = replace(t, reward=(t.reward * a + a))
+            return s, t
+
+    scale_reward = ScaleRewardWrapper(dummy_env)
+    stopped = wrappers.StopGradient(scale_reward)
+
+    jacfun = jax.jacrev(
+        lambda *a: scale_reward.step(*a)[1].reward,
+        argnums=1
+    )
+    stop_jacfun = jax.jacrev(
+        lambda *a: stopped.step(*a)[1].reward,
+        argnums=1
+    )
+
+    action = jnp.ones_like(dummy_env.action_spec().generate_value())
+    action = action * 10.0
+
+    state, _ = dummy_env.reset(jax.random.PRNGKey(0))
+    _, reference_step = dummy_env.step(state, action)
+
+    jac = jacfun(state, action)
+    jac_zero = stop_jacfun(state, action)
+
+    # Computation:
+    # y = constant * x + x
+    # dy/dx = constant + 1
+    assert (jac == (reference_step.reward + 1.0)).all()
+    assert (jac_zero == 0.0).all()
+
+
+@pytest.mark.usefixtures('dummy_env')
 def test_autoreset(dummy_env: jit_env.Environment):
     env = wrappers.AutoReset(dummy_env)
 
     state, step = env.reset(jax.random.PRNGKey(0))
     ref_state, ref_step = dummy_env.reset(jax.random.PRNGKey(0))
 
     assert step.first()
@@ -140,23 +189,28 @@
     assert jnp.all(step.observation == 0.0)
     assert jnp.all(step.observation != ref_step.observation)
 
 
 class TestVmap:
 
     @pytest.mark.usefixtures('dummy_env')
-    def test_env(self, dummy_env: jit_env.Environment, batch_size: int = 5):
+    def test_env(
+            self,
+            dummy_env: jit_env.Environment[
+                jit_env.State, jax.Array, jit_env.Observation
+            ],
+            batch_size: int = 5
+    ):
         key = jax.random.PRNGKey(0)
         batched = wrappers.Vmap(dummy_env)
 
-        # Reset logic
-
         # For type checker
         states: jit_env.State
 
+        # Reset logic
         state, step = dummy_env.reset(key)
         states, steps = batched.reset(jax.random.split(key, num=batch_size))
 
         chex.assert_tree_shape_prefix(
             (states, steps), (batch_size,), ignore_nones=True
         )
 
@@ -175,15 +229,21 @@
 
         sliced = jax.tree_map(lambda x: x.at[0].get(), (states, steps))
         chex.assert_trees_all_equal_shapes_and_dtypes(
             sliced, (state, step), ignore_nones=True
         )
 
     @pytest.mark.usefixtures('dummy_env')
-    def test_render(self, dummy_env: jit_env.Environment, batch_size: int = 5):
+    def test_render(
+            self,
+            dummy_env: jit_env.Environment[
+                jit_env.State, jit_env.Action, jit_env.Observation
+            ],
+            batch_size: int = 5
+    ):
         key = jax.random.PRNGKey(0)
         batched = wrappers.Vmap(dummy_env)
 
         # For type checker
         states: jit_env.State
 
         state, _ = dummy_env.reset(key)
@@ -196,15 +256,20 @@
             single_render, batch_render, ignore_nones=True
         )
         chex.assert_trees_all_equal_shapes_and_dtypes(
             single_render, batch_render, ignore_nones=True
         )
 
     @pytest.mark.usefixtures('dummy_env')
-    def test_wrongly_wrapped_autoreset(self, dummy_env: jit_env.Environment):
+    def test_wrongly_wrapped_autoreset(
+            self,
+            dummy_env: jit_env.Environment[
+                jit_env.State, jit_env.Action, jit_env.Observation
+            ]
+    ):
         vmap_first = wrappers.AutoReset(wrappers.Vmap(dummy_env))
         vmap_last = wrappers.Vmap(wrappers.AutoReset(dummy_env))
 
         keys = jax.random.split(jax.random.PRNGKey(0), num=5)
         first, _ = vmap_first.reset(keys)
         last: jit_env.State = vmap_last.reset(keys)[0]
 
@@ -212,15 +277,21 @@
             # lax.cond in AutoReset will receive incompatible Array of bools
             vmap_first.step(first, jnp.zeros((5,)))
 
         # Array of bools can be handled per element by vmapping last.
         vmap_last.step(last, jnp.zeros((5,)))
 
     @pytest.mark.usefixtures('dummy_env')
-    def test_autoreset(self, dummy_env: jit_env.Environment, num: int = 2):
+    def test_autoreset(
+            self,
+            dummy_env: jit_env.Environment[
+                jit_env.State, jit_env.Action, jit_env.Observation
+            ],
+            num: int = 2
+    ):
         # Doubly or single-wrapping should both work.
         # Singly is preferred as it is faster, this is not explicitly tested.
         doubly_wrapped = wrappers.Vmap(
             wrappers.AutoReset(dummy_env), in_axes=(0, None)
         )
         singly_wrapped = wrappers.VmapAutoReset(dummy_env, in_axes=(0, None))
         keys = jax.random.split(jax.random.PRNGKey(0), num=num)
@@ -313,15 +384,21 @@
         states, steps = tiled_env.reset(jax.random.PRNGKey(0))  # type: ignore
 
         chex.assert_tree_shape_prefix(
             (states, steps), (num,), ignore_nones=True
         )
 
     @pytest.mark.usefixtures('dummy_env')
-    def test_autoreset(self, dummy_env: jit_env.Environment, num: int = 2):
+    def test_autoreset(
+            self,
+            dummy_env: jit_env.Environment[
+                jit_env.State, jit_env.Action, jit_env.Observation
+            ],
+            num: int = 2
+    ):
         # Tile and Vmap are equivalent aside from the `reset` call.
         vmapped = wrappers.VmapAutoReset(dummy_env, in_axes=(0, None))
         tiled = wrappers.TileAutoReset(dummy_env, num=num, in_axes=(0, None))
 
         keys = jax.random.split(jax.random.PRNGKey(0), num=num)
 
         # For type checker
```

### Comparing `jit_env-0.1.2/jit_env/compat.py` & `jit_env-0.1.3/jit_env/compat.py`

 * *Files identical despite different names*

### Comparing `jit_env-0.1.2/jit_env/specs.py` & `jit_env-0.1.3/jit_env/specs.py`

 * *Files identical despite different names*

### Comparing `jit_env-0.1.2/jit_env/wrappers.py` & `jit_env-0.1.3/jit_env/wrappers.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,14 +112,27 @@
 
     def render(self, state: _core.State) -> _typing.Any:
         """Generate a pixel-observation based on the 0'th state slice. """
         state_0 = _jax.tree_map(lambda x: x.at[0].get(), state)
         return super().render(state_0)
 
 
+class StopGradient(_core.Wrapper):
+    """Wrapper to cancel out all Env-dependent gradients."""
+
+    def step(
+            self,
+            state: _core.State,
+            action: _core.Action
+    ) -> tuple[_core.State, _core.TimeStep]:
+        return _jax.tree_map(
+            _jax.lax.stop_gradient, super().step(state, action)
+        )
+
+
 class BatchSpecMixin:
     """Provide a fixed-size batched environment-spec as a MixIn."""
     env: _core.Environment
 
     def __init__(
             self,
             env: _core.Environment,
```

### Comparing `jit_env-0.1.2/jit_env.egg-info/PKG-INFO` & `jit_env-0.1.3/jit_env.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jit-env
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Jax interface for Reinforcement Learning environments.
 Home-page: https://github.com/joeryjoery/jit_env
 Author: Joery A. de Vries
 Author-email: J.A.deVries@tudelft.nl
 License: MIT
 Keywords: reinforcement-learning python machine learning jax
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 ![Run Tox Tests](https://github.com/joeryjoery/jit_env/actions/workflows/tests.yml/badge.svg)
 ![Python Version](https://img.shields.io/badge/Python-3.9%20%7C%203.10%20%7C%203.11-blue)
-![Package Version](https://img.shields.io/badge/jit__env-0.1.2-blue)
+![Package Version](https://img.shields.io/badge/jit__env-0.1.3-blue)
 # `jit_env`: A Jax Compatible RL Environment API
 `jit_env` is a library that aims to adhere closely to the `dm_env` interface
 while allowing for `jax` transformations inside Environment implementations
 and defining clear type annotations.
 
 Like `dm_env` our API consists of the main components:
```

### Comparing `jit_env-0.1.2/setup.py` & `jit_env-0.1.3/setup.py`

 * *Files identical despite different names*

