# Comparing `tmp/fastestimator-1.5.1.tar.gz` & `tmp/fastestimator-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastestimator-1.5.1.tar", last modified: Tue Apr 25 19:12:45 2023, max compression
+gzip compressed data, was "dist/fastestimator-1.5.2.tar", last modified: Tue Apr 25 20:41:41 2023, max compression
```

## Comparing `fastestimator-1.5.1.tar` & `fastestimator-1.5.2.tar`

### file list

```diff
@@ -1,766 +1,766 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:18.318213 fastestimator-1.5.1/
--rw-r--r--   0 root         (0) root         (0)      591 2023-04-25 19:11:18.316242 fastestimator-1.5.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5698 2023-04-25 17:05:48.000000 fastestimator-1.5.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:10.582542 fastestimator-1.5.1/fastestimator/
--rw-r--r--   0 root         (0) root         (0)     3092 2023-04-24 03:07:42.000000 fastestimator-1.5.1/fastestimator/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:10.593073 fastestimator-1.5.1/fastestimator/architecture/
--rw-r--r--   0 root         (0) root         (0)     1018 2023-04-24 02:38:58.000000 fastestimator-1.5.1/fastestimator/architecture/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:10.657368 fastestimator-1.5.1/fastestimator/architecture/pytorch/
--rw-r--r--   0 root         (0) root         (0)     1609 2023-04-24 02:38:58.000000 fastestimator-1.5.1/fastestimator/architecture/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7452 2023-04-24 02:38:58.000000 fastestimator-1.5.1/fastestimator/architecture/pytorch/attention_unet.py
--rw-r--r--   0 root         (0) root         (0)     2898 2023-04-24 02:38:58.000000 fastestimator-1.5.1/fastestimator/architecture/pytorch/lenet.py
--rw-r--r--   0 root         (0) root         (0)     4148 2023-04-24 02:38:58.000000 fastestimator-1.5.1/fastestimator/architecture/pytorch/resnet9.py
--rw-r--r--   0 root         (0) root         (0)     5889 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/architecture/pytorch/unet.py
--rw-r--r--   0 root         (0) root         (0)     6188 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/architecture/pytorch/wideresnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:10.720890 fastestimator-1.5.1/fastestimator/architecture/tensorflow/
--rw-r--r--   0 root         (0) root         (0)     1624 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/architecture/tensorflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4800 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/architecture/tensorflow/attention_unet.py
--rw-r--r--   0 root         (0) root         (0)     2216 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/architecture/tensorflow/lenet.py
--rw-r--r--   0 root         (0) root         (0)     3355 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/architecture/tensorflow/resnet9.py
--rw-r--r--   0 root         (0) root         (0)     3718 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/architecture/tensorflow/unet.py
--rw-r--r--   0 root         (0) root         (0)     5580 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/architecture/tensorflow/wideresnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:11.391343 fastestimator-1.5.1/fastestimator/backend/
--rw-r--r--   0 root         (0) root         (0)    10290 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_abs.py
--rw-r--r--   0 root         (0) root         (0)     2252 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_argmax.py
--rw-r--r--   0 root         (0) root         (0)     4939 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_binary_crossentropy.py
--rw-r--r--   0 root         (0) root         (0)     3876 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_cast.py
--rw-r--r--   0 root         (0) root         (0)     5024 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_categorical_crossentropy.py
--rw-r--r--   0 root         (0) root         (0)     1859 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_check_nan.py
--rw-r--r--   0 root         (0) root         (0)     3294 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_clip_by_value.py
--rw-r--r--   0 root         (0) root         (0)     2539 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_concat.py
--rw-r--r--   0 root         (0) root         (0)     1410 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_convert_tensor_precision.py
--rw-r--r--   0 root         (0) root         (0)     7734 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_dice_score.py
--rw-r--r--   0 root         (0) root         (0)     1850 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_exp.py
--rw-r--r--   0 root         (0) root         (0)     2335 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_expand_dims.py
--rw-r--r--   0 root         (0) root         (0)     2502 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_feed_forward.py
--rw-r--r--   0 root         (0) root         (0)     2699 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_flip.py
--rw-r--r--   0 root         (0) root         (0)     6244 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_focal_loss.py
--rw-r--r--   0 root         (0) root         (0)     3148 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_gather.py
--rw-r--r--   0 root         (0) root         (0)     3421 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_gather_from_batch.py
--rw-r--r--   0 root         (0) root         (0)     4694 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_get_gradient.py
--rw-r--r--   0 root         (0) root         (0)     2512 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_get_image_dims.py
--rw-r--r--   0 root         (0) root         (0)     1895 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_get_lr.py
--rw-r--r--   0 root         (0) root         (0)     1979 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_get_shape.py
--rw-r--r--   0 root         (0) root         (0)     2225 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_hinge.py
--rw-r--r--   0 root         (0) root         (0)     3484 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_huber.py
--rw-r--r--   0 root         (0) root         (0)     4511 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_iwd.py
--rw-r--r--   0 root         (0) root         (0)     3161 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_l1_loss.py
--rw-r--r--   0 root         (0) root         (0)     1797 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_l2_regularization.py
--rw-r--r--   0 root         (0) root         (0)     4558 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_lambertw.py
--rw-r--r--   0 root         (0) root         (0)     4420 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_load_model.py
--rw-r--r--   0 root         (0) root         (0)     2226 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_matmul.py
--rw-r--r--   0 root         (0) root         (0)     2161 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_maximum.py
--rw-r--r--   0 root         (0) root         (0)     2788 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_mean_squared_error.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_ones_like.py
--rw-r--r--   0 root         (0) root         (0)     5065 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_percentile.py
--rw-r--r--   0 root         (0) root         (0)     2727 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_permute.py
--rw-r--r--   0 root         (0) root         (0)     1952 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_pow.py
--rw-r--r--   0 root         (0) root         (0)     2923 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_random_normal_like.py
--rw-r--r--   0 root         (0) root         (0)     3005 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_random_uniform_like.py
--rw-r--r--   0 root         (0) root         (0)     3123 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_reduce_max.py
--rw-r--r--   0 root         (0) root         (0)     3259 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_reduce_mean.py
--rw-r--r--   0 root         (0) root         (0)     3159 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_reduce_min.py
--rw-r--r--   0 root         (0) root         (0)     3199 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_reduce_std.py
--rw-r--r--   0 root         (0) root         (0)     2997 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_reduce_sum.py
--rw-r--r--   0 root         (0) root         (0)     3067 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_reshape.py
--rw-r--r--   0 root         (0) root         (0)     4256 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_resize3d.py
--rw-r--r--   0 root         (0) root         (0)     3182 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_roll.py
--rw-r--r--   0 root         (0) root         (0)     4633 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_save_model.py
--rw-r--r--   0 root         (0) root         (0)     3069 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_set_lr.py
--rw-r--r--   0 root         (0) root         (0)     1839 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_sign.py
--rw-r--r--   0 root         (0) root         (0)     3639 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_smooth_l1_loss.py
--rw-r--r--   0 root         (0) root         (0)     4889 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_sparse_categorical_crossentropy.py
--rw-r--r--   0 root         (0) root         (0)     2785 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_squeeze.py
--rw-r--r--   0 root         (0) root         (0)     5661 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_tensor_normalize.py
--rw-r--r--   0 root         (0) root         (0)     2431 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_tensor_pow.py
--rw-r--r--   0 root         (0) root         (0)     1994 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_tensor_round.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_tensor_sqrt.py
--rw-r--r--   0 root         (0) root         (0)     3832 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_to_shape.py
--rw-r--r--   0 root         (0) root         (0)     3835 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_to_tensor.py
--rw-r--r--   0 root         (0) root         (0)     2807 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_to_type.py
--rw-r--r--   0 root         (0) root         (0)     1948 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_transpose.py
--rw-r--r--   0 root         (0) root         (0)     5245 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_update_model.py
--rw-r--r--   0 root         (0) root         (0)     2207 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_watch.py
--rw-r--r--   0 root         (0) root         (0)     2482 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_zeros_like.py
--rw-r--r--   0 root         (0) root         (0)     2416 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/backend/_zscore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:11.464607 fastestimator-1.5.1/fastestimator/cli/
--rw-r--r--   0 root         (0) root         (0)     1618 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8845 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/cli/history.py
--rw-r--r--   0 root         (0) root         (0)     5358 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/cli/logs.py
--rw-r--r--   0 root         (0) root         (0)     1843 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/cli/main.py
--rw-r--r--   0 root         (0) root         (0)     5468 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/cli/plot.py
--rw-r--r--   0 root         (0) root         (0)     3485 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/cli/run.py
--rw-r--r--   0 root         (0) root         (0)     6574 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/cli/train.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:11.599202 fastestimator-1.5.1/fastestimator/dataset/
--rw-r--r--   0 root         (0) root         (0)     2529 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16449 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/batch_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1804 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/csv_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:11.868519 fastestimator-1.5.1/fastestimator/dataset/data/
--rw-r--r--   0 root         (0) root         (0)     1757 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/data/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1566 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/data/breast_cancer.py
--rw-r--r--   0 root         (0) root         (0)     3396 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/data/cifair10.py
--rw-r--r--   0 root         (0) root         (0)     2831 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/data/cifair100.py
--rw-r--r--   0 root         (0) root         (0)     1568 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/data/cifar10.py
--rw-r--r--   0 root         (0) root         (0)     1915 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/data/cifar100.py
--rw-r--r--   0 root         (0) root         (0)     5708 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/data/cub200.py
--rw-r--r--   0 root         (0) root         (0)     3698 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/data/food101.py
--rw-r--r--   0 root         (0) root         (0)     3712 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/data/horse2zebra.py
--rw-r--r--   0 root         (0) root         (0)     2174 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/data/imdb_review.py
--rw-r--r--   0 root         (0) root         (0)     3750 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/data/mendeley.py
--rw-r--r--   0 root         (0) root         (0)     4011 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/data/mitmovie_ner.py
--rw-r--r--   0 root         (0) root         (0)     1338 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/data/mnist.py
--rw-r--r--   0 root         (0) root         (0)     3321 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/data/montgomery.py
--rw-r--r--   0 root         (0) root         (0)    10000 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/data/mscoco.py
--rw-r--r--   0 root         (0) root         (0)     3856 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/data/nih_chestxray.py
--rw-r--r--   0 root         (0) root         (0)     2643 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/data/omniglot.py
--rw-r--r--   0 root         (0) root         (0)     3269 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/data/penn_treebank.py
--rw-r--r--   0 root         (0) root         (0)     2695 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/data/shakespeare.py
--rw-r--r--   0 root         (0) root         (0)     1195 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/data/skl_digits.py
--rw-r--r--   0 root         (0) root         (0)     6097 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/data/svhn.py
--rw-r--r--   0 root         (0) root         (0)     2827 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/data/svhn_cropped.py
--rw-r--r--   0 root         (0) root         (0)     3914 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/data/tednmt.py
--rw-r--r--   0 root         (0) root         (0)     4183 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/data/tiny_imagenet.py
--rw-r--r--   0 root         (0) root         (0)     5509 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/data/usps.py
--rw-r--r--   0 root         (0) root         (0)    20437 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/dataloader.py
--rw-r--r--   0 root         (0) root         (0)    25375 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/dataset.py
--rw-r--r--   0 root         (0) root         (0)     1974 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/dir_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2263 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/extend_dataset.py
--rw-r--r--   0 root         (0) root         (0)     4086 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/generator_dataset.py
--rw-r--r--   0 root         (0) root         (0)     3599 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/labeled_dir_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1988 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/numpy_dataset.py
--rw-r--r--   0 root         (0) root         (0)     8402 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/op_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1476 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/pickle_dataset.py
--rw-r--r--   0 root         (0) root         (0)     9018 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/dataset/siamese_dir_dataset.py
--rw-r--r--   0 root         (0) root         (0)    31566 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/estimator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:11.878463 fastestimator-1.5.1/fastestimator/layers/
--rw-r--r--   0 root         (0) root         (0)     1012 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/layers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:11.912067 fastestimator-1.5.1/fastestimator/layers/pytorch/
--rw-r--r--   0 root         (0) root         (0)     1200 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/layers/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3887 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/layers/pytorch/cropping_2d.py
--rw-r--r--   0 root         (0) root         (0)     6553 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/layers/pytorch/hadamard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:11.997352 fastestimator-1.5.1/fastestimator/layers/tensorflow/
--rw-r--r--   0 root         (0) root         (0)     1370 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/layers/tensorflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7334 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/layers/tensorflow/hadamard.py
--rw-r--r--   0 root         (0) root         (0)     2591 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/layers/tensorflow/instance_norm.py
--rw-r--r--   0 root         (0) root         (0)     2490 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/layers/tensorflow/reflection_padding_2d.py
--rw-r--r--   0 root         (0) root         (0)    50615 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/network.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:12.028384 fastestimator-1.5.1/fastestimator/op/
--rw-r--r--   0 root         (0) root         (0)     1152 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:12.048468 fastestimator-1.5.1/fastestimator/op/numpyop/
--rw-r--r--   0 root         (0) root         (0)     1318 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:12.135168 fastestimator-1.5.1/fastestimator/op/numpyop/meta/
--rw-r--r--   0 root         (0) root         (0)     1390 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4118 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/meta/fuse.py
--rw-r--r--   0 root         (0) root         (0)     4386 2023-04-25 17:07:40.000000 fastestimator-1.5.1/fastestimator/op/numpyop/meta/one_of.py
--rw-r--r--   0 root         (0) root         (0)     5873 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/meta/repeat.py
--rw-r--r--   0 root         (0) root         (0)     4997 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/meta/sometimes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:12.529198 fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/
--rw-r--r--   0 root         (0) root         (0)     5956 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7544 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/affine.py
--rw-r--r--   0 root         (0) root         (0)     4466 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/center_crop.py
--rw-r--r--   0 root         (0) root         (0)     4639 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/crop.py
--rw-r--r--   0 root         (0) root         (0)     5041 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/crop_non_empty_mask_if_exists.py
--rw-r--r--   0 root         (0) root         (0)     4920 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/elastic_transform.py
--rw-r--r--   0 root         (0) root         (0)     4292 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/flip.py
--rw-r--r--   0 root         (0) root         (0)     4545 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/grid_distortion.py
--rw-r--r--   0 root         (0) root         (0)     4284 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/horizontal_flip.py
--rw-r--r--   0 root         (0) root         (0)     4568 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/iaa_crop_and_pad.py
--rw-r--r--   0 root         (0) root         (0)     4797 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/longest_max_size.py
--rw-r--r--   0 root         (0) root         (0)     4014 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/mask_dropout.py
--rw-r--r--   0 root         (0) root         (0)     6019 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/multivariate.py
--rw-r--r--   0 root         (0) root         (0)     4665 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/optical_distortion.py
--rw-r--r--   0 root         (0) root         (0)     5191 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/pad_if_needed.py
--rw-r--r--   0 root         (0) root         (0)     4439 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/random_crop.py
--rw-r--r--   0 root         (0) root         (0)     4680 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/random_crop_near_bbox.py
--rw-r--r--   0 root         (0) root         (0)     3406 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/random_grid_shuffle.py
--rw-r--r--   0 root         (0) root         (0)     5091 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/random_resized_crop.py
--rw-r--r--   0 root         (0) root         (0)     4294 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/random_rotate_90.py
--rw-r--r--   0 root         (0) root         (0)     4887 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/random_scale.py
--rw-r--r--   0 root         (0) root         (0)     4454 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/random_sized_bbox_safe_crop.py
--rw-r--r--   0 root         (0) root         (0)     5023 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/random_sized_crop.py
--rw-r--r--   0 root         (0) root         (0)     3034 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/read_mat.py
--rw-r--r--   0 root         (0) root         (0)     4755 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/resize.py
--rw-r--r--   0 root         (0) root         (0)     5430 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/rotate.py
--rw-r--r--   0 root         (0) root         (0)     6176 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/shift_scale_rotate.py
--rw-r--r--   0 root         (0) root         (0)     4818 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/smallest_max_size.py
--rw-r--r--   0 root         (0) root         (0)     4306 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/transpose.py
--rw-r--r--   0 root         (0) root         (0)     4308 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/vertical_flip.py
--rw-r--r--   0 root         (0) root         (0)    16413 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/numpyop.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:13.203748 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/
--rw-r--r--   0 root         (0) root         (0)    10320 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2760 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/autocontrast.py
--rw-r--r--   0 root         (0) root         (0)     2280 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/binarize.py
--rw-r--r--   0 root         (0) root         (0)     2245 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/blur.py
--rw-r--r--   0 root         (0) root         (0)     3497 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/brightness.py
--rw-r--r--   0 root         (0) root         (0)     3718 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/calibate.py
--rw-r--r--   0 root         (0) root         (0)     2494 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/channel_dropout.py
--rw-r--r--   0 root         (0) root         (0)     2089 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/channel_shuffle.py
--rw-r--r--   0 root         (0) root         (0)     2287 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/channel_transpose.py
--rw-r--r--   0 root         (0) root         (0)     2580 2023-04-24 02:38:59.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/clahe.py
--rw-r--r--   0 root         (0) root         (0)     3349 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/coarse_dropout.py
--rw-r--r--   0 root         (0) root         (0)     3488 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/color.py
--rw-r--r--   0 root         (0) root         (0)     3208 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/color_jitter.py
--rw-r--r--   0 root         (0) root         (0)     3488 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/contrast.py
--rw-r--r--   0 root         (0) root         (0)     2563 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/downscale.py
--rw-r--r--   0 root         (0) root         (0)     2864 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/equalize.py
--rw-r--r--   0 root         (0) root         (0)     2256 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/expand_dims.py
--rw-r--r--   0 root         (0) root         (0)     2551 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/from_float.py
--rw-r--r--   0 root         (0) root         (0)     2761 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/gaussian_blur.py
--rw-r--r--   0 root         (0) root         (0)     2672 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/gaussian_noise.py
--rw-r--r--   0 root         (0) root         (0)     3575 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/hadamard.py
--rw-r--r--   0 root         (0) root         (0)     3064 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/hue_saturation_value.py
--rw-r--r--   0 root         (0) root         (0)     2520 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/iaa_additive_gaussian_noise.py
--rw-r--r--   0 root         (0) root         (0)     2812 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/image_compression.py
--rw-r--r--   0 root         (0) root         (0)     2078 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/invert_img.py
--rw-r--r--   0 root         (0) root         (0)     2562 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/iso_noise.py
--rw-r--r--   0 root         (0) root         (0)     2473 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/median_blur.py
--rw-r--r--   0 root         (0) root         (0)     2497 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/minmax.py
--rw-r--r--   0 root         (0) root         (0)     2381 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/motion_blur.py
--rw-r--r--   0 root         (0) root         (0)     3004 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/multiplicative_noise.py
--rw-r--r--   0 root         (0) root         (0)     2615 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/normalize.py
--rw-r--r--   0 root         (0) root         (0)     3310 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/onehot.py
--rw-r--r--   0 root         (0) root         (0)     3155 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/pad_sequence.py
--rw-r--r--   0 root         (0) root         (0)     2708 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/posterize.py
--rw-r--r--   0 root         (0) root         (0)     3022 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/random_brightness_contrast.py
--rw-r--r--   0 root         (0) root         (0)     2687 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/random_fog.py
--rw-r--r--   0 root         (0) root         (0)     2508 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/random_gamma.py
--rw-r--r--   0 root         (0) root         (0)     3433 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/random_rain.py
--rw-r--r--   0 root         (0) root         (0)     3368 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/random_shadow.py
--rw-r--r--   0 root         (0) root         (0)     5438 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/random_shapes.py
--rw-r--r--   0 root         (0) root         (0)     2744 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/random_snow.py
--rw-r--r--   0 root         (0) root         (0)     3585 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/random_sun_flare.py
--rw-r--r--   0 root         (0) root         (0)     3696 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/read_image.py
--rw-r--r--   0 root         (0) root         (0)     2424 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/reshape.py
--rw-r--r--   0 root         (0) root         (0)     3017 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/rgb_shift.py
--rw-r--r--   0 root         (0) root         (0)    23957 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/rua.py
--rw-r--r--   0 root         (0) root         (0)     3546 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/sharpness.py
--rw-r--r--   0 root         (0) root         (0)     3808 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/shear_x.py
--rw-r--r--   0 root         (0) root         (0)     3809 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/shear_y.py
--rw-r--r--   0 root         (0) root         (0)     2407 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/solarize.py
--rw-r--r--   0 root         (0) root         (0)     2367 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/to_array.py
--rw-r--r--   0 root         (0) root         (0)     2396 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/to_float.py
--rw-r--r--   0 root         (0) root         (0)     2138 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/to_gray.py
--rw-r--r--   0 root         (0) root         (0)     2060 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/to_sepia.py
--rw-r--r--   0 root         (0) root         (0)     3114 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/tokenize.py
--rw-r--r--   0 root         (0) root         (0)     3709 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/translate_x.py
--rw-r--r--   0 root         (0) root         (0)     3711 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/translate_y.py
--rw-r--r--   0 root         (0) root         (0)     3279 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/univariate.py
--rw-r--r--   0 root         (0) root         (0)     3057 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/numpyop/univariate/word_to_id.py
--rw-r--r--   0 root         (0) root         (0)     6800 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/op.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:13.320328 fastestimator-1.5.1/fastestimator/op/tensorop/
--rw-r--r--   0 root         (0) root         (0)     2454 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2342 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/argmax.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:13.353292 fastestimator-1.5.1/fastestimator/op/tensorop/augmentation/
--rw-r--r--   0 root         (0) root         (0)     1226 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/augmentation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7301 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/augmentation/cutmix_batch.py
--rw-r--r--   0 root         (0) root         (0)     4185 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/augmentation/mixup_batch.py
--rw-r--r--   0 root         (0) root         (0)     2277 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/average.py
--rw-r--r--   0 root         (0) root         (0)     3393 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/dice.py
--rw-r--r--   0 root         (0) root         (0)     3568 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/gather.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:13.399740 fastestimator-1.5.1/fastestimator/op/tensorop/gradient/
--rw-r--r--   0 root         (0) root         (0)     1323 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/gradient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3673 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/gradient/fgsm.py
--rw-r--r--   0 root         (0) root         (0)     4835 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/gradient/gradient.py
--rw-r--r--   0 root         (0) root         (0)     2455 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/gradient/watch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:13.510771 fastestimator-1.5.1/fastestimator/op/tensorop/loss/
--rw-r--r--   0 root         (0) root         (0)     2296 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/loss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5519 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/loss/cross_entropy.py
--rw-r--r--   0 root         (0) root         (0)     3404 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/loss/focal_loss.py
--rw-r--r--   0 root         (0) root         (0)     2522 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/loss/hinge.py
--rw-r--r--   0 root         (0) root         (0)     4060 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/loss/l1_loss.py
--rw-r--r--   0 root         (0) root         (0)     2257 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/loss/l2_regularization.py
--rw-r--r--   0 root         (0) root         (0)     2495 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/loss/loss.py
--rw-r--r--   0 root         (0) root         (0)     2585 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/loss/mean_squared_error.py
--rw-r--r--   0 root         (0) root         (0)     2866 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/loss/mix_loss.py
--rw-r--r--   0 root         (0) root         (0)     9186 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/loss/super_loss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:13.568150 fastestimator-1.5.1/fastestimator/op/tensorop/meta/
--rw-r--r--   0 root         (0) root         (0)     1454 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3687 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/meta/fuse.py
--rw-r--r--   0 root         (0) root         (0)     4517 2023-04-25 17:08:18.000000 fastestimator-1.5.1/fastestimator/op/tensorop/meta/one_of.py
--rw-r--r--   0 root         (0) root         (0)     7965 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/meta/repeat.py
--rw-r--r--   0 root         (0) root         (0)     4195 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/meta/sometimes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:13.602120 fastestimator-1.5.1/fastestimator/op/tensorop/model/
--rw-r--r--   0 root         (0) root         (0)     1176 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10649 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/model/model.py
--rw-r--r--   0 root         (0) root         (0)    11964 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/model/update.py
--rw-r--r--   0 root         (0) root         (0)     2968 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/normalize.py
--rw-r--r--   0 root         (0) root         (0)     2362 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/permute.py
--rw-r--r--   0 root         (0) root         (0)     2385 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/reshape.py
--rw-r--r--   0 root         (0) root         (0)     2720 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/resize3d.py
--rw-r--r--   0 root         (0) root         (0)     5991 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/tensorop.py
--rw-r--r--   0 root         (0) root         (0)     4326 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/op/tensorop/un_hadamard.py
--rw-r--r--   0 root         (0) root         (0)    35452 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:13.633003 fastestimator-1.5.1/fastestimator/schedule/
--rw-r--r--   0 root         (0) root         (0)     1448 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/schedule/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8480 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/schedule/lr_shedule.py
--rw-r--r--   0 root         (0) root         (0)     9875 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/schedule/schedule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:13.675758 fastestimator-1.5.1/fastestimator/search/
--rw-r--r--   0 root         (0) root         (0)     1386 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/search/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5793 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/search/golden_section.py
--rw-r--r--   0 root         (0) root         (0)     3425 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/search/grid_search.py
--rw-r--r--   0 root         (0) root         (0)     9034 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/search/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:13.739724 fastestimator-1.5.1/fastestimator/search/visualize/
--rw-r--r--   0 root         (0) root         (0)     1829 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/search/visualize/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7925 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/search/visualize/cartesian.py
--rw-r--r--   0 root         (0) root         (0)     7666 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/search/visualize/heatmap.py
--rw-r--r--   0 root         (0) root         (0)     4789 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/search/visualize/parallel_coordinate_plot.py
--rw-r--r--   0 root         (0) root         (0)     4977 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/search/visualize/vis_util.py
--rw-r--r--   0 root         (0) root         (0)     3193 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/search/visualize/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:13.781039 fastestimator-1.5.1/fastestimator/summary/
--rw-r--r--   0 root         (0) root         (0)     1621 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/summary/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41578 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/summary/history.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:13.813454 fastestimator-1.5.1/fastestimator/summary/logs/
--rw-r--r--   0 root         (0) root         (0)     1321 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/summary/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8515 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/summary/logs/log_parse.py
--rw-r--r--   0 root         (0) root         (0)    34368 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/summary/logs/log_plot.py
--rw-r--r--   0 root         (0) root         (0)     7620 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/summary/summary.py
--rw-r--r--   0 root         (0) root         (0)    17954 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/summary/system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:13.844353 fastestimator-1.5.1/fastestimator/test/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2840 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/test/nightly_util.py
--rw-r--r--   0 root         (0) root         (0)    10332 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/test/unittest_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:13.864194 fastestimator-1.5.1/fastestimator/trace/
--rw-r--r--   0 root         (0) root         (0)     1410 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:13.929525 fastestimator-1.5.1/fastestimator/trace/adapt/
--rw-r--r--   0 root         (0) root         (0)     1678 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/adapt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3857 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/adapt/early_stopping.py
--rw-r--r--   0 root         (0) root         (0)     5529 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/adapt/lr_scheduler.py
--rw-r--r--   0 root         (0) root         (0)     5503 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/adapt/pbm_calibrator.py
--rw-r--r--   0 root         (0) root         (0)     3590 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/adapt/reduce_lr_on_plateau.py
--rw-r--r--   0 root         (0) root         (0)     3453 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/adapt/terminate_on_nan.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:14.036732 fastestimator-1.5.1/fastestimator/trace/io/
--rw-r--r--   0 root         (0) root         (0)     2227 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4977 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/io/best_model_saver.py
--rw-r--r--   0 root         (0) root         (0)     7098 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/io/csv_logger.py
--rw-r--r--   0 root         (0) root         (0)     3490 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/io/image_saver.py
--rw-r--r--   0 root         (0) root         (0)     3056 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/io/image_viewer.py
--rw-r--r--   0 root         (0) root         (0)     3908 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/io/model_saver.py
--rw-r--r--   0 root         (0) root         (0)     4974 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/io/restore_wizard.py
--rw-r--r--   0 root         (0) root         (0)    25346 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/io/tensorboard.py
--rw-r--r--   0 root         (0) root         (0)    22579 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/io/test_report.py
--rw-r--r--   0 root         (0) root         (0)    41506 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/io/traceability.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:14.058434 fastestimator-1.5.1/fastestimator/trace/meta/
--rw-r--r--   0 root         (0) root         (0)      965 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4238 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/meta/_per_ds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:14.172251 fastestimator-1.5.1/fastestimator/trace/metric/
--rw-r--r--   0 root         (0) root         (0)     2360 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/metric/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4100 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/metric/accuracy.py
--rw-r--r--   0 root         (0) root         (0)    10591 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/metric/bleu_score.py
--rw-r--r--   0 root         (0) root         (0)     5417 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/metric/calibration_error.py
--rw-r--r--   0 root         (0) root         (0)     4839 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/metric/confusion_matrix.py
--rw-r--r--   0 root         (0) root         (0)     3795 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/metric/dice.py
--rw-r--r--   0 root         (0) root         (0)     4950 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/metric/f1_score.py
--rw-r--r--   0 root         (0) root         (0)     5061 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/metric/mcc.py
--rw-r--r--   0 root         (0) root         (0)    18344 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/metric/mean_average_precision.py
--rw-r--r--   0 root         (0) root         (0)     4895 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/metric/precision.py
--rw-r--r--   0 root         (0) root         (0)     4866 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/metric/recall.py
--rw-r--r--   0 root         (0) root         (0)    19578 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/trace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:14.236910 fastestimator-1.5.1/fastestimator/trace/xai/
--rw-r--r--   0 root         (0) root         (0)     1588 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/xai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10667 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/xai/eigen_cam.py
--rw-r--r--   0 root         (0) root         (0)     7808 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/xai/grad_cam.py
--rw-r--r--   0 root         (0) root         (0)     7266 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/xai/instance_tracker.py
--rw-r--r--   0 root         (0) root         (0)     6905 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/xai/label_tracker.py
--rw-r--r--   0 root         (0) root         (0)     9267 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/trace/xai/saliency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:14.337017 fastestimator-1.5.1/fastestimator/util/
--rw-r--r--   0 root         (0) root         (0)     3768 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23214 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/util/base_util.py
--rw-r--r--   0 root         (0) root         (0)     4225 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/util/cli_util.py
--rw-r--r--   0 root         (0) root         (0)     5328 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/util/data.py
--rw-r--r--   0 root         (0) root         (0)    24492 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/util/img_data.py
--rw-r--r--   0 root         (0) root         (0)     8260 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/util/latex_util.py
--rw-r--r--   0 root         (0) root         (0)    57327 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/util/traceability_util.py
--rw-r--r--   0 root         (0) root         (0)    11038 2023-04-24 02:39:00.000000 fastestimator-1.5.1/fastestimator/util/util.py
--rw-r--r--   0 root         (0) root         (0)     5366 2023-04-24 02:39:01.000000 fastestimator-1.5.1/fastestimator/util/wget_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:14.356267 fastestimator-1.5.1/fastestimator/xai/
--rw-r--r--   0 root         (0) root         (0)     1030 2023-04-24 02:39:01.000000 fastestimator-1.5.1/fastestimator/xai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12171 2023-04-24 02:39:01.000000 fastestimator-1.5.1/fastestimator/xai/saliency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:18.306476 fastestimator-1.5.1/fastestimator.egg-info/
--rw-r--r--   0 root         (0) root         (0)      591 2023-04-25 19:11:08.000000 fastestimator-1.5.1/fastestimator.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    34489 2023-04-25 19:11:10.000000 fastestimator-1.5.1/fastestimator.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 19:11:08.000000 fastestimator-1.5.1/fastestimator.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-04-25 19:11:08.000000 fastestimator-1.5.1/fastestimator.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      655 2023-04-25 19:11:08.000000 fastestimator-1.5.1/fastestimator.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-25 19:11:08.000000 fastestimator-1.5.1/fastestimator.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 19:11:18.320177 fastestimator-1.5.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3090 2023-04-24 03:05:56.000000 fastestimator-1.5.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:14.373739 fastestimator-1.5.1/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:14.383049 fastestimator-1.5.1/test/PR_test/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:14.425830 fastestimator-1.5.1/test/PR_test/integration_test/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:14.483659 fastestimator-1.5.1/test/PR_test/integration_test/backend/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/backend/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1665 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/backend/test_get_lr.py
--rw-r--r--   0 root         (0) root         (0)     3584 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/backend/test_save_model_load_model.py
--rw-r--r--   0 root         (0) root         (0)     1694 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/backend/test_set_lr.py
--rw-r--r--   0 root         (0) root         (0)     4617 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/backend/test_update_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:14.516215 fastestimator-1.5.1/test/PR_test/integration_test/cli/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3718 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/cli/test_main.py
--rw-r--r--   0 root         (0) root         (0)     1883 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/cli/test_train.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:14.536076 fastestimator-1.5.1/test/PR_test/integration_test/dataset/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2376 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/dataset/test_batch_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:14.559052 fastestimator-1.5.1/test/PR_test/integration_test/op/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:14.571190 fastestimator-1.5.1/test/PR_test/integration_test/op/numpyop/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/numpyop/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:14.631405 fastestimator-1.5.1/test/PR_test/integration_test/op/numpyop/meta/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/numpyop/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3002 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/numpyop/meta/test_fuse.py
--rw-r--r--   0 root         (0) root         (0)     2190 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/numpyop/meta/test_one_of.py
--rw-r--r--   0 root         (0) root         (0)     1975 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/numpyop/meta/test_repeat.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/numpyop/meta/test_sometimes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:14.656495 fastestimator-1.5.1/test/PR_test/integration_test/op/numpyop/multivariate/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/numpyop/multivariate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1615 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/numpyop/multivariate/test_read_mat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:14.694516 fastestimator-1.5.1/test/PR_test/integration_test/op/numpyop/univariate/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/numpyop/univariate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2342 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/numpyop/univariate/test_hadamard.py
--rw-r--r--   0 root         (0) root         (0)     2054 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/numpyop/univariate/test_read_image.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:14.757984 fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:14.783509 fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/augmentation/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/augmentation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5170 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/augmentation/test_cutmix_batch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:14.832450 fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/gradient/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/gradient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2144 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/gradient/test_fgsm.py
--rw-r--r--   0 root         (0) root         (0)     3632 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/gradient/test_gradientop.py
--rw-r--r--   0 root         (0) root         (0)     2076 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/gradient/test_watch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:14.921383 fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/loss/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/loss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4052 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/loss/test_cross_entropy.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/loss/test_hinge.py
--rw-r--r--   0 root         (0) root         (0)     3804 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/loss/test_l1_loss.py
--rw-r--r--   0 root         (0) root         (0)    10344 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/loss/test_l2_regularization.py
--rw-r--r--   0 root         (0) root         (0)     1810 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/loss/test_mean_squared_error.py
--rw-r--r--   0 root         (0) root         (0)     8515 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/loss/test_super_loss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:14.982949 fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/meta/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2673 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/meta/test_fuse.py
--rw-r--r--   0 root         (0) root         (0)     2632 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/meta/test_one_of.py
--rw-r--r--   0 root         (0) root         (0)     2511 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/meta/test_repeat.py
--rw-r--r--   0 root         (0) root         (0)     2408 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/meta/test_sometimes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:15.020029 fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/model/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7189 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/model/test_modelop.py
--rw-r--r--   0 root         (0) root         (0)    22429 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/model/test_updateop.py
--rw-r--r--   0 root         (0) root         (0)     1592 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/test_argmax.py
--rw-r--r--   0 root         (0) root         (0)     1613 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/test_average.py
--rw-r--r--   0 root         (0) root         (0)     1650 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/test_reshape.py
--rw-r--r--   0 root         (0) root         (0)     4149 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/test_un_hadamard.py
--rw-r--r--   0 root         (0) root         (0)     1190 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/op/test_op.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:15.077229 fastestimator-1.5.1/test/PR_test/integration_test/schedule/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/schedule/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3971 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/schedule/test_arc.py
--rw-r--r--   0 root         (0) root         (0)    13590 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/schedule/test_epoch_scheduler.py
--rw-r--r--   0 root         (0) root         (0)    14280 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/schedule/test_repeat_scheduler.py
--rw-r--r--   0 root         (0) root         (0)     1742 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/schedule/test_schedule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:15.088746 fastestimator-1.5.1/test/PR_test/integration_test/search/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/search/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:15.112275 fastestimator-1.5.1/test/PR_test/integration_test/search/visualize/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/search/visualize/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5667 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/search/visualize/test_visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:15.144527 fastestimator-1.5.1/test/PR_test/integration_test/summary/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/summary/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11980 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/summary/test_history.py
--rw-r--r--   0 root         (0) root         (0)    17978 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/summary/test_system.py
--rw-r--r--   0 root         (0) root         (0)    23833 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/test_estimator.py
--rw-r--r--   0 root         (0) root         (0)    28044 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/test_network.py
--rw-r--r--   0 root         (0) root         (0)    98463 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/test_pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:15.213376 fastestimator-1.5.1/test/PR_test/integration_test/trace/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:15.284346 fastestimator-1.5.1/test/PR_test/integration_test/trace/adapt/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/adapt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2952 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/adapt/test_early_stopping.py
--rw-r--r--   0 root         (0) root         (0)     4333 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/adapt/test_lr_scheduler.py
--rw-r--r--   0 root         (0) root         (0)     3709 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/adapt/test_pbm_calibrator.py
--rw-r--r--   0 root         (0) root         (0)     3934 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/adapt/test_reduce_lr_on_plateau.py
--rw-r--r--   0 root         (0) root         (0)     5057 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/adapt/test_terminate_on_nan.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:15.414444 fastestimator-1.5.1/test/PR_test/integration_test/trace/io/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4498 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/io/test_best_model_saver.py
--rw-r--r--   0 root         (0) root         (0)     2934 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/io/test_csv_logger.py
--rw-r--r--   0 root         (0) root         (0)     2822 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/io/test_image_saver.py
--rw-r--r--   0 root         (0) root         (0)     2021 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/io/test_image_viewer.py
--rw-r--r--   0 root         (0) root         (0)     8180 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/io/test_model_saver.py
--rw-r--r--   0 root         (0) root         (0)     4049 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/io/test_restore_wizard.py
--rw-r--r--   0 root         (0) root         (0)     3114 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/io/test_saliency.py
--rw-r--r--   0 root         (0) root         (0)     8691 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/io/test_tensorboard.py
--rw-r--r--   0 root         (0) root         (0)    13603 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/io/test_test_report.py
--rw-r--r--   0 root         (0) root         (0)     6037 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/io/test_traceability.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:15.535506 fastestimator-1.5.1/test/PR_test/integration_test/trace/metric/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/metric/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4671 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/metric/test_accuracy.py
--rw-r--r--   0 root         (0) root         (0)     3818 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/metric/test_calibration_error.py
--rw-r--r--   0 root         (0) root         (0)     8046 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/metric/test_confusion_matrix.py
--rw-r--r--   0 root         (0) root         (0)     2167 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/metric/test_dice.py
--rw-r--r--   0 root         (0) root         (0)     8699 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/metric/test_f1_score.py
--rw-r--r--   0 root         (0) root         (0)     7268 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/metric/test_mcc.py
--rw-r--r--   0 root         (0) root         (0)     3575 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/metric/test_mean_average_precision.py
--rw-r--r--   0 root         (0) root         (0)     8730 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/metric/test_precision.py
--rw-r--r--   0 root         (0) root         (0)     8644 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/metric/test_recall.py
--rw-r--r--   0 root         (0) root         (0)     2273 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/test_eval_essential.py
--rw-r--r--   0 root         (0) root         (0)     3766 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/test_logger.py
--rw-r--r--   0 root         (0) root         (0)     2273 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/test_test_essential.py
--rw-r--r--   0 root         (0) root         (0)     4778 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/test_trace.py
--rw-r--r--   0 root         (0) root         (0)     2989 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/test_train_essential.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:15.575067 fastestimator-1.5.1/test/PR_test/integration_test/trace/xai/
--rw-r--r--   0 root         (0) root         (0)      702 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/xai/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9440 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/xai/test_instance_tracker.py
--rw-r--r--   0 root         (0) root         (0)     8956 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/trace/xai/test_label_tracker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:15.618921 fastestimator-1.5.1/test/PR_test/integration_test/util/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1938 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/util/test_img_data.py
--rw-r--r--   0 root         (0) root         (0)    11088 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/util/test_traceability_util.py
--rw-r--r--   0 root         (0) root         (0)     6280 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/integration_test/util/test_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:15.628840 fastestimator-1.5.1/test/PR_test/unit_test/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/unit_test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:15.639205 fastestimator-1.5.1/test/PR_test/unit_test/architecture/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/unit_test/architecture/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:15.708056 fastestimator-1.5.1/test/PR_test/unit_test/architecture/pytorch/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/unit_test/architecture/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2991 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/unit_test/architecture/pytorch/test_attention_unet.py
--rw-r--r--   0 root         (0) root         (0)     2086 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/unit_test/architecture/pytorch/test_lenet.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/unit_test/architecture/pytorch/test_resnet9.py
--rw-r--r--   0 root         (0) root         (0)     2514 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/unit_test/architecture/pytorch/test_unet.py
--rw-r--r--   0 root         (0) root         (0)     1225 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/unit_test/architecture/pytorch/test_wideresnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:15.776245 fastestimator-1.5.1/test/PR_test/unit_test/architecture/tensorflow/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/unit_test/architecture/tensorflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2280 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/unit_test/architecture/tensorflow/test_attention_unet.py
--rw-r--r--   0 root         (0) root         (0)     2180 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/unit_test/architecture/tensorflow/test_lenet.py
--rw-r--r--   0 root         (0) root         (0)     2143 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/unit_test/architecture/tensorflow/test_resnet9.py
--rw-r--r--   0 root         (0) root         (0)     2174 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/unit_test/architecture/tensorflow/test_unet.py
--rw-r--r--   0 root         (0) root         (0)     1280 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/unit_test/architecture/tensorflow/test_wideresnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:16.364799 fastestimator-1.5.1/test/PR_test/unit_test/backend/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1451 2023-04-24 02:39:01.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_abs.py
--rw-r--r--   0 root         (0) root         (0)     2269 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_argmax.py
--rw-r--r--   0 root         (0) root         (0)     6396 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_binary_crossentropy.py
--rw-r--r--   0 root         (0) root         (0)     2682 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_cast.py
--rw-r--r--   0 root         (0) root         (0)     6604 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_categorical_crossentropy.py
--rw-r--r--   0 root         (0) root         (0)     2531 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_check_nan.py
--rw-r--r--   0 root         (0) root         (0)     2812 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_clip_by_value.py
--rw-r--r--   0 root         (0) root         (0)     2477 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_concat.py
--rw-r--r--   0 root         (0) root         (0)     3920 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_dice_score.py
--rw-r--r--   0 root         (0) root         (0)     1471 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_exp.py
--rw-r--r--   0 root         (0) root         (0)     2267 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_expand_dims.py
--rw-r--r--   0 root         (0) root         (0)     1475 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_feed_forward.py
--rw-r--r--   0 root         (0) root         (0)     2499 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_gather.py
--rw-r--r--   0 root         (0) root         (0)     3014 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_gather_from_batch.py
--rwxr-xr-x   0 root         (0) root         (0)     3742 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_get_gradient.py
--rw-r--r--   0 root         (0) root         (0)     1499 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_get_image_dims.py
--rw-r--r--   0 root         (0) root         (0)     1657 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_hinge.py
--rw-r--r--   0 root         (0) root         (0)     5710 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_iwd.py
--rw-r--r--   0 root         (0) root         (0)     1939 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_lambertw.py
--rw-r--r--   0 root         (0) root         (0)     1518 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_matmul.py
--rw-r--r--   0 root         (0) root         (0)     1479 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_maximum.py
--rw-r--r--   0 root         (0) root         (0)     1824 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_mean_squared_error.py
--rw-r--r--   0 root         (0) root         (0)     1596 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_ones_like.py
--rw-r--r--   0 root         (0) root         (0)     9198 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_percentile.py
--rw-r--r--   0 root         (0) root         (0)     2662 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_permute.py
--rw-r--r--   0 root         (0) root         (0)     1466 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_pow.py
--rw-r--r--   0 root         (0) root         (0)     2211 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_random_normal_like.py
--rw-r--r--   0 root         (0) root         (0)     2225 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_random_uniform_like.py
--rw-r--r--   0 root         (0) root         (0)     1964 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_reduce_max.py
--rw-r--r--   0 root         (0) root         (0)     1979 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_reduce_mean.py
--rw-r--r--   0 root         (0) root         (0)     1960 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_reduce_min.py
--rw-r--r--   0 root         (0) root         (0)     1909 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_reduce_std.py
--rw-r--r--   0 root         (0) root         (0)     1958 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_reduce_sum.py
--rw-r--r--   0 root         (0) root         (0)     1926 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_reshape.py
--rw-r--r--   0 root         (0) root         (0)     2645 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_resize3d.py
--rw-r--r--   0 root         (0) root         (0)     3089 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_roll.py
--rw-r--r--   0 root         (0) root         (0)     2029 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_sign.py
--rw-r--r--   0 root         (0) root         (0)     3546 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_sparse_categorical_crossentropy.py
--rw-r--r--   0 root         (0) root         (0)     2305 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_squeeze.py
--rw-r--r--   0 root         (0) root         (0)     2520 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_tensor_normalize.py
--rw-r--r--   0 root         (0) root         (0)     2536 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_tensor_pow.py
--rw-r--r--   0 root         (0) root         (0)     2182 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_tensor_round.py
--rw-r--r--   0 root         (0) root         (0)     2202 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_tensor_sqrt.py
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_to_shape.py
--rw-r--r--   0 root         (0) root         (0)     3038 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_to_tensor.py
--rw-r--r--   0 root         (0) root         (0)     2509 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_to_type.py
--rw-r--r--   0 root         (0) root         (0)     1499 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_transpose.py
--rw-r--r--   0 root         (0) root         (0)     1600 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_watch.py
--rw-r--r--   0 root         (0) root         (0)     1604 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_zeros_like.py
--rw-r--r--   0 root         (0) root         (0)     1463 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/backend/test_zscore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:16.386642 fastestimator-1.5.1/test/PR_test/unit_test/cli/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1494 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/cli/test_cli_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:16.536054 fastestimator-1.5.1/test/PR_test/unit_test/dataset/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1534 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/dataset/test_batch_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1215 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/dataset/test_csv_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2420 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/dataset/test_data.py
--rw-r--r--   0 root         (0) root         (0)     1383 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/dataset/test_dir_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1559 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/dataset/test_extend_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1076 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/dataset/test_generator_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1393 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/dataset/test_labeled_dir_dataset.py
--rw-r--r--   0 root         (0) root         (0)    13000 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/dataset/test_numpy_dataset.py
--rw-r--r--   0 root         (0) root         (0)      983 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/dataset/test_pickle_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1517 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/dataset/test_siamese_dir_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:16.549275 fastestimator-1.5.1/test/PR_test/unit_test/layers/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/layers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:16.583812 fastestimator-1.5.1/test/PR_test/unit_test/layers/pytorch/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/layers/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1675 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/layers/pytorch/test_cropping_2d.py
--rw-r--r--   0 root         (0) root         (0)     3029 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/layers/pytorch/test_hadamard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:16.633069 fastestimator-1.5.1/test/PR_test/unit_test/layers/tensorflow/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/layers/tensorflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2903 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/layers/tensorflow/test_hadamard.py
--rw-r--r--   0 root         (0) root         (0)     1157 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/layers/tensorflow/test_instance_norm.py
--rw-r--r--   0 root         (0) root         (0)     1628 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/layers/tensorflow/test_reflection_padding_2d.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:16.655660 fastestimator-1.5.1/test/PR_test/unit_test/op/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:16.692783 fastestimator-1.5.1/test/PR_test/unit_test/op/loss/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/loss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3752 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/loss/test_focal_loss.py
--rw-r--r--   0 root         (0) root         (0)     1749 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/loss/test_mix_loss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:16.716791 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:16.781592 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/meta/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1864 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/meta/test_fuse.py
--rw-r--r--   0 root         (0) root         (0)     3212 2023-04-25 17:11:51.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/meta/test_one_of.py
--rw-r--r--   0 root         (0) root         (0)     5323 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/meta/test_repeat.py
--rw-r--r--   0 root         (0) root         (0)     2117 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/meta/test_sometimes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:17.143054 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2012 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_affine.py
--rw-r--r--   0 root         (0) root         (0)     2092 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_center_crop.py
--rw-r--r--   0 root         (0) root         (0)     2122 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_crop.py
--rw-r--r--   0 root         (0) root         (0)     1590 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_crop_non_empy_mask_if_exists.py
--rw-r--r--   0 root         (0) root         (0)     2057 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_elastic_transform.py
--rw-r--r--   0 root         (0) root         (0)     1989 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_flip.py
--rw-r--r--   0 root         (0) root         (0)     2053 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_grid_distortion.py
--rw-r--r--   0 root         (0) root         (0)     2073 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_horizontal_flip.py
--rw-r--r--   0 root         (0) root         (0)     2049 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_iaa_crop_and_pad.py
--rw-r--r--   0 root         (0) root         (0)     2109 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_longest_max_size.py
--rw-r--r--   0 root         (0) root         (0)     2157 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_mask_dropout.py
--rw-r--r--   0 root         (0) root         (0)     2097 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_optical_distortion.py
--rw-r--r--   0 root         (0) root         (0)     2021 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_pad_if_needed.py
--rw-r--r--   0 root         (0) root         (0)     2160 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop.py
--rw-r--r--   0 root         (0) root         (0)     1820 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop_near_bbox.py
--rw-r--r--   0 root         (0) root         (0)     2073 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_random_grid_shuffle.py
--rw-r--r--   0 root         (0) root         (0)     2196 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_random_resized_crop.py
--rw-r--r--   0 root         (0) root         (0)     2065 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_random_rotate_90.py
--rw-r--r--   0 root         (0) root         (0)     1653 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_random_scale.py
--rw-r--r--   0 root         (0) root         (0)     2851 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_bbox_safe_crop.py
--rw-r--r--   0 root         (0) root         (0)     2390 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_crop.py
--rw-r--r--   0 root         (0) root         (0)     2128 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_resize.py
--rw-r--r--   0 root         (0) root         (0)     2005 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_rotate.py
--rw-r--r--   0 root         (0) root         (0)     2057 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_shift_scale_rotate.py
--rw-r--r--   0 root         (0) root         (0)     2123 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_smallest_max_size.py
--rw-r--r--   0 root         (0) root         (0)     2029 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_transpose.py
--rw-r--r--   0 root         (0) root         (0)     2057 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_vertical_flip.py
--rw-r--r--   0 root         (0) root         (0)     1494 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/test_numpyop.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:17.838417 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2165 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_autocontrast.py
--rw-r--r--   0 root         (0) root         (0)     1591 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_binarize.py
--rw-r--r--   0 root         (0) root         (0)     1970 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_blur.py
--rw-r--r--   0 root         (0) root         (0)     2149 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_brightness.py
--rw-r--r--   0 root         (0) root         (0)     2644 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_calibrate.py
--rw-r--r--   0 root         (0) root         (0)     2054 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_channel_dropout.py
--rw-r--r--   0 root         (0) root         (0)     2054 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_channel_shuffle.py
--rw-r--r--   0 root         (0) root         (0)     2061 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_channel_transpose.py
--rw-r--r--   0 root         (0) root         (0)     2093 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_clahe.py
--rw-r--r--   0 root         (0) root         (0)     2037 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_coarse_dropout.py
--rw-r--r--   0 root         (0) root         (0)     2109 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_color.py
--rw-r--r--   0 root         (0) root         (0)     2078 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_color_jitter.py
--rw-r--r--   0 root         (0) root         (0)     2133 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_contrast.py
--rw-r--r--   0 root         (0) root         (0)     2001 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_downscale.py
--rw-r--r--   0 root         (0) root         (0)     2117 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_equalize.py
--rw-r--r--   0 root         (0) root         (0)     1602 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_expand_dims.py
--rw-r--r--   0 root         (0) root         (0)     2001 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_fromfloat.py
--rw-r--r--   0 root         (0) root         (0)     2029 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_blur.py
--rw-r--r--   0 root         (0) root         (0)     2037 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_noise.py
--rw-r--r--   0 root         (0) root         (0)     2181 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_hue_saturation_value.py
--rw-r--r--   0 root         (0) root         (0)     2124 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_iaa_additive_gaussian_noise.py
--rw-r--r--   0 root         (0) root         (0)     2161 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_image_compression.py
--rw-r--r--   0 root         (0) root         (0)     2005 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_invert_img.py
--rw-r--r--   0 root         (0) root         (0)     2117 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_iso_noise.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_median_blur.py
--rw-r--r--   0 root         (0) root         (0)     1559 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_minmax.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_motion_blur.py
--rw-r--r--   0 root         (0) root         (0)     2045 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_multiplicative_noise.py
--rw-r--r--   0 root         (0) root         (0)     2001 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_normalize.py
--rw-r--r--   0 root         (0) root         (0)     1380 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_onehot.py
--rw-r--r--   0 root         (0) root         (0)     2113 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_pad_sequence.py
--rw-r--r--   0 root         (0) root         (0)     2125 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_posterize.py
--rw-r--r--   0 root         (0) root         (0)     2186 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_random_brightness_contrast.py
--rw-r--r--   0 root         (0) root         (0)     2062 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_random_fog.py
--rw-r--r--   0 root         (0) root         (0)     2021 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_random_gamma.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_random_rain.py
--rw-r--r--   0 root         (0) root         (0)     2086 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_random_shadow.py
--rw-r--r--   0 root         (0) root         (0)     3662 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_random_shapes.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_random_snow.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_random_sun_flare.py
--rw-r--r--   0 root         (0) root         (0)     1586 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_reshape.py
--rw-r--r--   0 root         (0) root         (0)     1997 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_rgb_shift.py
--rw-r--r--   0 root         (0) root         (0)     2107 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_rua.py
--rw-r--r--   0 root         (0) root         (0)     2141 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_sharpness.py
--rw-r--r--   0 root         (0) root         (0)     2121 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_shear_x.py
--rw-r--r--   0 root         (0) root         (0)     2121 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_shear_y.py
--rw-r--r--   0 root         (0) root         (0)     2050 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_solarize.py
--rw-r--r--   0 root         (0) root         (0)     1199 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_to_array.py
--rw-r--r--   0 root         (0) root         (0)     2046 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_to_float.py
--rw-r--r--   0 root         (0) root         (0)     2038 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_to_gray.py
--rw-r--r--   0 root         (0) root         (0)     1989 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_to_sepia.py
--rw-r--r--   0 root         (0) root         (0)     2417 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_tokenize.py
--rw-r--r--   0 root         (0) root         (0)     2153 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_translate_x.py
--rw-r--r--   0 root         (0) root         (0)     2153 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_translate_y.py
--rw-r--r--   0 root         (0) root         (0)     2222 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_word_to_id.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:17.874483 fastestimator-1.5.1/test/PR_test/unit_test/op/tensorop/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/tensorop/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:17.899023 fastestimator-1.5.1/test/PR_test/unit_test/op/tensorop/augmentation/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/tensorop/augmentation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4002 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/tensorop/augmentation/test_mixup_batch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:17.968412 fastestimator-1.5.1/test/PR_test/unit_test/op/tensorop/meta/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/tensorop/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2783 2023-04-24 02:39:02.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/tensorop/meta/test_fuse.py
--rw-r--r--   0 root         (0) root         (0)     7141 2023-04-25 17:11:44.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/tensorop/meta/test_one_of.py
--rw-r--r--   0 root         (0) root         (0)    15616 2023-04-24 02:39:03.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/tensorop/meta/test_repeat.py
--rw-r--r--   0 root         (0) root         (0)     4632 2023-04-24 02:39:03.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/tensorop/meta/test_sometimes.py
--rw-r--r--   0 root         (0) root         (0)     5034 2023-04-24 02:39:03.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/tensorop/test_normalize.py
--rw-r--r--   0 root         (0) root         (0)     1296 2023-04-24 02:39:03.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/tensorop/test_tensorop.py
--rw-r--r--   0 root         (0) root         (0)     2279 2023-04-24 02:39:03.000000 fastestimator-1.5.1/test/PR_test/unit_test/op/test_op.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:18.013970 fastestimator-1.5.1/test/PR_test/unit_test/schedule/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:03.000000 fastestimator-1.5.1/test/PR_test/unit_test/schedule/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1315 2023-04-24 02:39:03.000000 fastestimator-1.5.1/test/PR_test/unit_test/schedule/test_epoch_scheduler.py
--rw-r--r--   0 root         (0) root         (0)     1606 2023-04-24 02:39:03.000000 fastestimator-1.5.1/test/PR_test/unit_test/schedule/test_lr_schedule.py
--rw-r--r--   0 root         (0) root         (0)     1188 2023-04-24 02:39:03.000000 fastestimator-1.5.1/test/PR_test/unit_test/schedule/test_repeat_scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:18.058617 fastestimator-1.5.1/test/PR_test/unit_test/search/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:03.000000 fastestimator-1.5.1/test/PR_test/unit_test/search/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1803 2023-04-24 02:39:03.000000 fastestimator-1.5.1/test/PR_test/unit_test/search/test_golden_section_search.py
--rw-r--r--   0 root         (0) root         (0)     1753 2023-04-24 02:39:03.000000 fastestimator-1.5.1/test/PR_test/unit_test/search/test_grid_search.py
--rw-r--r--   0 root         (0) root         (0)     4279 2023-04-24 02:39:03.000000 fastestimator-1.5.1/test/PR_test/unit_test/search/test_search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:18.093128 fastestimator-1.5.1/test/PR_test/unit_test/summary/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:03.000000 fastestimator-1.5.1/test/PR_test/unit_test/summary/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:18.115691 fastestimator-1.5.1/test/PR_test/unit_test/summary/logs/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:03.000000 fastestimator-1.5.1/test/PR_test/unit_test/summary/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3794 2023-04-24 02:39:03.000000 fastestimator-1.5.1/test/PR_test/unit_test/summary/logs/test_metrics.py
--rw-r--r--   0 root         (0) root         (0)    10448 2023-04-24 02:39:03.000000 fastestimator-1.5.1/test/PR_test/unit_test/summary/test_history.py
--rw-r--r--   0 root         (0) root         (0)     4160 2023-04-24 02:39:03.000000 fastestimator-1.5.1/test/PR_test/unit_test/summary/test_summary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:18.139030 fastestimator-1.5.1/test/PR_test/unit_test/test/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:03.000000 fastestimator-1.5.1/test/PR_test/unit_test/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4942 2023-04-24 02:39:03.000000 fastestimator-1.5.1/test/PR_test/unit_test/test/test_unittest_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:18.150078 fastestimator-1.5.1/test/PR_test/unit_test/trace/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:03.000000 fastestimator-1.5.1/test/PR_test/unit_test/trace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:18.173214 fastestimator-1.5.1/test/PR_test/unit_test/trace/metric/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:03.000000 fastestimator-1.5.1/test/PR_test/unit_test/trace/metric/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3591 2023-04-24 02:39:03.000000 fastestimator-1.5.1/test/PR_test/unit_test/trace/metric/test_bleu_score.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:18.230085 fastestimator-1.5.1/test/PR_test/unit_test/util/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:03.000000 fastestimator-1.5.1/test/PR_test/unit_test/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1278 2023-04-24 02:39:03.000000 fastestimator-1.5.1/test/PR_test/unit_test/util/test_data.py
--rw-r--r--   0 root         (0) root         (0)     5530 2023-04-24 02:39:03.000000 fastestimator-1.5.1/test/PR_test/unit_test/util/test_traceability_util.py
--rw-r--r--   0 root         (0) root         (0)    18690 2023-04-24 02:39:03.000000 fastestimator-1.5.1/test/PR_test/unit_test/util/test_util.py
--rw-r--r--   0 root         (0) root         (0)     1018 2023-04-24 02:39:03.000000 fastestimator-1.5.1/test/PR_test/unit_test/util/test_wget_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:11:18.252082 fastestimator-1.5.1/test/PR_test/unit_test/xai/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:03.000000 fastestimator-1.5.1/test/PR_test/unit_test/xai/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2825 2023-04-24 02:39:03.000000 fastestimator-1.5.1/test/PR_test/unit_test/xai/test_saliency.py
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-24 02:39:03.000000 fastestimator-1.5.1/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1255 2023-04-24 02:39:03.000000 fastestimator-1.5.1/test/run_pr_test.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      591 2023-04-25 20:41:41.000000 fastestimator-1.5.2/PKG-INFO
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5698 2023-04-25 20:02:11.000000 fastestimator-1.5.2/README.md
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3092 2023-04-25 20:40:45.000000 fastestimator-1.5.2/fastestimator/__init__.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/architecture/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1018 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/architecture/__init__.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/architecture/pytorch/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1609 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/architecture/pytorch/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     7452 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/architecture/pytorch/attention_unet.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2898 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/architecture/pytorch/lenet.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4148 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/architecture/pytorch/resnet9.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5889 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/architecture/pytorch/unet.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     6188 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/architecture/pytorch/wideresnet.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/architecture/tensorflow/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1624 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/architecture/tensorflow/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4800 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/architecture/tensorflow/attention_unet.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2216 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/architecture/tensorflow/lenet.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3355 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/architecture/tensorflow/resnet9.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3718 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/architecture/tensorflow/unet.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5580 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/architecture/tensorflow/wideresnet.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/backend/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    10290 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1836 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_abs.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2252 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_argmax.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4939 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_binary_crossentropy.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3876 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_cast.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5024 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_categorical_crossentropy.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1859 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_check_nan.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3294 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_clip_by_value.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2539 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_concat.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1410 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_convert_tensor_precision.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     7734 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_dice_score.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1850 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_exp.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2335 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_expand_dims.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2502 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_feed_forward.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2699 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_flip.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     6244 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_focal_loss.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3148 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_gather.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3421 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_gather_from_batch.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4694 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_get_gradient.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2512 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_get_image_dims.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1895 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_get_lr.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1979 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_get_shape.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2225 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_hinge.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3484 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_huber.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4511 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_iwd.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3161 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_l1_loss.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1797 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_l2_regularization.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4558 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_lambertw.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4420 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_load_model.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2226 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_matmul.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2161 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_maximum.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2788 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_mean_squared_error.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2483 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_ones_like.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5065 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_percentile.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2727 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_permute.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1952 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_pow.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2923 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_random_normal_like.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3005 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_random_uniform_like.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3123 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_reduce_max.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3259 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_reduce_mean.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3159 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_reduce_min.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3199 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_reduce_std.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2997 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_reduce_sum.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3067 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_reshape.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4256 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_resize3d.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3182 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_roll.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4633 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_save_model.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3069 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_set_lr.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1839 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_sign.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3639 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_smooth_l1_loss.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4889 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_sparse_categorical_crossentropy.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2785 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_squeeze.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5661 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_tensor_normalize.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2431 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_tensor_pow.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1994 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_tensor_round.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2070 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_tensor_sqrt.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3832 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_to_shape.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3835 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_to_tensor.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2807 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_to_type.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1948 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_transpose.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5245 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_update_model.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2207 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_watch.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2482 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_zeros_like.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2416 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/backend/_zscore.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/cli/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1618 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/cli/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     8845 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/cli/history.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5358 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/cli/logs.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1843 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/cli/main.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5468 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/cli/plot.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3485 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/cli/run.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     6574 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/cli/train.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/dataset/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2529 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    16449 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/batch_dataset.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1804 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/csv_dataset.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/dataset/data/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1757 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/data/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1566 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/data/breast_cancer.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3396 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/data/cifair10.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2831 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/data/cifair100.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1568 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/data/cifar10.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1915 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/data/cifar100.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5708 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/data/cub200.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3698 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/data/food101.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3712 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/data/horse2zebra.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2174 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/data/imdb_review.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3750 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/data/mendeley.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4011 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/data/mitmovie_ner.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1338 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/data/mnist.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3321 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/data/montgomery.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    10000 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/data/mscoco.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3856 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/data/nih_chestxray.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2643 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/data/omniglot.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3269 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/data/penn_treebank.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2695 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/data/shakespeare.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1195 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/data/skl_digits.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     6097 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/data/svhn.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2827 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/data/svhn_cropped.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3914 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/data/tednmt.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4183 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/data/tiny_imagenet.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5509 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/data/usps.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    20437 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/dataloader.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    25375 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/dataset.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1974 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/dir_dataset.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2263 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/extend_dataset.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4086 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/generator_dataset.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3599 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/labeled_dir_dataset.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1988 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/numpy_dataset.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     8402 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/op_dataset.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1476 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/pickle_dataset.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     9018 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/dataset/siamese_dir_dataset.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    31566 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/estimator.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/layers/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1012 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/layers/__init__.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/layers/pytorch/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1200 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/layers/pytorch/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3887 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/layers/pytorch/cropping_2d.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     6553 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/layers/pytorch/hadamard.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/layers/tensorflow/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1370 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/layers/tensorflow/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     7334 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/layers/tensorflow/hadamard.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2591 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/layers/tensorflow/instance_norm.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2490 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/layers/tensorflow/reflection_padding_2d.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    50615 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/network.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/op/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1152 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/__init__.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/op/numpyop/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1318 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/__init__.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/op/numpyop/meta/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1390 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/meta/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4118 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/meta/fuse.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4386 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/meta/one_of.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5873 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/meta/repeat.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4997 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/meta/sometimes.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5956 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     7544 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/affine.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4466 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/center_crop.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4639 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/crop.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5041 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/crop_non_empty_mask_if_exists.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4920 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/elastic_transform.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4292 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/flip.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4545 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/grid_distortion.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4284 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/horizontal_flip.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4568 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/iaa_crop_and_pad.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4797 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/longest_max_size.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4014 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/mask_dropout.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     6019 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/multivariate.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4665 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/optical_distortion.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5191 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/pad_if_needed.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4439 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/random_crop.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4680 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/random_crop_near_bbox.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3406 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/random_grid_shuffle.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5091 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/random_resized_crop.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4294 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/random_rotate_90.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4887 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/random_scale.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4454 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/random_sized_bbox_safe_crop.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5023 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/random_sized_crop.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3034 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/read_mat.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4755 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/resize.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5430 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/rotate.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     6176 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/shift_scale_rotate.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4818 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/smallest_max_size.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4306 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/transpose.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4308 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/vertical_flip.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    16413 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/numpyop.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    10320 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2760 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/autocontrast.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2280 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/binarize.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2245 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/blur.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3497 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/brightness.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3718 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/calibate.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2494 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/channel_dropout.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2089 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/channel_shuffle.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2287 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/channel_transpose.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2580 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/clahe.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3349 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/coarse_dropout.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3488 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/color.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3208 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/color_jitter.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3488 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/contrast.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2563 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/downscale.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2864 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/equalize.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2256 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/expand_dims.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2551 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/from_float.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2761 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/gaussian_blur.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2672 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/gaussian_noise.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3575 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/hadamard.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3064 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/hue_saturation_value.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2520 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/iaa_additive_gaussian_noise.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2812 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/image_compression.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2078 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/invert_img.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2562 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/iso_noise.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2473 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/median_blur.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2497 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/minmax.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2381 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/motion_blur.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3004 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/multiplicative_noise.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2615 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/normalize.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3310 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/onehot.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3155 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/pad_sequence.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2708 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/posterize.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3022 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/random_brightness_contrast.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2687 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/random_fog.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2508 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/random_gamma.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3433 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/random_rain.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3368 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/random_shadow.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5438 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/random_shapes.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2744 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/random_snow.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3585 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/random_sun_flare.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3696 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/read_image.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2424 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/reshape.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3017 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/rgb_shift.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    23957 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/rua.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3546 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/sharpness.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3808 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/shear_x.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3809 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/shear_y.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2407 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/solarize.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2367 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/to_array.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2396 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/to_float.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2138 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/to_gray.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2060 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/to_sepia.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3114 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/tokenize.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3709 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/translate_x.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3711 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/translate_y.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3279 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/univariate.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3057 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/numpyop/univariate/word_to_id.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     6800 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/op.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/op/tensorop/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2454 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2342 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/argmax.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/op/tensorop/augmentation/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1226 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/augmentation/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     7301 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/augmentation/cutmix_batch.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4185 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/augmentation/mixup_batch.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2277 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/average.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3393 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/dice.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3568 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/gather.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/op/tensorop/gradient/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1323 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/gradient/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3673 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/gradient/fgsm.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4835 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/gradient/gradient.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2455 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/gradient/watch.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/op/tensorop/loss/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2296 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/loss/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5519 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/loss/cross_entropy.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3404 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/loss/focal_loss.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2522 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/loss/hinge.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4060 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/loss/l1_loss.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2257 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/loss/l2_regularization.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2495 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/loss/loss.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2585 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/loss/mean_squared_error.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2866 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/loss/mix_loss.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     9186 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/loss/super_loss.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/op/tensorop/meta/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1454 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/meta/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3687 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/meta/fuse.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4517 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/meta/one_of.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     7965 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/meta/repeat.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4195 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/meta/sometimes.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/op/tensorop/model/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1176 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/model/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    10649 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/model/model.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    11964 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/model/update.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2968 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/normalize.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2362 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/permute.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2385 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/reshape.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2720 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/resize3d.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5991 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/tensorop.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4326 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/op/tensorop/un_hadamard.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    35452 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/pipeline.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/schedule/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1448 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/schedule/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     8480 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/schedule/lr_shedule.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     9875 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/schedule/schedule.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/search/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1386 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/search/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5793 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/search/golden_section.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3425 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/search/grid_search.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     9034 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/search/search.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/search/visualize/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1829 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/search/visualize/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     7925 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/search/visualize/cartesian.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     7666 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/search/visualize/heatmap.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4789 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/search/visualize/parallel_coordinate_plot.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4977 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/search/visualize/vis_util.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3193 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/search/visualize/visualize.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/summary/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1621 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/summary/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    41578 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/summary/history.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/summary/logs/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1321 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/summary/logs/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     8515 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/summary/logs/log_parse.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    34368 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/summary/logs/log_plot.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     7620 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/summary/summary.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    17954 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/summary/system.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/test/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/test/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2840 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/test/nightly_util.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    10332 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/test/unittest_util.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/trace/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1410 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/__init__.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/trace/adapt/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1678 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/adapt/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3857 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/adapt/early_stopping.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5529 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/adapt/lr_scheduler.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5503 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/adapt/pbm_calibrator.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3590 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/adapt/reduce_lr_on_plateau.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3453 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/adapt/terminate_on_nan.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/trace/io/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2227 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/io/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4977 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/io/best_model_saver.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     7098 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/io/csv_logger.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3490 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/io/image_saver.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3056 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/io/image_viewer.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3908 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/io/model_saver.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4974 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/io/restore_wizard.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    25346 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/io/tensorboard.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    22579 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/io/test_report.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    41506 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/io/traceability.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/trace/meta/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      965 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/meta/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4238 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/meta/_per_ds.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/trace/metric/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2360 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/metric/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4100 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/metric/accuracy.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    10591 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/metric/bleu_score.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5417 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/metric/calibration_error.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4839 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/metric/confusion_matrix.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3795 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/metric/dice.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4950 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/metric/f1_score.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5061 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/metric/mcc.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    18344 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/metric/mean_average_precision.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4895 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/metric/precision.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4866 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/metric/recall.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    19578 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/trace.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/trace/xai/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1588 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/xai/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    10667 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/xai/eigen_cam.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     7808 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/xai/grad_cam.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     7266 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/xai/instance_tracker.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     6905 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/xai/label_tracker.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     9267 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/trace/xai/saliency.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/util/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3768 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/util/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    23214 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/util/base_util.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4225 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/util/cli_util.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5328 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/util/data.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    24492 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/util/img_data.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     8260 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/util/latex_util.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    57327 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/util/traceability_util.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    11038 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/util/util.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5366 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/util/wget_util.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator/xai/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1030 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/xai/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    12171 2023-04-25 20:02:11.000000 fastestimator-1.5.2/fastestimator/xai/saliency.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator.egg-info/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      591 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator.egg-info/PKG-INFO
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    34489 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator.egg-info/SOURCES.txt
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)        1 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator.egg-info/dependency_links.txt
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)       63 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator.egg-info/entry_points.txt
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      655 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator.egg-info/requires.txt
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)       19 2023-04-25 20:41:41.000000 fastestimator-1.5.2/fastestimator.egg-info/top_level.txt
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)       38 2023-04-25 20:41:41.000000 fastestimator-1.5.2/setup.cfg
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3090 2023-04-25 20:40:45.000000 fastestimator-1.5.2/setup.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/__init__.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/integration_test/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/__init__.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/integration_test/backend/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/backend/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1665 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/backend/test_get_lr.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3584 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/backend/test_save_model_load_model.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1694 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/backend/test_set_lr.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4617 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/backend/test_update_model.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/integration_test/cli/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/cli/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3718 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/cli/test_main.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1883 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/cli/test_train.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/integration_test/dataset/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/dataset/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2376 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/dataset/test_batch_dataset.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/__init__.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/numpyop/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/numpyop/__init__.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/numpyop/meta/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/numpyop/meta/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3002 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/numpyop/meta/test_fuse.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2190 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/numpyop/meta/test_one_of.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1975 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/numpyop/meta/test_repeat.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1950 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/numpyop/meta/test_sometimes.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/numpyop/multivariate/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/numpyop/multivariate/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1615 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/numpyop/multivariate/test_read_mat.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/numpyop/univariate/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/numpyop/univariate/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2342 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/numpyop/univariate/test_hadamard.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2054 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/numpyop/univariate/test_read_image.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/__init__.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/augmentation/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/augmentation/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5170 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/augmentation/test_cutmix_batch.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/gradient/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/gradient/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2144 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/gradient/test_fgsm.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3632 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/gradient/test_gradientop.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2076 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/gradient/test_watch.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/loss/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/loss/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4052 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/loss/test_cross_entropy.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1836 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/loss/test_hinge.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3804 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/loss/test_l1_loss.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    10344 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/loss/test_l2_regularization.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1810 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/loss/test_mean_squared_error.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     8515 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/loss/test_super_loss.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/meta/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/meta/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2673 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/meta/test_fuse.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2632 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/meta/test_one_of.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2511 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/meta/test_repeat.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2408 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/meta/test_sometimes.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/model/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/model/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     7189 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/model/test_modelop.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    22429 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/model/test_updateop.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1592 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/test_argmax.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1613 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/test_average.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1650 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/test_reshape.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4149 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/test_un_hadamard.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1190 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/op/test_op.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/integration_test/schedule/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/schedule/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3971 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/schedule/test_arc.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    13590 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/schedule/test_epoch_scheduler.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    14280 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/schedule/test_repeat_scheduler.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1742 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/schedule/test_schedule.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/integration_test/search/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/search/__init__.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/integration_test/search/visualize/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/search/visualize/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5667 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/search/visualize/test_visualize.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/integration_test/summary/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/summary/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    11980 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/summary/test_history.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    17978 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/summary/test_system.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    23833 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/test_estimator.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    28044 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/test_network.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    98463 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/test_pipeline.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/__init__.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/adapt/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/adapt/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2952 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/adapt/test_early_stopping.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4333 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/adapt/test_lr_scheduler.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3709 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/adapt/test_pbm_calibrator.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3934 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/adapt/test_reduce_lr_on_plateau.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5057 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/adapt/test_terminate_on_nan.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/io/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/io/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4498 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/io/test_best_model_saver.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2934 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/io/test_csv_logger.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2822 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/io/test_image_saver.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2021 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/io/test_image_viewer.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     8180 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/io/test_model_saver.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4049 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/io/test_restore_wizard.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3114 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/io/test_saliency.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     8691 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/io/test_tensorboard.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    13603 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/io/test_test_report.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     6037 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/io/test_traceability.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/metric/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/metric/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4671 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/metric/test_accuracy.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3818 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/metric/test_calibration_error.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     8046 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/metric/test_confusion_matrix.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2167 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/metric/test_dice.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     8699 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/metric/test_f1_score.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     7268 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/metric/test_mcc.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3575 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/metric/test_mean_average_precision.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     8730 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/metric/test_precision.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     8644 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/metric/test_recall.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2273 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/test_eval_essential.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3766 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/test_logger.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2273 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/test_test_essential.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4778 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/test_trace.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2989 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/test_train_essential.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/xai/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      702 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/xai/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     9440 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/xai/test_instance_tracker.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     8956 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/trace/xai/test_label_tracker.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/integration_test/util/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/util/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1938 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/util/test_img_data.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    11088 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/util/test_traceability_util.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     6280 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/integration_test/util/test_util.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/unit_test/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/__init__.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/unit_test/architecture/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/architecture/__init__.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/unit_test/architecture/pytorch/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/architecture/pytorch/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2991 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/architecture/pytorch/test_attention_unet.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2086 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/architecture/pytorch/test_lenet.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1950 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/architecture/pytorch/test_resnet9.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2514 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/architecture/pytorch/test_unet.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1225 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/architecture/pytorch/test_wideresnet.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/unit_test/architecture/tensorflow/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/architecture/tensorflow/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2280 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/architecture/tensorflow/test_attention_unet.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2180 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/architecture/tensorflow/test_lenet.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2143 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/architecture/tensorflow/test_resnet9.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2174 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/architecture/tensorflow/test_unet.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1280 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/architecture/tensorflow/test_wideresnet.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1451 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_abs.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2269 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_argmax.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     6396 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_binary_crossentropy.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2682 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_cast.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     6604 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_categorical_crossentropy.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2531 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_check_nan.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2812 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_clip_by_value.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2477 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_concat.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3920 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_dice_score.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1471 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_exp.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2267 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_expand_dims.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1475 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_feed_forward.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2499 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_gather.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3014 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_gather_from_batch.py
+-rwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)     3742 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_get_gradient.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1499 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_get_image_dims.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1657 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_hinge.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5710 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_iwd.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1939 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_lambertw.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1518 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_matmul.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1479 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_maximum.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1824 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_mean_squared_error.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1596 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_ones_like.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     9198 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_percentile.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2662 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_permute.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1466 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_pow.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2211 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_random_normal_like.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2225 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_random_uniform_like.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1964 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_reduce_max.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1979 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_reduce_mean.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1960 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_reduce_min.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1909 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_reduce_std.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1958 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_reduce_sum.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1926 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_reshape.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2645 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_resize3d.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3089 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_roll.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2029 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_sign.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3546 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_sparse_categorical_crossentropy.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2305 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_squeeze.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2520 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_tensor_normalize.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2536 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_tensor_pow.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2182 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_tensor_round.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2202 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_tensor_sqrt.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1679 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_to_shape.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3038 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_to_tensor.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2509 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_to_type.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1499 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_transpose.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1600 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_watch.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1604 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_zeros_like.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1463 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/backend/test_zscore.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/unit_test/cli/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/cli/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1494 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/cli/test_cli_util.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/unit_test/dataset/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/dataset/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1534 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/dataset/test_batch_dataset.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1215 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/dataset/test_csv_dataset.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2420 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/dataset/test_data.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1383 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/dataset/test_dir_dataset.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1559 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/dataset/test_extend_dataset.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1076 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/dataset/test_generator_dataset.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1393 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/dataset/test_labeled_dir_dataset.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    13000 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/dataset/test_numpy_dataset.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      983 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/dataset/test_pickle_dataset.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1517 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/dataset/test_siamese_dir_dataset.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/unit_test/layers/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/layers/__init__.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/unit_test/layers/pytorch/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/layers/pytorch/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1675 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/layers/pytorch/test_cropping_2d.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3029 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/layers/pytorch/test_hadamard.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/unit_test/layers/tensorflow/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/layers/tensorflow/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2903 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/layers/tensorflow/test_hadamard.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1157 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/layers/tensorflow/test_instance_norm.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1628 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/layers/tensorflow/test_reflection_padding_2d.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/__init__.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/loss/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/loss/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3752 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/loss/test_focal_loss.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1749 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/loss/test_mix_loss.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/__init__.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/meta/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/meta/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1864 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/meta/test_fuse.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3212 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/meta/test_one_of.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5323 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/meta/test_repeat.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2117 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/meta/test_sometimes.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2012 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_affine.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2092 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_center_crop.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2122 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_crop.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1590 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_crop_non_empy_mask_if_exists.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2057 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_elastic_transform.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1989 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_flip.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2053 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_grid_distortion.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2073 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_horizontal_flip.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2049 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_iaa_crop_and_pad.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2109 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_longest_max_size.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2157 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_mask_dropout.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2097 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_optical_distortion.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2021 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_pad_if_needed.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2160 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1820 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop_near_bbox.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2073 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_random_grid_shuffle.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2196 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_random_resized_crop.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2065 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_random_rotate_90.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1653 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_random_scale.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2851 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_bbox_safe_crop.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2390 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_crop.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2128 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_resize.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2005 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_rotate.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2057 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_shift_scale_rotate.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2123 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_smallest_max_size.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2029 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_transpose.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2057 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_vertical_flip.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1494 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/test_numpyop.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2165 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_autocontrast.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1591 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_binarize.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1970 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_blur.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2149 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_brightness.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2644 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_calibrate.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2054 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_channel_dropout.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2054 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_channel_shuffle.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2061 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_channel_transpose.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2093 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_clahe.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2037 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_coarse_dropout.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2109 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_color.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2078 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_color_jitter.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2133 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_contrast.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2001 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_downscale.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2117 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_equalize.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1602 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_expand_dims.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2001 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_fromfloat.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2029 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_blur.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2037 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_noise.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2181 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_hue_saturation_value.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2124 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_iaa_additive_gaussian_noise.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2161 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_image_compression.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2005 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_invert_img.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2117 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_iso_noise.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2070 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_median_blur.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1559 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_minmax.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2070 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_motion_blur.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2045 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_multiplicative_noise.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2001 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_normalize.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1380 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_onehot.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2113 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_pad_sequence.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2125 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_posterize.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2186 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_random_brightness_contrast.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2062 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_random_fog.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2021 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_random_gamma.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2070 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_random_rain.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2086 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_random_shadow.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3662 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_random_shapes.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2070 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_random_snow.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2106 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_random_sun_flare.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1586 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_reshape.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1997 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_rgb_shift.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2107 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_rua.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2141 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_sharpness.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2121 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_shear_x.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2121 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_shear_y.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2050 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_solarize.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1199 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_to_array.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2046 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_to_float.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2038 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_to_gray.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1989 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_to_sepia.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2417 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_tokenize.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2153 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_translate_x.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2153 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_translate_y.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2222 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_word_to_id.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/tensorop/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/tensorop/__init__.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/tensorop/augmentation/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/tensorop/augmentation/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4002 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/tensorop/augmentation/test_mixup_batch.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/tensorop/meta/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/tensorop/meta/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2783 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/tensorop/meta/test_fuse.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     7141 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/tensorop/meta/test_one_of.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    15616 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/tensorop/meta/test_repeat.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4632 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/tensorop/meta/test_sometimes.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5034 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/tensorop/test_normalize.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1296 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/tensorop/test_tensorop.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2279 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/op/test_op.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/unit_test/schedule/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/schedule/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1315 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/schedule/test_epoch_scheduler.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1606 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/schedule/test_lr_schedule.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1188 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/schedule/test_repeat_scheduler.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/unit_test/search/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/search/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1803 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/search/test_golden_section_search.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1753 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/search/test_grid_search.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4279 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/search/test_search.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/unit_test/summary/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/summary/__init__.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/unit_test/summary/logs/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/summary/logs/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3794 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/summary/logs/test_metrics.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    10448 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/summary/test_history.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4160 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/summary/test_summary.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/unit_test/test/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/test/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     4942 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/test/test_unittest_util.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/unit_test/trace/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/trace/__init__.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/unit_test/trace/metric/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/trace/metric/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     3591 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/trace/metric/test_bleu_score.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/unit_test/util/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/util/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1278 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/util/test_data.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     5530 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/util/test_traceability_util.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)    18690 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/util/test_util.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1018 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/util/test_wget_util.py
+drwxrwxr-x   0 xiaomeng  (1001) xiaomeng  (1001)        0 2023-04-25 20:41:41.000000 fastestimator-1.5.2/test/PR_test/unit_test/xai/
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/xai/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     2825 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/PR_test/unit_test/xai/test_saliency.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)      692 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/__init__.py
+-rw-rw-r--   0 xiaomeng  (1001) xiaomeng  (1001)     1255 2023-04-25 20:02:11.000000 fastestimator-1.5.2/test/run_pr_test.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `fastestimator-1.5.1/PKG-INFO` & `fastestimator-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: fastestimator
-Version: 1.5.1
+Version: 1.5.2
 Summary: Deep learning framework
 Home-page: https://github.com/fastestimator/fastestimator
 Author: FastEstimator Dev
 Author-email: UNKNOWN
 License: Apache License 2.0
 Description: FastEstimator is a high-level deep learning API. With the help of FastEstimator, you can easily                     build a high-performance deep learning model and run it anywhere.
 Keywords: fastestimator tensorflow pytorch
```

