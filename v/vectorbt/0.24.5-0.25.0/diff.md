# Comparing `tmp/vectorbt-0.24.5.tar.gz` & `tmp/vectorbt-0.25.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectorbt-0.24.5.tar", last modified: Fri Jan 27 16:32:59 2023, max compression
+gzip compressed data, was "vectorbt-0.25.0.tar", last modified: Wed Apr 26 17:40:24 2023, max compression
```

## Comparing `vectorbt-0.24.5.tar` & `vectorbt-0.25.0.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-01-27 16:32:59.267261 vectorbt-0.24.5/
--rw-r--r--   0 olegpolakow   (501) staff       (20)    12321 2021-08-27 15:59:45.000000 vectorbt-0.24.5/LICENSE.md
--rw-r--r--   0 olegpolakow   (501) staff       (20)       43 2020-12-16 11:21:09.000000 vectorbt-0.24.5/MANIFEST.in
--rw-r--r--   0 olegpolakow   (501) staff       (20)     9941 2023-01-27 16:32:59.267023 vectorbt-0.24.5/PKG-INFO
--rw-r--r--   0 olegpolakow   (501) staff       (20)     8799 2023-01-15 23:29:02.000000 vectorbt-0.24.5/README.md
--rw-r--r--   0 olegpolakow   (501) staff       (20)       38 2023-01-27 16:32:59.267309 vectorbt-0.24.5/setup.cfg
--rw-r--r--   0 olegpolakow   (501) staff       (20)     2480 2022-08-22 10:31:03.000000 vectorbt-0.24.5/setup.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-01-27 16:32:59.224251 vectorbt-0.24.5/tests/
--rw-r--r--   0 olegpolakow   (501) staff       (20)        0 2020-09-24 13:38:09.000000 vectorbt-0.24.5/tests/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)   133888 2022-02-04 19:42:08.000000 vectorbt-0.24.5/tests/test_base.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    41817 2021-12-11 19:17:59.000000 vectorbt-0.24.5/tests/test_data.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    71409 2021-12-11 19:17:59.000000 vectorbt-0.24.5/tests/test_generic.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)   113489 2021-12-11 19:17:59.000000 vectorbt-0.24.5/tests/test_indicators.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    17467 2021-12-11 19:17:59.000000 vectorbt-0.24.5/tests/test_labels.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)   340197 2022-01-08 23:21:38.000000 vectorbt-0.24.5/tests/test_portfolio.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)   144703 2021-12-11 19:17:59.000000 vectorbt-0.24.5/tests/test_records.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    30853 2021-12-20 21:46:30.000000 vectorbt-0.24.5/tests/test_returns.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)      485 2022-08-22 10:34:19.000000 vectorbt-0.24.5/tests/test_settings.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)   116566 2021-12-11 19:17:59.000000 vectorbt-0.24.5/tests/test_signals.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)   100085 2021-12-11 19:17:59.000000 vectorbt-0.24.5/tests/test_utils.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)      539 2021-12-11 19:17:59.000000 vectorbt-0.24.5/tests/utils.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-01-27 16:32:59.226124 vectorbt-0.24.5/vectorbt/
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1042 2021-12-29 16:06:17.000000 vectorbt-0.24.5/vectorbt/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    23974 2023-01-21 21:32:01.000000 vectorbt-0.24.5/vectorbt/_settings.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     5146 2021-12-11 19:18:51.000000 vectorbt-0.24.5/vectorbt/_typing.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)      178 2023-01-27 16:30:51.000000 vectorbt-0.24.5/vectorbt/_version.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-01-27 16:32:59.229500 vectorbt-0.24.5/vectorbt/base/
--rw-r--r--   0 olegpolakow   (501) staff       (20)      371 2021-12-10 15:32:09.000000 vectorbt-0.24.5/vectorbt/base/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    31667 2021-12-30 14:21:04.000000 vectorbt-0.24.5/vectorbt/base/accessors.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    34228 2021-12-29 18:25:09.000000 vectorbt-0.24.5/vectorbt/base/array_wrapper.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    11937 2021-12-11 19:17:59.000000 vectorbt-0.24.5/vectorbt/base/column_grouper.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    10064 2021-12-10 15:32:09.000000 vectorbt-0.24.5/vectorbt/base/combine_fns.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    15273 2021-12-11 19:17:59.000000 vectorbt-0.24.5/vectorbt/base/index_fns.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    11555 2021-12-30 14:20:04.000000 vectorbt-0.24.5/vectorbt/base/indexing.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    35550 2022-02-04 19:18:00.000000 vectorbt-0.24.5/vectorbt/base/reshape_fns.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-01-27 16:32:59.231257 vectorbt-0.24.5/vectorbt/data/
--rw-r--r--   0 olegpolakow   (501) staff       (20)      602 2021-12-28 22:07:56.000000 vectorbt-0.24.5/vectorbt/data/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    30578 2021-12-30 14:36:24.000000 vectorbt-0.24.5/vectorbt/data/base.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    38681 2021-12-30 22:47:03.000000 vectorbt-0.24.5/vectorbt/data/custom.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     5943 2021-12-30 14:07:40.000000 vectorbt-0.24.5/vectorbt/data/updater.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-01-27 16:32:59.235479 vectorbt-0.24.5/vectorbt/generic/
--rw-r--r--   0 olegpolakow   (501) staff       (20)      653 2021-12-11 19:17:59.000000 vectorbt-0.24.5/vectorbt/generic/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)   100294 2021-12-30 14:29:09.000000 vectorbt-0.24.5/vectorbt/generic/accessors.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     6179 2021-12-10 15:32:09.000000 vectorbt-0.24.5/vectorbt/generic/decorators.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    39242 2021-12-30 14:36:24.000000 vectorbt-0.24.5/vectorbt/generic/drawdowns.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1631 2021-12-10 15:32:09.000000 vectorbt-0.24.5/vectorbt/generic/enums.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    58884 2022-02-04 19:09:27.000000 vectorbt-0.24.5/vectorbt/generic/nb.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    32132 2021-12-30 14:24:06.000000 vectorbt-0.24.5/vectorbt/generic/plots_builder.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    34072 2021-12-30 14:23:52.000000 vectorbt-0.24.5/vectorbt/generic/plotting.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    23637 2021-12-30 14:36:24.000000 vectorbt-0.24.5/vectorbt/generic/ranges.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    10677 2021-12-30 14:29:09.000000 vectorbt-0.24.5/vectorbt/generic/splitters.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    30614 2021-12-30 14:24:15.000000 vectorbt-0.24.5/vectorbt/generic/stats_builder.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-01-27 16:32:59.237820 vectorbt-0.24.5/vectorbt/indicators/
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1536 2021-12-11 19:18:00.000000 vectorbt-0.24.5/vectorbt/indicators/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    28123 2021-12-30 14:36:24.000000 vectorbt-0.24.5/vectorbt/indicators/basic.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)      932 2021-12-10 15:32:09.000000 vectorbt-0.24.5/vectorbt/indicators/configs.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)   160408 2022-09-30 11:11:57.000000 vectorbt-0.24.5/vectorbt/indicators/factory.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     9340 2021-12-10 15:32:09.000000 vectorbt-0.24.5/vectorbt/indicators/nb.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-01-27 16:32:59.239107 vectorbt-0.24.5/vectorbt/labels/
--rw-r--r--   0 olegpolakow   (501) staff       (20)      585 2021-08-27 15:59:45.000000 vectorbt-0.24.5/vectorbt/labels/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1006 2021-12-10 15:32:09.000000 vectorbt-0.24.5/vectorbt/labels/enums.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     5272 2021-12-11 19:17:59.000000 vectorbt-0.24.5/vectorbt/labels/generators.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    12709 2021-12-10 15:32:09.000000 vectorbt-0.24.5/vectorbt/labels/nb.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-01-27 16:32:59.239814 vectorbt-0.24.5/vectorbt/messaging/
--rw-r--r--   0 olegpolakow   (501) staff       (20)      437 2021-08-27 15:59:45.000000 vectorbt-0.24.5/vectorbt/messaging/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    14938 2021-12-30 14:18:12.000000 vectorbt-0.24.5/vectorbt/messaging/telegram.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    14435 2021-12-30 14:18:12.000000 vectorbt-0.24.5/vectorbt/ohlcv_accessors.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-01-27 16:32:59.246492 vectorbt-0.24.5/vectorbt/portfolio/
--rw-r--r--   0 olegpolakow   (501) staff       (20)      616 2021-12-11 19:17:59.000000 vectorbt-0.24.5/vectorbt/portfolio/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)   238543 2022-12-04 18:11:12.000000 vectorbt-0.24.5/vectorbt/portfolio/base.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     2404 2021-12-10 15:32:09.000000 vectorbt-0.24.5/vectorbt/portfolio/decorators.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    53808 2021-12-30 14:36:24.000000 vectorbt-0.24.5/vectorbt/portfolio/enums.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    10068 2021-12-29 18:25:09.000000 vectorbt-0.24.5/vectorbt/portfolio/logs.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)   270564 2023-01-27 16:28:22.000000 vectorbt-0.24.5/vectorbt/portfolio/nb.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    17272 2021-12-30 14:36:24.000000 vectorbt-0.24.5/vectorbt/portfolio/orders.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    62285 2021-12-30 14:36:24.000000 vectorbt-0.24.5/vectorbt/portfolio/trades.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     4200 2021-12-30 14:18:12.000000 vectorbt-0.24.5/vectorbt/px_accessors.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-01-27 16:32:59.249412 vectorbt-0.24.5/vectorbt/records/
--rw-r--r--   0 olegpolakow   (501) staff       (20)      613 2021-12-11 19:17:59.000000 vectorbt-0.24.5/vectorbt/records/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    29384 2021-12-29 18:25:09.000000 vectorbt-0.24.5/vectorbt/records/base.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     3536 2021-12-11 19:17:59.000000 vectorbt-0.24.5/vectorbt/records/col_mapper.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     9486 2021-12-11 19:17:59.000000 vectorbt-0.24.5/vectorbt/records/decorators.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    42635 2021-12-29 18:25:09.000000 vectorbt-0.24.5/vectorbt/records/mapped_array.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    17680 2021-12-10 15:32:09.000000 vectorbt-0.24.5/vectorbt/records/nb.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-01-27 16:32:59.252529 vectorbt-0.24.5/vectorbt/returns/
--rw-r--r--   0 olegpolakow   (501) staff       (20)      486 2021-08-27 15:59:45.000000 vectorbt-0.24.5/vectorbt/returns/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    55618 2021-12-30 14:08:14.000000 vectorbt-0.24.5/vectorbt/returns/accessors.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1160 2021-12-11 19:17:59.000000 vectorbt-0.24.5/vectorbt/returns/metrics.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    27796 2021-12-29 18:25:09.000000 vectorbt-0.24.5/vectorbt/returns/nb.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     8672 2021-12-29 18:25:09.000000 vectorbt-0.24.5/vectorbt/returns/qs_adapter.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     5093 2021-12-11 19:17:59.000000 vectorbt-0.24.5/vectorbt/root_accessors.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-01-27 16:32:59.258851 vectorbt-0.24.5/vectorbt/signals/
--rw-r--r--   0 olegpolakow   (501) staff       (20)      712 2021-08-27 15:59:45.000000 vectorbt-0.24.5/vectorbt/signals/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    73582 2021-12-30 14:18:12.000000 vectorbt-0.24.5/vectorbt/signals/accessors.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1842 2021-12-11 19:17:59.000000 vectorbt-0.24.5/vectorbt/signals/enums.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    42731 2021-12-30 14:36:24.000000 vectorbt-0.24.5/vectorbt/signals/factory.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    22617 2021-12-30 14:10:40.000000 vectorbt-0.24.5/vectorbt/signals/generators.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    48870 2021-12-30 14:18:12.000000 vectorbt-0.24.5/vectorbt/signals/nb.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-01-27 16:32:59.259640 vectorbt-0.24.5/vectorbt/templates/
--rw-r--r--   0 olegpolakow   (501) staff       (20)    14983 2021-12-11 19:17:59.000000 vectorbt-0.24.5/vectorbt/templates/dark.json
--rw-r--r--   0 olegpolakow   (501) staff       (20)    14744 2021-12-11 19:17:59.000000 vectorbt-0.24.5/vectorbt/templates/light.json
--rw-r--r--   0 olegpolakow   (501) staff       (20)     5645 2021-12-11 19:17:59.000000 vectorbt-0.24.5/vectorbt/templates/seaborn.json
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-01-27 16:32:59.266666 vectorbt-0.24.5/vectorbt/utils/
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1229 2021-12-11 19:17:59.000000 vectorbt-0.24.5/vectorbt/utils/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     4205 2021-12-10 15:32:09.000000 vectorbt-0.24.5/vectorbt/utils/array_.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     7841 2021-12-11 19:16:46.000000 vectorbt-0.24.5/vectorbt/utils/attr_.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    18106 2021-12-11 19:17:59.000000 vectorbt-0.24.5/vectorbt/utils/checks.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1611 2021-12-11 19:17:59.000000 vectorbt-0.24.5/vectorbt/utils/colors.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    31370 2021-12-30 15:26:38.000000 vectorbt-0.24.5/vectorbt/utils/config.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     5844 2022-03-17 17:54:25.000000 vectorbt-0.24.5/vectorbt/utils/datetime_.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    21278 2021-12-30 14:18:12.000000 vectorbt-0.24.5/vectorbt/utils/decorators.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     2333 2021-12-30 15:33:01.000000 vectorbt-0.24.5/vectorbt/utils/docs.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1015 2021-10-16 12:03:47.000000 vectorbt-0.24.5/vectorbt/utils/enum_.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     3389 2021-12-10 15:32:09.000000 vectorbt-0.24.5/vectorbt/utils/figure.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     3037 2021-12-11 19:17:59.000000 vectorbt-0.24.5/vectorbt/utils/image_.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     6089 2021-12-11 19:16:46.000000 vectorbt-0.24.5/vectorbt/utils/mapping.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1934 2021-12-11 19:17:59.000000 vectorbt-0.24.5/vectorbt/utils/math_.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     2159 2021-12-11 19:17:59.000000 vectorbt-0.24.5/vectorbt/utils/module_.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     3358 2021-12-30 14:21:04.000000 vectorbt-0.24.5/vectorbt/utils/params.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)      493 2021-12-11 19:17:59.000000 vectorbt-0.24.5/vectorbt/utils/random_.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1787 2021-12-11 19:17:59.000000 vectorbt-0.24.5/vectorbt/utils/requests_.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     9968 2021-12-30 14:12:34.000000 vectorbt-0.24.5/vectorbt/utils/schedule_.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1951 2021-12-30 14:12:34.000000 vectorbt-0.24.5/vectorbt/utils/tags.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     8622 2021-12-30 14:12:47.000000 vectorbt-0.24.5/vectorbt/utils/template.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-01-27 16:32:59.226860 vectorbt-0.24.5/vectorbt.egg-info/
--rw-r--r--   0 olegpolakow   (501) staff       (20)     9941 2023-01-27 16:32:59.000000 vectorbt-0.24.5/vectorbt.egg-info/PKG-INFO
--rw-r--r--   0 olegpolakow   (501) staff       (20)     2937 2023-01-27 16:32:59.000000 vectorbt-0.24.5/vectorbt.egg-info/SOURCES.txt
--rw-r--r--   0 olegpolakow   (501) staff       (20)        1 2023-01-27 16:32:59.000000 vectorbt-0.24.5/vectorbt.egg-info/dependency_links.txt
--rw-r--r--   0 olegpolakow   (501) staff       (20)      460 2023-01-27 16:32:59.000000 vectorbt-0.24.5/vectorbt.egg-info/requires.txt
--rw-r--r--   0 olegpolakow   (501) staff       (20)       15 2023-01-27 16:32:59.000000 vectorbt-0.24.5/vectorbt.egg-info/top_level.txt
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-04-26 17:40:24.745911 vectorbt-0.25.0/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    12321 2021-08-27 15:59:45.000000 vectorbt-0.25.0/LICENSE.md
+-rw-r--r--   0 olegpolakow   (501) staff       (20)       43 2020-12-16 11:21:09.000000 vectorbt-0.25.0/MANIFEST.in
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     9941 2023-04-26 17:40:24.745520 vectorbt-0.25.0/PKG-INFO
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     8799 2023-01-15 23:29:02.000000 vectorbt-0.25.0/README.md
+-rw-r--r--   0 olegpolakow   (501) staff       (20)       38 2023-04-26 17:40:24.745994 vectorbt-0.25.0/setup.cfg
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     2480 2022-08-22 10:31:03.000000 vectorbt-0.25.0/setup.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-04-26 17:40:24.695423 vectorbt-0.25.0/tests/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)        0 2020-09-24 13:38:09.000000 vectorbt-0.25.0/tests/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)   133754 2023-04-26 17:23:51.000000 vectorbt-0.25.0/tests/test_base.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    41687 2023-04-26 17:34:55.000000 vectorbt-0.25.0/tests/test_data.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    71129 2023-04-26 17:32:19.000000 vectorbt-0.25.0/tests/test_generic.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)   113482 2023-04-26 17:28:11.000000 vectorbt-0.25.0/tests/test_indicators.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    17467 2021-12-11 19:17:59.000000 vectorbt-0.25.0/tests/test_labels.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)   340117 2023-04-26 17:22:10.000000 vectorbt-0.25.0/tests/test_portfolio.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)   144385 2023-04-26 17:36:53.000000 vectorbt-0.25.0/tests/test_records.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    30853 2021-12-20 21:46:30.000000 vectorbt-0.25.0/tests/test_returns.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      485 2022-08-22 10:34:19.000000 vectorbt-0.25.0/tests/test_settings.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)   116464 2023-04-26 17:22:30.000000 vectorbt-0.25.0/tests/test_signals.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)   100085 2021-12-11 19:17:59.000000 vectorbt-0.25.0/tests/test_utils.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      539 2021-12-11 19:17:59.000000 vectorbt-0.25.0/tests/utils.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-04-26 17:40:24.699763 vectorbt-0.25.0/vectorbt/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1042 2021-12-29 16:06:17.000000 vectorbt-0.25.0/vectorbt/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    23974 2023-01-21 21:32:01.000000 vectorbt-0.25.0/vectorbt/_settings.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     5146 2021-12-11 19:18:51.000000 vectorbt-0.25.0/vectorbt/_typing.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      178 2023-04-26 17:38:13.000000 vectorbt-0.25.0/vectorbt/_version.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-04-26 17:40:24.704301 vectorbt-0.25.0/vectorbt/base/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      371 2021-12-10 15:32:09.000000 vectorbt-0.25.0/vectorbt/base/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    31667 2021-12-30 14:21:04.000000 vectorbt-0.25.0/vectorbt/base/accessors.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    34228 2021-12-29 18:25:09.000000 vectorbt-0.25.0/vectorbt/base/array_wrapper.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    11937 2021-12-11 19:17:59.000000 vectorbt-0.25.0/vectorbt/base/column_grouper.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    10064 2021-12-10 15:32:09.000000 vectorbt-0.25.0/vectorbt/base/combine_fns.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    15273 2021-12-11 19:17:59.000000 vectorbt-0.25.0/vectorbt/base/index_fns.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    11555 2021-12-30 14:20:04.000000 vectorbt-0.25.0/vectorbt/base/indexing.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    35550 2022-02-04 19:18:00.000000 vectorbt-0.25.0/vectorbt/base/reshape_fns.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-04-26 17:40:24.706441 vectorbt-0.25.0/vectorbt/data/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      602 2021-12-28 22:07:56.000000 vectorbt-0.25.0/vectorbt/data/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    30567 2023-04-26 17:25:50.000000 vectorbt-0.25.0/vectorbt/data/base.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    38681 2021-12-30 22:47:03.000000 vectorbt-0.25.0/vectorbt/data/custom.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     5943 2021-12-30 14:07:40.000000 vectorbt-0.25.0/vectorbt/data/updater.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-04-26 17:40:24.714003 vectorbt-0.25.0/vectorbt/generic/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      653 2021-12-11 19:17:59.000000 vectorbt-0.25.0/vectorbt/generic/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)   100299 2023-04-26 17:29:09.000000 vectorbt-0.25.0/vectorbt/generic/accessors.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     6179 2021-12-10 15:32:09.000000 vectorbt-0.25.0/vectorbt/generic/decorators.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    39242 2021-12-30 14:36:24.000000 vectorbt-0.25.0/vectorbt/generic/drawdowns.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1631 2021-12-10 15:32:09.000000 vectorbt-0.25.0/vectorbt/generic/enums.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    58884 2022-02-04 19:09:27.000000 vectorbt-0.25.0/vectorbt/generic/nb.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    32132 2021-12-30 14:24:06.000000 vectorbt-0.25.0/vectorbt/generic/plots_builder.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    34072 2021-12-30 14:23:52.000000 vectorbt-0.25.0/vectorbt/generic/plotting.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    23637 2021-12-30 14:36:24.000000 vectorbt-0.25.0/vectorbt/generic/ranges.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    10677 2021-12-30 14:29:09.000000 vectorbt-0.25.0/vectorbt/generic/splitters.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    30614 2021-12-30 14:24:15.000000 vectorbt-0.25.0/vectorbt/generic/stats_builder.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-04-26 17:40:24.716877 vectorbt-0.25.0/vectorbt/indicators/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1536 2021-12-11 19:18:00.000000 vectorbt-0.25.0/vectorbt/indicators/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    28123 2021-12-30 14:36:24.000000 vectorbt-0.25.0/vectorbt/indicators/basic.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      932 2021-12-10 15:32:09.000000 vectorbt-0.25.0/vectorbt/indicators/configs.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)   160408 2022-09-30 11:11:57.000000 vectorbt-0.25.0/vectorbt/indicators/factory.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     9340 2021-12-10 15:32:09.000000 vectorbt-0.25.0/vectorbt/indicators/nb.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-04-26 17:40:24.718613 vectorbt-0.25.0/vectorbt/labels/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      585 2021-08-27 15:59:45.000000 vectorbt-0.25.0/vectorbt/labels/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1006 2021-12-10 15:32:09.000000 vectorbt-0.25.0/vectorbt/labels/enums.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     5272 2021-12-11 19:17:59.000000 vectorbt-0.25.0/vectorbt/labels/generators.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    12709 2021-12-10 15:32:09.000000 vectorbt-0.25.0/vectorbt/labels/nb.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-04-26 17:40:24.719311 vectorbt-0.25.0/vectorbt/messaging/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      437 2021-08-27 15:59:45.000000 vectorbt-0.25.0/vectorbt/messaging/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    14938 2021-12-30 14:18:12.000000 vectorbt-0.25.0/vectorbt/messaging/telegram.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    14435 2021-12-30 14:18:12.000000 vectorbt-0.25.0/vectorbt/ohlcv_accessors.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-04-26 17:40:24.724150 vectorbt-0.25.0/vectorbt/portfolio/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      616 2021-12-11 19:17:59.000000 vectorbt-0.25.0/vectorbt/portfolio/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)   238538 2023-04-26 17:22:09.000000 vectorbt-0.25.0/vectorbt/portfolio/base.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     2404 2021-12-10 15:32:09.000000 vectorbt-0.25.0/vectorbt/portfolio/decorators.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    53808 2021-12-30 14:36:24.000000 vectorbt-0.25.0/vectorbt/portfolio/enums.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    10068 2021-12-29 18:25:09.000000 vectorbt-0.25.0/vectorbt/portfolio/logs.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)   270564 2023-01-27 16:28:22.000000 vectorbt-0.25.0/vectorbt/portfolio/nb.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    17272 2021-12-30 14:36:24.000000 vectorbt-0.25.0/vectorbt/portfolio/orders.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    62285 2021-12-30 14:36:24.000000 vectorbt-0.25.0/vectorbt/portfolio/trades.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     4200 2021-12-30 14:18:12.000000 vectorbt-0.25.0/vectorbt/px_accessors.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-04-26 17:40:24.726956 vectorbt-0.25.0/vectorbt/records/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      613 2021-12-11 19:17:59.000000 vectorbt-0.25.0/vectorbt/records/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    29384 2021-12-29 18:25:09.000000 vectorbt-0.25.0/vectorbt/records/base.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     3536 2021-12-11 19:17:59.000000 vectorbt-0.25.0/vectorbt/records/col_mapper.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     9486 2021-12-11 19:17:59.000000 vectorbt-0.25.0/vectorbt/records/decorators.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    42640 2023-04-26 17:29:08.000000 vectorbt-0.25.0/vectorbt/records/mapped_array.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    17680 2021-12-10 15:32:09.000000 vectorbt-0.25.0/vectorbt/records/nb.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-04-26 17:40:24.729669 vectorbt-0.25.0/vectorbt/returns/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      486 2021-08-27 15:59:45.000000 vectorbt-0.25.0/vectorbt/returns/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    55618 2021-12-30 14:08:14.000000 vectorbt-0.25.0/vectorbt/returns/accessors.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1160 2021-12-11 19:17:59.000000 vectorbt-0.25.0/vectorbt/returns/metrics.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    27796 2021-12-29 18:25:09.000000 vectorbt-0.25.0/vectorbt/returns/nb.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     8672 2021-12-29 18:25:09.000000 vectorbt-0.25.0/vectorbt/returns/qs_adapter.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     5093 2021-12-11 19:17:59.000000 vectorbt-0.25.0/vectorbt/root_accessors.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-04-26 17:40:24.733696 vectorbt-0.25.0/vectorbt/signals/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      712 2021-08-27 15:59:45.000000 vectorbt-0.25.0/vectorbt/signals/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    73582 2021-12-30 14:18:12.000000 vectorbt-0.25.0/vectorbt/signals/accessors.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1842 2021-12-11 19:17:59.000000 vectorbt-0.25.0/vectorbt/signals/enums.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    42731 2021-12-30 14:36:24.000000 vectorbt-0.25.0/vectorbt/signals/factory.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    22617 2021-12-30 14:10:40.000000 vectorbt-0.25.0/vectorbt/signals/generators.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    48870 2021-12-30 14:18:12.000000 vectorbt-0.25.0/vectorbt/signals/nb.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-04-26 17:40:24.734795 vectorbt-0.25.0/vectorbt/templates/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    14983 2021-12-11 19:17:59.000000 vectorbt-0.25.0/vectorbt/templates/dark.json
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    14744 2021-12-11 19:17:59.000000 vectorbt-0.25.0/vectorbt/templates/light.json
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     5645 2021-12-11 19:17:59.000000 vectorbt-0.25.0/vectorbt/templates/seaborn.json
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-04-26 17:40:24.745011 vectorbt-0.25.0/vectorbt/utils/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1229 2021-12-11 19:17:59.000000 vectorbt-0.25.0/vectorbt/utils/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     4205 2021-12-10 15:32:09.000000 vectorbt-0.25.0/vectorbt/utils/array_.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     7841 2021-12-11 19:16:46.000000 vectorbt-0.25.0/vectorbt/utils/attr_.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    18106 2021-12-11 19:17:59.000000 vectorbt-0.25.0/vectorbt/utils/checks.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1611 2021-12-11 19:17:59.000000 vectorbt-0.25.0/vectorbt/utils/colors.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    31370 2021-12-30 15:26:38.000000 vectorbt-0.25.0/vectorbt/utils/config.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     5844 2022-03-17 17:54:25.000000 vectorbt-0.25.0/vectorbt/utils/datetime_.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    21278 2021-12-30 14:18:12.000000 vectorbt-0.25.0/vectorbt/utils/decorators.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     2333 2021-12-30 15:33:01.000000 vectorbt-0.25.0/vectorbt/utils/docs.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1015 2021-10-16 12:03:47.000000 vectorbt-0.25.0/vectorbt/utils/enum_.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     3389 2021-12-10 15:32:09.000000 vectorbt-0.25.0/vectorbt/utils/figure.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     3037 2021-12-11 19:17:59.000000 vectorbt-0.25.0/vectorbt/utils/image_.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     6085 2023-04-26 17:28:11.000000 vectorbt-0.25.0/vectorbt/utils/mapping.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1934 2021-12-11 19:17:59.000000 vectorbt-0.25.0/vectorbt/utils/math_.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     2159 2021-12-11 19:17:59.000000 vectorbt-0.25.0/vectorbt/utils/module_.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     3358 2021-12-30 14:21:04.000000 vectorbt-0.25.0/vectorbt/utils/params.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      493 2021-12-11 19:17:59.000000 vectorbt-0.25.0/vectorbt/utils/random_.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1787 2021-12-11 19:17:59.000000 vectorbt-0.25.0/vectorbt/utils/requests_.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     9968 2021-12-30 14:12:34.000000 vectorbt-0.25.0/vectorbt/utils/schedule_.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1951 2021-12-30 14:12:34.000000 vectorbt-0.25.0/vectorbt/utils/tags.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     8622 2021-12-30 14:12:47.000000 vectorbt-0.25.0/vectorbt/utils/template.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-04-26 17:40:24.701091 vectorbt-0.25.0/vectorbt.egg-info/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     9941 2023-04-26 17:40:24.000000 vectorbt-0.25.0/vectorbt.egg-info/PKG-INFO
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     2937 2023-04-26 17:40:24.000000 vectorbt-0.25.0/vectorbt.egg-info/SOURCES.txt
+-rw-r--r--   0 olegpolakow   (501) staff       (20)        1 2023-04-26 17:40:24.000000 vectorbt-0.25.0/vectorbt.egg-info/dependency_links.txt
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      460 2023-04-26 17:40:24.000000 vectorbt-0.25.0/vectorbt.egg-info/requires.txt
+-rw-r--r--   0 olegpolakow   (501) staff       (20)       15 2023-04-26 17:40:24.000000 vectorbt-0.25.0/vectorbt.egg-info/top_level.txt
```

### Comparing `vectorbt-0.24.5/LICENSE.md` & `vectorbt-0.25.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/PKG-INFO` & `vectorbt-0.25.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectorbt
-Version: 0.24.5
+Version: 0.25.0
 Summary: Python library for backtesting and analyzing trading strategies at scale
 Home-page: https://github.com/polakowo/vectorbt
 Author: Oleg Polakow
 Author-email: olegpolakow@gmail.com
 License: Apache 2.0 with Commons Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `vectorbt-0.24.5/README.md` & `vectorbt-0.25.0/README.md`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/setup.py` & `vectorbt-0.25.0/setup.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/tests/test_base.py` & `vectorbt-0.25.0/tests/test_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,19 +89,19 @@
         assert column_grouper.group_by_to_index(grouped_columns, group_by=None) is None
         pd.testing.assert_index_equal(
             column_grouper.group_by_to_index(grouped_columns, group_by=True),
             pd.Index(['group'] * len(grouped_columns))
         )
         pd.testing.assert_index_equal(
             column_grouper.group_by_to_index(grouped_columns, group_by=0),
-            pd.Int64Index([1, 1, 1, 1, 0, 0, 0, 0], dtype='int64', name='first')
+            pd.Index([1, 1, 1, 1, 0, 0, 0, 0], dtype='int64', name='first')
         )
         pd.testing.assert_index_equal(
             column_grouper.group_by_to_index(grouped_columns, group_by='first'),
-            pd.Int64Index([1, 1, 1, 1, 0, 0, 0, 0], dtype='int64', name='first')
+            pd.Index([1, 1, 1, 1, 0, 0, 0, 0], dtype='int64', name='first')
         )
         pd.testing.assert_index_equal(
             column_grouper.group_by_to_index(grouped_columns, group_by=[0, 1]),
             pd.MultiIndex.from_tuples([
                 (1, 3),
                 (1, 3),
                 (1, 2),
@@ -124,29 +124,29 @@
                 (0, 0),
                 (0, 0)
             ], names=['first', 'second'])
         )
         pd.testing.assert_index_equal(
             column_grouper.group_by_to_index(
                 grouped_columns, group_by=np.array([3, 2, 1, 1, 1, 0, 0, 0])),
-            pd.Int64Index([3, 2, 1, 1, 1, 0, 0, 0], dtype='int64')
+            pd.Index([3, 2, 1, 1, 1, 0, 0, 0], dtype='int64')
         )
         pd.testing.assert_index_equal(
             column_grouper.group_by_to_index(
                 grouped_columns, group_by=pd.Index([3, 2, 1, 1, 1, 0, 0, 0], name='fourth')),
-            pd.Int64Index([3, 2, 1, 1, 1, 0, 0, 0], dtype='int64', name='fourth')
+            pd.Index([3, 2, 1, 1, 1, 0, 0, 0], dtype='int64', name='fourth')
         )
 
     def test_get_groups_and_index(self):
         a, b = column_grouper.get_groups_and_index(grouped_columns, group_by=None)
         np.testing.assert_array_equal(a, np.array([0, 1, 2, 3, 4, 5, 6, 7]))
         pd.testing.assert_index_equal(b, grouped_columns)
         a, b = column_grouper.get_groups_and_index(grouped_columns, group_by=0)
         np.testing.assert_array_equal(a, np.array([0, 0, 0, 0, 1, 1, 1, 1]))
