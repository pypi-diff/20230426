# Comparing `tmp/ml-starter-0.0.23.tar.gz` & `tmp/ml-starter-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.0.23.tar", last modified: Thu Apr 20 20:36:47 2023, max compression
+gzip compressed data, was "ml-starter-0.0.24.tar", last modified: Wed Apr 26 21:40:08 2023, max compression
```

## Comparing `ml-starter-0.0.23.tar` & `ml-starter-0.0.24.tar`

### file list

```diff
@@ -1,150 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.259864 ml-starter-0.0.23/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-20 20:36:36.000000 ml-starter-0.0.23/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-20 20:36:47.259864 ml-starter-0.0.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-20 20:36:36.000000 ml-starter-0.0.23/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.235862 ml-starter-0.0.23/ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/__version__.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.239862 ml-starter-0.0.23/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    22561 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.239862 ml-starter-0.0.23/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    32984 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.239862 ml-starter-0.0.23/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.239862 ml-starter-0.0.23/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.239862 ml-starter-0.0.23/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/models/norms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.243863 ml-starter-0.0.23/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.243863 ml-starter-0.0.23/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/scripts/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/scripts/mp_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.243863 ml-starter-0.0.23/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17976 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.243863 ml-starter-0.0.23/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.243863 ml-starter-0.0.23/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13280 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.243863 ml-starter-0.0.23/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.247863 ml-starter-0.0.23/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17646 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.247863 ml-starter-0.0.23/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.247863 ml-starter-0.0.23/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19947 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/trainers/ddp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.251863 ml-starter-0.0.23/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/trainers/sl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/trainers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11504 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/trainers/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.255864 ml-starter-0.0.23/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/call_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.259864 ml-starter-0.0.23/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/torch_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    14933 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.259864 ml-starter-0.0.23/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-20 20:36:47.000000 ml-starter-0.0.23/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-20 20:36:47.000000 ml-starter-0.0.23/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 20:36:47.000000 ml-starter-0.0.23/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-20 20:36:47.000000 ml-starter-0.0.23/ml_starter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-20 20:36:47.000000 ml-starter-0.0.23/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-20 20:36:47.000000 ml-starter-0.0.23/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-20 20:36:36.000000 ml-starter-0.0.23/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-20 20:36:36.000000 ml-starter-0.0.23/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-20 20:36:36.000000 ml-starter-0.0.23/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-20 20:36:47.259864 ml-starter-0.0.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-20 20:36:36.000000 ml-starter-0.0.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.886796 ml-starter-0.0.24/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-26 21:39:56.000000 ml-starter-0.0.24/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-26 21:39:56.000000 ml-starter-0.0.24/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-26 21:40:08.886796 ml-starter-0.0.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-26 21:39:56.000000 ml-starter-0.0.24/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.866796 ml-starter-0.0.24/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.870796 ml-starter-0.0.24/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22358 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.870796 ml-starter-0.0.24/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32984 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.870796 ml-starter-0.0.24/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.870796 ml-starter-0.0.24/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.874796 ml-starter-0.0.24/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/models/norms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.874796 ml-starter-0.0.24/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.874796 ml-starter-0.0.24/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/scripts/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/scripts/mp_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.874796 ml-starter-0.0.24/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17976 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.878796 ml-starter-0.0.24/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.878796 ml-starter-0.0.24/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13280 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.878796 ml-starter-0.0.24/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.878796 ml-starter-0.0.24/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.878796 ml-starter-0.0.24/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.878796 ml-starter-0.0.24/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19947 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/trainers/ddp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.882796 ml-starter-0.0.24/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/trainers/sl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/trainers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/trainers/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.886796 ml-starter-0.0.24/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/call_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.886796 ml-starter-0.0.24/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/torch_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.886796 ml-starter-0.0.24/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-26 21:40:08.000000 ml-starter-0.0.24/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-26 21:40:08.000000 ml-starter-0.0.24/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 21:40:08.000000 ml-starter-0.0.24/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-26 21:40:08.000000 ml-starter-0.0.24/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-26 21:40:08.000000 ml-starter-0.0.24/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-26 21:39:56.000000 ml-starter-0.0.24/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-26 21:39:56.000000 ml-starter-0.0.24/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-26 21:39:56.000000 ml-starter-0.0.24/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-26 21:39:56.000000 ml-starter-0.0.24/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-26 21:40:08.886796 ml-starter-0.0.24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-26 21:39:56.000000 ml-starter-0.0.24/setup.py
```

### Comparing `ml-starter-0.0.23/PKG-INFO` & `ml-starter-0.0.24/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.23
+Version: 0.0.24
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: docs
+License-File: LICENSE
 
 # ML Starter
 
 This is the core code for my ML project template over [here](https://github.com/codekansas/ml-project-template).
 
 ## Installation
```

### Comparing `ml-starter-0.0.23/README.md` & `ml-starter-0.0.24/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/api.py` & `ml-starter-0.0.24/ml/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     "NormType",
     "open_atomic",
     "Output",
     "pad_all",
     "pad_sequence",
     "Phase",
     "project_dir_paths",
+    "read_gif",
     "read_video",
     "reduce",
     "register_logger",
     "register_lr_scheduler",
     "register_model",
     "register_optimizer",
     "register_task",
@@ -135,14 +136,15 @@
     "timeout",
     "Timer",
     "transforms",
     "VanillaTrainer",
     "VanillaTrainerConfig",
     "VideoFileDataset",
     "WorkerPool",
+    "write_gif",
     "write_video",
 ]
 
 from ml.core.common_types import Batch, Loss, Output
 from ml.core.config import conf_field
 from ml.core.env import (
     get_cache_dir,
@@ -241,14 +243,15 @@
     get_rank,
     get_rank_optional,
     get_world_size,
     get_world_size_optional,
     is_distributed,
     is_master,
 )