### Comparing `fastestimator-1.5.1/README.md` & `fastestimator-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/__init__.py` & `fastestimator-1.5.2/fastestimator/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 if TYPE_CHECKING:
     # Allow IDEs to play nice with lazy loading
     from fastestimator import architecture, backend, dataset, layers, op, schedule, search, summary, trace, util, xai
     from fastestimator.estimator import Estimator, enable_deterministic, record_history
     from fastestimator.network import Network, build
     from fastestimator.pipeline import Pipeline
 
-__version__ = '1.5.1'
+__version__ = '1.5.2'
 fe_deterministic_seed = None
 fe_history_path = None  # Where to save training histories. None for ~/fastestimator_data/history.db, False to disable
 fe_build_count = 0
 
 # Disable history logging for tests by default (they can still turn it on/off manually in setUpClass/tearDownClass)
 if __name__ != '__main__':
     for frame in inspect.stack()[1:]:
```

### Comparing `fastestimator-1.5.1/fastestimator/architecture/__init__.py` & `fastestimator-1.5.2/fastestimator/architecture/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/architecture/pytorch/__init__.py` & `fastestimator-1.5.2/fastestimator/architecture/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/architecture/pytorch/attention_unet.py` & `fastestimator-1.5.2/fastestimator/architecture/pytorch/attention_unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/architecture/pytorch/lenet.py` & `fastestimator-1.5.2/fastestimator/architecture/pytorch/lenet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/architecture/pytorch/resnet9.py` & `fastestimator-1.5.2/fastestimator/architecture/pytorch/resnet9.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/architecture/pytorch/unet.py` & `fastestimator-1.5.2/fastestimator/architecture/pytorch/unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/architecture/pytorch/wideresnet.py` & `fastestimator-1.5.2/fastestimator/architecture/pytorch/wideresnet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/architecture/tensorflow/__init__.py` & `fastestimator-1.5.2/fastestimator/architecture/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/architecture/tensorflow/attention_unet.py` & `fastestimator-1.5.2/fastestimator/architecture/tensorflow/attention_unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/architecture/tensorflow/lenet.py` & `fastestimator-1.5.2/fastestimator/architecture/tensorflow/lenet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/architecture/tensorflow/resnet9.py` & `fastestimator-1.5.2/fastestimator/architecture/tensorflow/resnet9.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/architecture/tensorflow/unet.py` & `fastestimator-1.5.2/fastestimator/architecture/tensorflow/unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/architecture/tensorflow/wideresnet.py` & `fastestimator-1.5.2/fastestimator/architecture/tensorflow/wideresnet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/__init__.py` & `fastestimator-1.5.2/fastestimator/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_abs.py` & `fastestimator-1.5.2/fastestimator/backend/_abs.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_argmax.py` & `fastestimator-1.5.2/fastestimator/backend/_argmax.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_binary_crossentropy.py` & `fastestimator-1.5.2/fastestimator/backend/_binary_crossentropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_cast.py` & `fastestimator-1.5.2/fastestimator/backend/_cast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_categorical_crossentropy.py` & `fastestimator-1.5.2/fastestimator/backend/_categorical_crossentropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_check_nan.py` & `fastestimator-1.5.2/fastestimator/backend/_check_nan.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_clip_by_value.py` & `fastestimator-1.5.2/fastestimator/backend/_clip_by_value.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_concat.py` & `fastestimator-1.5.2/fastestimator/backend/_concat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_convert_tensor_precision.py` & `fastestimator-1.5.2/fastestimator/backend/_convert_tensor_precision.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_dice_score.py` & `fastestimator-1.5.2/fastestimator/backend/_dice_score.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_exp.py` & `fastestimator-1.5.2/fastestimator/backend/_exp.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_expand_dims.py` & `fastestimator-1.5.2/fastestimator/backend/_expand_dims.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_feed_forward.py` & `fastestimator-1.5.2/fastestimator/backend/_feed_forward.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_flip.py` & `fastestimator-1.5.2/fastestimator/backend/_flip.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_focal_loss.py` & `fastestimator-1.5.2/fastestimator/backend/_focal_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_gather.py` & `fastestimator-1.5.2/fastestimator/backend/_gather.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_gather_from_batch.py` & `fastestimator-1.5.2/fastestimator/backend/_gather_from_batch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_get_gradient.py` & `fastestimator-1.5.2/fastestimator/backend/_get_gradient.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_get_image_dims.py` & `fastestimator-1.5.2/fastestimator/backend/_get_image_dims.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_get_lr.py` & `fastestimator-1.5.2/fastestimator/backend/_get_lr.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_get_shape.py` & `fastestimator-1.5.2/fastestimator/backend/_get_shape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_hinge.py` & `fastestimator-1.5.2/fastestimator/backend/_hinge.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_huber.py` & `fastestimator-1.5.2/fastestimator/backend/_huber.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_iwd.py` & `fastestimator-1.5.2/fastestimator/backend/_iwd.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_l1_loss.py` & `fastestimator-1.5.2/fastestimator/backend/_l1_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_l2_regularization.py` & `fastestimator-1.5.2/fastestimator/backend/_l2_regularization.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_lambertw.py` & `fastestimator-1.5.2/fastestimator/backend/_lambertw.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_load_model.py` & `fastestimator-1.5.2/fastestimator/backend/_load_model.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_matmul.py` & `fastestimator-1.5.2/fastestimator/backend/_matmul.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_maximum.py` & `fastestimator-1.5.2/fastestimator/backend/_maximum.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_mean_squared_error.py` & `fastestimator-1.5.2/fastestimator/backend/_mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_ones_like.py` & `fastestimator-1.5.2/fastestimator/backend/_ones_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_percentile.py` & `fastestimator-1.5.2/fastestimator/backend/_percentile.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_permute.py` & `fastestimator-1.5.2/fastestimator/backend/_permute.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_pow.py` & `fastestimator-1.5.2/fastestimator/backend/_pow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_random_normal_like.py` & `fastestimator-1.5.2/fastestimator/backend/_random_normal_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_random_uniform_like.py` & `fastestimator-1.5.2/fastestimator/backend/_random_uniform_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_reduce_max.py` & `fastestimator-1.5.2/fastestimator/backend/_reduce_max.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_reduce_mean.py` & `fastestimator-1.5.2/fastestimator/backend/_reduce_mean.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_reduce_min.py` & `fastestimator-1.5.2/fastestimator/backend/_reduce_min.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_reduce_std.py` & `fastestimator-1.5.2/fastestimator/backend/_reduce_std.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_reduce_sum.py` & `fastestimator-1.5.2/fastestimator/backend/_reduce_sum.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_reshape.py` & `fastestimator-1.5.2/fastestimator/backend/_reshape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_resize3d.py` & `fastestimator-1.5.2/fastestimator/backend/_resize3d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_roll.py` & `fastestimator-1.5.2/fastestimator/backend/_roll.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_save_model.py` & `fastestimator-1.5.2/fastestimator/backend/_save_model.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_set_lr.py` & `fastestimator-1.5.2/fastestimator/backend/_set_lr.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_sign.py` & `fastestimator-1.5.2/fastestimator/backend/_sign.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_smooth_l1_loss.py` & `fastestimator-1.5.2/fastestimator/backend/_smooth_l1_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_sparse_categorical_crossentropy.py` & `fastestimator-1.5.2/fastestimator/backend/_sparse_categorical_crossentropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_squeeze.py` & `fastestimator-1.5.2/fastestimator/backend/_squeeze.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_tensor_normalize.py` & `fastestimator-1.5.2/fastestimator/backend/_tensor_normalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_tensor_pow.py` & `fastestimator-1.5.2/fastestimator/backend/_tensor_pow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_tensor_round.py` & `fastestimator-1.5.2/fastestimator/backend/_tensor_round.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_tensor_sqrt.py` & `fastestimator-1.5.2/fastestimator/backend/_tensor_sqrt.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_to_shape.py` & `fastestimator-1.5.2/fastestimator/backend/_to_shape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_to_tensor.py` & `fastestimator-1.5.2/fastestimator/backend/_to_tensor.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_to_type.py` & `fastestimator-1.5.2/fastestimator/backend/_to_type.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_transpose.py` & `fastestimator-1.5.2/fastestimator/backend/_transpose.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_update_model.py` & `fastestimator-1.5.2/fastestimator/backend/_update_model.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_watch.py` & `fastestimator-1.5.2/fastestimator/backend/_watch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_zeros_like.py` & `fastestimator-1.5.2/fastestimator/backend/_zeros_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/backend/_zscore.py` & `fastestimator-1.5.2/fastestimator/backend/_zscore.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/cli/__init__.py` & `fastestimator-1.5.2/fastestimator/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/cli/history.py` & `fastestimator-1.5.2/fastestimator/cli/history.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/cli/logs.py` & `fastestimator-1.5.2/fastestimator/cli/logs.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/cli/main.py` & `fastestimator-1.5.2/fastestimator/cli/main.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/cli/plot.py` & `fastestimator-1.5.2/fastestimator/cli/plot.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/cli/run.py` & `fastestimator-1.5.2/fastestimator/cli/run.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/cli/train.py` & `fastestimator-1.5.2/fastestimator/cli/train.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/__init__.py` & `fastestimator-1.5.2/fastestimator/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/batch_dataset.py` & `fastestimator-1.5.2/fastestimator/dataset/batch_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/csv_dataset.py` & `fastestimator-1.5.2/fastestimator/dataset/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/data/__init__.py` & `fastestimator-1.5.2/fastestimator/dataset/data/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/data/breast_cancer.py` & `fastestimator-1.5.2/fastestimator/dataset/data/breast_cancer.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/data/cifair10.py` & `fastestimator-1.5.2/fastestimator/dataset/data/cifair10.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/data/cifair100.py` & `fastestimator-1.5.2/fastestimator/dataset/data/cifair100.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/data/cifar10.py` & `fastestimator-1.5.2/fastestimator/dataset/data/cifar10.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/data/cifar100.py` & `fastestimator-1.5.2/fastestimator/dataset/data/cifar100.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/data/cub200.py` & `fastestimator-1.5.2/fastestimator/dataset/data/cub200.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/data/food101.py` & `fastestimator-1.5.2/fastestimator/dataset/data/food101.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/data/horse2zebra.py` & `fastestimator-1.5.2/fastestimator/dataset/data/horse2zebra.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/data/imdb_review.py` & `fastestimator-1.5.2/fastestimator/dataset/data/imdb_review.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/data/mendeley.py` & `fastestimator-1.5.2/fastestimator/dataset/data/mendeley.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/data/mitmovie_ner.py` & `fastestimator-1.5.2/fastestimator/dataset/data/mitmovie_ner.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/data/mnist.py` & `fastestimator-1.5.2/fastestimator/dataset/data/mnist.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/data/montgomery.py` & `fastestimator-1.5.2/fastestimator/dataset/data/montgomery.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/data/mscoco.py` & `fastestimator-1.5.2/fastestimator/dataset/data/mscoco.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/data/nih_chestxray.py` & `fastestimator-1.5.2/fastestimator/dataset/data/nih_chestxray.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/data/omniglot.py` & `fastestimator-1.5.2/fastestimator/dataset/data/omniglot.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/data/penn_treebank.py` & `fastestimator-1.5.2/fastestimator/dataset/data/penn_treebank.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/data/shakespeare.py` & `fastestimator-1.5.2/fastestimator/dataset/data/shakespeare.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/data/skl_digits.py` & `fastestimator-1.5.2/fastestimator/dataset/data/skl_digits.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/data/svhn.py` & `fastestimator-1.5.2/fastestimator/dataset/data/svhn.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/data/svhn_cropped.py` & `fastestimator-1.5.2/fastestimator/dataset/data/svhn_cropped.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/data/tednmt.py` & `fastestimator-1.5.2/fastestimator/dataset/data/tednmt.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/data/tiny_imagenet.py` & `fastestimator-1.5.2/fastestimator/dataset/data/tiny_imagenet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/data/usps.py` & `fastestimator-1.5.2/fastestimator/dataset/data/usps.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/dataloader.py` & `fastestimator-1.5.2/fastestimator/dataset/dataloader.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/dataset.py` & `fastestimator-1.5.2/fastestimator/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/dir_dataset.py` & `fastestimator-1.5.2/fastestimator/dataset/dir_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/extend_dataset.py` & `fastestimator-1.5.2/fastestimator/dataset/extend_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/generator_dataset.py` & `fastestimator-1.5.2/fastestimator/dataset/generator_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/labeled_dir_dataset.py` & `fastestimator-1.5.2/fastestimator/dataset/labeled_dir_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/numpy_dataset.py` & `fastestimator-1.5.2/fastestimator/dataset/numpy_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/op_dataset.py` & `fastestimator-1.5.2/fastestimator/dataset/op_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/pickle_dataset.py` & `fastestimator-1.5.2/fastestimator/dataset/pickle_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/dataset/siamese_dir_dataset.py` & `fastestimator-1.5.2/fastestimator/dataset/siamese_dir_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/estimator.py` & `fastestimator-1.5.2/fastestimator/estimator.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/layers/__init__.py` & `fastestimator-1.5.2/fastestimator/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/layers/pytorch/__init__.py` & `fastestimator-1.5.2/fastestimator/layers/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/layers/pytorch/cropping_2d.py` & `fastestimator-1.5.2/fastestimator/layers/pytorch/cropping_2d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/layers/pytorch/hadamard.py` & `fastestimator-1.5.2/fastestimator/layers/pytorch/hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/layers/tensorflow/__init__.py` & `fastestimator-1.5.2/fastestimator/layers/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/layers/tensorflow/hadamard.py` & `fastestimator-1.5.2/fastestimator/layers/tensorflow/hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/layers/tensorflow/instance_norm.py` & `fastestimator-1.5.2/fastestimator/layers/tensorflow/instance_norm.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/layers/tensorflow/reflection_padding_2d.py` & `fastestimator-1.5.2/fastestimator/layers/tensorflow/reflection_padding_2d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/network.py` & `fastestimator-1.5.2/fastestimator/network.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/__init__.py` & `fastestimator-1.5.2/fastestimator/op/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/__init__.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/meta/__init__.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/meta/fuse.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/meta/fuse.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/meta/one_of.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/meta/one_of.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/meta/repeat.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/meta/repeat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/meta/sometimes.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/meta/sometimes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/__init__.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/affine.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/affine.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/center_crop.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/center_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/crop.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/crop_non_empty_mask_if_exists.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/crop_non_empty_mask_if_exists.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/elastic_transform.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/elastic_transform.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/flip.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/flip.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/grid_distortion.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/grid_distortion.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/horizontal_flip.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/horizontal_flip.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/iaa_crop_and_pad.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/iaa_crop_and_pad.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/longest_max_size.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/longest_max_size.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/mask_dropout.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/mask_dropout.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/multivariate.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/multivariate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/optical_distortion.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/optical_distortion.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/pad_if_needed.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/pad_if_needed.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/random_crop.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/random_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/random_crop_near_bbox.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/random_crop_near_bbox.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/random_grid_shuffle.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/random_grid_shuffle.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/random_resized_crop.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/random_resized_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/random_rotate_90.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/random_rotate_90.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/random_scale.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/random_scale.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/random_sized_bbox_safe_crop.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/random_sized_bbox_safe_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/random_sized_crop.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/random_sized_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/read_mat.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/read_mat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/resize.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/resize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/rotate.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/rotate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/shift_scale_rotate.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/shift_scale_rotate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/smallest_max_size.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/smallest_max_size.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/transpose.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/transpose.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/multivariate/vertical_flip.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/multivariate/vertical_flip.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/numpyop.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/numpyop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/__init__.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/autocontrast.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/autocontrast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/binarize.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/binarize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/blur.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/brightness.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/brightness.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/calibate.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/calibate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/channel_dropout.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/channel_dropout.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/channel_shuffle.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/channel_shuffle.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/channel_transpose.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/channel_transpose.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/clahe.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/clahe.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/coarse_dropout.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/coarse_dropout.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/color.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/color.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/color_jitter.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/color_jitter.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/contrast.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/contrast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/downscale.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/downscale.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/equalize.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/equalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/expand_dims.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/expand_dims.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/from_float.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/from_float.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/gaussian_blur.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/gaussian_blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/gaussian_noise.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/hadamard.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/hue_saturation_value.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/hue_saturation_value.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/iaa_additive_gaussian_noise.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/iaa_additive_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/image_compression.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/image_compression.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/invert_img.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/invert_img.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/iso_noise.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/iso_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/median_blur.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/median_blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/minmax.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/minmax.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/motion_blur.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/motion_blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/multiplicative_noise.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/multiplicative_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/normalize.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/normalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/onehot.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/onehot.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/pad_sequence.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/pad_sequence.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/posterize.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/posterize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/random_brightness_contrast.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/random_brightness_contrast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/random_fog.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/random_fog.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/random_gamma.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/random_gamma.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/random_rain.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/random_rain.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/random_shadow.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/random_shadow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/random_shapes.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/random_shapes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/random_snow.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/random_snow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/random_sun_flare.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/random_sun_flare.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/read_image.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/read_image.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/reshape.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/reshape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/rgb_shift.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/rgb_shift.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/rua.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/rua.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/sharpness.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/sharpness.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/shear_x.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/shear_x.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/shear_y.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/shear_y.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/solarize.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/solarize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/to_array.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/to_array.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/to_float.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/to_float.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/to_gray.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/to_gray.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/to_sepia.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/to_sepia.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/tokenize.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/tokenize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/translate_x.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/translate_x.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/translate_y.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/translate_y.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/univariate.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/univariate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/numpyop/univariate/word_to_id.py` & `fastestimator-1.5.2/fastestimator/op/numpyop/univariate/word_to_id.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/op.py` & `fastestimator-1.5.2/fastestimator/op/op.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/__init__.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/argmax.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/argmax.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/augmentation/__init__.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/augmentation/cutmix_batch.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/augmentation/cutmix_batch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/augmentation/mixup_batch.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/augmentation/mixup_batch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/average.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/average.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/dice.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/dice.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/gather.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/gather.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/gradient/__init__.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/gradient/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/gradient/fgsm.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/gradient/fgsm.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/gradient/gradient.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/gradient/gradient.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/gradient/watch.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/gradient/watch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/loss/__init__.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/loss/cross_entropy.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/loss/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/loss/focal_loss.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/loss/focal_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/loss/hinge.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/loss/hinge.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/loss/l1_loss.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/loss/l1_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/loss/l2_regularization.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/loss/l2_regularization.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/loss/loss.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/loss/loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/loss/mean_squared_error.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/loss/mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/loss/mix_loss.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/loss/mix_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/loss/super_loss.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/loss/super_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/meta/__init__.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/meta/fuse.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/meta/fuse.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/meta/one_of.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/meta/one_of.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/meta/repeat.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/meta/repeat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/meta/sometimes.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/meta/sometimes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/model/__init__.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/model/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/model/model.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/model/model.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/model/update.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/model/update.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/normalize.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/normalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/permute.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/permute.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/reshape.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/reshape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/resize3d.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/resize3d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/tensorop.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/tensorop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/op/tensorop/un_hadamard.py` & `fastestimator-1.5.2/fastestimator/op/tensorop/un_hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/pipeline.py` & `fastestimator-1.5.2/fastestimator/pipeline.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/schedule/__init__.py` & `fastestimator-1.5.2/fastestimator/schedule/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/schedule/lr_shedule.py` & `fastestimator-1.5.2/fastestimator/schedule/lr_shedule.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/schedule/schedule.py` & `fastestimator-1.5.2/fastestimator/schedule/schedule.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/search/__init__.py` & `fastestimator-1.5.2/fastestimator/search/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/search/golden_section.py` & `fastestimator-1.5.2/fastestimator/search/golden_section.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/search/grid_search.py` & `fastestimator-1.5.2/fastestimator/search/grid_search.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/search/search.py` & `fastestimator-1.5.2/fastestimator/search/search.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/search/visualize/__init__.py` & `fastestimator-1.5.2/fastestimator/search/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/search/visualize/cartesian.py` & `fastestimator-1.5.2/fastestimator/search/visualize/cartesian.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/search/visualize/heatmap.py` & `fastestimator-1.5.2/fastestimator/search/visualize/heatmap.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/search/visualize/parallel_coordinate_plot.py` & `fastestimator-1.5.2/fastestimator/search/visualize/parallel_coordinate_plot.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/search/visualize/vis_util.py` & `fastestimator-1.5.2/fastestimator/search/visualize/vis_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/search/visualize/visualize.py` & `fastestimator-1.5.2/fastestimator/search/visualize/visualize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/summary/__init__.py` & `fastestimator-1.5.2/fastestimator/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/summary/history.py` & `fastestimator-1.5.2/fastestimator/summary/history.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/summary/logs/__init__.py` & `fastestimator-1.5.2/fastestimator/summary/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/summary/logs/log_parse.py` & `fastestimator-1.5.2/fastestimator/summary/logs/log_parse.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/summary/logs/log_plot.py` & `fastestimator-1.5.2/fastestimator/summary/logs/log_plot.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/summary/summary.py` & `fastestimator-1.5.2/fastestimator/summary/summary.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/summary/system.py` & `fastestimator-1.5.2/fastestimator/summary/system.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/test/__init__.py` & `fastestimator-1.5.2/fastestimator/test/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/test/nightly_util.py` & `fastestimator-1.5.2/fastestimator/test/nightly_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/test/unittest_util.py` & `fastestimator-1.5.2/fastestimator/test/unittest_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/__init__.py` & `fastestimator-1.5.2/fastestimator/trace/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/adapt/__init__.py` & `fastestimator-1.5.2/fastestimator/trace/adapt/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/adapt/early_stopping.py` & `fastestimator-1.5.2/fastestimator/trace/adapt/early_stopping.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/adapt/lr_scheduler.py` & `fastestimator-1.5.2/fastestimator/trace/adapt/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/adapt/pbm_calibrator.py` & `fastestimator-1.5.2/fastestimator/trace/adapt/pbm_calibrator.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/adapt/reduce_lr_on_plateau.py` & `fastestimator-1.5.2/fastestimator/trace/adapt/reduce_lr_on_plateau.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/adapt/terminate_on_nan.py` & `fastestimator-1.5.2/fastestimator/trace/adapt/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/io/__init__.py` & `fastestimator-1.5.2/fastestimator/trace/io/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/io/best_model_saver.py` & `fastestimator-1.5.2/fastestimator/trace/io/best_model_saver.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/io/csv_logger.py` & `fastestimator-1.5.2/fastestimator/trace/io/csv_logger.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/io/image_saver.py` & `fastestimator-1.5.2/fastestimator/trace/io/image_saver.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/io/image_viewer.py` & `fastestimator-1.5.2/fastestimator/trace/io/image_viewer.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/io/model_saver.py` & `fastestimator-1.5.2/fastestimator/trace/io/model_saver.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/io/restore_wizard.py` & `fastestimator-1.5.2/fastestimator/trace/io/restore_wizard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/io/tensorboard.py` & `fastestimator-1.5.2/fastestimator/trace/io/tensorboard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/io/test_report.py` & `fastestimator-1.5.2/fastestimator/trace/io/test_report.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/io/traceability.py` & `fastestimator-1.5.2/fastestimator/trace/io/traceability.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/meta/__init__.py` & `fastestimator-1.5.2/fastestimator/trace/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/meta/_per_ds.py` & `fastestimator-1.5.2/fastestimator/trace/meta/_per_ds.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/metric/__init__.py` & `fastestimator-1.5.2/fastestimator/trace/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/metric/accuracy.py` & `fastestimator-1.5.2/fastestimator/trace/metric/accuracy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/metric/bleu_score.py` & `fastestimator-1.5.2/fastestimator/trace/metric/bleu_score.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/metric/calibration_error.py` & `fastestimator-1.5.2/fastestimator/trace/metric/calibration_error.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/metric/confusion_matrix.py` & `fastestimator-1.5.2/fastestimator/trace/metric/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/metric/dice.py` & `fastestimator-1.5.2/fastestimator/trace/metric/dice.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/metric/f1_score.py` & `fastestimator-1.5.2/fastestimator/trace/metric/f1_score.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/metric/mcc.py` & `fastestimator-1.5.2/fastestimator/trace/metric/mcc.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/metric/mean_average_precision.py` & `fastestimator-1.5.2/fastestimator/trace/metric/mean_average_precision.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/metric/precision.py` & `fastestimator-1.5.2/fastestimator/trace/metric/precision.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/metric/recall.py` & `fastestimator-1.5.2/fastestimator/trace/metric/recall.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/trace.py` & `fastestimator-1.5.2/fastestimator/trace/trace.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/xai/__init__.py` & `fastestimator-1.5.2/fastestimator/trace/xai/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/xai/eigen_cam.py` & `fastestimator-1.5.2/fastestimator/trace/xai/eigen_cam.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/xai/grad_cam.py` & `fastestimator-1.5.2/fastestimator/trace/xai/grad_cam.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/xai/instance_tracker.py` & `fastestimator-1.5.2/fastestimator/trace/xai/instance_tracker.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/xai/label_tracker.py` & `fastestimator-1.5.2/fastestimator/trace/xai/label_tracker.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/trace/xai/saliency.py` & `fastestimator-1.5.2/fastestimator/trace/xai/saliency.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/util/__init__.py` & `fastestimator-1.5.2/fastestimator/util/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/util/base_util.py` & `fastestimator-1.5.2/fastestimator/util/base_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/util/cli_util.py` & `fastestimator-1.5.2/fastestimator/util/cli_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/util/data.py` & `fastestimator-1.5.2/fastestimator/util/data.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/util/img_data.py` & `fastestimator-1.5.2/fastestimator/util/img_data.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/util/latex_util.py` & `fastestimator-1.5.2/fastestimator/util/latex_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/util/traceability_util.py` & `fastestimator-1.5.2/fastestimator/util/traceability_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/util/util.py` & `fastestimator-1.5.2/fastestimator/util/util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/util/wget_util.py` & `fastestimator-1.5.2/fastestimator/util/wget_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/xai/__init__.py` & `fastestimator-1.5.2/fastestimator/xai/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator/xai/saliency.py` & `fastestimator-1.5.2/fastestimator/xai/saliency.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator.egg-info/PKG-INFO` & `fastestimator-1.5.2/fastestimator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: fastestimator
-Version: 1.5.1
+Version: 1.5.2
 Summary: Deep learning framework
 Home-page: https://github.com/fastestimator/fastestimator
 Author: FastEstimator Dev
 Author-email: UNKNOWN
 License: Apache License 2.0
 Description: FastEstimator is a high-level deep learning API. With the help of FastEstimator, you can easily                     build a high-performance deep learning model and run it anywhere.
 Keywords: fastestimator tensorflow pytorch