-        pd.testing.assert_index_equal(b, pd.Int64Index([1, 0], dtype='int64', name='first'))
+        pd.testing.assert_index_equal(b, pd.Index([1, 0], dtype='int64', name='first'))
         a, b = column_grouper.get_groups_and_index(grouped_columns, group_by=[0, 1])
         np.testing.assert_array_equal(a, np.array([0, 0, 1, 1, 2, 2, 3, 3]))
         pd.testing.assert_index_equal(b, pd.MultiIndex.from_tuples([
             (1, 3),
             (1, 2),
             (0, 1),
             (0, 0)
@@ -264,23 +264,23 @@
         with pytest.raises(Exception):
             column_grouper.ColumnGrouper(grouped_columns, group_by=0, allow_modify=False).check_group_by(group_by=1)
 
     def test_resolve_group_by(self):
         assert column_grouper.ColumnGrouper(grouped_columns, group_by=None).resolve_group_by() is None  # default
         pd.testing.assert_index_equal(
             column_grouper.ColumnGrouper(grouped_columns, group_by=None).resolve_group_by(group_by=0),  # overrides
-            pd.Int64Index([1, 1, 1, 1, 0, 0, 0, 0], dtype='int64', name='first')
+            pd.Index([1, 1, 1, 1, 0, 0, 0, 0], dtype='int64', name='first')
         )
         pd.testing.assert_index_equal(
             column_grouper.ColumnGrouper(grouped_columns, group_by=0).resolve_group_by(),  # default
-            pd.Int64Index([1, 1, 1, 1, 0, 0, 0, 0], dtype='int64', name='first')
+            pd.Index([1, 1, 1, 1, 0, 0, 0, 0], dtype='int64', name='first')
         )
         pd.testing.assert_index_equal(
             column_grouper.ColumnGrouper(grouped_columns, group_by=0).resolve_group_by(group_by=1),  # overrides
-            pd.Int64Index([3, 3, 2, 2, 1, 1, 0, 0], dtype='int64', name='second')
+            pd.Index([3, 3, 2, 2, 1, 1, 0, 0], dtype='int64', name='second')
         )
 
     def test_get_groups(self):
         np.testing.assert_array_equal(
             column_grouper.ColumnGrouper(grouped_columns).get_groups(),
             np.array([0, 1, 2, 3, 4, 5, 6, 7])
         )
@@ -292,15 +292,15 @@
     def test_get_columns(self):
         pd.testing.assert_index_equal(
             column_grouper.ColumnGrouper(grouped_columns).get_columns(),
             column_grouper.ColumnGrouper(grouped_columns).columns
         )
         pd.testing.assert_index_equal(
             column_grouper.ColumnGrouper(grouped_columns).get_columns(group_by=0),
-            pd.Int64Index([1, 0], dtype='int64', name='first')
+            pd.Index([1, 0], dtype='int64', name='first')
         )
 
     def test_get_group_lens(self):
         np.testing.assert_array_equal(
             column_grouper.ColumnGrouper(grouped_columns).get_group_lens(),
             np.array([1, 1, 1, 1, 1, 1, 1, 1])
         )
@@ -676,15 +676,15 @@
         assert sr2_grouped_wrapper.get_shape_2d() == (3, 1)
         assert df4_grouped_wrapper.shape_2d == (3, 3)
         assert df4_grouped_wrapper.get_shape_2d() == (3, 2)
 
     def test_freq(self):
         assert sr2_wrapper.freq is None
         assert sr2_wrapper.replace(freq='1D').freq == day_dt
-        assert sr2_wrapper.replace(index=pd.Index([
+        assert sr2_wrapper.replace(index=pd.DatetimeIndex([
             datetime(2020, 1, 1),
             datetime(2020, 1, 2),
             datetime(2020, 1, 3)
         ], freq='1D')).freq == day_dt
         assert sr2_wrapper.replace(index=pd.Index([
             datetime(2020, 1, 1),
             datetime(2020, 1, 2),
@@ -1004,19 +1004,19 @@
         pd.testing.assert_index_equal(index_fns.get_index(pd.Series([1, 2, 3]), 1), pd.Index([0]))  # empty
         pd.testing.assert_index_equal(index_fns.get_index(df1, 0), df1.index)
         pd.testing.assert_index_equal(index_fns.get_index(df1, 1), df1.columns)
 
     def test_index_from_values(self):
         pd.testing.assert_index_equal(
             index_fns.index_from_values([0.1, 0.2], name='a'),
-            pd.Float64Index([0.1, 0.2], dtype='float64', name='a')
+            pd.Index([0.1, 0.2], dtype='float64', name='a')
         )
         pd.testing.assert_index_equal(
             index_fns.index_from_values(np.tile(np.arange(1, 4)[:, None][:, None], (1, 3, 3)), name='b'),
-            pd.Int64Index([1, 2, 3], dtype='int64', name='b')
+            pd.Index([1, 2, 3], dtype='int64', name='b')
         )
         pd.testing.assert_index_equal(
             index_fns.index_from_values(np.random.uniform(size=(3, 3, 3)), name='c'),
             pd.Index(['array_0', 'array_1', 'array_2'], dtype='object', name='c')
         )
         pd.testing.assert_index_equal(
             index_fns.index_from_values([(1, 2), (3, 4), (5, 6)], name='c'),
@@ -1034,18 +1034,18 @@
 
         pd.testing.assert_index_equal(
             index_fns.index_from_values([A(), B(), C()], name='c'),
             pd.Index(['A_0', 'B_1', 'C_2'], dtype='object', name='c')
         )
 
     def test_repeat_index(self):
-        i = pd.Int64Index([1, 2, 3], name='i')
+        i = pd.Index([1, 2, 3], name='i')
         pd.testing.assert_index_equal(
             index_fns.repeat_index(i, 3),
-            pd.Int64Index([1, 1, 1, 2, 2, 2, 3, 3, 3], dtype='int64', name='i')
+            pd.Index([1, 1, 1, 2, 2, 2, 3, 3, 3], dtype='int64', name='i')
         )
         pd.testing.assert_index_equal(
             index_fns.repeat_index(multi_i, 3),
             pd.MultiIndex.from_tuples([
                 ('x7', 'x8'),
                 ('x7', 'x8'),
                 ('x7', 'x8'),
@@ -1055,26 +1055,26 @@
                 ('z7', 'z8'),
                 ('z7', 'z8'),
                 ('z7', 'z8')
             ], names=['i7', 'i8'])
         )
         pd.testing.assert_index_equal(
             index_fns.repeat_index([0], 3),  # empty
-            pd.Int64Index([0, 1, 2], dtype='int64')
+            pd.Index([0, 1, 2], dtype='int64')
         )
         pd.testing.assert_index_equal(
             index_fns.repeat_index(sr_none.index, 3),  # simple range
             pd.RangeIndex(start=0, stop=3, step=1)
         )
 
     def test_tile_index(self):
-        i = pd.Int64Index([1, 2, 3], name='i')
+        i = pd.Index([1, 2, 3], name='i')
         pd.testing.assert_index_equal(
             index_fns.tile_index(i, 3),
-            pd.Int64Index([1, 2, 3, 1, 2, 3, 1, 2, 3], dtype='int64', name='i')
+            pd.Index([1, 2, 3, 1, 2, 3, 1, 2, 3], dtype='int64', name='i')
         )
         pd.testing.assert_index_equal(
             index_fns.tile_index(multi_i, 3),
             pd.MultiIndex.from_tuples([
                 ('x7', 'x8'),
                 ('y7', 'y8'),
                 ('z7', 'z8'),
@@ -1084,15 +1084,15 @@
                 ('x7', 'x8'),
                 ('y7', 'y8'),
                 ('z7', 'z8')
             ], names=['i7', 'i8'])
         )
         pd.testing.assert_index_equal(
             index_fns.tile_index([0], 3),  # empty
-            pd.Int64Index([0, 1, 2], dtype='int64')
+            pd.Index([0, 1, 2], dtype='int64')
         )
         pd.testing.assert_index_equal(
             index_fns.tile_index(sr_none.index, 3),  # simple range
             pd.RangeIndex(start=0, stop=3, step=1)
         )
 
     def test_stack_indexes(self):
@@ -1131,15 +1131,15 @@
             pd.MultiIndex.from_tuples([
                 (1, 2),
                 (1, 3)
             ])
         )
         pd.testing.assert_index_equal(
             index_fns.combine_indexes([pd.Index([1]), pd.Index([2, 3])], drop_redundant=True),
-            pd.Int64Index([2, 3], dtype='int64')
+            pd.Index([2, 3], dtype='int64')
         )
         pd.testing.assert_index_equal(
             index_fns.combine_indexes([pd.Index([1], name='i'), pd.Index([2, 3])], drop_redundant=True),
             pd.MultiIndex.from_tuples([
                 (1, 2),
                 (1, 3)
             ], names=['i', None])
@@ -1149,19 +1149,19 @@
             pd.MultiIndex.from_tuples([
                 (1, 3),
                 (2, 3)
             ])
         )
         pd.testing.assert_index_equal(
             index_fns.combine_indexes([pd.Index([1, 2]), pd.Index([3])], drop_redundant=True),
-            pd.Int64Index([1, 2], dtype='int64')
+            pd.Index([1, 2], dtype='int64')
         )
         pd.testing.assert_index_equal(
             index_fns.combine_indexes([pd.Index([1]), pd.Index([2, 3])], drop_redundant=(False, True)),
-            pd.Int64Index([2, 3], dtype='int64')
+            pd.Index([2, 3], dtype='int64')
         )
         pd.testing.assert_index_equal(
             index_fns.combine_indexes([df2.index, df5.index]),
             pd.MultiIndex.from_tuples([
                 ('x4', 'x7', 'x8'),
                 ('x4', 'y7', 'y8'),
                 ('x4', 'z7', 'z8'),
@@ -1197,18 +1197,18 @@
                 ('z7', 'z8')
             ], names=['i7', 'i8'])
         )
         with pytest.raises(Exception):
             _ = index_fns.drop_levels(multi_i, ['i7', 'i8'])
 
     def test_rename_levels(self):
-        i = pd.Int64Index([1, 2, 3], name='i')
+        i = pd.Index([1, 2, 3], name='i')
         pd.testing.assert_index_equal(
             index_fns.rename_levels(i, {'i': 'f'}),
-            pd.Int64Index([1, 2, 3], dtype='int64', name='f')
+            pd.Index([1, 2, 3], dtype='int64', name='f')
         )
         pd.testing.assert_index_equal(
             index_fns.rename_levels(i, {'a': 'b'}, strict=False),
             i
         )
         with pytest.raises(Exception):
             _ = index_fns.rename_levels(i, {'a': 'b'}, strict=True)
@@ -1285,15 +1285,15 @@
             ], names=['hi', 'hi2'])
         )
 
     def test_drop_duplicate_levels(self):
         pd.testing.assert_index_equal(
             index_fns.drop_duplicate_levels(pd.MultiIndex.from_arrays(
                 [[1, 2, 3], [1, 2, 3]], names=['a', 'a'])),
-            pd.Int64Index([1, 2, 3], dtype='int64', name='a')
+            pd.Index([1, 2, 3], dtype='int64', name='a')
         )
         pd.testing.assert_index_equal(
             index_fns.drop_duplicate_levels(pd.MultiIndex.from_tuples(
                 [(0, 1, 2, 1), ('a', 'b', 'c', 'b')], names=['x', 'y', 'z', 'y']), keep='last'),
             pd.MultiIndex.from_tuples([
                 (0, 2, 1),
                 ('a', 'c', 'b')
@@ -2224,16 +2224,16 @@
         pd.testing.assert_frame_equal(
             reshape_fns.unstack_to_df(sr, index_levels=0, column_levels=1),
             pd.DataFrame(
                 np.array([
                     [1.0, 2.0],
                     [3.0, 4.0]
                 ]),
-                index=pd.Int64Index([1, 2], dtype='int64'),
-                columns=pd.Int64Index([3, 4], dtype='int64')
+                index=pd.Index([1, 2], dtype='int64'),
+                columns=pd.Index([3, 4], dtype='int64')
             )
         )
         pd.testing.assert_frame_equal(
             reshape_fns.unstack_to_df(sr, index_levels=(0, 1), column_levels=2),
             pd.DataFrame(
                 np.array([
                     [1.0, np.nan, np.nan, np.nan],
@@ -2255,16 +2255,16 @@
             pd.DataFrame(
                 np.array([
                     [np.nan, np.nan, 1.0, 2.0],
                     [np.nan, np.nan, 3.0, 4.0],
                     [1.0, 3.0, np.nan, np.nan],
                     [2.0, 4.0, np.nan, np.nan]
                 ]),
-                index=pd.Int64Index([1, 2, 3, 4], dtype='int64'),
-                columns=pd.Int64Index([1, 2, 3, 4], dtype='int64')
+                index=pd.Index([1, 2, 3, 4], dtype='int64'),
+                columns=pd.Index([1, 2, 3, 4], dtype='int64')
             )
         )
 
     @pytest.mark.parametrize(
         "test_inputs",
         [
             (0, a1, a2, sr_none, sr1, sr2),
@@ -3055,15 +3055,15 @@
         pd.testing.assert_frame_equal(
             sr2.vbt.apply_and_concat(
                 3, np.array([1, 2, 3]), 10, apply_func=apply_func, d=100
             ),
             pd.DataFrame(
                 target.values,
                 index=target.index,
-                columns=pd.Int64Index([0, 1, 2], dtype='int64', name='apply_idx')
+                columns=pd.Index([0, 1, 2], dtype='int64', name='apply_idx')
             )
         )
 
         def apply_func2(i, x, y, c, d=1):
             return x + y + c + d
 
         pd.testing.assert_frame_equal(
```

### Comparing `vectorbt-0.24.5/tests/test_data.py` & `vectorbt-0.25.0/tests/test_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,28 +325,28 @@
             pd.DataFrame(
                 [
                     [0.15601864044243652],
                     [0.8661761457749352],
                     [0.020584494295802447]
                 ],
                 index=index[1:4],
-                columns=pd.Int64Index([1], dtype='int64')
+                columns=pd.Index([1], dtype='int64')
             )
         )
         pd.testing.assert_frame_equal(
             MyData.download([0, 1], shape=(5, 3), index_mask=index_mask, column_mask=column_mask,
                             missing_index='drop', missing_columns='drop').data[1],
             pd.DataFrame(
                 [
                     [1.15601864044243652],
                     [1.8661761457749352],
                     [1.020584494295802447]
                 ],
                 index=index[1:4],
-                columns=pd.Int64Index([1], dtype='int64')
+                columns=pd.Index([1], dtype='int64')
             )
         )
         with pytest.raises(Exception):
             MyData.download([0, 1], shape=(5, 3), index_mask=index_mask, column_mask=column_mask,
                             missing_index='raise', missing_columns='nan')
         with pytest.raises(Exception):
             MyData.download([0, 1], shape=(5, 3), index_mask=index_mask, column_mask=column_mask,
@@ -675,57 +675,57 @@
             pd.DataFrame(
                 [
                     [0.15601864044243652],
                     [0.8661761457749352],
                     [0.020584494295802447]
                 ],
                 index=index[1:4],
-                columns=pd.Int64Index([1], dtype='int64')
+                columns=pd.Index([1], dtype='int64')
             )
         )
         pd.testing.assert_frame_equal(
             MyData.download([0, 1], shape=(5, 3), index_mask=index_mask, column_mask=column_mask,
                             missing_index='drop', missing_columns='drop')
                 .update(index_mask=update_index_mask).data[1],
             pd.DataFrame(
                 [
                     [1.15601864044243652],
                     [1.8661761457749352],
                     [1.020584494295802447]
                 ],
                 index=index[1:4],
-                columns=pd.Int64Index([1], dtype='int64')
+                columns=pd.Index([1], dtype='int64')
             )
         )
         pd.testing.assert_frame_equal(
             MyData.download([0, 1], shape=(5, 3), index_mask=index_mask, column_mask=column_mask,
                             missing_index='drop', missing_columns='drop')
                 .update(n=2, index_mask=update_index_mask2).data[0],
             pd.DataFrame(
                 [
                     [0.15601864044243652],
                     [0.8661761457749352],
                     [0.020584494295802447]
                 ],
                 index=index[1:4],
-                columns=pd.Int64Index([1], dtype='int64')
+                columns=pd.Index([1], dtype='int64')
             )
         )
         pd.testing.assert_frame_equal(
             MyData.download([0, 1], shape=(5, 3), index_mask=index_mask, column_mask=column_mask,
                             missing_index='drop', missing_columns='drop')
                 .update(n=2, index_mask=update_index_mask2).data[1],
             pd.DataFrame(
                 [
                     [1.15601864044243652],
                     [1.8661761457749352],
                     [1.020584494295802447]
                 ],
                 index=index[1:4],
-                columns=pd.Int64Index([1], dtype='int64')
+                columns=pd.Index([1], dtype='int64')
             )
         )
 
     def test_concat(self):
         index = pd.DatetimeIndex(
             [
                 '2020-01-01 00:00:00',
@@ -758,15 +758,15 @@
                     [0.3745401188473625, 1.3745401188473625],
                     [0.9507143064099162, 1.9507143064099162],
                     [0.7319939418114051, 1.7319939418114051],
                     [0.5986584841970366, 1.5986584841970366],
                     [0.15601864044243652, 1.15601864044243652]
                 ],
                 index=index,
-                columns=pd.Int64Index([0, 1], dtype='int64', name='symbol')
+                columns=pd.Index([0, 1], dtype='int64', name='symbol')
             )
         )
         pd.testing.assert_series_equal(
             MyData.download(0, shape=(5, 3), columns=['feat0', 'feat1', 'feat2']).concat()['feat0'],
             pd.Series(
                 [
                     0.3745401188473625,
@@ -814,43 +814,43 @@
                     [0.3745401188473625, 1.3745401188473625],
                     [0.5986584841970366, 1.5986584841970366],
                     [0.05808361216819946, 1.05808361216819946],
                     [0.7080725777960455, 1.7080725777960455],
                     [0.8324426408004217, 1.8324426408004217]
                 ],
                 index=index,
-                columns=pd.Int64Index([0, 1], dtype='int64', name='symbol')
+                columns=pd.Index([0, 1], dtype='int64', name='symbol')
             )
         )
         pd.testing.assert_frame_equal(
             MyData.download([0, 1], shape=(5, 3), columns=['feat0', 'feat1', 'feat2']).concat()['feat1'],
             pd.DataFrame(
                 [
                     [0.9507143064099162, 1.9507143064099162],
                     [0.15601864044243652, 1.15601864044243652],
                     [0.8661761457749352, 1.8661761457749352],
                     [0.020584494295802447, 1.020584494295802447],
                     [0.21233911067827616, 1.21233911067827616]
                 ],
                 index=index,
-                columns=pd.Int64Index([0, 1], dtype='int64', name='symbol')
+                columns=pd.Index([0, 1], dtype='int64', name='symbol')
             )
         )
         pd.testing.assert_frame_equal(
             MyData.download([0, 1], shape=(5, 3), columns=['feat0', 'feat1', 'feat2']).concat()['feat2'],
             pd.DataFrame(
                 [
                     [0.7319939418114051, 1.7319939418114051],
                     [0.15599452033620265, 1.15599452033620265],
                     [0.6011150117432088, 1.6011150117432088],
                     [0.9699098521619943, 1.9699098521619943],
                     [0.18182496720710062, 1.18182496720710062]
                 ],
                 index=index,
-                columns=pd.Int64Index([0, 1], dtype='int64', name='symbol')
+                columns=pd.Index([0, 1], dtype='int64', name='symbol')
             )
         )
 
     def test_get(self):
         index = pd.DatetimeIndex(
             [
                 '2020-01-01 00:00:00',
@@ -911,57 +911,57 @@
                     [0.3745401188473625, 1.3745401188473625],
                     [0.9507143064099162, 1.9507143064099162],
                     [0.7319939418114051, 1.7319939418114051],
                     [0.5986584841970366, 1.5986584841970366],
                     [0.15601864044243652, 1.15601864044243652]
                 ],
                 index=index,
-                columns=pd.Int64Index([0, 1], dtype='int64', name='symbol')
+                columns=pd.Index([0, 1], dtype='int64', name='symbol')
             )
         )
         pd.testing.assert_frame_equal(
             MyData.download([0, 1], shape=(5, 3), columns=['feat0', 'feat1', 'feat2']).get('feat0'),
             pd.DataFrame(
                 [
                     [0.3745401188473625, 1.3745401188473625],
                     [0.5986584841970366, 1.5986584841970366],
                     [0.05808361216819946, 1.05808361216819946],
                     [0.7080725777960455, 1.7080725777960455],
                     [0.8324426408004217, 1.8324426408004217]
                 ],
                 index=index,
-                columns=pd.Int64Index([0, 1], dtype='int64', name='symbol')
+                columns=pd.Index([0, 1], dtype='int64', name='symbol')
             )
         )
         pd.testing.assert_frame_equal(
             MyData.download([0, 1], shape=(5, 3), columns=['feat0', 'feat1', 'feat2']).get(['feat0', 'feat1'])[0],
             pd.DataFrame(
                 [
                     [0.3745401188473625, 1.3745401188473625],
                     [0.5986584841970366, 1.5986584841970366],
                     [0.05808361216819946, 1.05808361216819946],
                     [0.7080725777960455, 1.7080725777960455],
                     [0.8324426408004217, 1.8324426408004217]
                 ],
                 index=index,
-                columns=pd.Int64Index([0, 1], dtype='int64', name='symbol')
+                columns=pd.Index([0, 1], dtype='int64', name='symbol')
             )
         )
         pd.testing.assert_frame_equal(
             MyData.download([0, 1], shape=(5, 3), columns=['feat0', 'feat1', 'feat2']).get()[0],
             pd.DataFrame(
                 [
                     [0.3745401188473625, 1.3745401188473625],
                     [0.5986584841970366, 1.5986584841970366],
                     [0.05808361216819946, 1.05808361216819946],
                     [0.7080725777960455, 1.7080725777960455],
                     [0.8324426408004217, 1.8324426408004217]
                 ],
                 index=index,
-                columns=pd.Int64Index([0, 1], dtype='int64', name='symbol')
+                columns=pd.Index([0, 1], dtype='int64', name='symbol')
             )
         )
 
     def test_indexing(self):
         assert MyData.download([0, 1], shape=(5,), columns='feat0').iloc[:3].wrapper == \
                MyData.download([0, 1], shape=(3,), columns='feat0').wrapper
         assert MyData.download([0, 1], shape=(5, 3), columns=['feat0', 'feat1', 'feat2']).iloc[:3].wrapper == \
@@ -986,40 +986,40 @@
 
         stats_index = pd.Index([
             'Start', 'End', 'Period', 'Total Symbols', 'Null Counts: 0', 'Null Counts: 1'
         ], dtype='object')
         pd.testing.assert_series_equal(
             data.stats(),
             pd.Series([
-                pd.Timestamp('2020-01-01 00:00:00+0000', tz='UTC', freq='D'),
-                pd.Timestamp('2020-01-05 00:00:00+0000', tz='UTC', freq='D'),
+                pd.Timestamp('2020-01-01 00:00:00+0000', tz='UTC'),
+                pd.Timestamp('2020-01-05 00:00:00+0000', tz='UTC'),
                 pd.Timedelta('5 days 00:00:00'),
                 2, 2.3333333333333335, 2.3333333333333335
             ],
                 index=stats_index,
                 name='agg_func_mean'
             )
         )
         pd.testing.assert_series_equal(
             data.stats(column='feat0'),
             pd.Series([
-                pd.Timestamp('2020-01-01 00:00:00+0000', tz='UTC', freq='D'),
-                pd.Timestamp('2020-01-05 00:00:00+0000', tz='UTC', freq='D'),
+                pd.Timestamp('2020-01-01 00:00:00+0000', tz='UTC'),
+                pd.Timestamp('2020-01-05 00:00:00+0000', tz='UTC'),
                 pd.Timedelta('5 days 00:00:00'),
                 2, 5, 1
             ],
                 index=stats_index,
                 name='feat0'
             )
         )
         pd.testing.assert_series_equal(
             data.stats(group_by=True),
             pd.Series([
-                pd.Timestamp('2020-01-01 00:00:00+0000', tz='UTC', freq='D'),
-                pd.Timestamp('2020-01-05 00:00:00+0000', tz='UTC', freq='D'),
+                pd.Timestamp('2020-01-01 00:00:00+0000', tz='UTC'),
+                pd.Timestamp('2020-01-05 00:00:00+0000', tz='UTC'),
                 pd.Timedelta('5 days 00:00:00'),
                 2, 7, 7
             ],
                 index=stats_index,
                 name='group'
             )
         )
```

### Comparing `vectorbt-0.24.5/tests/test_generic.py` & `vectorbt-0.25.0/tests/test_generic.py`

 * *Files 2% similar despite different names*

```diff
@@ -353,27 +353,27 @@
         )
         pd.testing.assert_frame_equal(
             df.vbt.ewm_mean(test_window),
             df.ewm(span=test_window).mean()
         )
 
     @pytest.mark.parametrize(
-        "test_window,test_minp,test_adjust,test_ddof",
-        list(product([1, 2, 3, 4, 5], [1, None], [False, True], [0, 1]))
+        "test_window,test_minp,test_adjust",
+        list(product([1, 2, 3, 4, 5], [1, None], [False, True]))
     )
-    def test_ewm_std(self, test_window, test_minp, test_adjust, test_ddof):
+    def test_ewm_std(self, test_window, test_minp, test_adjust):
         if test_minp is None:
             test_minp = test_window
         pd.testing.assert_series_equal(
-            df['a'].vbt.ewm_std(test_window, minp=test_minp, adjust=test_adjust, ddof=test_ddof),
-            df['a'].ewm(span=test_window, min_periods=test_minp, adjust=test_adjust).std(ddof=test_ddof)
+            df['a'].vbt.ewm_std(test_window, minp=test_minp, adjust=test_adjust),
+            df['a'].ewm(span=test_window, min_periods=test_minp, adjust=test_adjust).std()
         )
         pd.testing.assert_frame_equal(
-            df.vbt.ewm_std(test_window, minp=test_minp, adjust=test_adjust, ddof=test_ddof),
-            df.ewm(span=test_window, min_periods=test_minp, adjust=test_adjust).std(ddof=test_ddof)
+            df.vbt.ewm_std(test_window, minp=test_minp, adjust=test_adjust),
+            df.ewm(span=test_window, min_periods=test_minp, adjust=test_adjust).std()
         )
         pd.testing.assert_frame_equal(
             df.vbt.ewm_std(test_window),
             df.ewm(span=test_window).std()
         )
 
     @pytest.mark.parametrize(
@@ -543,15 +543,15 @@
             df.vbt.groupby_apply(np.asarray([1, 1, 2, 2, 3]), i_nanmean_nb, on_matrix=True),
             pd.DataFrame(
                 np.array([
                     [2., 2., 2.],
                     [2.8, 2.8, 2.8],
                     [1., 1., 1.]
                 ]),
-                index=pd.Int64Index([1, 2, 3], dtype='int64'),
+                index=pd.Index([1, 2, 3], dtype='int64'),
                 columns=df.columns
             )
         )
 
     @pytest.mark.parametrize(
         "test_freq",
         ['1h', '3d', '1w'],
@@ -777,15 +777,15 @@
         )
         pd.testing.assert_series_equal(
             pd.DataFrame([[False, True], [False, True]]).vbt.flatten_grouped(group_by=True, order='F'),
             pd.Series([False, False, True, True], name='group')
         )
         pd.testing.assert_frame_equal(
             pd.Series([False, True, True, False]).vbt.flatten_grouped(group_by=[0, 0, 0, 1]),
-            pd.DataFrame([[0., 0.], [1., np.nan], [1., np.nan]], columns=pd.Int64Index([0, 1], dtype='int64'))
+            pd.DataFrame([[0., 0.], [1., np.nan], [1., np.nan]], columns=pd.Index([0, 1], dtype='int64'))
         )
 
     @pytest.mark.parametrize(
         "test_name,test_func,test_func_nb",
         [
             ('min', lambda x, **kwargs: x.min(**kwargs), nb.nanmin_nb),
             ('max', lambda x, **kwargs: x.max(**kwargs), nb.nanmax_nb),
@@ -875,15 +875,15 @@
         )
 
     def test_value_counts(self):
         pd.testing.assert_series_equal(
             df['a'].vbt.value_counts(),
             pd.Series(
                 np.array([1, 1, 1, 1, 1]),
-                index=pd.Float64Index([1.0, 2.0, 3.0, 4.0, np.nan], dtype='float64'),
+                index=pd.Index([1.0, 2.0, 3.0, 4.0, np.nan], dtype='float64'),
                 name='a'
             )
         )
         mapping = {1.: 'one', 2.: 'two', 3.: 'three', 4.: 'four'}
         pd.testing.assert_series_equal(
             df['a'].vbt.value_counts(mapping=mapping),
             pd.Series(
@@ -898,98 +898,98 @@
                 np.array([
                     [1, 1, 2],
                     [1, 1, 2],
                     [1, 1, 0],
                     [1, 1, 0],
                     [1, 1, 1]
                 ]),
-                index=pd.Float64Index([1.0, 2.0, 3.0, 4.0, np.nan], dtype='float64'),
+                index=pd.Index([1.0, 2.0, 3.0, 4.0, np.nan], dtype='float64'),
                 columns=df.columns
             )
         )
         pd.testing.assert_frame_equal(
             df.vbt.value_counts(group_by=group_by),
             pd.DataFrame(
                 np.array([
                     [2, 2],
                     [2, 2],
                     [2, 0],
                     [2, 0],
                     [2, 1]
                 ]),
-                index=pd.Float64Index([1.0, 2.0, 3.0, 4.0, np.nan], dtype='float64'),
+                index=pd.Index([1.0, 2.0, 3.0, 4.0, np.nan], dtype='float64'),
                 columns=pd.Index(['g1', 'g2'], dtype='object')
             )
         )
         pd.testing.assert_frame_equal(
             df.vbt.value_counts(sort_uniques=False),
             pd.DataFrame(
                 np.array([
                     [1, 1, 2],
                     [1, 1, 2],
                     [1, 1, 0],
                     [1, 1, 0],
                     [1, 1, 1]
                 ]),
-                index=pd.Float64Index([1.0, 2.0, 4.0, 3.0, np.nan], dtype='float64'),
+                index=pd.Index([1.0, 2.0, 4.0, 3.0, np.nan], dtype='float64'),
                 columns=df.columns
             )
         )
         pd.testing.assert_frame_equal(
             df.vbt.value_counts(sort=True),
             pd.DataFrame(
                 np.array([
                     [1, 1, 2],
                     [1, 1, 2],
                     [1, 1, 1],
                     [1, 1, 0],
                     [1, 1, 0]
                 ]),
-                index=pd.Float64Index([1.0, 2.0, np.nan, 3.0, 4.0], dtype='float64'),
+                index=pd.Index([1.0, 2.0, np.nan, 3.0, 4.0], dtype='float64'),
                 columns=df.columns
             )
         )
         pd.testing.assert_frame_equal(
             df.vbt.value_counts(sort=True, ascending=True),
             pd.DataFrame(
                 np.array([
                     [1, 1, 0],
                     [1, 1, 0],
                     [1, 1, 1],
                     [1, 1, 2],
                     [1, 1, 2]
                 ]),
-                index=pd.Float64Index([3.0, 4.0, np.nan, 1.0, 2.0], dtype='float64'),
+                index=pd.Index([3.0, 4.0, np.nan, 1.0, 2.0], dtype='float64'),
                 columns=df.columns
             )
         )
         pd.testing.assert_frame_equal(
             df.vbt.value_counts(sort=True, normalize=True),
             pd.DataFrame(
                 np.array([
                     [0.06666666666666667, 0.06666666666666667, 0.13333333333333333],
                     [0.06666666666666667, 0.06666666666666667, 0.13333333333333333],
                     [0.06666666666666667, 0.06666666666666667, 0.06666666666666667],
                     [0.06666666666666667, 0.06666666666666667, 0.0],
                     [0.06666666666666667, 0.06666666666666667, 0.0]
                 ]),
-                index=pd.Float64Index([1.0, 2.0, np.nan, 3.0, 4.0], dtype='float64'),
+                index=pd.Index([1.0, 2.0, np.nan, 3.0, 4.0], dtype='float64'),
                 columns=df.columns
             )
         )
         pd.testing.assert_frame_equal(
             df.vbt.value_counts(sort=True, normalize=True, dropna=True),
             pd.DataFrame(
                 np.array([
                     [0.08333333333333333, 0.08333333333333333, 0.16666666666666666],
                     [0.08333333333333333, 0.08333333333333333, 0.16666666666666666],
                     [0.08333333333333333, 0.08333333333333333, 0.0],
                     [0.08333333333333333, 0.08333333333333333, 0.0]
                 ]),
-                index=pd.Float64Index([1.0, 2.0, 3.0, 4.0], dtype='float64'),
+                index=pd.Index([1.0, 2.0, 3.0, 4.0], dtype='float64'),
                 columns=df.columns
             )
         )
 
     def test_drawdown(self):
         pd.testing.assert_series_equal(
             df['a'].vbt.drawdown(),
@@ -1051,15 +1051,15 @@
                 np.array([
                     [1.0, 1.0],
                     [2.0, 2.0],
                     [3.0, 3.0],
                     [np.nan, 4.0]
                 ]),
                 index=pd.RangeIndex(start=0, stop=4, step=1),
-                columns=pd.Int64Index([0, 1], dtype='int64', name='split_idx')
+                columns=pd.Index([0, 1], dtype='int64', name='split_idx')
             )
         )
         target = [
             pd.DatetimeIndex(['2018-01-01', '2018-01-02', '2018-01-03'],
                              dtype='datetime64[ns]', name='split_0', freq=None),
             pd.DatetimeIndex(['2018-01-01', '2018-01-02', '2018-01-03', '2018-01-04'],
                              dtype='datetime64[ns]', name='split_1', freq=None)
@@ -1072,15 +1072,15 @@
         pd.testing.assert_frame_equal(
             test_df,
             pd.DataFrame(
                 np.array([
                     [4.0, np.nan]
                 ]),
                 index=pd.RangeIndex(start=0, stop=1, step=1),
-                columns=pd.Int64Index([0, 1], dtype='int64', name='split_idx')
+                columns=pd.Index([0, 1], dtype='int64', name='split_idx')
             )
         )
         target = [
             pd.DatetimeIndex(['2018-01-04'], dtype='datetime64[ns]', name='split_0', freq=None),
             pd.DatetimeIndex(['2018-01-05'], dtype='datetime64[ns]', name='split_1', freq=None)
         ]
         for i in range(len(target)):
@@ -1152,15 +1152,15 @@
             df['a'].vbt.range_split(n=2)[0],
             pd.DataFrame(
                 np.array([
                     [1., 4.],
                     [2., np.nan]
                 ]),
                 index=pd.RangeIndex(start=0, stop=2, step=1),
-                columns=pd.Int64Index([0, 1], dtype='int64', name='split_idx')
+                columns=pd.Index([0, 1], dtype='int64', name='split_idx')
             )
         )
         target = [
             pd.DatetimeIndex(['2018-01-01', '2018-01-02'], dtype='datetime64[ns]', name='split_0', freq=None),
             pd.DatetimeIndex(['2018-01-04', '2018-01-05'], dtype='datetime64[ns]', name='split_1', freq=None)
         ]
         for i in range(len(target)):
@@ -1172,15 +1172,15 @@
             df['a'].vbt.range_split(range_len=2)[0],
             pd.DataFrame(
                 np.array([
                     [1., 2., 3., 4.],
                     [2., 3., 4., np.nan]
                 ]),
                 index=pd.RangeIndex(start=0, stop=2, step=1),
-                columns=pd.Int64Index([0, 1, 2, 3], dtype='int64', name='split_idx')
+                columns=pd.Index([0, 1, 2, 3], dtype='int64', name='split_idx')
             )
         )
         target = [
             pd.DatetimeIndex(['2018-01-01', '2018-01-02'], dtype='datetime64[ns]', name='split_0', freq=None),
             pd.DatetimeIndex(['2018-01-02', '2018-01-03'], dtype='datetime64[ns]', name='split_1', freq=None),
             pd.DatetimeIndex(['2018-01-03', '2018-01-04'], dtype='datetime64[ns]', name='split_2', freq=None),
             pd.DatetimeIndex(['2018-01-04', '2018-01-05'], dtype='datetime64[ns]', name='split_3', freq=None)
@@ -1194,15 +1194,15 @@
             df['a'].vbt.range_split(range_len=2, n=3)[0],
             pd.DataFrame(
                 np.array([
                     [1., 3., 4.],
                     [2., 4., np.nan]
                 ]),
                 index=pd.RangeIndex(start=0, stop=2, step=1),
-                columns=pd.Int64Index([0, 1, 2], dtype='int64', name='split_idx')
+                columns=pd.Index([0, 1, 2], dtype='int64', name='split_idx')
             )
         )
         target = [
             pd.DatetimeIndex(['2018-01-01', '2018-01-02'], dtype='datetime64[ns]', name='split_0', freq=None),
             pd.DatetimeIndex(['2018-01-03', '2018-01-04'], dtype='datetime64[ns]', name='split_1', freq=None),
             pd.DatetimeIndex(['2018-01-04', '2018-01-05'], dtype='datetime64[ns]', name='split_2', freq=None)
         ]
@@ -1216,15 +1216,15 @@
             pd.DataFrame(
                 np.array([
                     [1., 3.],
                     [2., 4.],
                     [3., np.nan]
                 ]),
                 index=pd.RangeIndex(start=0, stop=3, step=1),
-                columns=pd.Int64Index([0, 1], dtype='int64', name='split_idx')
+                columns=pd.Index([0, 1], dtype='int64', name='split_idx')
             )
         )
         target = [
             pd.DatetimeIndex(['2018-01-01', '2018-01-02', '2018-01-03'],
                              dtype='datetime64[ns]', name='split_0', freq=None),
             pd.DatetimeIndex(['2018-01-03', '2018-01-04', '2018-01-05'],
                              dtype='datetime64[ns]', name='split_1', freq=None)
@@ -1239,15 +1239,15 @@
             pd.DataFrame(
                 np.array([
                     [1.0, np.nan, 1.0, 4.0, 2.0, 2.0],
                     [2.0, 4.0, 2.0, np.nan, 1.0, 1.0]
                 ]),
                 index=pd.RangeIndex(start=0, stop=2, step=1),
                 columns=pd.MultiIndex.from_arrays([
-                    pd.Int64Index([0, 0, 0, 1, 1, 1], dtype='int64', name='split_idx'),
+                    pd.Index([0, 0, 0, 1, 1, 1], dtype='int64', name='split_idx'),
                     pd.Index(['a', 'b', 'c', 'a', 'b', 'c'], dtype='object')
                 ])
             )
         )
         target = [
             pd.DatetimeIndex(['2018-01-01', '2018-01-02'], dtype='datetime64[ns]', name='split_0', freq=None),
             pd.DatetimeIndex(['2018-01-04', '2018-01-05'], dtype='datetime64[ns]', name='split_1', freq=None)
@@ -1263,15 +1263,15 @@
                 np.array([
                     [1.0, np.nan, 1.0, 2.0, 4.0, 2.0],
                     [2.0, 4.0, 2.0, 3.0, 3.0, np.nan],
                     [3.0, 3.0, np.nan, 4.0, 2.0, 2.0]
                 ]),
                 index=pd.RangeIndex(start=0, stop=3, step=1),
                 columns=pd.MultiIndex.from_arrays([
-                    pd.Int64Index([0, 0, 0, 1, 1, 1], dtype='int64', name='split_idx'),
+                    pd.Index([0, 0, 0, 1, 1, 1], dtype='int64', name='split_idx'),
                     pd.Index(['a', 'b', 'c', 'a', 'b', 'c'], dtype='object')
                 ])
             )
         )
         target = [
             pd.DatetimeIndex(['2018-01-01', '2018-01-02', '2018-01-03'],
                              dtype='datetime64[ns]', name='split_0', freq=None),
@@ -1289,15 +1289,15 @@
                 np.array([
                     [1.0, np.nan, 1.0, 2.0, 4.0, 2.0],
                     [2.0, 4.0, 2.0, 3.0, 3.0, np.nan],
                     [3.0, 3.0, np.nan, 4.0, 2.0, 2.0]
                 ]),
                 index=pd.RangeIndex(start=0, stop=3, step=1),
                 columns=pd.MultiIndex.from_arrays([
-                    pd.Int64Index([0, 0, 0, 1, 1, 1], dtype='int64', name='split_idx'),
+                    pd.Index([0, 0, 0, 1, 1, 1], dtype='int64', name='split_idx'),
                     pd.Index(['a', 'b', 'c', 'a', 'b', 'c'], dtype='object')
                 ])
             )
         )
         target = [
             pd.DatetimeIndex(['2018-01-01', '2018-01-02', '2018-01-03'],
                              dtype='datetime64[ns]', name='split_0', freq=None),
@@ -1316,15 +1316,15 @@
                     [1.0, np.nan, 1.0, 1.0, np.nan, 1.0],
                     [2.0, 4.0, 2.0, 2.0, 4.0, 2.0],
                     [3.0, 3.0, np.nan, 3.0, 3.0, np.nan],
                     [np.nan, np.nan, np.nan, 4.0, 2.0, 2.0]
                 ]),
                 index=pd.RangeIndex(start=0, stop=4, step=1),
                 columns=pd.MultiIndex.from_arrays([
-                    pd.Int64Index([0, 0, 0, 1, 1, 1], dtype='int64', name='split_idx'),
+                    pd.Index([0, 0, 0, 1, 1, 1], dtype='int64', name='split_idx'),
                     pd.Index(['a', 'b', 'c', 'a', 'b', 'c'], dtype='object')
                 ])
             )
         )
         target = [
             pd.DatetimeIndex(['2018-01-01', '2018-01-02', '2018-01-03'],
                              dtype='datetime64[ns]', name='split_0', freq=None),
@@ -1354,15 +1354,15 @@
             df1,
             pd.DataFrame(
                 np.array([
                     [1.0, 2.0],
                     [2.0, 3.0]
                 ]),
                 index=pd.RangeIndex(start=0, stop=2, step=1),
-                columns=pd.Int64Index([0, 1], dtype='int64', name='split_idx')
+                columns=pd.Index([0, 1], dtype='int64', name='split_idx')
             )
         )
         target = [
             pd.DatetimeIndex(['2018-01-01', '2018-01-02'], dtype='datetime64[ns]', name='split_0', freq=None),
             pd.DatetimeIndex(['2018-01-02', '2018-01-03'], dtype='datetime64[ns]', name='split_1', freq=None)
         ]
         for i in range(len(target)):
@@ -1373,15 +1373,15 @@
         pd.testing.assert_frame_equal(
             df2,
             pd.DataFrame(
                 np.array([
                     [3.0, 4.0]
                 ]),
                 index=pd.RangeIndex(start=0, stop=1, step=1),
-                columns=pd.Int64Index([0, 1], dtype='int64', name='split_idx')
+                columns=pd.Index([0, 1], dtype='int64', name='split_idx')
             )
         )
         target = [
             pd.DatetimeIndex(['2018-01-03'], dtype='datetime64[ns]', name='split_0', freq=None),
             pd.DatetimeIndex(['2018-01-04'], dtype='datetime64[ns]', name='split_1', freq=None)
         ]
         for i in range(len(target)):
@@ -1392,15 +1392,15 @@
         pd.testing.assert_frame_equal(
             df3,
             pd.DataFrame(
                 np.array([
                     [4.0, np.nan]
                 ]),
                 index=pd.RangeIndex(start=0, stop=1, step=1),
-                columns=pd.Int64Index([0, 1], dtype='int64', name='split_idx')
+                columns=pd.Index([0, 1], dtype='int64', name='split_idx')
             )
         )
         target = [
             pd.DatetimeIndex(['2018-01-04'], dtype='datetime64[ns]', name='split_0', freq=None),
             pd.DatetimeIndex(['2018-01-05'], dtype='datetime64[ns]', name='split_1', freq=None)
         ]
         for i in range(len(target)):
@@ -1413,15 +1413,15 @@
         pd.testing.assert_frame_equal(
             df1,
             pd.DataFrame(
                 np.array([
                     [1.0, 2.0]
                 ]),
                 index=pd.RangeIndex(start=0, stop=1, step=1),
-                columns=pd.Int64Index([0, 1], dtype='int64', name='split_idx')
+                columns=pd.Index([0, 1], dtype='int64', name='split_idx')
             )
         )
         target = [
             pd.DatetimeIndex(['2018-01-01'], dtype='datetime64[ns]', name='split_0', freq=None),
             pd.DatetimeIndex(['2018-01-02'], dtype='datetime64[ns]', name='split_1', freq=None)
         ]
         for i in range(len(target)):
@@ -1432,15 +1432,15 @@
         pd.testing.assert_frame_equal(
             df2,
             pd.DataFrame(
                 np.array([
                     [2.0, 3.0]
                 ]),
                 index=pd.RangeIndex(start=0, stop=1, step=1),
-                columns=pd.Int64Index([0, 1], dtype='int64', name='split_idx')
+                columns=pd.Index([0, 1], dtype='int64', name='split_idx')
             )
         )
         target = [
             pd.DatetimeIndex(['2018-01-02'], dtype='datetime64[ns]', name='split_0', freq=None),
             pd.DatetimeIndex(['2018-01-03'], dtype='datetime64[ns]', name='split_1', freq=None)
         ]
         for i in range(len(target)):
@@ -1452,15 +1452,15 @@
             df3,
             pd.DataFrame(
                 np.array([
                     [3.0, 4.0],
                     [4.0, np.nan]
                 ]),
                 index=pd.RangeIndex(start=0, stop=2, step=1),
-                columns=pd.Int64Index([0, 1], dtype='int64', name='split_idx')
+                columns=pd.Index([0, 1], dtype='int64', name='split_idx')
             )
         )
         target = [
             pd.DatetimeIndex(['2018-01-03', '2018-01-04'], dtype='datetime64[ns]', name='split_0', freq=None),
             pd.DatetimeIndex(['2018-01-04', '2018-01-05'], dtype='datetime64[ns]', name='split_1', freq=None)
         ]
         for i in range(len(target)):
@@ -1474,15 +1474,15 @@
             df1,
             pd.DataFrame(
                 np.array([
                     [1.0, 2.0],
                     [2.0, np.nan]
                 ]),
                 index=pd.RangeIndex(start=0, stop=2, step=1),
-                columns=pd.Int64Index([0, 1], dtype='int64', name='split_idx')
+                columns=pd.Index([0, 1], dtype='int64', name='split_idx')
             )
         )
         target = [
             pd.DatetimeIndex(['2018-01-01', '2018-01-02'], dtype='datetime64[ns]', name='split_0', freq=None),
             pd.DatetimeIndex(['2018-01-02'], dtype='datetime64[ns]', name='split_1', freq=None)
         ]
         for i in range(len(target)):
@@ -1493,15 +1493,15 @@
         pd.testing.assert_frame_equal(
             df2,
             pd.DataFrame(
                 np.array([
                     [3.0, 3.0]
                 ]),
                 index=pd.RangeIndex(start=0, stop=1, step=1),
-                columns=pd.Int64Index([0, 1], dtype='int64', name='split_idx')
+                columns=pd.Index([0, 1], dtype='int64', name='split_idx')
             )
         )
         target = [
             pd.DatetimeIndex(['2018-01-03'], dtype='datetime64[ns]', name='split_0', freq=None),
             pd.DatetimeIndex(['2018-01-03'], dtype='datetime64[ns]', name='split_1', freq=None)
         ]
         for i in range(len(target)):
@@ -1513,15 +1513,15 @@
             df3,
             pd.DataFrame(
                 np.array([
                     [4.0, 4.0],
                     [np.nan, np.nan]
                 ]),
                 index=pd.RangeIndex(start=0, stop=2, step=1),
-                columns=pd.Int64Index([0, 1], dtype='int64', name='split_idx')
+                columns=pd.Index([0, 1], dtype='int64', name='split_idx')
             )
         )
         target = [
             pd.DatetimeIndex(['2018-01-04'], dtype='datetime64[ns]', name='split_0', freq=None),
             pd.DatetimeIndex(['2018-01-04', '2018-01-05'], dtype='datetime64[ns]', name='split_1', freq=None)
         ]
         for i in range(len(target)):
@@ -1534,15 +1534,15 @@
             df1,
             pd.DataFrame(
                 np.array([
                     [1.0, 4.0],
                     [2.0, np.nan]
                 ]),
                 index=pd.RangeIndex(start=0, stop=2, step=1),
-                columns=pd.Int64Index([0, 1], dtype='int64', name='split_idx')
+                columns=pd.Index([0, 1], dtype='int64', name='split_idx')
             )
         )
         target = [
             pd.DatetimeIndex(['2018-01-01', '2018-01-02'], dtype='datetime64[ns]', name='split_0', freq=None),
             pd.DatetimeIndex(['2018-01-04', '2018-01-05'], dtype='datetime64[ns]', name='split_1', freq=None)
         ]
         df1, indexes1 = df['a'].vbt.rolling_split(window_len=0.4, n=2)
