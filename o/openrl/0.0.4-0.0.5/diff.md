# Comparing `tmp/openrl-0.0.4.tar.gz` & `tmp/openrl-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openrl-0.0.4.tar", last modified: Tue Apr 18 10:09:36 2023, max compression
+gzip compressed data, was "openrl-0.0.5.tar", last modified: Wed Apr 26 15:36:17 2023, max compression
```

## Comparing `openrl-0.0.4.tar` & `openrl-0.0.5.tar`

### file list

```diff
@@ -1,132 +1,172 @@
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.219174 openrl-0.0.4/
--rw-r--r--   0 4paradigm   (501) staff       (20)    11357 2023-04-12 14:31:37.000000 openrl-0.0.4/LICENSE
--rw-r--r--   0 4paradigm   (501) staff       (20)    11342 2023-03-23 09:43:52.000000 openrl-0.0.4/LICENSE.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)     4729 2023-04-18 10:09:36.219020 openrl-0.0.4/PKG-INFO
--rw-r--r--   0 4paradigm   (501) staff       (20)     3684 2023-04-13 06:07:12.000000 openrl-0.0.4/README.md
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.194804 openrl-0.0.4/openrl/
--rw-r--r--   0 4paradigm   (501) staff       (20)      194 2023-04-18 10:09:23.000000 openrl-0.0.4/openrl/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.196428 openrl-0.0.4/openrl/algorithms/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/algorithms/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2915 2023-04-18 09:39:06.000000 openrl-0.0.4/openrl/algorithms/base_algorithm.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    15908 2023-04-18 09:39:19.000000 openrl-0.0.4/openrl/algorithms/ppo.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.197187 openrl-0.0.4/openrl/buffers/
--rw-r--r--   0 4paradigm   (501) staff       (20)      726 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/buffers/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3100 2023-04-18 09:40:26.000000 openrl-0.0.4/openrl/buffers/normal_buffer.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    54666 2023-04-18 09:41:36.000000 openrl-0.0.4/openrl/buffers/replay_data.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.198095 openrl-0.0.4/openrl/buffers/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/buffers/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1686 2023-04-18 09:39:57.000000 openrl-0.0.4/openrl/buffers/utils/obs_data.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3153 2023-04-18 09:39:57.000000 openrl-0.0.4/openrl/buffers/utils/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.198787 openrl-0.0.4/openrl/cli/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/cli/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2053 2023-04-18 08:43:57.000000 openrl-0.0.4/openrl/cli/cli.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1709 2023-04-18 08:57:15.000000 openrl-0.0.4/openrl/cli/train.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.199236 openrl-0.0.4/openrl/configs/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/configs/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    29480 2023-04-18 09:55:21.000000 openrl-0.0.4/openrl/configs/config.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.200300 openrl-0.0.4/openrl/drivers/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/drivers/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      236 2023-03-28 06:23:04.000000 openrl-0.0.4/openrl/drivers/base_driver.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     9767 2023-04-18 09:55:53.000000 openrl-0.0.4/openrl/drivers/onpolicy_driver.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      840 2023-04-12 14:35:57.000000 openrl-0.0.4/openrl/drivers/rl_driver.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.200537 openrl-0.0.4/openrl/envs/
--rw-r--r--   0 4paradigm   (501) staff       (20)      125 2023-04-07 13:42:53.000000 openrl-0.0.4/openrl/envs/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.201028 openrl-0.0.4/openrl/envs/common/
--rw-r--r--   0 4paradigm   (501) staff       (20)      716 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/envs/common/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     4196 2023-04-14 07:57:12.000000 openrl-0.0.4/openrl/envs/common/registration.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.201280 openrl-0.0.4/openrl/envs/gymnasium/
--rw-r--r--   0 4paradigm   (501) staff       (20)     1435 2023-04-12 14:35:57.000000 openrl-0.0.4/openrl/envs/gymnasium/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.203057 openrl-0.0.4/openrl/envs/mpe/
--rw-r--r--   0 4paradigm   (501) staff       (20)      673 2023-04-14 08:15:22.000000 openrl-0.0.4/openrl/envs/mpe/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    14285 2023-04-18 09:57:30.000000 openrl-0.0.4/openrl/envs/mpe/core.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      614 2023-04-07 13:47:06.000000 openrl-0.0.4/openrl/envs/mpe/mpe_env.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2489 2023-04-10 07:48:10.000000 openrl-0.0.4/openrl/envs/mpe/multi_discrete.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    19199 2023-04-18 09:57:30.000000 openrl-0.0.4/openrl/envs/mpe/multiagent_env.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    11584 2023-04-10 13:20:30.000000 openrl-0.0.4/openrl/envs/mpe/rendering.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      361 2022-07-24 12:50:33.000000 openrl-0.0.4/openrl/envs/mpe/scenario.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.203501 openrl-0.0.4/openrl/envs/mpe/scenarios/
--rw-r--r--   0 4paradigm   (501) staff       (20)      147 2022-07-24 12:50:33.000000 openrl-0.0.4/openrl/envs/mpe/scenarios/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     4404 2023-04-12 14:35:57.000000 openrl-0.0.4/openrl/envs/mpe/scenarios/simple_spread.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.204702 openrl-0.0.4/openrl/envs/vec_env/
--rw-r--r--   0 4paradigm   (501) staff       (20)      254 2023-04-12 14:35:57.000000 openrl-0.0.4/openrl/envs/vec_env/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    30677 2023-04-14 07:55:00.000000 openrl-0.0.4/openrl/envs/vec_env/async_venv.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     8063 2023-04-14 07:26:31.000000 openrl-0.0.4/openrl/envs/vec_env/base_venv.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    11100 2023-04-14 07:27:02.000000 openrl-0.0.4/openrl/envs/vec_env/sync_venv.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.205772 openrl-0.0.4/openrl/envs/vec_env/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/envs/vec_env/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     6519 2023-04-11 08:43:14.000000 openrl-0.0.4/openrl/envs/vec_env/utils/numpy_utils.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7903 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/envs/vec_env/utils/share_memory.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1909 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/envs/vec_env/utils/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.206548 openrl-0.0.4/openrl/envs/vec_env/wrappers/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/envs/vec_env/wrappers/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     9291 2023-04-14 07:16:41.000000 openrl-0.0.4/openrl/envs/vec_env/wrappers/base_wrapper.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2653 2023-04-14 08:16:46.000000 openrl-0.0.4/openrl/envs/vec_env/wrappers/vec_monitor.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.207870 openrl-0.0.4/openrl/envs/wrappers/
--rw-r--r--   0 4paradigm   (501) staff       (20)      372 2023-04-14 07:11:32.000000 openrl-0.0.4/openrl/envs/wrappers/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1419 2023-04-13 02:36:05.000000 openrl-0.0.4/openrl/envs/wrappers/base_wrapper.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2480 2023-04-17 07:08:30.000000 openrl-0.0.4/openrl/envs/wrappers/extra_wrappers.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2533 2023-04-13 02:35:11.000000 openrl-0.0.4/openrl/envs/wrappers/multiagent_wrapper.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1188 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/envs/wrappers/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.208940 openrl-0.0.4/openrl/modules/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/modules/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1540 2023-04-14 07:55:18.000000 openrl-0.0.4/openrl/modules/base_module.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.209734 openrl-0.0.4/openrl/modules/common/
--rw-r--r--   0 4paradigm   (501) staff       (20)       55 2023-03-27 09:25:06.000000 openrl-0.0.4/openrl/modules/common/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      738 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/modules/common/base_net.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3300 2023-04-14 07:46:31.000000 openrl-0.0.4/openrl/modules/common/ppo_net.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1233 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/modules/model_config.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.211431 openrl-0.0.4/openrl/modules/networks/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/modules/networks/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1227 2023-04-14 07:55:00.000000 openrl-0.0.4/openrl/modules/networks/base_policy_network.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1190 2023-04-14 07:55:00.000000 openrl-0.0.4/openrl/modules/networks/base_value_network.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     8075 2023-04-14 07:55:55.000000 openrl-0.0.4/openrl/modules/networks/policy_network.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     6467 2023-04-14 07:55:55.000000 openrl-0.0.4/openrl/modules/networks/policy_value_network.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.214342 openrl-0.0.4/openrl/modules/networks/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)        0 2022-09-12 08:05:59.000000 openrl-0.0.4/openrl/modules/networks/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7493 2023-04-06 11:59:56.000000 openrl-0.0.4/openrl/modules/networks/utils/act.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     9383 2023-04-14 07:55:18.000000 openrl-0.0.4/openrl/modules/networks/utils/attention.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2378 2023-04-14 07:55:18.000000 openrl-0.0.4/openrl/modules/networks/utils/cnn.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      803 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/modules/networks/utils/distributed_utils.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3601 2022-09-16 11:16:47.000000 openrl-0.0.4/openrl/modules/networks/utils/distributions.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    10433 2023-04-14 07:55:18.000000 openrl-0.0.4/openrl/modules/networks/utils/mix.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     5956 2023-04-14 07:55:55.000000 openrl-0.0.4/openrl/modules/networks/utils/mlp.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3796 2022-07-24 12:50:33.000000 openrl-0.0.4/openrl/modules/networks/utils/popart.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3533 2022-07-24 12:50:33.000000 openrl-0.0.4/openrl/modules/networks/utils/rnn.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3332 2023-03-28 07:32:22.000000 openrl-0.0.4/openrl/modules/networks/utils/transformer_act.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      319 2023-03-28 07:32:36.000000 openrl-0.0.4/openrl/modules/networks/utils/util.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     4602 2023-04-14 07:55:55.000000 openrl-0.0.4/openrl/modules/networks/value_network.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     5674 2023-04-14 07:51:42.000000 openrl-0.0.4/openrl/modules/ppo_module.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     5172 2023-04-14 07:55:34.000000 openrl-0.0.4/openrl/modules/rl_module.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.215258 openrl-0.0.4/openrl/modules/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/modules/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      616 2023-03-28 07:42:17.000000 openrl-0.0.4/openrl/modules/utils/util.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3381 2022-09-27 11:21:49.000000 openrl-0.0.4/openrl/modules/utils/valuenorm.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.215479 openrl-0.0.4/openrl/runners/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/runners/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.216196 openrl-0.0.4/openrl/runners/common/
--rw-r--r--   0 4paradigm   (501) staff       (20)       83 2023-04-12 14:35:57.000000 openrl-0.0.4/openrl/runners/common/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1269 2023-04-14 08:27:24.000000 openrl-0.0.4/openrl/runners/common/base_agent.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     6139 2023-04-14 09:38:42.000000 openrl-0.0.4/openrl/runners/common/ppo_agent.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.216432 openrl-0.0.4/openrl/supports/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/supports/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.217122 openrl-0.0.4/openrl/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     6608 2023-04-14 10:20:15.000000 openrl-0.0.4/openrl/utils/logger.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      588 2023-04-14 09:35:30.000000 openrl-0.0.4/openrl/utils/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.195626 openrl-0.0.4/openrl.egg-info/
--rw-r--r--   0 4paradigm   (501) staff       (20)     4729 2023-04-18 10:09:36.000000 openrl-0.0.4/openrl.egg-info/PKG-INFO
--rw-r--r--   0 4paradigm   (501) staff       (20)     3216 2023-04-18 10:09:36.000000 openrl-0.0.4/openrl.egg-info/SOURCES.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)        1 2023-04-18 10:09:36.000000 openrl-0.0.4/openrl.egg-info/dependency_links.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       46 2023-04-18 10:09:36.000000 openrl-0.0.4/openrl.egg-info/entry_points.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)      151 2023-04-18 10:09:36.000000 openrl-0.0.4/openrl.egg-info/requires.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       13 2023-04-18 10:09:36.000000 openrl-0.0.4/openrl.egg-info/top_level.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       38 2023-04-18 10:09:36.219223 openrl-0.0.4/setup.cfg
--rw-r--r--   0 4paradigm   (501) staff       (20)     2740 2023-04-14 07:27:41.000000 openrl-0.0.4/setup.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.217347 openrl-0.0.4/tests/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.4/tests/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.217866 openrl-0.0.4/tests/project/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.4/tests/project/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      971 2023-04-12 14:36:21.000000 openrl-0.0.4/tests/project/test_version.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.218330 openrl-0.0.4/tests/test_buffer/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.4/tests/test_buffer/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1803 2023-04-12 14:35:57.000000 openrl-0.0.4/tests/test_buffer/test_buffer.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.149727 openrl-0.0.5/
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11357 2023-04-12 14:31:37.000000 openrl-0.0.5/LICENSE
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11342 2023-03-23 09:43:52.000000 openrl-0.0.5/LICENSE.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11299 2023-04-26 15:36:17.149418 openrl-0.0.5/PKG-INFO
+-rw-r--r--   0 4paradigm   (501) staff       (20)    10214 2023-04-26 08:59:55.000000 openrl-0.0.5/README.md
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.115630 openrl-0.0.5/openrl/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      194 2023-04-26 13:13:37.000000 openrl-0.0.5/openrl/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.117819 openrl-0.0.5/openrl/algorithms/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.5/openrl/algorithms/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2916 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/algorithms/base_algorithm.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    16410 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/algorithms/ppo.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.118964 openrl-0.0.5/openrl/buffers/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      726 2023-04-12 14:34:56.000000 openrl-0.0.5/openrl/buffers/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3100 2023-04-18 09:40:26.000000 openrl-0.0.5/openrl/buffers/normal_buffer.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    54804 2023-04-26 13:14:52.000000 openrl-0.0.5/openrl/buffers/replay_data.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.120182 openrl-0.0.5/openrl/buffers/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.5/openrl/buffers/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1938 2023-04-26 13:14:42.000000 openrl-0.0.5/openrl/buffers/utils/obs_data.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3153 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/buffers/utils/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.120705 openrl-0.0.5/openrl/cli/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.5/openrl/cli/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2551 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/cli/cli.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1579 2023-04-26 12:06:55.000000 openrl-0.0.5/openrl/cli/train.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.121193 openrl-0.0.5/openrl/configs/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.5/openrl/configs/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    31231 2023-04-26 12:06:55.000000 openrl-0.0.5/openrl/configs/config.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.122275 openrl-0.0.5/openrl/drivers/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.5/openrl/drivers/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      238 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/drivers/base_driver.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     9926 2023-04-26 12:08:00.000000 openrl-0.0.5/openrl/drivers/onpolicy_driver.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      841 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/drivers/rl_driver.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.122480 openrl-0.0.5/openrl/envs/
+-rw-r--r--   0 4paradigm   (501) staff       (20)       79 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.123191 openrl-0.0.5/openrl/envs/common/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      739 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/common/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1621 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/common/build_envs.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3299 2023-04-26 13:14:52.000000 openrl-0.0.5/openrl/envs/common/registration.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.123446 openrl-0.0.5/openrl/envs/gymnasium/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1425 2023-04-26 13:14:52.000000 openrl-0.0.5/openrl/envs/gymnasium/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.126217 openrl-0.0.5/openrl/envs/mpe/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      628 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/mpe/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    14285 2023-04-18 09:57:30.000000 openrl-0.0.5/openrl/envs/mpe/core.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      615 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/mpe/mpe_env.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2488 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/mpe/multi_discrete.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    19199 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/mpe/multiagent_env.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11650 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/mpe/rendering.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      343 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/mpe/scenario.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.126558 openrl-0.0.5/openrl/envs/mpe/scenarios/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      145 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/mpe/scenarios/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4405 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/mpe/scenarios/simple_spread.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.127627 openrl-0.0.5/openrl/envs/nlp/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      876 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/nlp/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7259 2023-04-26 12:38:02.000000 openrl-0.0.5/openrl/envs/nlp/daily_dialog_env.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      347 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/nlp/nlp_env.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11061 2023-04-26 13:14:52.000000 openrl-0.0.5/openrl/envs/nlp/nlp_rewards.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.129228 openrl-0.0.5/openrl/envs/nlp/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)        0 2023-04-26 13:39:44.000000 openrl-0.0.5/openrl/envs/nlp/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2765 2023-04-26 13:14:42.000000 openrl-0.0.5/openrl/envs/nlp/utils/custom_text_generation_pools.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4515 2023-04-26 12:50:40.000000 openrl-0.0.5/openrl/envs/nlp/utils/distribution.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1823 2023-04-26 13:14:42.000000 openrl-0.0.5/openrl/envs/nlp/utils/evaluation_utils.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.129875 openrl-0.0.5/openrl/envs/nlp/utils/metrics/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-26 08:59:55.000000 openrl-0.0.5/openrl/envs/nlp/utils/metrics/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7088 2023-04-26 13:14:42.000000 openrl-0.0.5/openrl/envs/nlp/utils/metrics/meteor.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7201 2023-04-26 12:51:48.000000 openrl-0.0.5/openrl/envs/nlp/utils/observation.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1363 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/nlp/utils/sampler.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1233 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/nlp/utils/text_generation_pool.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.131039 openrl-0.0.5/openrl/envs/vec_env/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      326 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/vec_env/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    30978 2023-04-26 13:14:52.000000 openrl-0.0.5/openrl/envs/vec_env/async_venv.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7845 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/vec_env/base_venv.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11100 2023-04-26 13:14:52.000000 openrl-0.0.5/openrl/envs/vec_env/sync_venv.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.132089 openrl-0.0.5/openrl/envs/vec_env/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.5/openrl/envs/vec_env/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     6518 2023-04-26 13:14:52.000000 openrl-0.0.5/openrl/envs/vec_env/utils/numpy_utils.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7902 2023-04-26 13:14:52.000000 openrl-0.0.5/openrl/envs/vec_env/utils/share_memory.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1909 2023-04-12 14:34:56.000000 openrl-0.0.5/openrl/envs/vec_env/utils/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.133414 openrl-0.0.5/openrl/envs/vec_env/wrappers/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.5/openrl/envs/vec_env/wrappers/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     9266 2023-04-26 13:14:52.000000 openrl-0.0.5/openrl/envs/vec_env/wrappers/base_wrapper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2174 2023-04-26 13:14:42.000000 openrl-0.0.5/openrl/envs/vec_env/wrappers/reward_wrapper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3343 2023-04-26 12:42:13.000000 openrl-0.0.5/openrl/envs/vec_env/wrappers/vec_info.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2078 2023-04-26 12:38:40.000000 openrl-0.0.5/openrl/envs/vec_env/wrappers/vec_monitor.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.134682 openrl-0.0.5/openrl/envs/wrappers/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      372 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/wrappers/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2199 2023-04-26 08:59:48.000000 openrl-0.0.5/openrl/envs/wrappers/base_wrapper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2454 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/wrappers/extra_wrappers.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2533 2023-04-13 02:35:11.000000 openrl-0.0.5/openrl/envs/wrappers/multiagent_wrapper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1188 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/wrappers/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.135757 openrl-0.0.5/openrl/modules/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.5/openrl/modules/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1540 2023-04-14 07:55:18.000000 openrl-0.0.5/openrl/modules/base_module.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.136502 openrl-0.0.5/openrl/modules/common/
+-rw-r--r--   0 4paradigm   (501) staff       (20)       57 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/common/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      738 2023-04-12 14:34:56.000000 openrl-0.0.5/openrl/modules/common/base_net.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3407 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/common/ppo_net.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1210 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/model_config.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.138190 openrl-0.0.5/openrl/modules/networks/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.5/openrl/modules/networks/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1227 2023-04-14 07:55:00.000000 openrl-0.0.5/openrl/modules/networks/base_policy_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1191 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/networks/base_value_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     8075 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/networks/policy_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     6445 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/networks/policy_value_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3967 2023-04-26 13:14:52.000000 openrl-0.0.5/openrl/modules/networks/policy_value_network_gpt.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.140445 openrl-0.0.5/openrl/modules/networks/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)        0 2022-09-12 08:05:59.000000 openrl-0.0.5/openrl/modules/networks/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7389 2023-04-26 12:18:00.000000 openrl-0.0.5/openrl/modules/networks/utils/act.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     9343 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/networks/utils/attention.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2270 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/networks/utils/cnn.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      805 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/networks/utils/distributed_utils.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3551 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/networks/utils/distributions.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    10432 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/networks/utils/mix.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     5904 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/networks/utils/mlp.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.141256 openrl-0.0.5/openrl/modules/networks/utils/nlp/
+-rw-r--r--   0 4paradigm   (501) staff       (20)        0 2022-09-12 08:05:59.000000 openrl-0.0.5/openrl/modules/networks/utils/nlp/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11814 2023-04-26 13:14:42.000000 openrl-0.0.5/openrl/modules/networks/utils/nlp/base_policy.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    10986 2023-04-26 13:14:52.000000 openrl-0.0.5/openrl/modules/networks/utils/nlp/causal_policy.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)   188639 2023-04-26 13:14:53.000000 openrl-0.0.5/openrl/modules/networks/utils/nlp/hf_generation_utils.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3973 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/networks/utils/popart.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3515 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/networks/utils/rnn.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3344 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/networks/utils/transformer_act.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      317 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/networks/utils/util.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4602 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/networks/value_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7053 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/ppo_module.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     5206 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/rl_module.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.142672 openrl-0.0.5/openrl/modules/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.5/openrl/modules/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      631 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/utils/util.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3599 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/utils/valuenorm.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.143559 openrl-0.0.5/openrl/rewards/
+-rw-r--r--   0 4paradigm   (501) staff       (20)        0 2023-04-26 08:59:55.000000 openrl-0.0.5/openrl/rewards/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      366 2023-04-26 13:14:42.000000 openrl-0.0.5/openrl/rewards/base_reward.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2808 2023-04-26 13:14:42.000000 openrl-0.0.5/openrl/rewards/nlp_reward.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      572 2023-04-26 13:14:42.000000 openrl-0.0.5/openrl/rewards/register.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.143787 openrl-0.0.5/openrl/runners/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.5/openrl/runners/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.145211 openrl-0.0.5/openrl/runners/common/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      156 2023-04-26 13:14:42.000000 openrl-0.0.5/openrl/runners/common/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1263 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/runners/common/base_agent.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3186 2023-04-26 13:56:42.000000 openrl-0.0.5/openrl/runners/common/chat_agent.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     6112 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/runners/common/ppo_agent.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.145417 openrl-0.0.5/openrl/supports/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.5/openrl/supports/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.145681 openrl-0.0.5/openrl/supports/opendata/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-26 13:08:19.000000 openrl-0.0.5/openrl/supports/opendata/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.146289 openrl-0.0.5/openrl/supports/opendata/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-26 13:08:19.000000 openrl-0.0.5/openrl/supports/opendata/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2132 2023-04-26 12:30:15.000000 openrl-0.0.5/openrl/supports/opendata/utils/opendata_utils.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.146921 openrl-0.0.5/openrl/supports/opengpu/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-26 13:08:19.000000 openrl-0.0.5/openrl/supports/opengpu/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3897 2023-04-26 13:11:15.000000 openrl-0.0.5/openrl/supports/opengpu/gpu_info.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7051 2023-04-26 13:14:52.000000 openrl-0.0.5/openrl/supports/opengpu/manager.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.147913 openrl-0.0.5/openrl/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.5/openrl/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     5744 2023-04-26 13:12:54.000000 openrl-0.0.5/openrl/utils/logger.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1482 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/utils/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.116857 openrl-0.0.5/openrl.egg-info/
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11299 2023-04-26 15:36:17.000000 openrl-0.0.5/openrl.egg-info/PKG-INFO
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4465 2023-04-26 15:36:17.000000 openrl-0.0.5/openrl.egg-info/SOURCES.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)        1 2023-04-26 15:36:17.000000 openrl-0.0.5/openrl.egg-info/dependency_links.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       46 2023-04-26 15:36:17.000000 openrl-0.0.5/openrl.egg-info/entry_points.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)      284 2023-04-26 15:36:17.000000 openrl-0.0.5/openrl.egg-info/requires.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       13 2023-04-26 15:36:17.000000 openrl-0.0.5/openrl.egg-info/top_level.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       38 2023-04-26 15:36:17.149782 openrl-0.0.5/setup.cfg
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3066 2023-04-26 14:24:44.000000 openrl-0.0.5/setup.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.148153 openrl-0.0.5/tests/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.5/tests/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.148713 openrl-0.0.5/tests/project/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.5/tests/project/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      972 2023-04-25 09:16:38.000000 openrl-0.0.5/tests/project/test_version.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.149152 openrl-0.0.5/tests/test_buffer/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.5/tests/test_buffer/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1803 2023-04-25 09:16:38.000000 openrl-0.0.5/tests/test_buffer/test_buffer.py
```

### Comparing `openrl-0.0.4/LICENSE` & `openrl-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openrl-0.0.4/LICENSE.txt` & `openrl-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openrl-0.0.4/openrl/algorithms/__init__.py` & `openrl-0.0.5/openrl/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.4/openrl/algorithms/base_algorithm.py` & `openrl-0.0.5/openrl/algorithms/base_algorithm.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 
 from abc import ABC, abstractmethod