```

### Comparing `fastestimator-1.5.1/fastestimator.egg-info/SOURCES.txt` & `fastestimator-1.5.2/fastestimator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/fastestimator.egg-info/requires.txt` & `fastestimator-1.5.2/fastestimator.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 pytorch-model-summary==0.1.2
 graphviz==0.19.1
 hiddenlayer==0.3
 pydot==1.4.2
 dot2tex==2.11.3
 gdown==3.12.0
 PySocks==1.7.1
-uncertainty-calibration==0.0.9
+uncertainty-calibration==0.1.4
 dill==0.3.4
 scikit-image==0.19.1
 prettytable==3.1.0
 nltk==3.7
 requests==2.22.0
 tqdm==4.64.0
 numpy<=1.23.5
```

### Comparing `fastestimator-1.5.1/setup.py` & `fastestimator-1.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         'pytorch-model-summary==0.1.2',
         'graphviz==0.19.1',
         'hiddenlayer==0.3',
         'pydot==1.4.2',
         'dot2tex==2.11.3',
         'gdown==3.12.0',
         'PySocks==1.7.1',
-        'uncertainty-calibration==0.0.9',
+        'uncertainty-calibration==0.1.4',
         'dill==0.3.4',
         'scikit-image==0.19.1',
         'prettytable==3.1.0',
         'nltk==3.7',
         'requests==2.22.0',
         'tqdm==4.64.0',
         'numpy<=1.23.5',