@@ -1550,15 +1550,15 @@
             df1,
             pd.DataFrame(
                 np.array([
                     [1.0, 4.0],
                     [2.0, np.nan]
                 ]),
                 index=pd.RangeIndex(start=0, stop=2, step=1),
-                columns=pd.Int64Index([0, 1], dtype='int64', name='split_idx')
+                columns=pd.Index([0, 1], dtype='int64', name='split_idx')
             )
         )
         target = [
             pd.DatetimeIndex(['2018-01-01', '2018-01-02'], dtype='datetime64[ns]', name='split_0', freq=None),
             pd.DatetimeIndex(['2018-01-04', '2018-01-05'], dtype='datetime64[ns]', name='split_1', freq=None)
         ]
         for i in range(len(target)):
@@ -1585,15 +1585,15 @@
             pd.DataFrame(
                 np.array([
                     [1.0, 1.0],
                     [2.0, 2.0],
                     [np.nan, 3.0]
                 ]),
                 index=pd.RangeIndex(start=0, stop=3, step=1),
-                columns=pd.Int64Index([0, 1], dtype='int64', name='split_idx')
+                columns=pd.Index([0, 1], dtype='int64', name='split_idx')
             )
         )
         target = [
             pd.DatetimeIndex(['2018-01-01', '2018-01-02'],
                              dtype='datetime64[ns]', name='split_0', freq=None),
             pd.DatetimeIndex(['2018-01-01', '2018-01-02', '2018-01-03'],
                              dtype='datetime64[ns]', name='split_1', freq=None)
@@ -1606,15 +1606,15 @@
         pd.testing.assert_frame_equal(
             df2,
             pd.DataFrame(
                 np.array([
                     [3.0, 4.0]
                 ]),
                 index=pd.RangeIndex(start=0, stop=1, step=1),
-                columns=pd.Int64Index([0, 1], dtype='int64', name='split_idx')
+                columns=pd.Index([0, 1], dtype='int64', name='split_idx')
             )
         )
         target = [
             pd.DatetimeIndex(['2018-01-03'], dtype='datetime64[ns]', name='split_0', freq=None),
             pd.DatetimeIndex(['2018-01-04'], dtype='datetime64[ns]', name='split_1', freq=None)
         ]
         for i in range(len(target)):
@@ -1625,15 +1625,15 @@
         pd.testing.assert_frame_equal(
             df3,
             pd.DataFrame(
                 np.array([
                     [4.0, np.nan]
                 ]),
                 index=pd.RangeIndex(start=0, stop=1, step=1),
-                columns=pd.Int64Index([0, 1], dtype='int64', name='split_idx')
+                columns=pd.Index([0, 1], dtype='int64', name='split_idx')
             )
         )
         target = [
             pd.DatetimeIndex(['2018-01-04'], dtype='datetime64[ns]', name='split_0', freq=None),
             pd.DatetimeIndex(['2018-01-05'], dtype='datetime64[ns]', name='split_1', freq=None)
         ]
         for i in range(len(target)):
@@ -1649,15 +1649,15 @@
                     [1.0, 1.0],
                     [2.0, 2.0],
                     [np.nan, 3.0],
                     [np.nan, 4.0],
                     [np.nan, np.nan]
                 ]),
                 index=pd.RangeIndex(start=0, stop=5, step=1),