+from ml.utils.image import read_gif, write_gif
 from ml.utils.io import instantiate_config, load_model_and_task
 from ml.utils.large_models import init_empty_weights, meta_to_empty_func
 from ml.utils.logging import configure_logging
 from ml.utils.numpy import as_cpu_tensor, as_numpy_array
 from ml.utils.random import set_random_seed
 from ml.utils.staging import stage_environment
 from ml.utils.timer import Timer, timeout
```

### Comparing `ml-starter-0.0.23/ml/core/config.py` & `ml-starter-0.0.24/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/core/env.py` & `ml-starter-0.0.24/ml/core/env.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 easily referenced, don't use `os.environ` or `os.getenv` outside of this file.
 Instead, add a new accessor function to this file.
 """
 
 
 import os
 from pathlib import Path
-from typing import Set
 
 
 class _StrEnvVar:
     def __init__(self, key: str, *, default: str | None = None) -> None:
         self.key = key
         self.default = default
 
@@ -29,18 +28,18 @@
 
 
 class _StrSetEnvVar:
     def __init__(self, key: str, *, sep: str = ",") -> None:
         self.key = key
         self.sep = sep
 
-    def get(self) -> Set[str]:
+    def get(self) -> set[str]:
         return {v for v in os.environ.get(self.key, "").split(self.key) if v}
 
-    def set(self, values: Set[str]) -> None:
+    def set(self, values: set[str]) -> None:
         os.environ[self.key] = self.sep.join(v for v in sorted(values) if v)
 
     def add(self, value: str) -> None:
         self.set(self.get() | {value})
 
 
 class _BoolEnvVar:
```

### Comparing `ml-starter-0.0.23/ml/core/registry.py` & `ml-starter-0.0.24/ml/core/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,25 +83,15 @@
     name = config[NAME_KEY]
     if not isinstance(name, str):
         raise ValueError(f"Expected {key} name to be a string, got {name}")
     return name
 
 
 class register_base(ABC, Generic[Entry, Config]):  # pylint: disable=invalid-name
-    """Defines the base registry type.
-
-    Usage:
-
-    ```
-    @register("my_thing", dataclass=MyThingConfig)
-    class MyThing(BaseThing):
-        def __init__(self, config: MyThingConfig):
-            super().__init__(config)
-    ```
-    """
+    """Defines the base registry type."""
 
     REGISTRY: dict[str, tuple[type[Entry], type[Config]]] = {}
     REGISTRY_LOCATIONS: dict[str, Path] = {}
 
     @classmethod
     @abstractmethod
     def search_directory(cls) -> Path:
```

### Comparing `ml-starter-0.0.23/ml/core/state.py` & `ml-starter-0.0.24/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/loggers/base.py` & `ml-starter-0.0.24/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/loggers/meter.py` & `ml-starter-0.0.24/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/loggers/multi.py` & `ml-starter-0.0.24/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/loggers/stdout.py` & `ml-starter-0.0.24/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/loggers/tensorboard.py` & `ml-starter-0.0.24/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/lr_schedulers/base.py` & `ml-starter-0.0.24/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/lr_schedulers/cosine.py` & `ml-starter-0.0.24/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.0.24/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/lr_schedulers/linear.py` & `ml-starter-0.0.24/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.0.24/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.0.24/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/models/activations.py` & `ml-starter-0.0.24/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/models/base.py` & `ml-starter-0.0.24/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/models/embeddings.py` & `ml-starter-0.0.24/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/models/init.py` & `ml-starter-0.0.24/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/models/norms.py` & `ml-starter-0.0.24/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/optimizers/adam.py` & `ml-starter-0.0.24/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/optimizers/adamw.py` & `ml-starter-0.0.24/ml/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/optimizers/adan.py` & `ml-starter-0.0.24/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/optimizers/base.py` & `ml-starter-0.0.24/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/optimizers/sgd.py` & `ml-starter-0.0.24/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/optimizers/shampoo.py` & `ml-starter-0.0.24/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/scripts/cli.py` & `ml-starter-0.0.24/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/scripts/compiler.py` & `ml-starter-0.0.24/ml/scripts/compiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/scripts/stage.py` & `ml-starter-0.0.24/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/scripts/train.py` & `ml-starter-0.0.24/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/tasks/base.py` & `ml-starter-0.0.24/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.0.24/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/tasks/datasets/clippify.py` & `ml-starter-0.0.24/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/tasks/datasets/collate.py` & `ml-starter-0.0.24/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/tasks/datasets/error_handling.py` & `ml-starter-0.0.24/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.0.24/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/tasks/datasets/samplers.py` & `ml-starter-0.0.24/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/tasks/datasets/streaming.py` & `ml-starter-0.0.24/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/tasks/datasets/transforms.py` & `ml-starter-0.0.24/ml/tasks/datasets/transforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
 
         self.height, self.width = height, width
 
     def forward(self, img: Image) -> Image:
         return upper_left_crop(img, self.height, self.width)
 
 
-class Rescale(nn.Module):
+class RescaleImage(nn.Module):
     __constants__ = ["min_val", "scale", "do_checks"]
 
     def __init__(self, min_val: float, max_val: float, do_checks: bool = True) -> None:
         """Rescales an image from (0, 1) to some other scale.
 
         Args:
             min_val: The scale if `max_val` is None, otherwise the min value