+
 import torch
 
 
 class BaseAlgorithm(ABC):
     def __init__(self, cfg, init_module, agent_num: int, device=torch.device("cpu")):
         self.cfg = cfg
```

### Comparing `openrl-0.0.4/openrl/algorithms/ppo.py` & `openrl-0.0.5/openrl/algorithms/ppo.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import numpy as np
 import torch
 import torch.nn as nn
 from torch.nn.parallel import DistributedDataParallel
 
 from openrl.algorithms.base_algorithm import BaseAlgorithm
-from openrl.utils.util import check
-from openrl.modules.utils.util import get_gard_norm, huber_loss, mse_loss
-
 from openrl.modules.networks.utils.distributed_utils import reduce_tensor
+from openrl.modules.utils.util import get_gard_norm, huber_loss, mse_loss
+from openrl.utils.util import check
 
 
 class PPOAlgorithm(BaseAlgorithm):
     def __init__(
         self,
         cfg,
         init_module,
         agent_num: int = 1,
         device: Union[str, torch.device] = "cpu",
     ) -> None:
+        self._use_share_model = cfg.use_share_model
         self.use_joint_action_loss = cfg.use_joint_action_loss
         super(PPOAlgorithm, self).__init__(cfg, init_module, agent_num, device)
 
     def ppo_update(self, sample, turn_on=True):
         for optimizer in self.algo_module.optimizers.values():
             optimizer.zero_grad()
 
@@ -120,31 +120,37 @@
                 grad_norm = get_gard_norm(
                     self.algo_module.models["transformer"].parameters()
                 )
             critic_grad_norm = grad_norm
             actor_grad_norm = grad_norm
 
         else:
+            if self._use_share_model:
+                actor_para = self.algo_module.models["model"].get_actor_para()
+            else:
+                actor_para = self.algo_module.models["policy"].parameters()
+
             if self._use_max_grad_norm:
                 actor_grad_norm = nn.utils.clip_grad_norm_(
-                    self.algo_module.models["policy"].parameters(), self.max_grad_norm
+                    actor_para, self.max_grad_norm
                 )
             else:
-                actor_grad_norm = get_gard_norm(
-                    self.algo_module.models["policy"].parameters()
-                )
+                actor_grad_norm = get_gard_norm(actor_para)
+
+            if self._use_share_model:
+                critic_para = self.algo_module.models["model"].get_critic_para()
+            else:
+                critic_para = self.algo_module.models["critic"].parameters()
 
             if self._use_max_grad_norm:
                 critic_grad_norm = nn.utils.clip_grad_norm_(
-                    self.algo_module.models["critic"].parameters(), self.max_grad_norm
+                    critic_para, self.max_grad_norm
                 )
             else:
-                critic_grad_norm = get_gard_norm(
-                    self.algo_module.models["critic"].parameters()
-                )
+                critic_grad_norm = get_gard_norm(critic_para)
 
         if self.use_amp:
             for optimizer in self.algo_module.optimizers.values():
                 self.algo_module.scaler.unscale_(optimizer)
 
             for optimizer in self.algo_module.optimizers.values():
                 self.algo_module.scaler.step(optimizer)
@@ -317,15 +323,17 @@
             policy_loss = (
                 policy_action_loss + policy_value_loss * self.policy_value_loss_coef
             )
         else:
             policy_loss = policy_action_loss
 
         # critic update