-                columns=pd.Int64Index([0, 1], dtype='int64', name='split_idx')
+                columns=pd.Index([0, 1], dtype='int64', name='split_idx')
             )
         )
         target = [
             pd.DatetimeIndex(['2018-01-01', '2018-01-02'],
                              dtype='datetime64[ns]', name='split_0', freq=None),
             pd.DatetimeIndex(['2018-01-01', '2018-01-02', '2018-01-03', '2018-01-04', '2018-01-05'],
                              dtype='datetime64[ns]', name='split_1', freq=None)
```

### Comparing `vectorbt-0.24.5/tests/test_indicators.py` & `vectorbt-0.25.0/tests/test_indicators.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
                 [110., 111.],
                 [110., 112.],
                 [110., 113.],
                 [110., 114.],
                 [110., 115.]
             ]),
             index=ts.index,
-            columns=pd.Int64Index([0, 1], dtype='int64', name='custom_p')
+            columns=pd.Index([0, 1], dtype='int64', name='custom_p')
         )
         pd.testing.assert_frame_equal(
             F.from_custom_func(custom_func, var_args=True).run(ts['a'], [0, 1], 10, b=100).out,
             target
         )
         pd.testing.assert_frame_equal(
             F.from_custom_func(custom_func_nb, var_args=True).run(ts['a'], [0, 1], 10, 100).out,
@@ -271,15 +271,15 @@
                 [110., 111.],
                 [110., 112.],
                 [110., 113.],
                 [110., 114.],
                 [110., 115.]
             ]),
             index=ts.index,