```

### Comparing `ml-starter-0.0.23/ml/tasks/datasets/utils.py` & `ml-starter-0.0.24/ml/tasks/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/tasks/datasets/video_file.py` & `ml-starter-0.0.24/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/tasks/environments/base.py` & `ml-starter-0.0.24/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/tasks/environments/utils.py` & `ml-starter-0.0.24/ml/tasks/environments/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from ml.utils.video import Writer, write_video
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 def test_environment(
     env: Environment,
+    *,
     max_steps: int = 100,
     save_path: str | Path | None = None,
     writer: Writer = "ffmpeg",
 ) -> None:
     """Samples a clip from the environment using a random policy.
 
     Args:
@@ -48,8 +49,8 @@
                 yield env.render(state)
 
     # Save the video if a path is provided, otherwise just iterate through the
     # samples from the environment.
     if save_path is None:
         iter_environment()
     else:
-        write_video(writer, iter_environment(), save_path)
+        write_video(iter_environment(), save_path, writer=writer)
```

### Comparing `ml-starter-0.0.23/ml/tasks/environments/worker.py` & `ml-starter-0.0.24/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/tasks/losses/reduce.py` & `ml-starter-0.0.24/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/tasks/rl/base.py` & `ml-starter-0.0.24/ml/tasks/rl/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -440,9 +440,9 @@
 
             images_np = [standardize_image(image) for image in iter_images()]
             return torch.from_numpy(np.stack(images_np))
 
         if return_states:
             raise ValueError("Cannot return states when saving to a file")
 
-        write_video(writer, iter_images(), save_path, fps=environment.fps)
+        write_video(iter_images(), save_path, fps=environment.fps, writer=writer)
         return None
```

### Comparing `ml-starter-0.0.23/ml/tasks/rl/replay.py` & `ml-starter-0.0.24/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/tasks/sl/base.py` & `ml-starter-0.0.24/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/trainers/base.py` & `ml-starter-0.0.24/ml/trainers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/trainers/ddp.py` & `ml-starter-0.0.24/ml/trainers/ddp.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,26 +3,14 @@
 This is a light-weight wrapper around PyTorch's built-in Distributed Data
 Parallel class.
 
 For multiple devices, data is split along the batch dimension, passed to each
 device, which computes losses independently. The loss tensors are gathered to
 the master device to compute a single loss. In other words, each device
 belongs to exactly one process.
-
-Currently this trainer doesn't do anything different from the vanilla trainer
-besides warning when there is more than one GPU. It will be implemented once
-we have a cluster that necessitates it.
-
-Summary table:
-
-|         | device 1    | device 2    | ... | device N       |
-|---------|-------------|-------------|-----|----------------|
-| data    | data[0::N]  | data[1::N]  | ... | data[N - 1::N] |
-| step    | model(x_1)  | model(x_2)  | ... | model(x_N)     |
-| loss    | E(x_1, o_1) | E(x_2, o_2) | ... | E(x_N, o_N)    |
 """
 
 import functools
 import logging
 import os
 import sys
 import traceback