```

### Comparing `fastestimator-1.5.1/test/PR_test/__init__.py` & `fastestimator-1.5.2/test/PR_test/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/__init__.py` & `fastestimator-1.5.2/test/PR_test/integration_test/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/backend/__init__.py` & `fastestimator-1.5.2/test/PR_test/integration_test/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/backend/test_get_lr.py` & `fastestimator-1.5.2/test/PR_test/integration_test/backend/test_get_lr.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/backend/test_save_model_load_model.py` & `fastestimator-1.5.2/test/PR_test/integration_test/backend/test_save_model_load_model.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/backend/test_set_lr.py` & `fastestimator-1.5.2/test/PR_test/integration_test/backend/test_set_lr.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/backend/test_update_model.py` & `fastestimator-1.5.2/test/PR_test/integration_test/backend/test_update_model.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/cli/__init__.py` & `fastestimator-1.5.2/test/PR_test/integration_test/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/cli/test_main.py` & `fastestimator-1.5.2/test/PR_test/integration_test/cli/test_main.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/cli/test_train.py` & `fastestimator-1.5.2/test/PR_test/integration_test/cli/test_train.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/dataset/test_batch_dataset.py` & `fastestimator-1.5.2/test/PR_test/integration_test/dataset/test_batch_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/__init__.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/numpyop/__init__.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/numpyop/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/numpyop/meta/test_fuse.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/numpyop/meta/test_fuse.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/numpyop/meta/test_one_of.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/numpyop/meta/test_one_of.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/numpyop/meta/test_repeat.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/numpyop/meta/test_repeat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/numpyop/meta/test_sometimes.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/numpyop/meta/test_sometimes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/numpyop/multivariate/__init__.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/numpyop/multivariate/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/numpyop/multivariate/test_read_mat.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/numpyop/multivariate/test_read_mat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/numpyop/univariate/__init__.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/numpyop/univariate/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/numpyop/univariate/test_hadamard.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/numpyop/univariate/test_hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/numpyop/univariate/test_read_image.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/numpyop/univariate/test_read_image.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/__init__.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/augmentation/__init__.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/augmentation/test_cutmix_batch.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/augmentation/test_cutmix_batch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/gradient/__init__.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/gradient/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/gradient/test_fgsm.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/gradient/test_fgsm.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/gradient/test_gradientop.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/gradient/test_gradientop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/gradient/test_watch.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/gradient/test_watch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/loss/__init__.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/loss/test_cross_entropy.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/loss/test_cross_entropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/loss/test_hinge.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/loss/test_hinge.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/loss/test_l1_loss.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/loss/test_l1_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/loss/test_l2_regularization.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/loss/test_l2_regularization.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/loss/test_mean_squared_error.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/loss/test_mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/loss/test_super_loss.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/loss/test_super_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/meta/test_fuse.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/meta/test_fuse.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/meta/test_one_of.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/meta/test_one_of.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/meta/test_repeat.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/meta/test_repeat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/meta/test_sometimes.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/meta/test_sometimes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/model/__init__.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/model/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/model/test_modelop.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/model/test_modelop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/model/test_updateop.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/model/test_updateop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/test_argmax.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/test_argmax.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/test_average.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/test_average.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/test_reshape.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/test_reshape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/tensorop/test_un_hadamard.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/tensorop/test_un_hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/op/test_op.py` & `fastestimator-1.5.2/test/PR_test/integration_test/op/test_op.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/schedule/__init__.py` & `fastestimator-1.5.2/test/PR_test/integration_test/schedule/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/schedule/test_arc.py` & `fastestimator-1.5.2/test/PR_test/integration_test/schedule/test_arc.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/schedule/test_epoch_scheduler.py` & `fastestimator-1.5.2/test/PR_test/integration_test/schedule/test_epoch_scheduler.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/schedule/test_repeat_scheduler.py` & `fastestimator-1.5.2/test/PR_test/integration_test/schedule/test_repeat_scheduler.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/schedule/test_schedule.py` & `fastestimator-1.5.2/test/PR_test/integration_test/schedule/test_schedule.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/search/__init__.py` & `fastestimator-1.5.2/test/PR_test/integration_test/search/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/search/visualize/__init__.py` & `fastestimator-1.5.2/test/PR_test/integration_test/search/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/search/visualize/test_visualize.py` & `fastestimator-1.5.2/test/PR_test/integration_test/search/visualize/test_visualize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/summary/__init__.py` & `fastestimator-1.5.2/test/PR_test/integration_test/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/summary/test_history.py` & `fastestimator-1.5.2/test/PR_test/integration_test/summary/test_history.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/summary/test_system.py` & `fastestimator-1.5.2/test/PR_test/integration_test/summary/test_system.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/test_estimator.py` & `fastestimator-1.5.2/test/PR_test/integration_test/test_estimator.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/test_network.py` & `fastestimator-1.5.2/test/PR_test/integration_test/test_network.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/test_pipeline.py` & `fastestimator-1.5.2/test/PR_test/integration_test/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/__init__.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/adapt/__init__.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/adapt/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/adapt/test_early_stopping.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/adapt/test_early_stopping.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/adapt/test_lr_scheduler.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/adapt/test_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/adapt/test_pbm_calibrator.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/adapt/test_pbm_calibrator.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/adapt/test_reduce_lr_on_plateau.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/adapt/test_reduce_lr_on_plateau.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/adapt/test_terminate_on_nan.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/adapt/test_terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/io/__init__.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/io/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/io/test_best_model_saver.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/io/test_best_model_saver.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/io/test_csv_logger.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/io/test_csv_logger.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/io/test_image_saver.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/io/test_image_saver.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/io/test_image_viewer.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/io/test_image_viewer.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/io/test_model_saver.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/io/test_model_saver.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/io/test_restore_wizard.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/io/test_restore_wizard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/io/test_saliency.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/io/test_saliency.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/io/test_tensorboard.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/io/test_tensorboard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/io/test_test_report.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/io/test_test_report.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/io/test_traceability.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/io/test_traceability.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/metric/__init__.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/metric/test_accuracy.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/metric/test_accuracy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/metric/test_calibration_error.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/metric/test_calibration_error.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/metric/test_confusion_matrix.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/metric/test_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/metric/test_dice.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/metric/test_dice.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/metric/test_f1_score.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/metric/test_f1_score.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/metric/test_mcc.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/metric/test_mcc.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/metric/test_mean_average_precision.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/metric/test_mean_average_precision.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/metric/test_precision.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/metric/test_precision.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/metric/test_recall.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/metric/test_recall.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/test_eval_essential.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/test_eval_essential.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/test_logger.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/test_logger.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/test_test_essential.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/test_test_essential.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/test_trace.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/test_trace.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/test_train_essential.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/test_train_essential.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/xai/__init__.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/xai/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/xai/test_instance_tracker.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/xai/test_instance_tracker.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/trace/xai/test_label_tracker.py` & `fastestimator-1.5.2/test/PR_test/integration_test/trace/xai/test_label_tracker.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/util/__init__.py` & `fastestimator-1.5.2/test/PR_test/integration_test/util/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/util/test_img_data.py` & `fastestimator-1.5.2/test/PR_test/integration_test/util/test_img_data.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/util/test_traceability_util.py` & `fastestimator-1.5.2/test/PR_test/integration_test/util/test_traceability_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/integration_test/util/test_util.py` & `fastestimator-1.5.2/test/PR_test/integration_test/util/test_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/__init__.py` & `fastestimator-1.5.2/test/PR_test/unit_test/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/architecture/__init__.py` & `fastestimator-1.5.2/test/PR_test/unit_test/architecture/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/architecture/pytorch/__init__.py` & `fastestimator-1.5.2/test/PR_test/unit_test/architecture/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/architecture/pytorch/test_attention_unet.py` & `fastestimator-1.5.2/test/PR_test/unit_test/architecture/pytorch/test_attention_unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/architecture/pytorch/test_lenet.py` & `fastestimator-1.5.2/test/PR_test/unit_test/architecture/pytorch/test_lenet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/architecture/pytorch/test_resnet9.py` & `fastestimator-1.5.2/test/PR_test/unit_test/architecture/pytorch/test_resnet9.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/architecture/pytorch/test_unet.py` & `fastestimator-1.5.2/test/PR_test/unit_test/architecture/pytorch/test_unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/architecture/pytorch/test_wideresnet.py` & `fastestimator-1.5.2/test/PR_test/unit_test/architecture/pytorch/test_wideresnet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/architecture/tensorflow/__init__.py` & `fastestimator-1.5.2/test/PR_test/unit_test/architecture/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/architecture/tensorflow/test_attention_unet.py` & `fastestimator-1.5.2/test/PR_test/unit_test/architecture/tensorflow/test_attention_unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/architecture/tensorflow/test_lenet.py` & `fastestimator-1.5.2/test/PR_test/unit_test/architecture/tensorflow/test_lenet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/architecture/tensorflow/test_resnet9.py` & `fastestimator-1.5.2/test/PR_test/unit_test/architecture/tensorflow/test_resnet9.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/architecture/tensorflow/test_unet.py` & `fastestimator-1.5.2/test/PR_test/unit_test/architecture/tensorflow/test_unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/architecture/tensorflow/test_wideresnet.py` & `fastestimator-1.5.2/test/PR_test/unit_test/architecture/tensorflow/test_wideresnet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/__init__.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_abs.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_abs.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_argmax.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_argmax.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_binary_crossentropy.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_binary_crossentropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_cast.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_cast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_categorical_crossentropy.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_categorical_crossentropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_check_nan.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_check_nan.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_clip_by_value.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_clip_by_value.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_concat.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_concat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_dice_score.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_dice_score.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_exp.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_exp.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_expand_dims.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_expand_dims.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_feed_forward.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_feed_forward.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_gather.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_gather.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_gather_from_batch.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_gather_from_batch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_get_gradient.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_get_gradient.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_get_image_dims.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_get_image_dims.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_hinge.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_hinge.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_iwd.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_iwd.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_lambertw.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_lambertw.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_matmul.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_matmul.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_maximum.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_maximum.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_mean_squared_error.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_ones_like.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_ones_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_percentile.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_percentile.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_permute.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_permute.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_pow.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_pow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_random_normal_like.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_random_normal_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_random_uniform_like.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_random_uniform_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_reduce_max.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_reduce_max.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_reduce_mean.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_reduce_mean.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_reduce_min.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_reduce_min.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_reduce_std.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_reduce_std.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_reduce_sum.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_reduce_sum.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_reshape.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_reshape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_resize3d.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_resize3d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_roll.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_roll.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_sign.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_sign.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_sparse_categorical_crossentropy.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_sparse_categorical_crossentropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_squeeze.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_squeeze.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_tensor_normalize.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_tensor_normalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_tensor_pow.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_tensor_pow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_tensor_round.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_tensor_round.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_tensor_sqrt.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_tensor_sqrt.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_to_shape.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_to_shape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_to_tensor.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_to_tensor.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_to_type.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_to_type.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_transpose.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_transpose.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_watch.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_watch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_zeros_like.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_zeros_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/backend/test_zscore.py` & `fastestimator-1.5.2/test/PR_test/unit_test/backend/test_zscore.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/cli/__init__.py` & `fastestimator-1.5.2/test/PR_test/unit_test/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/cli/test_cli_util.py` & `fastestimator-1.5.2/test/PR_test/unit_test/cli/test_cli_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/dataset/__init__.py` & `fastestimator-1.5.2/test/PR_test/unit_test/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/dataset/test_batch_dataset.py` & `fastestimator-1.5.2/test/PR_test/unit_test/dataset/test_batch_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/dataset/test_csv_dataset.py` & `fastestimator-1.5.2/test/PR_test/unit_test/dataset/test_csv_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/dataset/test_data.py` & `fastestimator-1.5.2/test/PR_test/unit_test/dataset/test_data.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/dataset/test_dir_dataset.py` & `fastestimator-1.5.2/test/PR_test/unit_test/dataset/test_dir_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/dataset/test_extend_dataset.py` & `fastestimator-1.5.2/test/PR_test/unit_test/dataset/test_extend_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/dataset/test_generator_dataset.py` & `fastestimator-1.5.2/test/PR_test/unit_test/dataset/test_generator_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/dataset/test_labeled_dir_dataset.py` & `fastestimator-1.5.2/test/PR_test/unit_test/dataset/test_labeled_dir_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/dataset/test_numpy_dataset.py` & `fastestimator-1.5.2/test/PR_test/unit_test/dataset/test_numpy_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/dataset/test_pickle_dataset.py` & `fastestimator-1.5.2/test/PR_test/unit_test/dataset/test_pickle_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/dataset/test_siamese_dir_dataset.py` & `fastestimator-1.5.2/test/PR_test/unit_test/dataset/test_siamese_dir_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/layers/__init__.py` & `fastestimator-1.5.2/test/PR_test/unit_test/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/layers/pytorch/__init__.py` & `fastestimator-1.5.2/test/PR_test/unit_test/layers/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/layers/pytorch/test_cropping_2d.py` & `fastestimator-1.5.2/test/PR_test/unit_test/layers/pytorch/test_cropping_2d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/layers/pytorch/test_hadamard.py` & `fastestimator-1.5.2/test/PR_test/unit_test/layers/pytorch/test_hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/layers/tensorflow/__init__.py` & `fastestimator-1.5.2/test/PR_test/unit_test/layers/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/layers/tensorflow/test_hadamard.py` & `fastestimator-1.5.2/test/PR_test/unit_test/layers/tensorflow/test_hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/layers/tensorflow/test_instance_norm.py` & `fastestimator-1.5.2/test/PR_test/unit_test/layers/tensorflow/test_instance_norm.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/layers/tensorflow/test_reflection_padding_2d.py` & `fastestimator-1.5.2/test/PR_test/unit_test/layers/tensorflow/test_reflection_padding_2d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/__init__.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/loss/__init__.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/loss/test_focal_loss.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/loss/test_focal_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/loss/test_mix_loss.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/loss/test_mix_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/__init__.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/meta/__init__.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/meta/test_fuse.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/meta/test_fuse.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/meta/test_one_of.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/meta/test_one_of.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/meta/test_repeat.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/meta/test_repeat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/meta/test_sometimes.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/meta/test_sometimes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/__init__.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_affine.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_affine.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_center_crop.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_center_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_crop.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_crop_non_empy_mask_if_exists.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_crop_non_empy_mask_if_exists.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_elastic_transform.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_elastic_transform.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_flip.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_flip.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_grid_distortion.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_grid_distortion.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_horizontal_flip.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_horizontal_flip.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_iaa_crop_and_pad.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_iaa_crop_and_pad.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_longest_max_size.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_longest_max_size.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_mask_dropout.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_mask_dropout.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_optical_distortion.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_optical_distortion.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_pad_if_needed.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_pad_if_needed.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop_near_bbox.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop_near_bbox.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_random_grid_shuffle.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_random_grid_shuffle.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_random_resized_crop.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_random_resized_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_random_rotate_90.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_random_rotate_90.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_random_scale.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_random_scale.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_bbox_safe_crop.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_bbox_safe_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_crop.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_resize.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_resize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_rotate.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_rotate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_shift_scale_rotate.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_shift_scale_rotate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_smallest_max_size.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_smallest_max_size.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_transpose.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_transpose.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/multivariate/test_vertical_flip.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/multivariate/test_vertical_flip.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/test_numpyop.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/test_numpyop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/__init__.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_autocontrast.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_autocontrast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_binarize.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_binarize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_blur.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_brightness.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_brightness.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_calibrate.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_calibrate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_channel_dropout.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_channel_dropout.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_channel_shuffle.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_channel_shuffle.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_channel_transpose.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_channel_transpose.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_clahe.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_clahe.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_coarse_dropout.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_coarse_dropout.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_color.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_color.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_color_jitter.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_color_jitter.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_contrast.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_contrast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_downscale.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_downscale.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_equalize.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_equalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_expand_dims.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_expand_dims.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_fromfloat.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_fromfloat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_blur.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_noise.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_hue_saturation_value.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_hue_saturation_value.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_iaa_additive_gaussian_noise.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_iaa_additive_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_image_compression.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_image_compression.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_invert_img.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_invert_img.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_iso_noise.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_iso_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_median_blur.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_median_blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_minmax.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_minmax.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_motion_blur.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_motion_blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_multiplicative_noise.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_multiplicative_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_normalize.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_normalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_onehot.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_onehot.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_pad_sequence.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_pad_sequence.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_posterize.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_posterize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_random_brightness_contrast.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_random_brightness_contrast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_random_fog.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_random_fog.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_random_gamma.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_random_gamma.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_random_rain.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_random_rain.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_random_shadow.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_random_shadow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_random_shapes.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_random_shapes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_random_snow.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_random_snow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_random_sun_flare.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_random_sun_flare.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_reshape.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_reshape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_rgb_shift.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_rgb_shift.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_rua.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_rua.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_sharpness.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_sharpness.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_shear_x.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_shear_x.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_shear_y.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_shear_y.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_solarize.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_solarize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_to_array.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_to_array.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_to_float.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_to_float.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_to_gray.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_to_gray.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_to_sepia.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_to_sepia.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_tokenize.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_translate_x.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_translate_x.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_translate_y.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_translate_y.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/numpyop/univariate/test_word_to_id.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/numpyop/univariate/test_word_to_id.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/tensorop/__init__.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/tensorop/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/tensorop/augmentation/__init__.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/tensorop/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/tensorop/augmentation/test_mixup_batch.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/tensorop/augmentation/test_mixup_batch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/tensorop/meta/__init__.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/tensorop/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/tensorop/meta/test_fuse.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/tensorop/meta/test_fuse.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/tensorop/meta/test_one_of.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/tensorop/meta/test_one_of.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/tensorop/meta/test_repeat.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/tensorop/meta/test_repeat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/tensorop/meta/test_sometimes.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/tensorop/meta/test_sometimes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/tensorop/test_normalize.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/tensorop/test_normalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/tensorop/test_tensorop.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/tensorop/test_tensorop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/op/test_op.py` & `fastestimator-1.5.2/test/PR_test/unit_test/op/test_op.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/schedule/__init__.py` & `fastestimator-1.5.2/test/PR_test/unit_test/schedule/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/schedule/test_epoch_scheduler.py` & `fastestimator-1.5.2/test/PR_test/unit_test/schedule/test_epoch_scheduler.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/schedule/test_lr_schedule.py` & `fastestimator-1.5.2/test/PR_test/unit_test/schedule/test_lr_schedule.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/schedule/test_repeat_scheduler.py` & `fastestimator-1.5.2/test/PR_test/unit_test/schedule/test_repeat_scheduler.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/search/__init__.py` & `fastestimator-1.5.2/test/PR_test/unit_test/search/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/search/test_golden_section_search.py` & `fastestimator-1.5.2/test/PR_test/unit_test/search/test_golden_section_search.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/search/test_grid_search.py` & `fastestimator-1.5.2/test/PR_test/unit_test/search/test_grid_search.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/search/test_search.py` & `fastestimator-1.5.2/test/PR_test/unit_test/search/test_search.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/summary/__init__.py` & `fastestimator-1.5.2/test/PR_test/unit_test/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/summary/logs/__init__.py` & `fastestimator-1.5.2/test/PR_test/unit_test/summary/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/summary/logs/test_metrics.py` & `fastestimator-1.5.2/test/PR_test/unit_test/summary/logs/test_metrics.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/summary/test_history.py` & `fastestimator-1.5.2/test/PR_test/unit_test/summary/test_history.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/summary/test_summary.py` & `fastestimator-1.5.2/test/PR_test/unit_test/summary/test_summary.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/test/__init__.py` & `fastestimator-1.5.2/test/PR_test/unit_test/test/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/test/test_unittest_util.py` & `fastestimator-1.5.2/test/PR_test/unit_test/test/test_unittest_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/trace/__init__.py` & `fastestimator-1.5.2/test/PR_test/unit_test/trace/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/trace/metric/__init__.py` & `fastestimator-1.5.2/test/PR_test/unit_test/trace/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/trace/metric/test_bleu_score.py` & `fastestimator-1.5.2/test/PR_test/unit_test/trace/metric/test_bleu_score.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/util/__init__.py` & `fastestimator-1.5.2/test/PR_test/unit_test/util/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/util/test_data.py` & `fastestimator-1.5.2/test/PR_test/unit_test/util/test_data.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/util/test_traceability_util.py` & `fastestimator-1.5.2/test/PR_test/unit_test/util/test_traceability_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/util/test_util.py` & `fastestimator-1.5.2/test/PR_test/unit_test/util/test_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/util/test_wget_util.py` & `fastestimator-1.5.2/test/PR_test/unit_test/util/test_wget_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/xai/__init__.py` & `fastestimator-1.5.2/test/PR_test/unit_test/xai/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/PR_test/unit_test/xai/test_saliency.py` & `fastestimator-1.5.2/test/PR_test/unit_test/xai/test_saliency.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/__init__.py` & `fastestimator-1.5.2/test/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-1.5.1/test/run_pr_test.py` & `fastestimator-1.5.2/test/run_pr_test.py`

 * *Files identical despite different names*