-            columns=pd.Int64Index([0, 1], dtype='int64', name='custom_p')
+            columns=pd.Index([0, 1], dtype='int64', name='custom_p')
         )
         pd.testing.assert_frame_equal(
             F.from_apply_func(apply_func, var_args=True).run(ts['a'], [0, 1], 10, b=100).out,
             target
         )
         pd.testing.assert_frame_equal(
             F.from_apply_func(apply_func_nb, numba_loop=True, var_args=True).run(ts['a'], [0, 1], 10, 100).out,
@@ -406,15 +406,15 @@
                 [0, 1],
                 [0, 1],
                 [0, 1],
                 [0, 1],
                 [0, 1]
             ]),
             index=pd.RangeIndex(start=0, stop=5, step=1),
-            columns=pd.Int64Index([0, 1], dtype='int64', name='custom_p')
+            columns=pd.Index([0, 1], dtype='int64', name='custom_p')
         )
         pd.testing.assert_frame_equal(
             F.from_apply_func(apply_func, require_input_shape=True).run(5, [0, 1]).out,
             target
         )
         pd.testing.assert_frame_equal(
             F.from_apply_func(apply_func_nb, numba_loop=True, require_input_shape=True).run(5, [0, 1]).out,
@@ -1939,15 +1939,15 @@
                 (3, 1, 'c'),
             ], names=['custom_out_above', 'custom_p', None])
         )
         pd.testing.assert_frame_equal(
             obj.out_above([2, 3]),
             target
         )