```

### Comparing `ml-starter-0.0.23/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.0.24/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.0.24/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.0.24/ml/trainers/mixins/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.0.24/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.0.24/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.0.24/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/trainers/mixins/profiler.py` & `ml-starter-0.0.24/ml/trainers/mixins/profiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import contextlib
 import datetime
 import logging
 import time
 from dataclasses import dataclass
-from typing import Any, ContextManager, Iterator, Set, TypeVar
+from typing import Any, ContextManager, Iterator, TypeVar
 
 import torch
 
 from ml.core.config import conf_field
 from ml.core.state import State
 from ml.trainers.base import BaseTrainer, BaseTrainerConfig, ModelT, TaskT
 from ml.trainers.mixins.step_wrapper import StepContextMixin, StepType
@@ -27,15 +27,15 @@
     warmup_steps: int = conf_field(10, help="Number of profiler warmup steps")
     active_steps: int = conf_field(10, help="Number of profiler active steps")
     repeat_steps: int = conf_field(1, help="Number of profiler repetitions")
     skip_first_steps: int = conf_field(10, help="Number of profiler steps to skip at first")
     table_size: int = conf_field(10, help="Number of profiling ops to print")
 
 
-STEPS_TO_TIME: Set[StepType] = {
+STEPS_TO_TIME: set[StepType] = {
     "backward",
     "clip_grads",
     "forward",
     "get_single_loss",
     "log_losses",
     "on_step_end",
     "on_step_start",
```

### Comparing `ml-starter-0.0.23/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.0.24/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/trainers/rl.py` & `ml-starter-0.0.24/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/trainers/sl.py` & `ml-starter-0.0.24/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/trainers/slurm.py` & `ml-starter-0.0.24/ml/trainers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/trainers/vanilla.py` & `ml-starter-0.0.24/ml/trainers/vanilla.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,11 @@
 """Defines a vanilla trainer which doesn't do any device or data manipulation.
 
 This trainer expects the task to handle all the relevant movement of data and
 models to their associated devices.
-
-Summary table:
-
-|         | device 1 - N |
-|---------|--------------|
-| data    | data[:]      |
-| step    | model(x)     |
-| loss    | E(x, o)      |
 """
 
 import logging
 import signal
 from dataclasses import dataclass
 from types import FrameType
 from typing import Callable, Generic, TypeVar, cast
```

### Comparing `ml-starter-0.0.23/ml/utils/argparse.py` & `ml-starter-0.0.24/ml/utils/argparse.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,53 @@
+"""Utilities for using argparse with dataclasses."""
+
 import argparse
 from dataclasses import MISSING, fields
 from typing import Any, Type, TypeVar, Union, cast, get_args, get_origin
 
 from omegaconf import OmegaConf
 
 from ml.core.config import BaseConfig
 
 Config = TypeVar("Config", bound=BaseConfig)
 
 
 def get_type_from_string(type_name: str) -> Type:
+    """Parses a type name to a string.
+
+    Args:
+        type_name: The type name to parse.
+
+    Returns:
+        The type corresponding to the type name.
+
+    Raises:
+        ValueError: If the type name is not supported.
+    """
+
     if type_name == "str":
         return str
     if type_name == "float":
         return float
     if type_name == "int":
         return int
     raise ValueError(type_name)
 
 
 def add_args(parser: argparse.ArgumentParser, dc: Type[Config]) -> None:
+    """Adds arguments to an argument parser from a dataclass.
+
+    Args:
+        parser: The argument parser to add arguments to.
+        dc: The dataclass to add arguments from.
+
+    Raises:
+        NotImplementedError: If the dataclass has a field with an unsupported type.
+    """
+
     for field in fields(dc):
         args: list[str] = []
         if field.metadata.get("short") is not None:
             args.append(f"-{field.metadata['short']}")
         args.append(f"--{field.name.replace('_', '-')}")
         kwargs: dict[str, Any] = {}
         if field.default != MISSING:
@@ -58,13 +82,23 @@
             kwargs["type"] = field_type
         else:
             raise NotImplementedError(f"Couldn't get type for {field.name}")
         parser.add_argument(*args, **kwargs)
 
 
 def from_args(args: argparse.Namespace, dc: Type[Config]) -> Config:
+    """Creates a dataclass from an argument parser namespace.
+
+    Args:
+        args: The argument parser namespace to create the dataclass from.
+        dc: The dataclass to create.
+
+    Returns:
+        The dataclass created from the argument parser namespace.
+    """
+
     values: dict[str, Any] = {}
     for field in fields(dc):
         values[field.name] = getattr(args, field.name)
     cfg = OmegaConf.structured(dc(**values))
     dc.resolve(cfg)
     return cfg
```

### Comparing `ml-starter-0.0.23/ml/utils/augmentation.py` & `ml-starter-0.0.24/ml/utils/augmentation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Augmentation utilities for image data."""
+
 import torch
 from torch import Tensor
 
 
 def get_image_mask(image: Tensor, *, min_prct: float = 0.2, max_prct: float = 0.5) -> Tensor:
     """Gets a random mask for the image.
```

### Comparing `ml-starter-0.0.23/ml/utils/caching.py` & `ml-starter-0.0.24/ml/utils/caching.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Defines a wrapper for caching function calls to a file location."""
+
 import functools
 import json
 import logging
 import pickle
 from typing import Any, Callable, Generic, Literal, Mapping, Sequence, TypeVar, get_args
 
 import numpy as np
@@ -20,23 +22,14 @@
 class cached_object:  # pylint: disable=invalid-name
     def __init__(self, cache_key: str, ext: CacheType = "pkl", ignore: bool = False, cache_obj: bool = True) -> None:
         """Defines a wrapper for caching function calls to a file location.
 
         This is just a convenient way of caching heavy operations to disk,
         using a specific key.
 
-        Usage:
-
-            ```
-            @cached_object("video-dataset-clips")
-            def get_clip_paths(dataset_name: str) -> list[str]:
-                root_path = dataset_root / dataset_name
-                return [str(path.resolve()) for path in root_path.glob("**/*.mov")]
-            ```
-
         Args:
             cache_key: The key to use for caching the file
             ext: The caching type to use (JSON or pickling)
             ignore: Should the cache be ignored?
             cache_obj: If set, keep the object around to avoid deserializing it
                 when it is accessed again
         """
```

### Comparing `ml-starter-0.0.23/ml/utils/call_train.py` & `ml-starter-0.0.24/ml/utils/call_train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/utils/cli.py` & `ml-starter-0.0.24/ml/utils/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Command-line interface utilities."""
+
 import logging
 import sys
 from functools import partial
 from pathlib import Path
 from typing import cast
 
 from omegaconf import DictConfig, OmegaConf
```

### Comparing `ml-starter-0.0.23/ml/utils/colors.py` & `ml-starter-0.0.24/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/utils/compiler.py` & `ml-starter-0.0.24/ml/utils/compiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/utils/data.py` & `ml-starter-0.0.24/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/utils/datetime.py` & `ml-starter-0.0.24/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/utils/device/auto.py` & `ml-starter-0.0.24/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/utils/device/base.py` & `ml-starter-0.0.24/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/utils/device/cpu.py` & `ml-starter-0.0.24/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/utils/device/gpu.py` & `ml-starter-0.0.24/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/utils/device/metal.py` & `ml-starter-0.0.24/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/utils/distributed.py` & `ml-starter-0.0.24/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/utils/io.py` & `ml-starter-0.0.24/ml/utils/io.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/utils/large_models.py` & `ml-starter-0.0.24/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/utils/logging.py` & `ml-starter-0.0.24/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/utils/meter.py` & `ml-starter-0.0.24/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/utils/staging.py` & `ml-starter-0.0.24/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/utils/timer.py` & `ml-starter-0.0.24/ml/utils/timer.py`

 * *Files 6% similar despite different names*

```diff
@@ -102,22 +102,14 @@
 
 
 def timeout(seconds: int, error_message: str = os.strerror(errno.ETIME)) -> Callable[[TimeoutFunc], TimeoutFunc]:
     """Decorator for timing out long-running functions.
 
     Note that this function won't work on Windows.
 
-    Usage:
-        try:
-            @timeout(5)
-            def long_running_function():
-                ...
-        except TimeoutError:
-            handle_timeout()
-
     Args:
         seconds: Timeout after this many seconds
         error_message: Error message to pass to TimeoutError
 
     Returns:
         Decorator function
     """
```

### Comparing `ml-starter-0.0.23/ml/utils/torch_distributed.py` & `ml-starter-0.0.24/ml/utils/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/ml/utils/video.py` & `ml-starter-0.0.24/ml/utils/video.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,24 @@
 import asyncio
-import math
 import re
 import shutil
 import warnings
 from dataclasses import dataclass
 from fractions import Fraction
 from pathlib import Path
 from typing import AsyncGenerator, Iterator, Literal
 
 import cv2
 import ffmpeg
 import matplotlib.animation as ani
 import matplotlib.pyplot as plt
 import numpy as np
-import torch
-import torchvision.transforms.functional as V
 from torch import Tensor
-from torchvision.transforms import InterpolationMode
 
-VALID_CHANNEL_COUNTS = {1, 3}
-
-
-def as_uint8(arr: np.ndarray) -> np.ndarray:
-    if np.issubdtype(arr.dtype, np.integer):
-        return arr.astype(np.uint8)
-    if np.issubdtype(arr.dtype, np.floating):
-        return (arr * 255).round().astype(np.uint8)
-    raise NotImplementedError(f"Unsupported dtype: {arr.dtype}")
+from ml.utils.image import as_uint8, standardize_image
 
 
 @dataclass
 class VideoProps:
     frame_width: int
     frame_height: int
     frame_count: int
@@ -61,94 +49,14 @@
                     frame_count=count,
                     fps=Fraction(int(fps_num), int(fps_denom)),
                 )
 
         raise ValueError(f"Could not parse video properties from video in {fpath}")
 
 
-def _aminmax(t: Tensor) -> tuple[Tensor, Tensor]:
-    # `aminmax` isn't supported for MPS tensors, fall back to separate calls.
-    minv, maxv = (t.min(), t.max()) if t.is_mps else tuple(t.aminmax())
-    return minv, maxv
-
-
-def make_human_viewable_resolution(
-    image: Tensor,
-    interpolation: InterpolationMode = InterpolationMode.BILINEAR,
-    trg_res: tuple[int, int] = (250, 250),
-) -> Tensor:
-    """Resizes image to human-viewable resolution.
-
-    Args:
-        image: The image to resize, with shape (C, H, W)
-        interpolation: Interpolation mode to use for image resizing
-        trg_res: The target image resolution; the image will be reshaped to
-            have approximately the same area as an image with this resolution
-
-    Returns:
-        The resized image
-    """
-
-    width, height = V.get_image_size(image)
-    trg_height, trg_width = trg_res
-    factor = math.sqrt((trg_height * trg_width) / (height * width))
-    new_height, new_width = int(height * factor), int(width * factor)
-    return V.resize(image, [new_height, new_width], interpolation)
-
-
-def standardize_image(
-    image: np.ndarray | Tensor,
-    *,
-    log_key: str | None = None,
-    normalize: bool = True,
-    keep_resolution: bool = False,
-) -> np.ndarray:
-    """Converts an arbitrary image to shape (C, H, W).
-
-    Args:
-        image: The image tensor to log
-        log_key: An optional logging key to use in the exception message
-        normalize: Normalize images to (0, 1)
-        keep_resolution: If set, preserve original image resolution, otherwise
-            change image resolution to human-viewable
-
-    Returns:
-        The normalized image, with shape (H, W, C)
-
-    Raises:
-        ValueError: If the image shape is invalid
-    """
-
-    if isinstance(image, np.ndarray):
-        image = torch.from_numpy(image)
-
-    if normalize and image.is_floating_point():
-        minv, maxv = _aminmax(image)
-        maxv.clamp_min_(1.0)
-        minv.clamp_max_(0.0)
-        image = torch.clamp((image.detach() - minv) / (maxv - minv), 0.0, 1.0)
-
-    if image.ndim == 2:
-        image = image.unsqueeze(0)
-    elif image.ndim == 3:
-        if image.shape[0] in VALID_CHANNEL_COUNTS:
-            pass
-        elif image.shape[2] in VALID_CHANNEL_COUNTS:
-            image = image.permute(2, 0, 1)
-        else:
-            raise ValueError(f"Invalid channel count{'' if log_key is None else f' for {log_key}'}: {image.shape}")
-    else:
-        raise ValueError(f"Invalid image shape{'' if log_key is None else f' for {log_key}'}: {image.shape}")
-
-    if not keep_resolution:
-        image = make_human_viewable_resolution(image)
-
-    return image.permute(1, 2, 0).detach().cpu().numpy()
-
-
 def read_video_ffmpeg(
     in_file: str | Path,
     *,
     output_fmt: str = "rgb24",
     channels: int = 3,
 ) -> Iterator[np.ndarray]:
     """Function that reads a video to a stream of numpy arrays using FFMPEG.
@@ -277,117 +185,126 @@
         yield buffer
 
 
 def write_video_opencv(
     itr: Iterator[np.ndarray | Tensor],
     out_file: str | Path,
     *,
+    keep_resolution: bool = False,
     fps: int | Fraction = 30,
     codec: str = "MP4V",
 ) -> None:
     """Function that writes a video from a stream of numpy arrays using OpenCV.
 
     Args:
         itr: The image iterator, yielding images with shape (H, W, C).
         out_file: The path to the output file.
+        keep_resolution: If set, don't change the image resolution, otherwise
+            resize to a human-friendly resolution.
         fps: Frames per second for the video.
         codec: FourCC code specifying OpenCV video codec type. Examples are
             MPEG, MP4V, DIVX, AVC1, H236.
     """
 
     Path(out_file).parent.mkdir(exist_ok=True, parents=True)
 
-    first_img = standardize_image(next(itr))
+    first_img = standardize_image(next(itr), keep_resolution=keep_resolution)
     height, width, _ = first_img.shape
 
     fourcc = cv2.VideoWriter_fourcc(*codec)
     stream = cv2.VideoWriter(str(out_file), fourcc, fps if isinstance(fps, int) else round(fps), (width, height))
 
     def write_frame(img: np.ndarray) -> None:
         stream.write(as_uint8(img))
 
     write_frame(first_img)
     for img in itr:
-        write_frame(standardize_image(img))
+        write_frame(standardize_image(img, keep_resolution=keep_resolution))
 
     stream.release()
     cv2.destroyAllWindows()
 
 
 def write_video_ffmpeg(
     itr: Iterator[np.ndarray | Tensor],
     out_file: str | Path,
     *,
+    keep_resolution: bool = False,
     fps: int | Fraction = 30,
     out_fps: int | Fraction = 30,
     vcodec: str = "libx264",
     input_fmt: str = "rgb24",
     output_fmt: str = "yuv420p",
 ) -> None:
     """Function that writes an video from a stream of numpy arrays using FFMPEG.
 
     Args:
         itr: The image iterator, yielding images with shape (H, W, C).
         out_file: The path to the output file.
+        keep_resolution: If set, don't change the image resolution, otherwise
+            resize to a human-friendly resolution.
         fps: Frames per second for the video.
         out_fps: Frames per second for the saved video.
         vcodec: The video codec to use for the output video
         input_fmt: The input image format
         output_fmt: The output image format
     """
 
     Path(out_file).parent.mkdir(exist_ok=True, parents=True)
 
-    first_img = standardize_image(next(itr))
+    first_img = standardize_image(next(itr), keep_resolution=keep_resolution)
     height, width, _ = first_img.shape
 
     stream = ffmpeg.input("pipe:", format="rawvideo", pix_fmt=input_fmt, s=f"{width}x{height}", r=float(fps))
     stream = ffmpeg.output(stream, str(out_file), pix_fmt=output_fmt, vcodec=vcodec, r=float(out_fps))
     stream = ffmpeg.overwrite_output(stream)
     stream = ffmpeg.run_async(stream, pipe_stdin=True)
 
     def write_frame(img: np.ndarray) -> None:
         stream.stdin.write(as_uint8(img).tobytes())
 
     # Writes all the video frames to the file.
     write_frame(first_img)
     for img in itr:
-        write_frame(standardize_image(img))
+        write_frame(standardize_image(img, keep_resolution=keep_resolution))
 
     stream.stdin.close()
     stream.wait()
 
 
 def write_video_matplotlib(
     itr: Iterator[np.ndarray | Tensor],
     out_file: str | Path,
     *,
+    keep_resolution: bool = False,
     dpi: int = 50,
     fps: int | Fraction = 30,
     title: str = "Video",
     comment: str | None = None,
     writer: str = "ffmpeg",
 ) -> None:
     """Function that writes an video from a stream of input tensors.
 
     Args:
         itr: The image iterator, yielding images with shape (H, W, C).
         out_file: The path to the output file.
+        keep_resolution: If set, don't change the image resolution, otherwise
+            resize to a human-friendly resolution.
         dpi: Dots per inch for output image.
         fps: Frames per second for the video.
         title: Title for the video metadata.
         comment: Comment for the video metadata.
         writer: The Matplotlib video writer to use (if you use the
             default one, make sure you have `ffmpeg` installed on your
             system).
     """
 
     Path(out_file).parent.mkdir(exist_ok=True, parents=True)
 
-    first_img = standardize_image(next(itr))
+    first_img = standardize_image(next(itr), keep_resolution=keep_resolution)
     height, width, _ = first_img.shape
     fig, ax = plt.subplots(figsize=(width / dpi, height / dpi))
 
     # Ensures that there's no extra space around the image.
     fig.subplots_adjust(
         left=0,
         bottom=0,
@@ -410,15 +327,15 @@
     )
 
     with mpl_writer.saving(fig, out_file, dpi=dpi):
         im = ax.imshow(as_uint8(first_img), interpolation="nearest")
         mpl_writer.grab_frame()
 
         for img in itr:
-            im.set_data(as_uint8(standardize_image(img)))
+            im.set_data(as_uint8(standardize_image(img, keep_resolution=keep_resolution)))
             mpl_writer.grab_frame()
 
 
 Reader = Literal["ffmpeg", "opencv"]
 Writer = Literal["ffmpeg", "matplotlib", "opencv"]
 
 
@@ -433,31 +350,49 @@
     if reader == "opencv":
         return read_video_opencv(in_file)
 
     raise ValueError(f"Invalid reader: {reader}")
 
 
 def write_video(
-    writer: Writer,
     itr: Iterator[np.ndarray | Tensor],
     out_file: str | Path,
     *,
     fps: int | Fraction = 30,
+    keep_resolution: bool = False,
+    writer: Writer = "ffmpeg",
 ) -> None:
+    """Function that writes an video from a stream of input tensors.
+
+    Args:
+        itr: The image iterator, yielding images with shape (H, W, C).
+        out_file: The path to the output file.
+        fps: Frames per second for the video.
+        keep_resolution: If set, don't change the image resolution, otherwise
+            resize to a human-friendly resolution.
+        writer: The video writer to use.
+
+    Raises:
+        ValueError: If the writer is invalid.
+    """
+
     if writer == "ffmpeg":
         if not shutil.which("ffmpeg"):
             warnings.warn("FFMPEG is not available in the system. Falling back to OpenCV.")
             writer = "opencv"
         else:
-            return write_video_ffmpeg(itr, out_file, fps=fps)
+            write_video_ffmpeg(itr, out_file, fps=fps, keep_resolution=keep_resolution)
+            return
 
     if writer == "matplotlib":
         if not shutil.which("ffmpeg"):
             warnings.warn("FFMPEG is not available in the system. Falling back to OpenCV.")
             writer = "opencv"
         else:
-            return write_video_matplotlib(itr, out_file, fps=fps)
+            write_video_matplotlib(itr, out_file, fps=fps, keep_resolution=keep_resolution)
+            return
 
     if writer == "opencv":
-        return write_video_opencv(itr, out_file, fps=fps)
+        write_video_opencv(itr, out_file, fps=fps, keep_resolution=keep_resolution)
+        return
 
     raise ValueError(f"Invalid writer: {writer}")
```

### Comparing `ml-starter-0.0.23/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.0.24/ml_starter.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.23
+Version: 0.0.24
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: docs
+License-File: LICENSE
 
 # ML Starter
 
 This is the core code for my ML project template over [here](https://github.com/codekansas/ml-project-template).
 
 ## Installation
```

### Comparing `ml-starter-0.0.23/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.0.24/ml_starter.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements-dev.txt
+requirements-docs.txt
 requirements.txt
 setup.cfg
 setup.py
 ml/__init__.py
-ml/__version__.txt
 ml/api.py
 ml/py.typed
 ml/core/__init__.py
 ml/core/common_types.py
 ml/core/config.py
 ml/core/env.py
 ml/core/registry.py
@@ -100,14 +101,15 @@
 ml/utils/checks.py
 ml/utils/cli.py
 ml/utils/colors.py
 ml/utils/compiler.py
 ml/utils/data.py
 ml/utils/datetime.py
 ml/utils/distributed.py
+ml/utils/image.py
 ml/utils/io.py
 ml/utils/large_models.py
 ml/utils/logging.py
 ml/utils/meter.py
 ml/utils/networking.py
 ml/utils/numpy.py
 ml/utils/random.py
@@ -120,10 +122,9 @@
 ml/utils/device/base.py
 ml/utils/device/cpu.py
 ml/utils/device/gpu.py
 ml/utils/device/metal.py
 ml_starter.egg-info/PKG-INFO
 ml_starter.egg-info/SOURCES.txt
 ml_starter.egg-info/dependency_links.txt
-ml_starter.egg-info/entry_points.txt
 ml_starter.egg-info/requires.txt
 ml_starter.egg-info/top_level.txt
```

### Comparing `ml-starter-0.0.23/pyproject.toml` & `ml-starter-0.0.24/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.23/setup.py` & `ml-starter-0.0.24/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 #!/usr/bin/env python
 
+import re
+
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description: str = f.read()
 
 
 with open("requirements.txt", "r", encoding="utf-8") as f:
     requirements: list[str] = f.read().splitlines()
 
 
 with open("requirements-dev.txt", "r", encoding="utf-8") as f:
     requirements_dev: list[str] = f.read().splitlines()
 
 
-with open("ml/__version__.txt", "r", encoding="utf-8") as fh:
-    version = fh.read().strip()
+with open("requirements-docs.txt", "r", encoding="utf-8") as f:
+    requirements_docs: list[str] = f.read().splitlines()
+
+
+with open("ml/__init__.py", "r", encoding="utf-8") as fh:
+    version_re = re.search(r"^__version__ = \"([^\"]*)\"", fh.read(), re.MULTILINE)
+assert version_re is not None, "Could not find version in ml/__init__.py"
+version: str = version_re.group(1)
 
 
 setup(
     name="ml-starter",
     version=version,
     description="ML project template repository",
     author="Benjamin Bolte",
@@ -32,10 +40,10 @@
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
     ],
     python_requires=">=3.10",
     install_requires=requirements,
     tests_require=requirements_dev,
-    extras_require={"dev": requirements_dev},
+    extras_require={"dev": requirements_dev, "docs": requirements_docs},
     package_data={"ml": ["py.typed"]},
 )
```