-        if isinstance(self.algo_module.models["critic"], DistributedDataParallel):
+        if self._use_share_model:
+            value_normalizer = self.algo_module.models["model"].value_normalizer
+        elif isinstance(self.algo_module.models["critic"], DistributedDataParallel):
             value_normalizer = self.algo_module.models["critic"].module.value_normalizer
         else:
             value_normalizer = self.algo_module.get_critic_value_normalizer()
         value_loss = self.cal_value_loss(
             value_normalizer,
             values,
             value_preds_batch,
@@ -347,15 +355,17 @@
                 loss_list.append(final_p_loss)
             final_v_loss = value_loss * self.value_loss_coef
             loss_list.append(final_v_loss)
         return loss_list, value_loss, policy_loss, dist_entropy, ratio
 
     def train(self, buffer, turn_on=True):
         if self._use_popart or self._use_valuenorm:
-            if isinstance(self.algo_module.models["critic"], DistributedDataParallel):
+            if self._use_share_model:
+                value_normalizer = self.algo_module.models["model"].value_normalizer
+            elif isinstance(self.algo_module.models["critic"], DistributedDataParallel):
                 value_normalizer = self.algo_module.models[
                     "critic"
                 ].module.value_normalizer
             else:
                 value_normalizer = self.algo_module.get_critic_value_normalizer()
             advantages = buffer.returns[:-1] - value_normalizer.denormalize(
                 buffer.value_preds[:-1]
```

### Comparing `openrl-0.0.4/openrl/buffers/__init__.py` & `openrl-0.0.5/openrl/buffers/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.4/openrl/buffers/normal_buffer.py` & `openrl-0.0.5/openrl/buffers/normal_buffer.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.4/openrl/buffers/replay_data.py` & `openrl-0.0.5/openrl/buffers/replay_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,33 +12,32 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 
-import torch
-import numpy as np
 from collections import defaultdict
+
+import numpy as np
+import torch
 from torch.utils.data.sampler import BatchSampler, SubsetRandomSampler
 
-from openrl.buffers.utils.util import (
-    get_policy_obs_space,
-    get_critic_obs_space,
-    get_shape_from_act_space,
-    get_policy_obs,
-    get_critic_obs,
-)
 from openrl.buffers.utils.obs_data import ObsData
 from openrl.buffers.utils.util import (
-    _flatten,
-    _flatten_v3,
     _cast,
     _cast_v3,
+    _flatten,
+    _flatten_v3,
     _shuffle_agent_grid,
+    get_critic_obs,
+    get_critic_obs_space,
+    get_policy_obs,
+    get_policy_obs_space,
+    get_shape_from_act_space,
 )
 
 
 class ReplayData(object):
     def __init__(
         self,
         cfg,
@@ -100,15 +99,15 @@
                 )
             self.policy_obs = ObsData(self.policy_obs)
             self.critic_obs = ObsData(self.critic_obs)
 
         else:
             # deal with special attn format
             if type(policy_obs_shape[-1]) == list:
-                obs_shape = policy_obs_shape[:1]
+                policy_obs_shape[:1]
 
             if type(critic_obs_shape[-1]) == list:
                 critic_obs_shape = critic_obs_shape[:1]
 
             self.critic_obs = np.zeros(
                 (
                     self.episode_length + 1,
@@ -193,14 +192,23 @@
         data = getattr(self, data_name)
 
         if isinstance(data, ObsData):
             return data.step_batch(step)
         else:
             return np.concatenate(data[step])
 
+    def all_batch_data(self, data_name: str, min=None, max=None):
+        assert hasattr(self, data_name)
+        data = getattr(self, data_name)
+
+        if isinstance(data, ObsData):
+            return data.all_batch(min, max)
+        else:
+            return data[min:max].reshape((-1, *data.shape[3:]))
+
     def dict_insert(self, data):
         if self._mixed_obs:
             for key in self.critic_obs.keys():
                 self.critic_obs[key][self.step + 1] = data["critic_obs"][key].copy()
             for key in self.policy_obs.keys():
                 self.policy_obs[key][self.step + 1] = data["policy_obs"][key].copy()
         else:
@@ -256,16 +264,14 @@
         else:
             self.critic_obs[self.step + 1] = critic_obs.copy()
             self.policy_obs[self.step + 1] = policy_obs.copy()
 
         self.rnn_states[self.step + 1] = rnn_states.copy()
         self.rnn_states_critic[self.step + 1] = rnn_states_critic.copy()
         self.actions[self.step] = actions.copy()
-        # print(self.action_log_probs[self.step],action_log_probs,action_log_probs.shape)
-        # import pdb;pdb.set_trace()
         self.action_log_probs[self.step] = action_log_probs.copy()
         self.value_preds[self.step] = value_preds.copy()
         self.rewards[self.step] = rewards.copy()
         self.masks[self.step + 1] = masks.copy()
         if bad_masks is not None:
             self.bad_masks[self.step + 1] = bad_masks.copy()
         if active_masks is not None:
@@ -403,26 +409,158 @@
                 self.returns[-1] = next_value
                 for step in reversed(range(self.rewards.shape[0])):
                     self.returns[step] = (
                         self.returns[step + 1] * self.gamma * self.masks[step + 1]
                         + self.rewards[step]
                     )
 
+    def recurrent_generator_v3(self, advantages, num_mini_batch, data_chunk_length):
+        episode_length, n_rollout_threads, num_agents = self.rewards.shape[0:3]
+        batch_size = n_rollout_threads * episode_length
+        data_chunks = batch_size // data_chunk_length  # [C=r*T*M/L]
+        mini_batch_size = data_chunks // num_mini_batch
+
+        assert n_rollout_threads * episode_length >= data_chunk_length, (
+            "PPO requires the nfumber of processes ({}) * episode length ({}) "
+            "to be greater than or equal to the number of "
+            "data chunk length ({}).".format(
+                n_rollout_threads, num_agents, episode_length, data_chunk_length
+            )
+        )
+
+        rand = torch.randperm(data_chunks).numpy()
+        sampler = [
+            rand[i * mini_batch_size : (i + 1) * mini_batch_size]
+            for i in range(num_mini_batch)
+        ]
+
+        critic_obs = _cast_v3(self.critic_obs[:-1])
+        policy_obs = _cast_v3(self.policy_obs[:-1])
+
+        actions = _cast_v3(self.actions)
+        action_log_probs = _cast_v3(self.action_log_probs)
+        advantages = _cast_v3(advantages)
+        value_preds = _cast_v3(self.value_preds[:-1])
+        returns = _cast_v3(self.returns[:-1])
+        masks = _cast_v3(self.masks[:-1])
+        active_masks = _cast_v3(self.active_masks[:-1])
+
+        rnn_states = (
+            self.rnn_states[:-1]
+            .transpose(1, 0, 2, 3, 4)
+            .reshape(-1, *self.rnn_states.shape[2:])
+        )
+        rnn_states_critic = (
+            self.rnn_states_critic[:-1]
+            .transpose(1, 0, 2, 3, 4)
+            .reshape(-1, *self.rnn_states_critic.shape[2:])
+        )
+
+        if self.available_actions is not None:
+            available_actions = _cast_v3(self.available_actions[:-1])
+
+        for indices in sampler:
+            critic_obs_batch = []
+            policy_obs_batch = []
+
+            rnn_states_batch = []
+            rnn_states_critic_batch = []
+            actions_batch = []
+            available_actions_batch = []
+            value_preds_batch = []
+            return_batch = []
+            masks_batch = []
+            active_masks_batch = []
+            old_action_log_probs_batch = []
+            adv_targ = []
+
+            for index in indices:
+                ind = index * data_chunk_length
+                # size [T+1 N M Dim]-->[T N M Dim]-->[N,M,T,Dim]-->[N*M*T,Dim]-->[L,Dim]
+                # [L, agent_num, Dim]
+                critic_obs_batch.append(critic_obs[ind : ind + data_chunk_length])
+                policy_obs_batch.append(policy_obs[ind : ind + data_chunk_length])
+
+                actions_batch.append(actions[ind : ind + data_chunk_length])
+                if self.available_actions is not None:
+                    available_actions_batch.append(
+                        available_actions[ind : ind + data_chunk_length]
+                    )
+                value_preds_batch.append(value_preds[ind : ind + data_chunk_length])
+                return_batch.append(returns[ind : ind + data_chunk_length])
+                masks_batch.append(masks[ind : ind + data_chunk_length])
+                active_masks_batch.append(active_masks[ind : ind + data_chunk_length])
+                old_action_log_probs_batch.append(
+                    action_log_probs[ind : ind + data_chunk_length]
+                )
+                adv_targ.append(advantages[ind : ind + data_chunk_length])
+                # size [T+1 N M Dim]-->[T N M Dim]-->[N M T Dim]-->[N*M*T,Dim]-->[1,Dim]
+                # [1,agent_num, Dim]
+                rnn_states_batch.append(rnn_states[ind])
+                rnn_states_critic_batch.append(rnn_states_critic[ind])
+
+            L, N = data_chunk_length, mini_batch_size
+
+            # These are all from_numpys of size (L, N, agent_num, Dim)
+
+            critic_obs_batch = np.stack(critic_obs_batch, axis=1)
+            policy_obs_batch = np.stack(policy_obs_batch, axis=1)
+
+            actions_batch = np.stack(actions_batch, axis=1)
+            if self.available_actions is not None:
+                available_actions_batch = np.stack(available_actions_batch, axis=1)
+            value_preds_batch = np.stack(value_preds_batch, axis=1)
+            return_batch = np.stack(return_batch, axis=1)
+            masks_batch = np.stack(masks_batch, axis=1)
+            active_masks_batch = np.stack(active_masks_batch, axis=1)
+            old_action_log_probs_batch = np.stack(old_action_log_probs_batch, axis=1)
+            adv_targ = np.stack(adv_targ, axis=1)
+
+            # States is just a (N, agent_num, -1) from_numpy
+            rnn_states_batch = np.stack(rnn_states_batch).reshape(
+                N * num_agents, *self.rnn_states.shape[3:]
+            )
+            rnn_states_critic_batch = np.stack(rnn_states_critic_batch).reshape(
+                N * num_agents, *self.rnn_states_critic.shape[3:]
+            )
+            # Flatten the (L, N, ...) from_numpys to (L * N, ...)
+
+            critic_obs_batch = _flatten_v3(L, N, num_agents, critic_obs_batch)
+            policy_obs_batch = _flatten_v3(L, N, num_agents, policy_obs_batch)
+            actions_batch = _flatten_v3(L, N, num_agents, actions_batch)
+            if self.available_actions is not None:
+                available_actions_batch = _flatten_v3(
+                    L, N, num_agents, available_actions_batch
+                )
+            else:
+                available_actions_batch = None
+            value_preds_batch = _flatten_v3(L, N, num_agents, value_preds_batch)
+            return_batch = _flatten_v3(L, N, num_agents, return_batch)
+            masks_batch = _flatten_v3(L, N, num_agents, masks_batch)
+            active_masks_batch = _flatten_v3(L, N, num_agents, active_masks_batch)
+            old_action_log_probs_batch = _flatten_v3(
+                L, N, num_agents, old_action_log_probs_batch
+            )
+            adv_targ = _flatten_v3(L, N, num_agents, adv_targ)
+            yield critic_obs_batch, policy_obs_batch, rnn_states_batch, rnn_states_critic_batch, actions_batch, value_preds_batch, return_batch, masks_batch, active_masks_batch, old_action_log_probs_batch, adv_targ, available_actions_batch
+
     def feed_forward_generator(
         self,
         advantages,
         num_mini_batch=None,
         mini_batch_size=None,
         critic_obs_process_func=None,
     ):
         episode_length, n_rollout_threads, num_agents = self.rewards.shape[0:3]
         batch_size = n_rollout_threads * episode_length * num_agents
 
         if mini_batch_size is None:
-            assert batch_size >= num_mini_batch, (
+            assert (
+                batch_size >= num_mini_batch
+            ), (
                 "PPO requires the number of processes ({}) "
                 "* number of steps ({}) * number of agents ({}) = {} "
                 "to be greater than or equal to the number of PPO mini batches ({})."
                 "".format(
                     n_rollout_threads,
                     episode_length,
                     num_agents,
@@ -509,15 +647,17 @@
         mini_batch_size=None,
         critic_obs_process_func=None,
     ):
         episode_length, n_rollout_threads, num_agents = self.rewards.shape[0:3]
         batch_size = n_rollout_threads * episode_length
 
         if mini_batch_size is None:
-            assert batch_size >= num_mini_batch, (
+            assert (
+                batch_size >= num_mini_batch
+            ), (
                 "PPO requires the number of processes ({}) "
                 "* number of steps ({}) * number of agents ({}) = {} "
                 "to be greater than or equal to the number of PPO mini batches ({})."
                 "".format(
                     n_rollout_threads,
                     episode_length,
                     num_agents,
@@ -570,15 +710,17 @@
         :param num_mini_batch: (int) number of minibatches to split the batch into.
         :param mini_batch_size: (int) number of samples in each minibatch.
         """
         episode_length, n_rollout_threads, num_agents = self.rewards.shape[0:3]
         batch_size = n_rollout_threads * episode_length
 
         if mini_batch_size is None:
-            assert batch_size >= num_mini_batch, (
+            assert (
+                batch_size >= num_mini_batch
+            ), (
                 "PPO requires the number of processes ({}) "
                 "* number of steps ({}) = {} "
                 "to be greater than or equal to the number of PPO mini batches ({})."
                 "".format(
                     n_rollout_threads,
                     episode_length,
                     n_rollout_threads * episode_length,
@@ -811,15 +953,17 @@
         :param num_mini_batch: (int) number of minibatches to split the batch into.
         :param mini_batch_size: (int) number of samples in each minibatch.
         """
         episode_length, n_rollout_threads, num_agents = self.rewards.shape[0:3]
         batch_size = n_rollout_threads * episode_length
 
         if mini_batch_size is None:
-            assert batch_size >= num_mini_batch, (
+            assert (
+                batch_size >= num_mini_batch
+            ), (
                 "PPO requires the number of processes ({}) "
                 "* number of steps ({}) = {} "
                 "to be greater than or equal to the number of PPO mini batches ({})."
                 "".format(
                     n_rollout_threads,
                     episode_length,
                     n_rollout_threads * episode_length,
@@ -910,157 +1054,24 @@
             )
             if advantages is None:
                 adv_targ = None
             else:
                 adv_targ = advantages[indices].reshape(-1, *advantages.shape[2:])
             yield critic_obs_batch, policy_obs_batch, rnn_states_batch, rnn_states_critic_batch, actions_batch, value_preds_batch, return_batch, masks_batch, active_masks_batch, old_action_log_probs_batch, adv_targ, available_actions_batch
 
-    def recurrent_generator_v3(self, advantages, num_mini_batch, data_chunk_length):
-        episode_length, n_rollout_threads, num_agents = self.rewards.shape[0:3]
-        batch_size = n_rollout_threads * episode_length
-        data_chunks = batch_size // data_chunk_length  # [C=r*T*M/L]
-        mini_batch_size = data_chunks // num_mini_batch
-
-        assert n_rollout_threads * episode_length >= data_chunk_length, (
-            "PPO requires the nfumber of processes ({}) * episode length ({}) "
-            "to be greater than or equal to the number of "
-            "data chunk length ({}).".format(
-                n_rollout_threads, num_agents, episode_length, data_chunk_length
-            )
-        )
-
-        rand = torch.randperm(data_chunks).numpy()
-        sampler = [
-            rand[i * mini_batch_size : (i + 1) * mini_batch_size]
-            for i in range(num_mini_batch)
-        ]
-
-        critic_obs = _cast_v3(self.critic_obs[:-1])
-        policy_obs = _cast_v3(self.policy_obs[:-1])
-
-        actions = _cast_v3(self.actions)
-        action_log_probs = _cast_v3(self.action_log_probs)
-        advantages = _cast_v3(advantages)
-        value_preds = _cast_v3(self.value_preds[:-1])
-        returns = _cast_v3(self.returns[:-1])
-        masks = _cast_v3(self.masks[:-1])
-        active_masks = _cast_v3(self.active_masks[:-1])
-
-        rnn_states = (
-            self.rnn_states[:-1]
-            .transpose(1, 0, 2, 3, 4)
-            .reshape(-1, *self.rnn_states.shape[2:])
-        )
-        rnn_states_critic = (
-            self.rnn_states_critic[:-1]
-            .transpose(1, 0, 2, 3, 4)
-            .reshape(-1, *self.rnn_states_critic.shape[2:])
-        )
-
-        if self.available_actions is not None:
-            available_actions = _cast_v3(self.available_actions[:-1])
-
-        for indices in sampler:
-            critic_obs_batch = []
-            policy_obs_batch = []
-
-            rnn_states_batch = []
-            rnn_states_critic_batch = []
-            actions_batch = []
-            available_actions_batch = []
-            value_preds_batch = []
-            return_batch = []
-            masks_batch = []
-            active_masks_batch = []
-            old_action_log_probs_batch = []
-            adv_targ = []
-
-            for index in indices:
-                ind = index * data_chunk_length
-                # size [T+1 N M Dim]-->[T N M Dim]-->[N,M,T,Dim]-->[N*M*T,Dim]-->[L,Dim]
-                # [L, agent_num, Dim]
-                critic_obs_batch.append(critic_obs[ind : ind + data_chunk_length])
-                policy_obs_batch.append(policy_obs[ind : ind + data_chunk_length])
-
-                actions_batch.append(actions[ind : ind + data_chunk_length])
-                if self.available_actions is not None:
-                    available_actions_batch.append(
-                        available_actions[ind : ind + data_chunk_length]
-                    )
-                value_preds_batch.append(value_preds[ind : ind + data_chunk_length])
-                return_batch.append(returns[ind : ind + data_chunk_length])
-                masks_batch.append(masks[ind : ind + data_chunk_length])
-                active_masks_batch.append(active_masks[ind : ind + data_chunk_length])
-                old_action_log_probs_batch.append(
-                    action_log_probs[ind : ind + data_chunk_length]
-                )
-                adv_targ.append(advantages[ind : ind + data_chunk_length])
-                # size [T+1 N M Dim]-->[T N M Dim]-->[N M T Dim]-->[N*M*T,Dim]-->[1,Dim]
-                # [1,agent_num, Dim]
-                rnn_states_batch.append(rnn_states[ind])
-                rnn_states_critic_batch.append(rnn_states_critic[ind])
-
-            L, N = data_chunk_length, mini_batch_size
-
-            # These are all from_numpys of size (L, N, agent_num, Dim)
-
-            critic_obs_batch = np.stack(critic_obs_batch, axis=1)
-            policy_obs_batch = np.stack(policy_obs_batch, axis=1)
-
-            actions_batch = np.stack(actions_batch, axis=1)
-            if self.available_actions is not None:
-                available_actions_batch = np.stack(available_actions_batch, axis=1)
-            value_preds_batch = np.stack(value_preds_batch, axis=1)
-            return_batch = np.stack(return_batch, axis=1)
-            masks_batch = np.stack(masks_batch, axis=1)
-            active_masks_batch = np.stack(active_masks_batch, axis=1)
-            old_action_log_probs_batch = np.stack(old_action_log_probs_batch, axis=1)
-            adv_targ = np.stack(adv_targ, axis=1)
-
-            # States is just a (N, agent_num, -1) from_numpy
-            rnn_states_batch = np.stack(rnn_states_batch).reshape(
-                N * num_agents, *self.rnn_states.shape[3:]
-            )
-            rnn_states_critic_batch = np.stack(rnn_states_critic_batch).reshape(
-                N * num_agents, *self.rnn_states_critic.shape[3:]
-            )
-            # import pdb;pdb.set_trace()
-            # Flatten the (L, N, ...) from_numpys to (L * N, ...)
-
-            critic_obs_batch = _flatten_v3(L, N, num_agents, critic_obs_batch)
-            policy_obs_batch = _flatten_v3(L, N, num_agents, policy_obs_batch)
-            actions_batch = _flatten_v3(L, N, num_agents, actions_batch)
-            if self.available_actions is not None:
-                available_actions_batch = _flatten_v3(
-                    L, N, num_agents, available_actions_batch
-                )
-            else:
-                available_actions_batch = None
-            value_preds_batch = _flatten_v3(L, N, num_agents, value_preds_batch)
-            return_batch = _flatten_v3(L, N, num_agents, return_batch)
-            masks_batch = _flatten_v3(L, N, num_agents, masks_batch)
-            active_masks_batch = _flatten_v3(L, N, num_agents, active_masks_batch)
-            old_action_log_probs_batch = _flatten_v3(
-                L, N, num_agents, old_action_log_probs_batch
-            )
-            adv_targ = _flatten_v3(L, N, num_agents, adv_targ)
-            # print(L,N,num_agents)
-            # import pdb;pdb.set_trace()
-            yield critic_obs_batch, policy_obs_batch, rnn_states_batch, rnn_states_critic_batch, actions_batch, value_preds_batch, return_batch, masks_batch, active_masks_batch, old_action_log_probs_batch, adv_targ, available_actions_batch
-
     def recurrent_generator(self, advantages, num_mini_batch, data_chunk_length):
         episode_length, n_rollout_threads, num_agents = self.rewards.shape[0:3]
         batch_size = n_rollout_threads * episode_length * num_agents
         data_chunks = batch_size // data_chunk_length  # [C=r*T*M/L]
         mini_batch_size = data_chunks // num_mini_batch
 
         assert n_rollout_threads * episode_length * num_agents >= data_chunk_length, (
-            "PPO requires the number of processes ({})* number of agents ({}) * episode length ({}) "
-            "to be greater than or equal to the number of "
-            "data chunk length ({}).".format(
+            "PPO requires the number of processes ({})* number of agents ({}) * episode"
+            " length ({}) to be greater than or equal to the number of data chunk"
+            " length ({}).".format(
                 n_rollout_threads, num_agents, episode_length, data_chunk_length
             )
         )
 
         rand = torch.randperm(data_chunks).numpy()
         sampler = [
             rand[i * mini_batch_size : (i + 1) * mini_batch_size]
```

### Comparing `openrl-0.0.4/openrl/buffers/utils/__init__.py` & `openrl-0.0.5/openrl/buffers/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.4/openrl/buffers/utils/obs_data.py` & `openrl-0.0.5/openrl/buffers/utils/obs_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,14 +36,22 @@
 
     def step_batch(self, step):
         return_dict = {}
         for str_key in self.keys():
             return_dict[str_key] = np.concatenate(self[str_key][step])
         return return_dict
 
+    def all_batch(self, min, max):
+        return_dict = {}
+        for str_key in self.keys():
+            return_dict[str_key] = self[str_key][min:max].reshape(
+                (-1, *self[str_key].shape[3:])
+            )
+        return return_dict
+
     def __getitem__(self, key):
         if isinstance(key, int):
             return self.step_batch(key)
         else:
             return super().__getitem__(key)
 
     def step_flatten(self, step):
```

### Comparing `openrl-0.0.4/openrl/buffers/utils/util.py` & `openrl-0.0.5/openrl/buffers/utils/util.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
-from gymnasium.spaces import Dict
 import numpy as np
+from gymnasium.spaces import Dict
 
 
 def get_policy_obs(raw_obs):
     if isinstance(raw_obs, dict):
         if "policy" in raw_obs:
             return get_obs(raw_obs, model_name="policy")
     return get_obs(raw_obs)
```

### Comparing `openrl-0.0.4/openrl/cli/__init__.py` & `openrl-0.0.5/openrl/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.4/openrl/cli/cli.py` & `openrl-0.0.5/openrl/cli/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,18 +14,19 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 
 import click
 from click.core import Context, Option
-
-from openrl import __TITLE__, __VERSION__, __AUTHOR__, __EMAIL__
 from termcolor import colored
 
+from openrl import __AUTHOR__, __EMAIL__, __TITLE__, __VERSION__
+from openrl.utils.util import get_system_info
+
 
 def red(text: str):
     return colored(text, "red")
 
 
 def print_version(
     ctx: Context,
@@ -35,27 +36,48 @@
     if not value or ctx.resilient_parsing:
         return
     click.secho(f"{__TITLE__.upper()} version: {red(__VERSION__)}")
     click.secho(f"Developed by {__AUTHOR__}, Email: {red(__EMAIL__)}")
     ctx.exit()
 
 
+def print_system_info(
+    ctx: Context,
+    param: Option,
+    value: bool,
+) -> None:
+    if not value or ctx.resilient_parsing:
+        return
+    info_dict = get_system_info()
+    for key, value in info_dict.items():
+        click.secho(f"- {key}: {red(value)}")
+    ctx.exit()
+
+
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 
 @click.command(context_settings=CONTEXT_SETTINGS)
 @click.option(
     "--version",
     is_flag=True,
     callback=print_version,
     expose_value=False,
     is_eager=True,
     help="Show package's version information.",
 )
 @click.option(
+    "--system_info",
+    is_flag=True,
+    callback=print_system_info,
+    expose_value=False,
+    is_eager=True,
+    help="Show system information.",
+)
+@click.option(
     "--mode",
     prompt="Choose execution mode",
     type=click.Choice(
         [
             "train",
         ]
     ),
```

### Comparing `openrl-0.0.4/openrl/cli/train.py` & `openrl-0.0.5/openrl/cli/train.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,41 +13,36 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 import numpy as np
 
+from openrl.configs.config import create_config_parser
 from openrl.envs.common import make
 from openrl.modules.common import PPONet as Net
 from openrl.runners.common import PPOAgent as Agent
-from openrl.configs.config import create_config_parser
 
 
 def train_agent(env: str, total_time_steps: int = 20000):
     render_model = "rgb_array"
     env_num = 9
-    env = make(env, render_mode=render_model, env_num=env_num, asynchronous=True)
+    env = make(env, render_mode=render_model, env_num=env_num, asynchronous=False)
     cfg_parser = create_config_parser()
     cfg = cfg_parser.parse_args([])
-    # 创建 神经网络
     net = Net(env, cfg=cfg)
-
-    # 初始化训练器
     agent = Agent(net, use_wandb=False)
-    # 开始训练
     agent.train(total_time_steps=total_time_steps)
 
     agent.set_env(env)
     obs, info = env.reset()
     done = False
     step = 0
     total_reward = 0
     while not np.any(done):
-        # 智能体根据 observation 预测下一个动作
         action, _ = agent.act(obs, deterministic=True)
         obs, r, done, info = env.step(action)
         total_reward += np.mean(r)
         step += 1
     print(f"Total reward: {total_reward}")
 
     env.close()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `openrl-0.0.4/openrl/configs/__init__.py` & `openrl-0.0.5/openrl/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.4/openrl/configs/config.py` & `openrl-0.0.5/openrl/configs/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """"""
-from jsonargparse import ArgumentParser, ActionConfigFile
+from jsonargparse import ActionConfigFile, ArgumentParser
 
 
 def create_config_parser():
     """
     The configuration parser.
     """
     parser = ArgumentParser(
@@ -69,15 +69,15 @@
     parser.add_argument(
         "--gail_epoch", type=int, default=5, help="gail epochs (default: 5)"
     )
     parser.add_argument(
         "--disable_action",
         action="store_true",
         default=False,
-        help="whether to use action as the input of the " "discriminator",
+        help="whether to use action as the input of the discriminator",
     )
     parser.add_argument(
         "--gail_hidden_size",
         type=int,
         default=256,
         help="gail hidden state size (default: 256)",
     )
@@ -299,27 +299,32 @@
     )
 
     parser.add_argument(
         "--gpu_usage_type",
         type=str,
         default="auto",
         choices=["auto", "single"],
-        help="by default auto, will determine the GPU automatically. If using single, use only use single GPU.",
+        help=(
+            "by default auto, will determine the GPU automatically. If using single,"
+            " use only use single GPU."
+        ),
     )
     parser.add_argument(
         "--disable_cuda",
         action="store_true",
         default=False,
         help="by default False, will use GPU to train; or else will use CPU;",
     )
     parser.add_argument(
         "--cuda_deterministic",
         action="store_false",
         default=True,
-        help="by default, make sure random seed effective. if set, bypass such function.",
+        help=(
+            "by default, make sure random seed effective. if set, bypass such function."
+        ),
     )
     parser.add_argument(
         "--pytorch_threads",
         type=int,
         default=1,
         help="Number of torch threads for training",
     )
@@ -353,21 +358,26 @@
         default="openrl",
         help="user name for the running process",
     )
     parser.add_argument(
         "--wandb_entity",
         type=str,
         default=None,
-        help="[for wandb usage], to specify entity for simply collecting training data.",
+        help=(
+            "[for wandb usage], to specify entity for simply collecting training data."
+        ),
     )
     parser.add_argument(
         "--disable_wandb",
         action="store_true",
         default=False,
-        help="[for wandb usage], by default False, will log date to wandb server. or else will use tensorboard to log data.",
+        help=(
+            "[for wandb usage], by default False, will log date to wandb server. or"
+            " else will use tensorboard to log data."
+        ),
     )
     # env parameters
     parser.add_argument(
         "--env_name",
         type=str,
         default="StarCraft2",
         help="specify the name of environment",
@@ -472,15 +482,18 @@
         default=False,
         help="Whether to apply layernorm to the inputs",
     )
     parser.add_argument(
         "--use_orthogonal",
         action="store_false",
         default=True,
-        help="Whether to use Orthogonal initialization for weights and 0 initialization for biases",
+        help=(
+            "Whether to use Orthogonal initialization for weights and 0 initialization"
+            " for biases"
+        ),
     )
     parser.add_argument(
         "--gain", type=float, default=0.01, help="The gain # of last action layer"
     )
     parser.add_argument(
         "--cnn_layers_params",
         type=str,
@@ -756,15 +769,18 @@
         help="time duration between contiunous twice log printing.",
     )
     # eval parameters
     parser.add_argument(
         "--use_eval",
         action="store_true",
         default=False,
-        help="by default, do not start evaluation. If set`, start evaluation alongside with training.",
+        help=(
+            "by default, do not start evaluation. If set`, start evaluation alongside"
+            " with training."
+        ),
     )
     parser.add_argument(
         "--eval_interval",
         type=int,
         default=25,
         help="time duration between contiunous twice evaluation progress.",
     )
@@ -781,15 +797,19 @@
         default=False,
         help="by default, do not save render video. If set, save video.",
     )
     parser.add_argument(
         "--use_render",
         action="store_true",
         default=False,
-        help="by default, do not render the env during training. If set, start render. Note: something, the environment has internal render process which is not controlled by this hyperparam.",
+        help=(
+            "by default, do not render the env during training. If set, start render."
+            " Note: something, the environment has internal render process which is not"
+            " controlled by this hyperparam."
+        ),
     )
     parser.add_argument(
         "--render_episodes",
         type=int,
         default=5,
         help="the number of episodes to render a given env",
     )
@@ -825,15 +845,18 @@
         help="root dir to save curves, logs and models.",
     )
     # replay buffer parameters
     parser.add_argument(
         "--use_transmit",
         action="store_true",
         default=False,
-        help="by default, do not use transmit. If set`, use transmit as the replay buffer.",
+        help=(
+            "by default, do not use transmit. If set`, use transmit as the replay"
+            " buffer."
+        ),
     )
     # reverb server address
     parser.add_argument(
         "--server_address", type=str, default=None, help="Replay buffer server address."
     )
     parser.add_argument(
         "--use_tlaunch", action="store_true", default=False, help="whether use tlaunch."
@@ -990,17 +1013,82 @@
         default=32,
         help="Dimension of hidden layer of mixing network",
     )
     parser.add_argument(
         "--hypernet_hidden_dim",
         type=int,
         default=64,
-        help="Dimension of hidden layer of hypernetwork (only applicable if hypernet_layers == 2",
+        help=(
+            "Dimension of hidden layer of hypernetwork (only applicable if"
+            " hypernet_layers == 2"
+        ),
     )
     # rmatd3 parameters
     parser.add_argument(
         "--target_action_noise_std",
         default=0.2,
         help="Target action smoothing noise for matd3",
     )
+
+    parser.add_argument(
+        "--data_path",
+        default=None,
+        type=str,
+        help="the path of the training data",
+    )
+    parser.add_argument(
+        "--env.args",
+        default={},
+        type=dict,
+        help="the args of the env",
+    )
+    parser.add_argument(
+        "--model_path",
+        default=None,
+        type=str,
+        help="the path of the model",
+    )
+    parser.add_argument(
+        "--use_share_model",
+        action="store_true",
+        default=False,
+        help="use one class to implement policy and value networks",
+    )
+
+    # rewards class
+    parser.add_argument(
+        "--reward_class.id",
+        default=None,
+        type=str,
+        help="the id of the reward class",
+    )
+    parser.add_argument(
+        "--reward_class.args",
+        default={},
+        type=dict,
+        help="the parameters of the reward class",
+    )
+
+    # vec info class
+    parser.add_argument(
+        "--vec_info_class.id",
+        default=None,
+        type=str,
+        help="the id of the vec env's info class",
+    )
+    parser.add_argument(
+        "--vec_info_class.args",
+        default={},
+        type=dict,
+        help="the parameters of the vec info class",
+    )
+
+    # vec info class
+    parser.add_argument(
+        "--eval_metrics",
+        nargs="+",
+        type=dict,
+        default=[],
+        help="the id of the vec env's info class",
+    )
     parser.add_argument("--config", action=ActionConfigFile)
     return parser
```

### Comparing `openrl-0.0.4/openrl/drivers/__init__.py` & `openrl-0.0.5/openrl/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.4/openrl/drivers/onpolicy_driver.py` & `openrl-0.0.5/openrl/drivers/onpolicy_driver.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
-from typing import Dict, Any, Optional
+from typing import Any, Dict, Optional
+
 import numpy as np
 import torch
 from torch.nn.parallel import DistributedDataParallel
 
 from openrl.drivers.rl_driver import RLDriver
-
-from openrl.utils.util import _t2n
 from openrl.utils.logger import Logger
+from openrl.utils.util import _t2n
 
 
 class OnPolicyDriver(RLDriver):
     def __init__(
         self,
         config: Dict[str, Any],
         trainer,
@@ -50,16 +50,14 @@
         self.device = config["device"]
 
         assert not (
             self.program_type != "actor" and self.world_size is None
         ), "world size can not be none, get {}".format(world_size)
 
         self.num_agents = config["num_agents"]
-
-        # print(cfg)
         assert isinstance(rank, int), "rank must be int, but get {}".format(rank)
         self.rank = rank
 
         # for distributed learning
         assert not (
             world_size is None and self.program_type == "learner"
         ), "world_size must be int, but get {}".format(world_size)
@@ -93,18 +91,17 @@
         self.actor_num = cfg.actor_num
 
         if self.distributed_type == "async" and self.program_type == "whole":
             print("can't use async mode when program_type is whole!")
             exit()
 
         if self.program_type in ["whole", "local"]:
-            assert (
-                self.actor_num == 1
-            ), "when running actor and learner the same time, the actor number should be 1, but received {}".format(
-                self.actor_num
+            assert self.actor_num == 1, (
+                "when running actor and learner the same time, the actor number should"
+                " be 1, but received {}".format(self.actor_num)
             )
         # dir
         self.model_dir = cfg.model_dir
         if hasattr(cfg, "save_dir"):
             self.save_dir = cfg.save_dir
 
         self.cfg = cfg
@@ -146,70 +143,80 @@
             values,
             actions,
             action_log_probs,
             rnn_states,
             rnn_states_critic,
         ) = data
 
-        rnn_states[dones == True] = np.zeros(
-            ((dones == True).sum(), self.recurrent_N, self.hidden_size),
+        rnn_states[dones] = np.zeros(
+            (dones.sum(), self.recurrent_N, self.hidden_size),
             dtype=np.float32,
         )
 
-        rnn_states_critic[dones == True] = np.zeros(
-            ((dones == True).sum(), *self.buffer.data.rnn_states_critic.shape[3:]),
+        rnn_states_critic[dones] = np.zeros(
+            (dones.sum(), *self.buffer.data.rnn_states_critic.shape[3:]),
             dtype=np.float32,
         )
         masks = np.ones((self.n_rollout_threads, self.num_agents, 1), dtype=np.float32)
-        masks[dones == True] = np.zeros(((dones == True).sum(), 1), dtype=np.float32)
+        masks[dones] = np.zeros((dones.sum(), 1), dtype=np.float32)
 
         self.buffer.insert(
             obs,
             rnn_states,
             rnn_states_critic,
             actions,
             action_log_probs,
             values,
             rewards,
             masks,
         )
 
     def actor_rollout(self):
         self.trainer.prep_rollout()
+        import time
 
         for step in range(self.episode_length):
-            # Sample actions
+            act_data = self.act(step)
+
             (
                 values,
                 actions,
                 action_log_probs,
                 rnn_states,
                 rnn_states_critic,
-            ) = self.act(step)
+            ) = act_data
+
+            extra_data = {
+                "act_data": act_data,
+                "buffer": self.buffer,
+                "step": step,
+            }
 
-            obs, rewards, dones, infos = self.envs.step(actions)
+            obs, rewards, dones, infos = self.envs.step(actions, extra_data)
 
             data = (
                 obs,
                 rewards,
                 dones,
                 infos,
                 values,
                 actions,
                 action_log_probs,
                 rnn_states,
                 rnn_states_critic,
             )
 
             self.add2buffer(data)
-
+        infos = self.envs.batch_rewards(self.buffer)
         if self.envs.use_monitor:
-            return self.envs.statistics()
+            statistics_info = self.envs.statistics()
+            infos.update(statistics_info)
+            return infos
         else:
-            return {}
+            return infos
 
     def run(self) -> None:
         episodes = (
             int(self.num_env_steps)
             // self.episode_length
             // self.learner_n_rollout_threads
         )
@@ -252,17 +259,15 @@
         ):
             value_normalizer = self.trainer.algo_module.models[
                 "critic"
             ].module.value_normalizer
         elif "model" in self.trainer.algo_module.models and isinstance(
             self.trainer.algo_module.models["model"], DistributedDataParallel
         ):
-            value_normalizer = self.trainer.algo_module.models[
-                "model"
-            ].module.value_normalizer
+            value_normalizer = self.trainer.algo_module.models["model"].value_normalizer
         else:
             value_normalizer = self.trainer.algo_module.get_critic_value_normalizer()
         self.buffer.compute_returns(next_values, value_normalizer)
 
     @torch.no_grad()
     def act(
         self,
@@ -280,15 +285,14 @@
             self.buffer.data.get_batch_data("critic_obs", step),
             self.buffer.data.get_batch_data("policy_obs", step),
             np.concatenate(self.buffer.data.rnn_states[step]),
             np.concatenate(self.buffer.data.rnn_states_critic[step]),
             np.concatenate(self.buffer.data.masks[step]),
         )
 
-        # [self.envs, agents, dim]
         values = np.array(np.split(_t2n(value), self.n_rollout_threads))
         actions = np.array(np.split(_t2n(action), self.n_rollout_threads))
         action_log_probs = np.array(
             np.split(_t2n(action_log_prob), self.n_rollout_threads)
         )
         rnn_states = np.array(np.split(_t2n(rnn_states), self.n_rollout_threads))
         rnn_states_critic = np.array(
```

### Comparing `openrl-0.0.4/openrl/drivers/rl_driver.py` & `openrl-0.0.5/openrl/drivers/rl_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,11 +15,12 @@
 # limitations under the License.
 
 """"""
 from abc import ABC, abstractmethod
 
 from openrl.drivers.base_driver import BaseDriver
 
+
 class RLDriver(BaseDriver, ABC):
     @abstractmethod
     def _inner_loop(self):
         raise NotImplementedError
```

### Comparing `openrl-0.0.4/openrl/envs/common/__init__.py` & `openrl-0.0.5/openrl/envs/common/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,10 +12,11 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 
-from .registration import make, build_envs
+from .build_envs import build_envs
+from .registration import make
 
 __all__ = ["make", "build_envs"]
```

### Comparing `openrl-0.0.4/openrl/envs/gymnasium/__init__.py` & `openrl-0.0.5/openrl/envs/gymnasium/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,33 +11,33 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
-from typing import Callable, List, Optional, Union, Iterable
-import gymnasium as gym
+from typing import Callable, List, Optional, Union
 
+import gymnasium as gym
 from gymnasium import Env
 
 from openrl.envs.common import build_envs
 
 
 def make_gym_envs(
     id: str,
     env_num: int = 1,
     render_mode: Optional[Union[str, List[str]]] = None,
     **kwargs,
 ) -> List[Callable[[], Env]]:
     from openrl.envs.wrappers import (
-        DictWrapper,
-        Single2MultiAgentWrapper,
         AutoReset,
+        DictWrapper,
         RemoveTruncated,
+        Single2MultiAgentWrapper,
     )
 
     env_wrappers = [
         DictWrapper,
         Single2MultiAgentWrapper,
         AutoReset,
         RemoveTruncated,
```

### Comparing `openrl-0.0.4/openrl/envs/mpe/__init__.py` & `openrl-0.0.5/openrl/envs/mpe/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # MPE env fetched from https://github.com/marlbenchmark/on-policy/tree/main/onpolicy/envs/mpe
+from typing import Callable, List, Optional, Union
+
 from gymnasium import Env
-from typing import Optional, Union, List, Callable, Iterable
+
 from openrl.envs.common import build_envs
 from openrl.envs.mpe.mpe_env import make
 
-all_envs = [
-    "simple_spread",
-]
-
 
 def make_mpe_envs(
     id: str,
     env_num: int = 1,
     render_mode: Optional[Union[str, List[str]]] = None,
     **kwargs,
 ) -> List[Callable[[], Env]]:
```

### Comparing `openrl-0.0.4/openrl/envs/mpe/core.py` & `openrl-0.0.5/openrl/envs/mpe/core.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.4/openrl/envs/mpe/mpe_env.py` & `openrl-0.0.5/openrl/envs/mpe/mpe_env.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Any, Optional
+
 from gymnasium import Env
 
 from .multiagent_env import MultiAgentEnv
 from .scenarios import load
 
 
 def make(
```

### Comparing `openrl-0.0.4/openrl/envs/mpe/multi_discrete.py` & `openrl-0.0.5/openrl/envs/mpe/multi_discrete.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # An old version of OpenAI Gym's multi_discrete.py. (Was getting affected by Gym updates)
 # (https://github.com/openai/gym/blob/1fb81d4e3fb780ccf77fec731287ba07da35eb84/gym/spaces/multi_discrete.py)
 
-import numpy as np
-
 import gym
+import numpy as np
 
 
 class MultiDiscrete(gym.Space):
     """
     - The multi-discrete action space consists of a series of discrete action spaces with different parameters
     - It can be adapted to both a Discrete action space or a continuous (Box) action space
     - It is useful to represent game controllers or keyboards where each key can be represented as a discrete action space
```

### Comparing `openrl-0.0.4/openrl/envs/mpe/multiagent_env.py` & `openrl-0.0.5/openrl/envs/mpe/multiagent_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from typing import Union, Optional, Any, List, Dict, Tuple
 from dataclasses import dataclass
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import gymnasium as gym
+import numpy as np
 from gymnasium import spaces
 from gymnasium.core import ObsType
 from gymnasium.utils import seeding
 
-import numpy as np
 from .multi_discrete import MultiDiscrete
 
 # update bounds to center around agent
 cam_range = 2
 
 
 @dataclass
```

### Comparing `openrl-0.0.4/openrl/envs/mpe/rendering.py` & `openrl-0.0.5/openrl/envs/mpe/rendering.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,48 @@
 """
 2D rendering framework
 """
 from __future__ import division
+
 import os
-import six
 import sys
 
+import six
+
 if "Apple" in sys.version:
     if "DYLD_FALLBACK_LIBRARY_PATH" in os.environ:
         os.environ["DYLD_FALLBACK_LIBRARY_PATH"] += ":/usr/lib"
         # (JDS 2016/04/15): avoid bug on Anaconda 2.3.0 / Yosemite
 
 from gym import error
 
 try:
     import pyglet
-except ImportError as e:
+except ImportError:
     print(
-        "HINT: you can install pyglet directly via 'pip install pyglet'. But if you really just want to install all Gym dependencies and not have to think about it, 'pip install -e .[all]' or 'pip install gym[all]' will do it."
+        "HINT: you can install pyglet directly via 'pip install pyglet'. But if you"
+        " really just want to install all Gym dependencies and not have to think about"
+        " it, 'pip install -e .[all]' or 'pip install gym[all]' will do it."
     )
 
 try:
     from pyglet.gl import *
-except ImportError as e:
+except ImportError:
     print(
         "Error occured while running `from pyglet.gl import *`",
-        "HINT: make sure you have OpenGL install. On Ubuntu, you can run 'apt-get install python-opengl'. If you're running on a server, you may need a virtual frame buffer; something like this should work: 'xvfb-run -s \"-screen 0 1400x900x24\" python <your_script.py>'",
+        (
+            "HINT: make sure you have OpenGL install. On Ubuntu, you can run 'apt-get"
+            " install python-opengl'. If you're running on a server, you may need a"
+            " virtual frame buffer; something like this should work: 'xvfb-run -s"
+            ' "-screen 0 1400x900x24" python <your_script.py>\''
+        ),
     )
 
 import math
+
 import numpy as np
 
 RAD2DEG = 57.29577951308232
 
 
 def get_display(spec):
     """Convert a display specification (such as :0) into an actual Display
@@ -42,17 +52,16 @@
     """
     if spec is None:
         return None
     elif isinstance(spec, six.string_types):
         return pyglet.canvas.Display(spec)
     else:
         raise error.Error(
-            "Invalid display specification: {}. (Must be a string like :0 or None.)".format(
-                spec
-            )
+            "Invalid display specification: {}. (Must be a string like :0 or None.)"
+            .format(spec)
         )
 
 
 class Viewer(object):
     def __init__(self, width, height, display=None):
         display = get_display(display)
```

### Comparing `openrl-0.0.4/openrl/envs/mpe/scenarios/simple_spread.py` & `openrl-0.0.5/openrl/envs/mpe/scenarios/simple_spread.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Optional
 
 import numpy as np
-from openrl.envs.mpe.core import World, Agent, Landmark
+
+from openrl.envs.mpe.core import Agent, Landmark, World
 from openrl.envs.mpe.scenario import BaseScenario
 
 
 class Scenario(BaseScenario):
     def __init__(self):
         self.render_mode = None
```

### Comparing `openrl-0.0.4/openrl/envs/vec_env/async_venv.py` & `openrl-0.0.5/openrl/envs/vec_env/async_venv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 """An async vector environment."""
 import multiprocessing as mp
-from multiprocessing import Queue
-from multiprocessing.connection import Connection
 import sys
 import time
 from copy import deepcopy
 from enum import Enum
-from typing import Any, Callable, List, Optional, Sequence, Tuple, Union, Dict
-
-import numpy as np
-from numpy.typing import NDArray
+from multiprocessing import Queue
+from multiprocessing.connection import Connection
+from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union
 
 import gymnasium as gym
+import numpy as np
 from gymnasium import logger
-from gymnasium.core import Env, ActType, ObsType
+from gymnasium.core import ActType, Env, ObsType
 from gymnasium.error import (
     AlreadyPendingCallError,
     ClosedEnvironmentError,
     CustomSpaceError,
     NoAsyncCallError,
 )
-from gymnasium.vector.utils import (
-    CloudpickleWrapper,
-    clear_mpi_env_vars,
-)
+from gymnasium.vector.utils import CloudpickleWrapper, clear_mpi_env_vars
+from numpy.typing import NDArray
+
 from openrl.envs.vec_env.base_venv import BaseVecEnv
 from openrl.envs.vec_env.utils.numpy_utils import (
-    create_empty_array,
     concatenate,
+    create_empty_array,
     iterate_action,
 )
 from openrl.envs.vec_env.utils.share_memory import (
     create_shared_memory,
     read_from_shared_memory,
     write_to_shared_memory,
 )
@@ -51,15 +48,15 @@
     """
 
     def __init__(
         self,
         env_fns: Sequence[Callable[[], Env]],
         observation_space: Optional[gym.Space] = None,
         action_space: Optional[gym.Space] = None,
-        shared_memory: bool = True,
+        shared_memory: bool = False,  # TODO True,
         copy: bool = True,
         context: Optional[str] = None,
         daemon: bool = True,
         worker: Optional[Callable] = None,
         render_mode: Optional[str] = None,
     ):
         """Vectorized environment that runs multiple environments in parallel.
@@ -224,15 +221,18 @@
             seed = [None for _ in range(self.parallel_env_num)]
         if isinstance(seed, int):
             seed = [seed + i * 10086 for i in range(self.parallel_env_num)]
         assert len(seed) == self.parallel_env_num
 
         if self._state != AsyncState.DEFAULT:
             raise AlreadyPendingCallError(
-                f"Calling `reset_send` while waiting for a pending call to `{self._state.value}` to complete",
+                (
+                    "Calling `reset_send` while waiting for a pending call to"
+                    f" `{self._state.value}` to complete"
+                ),
                 self._state.value,
             )
 
         for pipe, single_seed in zip(self.parent_pipes, seed):
             single_kwargs = {}
             if single_seed is not None:
                 single_kwargs["seed"] = single_seed
@@ -260,15 +260,15 @@
             ClosedEnvironmentError: If the environment was closed (if :meth:`close` was previously called).
             NoAsyncCallError: If :meth:`reset_fetch` was called without any prior call to :meth:`reset_send`.
             TimeoutError: If :meth:`reset_fetch` timed out.
         """
         self._assert_is_running()
         if self._state != AsyncState.WAITING_RESET:
             raise NoAsyncCallError(
-                "Calling `reset_fetch` without any prior " "call to `reset_send`.",
+                "Calling `reset_fetch` without any prior call to `reset_send`.",
                 AsyncState.WAITING_RESET.value,
             )
 
         if not self._poll(timeout):
             self._state = AsyncState.DEFAULT
             raise mp.TimeoutError(
                 f"The call to `reset_fetch` has timed out after {timeout} second(s)."
@@ -316,15 +316,18 @@
                 method (e.g. :meth:`reset_send`). This can be caused by two consecutive
                 calls to :meth:`step_send`, with no call to :meth:`step_fetch` in
                 between.
         """
         self._assert_is_running()
         if self._state != AsyncState.DEFAULT:
             raise AlreadyPendingCallError(
-                f"Calling `step_send` while waiting for a pending call to `{self._state.value}` to complete.",
+                (
+                    "Calling `step_send` while waiting for a pending call to"
+                    f" `{self._state.value}` to complete."
+                ),
                 self._state.value,
             )
 
         actions = iterate_action(self.action_space, actions)
 
         for pipe, action in zip(self.parent_pipes, actions):
             pipe.send(("step", action))
@@ -348,15 +351,15 @@
             ClosedEnvironmentError: If the environment was closed (if :meth:`close` was previously called).
             NoAsyncCallError: If :meth:`step_fetch` was called without any prior call to :meth:`step_send`.
             TimeoutError: If :meth:`step_fetch` timed out.
         """
         self._assert_is_running()
         if self._state != AsyncState.WAITING_STEP:
             raise NoAsyncCallError(
-                "Calling `step_fetch` without any prior call " "to `step_send`.",
+                "Calling `step_fetch` without any prior call to `step_send`.",
                 AsyncState.WAITING_STEP.value,
             )
 
         if not self._poll(timeout):
             self._state = AsyncState.DEFAULT
             raise mp.TimeoutError(
                 f"The call to `step_fetch` has timed out after {timeout} second(s)."
@@ -430,15 +433,16 @@
         Raises:
             TimeoutError: If :meth:`close` timed out.
         """
         timeout = 0 if terminate else timeout
         try:
             if self._state != AsyncState.DEFAULT:
                 logger.warn(
-                    f"Calling `close` while waiting for a pending call to `{self._state.value}` to complete."
+                    "Calling `close` while waiting for a pending call to"
+                    f" `{self._state.value}` to complete."
                 )
                 function = getattr(self, f"{self._state.value}_fetch")
                 function(timeout)
         except mp.TimeoutError:
             terminate = True
 
         if terminate:
@@ -493,27 +497,29 @@
                 f"`{self.action_space}`. In order to batch actions, the "
                 "action spaces from all environments must be equal."
             )
 
     def _assert_is_running(self):
         if self.closed:
             raise ClosedEnvironmentError(
-                f"Trying to operate on `{type(self).__name__}`, after a call to `close()`."
+                f"Trying to operate on `{type(self).__name__}`, after a call to"
+                " `close()`."
             )
 
     def _raise_if_errors(self, successes):
         if all(successes):
             return
 
         num_errors = self.parallel_env_num - sum(successes)
         assert num_errors > 0
         for i in range(num_errors):
             index, exctype, value = self.error_queue.get()
             logger.error(
-                f"Received the following error from Worker-{index}: {exctype.__name__}: {value}"
+                f"Received the following error from Worker-{index}: {exctype.__name__}:"
+                f" {value}"
             )
             logger.error(f"Shutting down Worker-{index}.")
             self.parent_pipes[index].close()
             self.parent_pipes[index] = None
 
             if i == num_errors - 1:
                 logger.error("Raising the last exception back to the main process.")
@@ -554,21 +560,23 @@
         Raises:
             ClosedEnvironmentError: If the environment was closed (if :meth:`close` was previously called).
             AlreadyPendingCallError: Calling `call_send` while waiting for a pending call to complete
         """
         self._assert_is_running()
         if self._state != AsyncState.DEFAULT:
             raise AlreadyPendingCallError(
-                "Calling `call_send` while waiting "
-                f"for a pending call to `{self._state.value}` to complete.",
+                (
+                    "Calling `call_send` while waiting "
+                    f"for a pending call to `{self._state.value}` to complete."
+                ),
                 str(self._state.value),
             )
 
         for pipe in self.parent_pipes:
-            pipe.send(("_call", (name, cfg, kwargs)))
+            pipe.send(("_call", (name, args, kwargs)))
         self._state = AsyncState.WAITING_CALL
 
     def call_fetch(self, timeout: Union[int, float, None] = None) -> list:
         """Calls all parent pipes and waits for the results.
 
         Args:
             timeout: Number of seconds before the call to `step_fetch` times out.
@@ -646,16 +654,18 @@
                 "Values must be a list or tuple with length equal to the "
                 f"number of environments. Got `{len(values)}` values for "
                 f"{self.parallel_env_num} environments."
             )
 
         if self._state != AsyncState.DEFAULT:
             raise AlreadyPendingCallError(
-                "Calling `set_attr` while waiting "
-                f"for a pending call to `{self._state.value}` to complete.",
+                (
+                    "Calling `set_attr` while waiting "
+                    f"for a pending call to `{self._state.value}` to complete."
+                ),
                 str(self._state.value),
             )
 
         for pipe, value in zip(self.parent_pipes, values):
             pipe.send(("_setattr", (name, value)))
         _, successes = zip(*[pipe.recv() for pipe in self.parent_pipes])
         self._raise_if_errors(successes)
@@ -692,17 +702,18 @@
     try:
         while True:
             command, data = pipe.recv()
             if command == "reset":
                 result = env.reset(**data)
 
                 if isinstance(result, tuple):
-                    assert (
-                        len(result) == 2
-                    ), "The `reset` method of the environment must return either a single observation or a tuple of (observation, info)."
+                    assert len(result) == 2, (
+                        "The `reset` method of the environment must return either a"
+                        " single observation or a tuple of (observation, info)."
+                    )
                     observation, info = result
                     observation = prepare_obs(observation)
                     pipe.send(((observation, info), True))
                 else:
                     observation = result
                     observation = prepare_obs(observation)
                     pipe.send(((observation,), True))
@@ -757,15 +768,15 @@
                 pipe.send(
                     (
                         (data[0] == observation_space, data[1] == action_space),
                         True,
                     )
                 )
             elif command == "_call":
-                name, cfg, kwargs = data
+                name, args, kwargs = data
                 if name in ["reset", "step", "seed", "close"]:
                     raise ValueError(
                         f"Trying to call function `{name}` with "
                         f"`_call`. Use `{name}` directly instead."
                     )
                 function = getattr(env, name)
                 if callable(function):
```

### Comparing `openrl-0.0.4/openrl/envs/vec_env/base_venv.py` & `openrl-0.0.5/openrl/envs/vec_env/base_venv.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,32 +12,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 import warnings
-from typing import (
-    TYPE_CHECKING,
-    Optional,
-    Sequence,
-    Union,
-    List,
-    Any,
-    SupportsFloat,
-    TypeVar,
-)
 from abc import ABC, abstractmethod
-
-import numpy as np
+from typing import Any, List, Optional, Sequence, Union
 
 import gymnasium as gym
-from gymnasium.core import ActType, ObsType, WrapperActType, WrapperObsType
-from gymnasium import spaces
-from gymnasium.utils import seeding
+import numpy as np
 
 from openrl.envs.vec_env.utils.util import tile_images
 
 
 class BaseVecEnv(
     ABC,
 ):
```

### Comparing `openrl-0.0.4/openrl/envs/vec_env/sync_venv.py` & `openrl-0.0.5/openrl/envs/vec_env/sync_venv.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 from copy import deepcopy
-from typing import Callable, Iterable, Optional, Sequence, Union, List, Any
+from typing import Any, Callable, Iterable, List, Optional, Sequence, Union
 
 import numpy as np
+from gymnasium import Env
 from gymnasium.core import ActType
 from gymnasium.spaces import Space
-from gymnasium import Env
 
 from openrl.envs.vec_env.base_venv import BaseVecEnv
 from openrl.envs.vec_env.utils.numpy_utils import (
-    create_empty_array,
     concatenate,
+    create_empty_array,
     iterate_action,
 )
 
 
 class SyncVectorEnv(BaseVecEnv):
     """Vectorized environment that serially runs multiple environments."""
```

### Comparing `openrl-0.0.4/openrl/envs/vec_env/utils/__init__.py` & `openrl-0.0.5/openrl/envs/vec_env/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.4/openrl/envs/vec_env/utils/numpy_utils.py` & `openrl-0.0.5/openrl/envs/vec_env/utils/numpy_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # source code from https://github.com/Farama-Foundation/Gymnasium/blob/main/gymnasium/vector/utils/numpy_utils.py
 """Numpy utility functions: concatenate space samples and create empty array."""
 from collections import OrderedDict
 from functools import singledispatch
-from typing import Callable, Iterable, Union, Iterator
+from typing import Callable, Iterable, Iterator, Union
 
 import numpy as np
-
+from gymnasium.error import CustomSpaceError
 from gymnasium.spaces import (
     Box,
     Dict,
     Discrete,
     MultiBinary,
     MultiDiscrete,
     Space,
     Tuple,
 )
-from gymnasium.error import CustomSpaceError
 
 __all__ = [
     "concatenate",
     "create_empty_array",
     "iterate_action",
 ]
```

### Comparing `openrl-0.0.4/openrl/envs/vec_env/utils/share_memory.py` & `openrl-0.0.5/openrl/envs/vec_env/utils/share_memory.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 import multiprocessing as mp
 from collections import OrderedDict
 from ctypes import c_bool
 from functools import singledispatch
 from typing import Union
 
 import numpy as np
-
 from gymnasium.error import CustomSpaceError
 from gymnasium.spaces import (
     Box,
     Dict,
     Discrete,
     MultiBinary,
     MultiDiscrete,
```

### Comparing `openrl-0.0.4/openrl/envs/vec_env/utils/util.py` & `openrl-0.0.5/openrl/envs/vec_env/utils/util.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.4/openrl/envs/vec_env/wrappers/__init__.py` & `openrl-0.0.5/openrl/envs/vec_env/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.4/openrl/envs/vec_env/wrappers/base_wrapper.py` & `openrl-0.0.5/openrl/envs/vec_env/wrappers/base_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,27 +13,23 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 
 
-from typing import Optional, Sequence, Union, Any, SupportsFloat, TypeVar, Tuple, Dict
-
+from typing import Any, Dict, Optional, Sequence, SupportsFloat, Tuple, TypeVar, Union
 
 import numpy as np
-
-from gymnasium.core import ActType, ObsType, WrapperActType, WrapperObsType
 from gymnasium import spaces
+from gymnasium.core import ActType, ObsType, WrapperActType, WrapperObsType
 from gymnasium.utils import seeding
 
-
 from openrl.envs.vec_env.base_venv import BaseVecEnv
 
-
 ArrayType = TypeVar("ArrayType")
 
 
 class VecEnvWrapper(BaseVecEnv):
     """Wraps the vectorized environment to allow a modular transformation.
 
     This class is the base class for all wrappers for vectorized environments. The subclass
@@ -218,17 +214,16 @@
                 observation,
                 reward,
                 done,
                 info,
             )
         else:
             raise ValueError(
-                "Invalid step return value, expected 4 or 5 values, got {} values".format(
-                    len(results)
-                )
+                "Invalid step return value, expected 4 or 5 values, got {} values"
+                .format(len(results))
             )
 
     def observation(self, observation: ObsType) -> ObsType:
         """Defines the observation transformation.
 
         Args:
             observation (object): the observation from the environment
```

### Comparing `openrl-0.0.4/openrl/envs/vec_env/wrappers/vec_monitor.py` & `openrl-0.0.5/openrl/envs/wrappers/base_wrapper.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,77 +11,60 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
-from typing import Any, Dict
-import time
+from typing import Any, Dict, Optional
 
-import numpy as np
-from gymnasium.core import ActType
+import gymnasium as gym
 
-from openrl.envs.vec_env.base_venv import (
-    BaseVecEnv,
-)
-from openrl.envs.vec_env.wrappers.base_wrapper import VecEnvWrapper
-
-
-class VecInfo:
-    def __init__(self, parallel_env_num, agent_num):
-        self.parallel_env_num = parallel_env_num
-        self.agent_num = agent_num
-
-        self.infos = []
-        self.rewards = []
-
-        self.start_time = time.time()
-        self.total_step = 0
-
-    def statistics(self) -> Dict[str, Any]:
-        # this function should be called each episode
-        rewards = np.array(self.rewards)
-        self.total_step += np.prod(rewards.shape[:2])
-        rewards = rewards.transpose(2, 1, 0, 3)
-        info_dict = {}
-        ep_rewards = []
-        for i in range(self.agent_num):
-            agent_reward = rewards[i].mean(0).sum()
-            ep_rewards.append(agent_reward)
-            info_dict["agent_{}/episode_reward".format(i)] = agent_reward
-
-        info_dict["FPS"] = int(self.total_step / (time.time() - self.start_time))
-        info_dict["episode_reward"] = np.mean(ep_rewards)
-        return info_dict
-
-    def append(self, reward, info):
-        assert reward.shape[:2] == (self.parallel_env_num, self.agent_num)
-        self.infos.append(info)
-        self.rewards.append(reward)
-
-    def reset(self):
-        self.infos = []
-        self.rewards = []
 
-
-class VecMonitor(VecEnvWrapper):
-    def __init__(self, env: BaseVecEnv):
+class BaseWrapper(gym.Wrapper):
+    def __init__(self, env, reward_class=None) -> None:
         super().__init__(env)
-        self.vec_info = VecInfo(self.env.parallel_env_num, self.env.agent_num)
+        self.reward_class = reward_class
+
+    def step(self, action, extra_data: Optional[Dict[str, Any]] = None):
+        returns = super().step(action)
+        rewards = returns[1]
+        if self.reward_class is not None and extra_data is not None:
+            extra_data.update({"action": action})
+            extra_data.update({"reward": returns[1]})
+            extra_data.update({"returns": returns})
+            rewards = self.reward_class.get_reward(extra_data)
+
+        return returns[0], rewards, *returns[2:]
+
+    def batch_rewards(self, buffer):
+        if self.reward_class is not None:
+            self.reward_class.batch_rewards(buffer)
 
     @property
-    def use_monitor(self):
-        return True
+    def env_name(self):
+        if hasattr(self.env, "env_name"):
+            return self.env.env_name
+        return self.env.unwrapped.spec.id
 
-    def step(self, action: ActType):
-        returns = self.env.step(action)
+    @property
+    def agent_num(self):
+        if hasattr(self.env, "agent_num"):
+            return self.env.agent_num
+        else:
+            raise NotImplementedError("Not support agent_num")
 
-        self.vec_info.append(reward=returns[1], info=returns[-1])
+    @property
+    def use_monitor(self):
+        return False
+
+    @property
+    def has_auto_reset(self):
+        if hasattr(self.env, "has_auto_reset"):
+            return self.env.has_auto_reset
+        else:
+            return False
 
-        return returns
 
-    def statistics(self):
-        # this function should be called each episode
-        info_dict = self.vec_info.statistics()
-        self.vec_info.reset()
-        return info_dict
+class BaseObservationWrapper(BaseWrapper, gym.ObservationWrapper):
+    def __init__(self, env):
+        super().__init__(env)
```

### Comparing `openrl-0.0.4/openrl/envs/wrappers/extra_wrappers.py` & `openrl-0.0.5/openrl/envs/wrappers/extra_wrappers.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,23 +14,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 from copy import deepcopy
 
 import gymnasium as gym
-from gymnasium.wrappers import (
-    StepAPICompatibility,
-    AutoResetWrapper,
-)
+from gymnasium.wrappers import AutoResetWrapper, StepAPICompatibility
 
-from openrl.envs.wrappers import (
-    BaseWrapper,
-    BaseObservationWrapper,
-)
+from openrl.envs.wrappers import BaseObservationWrapper, BaseWrapper
 
 
 class RemoveTruncated(StepAPICompatibility, BaseWrapper):
     def __init__(
         self,
         env: gym.Env,
     ):
```

### Comparing `openrl-0.0.4/openrl/envs/wrappers/multiagent_wrapper.py` & `openrl-0.0.5/openrl/envs/wrappers/multiagent_wrapper.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.4/openrl/envs/wrappers/util.py` & `openrl-0.0.5/openrl/envs/wrappers/util.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 
 from typing import Any
-import numpy as np
 
+import numpy as np
 from gymnasium.spaces.box import Box
 
 
 def nest_expand_dim(input: Any) -> Any:
     if isinstance(input, (np.ndarray, float, int)):
         return np.expand_dims(input, 0)
     elif isinstance(input, list):
```

### Comparing `openrl-0.0.4/openrl/modules/__init__.py` & `openrl-0.0.5/openrl/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.4/openrl/modules/base_module.py` & `openrl-0.0.5/openrl/modules/base_module.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.4/openrl/modules/common/base_net.py` & `openrl-0.0.5/openrl/modules/common/base_net.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.4/openrl/modules/common/ppo_net.py` & `openrl-0.0.5/openrl/modules/common/ppo_net.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,33 +12,34 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 
-from typing import Union, Tuple, Dict, Optional
+from typing import Any, Dict, Optional, Tuple, Union
 
-import numpy as np
 import gym
+import numpy as np
 import torch
 
-from openrl.modules.ppo_module import PPOModule
 from openrl.configs.config import create_config_parser
 from openrl.modules.common.base_net import BaseNet
+from openrl.modules.ppo_module import PPOModule
 from openrl.utils.util import set_seed
 
 
 class PPONet(BaseNet):
     def __init__(
         self,
         env: Union[gym.Env, str],
         cfg=None,
         device: Union[torch.device, str] = "cpu",
         n_rollout_threads: int = 1,
+        model_dict: Optional[Dict[str, Any]] = None,
     ) -> None:
         super().__init__()
 
         if cfg is None:
             cfg_parser = create_config_parser()
             cfg = cfg_parser.parse_args()
 
@@ -62,18 +63,19 @@
             device = torch.device(device)
 
         self.module = PPOModule(
             cfg=cfg,
             policy_input_space=env.observation_space,
             critic_input_space=env.observation_space,
             act_space=env.action_space,
-            share_model=False,
+            share_model=cfg.use_share_model,
             device=device,
             rank=0,
             world_size=1,
+            model_dict=model_dict,
         )
 
         self.cfg = cfg
         self.env = env
         self.device = device
         self.rnn_states_actor = None
         self.masks = None
```

### Comparing `openrl-0.0.4/openrl/modules/model_config.py` & `openrl-0.0.5/openrl/modules/model_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,29 +13,30 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 
 from typing import Optional
-import torch
+
 import gym
+import torch
 
 
 class ModelConfig(dict):
     def __init__(self, *args, **kwargs) -> None:
         super(ModelConfig, self).__init__(*args, **kwargs)
 
 
 class ModelTrainConfig(ModelConfig):
     def __init__(
-            self,
-            model: torch.nn.Module,
-            input_space: gym.spaces.Box,
-            lr: Optional[float] = None,
-            *args,
-            **kwargs
+        self,
+        model: torch.nn.Module,
+        input_space: gym.spaces.Box,
+        lr: Optional[float] = None,
+        *args,
+        **kwargs
     ) -> None:
         super(ModelTrainConfig, self).__init__(*args, **kwargs)
         self["model"] = model
         self["input_space"] = input_space
         self["lr"] = lr
```

### Comparing `openrl-0.0.4/openrl/modules/networks/__init__.py` & `openrl-0.0.5/openrl/modules/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.4/openrl/modules/networks/base_policy_network.py` & `openrl-0.0.5/openrl/modules/networks/base_policy_network.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.4/openrl/modules/networks/base_value_network.py` & `openrl-0.0.5/openrl/modules/networks/base_value_network.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 from abc import ABC, abstractmethod
+
 import torch.nn as nn
 
 from openrl.modules.utils.valuenorm import ValueNorm
 
 
 class BaseValueNetwork(ABC, nn.Module):
     def __init__(self, cfg, device):
```

### Comparing `openrl-0.0.4/openrl/modules/networks/policy_network.py` & `openrl-0.0.5/openrl/modules/networks/policy_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 import torch
 import torch.nn as nn
 
-from openrl.modules.networks.utils.util import init
-from openrl.modules.networks.utils.mlp import MLPBase, MLPLayer
-from openrl.modules.networks.utils.rnn import RNNLayer
+from openrl.buffers.utils.util import get_policy_obs, get_policy_obs_space
+from openrl.modules.networks.base_policy_network import BasePolicyNetwork
 from openrl.modules.networks.utils.act import ACTLayer
-from openrl.modules.networks.utils.popart import PopArt
-from openrl.buffers.utils.util import get_policy_obs_space, get_policy_obs
-from openrl.modules.networks.utils.mix import MIXBase
 from openrl.modules.networks.utils.cnn import CNNBase
-from openrl.modules.networks.base_policy_network import BasePolicyNetwork
+from openrl.modules.networks.utils.mix import MIXBase
+from openrl.modules.networks.utils.mlp import MLPBase, MLPLayer
+from openrl.modules.networks.utils.popart import PopArt
+from openrl.modules.networks.utils.rnn import RNNLayer
+from openrl.modules.networks.utils.util import init
 from openrl.utils.util import check_v2 as check
 
 
 class PolicyNetwork(BasePolicyNetwork):
     def __init__(
         self,
         cfg,
```

### Comparing `openrl-0.0.4/openrl/modules/networks/policy_value_network.py` & `openrl-0.0.5/openrl/modules/networks/policy_value_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 # limitations under the License.
 
 """"""
 
 import torch
 import torch.nn as nn
 
+from openrl.buffers.utils.util import get_policy_obs_space
+from openrl.modules.networks.utils.act import ACTLayer
 from openrl.modules.networks.utils.cnn import CNNBase
 from openrl.modules.networks.utils.mlp import MLPBase, MLPLayer
+from openrl.modules.networks.utils.popart import PopArt
 from openrl.modules.networks.utils.rnn import RNNLayer
-from openrl.modules.networks.utils.act import ACTLayer
 from openrl.modules.networks.utils.util import init
-from openrl.modules.networks.utils.popart import PopArt
 from openrl.utils.util import check_v2 as check
-from openrl.buffers.utils.util import get_policy_obs_space, get_critic_obs_space
 
 
 class PolicyValueNetwork(nn.Module):
     def __init__(
         self,
         cfg,
         obs_space,
```

### Comparing `openrl-0.0.4/openrl/modules/networks/utils/act.py` & `openrl-0.0.5/openrl/modules/networks/utils/act.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-from .distributions import Bernoulli, Categorical, DiagGaussian
-import math
-import numpy as np
-
 import torch
 import torch.nn as nn
-import torch.nn.functional as F
+
+from .distributions import Bernoulli, Categorical, DiagGaussian
 
 
 class ACTLayer(nn.Module):
     def __init__(self, action_space, inputs_dim, use_orthogonal, gain):
         super(ACTLayer, self).__init__()
         self.multidiscrete_action = False
         self.continuous_action = False
@@ -151,15 +148,14 @@
             action_log_probs = torch.cat(action_log_probs, -1)  # ! could be wrong
             dist_entropy = torch.tensor(dist_entropy).mean()
 
         elif self.continuous_action:
             action_logits = self.action_out(x)
             action_log_probs = action_logits.log_probs(action)
             act_entropy = action_logits.entropy()
-            # import pdb;pdb.set_trace()
             if active_masks is not None:
                 dist_entropy = (act_entropy * active_masks).sum() / active_masks.sum()
             else:
                 dist_entropy = act_entropy.mean()
 
         else:
             action_logits = self.action_out(x, available_actions)
```

### Comparing `openrl-0.0.4/openrl/modules/networks/utils/attention.py` & `openrl-0.0.5/openrl/modules/networks/utils/attention.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import math
-import numpy as np
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
-from .util import init, get_clones
+from .util import get_clones, init
 
 
 class Encoder(nn.Module):
     def __init__(self, cfg, split_shape, cat_self=True):
         super(Encoder, self).__init__()
         self._use_orthogonal = cfg.use_orthogonal
         self._activation_id = cfg.activation_id
@@ -231,17 +230,17 @@
 
         x1 = []
         self_x = x[self_idx]
         for i in range(N - 1):
             K = self.split_shape[i][0]
             L = self.split_shape[i][1]
             for j in range(K):
-                temp = torch.cat((x[i][:, (L * j) : (L * j + L)], self_x), dim=-1)
+                torch.cat((x[i][:, (L * j) : (L * j + L)], self_x), dim=-1)
                 exec("x1.append(self.fc_{}(temp))".format(i))
-        temp = x[self_idx]
+        x[self_idx]
         exec("x1.append(self.fc_{}(temp))".format(N - 1))
 
         out = torch.stack(x1, 1)
 
         return out, self_x
 
 
@@ -275,15 +274,15 @@
         N = len(x)
 
         x1 = []
         for i in range(N):
             K = self.split_shape[i][0]
             L = self.split_shape[i][1]
             for j in range(K):
-                temp = x[i][:, (L * j) : (L * j + L)]
+                x[i][:, (L * j) : (L * j + L)]
                 exec("x1.append(self.fc_{}(temp))".format(i))
 
         out = torch.stack(x1, 1)
 
         if self_idx is None:
             return out, None
         else:
```

### Comparing `openrl-0.0.4/openrl/modules/networks/utils/cnn.py` & `openrl-0.0.5/openrl/modules/networks/utils/cnn.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-import numpy as np
-
-import torch
 import torch.nn as nn
-import torch.nn.functional as F
 
 from .util import init
 
 
 class Flatten(nn.Module):
     def forward(self, x):
         return x.view(x.size(0), -1)
@@ -20,26 +16,26 @@
         use_orthogonal,
         activation_id,
         kernel_size=3,
         stride=1,
     ):
         super(CNNLayer, self).__init__()
 
-        active_func = [nn.Tanh(), nn.ReLU(), nn.LeakyReLU(), nn.ELU()][activation_id]
+        [nn.Tanh(), nn.ReLU(), nn.LeakyReLU(), nn.ELU()][activation_id]
         init_method = [nn.init.xavier_uniform_, nn.init.orthogonal_][use_orthogonal]
         gain = nn.init.calculate_gain(
             ["tanh", "relu", "leaky_relu", "leaky_relu"][activation_id]
         )
 
         def init_(m):
             return init(m, init_method, lambda x: nn.init.constant_(x, 0), gain=gain)
 
         input_channel = obs_shape[0]
-        input_width = obs_shape[1]
-        input_height = obs_shape[2]
+        obs_shape[1]
+        obs_shape[2]
 
         # self.cnn = nn.Sequential(
         #     init_(nn.Conv2d(in_channels=input_channel, out_channels=hidden_size//2, kernel_size=kernel_size, stride=stride)), active_func,
         #     Flatten(),
         #     init_(nn.Linear(hidden_size//2 * (input_width-kernel_size+stride) * (input_height-kernel_size+stride), hidden_size)), active_func,
         #     init_(nn.Linear(hidden_size, hidden_size)), active_func)
         # only for atari
```

### Comparing `openrl-0.0.4/openrl/modules/networks/utils/distributed_utils.py` & `openrl-0.0.5/openrl/modules/networks/utils/distributed_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,12 +14,13 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 
 from torch import distributed as dist
 
+
 def reduce_tensor(tensor, n):
     rt = tensor.clone()
     dist.all_reduce(rt, op=dist.ReduceOp.SUM)
     rt /= n
-    return rt
+    return rt
```

### Comparing `openrl-0.0.4/openrl/modules/networks/utils/distributions.py` & `openrl-0.0.5/openrl/modules/networks/utils/distributions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-import math
-
 import torch
 import torch.nn as nn
-import torch.nn.functional as F
 
 from .util import init
 
 """
 Modify standard PyTorch distributions so they are compatible with this code.
 """
 
 #
 # Standardize distribution interfaces
 #
 
+
 # Categorical
 class FixedCategorical(torch.distributions.Categorical):
     def sample(self):
         return super().sample().unsqueeze(-1)
 
     def log_probs(self, actions):
         return (
@@ -27,14 +25,15 @@
             .sum(-1)
             .unsqueeze(-1)
         )
 
     def mode(self):
         return self.probs.argmax(dim=-1, keepdim=True)
 
+
 # Normal
 class FixedNormal(torch.distributions.Normal):
     def log_probs(self, actions):
         # return super().log_prob(actions).sum(-1, keepdim=True)
         return super().log_prob(actions)
 
     def entropy(self):
@@ -56,15 +55,16 @@
         return torch.gt(self.probs, 0.5).float()
 
 
 class Categorical(nn.Module):
     def __init__(self, num_inputs, num_outputs, use_orthogonal=True, gain=0.01):
         super(Categorical, self).__init__()
         init_method = [nn.init.xavier_uniform_, nn.init.orthogonal_][use_orthogonal]
-        def init_(m): 
+
+        def init_(m):
             return init(m, init_method, lambda x: nn.init.constant_(x, 0), gain)
 
         self.linear = init_(nn.Linear(num_inputs, num_outputs))
 
     def forward(self, x, available_actions=None):
         x = self.linear(x)
         if available_actions is not None:
@@ -73,15 +73,16 @@
 
 
 class DiagGaussian(nn.Module):
     def __init__(self, num_inputs, num_outputs, use_orthogonal=True, gain=0.01):
         super(DiagGaussian, self).__init__()
 
         init_method = [nn.init.xavier_uniform_, nn.init.orthogonal_][use_orthogonal]
-        def init_(m): 
+
+        def init_(m):
             return init(m, init_method, lambda x: nn.init.constant_(x, 0), gain)
 
         self.fc_mean = init_(nn.Linear(num_inputs, num_outputs))
         self.logstd = AddBias(torch.zeros(num_outputs))
 
     def forward(self, x):
         action_mean = self.fc_mean(x)
@@ -97,23 +98,25 @@
         return FixedNormal(action_mean, action_logstd.exp())
 
 
 class Bernoulli(nn.Module):
     def __init__(self, num_inputs, num_outputs, use_orthogonal=True, gain=0.01):
         super(Bernoulli, self).__init__()
         init_method = [nn.init.xavier_uniform_, nn.init.orthogonal_][use_orthogonal]
-        def init_(m): 
+
+        def init_(m):
             return init(m, init_method, lambda x: nn.init.constant_(x, 0), gain)
-        
+
         self.linear = init_(nn.Linear(num_inputs, num_outputs))
 
     def forward(self, x):
         x = self.linear(x)
         return FixedBernoulli(logits=x)
 
+
 class AddBias(nn.Module):
     def __init__(self, bias):
         super(AddBias, self).__init__()
         self._bias = nn.Parameter(bias.unsqueeze(1))
 
     def forward(self, x):
         if x.dim() == 2:
```

### Comparing `openrl-0.0.4/openrl/modules/networks/utils/mix.py` & `openrl-0.0.5/openrl/modules/networks/utils/mix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-
 import torch
 import torch.nn as nn
 
 from .util import init
 
 
 class Flatten(nn.Module):
```

### Comparing `openrl-0.0.4/openrl/modules/networks/utils/mlp.py` & `openrl-0.0.5/openrl/modules/networks/utils/mlp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-import numpy as np
-
 import torch
 import torch.nn as nn
-import torch.nn.functional as F
 
-from .util import init, get_clones
 from .attention import Encoder
+from .util import get_clones, init
 
 
 class MLPLayer(nn.Module):
     def __init__(self, input_dim, hidden_size, layer_N, use_orthogonal, activation_id):
         super(MLPLayer, self).__init__()
         self._layer_N = layer_N
```

### Comparing `openrl-0.0.4/openrl/modules/networks/utils/popart.py` & `openrl-0.0.5/openrl/modules/networks/utils/popart.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,52 @@
 import math
+
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
+
 class PopArt(torch.nn.Module):
-    
-    def __init__(self, input_shape, output_shape, norm_axes=1, beta=0.99999, epsilon=1e-5, device=torch.device("cpu")):
-        
+    def __init__(
+        self,
+        input_shape,
+        output_shape,
+        norm_axes=1,
+        beta=0.99999,
+        epsilon=1e-5,
+        device=torch.device("cpu"),
+    ):
         super(PopArt, self).__init__()
 
         self.beta = beta
         self.epsilon = epsilon
         self.norm_axes = norm_axes
         self.tpdv = dict(dtype=torch.float32, device=device)
 
         self.input_shape = input_shape
         self.output_shape = output_shape
 
-        self.weight = nn.Parameter(torch.Tensor(output_shape, input_shape)).to(**self.tpdv)
+        self.weight = nn.Parameter(torch.Tensor(output_shape, input_shape)).to(
+            **self.tpdv
+        )
         self.bias = nn.Parameter(torch.Tensor(output_shape)).to(**self.tpdv)
-        
-        self.stddev = nn.Parameter(torch.ones(output_shape), requires_grad=False).to(**self.tpdv)
-        self.mean = nn.Parameter(torch.zeros(output_shape), requires_grad=False).to(**self.tpdv)
-        self.mean_sq = nn.Parameter(torch.zeros(output_shape), requires_grad=False).to(**self.tpdv)
-        self.debiasing_term = nn.Parameter(torch.tensor(0.0), requires_grad=False).to(**self.tpdv)
+
+        self.stddev = nn.Parameter(torch.ones(output_shape), requires_grad=False).to(
+            **self.tpdv
+        )
+        self.mean = nn.Parameter(torch.zeros(output_shape), requires_grad=False).to(
+            **self.tpdv
+        )
+        self.mean_sq = nn.Parameter(torch.zeros(output_shape), requires_grad=False).to(
+            **self.tpdv
+        )
+        self.debiasing_term = nn.Parameter(torch.tensor(0.0), requires_grad=False).to(
+            **self.tpdv
+        )
 
         self.reset_parameters()
 
     def reset_parameters(self):
         torch.nn.init.kaiming_uniform_(self.weight, a=math.sqrt(5))
         if self.bias is not None:
             fan_in, _ = torch.nn.init._calculate_fan_in_and_fan_out(self.weight)
@@ -40,55 +58,60 @@
 
     def forward(self, input_vector):
         if type(input_vector) == np.ndarray:
             input_vector = torch.from_numpy(input_vector)
         input_vector = input_vector.to(**self.tpdv)
 
         return F.linear(input_vector, self.weight, self.bias)
-    
+
     @torch.no_grad()
     def update(self, input_vector):
         if type(input_vector) == np.ndarray:
             input_vector = torch.from_numpy(input_vector)
         input_vector = input_vector.to(**self.tpdv)
-        
+
         old_mean, old_stddev = self.mean, self.stddev
 
         batch_mean = input_vector.mean(dim=tuple(range(self.norm_axes)))
-        batch_sq_mean = (input_vector ** 2).mean(dim=tuple(range(self.norm_axes)))
+        batch_sq_mean = (input_vector**2).mean(dim=tuple(range(self.norm_axes)))
 
         self.mean.mul_(self.beta).add_(batch_mean * (1.0 - self.beta))
         self.mean_sq.mul_(self.beta).add_(batch_sq_mean * (1.0 - self.beta))
         self.debiasing_term.mul_(self.beta).add_(1.0 * (1.0 - self.beta))
 
-        self.stddev = (self.mean_sq - self.mean ** 2).sqrt().clamp(min=1e-4)
+        self.stddev = (self.mean_sq - self.mean**2).sqrt().clamp(min=1e-4)
 
         self.weight = self.weight * old_stddev / self.stddev
         self.bias = (old_stddev * self.bias + old_mean - self.mean) / self.stddev
 
     def debiased_mean_var(self):
         debiased_mean = self.mean / self.debiasing_term.clamp(min=self.epsilon)
         debiased_mean_sq = self.mean_sq / self.debiasing_term.clamp(min=self.epsilon)
-        debiased_var = (debiased_mean_sq - debiased_mean ** 2).clamp(min=1e-2)
+        debiased_var = (debiased_mean_sq - debiased_mean**2).clamp(min=1e-2)
         return debiased_mean, debiased_var
 
     def normalize(self, input_vector):
         if type(input_vector) == np.ndarray:
             input_vector = torch.from_numpy(input_vector)
         input_vector = input_vector.to(**self.tpdv)
 
         mean, var = self.debiased_mean_var()
-        out = (input_vector - mean[(None,) * self.norm_axes]) / torch.sqrt(var)[(None,) * self.norm_axes]
-        
+        out = (input_vector - mean[(None,) * self.norm_axes]) / torch.sqrt(var)[
+            (None,) * self.norm_axes
+        ]
+
         return out
 
     def denormalize(self, input_vector):
         if type(input_vector) == np.ndarray:
             input_vector = torch.from_numpy(input_vector)
         input_vector = input_vector.to(**self.tpdv)
 
         mean, var = self.debiased_mean_var()
-        out = input_vector * torch.sqrt(var)[(None,) * self.norm_axes] + mean[(None,) * self.norm_axes]
-        
+        out = (
+            input_vector * torch.sqrt(var)[(None,) * self.norm_axes]
+            + mean[(None,) * self.norm_axes]
+        )
+
         out = out.cpu().numpy()
 
         return out
```

### Comparing `openrl-0.0.4/openrl/modules/networks/utils/rnn.py` & `openrl-0.0.5/openrl/modules/networks/utils/rnn.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,54 @@
-
-import numpy as np
-
 import torch
 import torch.nn as nn
-import torch.nn.functional as F
+
 
 class RNNLayer(nn.Module):
-    def __init__(self, inputs_dim, outputs_dim, recurrent_N, use_orthogonal,rnn_type='gru'):
+    def __init__(
+        self, inputs_dim, outputs_dim, recurrent_N, use_orthogonal, rnn_type="gru"
+    ):
         super(RNNLayer, self).__init__()
         self._recurrent_N = recurrent_N
         self._use_orthogonal = use_orthogonal
         self.rnn_type = rnn_type
-        if rnn_type == 'gru':
+        if rnn_type == "gru":
             self.rnn = nn.GRU(inputs_dim, outputs_dim, num_layers=self._recurrent_N)
-        elif rnn_type == 'lstm':
+        elif rnn_type == "lstm":
             self.rnn = nn.LSTM(inputs_dim, outputs_dim, num_layers=self._recurrent_N)
         else:
-            raise NotImplementedError(f'RNN type {rnn_type} has not been implemented.')
+            raise NotImplementedError(f"RNN type {rnn_type} has not been implemented.")
 
         for name, param in self.rnn.named_parameters():
-            if 'bias' in name:
+            if "bias" in name:
                 nn.init.constant_(param, 0)
-            elif 'weight' in name:
+            elif "weight" in name:
                 if self._use_orthogonal:
                     nn.init.orthogonal_(param)
                 else:
                     nn.init.xavier_uniform_(param)
         self.norm = nn.LayerNorm(outputs_dim)
 
     def rnn_forward(self, x, h):
-        if self.rnn_type == 'lstm':
+        if self.rnn_type == "lstm":
             h = torch.split(h, h.shape[-1] // 2, dim=-1)
             h = (h[0].contiguous(), h[1].contiguous())
         x_, h_ = self.rnn(x, h)
-        if self.rnn_type == 'lstm':
+        if self.rnn_type == "lstm":
             h_ = torch.cat(h_, -1)
         return x_, h_
 
     def forward(self, x, hxs, masks):
         if x.size(0) == hxs.size(0):
-            x, hxs = self.rnn_forward(x.unsqueeze(0), (hxs * masks.repeat(1, self._recurrent_N).unsqueeze(-1)).transpose(0, 1).contiguous())
-            #x= self.gru(x.unsqueeze(0))
+            x, hxs = self.rnn_forward(
+                x.unsqueeze(0),
+                (hxs * masks.repeat(1, self._recurrent_N).unsqueeze(-1))
+                .transpose(0, 1)
+                .contiguous(),
+            )
+            # x= self.gru(x.unsqueeze(0))
             x = x.squeeze(0)
             hxs = hxs.transpose(0, 1)
         else:
             # x is a (T, N, -1) tensor that has been flatten to (T * N, -1)
             N = hxs.size(0)
             T = int(x.size(0) / N)
 
@@ -52,19 +56,15 @@
             x = x.view(T, N, x.size(1))
 
             # Same deal with masks
             masks = masks.view(T, N)
 
             # Let's figure out which steps in the sequence have a zero for any agent
             # We will always assume t=0 has a zero in it as that makes the logic cleaner
-            has_zeros = ((masks[1:] == 0.0)
-                         .any(dim=-1)
-                         .nonzero()
-                         .squeeze()
-                         .cpu())
+            has_zeros = (masks[1:] == 0.0).any(dim=-1).nonzero().squeeze().cpu()
 
             # +1 to correct the masks[1:]
             if has_zeros.dim() == 0:
                 # Deal with scalar
                 has_zeros = [has_zeros.item() + 1]
             else:
                 has_zeros = (has_zeros + 1).numpy().tolist()
@@ -75,16 +75,19 @@
             hxs = hxs.transpose(0, 1)
 
             outputs = []
             for i in range(len(has_zeros) - 1):
                 # We can now process steps that don't have any zeros in masks together!
                 # This is much faster
                 start_idx = has_zeros[i]
-                end_idx = has_zeros[i + 1]               
-                temp = (hxs * masks[start_idx].view(1, -1, 1).repeat(self._recurrent_N, 1, 1)).contiguous()
+                end_idx = has_zeros[i + 1]
+                temp = (
+                    hxs
+                    * masks[start_idx].view(1, -1, 1).repeat(self._recurrent_N, 1, 1)
+                ).contiguous()
                 rnn_scores, hxs = self.rnn_forward(x[start_idx:end_idx], temp)
                 outputs.append(rnn_scores)
 
             # assert len(outputs) == T
             # x is a (T, N, -1) tensor
             x = torch.cat(outputs, dim=0)
```

### Comparing `openrl-0.0.4/openrl/modules/networks/utils/transformer_act.py` & `openrl-0.0.5/openrl/modules/networks/utils/transformer_act.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 import torch
 from torch.distributions import Categorical, Normal
 from torch.nn import functional as F
 
 
-def discrete_autoregreesive_act(decoder, obs_rep, obs, batch_size, n_agent, action_dim, tpdv,
-                                available_actions=None, deterministic=False):
+def discrete_autoregreesive_act(
+    decoder,
+    obs_rep,
+    obs,
+    batch_size,
+    n_agent,
+    action_dim,
+    tpdv,
+    available_actions=None,
+    deterministic=False,
+):
     shifted_action = torch.zeros((batch_size, n_agent, action_dim + 1)).to(**tpdv)
     shifted_action[:, 0, 0] = 1
     output_action = torch.zeros((batch_size, n_agent, 1), dtype=torch.long)
     output_action_log = torch.zeros_like(output_action, dtype=torch.float32)
 
     for i in range(n_agent):
         logit = decoder(shifted_action, obs_rep, obs)[:, i, :]
@@ -22,32 +31,44 @@
         output_action[:, i, :] = action.unsqueeze(-1)
         output_action_log[:, i, :] = action_log.unsqueeze(-1)
         if i + 1 < n_agent:
             shifted_action[:, i + 1, 1:] = F.one_hot(action, num_classes=action_dim)
     return output_action, output_action_log
 
 
-def discrete_parallel_act(decoder, obs_rep, obs, action, batch_size, n_agent, action_dim, tpdv,
-                          available_actions=None):
-    one_hot_action = F.one_hot(action.squeeze(-1), num_classes=action_dim)  # (batch, n_agent, action_dim)
+def discrete_parallel_act(
+    decoder,
+    obs_rep,
+    obs,
+    action,
+    batch_size,
+    n_agent,
+    action_dim,
+    tpdv,
+    available_actions=None,
+):
+    one_hot_action = F.one_hot(
+        action.squeeze(-1), num_classes=action_dim
+    )  # (batch, n_agent, action_dim)
     shifted_action = torch.zeros((batch_size, n_agent, action_dim + 1)).to(**tpdv)
     shifted_action[:, 0, 0] = 1
     shifted_action[:, 1:, 1:] = one_hot_action[:, :-1, :]
     logit = decoder(shifted_action, obs_rep, obs)
     if available_actions is not None:
         logit[available_actions == 0] = -1e10
 
     distri = Categorical(logits=logit)
     action_log = distri.log_prob(action.squeeze(-1)).unsqueeze(-1)
     entropy = distri.entropy().unsqueeze(-1)
     return action_log, entropy
 
 
-def continuous_autoregreesive_act(decoder, obs_rep, obs, batch_size, n_agent, action_dim, tpdv,
-                                  deterministic=False):
+def continuous_autoregreesive_act(
+    decoder, obs_rep, obs, batch_size, n_agent, action_dim, tpdv, deterministic=False
+):
     shifted_action = torch.zeros((batch_size, n_agent, action_dim)).to(**tpdv)
     output_action = torch.zeros((batch_size, n_agent, action_dim), dtype=torch.float32)
     output_action_log = torch.zeros_like(output_action, dtype=torch.float32)
 
     for i in range(n_agent):
         act_mean = decoder(shifted_action, obs_rep, obs)[:, i, :]
         action_std = torch.sigmoid(decoder.log_std) * 0.5
@@ -60,15 +81,17 @@
         output_action_log[:, i, :] = action_log
         if i + 1 < n_agent:
             shifted_action[:, i + 1, :] = action
 
     return output_action, output_action_log
 
 
-def continuous_parallel_act(decoder, obs_rep, obs, action, batch_size, n_agent, action_dim, tpdv):
+def continuous_parallel_act(
+    decoder, obs_rep, obs, action, batch_size, n_agent, action_dim, tpdv
+):
     shifted_action = torch.zeros((batch_size, n_agent, action_dim)).to(**tpdv)
     shifted_action[:, 1:, :] = action[:, :-1, :]
 
     act_mean = decoder(shifted_action, obs_rep, obs)
     action_std = torch.sigmoid(decoder.log_std) * 0.5
     distri = Normal(act_mean, action_std)
```

### Comparing `openrl-0.0.4/openrl/modules/networks/value_network.py` & `openrl-0.0.5/openrl/modules/networks/value_network.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 # limitations under the License.
 
 """"""
 
 import torch
 import torch.nn as nn
 
-from openrl.modules.networks.utils.util import init
+from openrl.buffers.utils.util import get_critic_obs_space
+from openrl.modules.networks.base_value_network import BaseValueNetwork
+from openrl.modules.networks.utils.cnn import CNNBase
+from openrl.modules.networks.utils.mix import MIXBase
 from openrl.modules.networks.utils.mlp import MLPBase, MLPLayer
-from openrl.modules.networks.utils.rnn import RNNLayer
 from openrl.modules.networks.utils.popart import PopArt
-from openrl.modules.networks.utils.mix import MIXBase
-from openrl.modules.networks.utils.cnn import CNNBase
-from openrl.modules.networks.base_value_network import BaseValueNetwork
-from openrl.buffers.utils.util import get_critic_obs_space
+from openrl.modules.networks.utils.rnn import RNNLayer
+from openrl.modules.networks.utils.util import init
 from openrl.utils.util import check_v2 as check
 
 
 class ValueNetwork(BaseValueNetwork):
     def __init__(
         self,
         cfg,
```

### Comparing `openrl-0.0.4/openrl/modules/ppo_module.py` & `openrl-0.0.5/openrl/modules/ppo_module.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,57 +12,69 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 
-from typing import Optional, Union
+from typing import Any, Dict, Optional, Union
 
-import numpy as np
 import gym
+import numpy as np
 import torch
 
-from openrl.modules.rl_module import RLModule
 from openrl.modules.model_config import ModelTrainConfig
-
-from openrl.modules.networks.policy_value_network import PolicyValueNetwork
 from openrl.modules.networks.policy_network import PolicyNetwork
+from openrl.modules.networks.policy_value_network import PolicyValueNetwork
 from openrl.modules.networks.value_network import ValueNetwork
+from openrl.modules.rl_module import RLModule
 from openrl.modules.utils.util import update_linear_schedule
 
 
 class PPOModule(RLModule):
     def __init__(
         self,
         cfg,
         policy_input_space: gym.spaces.Box,
         critic_input_space: gym.spaces.Box,
         act_space: gym.spaces.Box,
         share_model: bool = False,
         device: Union[str, torch.device] = "cpu",
         rank: Optional[int] = None,
         world_size: Optional[int] = None,
+        model_dict: Optional[Dict[str, Any]] = None,
     ):
         model_configs = {}
         if share_model:
             model_configs["model"] = ModelTrainConfig(
                 lr=cfg.lr,
-                model=PolicyValueNetwork,
+                model=(
+                    model_dict["model"]
+                    if model_dict and "model" in model_dict
+                    else PolicyValueNetwork
+                ),
                 input_space=policy_input_space,
             )
         else:
             model_configs["policy"] = ModelTrainConfig(
                 lr=cfg.lr,
-                model=PolicyNetwork,
+                model=(
+                    model_dict["policy"]
+                    if model_dict and "policy" in model_dict
+                    else PolicyNetwork
+                ),
                 input_space=policy_input_space,
             )
             model_configs["critic"] = ModelTrainConfig(
                 lr=cfg.critic_lr,
-                model=ValueNetwork,
+                model=(
+                    model_dict["critic"]
+                    if model_dict and "critic" in model_dict
+                    else ValueNetwork
+                ),
                 input_space=critic_input_space,
             )
 
         super(PPOModule, self).__init__(
             cfg=cfg,
             model_configs=model_configs,
             act_space=act_space,
@@ -89,15 +101,26 @@
         rnn_states_actor,
         rnn_states_critic,
         masks,
         available_actions=None,
         deterministic=False,
     ):
         if self.share_model:
-            raise NotImplementedError
+            actions, action_log_probs, rnn_states_actor = self.models["model"](
+                "original",
+                obs,
+                rnn_states_actor,
+                masks,
+                available_actions,
+                deterministic,
+            )
+
+            values, rnn_states_critic = self.models["model"](
+                "get_values", critic_obs, rnn_states_critic, masks
+            )
         else:
             actions, action_log_probs, rnn_states_actor = self.models["policy"](
                 "original",
                 obs,
                 rnn_states_actor,
                 masks,
                 available_actions,
@@ -108,15 +131,17 @@
                 critic_obs, rnn_states_critic, masks
             )
 
         return values, actions, action_log_probs, rnn_states_actor, rnn_states_critic
 
     def get_values(self, critic_obs, rnn_states_critic, masks):
         if self.share_model:
-            raise NotImplementedError
+            values, _ = self.models["model"](
+                "get_values", critic_obs, rnn_states_critic, masks
+            )
         else:
             values, _ = self.models["critic"](critic_obs, rnn_states_critic, masks)
         return values
 
     def evaluate_actions(
         self,
         critic_obs,
@@ -129,15 +154,27 @@
         active_masks=None,
         critic_masks_batch=None,
     ):
         if critic_masks_batch is None:
             critic_masks_batch = masks
 
         if self.share_model:
-            raise NotImplementedError
+            values, _ = self.models["model"](
+                "get_values", critic_obs, rnn_states_critic, critic_masks_batch
+            )
+
+            action_log_probs, dist_entropy, policy_values = self.models["model"](
+                "eval_actions",
+                obs,
+                rnn_states_actor,
+                action,
+                masks,
+                available_actions,
+                active_masks,
+            )
         else:
             values, _ = self.models["critic"](
                 critic_obs, rnn_states_critic, critic_masks_batch
             )
 
             action_log_probs, dist_entropy, policy_values = self.models["policy"](
                 "eval_actions",
@@ -151,29 +188,32 @@
 
         return values, action_log_probs, dist_entropy, policy_values
 
     def act(
         self, obs, rnn_states_actor, masks, available_actions=None, deterministic=False
     ):
         if self.share_model:
-            raise NotImplementedError
+            model = self.models["model"]
         else:
-            actions, _, rnn_states_actor = self.models["policy"](
-                "original",
-                obs,
-                rnn_states_actor,
-                masks,
-                available_actions,
-                deterministic,
-            )
+            model = self.models["policy"]
+
+        actions, _, rnn_states_actor = model(
+            "original",
+            obs,
+            rnn_states_actor,
+            masks,
+            available_actions,
+            deterministic,
+        )
+
         return actions, rnn_states_actor
 
     def get_critic_value_normalizer(self):
         if self.share_model:
-            raise NotImplementedError
+            return self.models["model"].value_normalizer
         else:
             return self.models["critic"].value_normalizer
 
     @staticmethod
     def init_rnn_states(
         rollout_num: int, agent_num: int, rnn_layers: int, hidden_size: int
     ):
```

### Comparing `openrl-0.0.4/openrl/modules/rl_module.py` & `openrl-0.0.5/openrl/modules/rl_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 from abc import abstractmethod
+from pathlib import Path
 from typing import Dict, Union
 
 import torch
 from gym import spaces
-from pathlib import Path
 
 from openrl.modules.base_module import BaseModule
 from openrl.modules.model_config import ModelTrainConfig
 
 
 class RLModule(BaseModule):
     def __init__(
@@ -161,8 +161,9 @@
                     del state_dict
             else:
                 print("can't find optimizer to restore")
         # TODO
         # optimizer.load_state_dict(resume_state['optimizer'])
 
     def save(self, save_dir: str) -> None:
+        print("\n\n\nenter here")
         pass
```

### Comparing `openrl-0.0.4/openrl/modules/utils/__init__.py` & `openrl-0.0.5/openrl/modules/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.4/openrl/modules/utils/util.py` & `openrl-0.0.5/openrl/modules/utils/util.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import math
 
+
 def get_gard_norm(it):
     sum_grad = 0
     for x in it:
         if x.grad is None:
             continue
         sum_grad += x.grad.norm() ** 2
     return math.sqrt(sum_grad)
 
 
 def update_linear_schedule(optimizer, epoch, total_num_epochs, initial_lr):
     """Decreases the learning rate linearly"""
     lr = initial_lr - (initial_lr * (epoch / float(total_num_epochs)))
     for param_group in optimizer.param_groups:
-        param_group['lr'] = lr
+        param_group["lr"] = lr
 
 
 def huber_loss(e, d):
     a = (abs(e) <= d).float()
     b = (e > d).float()
-    return a*e**2/2 + b*d*(abs(e)-d/2)
+    return a * e**2 / 2 + b * d * (abs(e) - d / 2)
 
 
 def mse_loss(e):
-    return e**2/2
+    return e**2 / 2
```

### Comparing `openrl-0.0.4/openrl/modules/utils/valuenorm.py` & `openrl-0.0.5/openrl/modules/utils/valuenorm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,85 +1,100 @@
-
 import numpy as np
-
 import torch
 import torch.nn as nn
 
 
 class ValueNorm(nn.Module):
-    """ Normalize a vector of observations - across the first norm_axes dimensions"""
+    """Normalize a vector of observations - across the first norm_axes dimensions"""
 
-    def __init__(self, input_shape, norm_axes=1, beta=0.99999, per_element_update=False, epsilon=1e-5, device=torch.device("cpu")):
+    def __init__(
+        self,
+        input_shape,
+        norm_axes=1,
+        beta=0.99999,
+        per_element_update=False,
+        epsilon=1e-5,
+        device=torch.device("cpu"),
+    ):
         super(ValueNorm, self).__init__()
 
         self.input_shape = input_shape
         self.norm_axes = norm_axes
         self.epsilon = epsilon
         self.beta = beta
         self.per_element_update = per_element_update
         self.tpdv = dict(dtype=torch.float32, device=device)
 
         # self.running_mean = nn.Parameter(torch.zeros(input_shape), requires_grad=False).to(**self.tpdv)
         # self.running_mean_sq = nn.Parameter(torch.zeros(input_shape), requires_grad=False).to(**self.tpdv)
         # self.debiasing_term = nn.Parameter(torch.tensor(0.0), requires_grad=False).to(**self.tpdv)
 
         self.running_mean = nn.Parameter(torch.zeros(input_shape), requires_grad=False)
-        self.running_mean_sq = nn.Parameter(torch.zeros(input_shape), requires_grad=False)
+        self.running_mean_sq = nn.Parameter(
+            torch.zeros(input_shape), requires_grad=False
+        )
         self.debiasing_term = nn.Parameter(torch.tensor(0.0), requires_grad=False)
-        
-        self.reset_parameters()
-
 
+        self.reset_parameters()
 
     def reset_parameters(self):
         self.running_mean.zero_()
         self.running_mean_sq.zero_()
         self.debiasing_term.zero_()
 
     def running_mean_var(self):
         debiased_mean = self.running_mean / self.debiasing_term.clamp(min=self.epsilon)
-        debiased_mean_sq = self.running_mean_sq / self.debiasing_term.clamp(min=self.epsilon)
-        debiased_var = (debiased_mean_sq - debiased_mean ** 2).clamp(min=1e-2)
-        return debiased_mean, debiased_var
+        debiased_mean_sq = self.running_mean_sq / self.debiasing_term.clamp(
+            min=self.epsilon
+        )
+        debiased_var = (debiased_mean_sq - debiased_mean**2).clamp(min=1e-2)
+        return debiased_mean.to(**self.tpdv), debiased_var.to(**self.tpdv)  # TODO
 
     @torch.no_grad()
     def update(self, input_vector):
         if type(input_vector) == np.ndarray:
             input_vector = torch.from_numpy(input_vector)
         input_vector = input_vector.to(**self.tpdv)
 
         batch_mean = input_vector.mean(dim=tuple(range(self.norm_axes)))
-        batch_sq_mean = (input_vector ** 2).mean(dim=tuple(range(self.norm_axes)))
+        batch_sq_mean = (input_vector**2).mean(dim=tuple(range(self.norm_axes)))
 
         if self.per_element_update:
-            batch_size = np.prod(input_vector.size()[:self.norm_axes])
-            weight = self.beta ** batch_size
+            batch_size = np.prod(input_vector.size()[: self.norm_axes])
+            weight = self.beta**batch_size
         else:
             weight = self.beta
 
+        batch_mean = batch_mean.to(**self.tpdv)  # TODO
+
         self.running_mean.mul_(weight).add_(batch_mean * (1.0 - weight))
         self.running_mean_sq.mul_(weight).add_(batch_sq_mean * (1.0 - weight))
         self.debiasing_term.mul_(weight).add_(1.0 * (1.0 - weight))
 
     def normalize(self, input_vector):
         # Make sure input is float32
         if type(input_vector) == np.ndarray:
             input_vector = torch.from_numpy(input_vector)
         input_vector = input_vector.to(**self.tpdv)
 
         mean, var = self.running_mean_var()
-        out = (input_vector - mean[(None,) * self.norm_axes]) / torch.sqrt(var)[(None,) * self.norm_axes]
-        
+        out = (input_vector - mean[(None,) * self.norm_axes]) / torch.sqrt(var)[
+            (None,) * self.norm_axes
+        ]
+
         return out
 
     def denormalize(self, input_vector):
-        """ Transform normalized data back into original distribution """
+        """Transform normalized data back into original distribution"""
         if type(input_vector) == np.ndarray:
             input_vector = torch.from_numpy(input_vector)
         input_vector = input_vector.to(**self.tpdv)
 
         mean, var = self.running_mean_var()
-        out = input_vector * torch.sqrt(var)[(None,) * self.norm_axes] + mean[(None,) * self.norm_axes]
-        
+        out = (
+            input_vector * torch.sqrt(var)[(None,) * self.norm_axes]
+            + mean[(None,) * self.norm_axes]
+        )
+
         out = out.cpu().numpy()
-        
+
         return out
```

### Comparing `openrl-0.0.4/openrl/runners/__init__.py` & `openrl-0.0.5/openrl/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.4/openrl/runners/common/base_agent.py` & `openrl-0.0.5/openrl/runners/common/base_agent.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 import io
-from typing import Union, Type, TypeVar
-from abc import ABC, abstractmethod
 import pathlib
+from abc import ABC, abstractmethod
+from typing import TypeVar, Union
 
 SelfAgent = TypeVar("SelfAgent", bound="BaseAgent")
 
 SelfBaseAgent = TypeVar("SelfBaseAgent", bound="BaseAgent")
 
 
 class BaseAgent(ABC):
```

### Comparing `openrl-0.0.4/openrl/runners/common/ppo_agent.py` & `openrl-0.0.5/openrl/runners/common/ppo_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,29 +13,26 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 import io
 import pathlib
+from typing import Dict, Optional, Tuple, Union
 
-from typing import Union, Dict, Tuple, Optional
-
+import gym
 import numpy as np
 import torch
-import gym
-
-from openrl.runners.common.base_agent import BaseAgent
-from openrl.runners.common.base_agent import SelfAgent
 
-from openrl.drivers.onpolicy_driver import OnPolicyDriver as Driver
 from openrl.algorithms.ppo import PPOAlgorithm as TrainAlgo
 from openrl.buffers import NormalReplayBuffer as ReplayBuffer
-from openrl.utils.logger import Logger
 from openrl.buffers.utils.obs_data import ObsData
+from openrl.drivers.onpolicy_driver import OnPolicyDriver as Driver
+from openrl.runners.common.base_agent import BaseAgent, SelfAgent
+from openrl.utils.logger import Logger
 from openrl.utils.util import _t2n
 
 
 class PPOAgent(BaseAgent):
     def __init__(
         self,
         net: Optional[torch.nn.Module] = None,
@@ -75,16 +72,17 @@
         if run_dir is None:
             self.run_dir = self._cfg.run_dir
         else:
             self.run_dir = run_dir
 
         if self.run_dir is None:
             assert (not self._use_wandb) and (not self._use_tensorboard), (
-                "log_path must be set when using wandb or tensorboard."
-                "Please set log_path in PPOAgent or in the config file or pass run_dir in the command line."
+                "log_path must be set when using wandb or tensorboard.Please set"
+                " log_path in PPOAgent or in the config file or pass run_dir in the"
+                " command line."
             )
 
         if self._cfg.experiment_name == "":
             self.exp_name = "ppo"
         else:
             self.exp_name = self._cfg.experiment_name
```

### Comparing `openrl-0.0.4/openrl/supports/__init__.py` & `openrl-0.0.5/openrl/supports/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.4/openrl/utils/__init__.py` & `openrl-0.0.5/openrl/supports/opendata/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.4/openrl/utils/logger.py` & `openrl-0.0.5/openrl/utils/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,23 +12,24 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 
-import socket
-from typing import Optional, Dict, Any
-import os
 import logging
-from rich.logging import RichHandler
-import wandb
+import os
+import socket
 from pathlib import Path
+from typing import Any, Dict, Optional
+
 import numpy as np
 import torch
+import wandb
+from rich.logging import RichHandler
 
 
 class Logger:
     def __init__(
         self,
         cfg,
         project_name: str,
@@ -60,15 +61,15 @@
         running_programs = [
             "learner",
             "server_learner",
             "local",
             "whole",
             "local_evaluator",
         ]
-        if not self.cfg.program_type in running_programs:
+        if self.cfg.program_type not in running_programs:
             return None
 
         if self.log_path is None:
             assert (not self.use_wandb) and (
                 not self.use_tensorboard
             ), "log_path must be set when using wandb or tensorboard"
             self.use_wandb = False
@@ -171,49 +172,17 @@
         infos: Dict[str, Any],
         step: int,
     ) -> None:
         if not (self.use_wandb or self.use_tensorboard):
             return
 
         for k, v in infos.items():
-            # print(k,v)
-
             if isinstance(v, torch.Tensor):
                 v = v.item()
 
             if not isinstance(v, (int, float)):
                 v = np.mean(v)
 
             if self.use_wandb:
                 wandb.log({k: v}, step=step)
             elif self.use_tensorboard:
                 self.writter.add_scalars(k, {k: v}, step)
-
-
-if __name__ == "__main__":
-    from collections import namedtuple
-
-    ARG = namedtuple("cfg", ["seed", "algorithm_name", "program_type"])
-
-    class Namespace(ARG):
-        @property
-        def __dict__(self):
-            return self._asdict()
-
-    cfg = Namespace(seed=1, algorithm_name="algorithm", program_type="local")
-
-    logger = Logger(
-        cfg=cfg,
-        project_name="test_logger",
-        scenario_name="logger",
-        wandb_entity="openrl",
-        exp_name="test",
-        log_path="../../../test_logger/",
-        use_wandb=False,
-        use_tensorboard=True,
-    )
-    for step in range(100):
-        logger.log_info({"test": step}, step)
-        logger.log_info({"test2": [step, 2 * step]}, step)
-        logger.log_info({"test3": np.random.random((10, 10))}, step)
-    logger.info("hello")
-    logger.close()
```

### Comparing `openrl-0.0.4/openrl.egg-info/SOURCES.txt` & `openrl-0.0.5/openrl.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -25,35 +25,51 @@
 openrl/configs/config.py
 openrl/drivers/__init__.py
 openrl/drivers/base_driver.py
 openrl/drivers/onpolicy_driver.py
 openrl/drivers/rl_driver.py
 openrl/envs/__init__.py
 openrl/envs/common/__init__.py
+openrl/envs/common/build_envs.py
 openrl/envs/common/registration.py
 openrl/envs/gymnasium/__init__.py
 openrl/envs/mpe/__init__.py
 openrl/envs/mpe/core.py
 openrl/envs/mpe/mpe_env.py
 openrl/envs/mpe/multi_discrete.py
 openrl/envs/mpe/multiagent_env.py
 openrl/envs/mpe/rendering.py
 openrl/envs/mpe/scenario.py
 openrl/envs/mpe/scenarios/__init__.py
 openrl/envs/mpe/scenarios/simple_spread.py
+openrl/envs/nlp/__init__.py
+openrl/envs/nlp/daily_dialog_env.py
+openrl/envs/nlp/nlp_env.py
+openrl/envs/nlp/nlp_rewards.py
+openrl/envs/nlp/utils/__init__.py
+openrl/envs/nlp/utils/custom_text_generation_pools.py
+openrl/envs/nlp/utils/distribution.py
+openrl/envs/nlp/utils/evaluation_utils.py
+openrl/envs/nlp/utils/observation.py
+openrl/envs/nlp/utils/sampler.py
+openrl/envs/nlp/utils/text_generation_pool.py
+openrl/envs/nlp/utils/metrics/__init__.py
+openrl/envs/nlp/utils/metrics/meteor.py
 openrl/envs/vec_env/__init__.py
 openrl/envs/vec_env/async_venv.py
 openrl/envs/vec_env/base_venv.py
 openrl/envs/vec_env/sync_venv.py
 openrl/envs/vec_env/utils/__init__.py
 openrl/envs/vec_env/utils/numpy_utils.py
 openrl/envs/vec_env/utils/share_memory.py
 openrl/envs/vec_env/utils/util.py
 openrl/envs/vec_env/wrappers/__init__.py
 openrl/envs/vec_env/wrappers/base_wrapper.py
+openrl/envs/vec_env/wrappers/reward_wrapper.py
+openrl/envs/vec_env/wrappers/vec_info.py
 openrl/envs/vec_env/wrappers/vec_monitor.py
 openrl/envs/wrappers/__init__.py
 openrl/envs/wrappers/base_wrapper.py
 openrl/envs/wrappers/extra_wrappers.py
 openrl/envs/wrappers/multiagent_wrapper.py
 openrl/envs/wrappers/util.py
 openrl/modules/__init__.py
@@ -65,35 +81,51 @@
 openrl/modules/common/base_net.py
 openrl/modules/common/ppo_net.py
 openrl/modules/networks/__init__.py
 openrl/modules/networks/base_policy_network.py
 openrl/modules/networks/base_value_network.py
 openrl/modules/networks/policy_network.py
 openrl/modules/networks/policy_value_network.py
+openrl/modules/networks/policy_value_network_gpt.py
 openrl/modules/networks/value_network.py
 openrl/modules/networks/utils/__init__.py
 openrl/modules/networks/utils/act.py
 openrl/modules/networks/utils/attention.py
 openrl/modules/networks/utils/cnn.py
 openrl/modules/networks/utils/distributed_utils.py
 openrl/modules/networks/utils/distributions.py
 openrl/modules/networks/utils/mix.py
 openrl/modules/networks/utils/mlp.py
 openrl/modules/networks/utils/popart.py
 openrl/modules/networks/utils/rnn.py
 openrl/modules/networks/utils/transformer_act.py
 openrl/modules/networks/utils/util.py
+openrl/modules/networks/utils/nlp/__init__.py
+openrl/modules/networks/utils/nlp/base_policy.py
+openrl/modules/networks/utils/nlp/causal_policy.py
+openrl/modules/networks/utils/nlp/hf_generation_utils.py
 openrl/modules/utils/__init__.py
 openrl/modules/utils/util.py
 openrl/modules/utils/valuenorm.py
+openrl/rewards/__init__.py
+openrl/rewards/base_reward.py
+openrl/rewards/nlp_reward.py
+openrl/rewards/register.py
 openrl/runners/__init__.py
 openrl/runners/common/__init__.py
 openrl/runners/common/base_agent.py
+openrl/runners/common/chat_agent.py
 openrl/runners/common/ppo_agent.py
 openrl/supports/__init__.py
+openrl/supports/opendata/__init__.py
+openrl/supports/opendata/utils/__init__.py
+openrl/supports/opendata/utils/opendata_utils.py
+openrl/supports/opengpu/__init__.py
+openrl/supports/opengpu/gpu_info.py
+openrl/supports/opengpu/manager.py
 openrl/utils/__init__.py
 openrl/utils/logger.py
 openrl/utils/util.py
 tests/__init__.py
 tests/project/__init__.py
 tests/project/test_version.py
 tests/test_buffer/__init__.py
```

### Comparing `openrl-0.0.4/setup.py` & `openrl-0.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 
 import os
-from setuptools import setup, find_packages
+
 import setuptools
+from setuptools import setup
 
 
 def get_install_requires() -> list:
     return [
         "setuptools>=50.0",
         "gymnasium",
         "click",
@@ -31,24 +32,37 @@
         "torch",
         "treevalue",
         "rich",
         "wandb",
         "seaborn",
         "jsonargparse",
         "imageio",
+        "python-opencv",
     ]
 
 
 def get_extra_requires() -> dict:
     req = {
         "test": [
             "pytest",
             "pytest-cov",
+            "mypy",
+            "isort",
+            "black",
+            "ruff",
         ],
+        "dev": ["build", "twine"],
         "mpe": ["pyglet==1.5.27"],
+        "nlp": [
+            "stable-baselines3==1.5.1a5",
+            "transformers==4.18.0",
+            "datasets",
+            "nltk",
+            "evaluate",
+        ],
     }
     return req
 
 
 def get_version() -> str:
     # https://packaging.python.org/guides/single-sourcing-package-version/
     init = open(os.path.join("openrl", "__init__.py"), "r").read().split()
@@ -75,14 +89,16 @@
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
-    keywords="reinforcement-learning multi-agent "
-    "reinforcement-learning-algorithms pytorch machine-learning "
-    "baselines toolbox python data-science gym gymnasium",
+    keywords=(
+        "reinforcement-learning multi-agent "
+        "reinforcement-learning-algorithms pytorch machine-learning "
+        "baselines toolbox python data-science gym gymnasium"
+    ),
     python_requires=">=3.8",
     install_requires=get_install_requires(),
     extras_require=get_extra_requires(),
 )
```

### Comparing `openrl-0.0.4/tests/__init__.py` & `openrl-0.0.5/openrl/supports/opendata/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.4/tests/project/__init__.py` & `openrl-0.0.5/openrl/supports/opengpu/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.4/tests/project/test_version.py` & `openrl-0.0.5/tests/project/test_version.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 import os
 import sys
+
 import pytest
 
 
 @pytest.mark.unittest
 def test_version():
     import openrl
```

### Comparing `openrl-0.0.4/tests/test_buffer/__init__.py` & `openrl-0.0.5/openrl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.4/tests/test_buffer/test_buffer.py` & `openrl-0.0.5/tests/test_buffer/test_buffer.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
-import sys
 import os
+import sys
 
 import numpy as np
 import pytest
 
 from openrl.buffers.utils.obs_data import ObsData
```