-        columns = target.columns.rename('my_above', 0)
+        columns = target.columns.set_names('my_above', level=0)
         pd.testing.assert_frame_equal(
             obj.out_above([2, 3], level_name='my_above'),
             pd.DataFrame(
                 target.values,
                 index=target.index,
                 columns=columns
             )
@@ -2010,15 +2010,15 @@
                 (True, 2, 'c'),
             ], names=['custom_out_and', 'custom_p', None])
         )
         pd.testing.assert_frame_equal(
             obj.out_and([False, True]),
             target
         )
-        columns = target.columns.rename('my_and', 0)
+        columns = target.columns.set_names('my_and', level=0)
         pd.testing.assert_frame_equal(
             obj.out_and([False, True], level_name='my_and'),
             pd.DataFrame(
                 target.values,
                 index=target.index,
                 columns=columns
             )
@@ -2346,15 +2346,15 @@
                 pd.DataFrame(
                     np.column_stack((
                         ts['a'].rolling(2).mean().values,
                         ts['a'].rolling(3).mean().values,
                         ts['a'].rolling(4).mean().values
                     )),
                     index=ts.index,
-                    columns=pd.Int64Index([2, 3, 4], dtype='int64', name='sma_length')
+                    columns=pd.Index([2, 3, 4], dtype='int64', name='sma_length')
                 )
             )
 
     def test_get_ta_indicators(self):
         if ta_available:
             assert len(vbt.IndicatorFactory.get_ta_indicators()) > 0
 
@@ -2374,15 +2374,15 @@
                 pd.DataFrame(
                     np.column_stack((
                         ts['a'].rolling(2).mean().values,
                         ts['a'].rolling(3).mean().values,
                         ts['a'].rolling(4).mean().values
                     )),
                     index=ts.index,
-                    columns=pd.Int64Index([2, 3, 4], dtype='int64', name='smaindicator_window')
+                    columns=pd.Index([2, 3, 4], dtype='int64', name='smaindicator_window')
                 )
             )
             target = pd.DataFrame(
                 np.array([
                     [np.nan, np.nan, np.nan],
                     [2.5, 5.5, 2.5],
                     [3.5, 4.5, 3.5],
```

### Comparing `vectorbt-0.24.5/tests/test_labels.py` & `vectorbt-0.25.0/tests/test_labels.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/tests/test_portfolio.py` & `vectorbt-0.25.0/tests/test_portfolio.py`

 * *Files 0% similar despite different names*

```diff
@@ -603,15 +603,15 @@
         pf = from_orders_both()
         pd.testing.assert_index_equal(
             pf.wrapper.index,
             pd.DatetimeIndex(['2020-01-01', '2020-01-02', '2020-01-03', '2020-01-04', '2020-01-05'])
         )
         pd.testing.assert_index_equal(
             pf.wrapper.columns,
-            pd.Int64Index([0], dtype='int64')
+            pd.Index([0], dtype='int64')
         )
         assert pf.wrapper.ndim == 1
         assert pf.wrapper.freq == day_dt
         assert pf.wrapper.grouper.group_by is None
 
     def test_multiple_columns(self):
         record_arrays_close(
@@ -1277,19 +1277,19 @@
                 (0, 0, 0, 100.0, 1.0, 0.0, 0), (1, 0, 1, 200.0, 2.0, 0.0, 1), (2, 0, 3, 100.0, 4.0, 0.0, 0),
                 (3, 1, 0, 100.0, 1.0, 0.0, 0), (4, 1, 1, 200.0, 2.0, 0.0, 1), (5, 1, 3, 100.0, 4.0, 0.0, 0),
                 (6, 2, 0, 100.0, 1.0, 0.0, 0), (7, 2, 1, 200.0, 2.0, 0.0, 1), (8, 2, 3, 100.0, 4.0, 0.0, 0)
             ], dtype=order_dt)
         )
         pd.testing.assert_index_equal(
             pf.wrapper.grouper.group_by,
-            pd.Int64Index([0, 0, 1], dtype='int64')
+            pd.Index([0, 0, 1], dtype='int64')
         )
         pd.testing.assert_series_equal(
             pf.init_cash,
-            pd.Series([200., 100.], index=pd.Int64Index([0, 1], dtype='int64')).rename('init_cash')
+            pd.Series([200., 100.], index=pd.Index([0, 1], dtype='int64')).rename('init_cash')
         )
         assert not pf.cash_sharing
 
     def test_cash_sharing(self):
         pf = from_orders_both(close=price_wide, group_by=np.array([0, 0, 1]), cash_sharing=True)
         record_arrays_close(
             pf.order_records,
@@ -1297,19 +1297,19 @@
                 (0, 0, 0, 100., 1., 0., 0), (1, 0, 1, 200., 2., 0., 1),
                 (2, 0, 3, 100., 4., 0., 0), (3, 2, 0, 100., 1., 0., 0),
                 (4, 2, 1, 200., 2., 0., 1), (5, 2, 3, 100., 4., 0., 0)
             ], dtype=order_dt)
         )
         pd.testing.assert_index_equal(
             pf.wrapper.grouper.group_by,
-            pd.Int64Index([0, 0, 1], dtype='int64')
+            pd.Index([0, 0, 1], dtype='int64')
         )
         pd.testing.assert_series_equal(
             pf.init_cash,
-            pd.Series([100., 100.], index=pd.Int64Index([0, 1], dtype='int64')).rename('init_cash')
+            pd.Series([100., 100.], index=pd.Index([0, 1], dtype='int64')).rename('init_cash')
         )
         assert pf.cash_sharing
         with pytest.raises(Exception):
             _ = pf.regroup(group_by=False)
 
     def test_call_seq(self):
         pf = from_orders_both(close=price_wide, group_by=np.array([0, 0, 1]), cash_sharing=True)
@@ -1760,15 +1760,15 @@
         pf = _from_signals_both()
         pd.testing.assert_index_equal(
             pf.wrapper.index,
             pd.DatetimeIndex(['2020-01-01', '2020-01-02', '2020-01-03', '2020-01-04', '2020-01-05'])
         )
         pd.testing.assert_index_equal(
             pf.wrapper.columns,
-            pd.Int64Index([0], dtype='int64')
+            pd.Index([0], dtype='int64')
         )
         assert pf.wrapper.ndim == 1
         assert pf.wrapper.freq == day_dt
         assert pf.wrapper.grouper.group_by is None
 
     @pytest.mark.parametrize(
         "test_ls",
@@ -2524,38 +2524,38 @@
             np.array([
                 (0, 0, 0, 100.0, 1.0, 0.0, 0), (1, 0, 3, 200.0, 4.0, 0.0, 1), (2, 1, 0, 100.0, 1.0, 0.0, 0),
                 (3, 1, 3, 200.0, 4.0, 0.0, 1), (4, 2, 0, 100.0, 1.0, 0.0, 0), (5, 2, 3, 200.0, 4.0, 0.0, 1)
             ], dtype=order_dt)
         )
         pd.testing.assert_index_equal(
             pf.wrapper.grouper.group_by,
-            pd.Int64Index([0, 0, 1], dtype='int64')
+            pd.Index([0, 0, 1], dtype='int64')
         )
         pd.testing.assert_series_equal(
             pf.init_cash,
-            pd.Series([200., 100.], index=pd.Int64Index([0, 1], dtype='int64')).rename('init_cash')
+            pd.Series([200., 100.], index=pd.Index([0, 1], dtype='int64')).rename('init_cash')
         )
         assert not pf.cash_sharing
 
     def test_cash_sharing(self):
         pf = from_signals_both(close=price_wide, group_by=np.array([0, 0, 1]), cash_sharing=True)
         record_arrays_close(
             pf.order_records,
             np.array([
                 (0, 0, 0, 100., 1., 0., 0), (1, 0, 3, 200., 4., 0., 1),
                 (2, 2, 0, 100., 1., 0., 0), (3, 2, 3, 200., 4., 0., 1)
             ], dtype=order_dt)
         )
         pd.testing.assert_index_equal(
             pf.wrapper.grouper.group_by,
-            pd.Int64Index([0, 0, 1], dtype='int64')
+            pd.Index([0, 0, 1], dtype='int64')
         )
         pd.testing.assert_series_equal(
             pf.init_cash,
-            pd.Series([100., 100.], index=pd.Int64Index([0, 1], dtype='int64')).rename('init_cash')
+            pd.Series([100., 100.], index=pd.Index([0, 1], dtype='int64')).rename('init_cash')
         )
         assert pf.cash_sharing
         with pytest.raises(Exception):
             _ = pf.regroup(group_by=False)
 
     def test_call_seq(self):
         pf = from_signals_both(close=price_wide, group_by=np.array([0, 0, 1]), cash_sharing=True)
@@ -3448,15 +3448,15 @@
             result.wrapper.index,
             pd.DatetimeIndex([
                 '2020-01-01', '2020-01-02', '2020-01-03', '2020-01-04', '2020-01-05'
             ], dtype='datetime64[ns]', freq=None)
         )
         pd.testing.assert_index_equal(
             result.wrapper.columns,
-            pd.Int64Index([1, 2], dtype='int64', name='randnx_n')
+            pd.Index([1, 2], dtype='int64', name='randnx_n')
         )
 
     def test_from_random_prob(self):
         result = vbt.Portfolio.from_random_signals(price, prob=0.5, seed=seed)
         record_arrays_close(
             result.order_records,
             vbt.Portfolio.from_signals(
@@ -3553,15 +3553,15 @@
         )
         pd.testing.assert_index_equal(
             pf.wrapper.index,
             pd.DatetimeIndex(['2020-01-01', '2020-01-02', '2020-01-03', '2020-01-04', '2020-01-05'])
         )
         pd.testing.assert_index_equal(
             pf.wrapper.columns,
-            pd.Int64Index([0], dtype='int64')
+            pd.Index([0], dtype='int64')
         )
         assert pf.wrapper.ndim == 1
         assert pf.wrapper.freq == day_dt
         assert pf.wrapper.grouper.group_by is None
 
     @pytest.mark.parametrize("test_row_wise", [False, True])
     @pytest.mark.parametrize("test_flexible", [False, True])
@@ -3638,19 +3638,19 @@
                     (10, 2, 0, 100.0, 1.0, 0.0, 0), (11, 2, 1, 200.0, 2.0, 0.0, 1),
                     (12, 2, 2, 133.33333333333334, 3.0, 0.0, 0), (13, 2, 3, 66.66666666666669, 4.0, 0.0, 1),
                     (14, 2, 4, 53.33333333333335, 5.0, 0.0, 0)
                 ], dtype=order_dt)
             )
         pd.testing.assert_index_equal(
             pf.wrapper.grouper.group_by,
-            pd.Int64Index([0, 0, 1], dtype='int64')
+            pd.Index([0, 0, 1], dtype='int64')
         )
         pd.testing.assert_series_equal(
             pf.init_cash,
-            pd.Series([200., 100.], index=pd.Int64Index([0, 1], dtype='int64')).rename('init_cash')
+            pd.Series([200., 100.], index=pd.Index([0, 1], dtype='int64')).rename('init_cash')
         )
         assert not pf.cash_sharing
 
     @pytest.mark.parametrize("test_row_wise", [False, True])
     @pytest.mark.parametrize("test_flexible", [False, True])
     def test_cash_sharing(self, test_row_wise, test_flexible):
         order_func = flex_order_func_nb if test_flexible else order_func_nb
@@ -3677,19 +3677,19 @@
                     (4, 0, 4, 53.33333333, 5., 0., 0), (5, 2, 0, 100., 1., 0., 0),
                     (6, 2, 1, 200., 2., 0., 1), (7, 2, 2, 133.33333333, 3., 0., 0),
                     (8, 2, 3, 66.66666667, 4., 0., 1), (9, 2, 4, 53.33333333, 5., 0., 0)
                 ], dtype=order_dt)
             )
         pd.testing.assert_index_equal(
             pf.wrapper.grouper.group_by,
-            pd.Int64Index([0, 0, 1], dtype='int64')
+            pd.Index([0, 0, 1], dtype='int64')
         )
         pd.testing.assert_series_equal(
             pf.init_cash,
-            pd.Series([100., 100.], index=pd.Int64Index([0, 1], dtype='int64')).rename('init_cash')
+            pd.Series([100., 100.], index=pd.Index([0, 1], dtype='int64')).rename('init_cash')
         )
         assert pf.cash_sharing
 
     @pytest.mark.parametrize(
         "test_row_wise",
         [False, True],
     )
```

### Comparing `vectorbt-0.24.5/tests/test_records.py` & `vectorbt-0.25.0/tests/test_records.py`

 * *Files 1% similar despite different names*

```diff
@@ -408,18 +408,14 @@
             pd.Series(np.array([11., 13.333333333333334, 11., np.nan]), index=wrapper.columns).rename('reduce')
         )
         pd.testing.assert_series_equal(
             mapped_array.reduce(mean_reduce_nb, fill_value=0.),
             pd.Series(np.array([11., 13.333333333333334, 11., 0.]), index=wrapper.columns).rename('reduce')
         )
         pd.testing.assert_series_equal(
-            mapped_array.reduce(mean_reduce_nb, fill_value=0., wrap_kwargs=dict(dtype=np.int_)),
-            pd.Series(np.array([11., 13.333333333333334, 11., 0.]), index=wrapper.columns).rename('reduce')
-        )
-        pd.testing.assert_series_equal(
             mapped_array.reduce(mean_reduce_nb, wrap_kwargs=dict(to_timedelta=True)),
             pd.Series(np.array([11., 13.333333333333334, 11., np.nan]), index=wrapper.columns).rename('reduce') * day_dt
         )
         pd.testing.assert_series_equal(
             mapped_array_grouped.reduce(mean_reduce_nb),
             pd.Series([12.166666666666666, 11.0], index=pd.Index(['g1', 'g2'], dtype='object')).rename('reduce')
         )
@@ -780,15 +776,15 @@
         )
 
     def test_value_counts(self):
         pd.testing.assert_series_equal(
             mapped_array['a'].value_counts(),
             pd.Series(
                 np.array([1, 1, 1]),
-                index=pd.Float64Index([10.0, 11.0, 12.0], dtype='float64'),
+                index=pd.Index([10.0, 11.0, 12.0], dtype='float64'),
                 name='a'
             )
         )
         pd.testing.assert_series_equal(
             mapped_array['a'].value_counts(mapping=mapping),
             pd.Series(
                 np.array([1, 1, 1]),
@@ -802,113 +798,113 @@
                 np.array([
                     [1, 0, 1, 0],
                     [1, 0, 1, 0],
                     [1, 0, 1, 0],
                     [0, 2, 0, 0],
                     [0, 1, 0, 0]
                 ]),
-                index=pd.Float64Index([10.0, 11.0, 12.0, 13.0, 14.0], dtype='float64'),
+                index=pd.Index([10.0, 11.0, 12.0, 13.0, 14.0], dtype='float64'),
                 columns=wrapper.columns
             )
         )
         pd.testing.assert_frame_equal(
             mapped_array_grouped.value_counts(),
             pd.DataFrame(
                 np.array([
                     [1, 1],
                     [1, 1],
                     [1, 1],
                     [2, 0],
                     [1, 0]
                 ]),
-                index=pd.Float64Index([10.0, 11.0, 12.0, 13.0, 14.0], dtype='float64'),
+                index=pd.Index([10.0, 11.0, 12.0, 13.0, 14.0], dtype='float64'),
                 columns=pd.Index(['g1', 'g2'], dtype='object')
             )
         )
         mapped_array2 = mapped_array.replace(mapped_arr=[4, 4, 3, 2, np.nan, 4, 3, 2, 1])
         pd.testing.assert_frame_equal(
             mapped_array2.value_counts(sort_uniques=False),
             pd.DataFrame(
                 np.array([
                     [2, 1, 0, 0],
                     [1, 0, 1, 0],
                     [0, 1, 1, 0],
                     [0, 0, 1, 0],
                     [0, 1, 0, 0]
                 ]),
-                index=pd.Float64Index([4.0, 3.0, 2.0, 1.0, None], dtype='float64'),
+                index=pd.Index([4.0, 3.0, 2.0, 1.0, None], dtype='float64'),
                 columns=wrapper.columns
             )
         )
         pd.testing.assert_frame_equal(
             mapped_array2.value_counts(sort_uniques=True),
             pd.DataFrame(
                 np.array([
                     [0, 0, 1, 0],
                     [0, 1, 1, 0],
                     [1, 0, 1, 0],
                     [2, 1, 0, 0],
                     [0, 1, 0, 0]
                 ]),
-                index=pd.Float64Index([1.0, 2.0, 3.0, 4.0, None], dtype='float64'),
+                index=pd.Index([1.0, 2.0, 3.0, 4.0, None], dtype='float64'),
                 columns=wrapper.columns
             )
         )
         pd.testing.assert_frame_equal(
             mapped_array2.value_counts(sort=True),
             pd.DataFrame(
                 np.array([
                     [2, 1, 0, 0],
                     [0, 1, 1, 0],
                     [1, 0, 1, 0],
                     [0, 0, 1, 0],
                     [0, 1, 0, 0]
                 ]),
-                index=pd.Float64Index([4.0, 2.0, 3.0, 1.0, np.nan], dtype='float64'),
+                index=pd.Index([4.0, 2.0, 3.0, 1.0, np.nan], dtype='float64'),
                 columns=wrapper.columns
             )
         )
         pd.testing.assert_frame_equal(
             mapped_array2.value_counts(sort=True, ascending=True),
             pd.DataFrame(
                 np.array([
                     [0, 0, 1, 0],
                     [0, 1, 0, 0],
                     [0, 1, 1, 0],
                     [1, 0, 1, 0],
                     [2, 1, 0, 0]
                 ]),
-                index=pd.Float64Index([1.0, np.nan, 2.0, 3.0, 4.0], dtype='float64'),
+                index=pd.Index([1.0, np.nan, 2.0, 3.0, 4.0], dtype='float64'),
                 columns=wrapper.columns
             )
         )
         pd.testing.assert_frame_equal(
             mapped_array2.value_counts(sort=True, normalize=True),
             pd.DataFrame(
                 np.array([
                     [0.2222222222222222, 0.1111111111111111, 0.0, 0.0],
                     [0.0, 0.1111111111111111, 0.1111111111111111, 0.0],
                     [0.1111111111111111, 0.0, 0.1111111111111111, 0.0],
                     [0.0, 0.0, 0.1111111111111111, 0.0],
                     [0.0, 0.1111111111111111, 0.0, 0.0]
                 ]),
-                index=pd.Float64Index([4.0, 2.0, 3.0, 1.0, np.nan], dtype='float64'),
+                index=pd.Index([4.0, 2.0, 3.0, 1.0, np.nan], dtype='float64'),
                 columns=wrapper.columns
             )
         )
         pd.testing.assert_frame_equal(
             mapped_array2.value_counts(sort=True, normalize=True, dropna=True),
             pd.DataFrame(
                 np.array([
                     [0.25, 0.125, 0.0, 0.0],
                     [0.0, 0.125, 0.125, 0.0],
                     [0.125, 0.0, 0.125, 0.0],
                     [0.0, 0.0, 0.125, 0.0]
                 ]),
-                index=pd.Float64Index([4.0, 2.0, 3.0, 1.0], dtype='float64'),
+                index=pd.Index([4.0, 2.0, 3.0, 1.0], dtype='float64'),
                 columns=wrapper.columns
             )
         )
 
     @pytest.mark.parametrize(
         "test_nosort",
         [False, True],
```

### Comparing `vectorbt-0.24.5/tests/test_returns.py` & `vectorbt-0.25.0/tests/test_returns.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/tests/test_signals.py` & `vectorbt-0.25.0/tests/test_signals.py`

 * *Files 0% similar despite different names*

```diff
@@ -2141,26 +2141,26 @@
             my_sig.entries,
             pd.DataFrame(np.array([
                 [True, True],
                 [False, False],
                 [False, False],
                 [False, False],
                 [False, False]
-            ]), columns=pd.Int64Index([1, 0], dtype='int64', name='custom_n2')
+            ]), columns=pd.Index([1, 0], dtype='int64', name='custom_n2')
             )
         )
         pd.testing.assert_frame_equal(
             my_sig.in_out2,
             pd.DataFrame(np.array([
                 [1100.0, 1100.0],
                 [np.nan, np.nan],
                 [np.nan, np.nan],
                 [np.nan, np.nan],
                 [np.nan, np.nan],
-            ]), columns=pd.Int64Index([1, 0], dtype='int64', name='custom_n2')
+            ]), columns=pd.Index([1, 0], dtype='int64', name='custom_n2')
             )
         )
 
     def test_exits(self):
         @njit
         def choice_nb(from_i, to_i, col, ts, in_out, n, arg, temp_idx_arr, kw):
             in_out[from_i, col] = ts[from_i, col] * n + arg + kw
@@ -2195,75 +2195,75 @@
             my_sig.entries,
             pd.DataFrame(np.array([
                 [True, True],
                 [False, False],
                 [True, True],
                 [False, False],
                 [True, True]
-            ]), columns=pd.Int64Index([1, 0], dtype='int64', name='custom_n2')
+            ]), columns=pd.Index([1, 0], dtype='int64', name='custom_n2')
             )
         )
         pd.testing.assert_frame_equal(
             my_sig.exits,
             pd.DataFrame(np.array([
                 [False, False],
                 [True, True],
                 [False, False],
                 [True, True],
                 [False, False]
-            ]), columns=pd.Int64Index([1, 0], dtype='int64', name='custom_n2')
+            ]), columns=pd.Index([1, 0], dtype='int64', name='custom_n2')
             )
         )
         pd.testing.assert_frame_equal(
             my_sig.in_out2,
             pd.DataFrame(np.array([
                 [np.nan, np.nan],
                 [1101.0, 1100.0],
                 [np.nan, np.nan],
                 [1103.0, 1100.0],
                 [np.nan, np.nan],
-            ]), columns=pd.Int64Index([1, 0], dtype='int64', name='custom_n2')
+            ]), columns=pd.Index([1, 0], dtype='int64', name='custom_n2')
             )
         )
         e = np.array([True, False, False, True, False, False])
         my_sig = MySignals.run(e, np.arange(6), [1, 0], 100, wait=2)
         pd.testing.assert_frame_equal(
             my_sig.entries,
             pd.DataFrame(np.array([
                 [True, True],
                 [False, False],
                 [False, False],
                 [True, True],
                 [False, False],
                 [False, False]
-            ]), columns=pd.Int64Index([1, 0], dtype='int64', name='custom_n2')
+            ]), columns=pd.Index([1, 0], dtype='int64', name='custom_n2')
             )
         )
         pd.testing.assert_frame_equal(
             my_sig.exits,
             pd.DataFrame(np.array([
                 [False, False],
                 [False, False],
                 [True, True],
                 [False, False],
                 [False, False],
                 [True, True]
-            ]), columns=pd.Int64Index([1, 0], dtype='int64', name='custom_n2')
+            ]), columns=pd.Index([1, 0], dtype='int64', name='custom_n2')
             )
         )
         pd.testing.assert_frame_equal(
             my_sig.in_out2,
             pd.DataFrame(np.array([
                 [np.nan, np.nan],
                 [np.nan, np.nan],
                 [1102.0, 1100.0],
                 [np.nan, np.nan],
                 [np.nan, np.nan],
                 [1105.0, 1100.0]
-            ]), columns=pd.Int64Index([1, 0], dtype='int64', name='custom_n2')
+            ]), columns=pd.Index([1, 0], dtype='int64', name='custom_n2')
             )
         )
 
     def test_chain(self):
         @njit
         def choice_nb(from_i, to_i, col, ts, in_out, n, arg, temp_idx_arr, kw):
             in_out[from_i, col] = ts[from_i, col] * n + arg + kw
@@ -2298,98 +2298,98 @@
             my_sig.entries,
             pd.DataFrame(np.array([
                 [True, True],
                 [True, True],
                 [True, True],
                 [True, True],
                 [True, True]
-            ]), columns=pd.Int64Index([1, 0], dtype='int64', name='custom_n2')
+            ]), columns=pd.Index([1, 0], dtype='int64', name='custom_n2')
             )
         )
         pd.testing.assert_frame_equal(
             my_sig.new_entries,
             pd.DataFrame(np.array([
                 [True, True],
                 [False, False],
                 [True, True],
                 [False, False],
                 [True, True]
-            ]), columns=pd.Int64Index([1, 0], dtype='int64', name='custom_n2')
+            ]), columns=pd.Index([1, 0], dtype='int64', name='custom_n2')
             )
         )
         pd.testing.assert_frame_equal(
             my_sig.exits,
             pd.DataFrame(np.array([
                 [False, False],
                 [True, True],
                 [False, False],
                 [True, True],
                 [False, False]
-            ]), columns=pd.Int64Index([1, 0], dtype='int64', name='custom_n2')
+            ]), columns=pd.Index([1, 0], dtype='int64', name='custom_n2')
             )
         )
         pd.testing.assert_frame_equal(
             my_sig.in_out2,
             pd.DataFrame(np.array([
                 [np.nan, np.nan],
                 [1101.0, 1100.0],
                 [np.nan, np.nan],
                 [1103.0, 1100.0],
                 [np.nan, np.nan],
-            ]), columns=pd.Int64Index([1, 0], dtype='int64', name='custom_n2')
+            ]), columns=pd.Index([1, 0], dtype='int64', name='custom_n2')
             )
         )
         e = np.array([True, True, True, True, True, True])
         my_sig = MySignals.run(e, np.arange(6), [1, 0], 100, wait=2)
         pd.testing.assert_frame_equal(
             my_sig.entries,
             pd.DataFrame(np.array([
                 [True, True],
                 [True, True],
                 [True, True],
                 [True, True],
                 [True, True],
                 [True, True]
-            ]), columns=pd.Int64Index([1, 0], dtype='int64', name='custom_n2')
+            ]), columns=pd.Index([1, 0], dtype='int64', name='custom_n2')
             )
         )
         pd.testing.assert_frame_equal(
             my_sig.new_entries,
             pd.DataFrame(np.array([
                 [True, True],
                 [False, False],
                 [False, False],
                 [True, True],
                 [False, False],
                 [False, False]
-            ]), columns=pd.Int64Index([1, 0], dtype='int64', name='custom_n2')
+            ]), columns=pd.Index([1, 0], dtype='int64', name='custom_n2')
             )
         )
         pd.testing.assert_frame_equal(
             my_sig.exits,
             pd.DataFrame(np.array([
                 [False, False],
                 [False, False],
                 [True, True],
                 [False, False],
                 [False, False],
                 [True, True]
-            ]), columns=pd.Int64Index([1, 0], dtype='int64', name='custom_n2')
+            ]), columns=pd.Index([1, 0], dtype='int64', name='custom_n2')
             )
         )
         pd.testing.assert_frame_equal(
             my_sig.in_out2,
             pd.DataFrame(np.array([
                 [np.nan, np.nan],
                 [np.nan, np.nan],
                 [1102.0, 1100.0],
                 [np.nan, np.nan],
                 [np.nan, np.nan],
                 [1105.0, 1100.0]
-            ]), columns=pd.Int64Index([1, 0], dtype='int64', name='custom_n2')
+            ]), columns=pd.Index([1, 0], dtype='int64', name='custom_n2')
             )
         )
 
     def test_both(self):
         @njit
         def cache_nb(ts1, ts2, in_out1, in_out2, n1, n2, arg0, temp_idx_arr0, kw0):
             return arg0
@@ -2579,15 +2579,15 @@
             pd.DataFrame(np.array([
                 [True, True, True],
                 [False, False, True],
                 [False, False, False],
                 [False, True, False],
                 [False, False, True],
                 [False, False, False]
-            ]), columns=pd.Int64Index([1, 2, 3], dtype='int64', name='rand_n')
+            ]), columns=pd.Index([1, 2, 3], dtype='int64', name='rand_n')
             )
         )
         rand = vbt.RAND.run(n=[np.array([1, 2]), np.array([3, 4])], input_shape=(8, 2), seed=seed)
         pd.testing.assert_frame_equal(
             rand.entries,
             pd.DataFrame(np.array([
                 [False, False, True, False],
@@ -2636,27 +2636,27 @@
             pd.DataFrame(np.array([
                 [True, True, True],
                 [False, False, False],
                 [False, True, True],
                 [False, False, False],
                 [False, False, True],
                 [False, False, False]
-            ]), columns=pd.Int64Index([1, 2, 3], dtype='int64', name='randnx_n')
+            ]), columns=pd.Index([1, 2, 3], dtype='int64', name='randnx_n')
             )
         )
         pd.testing.assert_frame_equal(
             randnx.exits,
             pd.DataFrame(np.array([
                 [False, False, False],
                 [True, True, True],
                 [False, False, False],
                 [False, True, True],
                 [False, False, False],
                 [False, False, True]
-            ]), columns=pd.Int64Index([1, 2, 3], dtype='int64', name='randnx_n')
+            ]), columns=pd.Index([1, 2, 3], dtype='int64', name='randnx_n')
             )
         )
         randnx = vbt.RANDNX.run(n=[np.array([1, 2]), np.array([3, 4])], input_shape=(8, 2), seed=seed)
         pd.testing.assert_frame_equal(
             randnx.entries,
             pd.DataFrame(np.array([
                 [False, True, True, True],
@@ -2706,15 +2706,15 @@
             rprob.entries,
             pd.DataFrame(np.array([
                 [False, True, True],
                 [False, True, True],
                 [False, False, True],
                 [False, False, True],
                 [False, False, True]
-            ]), columns=pd.Float64Index([0, 0.5, 1], dtype='float64', name='rprob_prob')
+            ]), columns=pd.Index([0, 0.5, 1], dtype='float64', name='rprob_prob')
             )
         )
         rprob = vbt.RPROB.run(prob=[np.array([0, 0.25]), np.array([0.75, 1])], input_shape=(5, 2), seed=seed)
         pd.testing.assert_frame_equal(
             rprob.entries,
             pd.DataFrame(np.array([
                 [False, True, True, True],
```

### Comparing `vectorbt-0.24.5/tests/test_utils.py` & `vectorbt-0.25.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/tests/utils.py` & `vectorbt-0.25.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/__init__.py` & `vectorbt-0.25.0/vectorbt/__init__.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/_settings.py` & `vectorbt-0.25.0/vectorbt/_settings.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/_typing.py` & `vectorbt-0.25.0/vectorbt/_typing.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/base/accessors.py` & `vectorbt-0.25.0/vectorbt/base/accessors.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/base/array_wrapper.py` & `vectorbt-0.25.0/vectorbt/base/array_wrapper.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/base/column_grouper.py` & `vectorbt-0.25.0/vectorbt/base/column_grouper.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/base/combine_fns.py` & `vectorbt-0.25.0/vectorbt/base/combine_fns.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/base/index_fns.py` & `vectorbt-0.25.0/vectorbt/base/index_fns.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/base/indexing.py` & `vectorbt-0.25.0/vectorbt/base/indexing.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/base/reshape_fns.py` & `vectorbt-0.25.0/vectorbt/base/reshape_fns.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/data/__init__.py` & `vectorbt-0.25.0/vectorbt/data/__init__.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/data/base.py` & `vectorbt-0.25.0/vectorbt/data/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -438,15 +438,15 @@
                     else:
                         raise ValueError(f"missing='{missing}' is not recognized")
 
         # reindex
         new_data = {}
         for k, v in data.items():
             if isinstance(v, pd.Series):
-                v = v.to_frame(name=v.name)
+                v = v.to_frame()
             v = v.reindex(columns=columns)
             if not multiple_columns:
                 v = v[columns[0]]
                 if name_is_none:
                     v = v.rename(None)
             new_data[k] = v
         return new_data
```

### Comparing `vectorbt-0.24.5/vectorbt/data/custom.py` & `vectorbt-0.25.0/vectorbt/data/custom.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/data/updater.py` & `vectorbt-0.25.0/vectorbt/data/updater.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/generic/__init__.py` & `vectorbt-0.25.0/vectorbt/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/generic/accessors.py` & `vectorbt-0.25.0/vectorbt/generic/accessors.py`

 * *Files 0% similar despite different names*

```diff
@@ -976,15 +976,15 @@
             mapping = self.mapping
         if isinstance(mapping, str):
             if mapping.lower() == 'index':
                 mapping = self.wrapper.index
             elif mapping.lower() == 'columns':
                 mapping = self.wrapper.columns
             mapping = to_mapping(mapping)
-        codes, uniques = pd.factorize(self.obj.values.flatten(), sort=False, na_sentinel=None)
+        codes, uniques = pd.factorize(self.obj.values.flatten(), sort=False, use_na_sentinel=False)
         codes = codes.reshape(self.wrapper.shape_2d)
         group_lens = self.wrapper.grouper.get_group_lens(group_by=group_by)
         value_counts = nb.value_counts_nb(codes, len(uniques), group_lens)
         if incl_all_keys and mapping is not None:
             missing_keys = []
             for x in mapping:
                 if pd.isnull(x) and pd.isnull(uniques).any():
```

### Comparing `vectorbt-0.24.5/vectorbt/generic/decorators.py` & `vectorbt-0.25.0/vectorbt/generic/decorators.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/generic/drawdowns.py` & `vectorbt-0.25.0/vectorbt/generic/drawdowns.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/generic/enums.py` & `vectorbt-0.25.0/vectorbt/generic/enums.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/generic/nb.py` & `vectorbt-0.25.0/vectorbt/generic/nb.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/generic/plots_builder.py` & `vectorbt-0.25.0/vectorbt/generic/plots_builder.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/generic/plotting.py` & `vectorbt-0.25.0/vectorbt/generic/plotting.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/generic/ranges.py` & `vectorbt-0.25.0/vectorbt/generic/ranges.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/generic/splitters.py` & `vectorbt-0.25.0/vectorbt/generic/splitters.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/generic/stats_builder.py` & `vectorbt-0.25.0/vectorbt/generic/stats_builder.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/indicators/__init__.py` & `vectorbt-0.25.0/vectorbt/indicators/__init__.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/indicators/basic.py` & `vectorbt-0.25.0/vectorbt/indicators/basic.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/indicators/configs.py` & `vectorbt-0.25.0/vectorbt/indicators/configs.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/indicators/factory.py` & `vectorbt-0.25.0/vectorbt/indicators/factory.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/indicators/nb.py` & `vectorbt-0.25.0/vectorbt/indicators/nb.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/labels/__init__.py` & `vectorbt-0.25.0/vectorbt/labels/__init__.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/labels/enums.py` & `vectorbt-0.25.0/vectorbt/labels/enums.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/labels/generators.py` & `vectorbt-0.25.0/vectorbt/labels/generators.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/labels/nb.py` & `vectorbt-0.25.0/vectorbt/labels/nb.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/messaging/telegram.py` & `vectorbt-0.25.0/vectorbt/messaging/telegram.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/ohlcv_accessors.py` & `vectorbt-0.25.0/vectorbt/ohlcv_accessors.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/portfolio/__init__.py` & `vectorbt-0.25.0/vectorbt/portfolio/__init__.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/portfolio/base.py` & `vectorbt-0.25.0/vectorbt/portfolio/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -625,15 +625,15 @@
 ...     "BTC-USD",
 ...     start='2020-01-01 UTC',
 ...     end='2020-09-01 UTC'
 ... ).get('Close')
 
 >>> pf = vbt.Portfolio.from_random_signals(close, n=[10, 20], seed=42)
 >>> pf.wrapper.columns
-Int64Index([10, 20], dtype='int64', name='rand_n')
+Index([10, 20], dtype='int64', name='rand_n')
 ```
 
 ### Column, group, and tag selection
 
 To return the statistics for a particular column/group, use the `column` argument:
 
 ```pycon
```

### Comparing `vectorbt-0.24.5/vectorbt/portfolio/decorators.py` & `vectorbt-0.25.0/vectorbt/portfolio/decorators.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/portfolio/enums.py` & `vectorbt-0.25.0/vectorbt/portfolio/enums.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/portfolio/logs.py` & `vectorbt-0.25.0/vectorbt/portfolio/logs.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/portfolio/nb.py` & `vectorbt-0.25.0/vectorbt/portfolio/nb.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/portfolio/orders.py` & `vectorbt-0.25.0/vectorbt/portfolio/orders.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/portfolio/trades.py` & `vectorbt-0.25.0/vectorbt/portfolio/trades.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/px_accessors.py` & `vectorbt-0.25.0/vectorbt/px_accessors.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/records/__init__.py` & `vectorbt-0.25.0/vectorbt/records/__init__.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/records/base.py` & `vectorbt-0.25.0/vectorbt/records/base.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/records/col_mapper.py` & `vectorbt-0.25.0/vectorbt/records/col_mapper.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/records/decorators.py` & `vectorbt-0.25.0/vectorbt/records/decorators.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/records/mapped_array.py` & `vectorbt-0.25.0/vectorbt/records/mapped_array.py`

 * *Files 0% similar despite different names*

```diff
@@ -992,15 +992,15 @@
             mapping = self.mapping
         if isinstance(mapping, str):
             if mapping.lower() == 'index':
                 mapping = self.wrapper.index
             elif mapping.lower() == 'columns':
                 mapping = self.wrapper.columns
             mapping = to_mapping(mapping)
-        mapped_codes, mapped_uniques = pd.factorize(self.values, sort=False, na_sentinel=None)
+        mapped_codes, mapped_uniques = pd.factorize(self.values, sort=False, use_na_sentinel=False)
         col_map = self.col_mapper.get_col_map(group_by=group_by)
         value_counts = nb.mapped_value_counts_nb(mapped_codes, len(mapped_uniques), col_map)
         if incl_all_keys and mapping is not None:
             missing_keys = []
             for x in mapping:
                 if pd.isnull(x) and pd.isnull(mapped_uniques).any():
                     continue
```

### Comparing `vectorbt-0.24.5/vectorbt/records/nb.py` & `vectorbt-0.25.0/vectorbt/records/nb.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/returns/accessors.py` & `vectorbt-0.25.0/vectorbt/returns/accessors.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/returns/metrics.py` & `vectorbt-0.25.0/vectorbt/returns/metrics.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/returns/nb.py` & `vectorbt-0.25.0/vectorbt/returns/nb.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/returns/qs_adapter.py` & `vectorbt-0.25.0/vectorbt/returns/qs_adapter.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/root_accessors.py` & `vectorbt-0.25.0/vectorbt/root_accessors.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/signals/__init__.py` & `vectorbt-0.25.0/vectorbt/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/signals/accessors.py` & `vectorbt-0.25.0/vectorbt/signals/accessors.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/signals/enums.py` & `vectorbt-0.25.0/vectorbt/signals/enums.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/signals/factory.py` & `vectorbt-0.25.0/vectorbt/signals/factory.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/signals/generators.py` & `vectorbt-0.25.0/vectorbt/signals/generators.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/signals/nb.py` & `vectorbt-0.25.0/vectorbt/signals/nb.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/templates/dark.json` & `vectorbt-0.25.0/vectorbt/templates/dark.json`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/templates/light.json` & `vectorbt-0.25.0/vectorbt/templates/light.json`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/templates/seaborn.json` & `vectorbt-0.25.0/vectorbt/templates/seaborn.json`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/utils/__init__.py` & `vectorbt-0.25.0/vectorbt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/utils/array_.py` & `vectorbt-0.25.0/vectorbt/utils/array_.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/utils/attr_.py` & `vectorbt-0.25.0/vectorbt/utils/attr_.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/utils/checks.py` & `vectorbt-0.25.0/vectorbt/utils/checks.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/utils/colors.py` & `vectorbt-0.25.0/vectorbt/utils/colors.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/utils/config.py` & `vectorbt-0.25.0/vectorbt/utils/config.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/utils/datetime_.py` & `vectorbt-0.25.0/vectorbt/utils/datetime_.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/utils/decorators.py` & `vectorbt-0.25.0/vectorbt/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/utils/docs.py` & `vectorbt-0.25.0/vectorbt/utils/docs.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/utils/enum_.py` & `vectorbt-0.25.0/vectorbt/utils/enum_.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/utils/figure.py` & `vectorbt-0.25.0/vectorbt/utils/figure.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/utils/image_.py` & `vectorbt-0.25.0/vectorbt/utils/image_.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/utils/mapping.py` & `vectorbt-0.25.0/vectorbt/utils/mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         if ignore_type is None or not _compatible_types(obj.dtype, obj[0]):
             return obj.map(_converter)
         return obj
     if isinstance(obj, pd.DataFrame):
         if obj.size == 0:
             return obj
         series = []
-        for sr_name, sr in obj.iteritems():
+        for sr_name, sr in obj.items():
             if ignore_type is None or not _compatible_types(sr.dtype, sr.iloc[0]):
                 series.append(sr.map(_converter))
             else:
                 series.append(sr)
         return pd.concat(series, axis=1, keys=obj.columns)
     if ignore_type is None or not _compatible_types(type(obj)):
         return _converter(obj)
```

### Comparing `vectorbt-0.24.5/vectorbt/utils/math_.py` & `vectorbt-0.25.0/vectorbt/utils/math_.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/utils/module_.py` & `vectorbt-0.25.0/vectorbt/utils/module_.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/utils/params.py` & `vectorbt-0.25.0/vectorbt/utils/params.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/utils/requests_.py` & `vectorbt-0.25.0/vectorbt/utils/requests_.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/utils/schedule_.py` & `vectorbt-0.25.0/vectorbt/utils/schedule_.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/utils/tags.py` & `vectorbt-0.25.0/vectorbt/utils/tags.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt/utils/template.py` & `vectorbt-0.25.0/vectorbt/utils/template.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.24.5/vectorbt.egg-info/PKG-INFO` & `vectorbt-0.25.0/vectorbt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectorbt
-Version: 0.24.5
+Version: 0.25.0
 Summary: Python library for backtesting and analyzing trading strategies at scale
 Home-page: https://github.com/polakowo/vectorbt
 Author: Oleg Polakow
 Author-email: olegpolakow@gmail.com
 License: Apache 2.0 with Commons Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `vectorbt-0.24.5/vectorbt.egg-info/SOURCES.txt` & `vectorbt-0.25.0/vectorbt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

