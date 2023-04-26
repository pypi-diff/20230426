# Comparing `tmp/nonebot_plugin_pixivbot-1.8.1.tar.gz` & `tmp/nonebot_plugin_pixivbot-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_pixivbot-1.8.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_pixivbot-1.8.2.tar", max compression
```

## Comparing `nonebot_plugin_pixivbot-1.8.1.tar` & `nonebot_plugin_pixivbot-1.8.2.tar`

### file list

```diff
@@ -1,166 +1,171 @@
--rw-r--r--   0        0        0     1085 2023-02-13 05:42:01.812872 nonebot_plugin_pixivbot-1.8.1/LICENSE
--rw-r--r--   0        0        0     1787 2023-03-29 02:49:22.423918 nonebot_plugin_pixivbot-1.8.1/pyproject.toml
--rw-r--r--   0        0        0    17352 2023-03-16 06:41:02.958294 nonebot_plugin_pixivbot-1.8.1/README.md
--rw-r--r--   0        0        0     1458 2023-03-29 02:34:22.106471 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/__init__.py
--rw-r--r--   0        0        0     7333 2023-03-29 02:34:22.107473 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/config.py
--rw-r--r--   0        0        0     4644 2023-02-14 03:37:13.328790 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/context.py
--rw-r--r--   0        0        0      443 2023-02-13 05:42:01.817870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/__init__.py
--rw-r--r--   0        0        0       56 2023-02-13 05:42:01.817870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/errors.py
--rw-r--r--   0        0        0     1515 2023-02-13 05:42:01.817870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/interval_task_repo.py
--rw-r--r--   0        0        0      993 2023-02-13 05:42:01.818870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/local_tag/__init__.py
--rw-r--r--   0        0        0     2694 2023-02-14 03:37:13.329788 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/local_tag/mongo.py
--rw-r--r--   0        0        0     2746 2023-03-29 02:34:22.108312 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/local_tag/sql.py
--rw-r--r--   0        0        0      894 2023-02-13 05:42:01.820870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/pixiv_binding/__init__.py
--rw-r--r--   0        0        0     2104 2023-02-14 03:37:13.330787 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/pixiv_binding/mongo.py
--rw-r--r--   0        0        0     2751 2023-03-29 02:34:22.108836 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/pixiv_binding/sql.py
--rw-r--r--   0        0        0      262 2023-02-13 05:42:01.821870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/pixiv_repo/__init__.py
--rw-r--r--   0        0        0     1524 2023-02-13 05:42:01.822870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/pixiv_repo/base.py
--rw-r--r--   0        0        0     1910 2023-02-14 03:37:13.338166 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/pixiv_repo/compressor.py
--rw-r--r--   0        0        0      355 2023-02-13 05:42:01.822870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/pixiv_repo/enums.py
--rw-r--r--   0        0        0      334 2023-02-13 05:42:01.823870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/pixiv_repo/errors.py
--rw-r--r--   0        0        0     1036 2023-02-13 05:42:01.823870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/pixiv_repo/lazy_illust.py
--rw-r--r--   0        0        0      826 2023-03-15 03:52:01.493698 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/__init__.py
--rw-r--r--   0        0        0     2823 2023-03-15 03:26:56.195873 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/base.py
--rw-r--r--   0        0        0     3436 2023-03-15 03:24:20.770207 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/dummy.py
--rw-r--r--   0        0        0    31932 2023-03-15 03:26:56.196873 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/mongo.py
--rw-r--r--   0        0        0     4802 2023-03-29 02:34:22.109808 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/mongo_models.py
--rw-r--r--   0        0        0    33665 2023-03-15 03:27:02.949775 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql.py
--rw-r--r--   0        0        0     3536 2023-03-29 02:34:22.110334 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql_models.py
--rw-r--r--   0        0        0     8686 2023-03-15 03:26:56.197872 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator.py
--rw-r--r--   0        0        0    20378 2023-03-15 03:26:56.197872 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator_repo.py
--rw-r--r--   0        0        0      476 2023-02-13 05:42:01.828871 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/pixiv_repo/models.py
--rw-r--r--   0        0        0    19635 2023-02-14 03:37:13.342166 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/pixiv_repo/remote_repo.py
--rw-r--r--   0        0        0     1079 2023-02-13 05:42:01.829870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/source/__init__.py
--rw-r--r--   0        0        0     1820 2023-02-13 05:42:01.830870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/source/lifecycle_mixin.py
--rw-r--r--   0        0        0     3211 2023-02-13 05:42:01.830870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/source/migration_manager.py
--rw-r--r--   0        0        0     5793 2023-02-14 03:37:13.343166 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/source/mongo/__init__.py
--rw-r--r--   0        0        0      447 2023-02-13 05:42:01.832870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/source/mongo/meta_info.py
--rw-r--r--   0        0        0      693 2023-02-13 05:42:01.833870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/source/mongo/migration/__init__.py
--rw-r--r--   0        0        0     1424 2023-02-13 05:42:01.833870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v1_to_v2.py
--rw-r--r--   0        0        0      674 2023-02-13 05:42:01.833870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v2_to_v3.py
--rw-r--r--   0        0        0     2729 2023-02-13 05:42:01.834869 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v3_to_v4.py
--rw-r--r--   0        0        0     1039 2023-02-13 05:42:01.834869 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v4_to_v5.py
--rw-r--r--   0        0        0     3306 2023-02-13 05:42:01.834869 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v5_to_v6.py
--rw-r--r--   0        0        0      416 2023-02-13 05:42:01.835870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v6_to_v7.py
--rw-r--r--   0        0        0     5816 2023-03-16 06:41:02.962293 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/source/sql/__init__.py
--rw-r--r--   0        0        0      306 2023-03-13 13:51:04.755048 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/source/sql/meta_info.py
--rw-r--r--   0        0        0      457 2023-02-13 05:42:01.837870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/source/sql/migration/__init__.py
--rw-r--r--   0        0        0     3824 2023-02-13 05:42:01.838869 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v1_to_v2.py
--rw-r--r--   0        0        0     1842 2023-02-13 05:42:01.839869 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v2_to_v3.py
--rw-r--r--   0        0        0      360 2023-02-13 05:42:01.839869 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v3_to_v4.py
--rw-r--r--   0        0        0      663 2023-02-13 05:42:01.840870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/subscription/__init__.py
--rw-r--r--   0        0        0     4479 2023-02-14 03:37:13.344165 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/subscription/mongo.py
--rw-r--r--   0        0        0     5749 2023-03-29 02:34:22.110873 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/subscription/sql.py
--rw-r--r--   0        0        0        0 2023-02-13 05:42:01.842870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/utils/__init__.py
--rw-r--r--   0        0        0      164 2023-02-13 05:42:01.842870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/utils/shortuuid.py
--rw-r--r--   0        0        0      814 2023-02-13 05:42:01.843869 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/utils/sql/__init__.py
--rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843869 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/utils/sql/utc_datetime.py
--rw-r--r--   0        0        0      720 2023-02-13 05:42:01.842870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/utils/sql.pyi
--rw-r--r--   0        0        0      712 2023-02-13 05:42:01.844870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/watch_task/__init__.py
--rw-r--r--   0        0        0     5206 2023-02-14 03:37:13.345167 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/watch_task/mongo.py
--rw-r--r--   0        0        0     6675 2023-03-29 02:34:22.111922 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/watch_task/sql.py
--rw-r--r--   0        0        0      964 2023-03-15 03:24:39.857013 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/enums.py
--rw-r--r--   0        0        0      102 2023-02-14 03:27:31.463009 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/global_context.py
--rw-r--r--   0        0        0       92 2023-02-13 05:42:01.847870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/__init__.py
--rw-r--r--   0        0        0     9057 2023-03-29 02:34:22.112452 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/base.py
--rw-r--r--   0        0        0      308 2023-02-13 05:42:01.847870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/command/__init__.py
--rw-r--r--   0        0        0     2543 2023-03-29 02:34:22.112985 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/command/bind.py
--rw-r--r--   0        0        0     2481 2023-03-29 02:34:22.114209 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/command/command.py
--rw-r--r--   0        0        0     1234 2023-03-29 02:34:22.114745 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/command/help.py
--rw-r--r--   0        0        0      860 2023-03-29 02:34:22.115281 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/command/invalidate_cache.py
--rw-r--r--   0        0        0     4301 2023-03-29 02:34:22.115805 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/command/schedule.py
--rw-r--r--   0        0        0     1363 2023-03-29 02:34:22.116335 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/command/subcommand.py
--rw-r--r--   0        0        0     6055 2023-03-29 02:34:22.117392 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/command/watch.py
--rw-r--r--   0        0        0      633 2023-02-13 05:42:01.851870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/common/__init__.py
--rw-r--r--   0        0        0      688 2023-03-29 02:34:22.117934 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/common/base.py
--rw-r--r--   0        0        0     1910 2023-03-29 02:34:22.118470 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/common/illust.py
--rw-r--r--   0        0        0     1717 2023-03-29 02:34:22.119541 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/common/more.py
--rw-r--r--   0        0        0     3114 2023-03-29 02:34:22.120079 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/common/random_bookmark.py
--rw-r--r--   0        0        0     2045 2023-03-29 02:34:22.120602 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/common/random_illust.py
--rw-r--r--   0        0        0     1914 2023-03-29 02:34:22.121131 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/common/random_recommended_illust.py
--rw-r--r--   0        0        0     2313 2023-03-29 02:34:22.122125 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/common/random_related_illust.py
--rw-r--r--   0        0        0     2390 2023-03-29 02:34:22.123124 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/common/random_user_illust.py
--rw-r--r--   0        0        0     4487 2023-03-29 02:34:22.124122 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/common/ranking.py
--rw-r--r--   0        0        0        0 2023-02-13 05:42:01.857869 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/interceptor/__init__.py
--rw-r--r--   0        0        0      524 2023-03-29 02:34:22.124122 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/interceptor/base.py
--rw-r--r--   0        0        0     2012 2023-03-29 02:34:22.125123 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/interceptor/combined_interceptor.py
--rw-r--r--   0        0        0     1380 2023-03-29 02:34:22.125123 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/interceptor/default_error_interceptor.py
--rw-r--r--   0        0        0     1134 2023-03-29 02:34:22.126120 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/interceptor/loading_prompt_interceptor.py
--rw-r--r--   0        0        0     1947 2023-03-29 02:34:54.094101 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/interceptor/permission_interceptor.py
--rw-r--r--   0        0        0      654 2023-03-29 02:34:22.127120 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/interceptor/record_req_interceptor.py
--rw-r--r--   0        0        0      919 2023-03-29 02:34:22.128120 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/interceptor/retry_interceptor.py
--rw-r--r--   0        0        0     1526 2023-03-29 02:34:22.128120 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/interceptor/service_interceptor.py
--rw-r--r--   0        0        0      673 2023-03-29 02:34:22.129121 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/interceptor/timeout_interceptor.py
--rw-r--r--   0        0        0      201 2023-02-13 05:42:01.861870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/pkg_context.py
--rw-r--r--   0        0        0     3350 2023-03-29 02:34:22.130121 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/recorder.py
--rw-r--r--   0        0        0      325 2023-02-14 11:56:02.041347 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/schedule/__init__.py
--rw-r--r--   0        0        0      421 2023-03-29 02:34:22.130121 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/schedule/base.py
--rw-r--r--   0        0        0      461 2023-03-29 02:34:22.131121 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/schedule/random_bookmark.py
--rw-r--r--   0        0        0      453 2023-03-29 02:34:22.131121 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/schedule/random_illust.py
--rw-r--r--   0        0        0      498 2023-03-29 02:34:22.132122 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/schedule/random_recommended_illust.py
--rw-r--r--   0        0        0      470 2023-03-29 02:34:22.132122 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/schedule/random_user_illust.py
--rw-r--r--   0        0        0      432 2023-03-29 02:34:22.133120 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/schedule/ranking.py
--rw-r--r--   0        0        0       27 2023-02-13 05:42:01.862870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/sniffer/__init__.py
--rw-r--r--   0        0        0     1300 2023-03-29 02:34:22.133120 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/sniffer/illust_link.py
--rw-r--r--   0        0        0     1382 2023-02-13 05:42:01.863870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/utils.py
--rw-r--r--   0        0        0      112 2023-02-14 12:15:47.490983 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/watch/__init__.py
--rw-r--r--   0        0        0      799 2023-03-29 02:34:22.134122 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/watch/base.py
--rw-r--r--   0        0        0     2544 2023-03-29 02:34:22.135123 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/watch/following_illusts.py
--rw-r--r--   0        0        0     1963 2023-03-29 02:34:22.135123 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/watch/user_illusts.py
--rw-r--r--   0        0        0      530 2023-02-13 05:42:01.865869 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/model/__init__.py
--rw-r--r--   0        0        0     1366 2023-02-13 05:42:01.865869 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/model/identifier.py
--rw-r--r--   0        0        0     1786 2023-02-13 05:42:01.865869 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/model/illust.py
--rw-r--r--   0        0        0      352 2023-02-13 05:42:01.866870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/model/interval_task.py
--rw-r--r--   0        0        0      157 2023-02-13 05:42:01.867870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/model/message/__init__.py
--rw-r--r--   0        0        0     2623 2023-02-13 05:42:01.867870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/model/message/illust_message.py
--rw-r--r--   0        0        0     2443 2023-02-13 05:42:01.867870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/model/message/illust_messages.py
--rw-r--r--   0        0        0        0 2023-02-13 05:42:01.868870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/model/old/__init__.py
--rw-r--r--   0        0        0      120 2023-02-13 05:42:01.868870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/model/old/pixiv_binding.py
--rw-r--r--   0        0        0      950 2023-02-13 05:42:01.868870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/model/old/subscription.py
--rw-r--r--   0        0        0      242 2023-02-13 05:42:01.869870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/model/pixiv_binding.py
--rw-r--r--   0        0        0     1417 2023-02-13 05:42:01.869870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/model/subscription.py
--rw-r--r--   0        0        0      203 2023-02-13 05:42:01.870869 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/model/tag.py
--rw-r--r--   0        0        0      131 2023-02-13 05:42:01.870869 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/model/user.py
--rw-r--r--   0        0        0      242 2023-02-13 05:42:01.871622 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/model/user_preview.py
--rw-r--r--   0        0        0      973 2023-02-13 05:42:01.871870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/model/watch_task.py
--rw-r--r--   0        0        0     1680 2023-02-14 03:39:10.628376 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/plugin_service.py
--rw-r--r--   0        0        0        0 2023-02-13 05:42:01.872870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/protocol_dep/__init__.py
--rw-r--r--   0        0        0      914 2023-03-14 09:12:27.158624 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/protocol_dep/authenticator.py
--rw-r--r--   0        0        0     2757 2023-03-29 02:34:22.136711 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/protocol_dep/post_dest.py
--rw-r--r--   0        0        0     1445 2023-02-14 03:32:29.851104 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/protocol_dep/postman.py
--rw-r--r--   0        0        0     1452 2023-02-14 03:32:29.852102 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/protocol_dep/protocol_dep.py
--rw-r--r--   0        0        0       49 2023-02-13 05:42:01.874870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/service/__init__.py
--rw-r--r--   0        0        0     5511 2023-02-14 08:48:16.627933 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/service/interval_task_worker.py
--rw-r--r--   0        0        0     1035 2023-02-14 03:37:13.359166 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/service/pixiv_account_binder.py
--rw-r--r--   0        0        0     6177 2023-02-14 03:37:13.360166 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/service/pixiv_service.py
--rw-r--r--   0        0        0     2244 2023-02-13 05:42:01.877869 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/service/roulette.py
--rw-r--r--   0        0        0     5656 2023-03-29 02:34:22.137711 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/service/scheduler.py
--rw-r--r--   0        0        0     4083 2023-03-29 02:34:22.137711 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/service/watchman.py
--rw-r--r--   0        0        0        0 2023-02-13 05:42:01.878870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/utils/__init__.py
--rw-r--r--   0        0        0      230 2023-03-29 02:34:22.138709 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/utils/algorithm.py
--rw-r--r--   0        0        0      265 2023-02-13 05:42:01.879870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/utils/coros.py
--rw-r--r--   0        0        0     1148 2023-02-13 05:42:01.879870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/utils/decode_integer.py
--rw-r--r--   0        0        0      515 2023-02-13 05:42:01.879870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/utils/errors.py
--rw-r--r--   0        0        0     3604 2023-02-13 05:42:01.880869 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/utils/expires_lru_dict.py
--rw-r--r--   0        0        0      494 2023-02-13 05:42:01.880869 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/utils/lazy_delegation.py
--rw-r--r--   0        0        0     4188 2023-02-13 05:42:01.880869 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/utils/lifecycler.py
--rw-r--r--   0        0        0      776 2023-03-01 13:53:49.845581 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/utils/nonebot.py
--rw-r--r--   0        0        0     8753 2023-03-15 03:26:56.198873 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/utils/shared_agen.py
--rw-r--r--   0        0        0      384 2023-02-13 05:42:01.882870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot_kook/__init__.py
--rw-r--r--   0        0        0      866 2023-03-14 09:12:27.159625 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot_kook/config.py
--rw-r--r--   0        0        0        0 2023-02-13 05:42:01.883870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot_kook/protocol_dep/__init__.py
--rw-r--r--   0        0        0     5195 2023-03-23 15:08:25.496164 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot_kook/protocol_dep/authenticator.py
--rw-r--r--   0        0        0     5346 2023-03-23 15:08:25.498161 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot_kook/protocol_dep/post_dest.py
--rw-r--r--   0        0        0     2046 2023-02-14 03:32:29.855103 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot_kook/protocol_dep/postman.py
--rw-r--r--   0        0        0        0 2023-02-13 05:42:01.885870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot_kook/utils/__init__.py
--rw-r--r--   0        0        0     1083 2023-02-13 05:42:01.885870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot_kook/utils/card_builder.py
--rw-r--r--   0        0        0     1008 2023-02-13 05:42:01.886870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot_kook/utils/illust_card.py
--rw-r--r--   0        0        0      479 2023-03-29 02:34:22.139710 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot_onebot_v11/__init__.py
--rw-r--r--   0        0        0      896 2023-02-13 05:42:01.887870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot_onebot_v11/config.py
--rw-r--r--   0        0        0       20 2023-03-29 02:34:22.139710 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot_onebot_v11/handler/__init__.py
--rw-r--r--   0        0        0     1468 2023-03-29 02:34:22.140709 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot_onebot_v11/handler/poke.py
--rw-r--r--   0        0        0        0 2023-02-13 05:42:01.888870 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/__init__.py
--rw-r--r--   0        0        0     1512 2023-02-14 03:32:29.856103 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/authenticator.py
--rw-r--r--   0        0        0     4845 2023-03-14 09:12:27.162624 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/post_dest.py
--rw-r--r--   0        0        0     3442 2023-02-14 03:37:13.361166 nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/postman.py
--rw-r--r--   0        0        0    18830 1970-01-01 00:00:00.000000 nonebot_plugin_pixivbot-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-02-13 05:42:01.812872 nonebot_plugin_pixivbot-1.8.2/LICENSE
+-rw-r--r--   0        0        0     1825 2023-04-26 10:41:59.754033 nonebot_plugin_pixivbot-1.8.2/pyproject.toml
+-rw-r--r--   0        0        0    17350 2023-04-26 10:41:42.613891 nonebot_plugin_pixivbot-1.8.2/README.md
+-rw-r--r--   0        0        0     1192 2023-04-26 10:41:42.734890 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/__init__.py
+-rw-r--r--   0        0        0     7747 2023-04-26 10:41:42.786890 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/config.py
+-rw-r--r--   0        0        0     4322 2023-04-26 10:41:42.734890 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/context.py
+-rw-r--r--   0        0        0      443 2023-02-13 05:42:01.817870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/__init__.py
+-rw-r--r--   0        0        0       56 2023-02-13 05:42:01.817870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/errors.py
+-rw-r--r--   0        0        0     1515 2023-02-13 05:42:01.817870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/interval_task_repo.py
+-rw-r--r--   0        0        0      488 2023-04-26 10:41:42.735891 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/local_tag/__init__.py
+-rw-r--r--   0        0        0      535 2023-04-26 10:41:42.735891 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/local_tag/base.py
+-rw-r--r--   0        0        0     2643 2023-04-26 10:41:42.736891 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/local_tag/mongo.py
+-rw-r--r--   0        0        0     2702 2023-04-26 10:41:42.736891 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/local_tag/sql.py
+-rw-r--r--   0        0        0      541 2023-04-26 10:41:42.737892 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_binding/__init__.py
+-rw-r--r--   0        0        0      387 2023-04-26 10:41:42.737892 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_binding/base.py
+-rw-r--r--   0        0        0     2087 2023-04-26 10:41:42.738890 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_binding/mongo.py
+-rw-r--r--   0        0        0     2715 2023-04-26 10:41:42.739891 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_binding/sql.py
+-rw-r--r--   0        0        0      262 2023-02-13 05:42:01.821870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/__init__.py
+-rw-r--r--   0        0        0     1524 2023-02-13 05:42:01.822870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/base.py
+-rw-r--r--   0        0        0     1829 2023-04-26 10:41:42.739891 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/compressor.py
+-rw-r--r--   0        0        0      355 2023-02-13 05:42:01.822870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/enums.py
+-rw-r--r--   0        0        0      334 2023-02-13 05:42:01.823870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/errors.py
+-rw-r--r--   0        0        0     1036 2023-02-13 05:42:01.823870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/lazy_illust.py
+-rw-r--r--   0        0        0      826 2023-03-15 03:52:01.493698 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/__init__.py
+-rw-r--r--   0        0        0     2823 2023-03-15 03:26:56.195873 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/base.py
+-rw-r--r--   0        0        0     3419 2023-04-26 10:41:42.740890 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/dummy.py
+-rw-r--r--   0        0        0    31650 2023-04-26 10:41:42.820890 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/mongo.py
+-rw-r--r--   0        0        0     4802 2023-04-26 08:33:36.389185 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/mongo_models.py
+-rw-r--r--   0        0        0    33317 2023-04-26 10:41:42.821890 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql.py
+-rw-r--r--   0        0        0     3536 2023-04-26 08:33:36.390185 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql_models.py
+-rw-r--r--   0        0        0     9990 2023-04-26 10:41:42.822892 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator.py
+-rw-r--r--   0        0        0    22139 2023-04-26 10:41:42.822892 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator_repo.py
+-rw-r--r--   0        0        0      332 2023-04-26 10:41:42.823892 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/models.py
+-rw-r--r--   0        0        0    19437 2023-04-26 10:41:42.824894 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/remote_repo.py
+-rw-r--r--   0        0        0     1079 2023-02-13 05:42:01.829870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/__init__.py
+-rw-r--r--   0        0        0     1820 2023-02-13 05:42:01.830870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/lifecycle_mixin.py
+-rw-r--r--   0        0        0     3211 2023-02-13 05:42:01.830870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/migration_manager.py
+-rw-r--r--   0        0        0     5774 2023-04-26 10:41:42.787891 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/mongo/__init__.py
+-rw-r--r--   0        0        0      290 2023-04-26 10:41:42.743890 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/mongo/meta_info.py
+-rw-r--r--   0        0        0      693 2023-02-13 05:42:01.833870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/mongo/migration/__init__.py
+-rw-r--r--   0        0        0     1424 2023-02-13 05:42:01.833870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v1_to_v2.py
+-rw-r--r--   0        0        0      674 2023-02-13 05:42:01.833870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v2_to_v3.py
+-rw-r--r--   0        0        0     2729 2023-02-13 05:42:01.834869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v3_to_v4.py
+-rw-r--r--   0        0        0     1039 2023-02-13 05:42:01.834869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v4_to_v5.py
+-rw-r--r--   0        0        0     3306 2023-02-13 05:42:01.834869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v5_to_v6.py
+-rw-r--r--   0        0        0      416 2023-02-13 05:42:01.835870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v6_to_v7.py
+-rw-r--r--   0        0        0     5781 2023-04-26 10:41:42.788890 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/sql/__init__.py
+-rw-r--r--   0        0        0      306 2023-03-13 13:51:04.755048 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/sql/meta_info.py
+-rw-r--r--   0        0        0      457 2023-02-13 05:42:01.837870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/sql/migration/__init__.py
+-rw-r--r--   0        0        0     3824 2023-02-13 05:42:01.838869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v1_to_v2.py
+-rw-r--r--   0        0        0     1842 2023-02-13 05:42:01.839869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v2_to_v3.py
+-rw-r--r--   0        0        0      360 2023-02-13 05:42:01.839869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v3_to_v4.py
+-rw-r--r--   0        0        0      520 2023-04-26 10:41:42.744892 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/subscription/__init__.py
+-rw-r--r--   0        0        0      177 2023-04-26 10:41:42.745891 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/subscription/base.py
+-rw-r--r--   0        0        0     4446 2023-04-26 10:41:42.745891 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/subscription/mongo.py
+-rw-r--r--   0        0        0     5698 2023-04-26 10:41:42.746890 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/subscription/sql.py
+-rw-r--r--   0        0        0        0 2023-02-13 05:42:01.842870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/utils/__init__.py
+-rw-r--r--   0        0        0      164 2023-02-13 05:42:01.842870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/utils/shortuuid.py
+-rw-r--r--   0        0        0      814 2023-02-13 05:42:01.843869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/utils/sql/__init__.py
+-rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/utils/sql/utc_datetime.py
+-rw-r--r--   0        0        0      720 2023-02-13 05:42:01.842870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/utils/sql.pyi
+-rw-r--r--   0        0        0      517 2023-04-26 10:41:42.747890 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/watch_task/__init__.py
+-rw-r--r--   0        0        0      226 2023-04-26 10:41:42.747890 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/watch_task/base.py
+-rw-r--r--   0        0        0     5155 2023-04-26 10:41:42.748890 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/watch_task/mongo.py
+-rw-r--r--   0        0        0     6613 2023-04-26 10:41:42.748890 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/watch_task/sql.py
+-rw-r--r--   0        0        0      964 2023-03-15 03:24:39.857013 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/enums.py
+-rw-r--r--   0        0        0      102 2023-02-14 03:27:31.463009 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/global_context.py
+-rw-r--r--   0        0        0       92 2023-02-13 05:42:01.847870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/__init__.py
+-rw-r--r--   0        0        0     9597 2023-04-26 11:20:41.866640 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/base.py
+-rw-r--r--   0        0        0      308 2023-02-13 05:42:01.847870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/command/__init__.py
+-rw-r--r--   0        0        0     2489 2023-04-26 11:20:41.835065 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/command/bind.py
+-rw-r--r--   0        0        0     2481 2023-03-29 02:34:22.114209 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/command/command.py
+-rw-r--r--   0        0        0     1207 2023-04-26 11:20:41.815065 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/command/help.py
+-rw-r--r--   0        0        0      804 2023-04-26 11:20:41.870642 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/command/invalidate_cache.py
+-rw-r--r--   0        0        0     4291 2023-04-26 11:28:38.961827 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/command/schedule.py
+-rw-r--r--   0        0        0     1363 2023-03-29 02:34:22.116335 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/command/subcommand.py
+-rw-r--r--   0        0        0     6050 2023-04-26 11:28:38.966828 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/command/watch.py
+-rw-r--r--   0        0        0      633 2023-02-13 05:42:01.851870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/__init__.py
+-rw-r--r--   0        0        0      688 2023-03-29 02:34:22.117934 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/base.py
+-rw-r--r--   0        0        0     1629 2023-04-26 11:11:55.420381 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/illust.py
+-rw-r--r--   0        0        0     1440 2023-04-26 11:20:41.831066 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/more.py
+-rw-r--r--   0        0        0     2817 2023-04-26 11:20:41.858064 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/random_bookmark.py
+-rw-r--r--   0        0        0     1752 2023-04-26 11:20:41.846065 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/random_illust.py
+-rw-r--r--   0        0        0     1599 2023-04-26 11:20:41.862066 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/random_recommended_illust.py
+-rw-r--r--   0        0        0     2006 2023-04-26 11:20:41.839065 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/random_related_illust.py
+-rw-r--r--   0        0        0     2089 2023-04-26 11:20:41.819065 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/random_user_illust.py
+-rw-r--r--   0        0        0     4204 2023-04-26 11:20:41.854065 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/ranking.py
+-rw-r--r--   0        0        0        0 2023-02-13 05:42:01.857869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/__init__.py
+-rw-r--r--   0        0        0      524 2023-03-29 02:34:22.124122 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/base.py
+-rw-r--r--   0        0        0     2012 2023-03-29 02:34:22.125123 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/combined_interceptor.py
+-rw-r--r--   0        0        0     1380 2023-03-29 02:34:22.125123 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/default_error_interceptor.py
+-rw-r--r--   0        0        0     1134 2023-03-29 02:34:22.126120 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/loading_prompt_interceptor.py
+-rw-r--r--   0        0        0     1947 2023-03-29 02:34:54.094101 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/permission_interceptor.py
+-rw-r--r--   0        0        0      654 2023-03-29 02:34:22.127120 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/record_req_interceptor.py
+-rw-r--r--   0        0        0      919 2023-03-29 02:34:22.128120 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/retry_interceptor.py
+-rw-r--r--   0        0        0     1526 2023-03-29 02:34:22.128120 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/service_interceptor.py
+-rw-r--r--   0        0        0      673 2023-03-29 02:34:22.129121 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/timeout_interceptor.py
+-rw-r--r--   0        0        0      201 2023-02-13 05:42:01.861870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/pkg_context.py
+-rw-r--r--   0        0        0     3378 2023-04-26 10:41:42.749891 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/recorder.py
+-rw-r--r--   0        0        0      325 2023-02-14 11:56:02.041347 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/schedule/__init__.py
+-rw-r--r--   0        0        0      349 2023-04-26 11:20:41.850065 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/schedule/base.py
+-rw-r--r--   0        0        0      461 2023-03-29 02:34:22.131121 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/schedule/random_bookmark.py
+-rw-r--r--   0        0        0      453 2023-03-29 02:34:22.131121 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/schedule/random_illust.py
+-rw-r--r--   0        0        0      498 2023-03-29 02:34:22.132122 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/schedule/random_recommended_illust.py
+-rw-r--r--   0        0        0      470 2023-03-29 02:34:22.132122 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/schedule/random_user_illust.py
+-rw-r--r--   0        0        0      432 2023-03-29 02:34:22.133120 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/schedule/ranking.py
+-rw-r--r--   0        0        0       27 2023-02-13 05:42:01.862870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/sniffer/__init__.py
+-rw-r--r--   0        0        0     1011 2023-04-26 11:20:41.843065 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/sniffer/illust_link.py
+-rw-r--r--   0        0        0     1382 2023-02-13 05:42:01.863870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/utils.py
+-rw-r--r--   0        0        0      112 2023-02-14 12:15:47.490983 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/watch/__init__.py
+-rw-r--r--   0        0        0      865 2023-04-26 11:20:41.827066 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/watch/base.py
+-rw-r--r--   0        0        0     2498 2023-04-26 10:41:42.749891 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/watch/following_illusts.py
+-rw-r--r--   0        0        0     1864 2023-04-26 10:41:42.750890 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/watch/user_illusts.py
+-rw-r--r--   0        0        0      530 2023-02-13 05:42:01.865869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/__init__.py
+-rw-r--r--   0        0        0     1366 2023-02-13 05:42:01.865869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/identifier.py
+-rw-r--r--   0        0        0     1786 2023-02-13 05:42:01.865869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/illust.py
+-rw-r--r--   0        0        0      352 2023-02-13 05:42:01.866870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/interval_task.py
+-rw-r--r--   0        0        0      157 2023-02-13 05:42:01.867870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/message/__init__.py
+-rw-r--r--   0        0        0     2623 2023-02-13 05:42:01.867870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/message/illust_message.py
+-rw-r--r--   0        0        0     2443 2023-02-13 05:42:01.867870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/message/illust_messages.py
+-rw-r--r--   0        0        0        0 2023-02-13 05:42:01.868870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/old/__init__.py
+-rw-r--r--   0        0        0      120 2023-02-13 05:42:01.868870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/old/pixiv_binding.py
+-rw-r--r--   0        0        0      950 2023-02-13 05:42:01.868870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/old/subscription.py
+-rw-r--r--   0        0        0      242 2023-02-13 05:42:01.869870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/pixiv_binding.py
+-rw-r--r--   0        0        0     1450 2023-04-26 10:52:37.464803 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/subscription.py
+-rw-r--r--   0        0        0      203 2023-02-13 05:42:01.870869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/tag.py
+-rw-r--r--   0        0        0      131 2023-02-13 05:42:01.870869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/user.py
+-rw-r--r--   0        0        0      242 2023-02-13 05:42:01.871622 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/user_preview.py
+-rw-r--r--   0        0        0     1004 2023-04-26 10:52:37.460801 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/watch_task.py
+-rw-r--r--   0        0        0     1680 2023-02-14 03:39:10.628376 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/plugin_service.py
+-rw-r--r--   0        0        0        0 2023-02-13 05:42:01.872870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/protocol_dep/__init__.py
+-rw-r--r--   0        0        0      914 2023-03-14 09:12:27.158624 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/protocol_dep/authenticator.py
+-rw-r--r--   0        0        0     2757 2023-03-29 02:34:22.136711 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/protocol_dep/post_dest.py
+-rw-r--r--   0        0        0     1445 2023-02-14 03:32:29.851104 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/protocol_dep/postman.py
+-rw-r--r--   0        0        0     1452 2023-02-14 03:32:29.852102 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/protocol_dep/protocol_dep.py
+-rw-r--r--   0        0        0       49 2023-02-13 05:42:01.874870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/service/__init__.py
+-rw-r--r--   0        0        0     5469 2023-04-26 11:26:09.322980 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/service/interval_task_worker.py
+-rw-r--r--   0        0        0      958 2023-04-26 10:41:42.751891 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/service/pixiv_account_binder.py
+-rw-r--r--   0        0        0     6023 2023-04-26 10:41:42.751891 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/service/pixiv_service.py
+-rw-r--r--   0        0        0     2244 2023-02-13 05:42:01.877869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/service/roulette.py
+-rw-r--r--   0        0        0     5640 2023-04-26 10:41:42.752891 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/service/scheduler.py
+-rw-r--r--   0        0        0     3821 2023-04-26 10:41:42.752891 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/service/watchman.py
+-rw-r--r--   0        0        0        0 2023-02-13 05:42:01.878870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/utils/__init__.py
+-rw-r--r--   0        0        0      230 2023-03-29 02:34:22.138709 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/utils/algorithm.py
+-rw-r--r--   0        0        0      265 2023-02-13 05:42:01.879870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/utils/coros.py
+-rw-r--r--   0        0        0     1148 2023-02-13 05:42:01.879870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/utils/decode_integer.py
+-rw-r--r--   0        0        0      515 2023-02-13 05:42:01.879870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/utils/errors.py
+-rw-r--r--   0        0        0     3604 2023-02-13 05:42:01.880869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/utils/expires_lru_dict.py
+-rw-r--r--   0        0        0       95 2023-04-26 10:41:42.825893 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/utils/format.py
+-rw-r--r--   0        0        0      494 2023-02-13 05:42:01.880869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/utils/lazy_delegation.py
+-rw-r--r--   0        0        0     4188 2023-02-13 05:42:01.880869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/utils/lifecycler.py
+-rw-r--r--   0        0        0      776 2023-03-01 13:53:49.845581 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/utils/nonebot.py
+-rw-r--r--   0        0        0     8753 2023-03-15 03:26:56.198873 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/utils/shared_agen.py
+-rw-r--r--   0        0        0      384 2023-02-13 05:42:01.882870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_kook/__init__.py
+-rw-r--r--   0        0        0      866 2023-03-14 09:12:27.159625 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_kook/config.py
+-rw-r--r--   0        0        0        0 2023-02-13 05:42:01.883870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_kook/protocol_dep/__init__.py
+-rw-r--r--   0        0        0     5195 2023-03-23 15:08:25.496164 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_kook/protocol_dep/authenticator.py
+-rw-r--r--   0        0        0     5346 2023-03-23 15:08:25.498161 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_kook/protocol_dep/post_dest.py
+-rw-r--r--   0        0        0     2046 2023-02-14 03:32:29.855103 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_kook/protocol_dep/postman.py
+-rw-r--r--   0        0        0        0 2023-02-13 05:42:01.885870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_kook/utils/__init__.py
+-rw-r--r--   0        0        0     1083 2023-02-13 05:42:01.885870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_kook/utils/card_builder.py
+-rw-r--r--   0        0        0     1008 2023-02-13 05:42:01.886870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_kook/utils/illust_card.py
+-rw-r--r--   0        0        0      479 2023-04-26 08:29:16.962322 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_onebot_v11/__init__.py
+-rw-r--r--   0        0        0      896 2023-02-13 05:42:01.887870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_onebot_v11/config.py
+-rw-r--r--   0        0        0       20 2023-03-29 02:34:22.139710 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_onebot_v11/handler/__init__.py
+-rw-r--r--   0        0        0     1468 2023-03-29 02:34:22.140709 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_onebot_v11/handler/poke.py
+-rw-r--r--   0        0        0        0 2023-02-13 05:42:01.888870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/__init__.py
+-rw-r--r--   0        0        0     1512 2023-02-14 03:32:29.856103 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/authenticator.py
+-rw-r--r--   0        0        0     4845 2023-03-14 09:12:27.162624 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/post_dest.py
+-rw-r--r--   0        0        0     3346 2023-04-26 10:41:42.753891 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/postman.py
+-rw-r--r--   0        0        0    18886 1970-01-01 00:00:00.000000 nonebot_plugin_pixivbot-1.8.2/PKG-INFO
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/LICENSE` & `nonebot_plugin_pixivbot-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/pyproject.toml` & `nonebot_plugin_pixivbot-1.8.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-pixivbot"
-version = "1.8.1"
+version = "1.8.2"
 description = "Nonebot Plugin PixivBot"
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/ssttkkl/nonebot-plugin-pixivbot"
 packages = [
     { include = "nonebot_plugin_pixivbot", from = "src" },
@@ -34,14 +34,15 @@
 
 motor = { version = "^3.0.0", optional = true }
 beanie = { version = "^1.17.0", optional = true }
 
 SQLAlchemy = { version = "^2.0.0", extras = ["asyncio"] }
 aiosqlite = "^0.18.0"
 asyncpg = { version = "^0.27.0", optional = true }
+nonebot-plugin-localstore = "^0.4.1"
 
 [tool.poetry.group.dev.dependencies]
 nb-cli = "^1.0.5"
 flake8 = "^6.0.0"
 nonebug = "^0.3.1"
 pytest-mock = "^3.10.0"
 pytest-cov = "^4.0.0"
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/README.md` & `nonebot_plugin_pixivbot-1.8.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -260,15 +260,15 @@
 # OneBot平台（主要是gocq）配置
 pixiv_poke_action=random_recommended_illust  # 响应戳一戳动作，可选值：ranking, random_recommended_illust, random_bookmark, 什么都不填即忽略戳一戳动作
 pixiv_onebot_with_link=False  # 发图时是否带上链接（容易被tx盯上）
 pixiv_onebot_send_forward_message=auto  # 发图时是否使用转发消息的形式，可选值：always(永远使用), auto(仅在多张图片时使用), never(永远不使用)
 
 # 功能配置
 pixiv_more_enabled=True  # 启用重复上一次请求（还要）功能
-pixiv_query_expires_in=10*60  # 上一次请求的过期时间（单位：秒）
+pixiv_query_expires_in=600  # 上一次请求的过期时间（单位：秒）
 
 pixiv_illust_query_enabled=True  # 启用插画查询（看看图）功能
 
 pixiv_ranking_query_enabled=True  # 启用榜单查询（看看榜）功能
 pixiv_ranking_default_mode=day  # 默认查询的榜单，可选值：day, week, month, day_male, day_female, week_original, week_rookie, day_manga
 pixiv_ranking_default_range=[1, 3]  # 默认查询的榜单范围
 pixiv_ranking_fetch_item=150  # 每次从服务器获取的榜单项数（查询的榜单范围必须在这个数目内）
```

#### html2text {}

```diff
@@ -176,15 +176,15 @@
 random_bookmark, ä»ä¹é½ä¸å¡«å³å¿½ç¥æ³ä¸æ³å¨ä½
 pixiv_onebot_with_link=False #
 åå¾æ¶æ¯å¦å¸¦ä¸é¾æ¥ï¼å®¹æè¢«txç¯ä¸ï¼
 pixiv_onebot_send_forward_message=auto #
 åå¾æ¶æ¯å¦ä½¿ç¨è½¬åæ¶æ¯çå½¢å¼ï¼å¯éå¼ï¼always(æ°¸è¿ä½¿ç¨),
 auto(ä»å¨å¤å¼ å¾çæ¶ä½¿ç¨), never(æ°¸è¿ä¸ä½¿ç¨) # åè½éç½®
 pixiv_more_enabled=True # å¯ç¨éå¤ä¸ä¸æ¬¡è¯·æ±ï¼è¿è¦ï¼åè½
-pixiv_query_expires_in=10*60 # ä¸ä¸æ¬¡è¯·æ±çè¿ææ¶é´ï¼åä½ï¼ç§ï¼
+pixiv_query_expires_in=600 # ä¸ä¸æ¬¡è¯·æ±çè¿ææ¶é´ï¼åä½ï¼ç§ï¼
 pixiv_illust_query_enabled=True # å¯ç¨æç»æ¥è¯¢ï¼ççå¾ï¼åè½
 pixiv_ranking_query_enabled=True # å¯ç¨æ¦åæ¥è¯¢ï¼ççæ¦ï¼åè½
 pixiv_ranking_default_mode=day # é»è®¤æ¥è¯¢çæ¦åï¼å¯éå¼ï¼day, week,
 month, day_male, day_female, week_original, week_rookie, day_manga
 pixiv_ranking_default_range=[1, 3] # é»è®¤æ¥è¯¢çæ¦åèå´
 pixiv_ranking_fetch_item=150 #
 æ¯æ¬¡ä»æå¡å¨è·åçæ¦åé¡¹æ°ï¼æ¥è¯¢çæ¦åèå´å¿é¡»å¨è¿ä¸ªæ°ç®åï¼
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/config.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,38 @@
+from pathlib import Path
 from typing import Optional, List
 from urllib.parse import urlparse
 
-from nonebot import get_driver, logger
+from nonebot import get_driver, logger, require
 from pydantic import BaseSettings, validator, root_validator
 from pydantic.fields import ModelField
 
+require("nonebot_plugin_localstore")
+
+import nonebot_plugin_localstore as store
+
 from nonebot_plugin_pixivbot.enums import *
 from nonebot_plugin_pixivbot.enums import DataSourceType
 from nonebot_plugin_pixivbot.global_context import context
 
 
 def _deprecated_warn(name: str):
     logger.warning(f"config \"{name}\" is deprecated, use nonebot-plugin-access-control instead "
                    "(MORE INFO: https://github.com/ssttkkl/nonebot-plugin-pixivbot#%E6%9D%83%E9%99%90%E6%8E%A7%E5%88%B6)")
 
 
+def _get_default_sql_conn_url():
+    # 旧版本的sqlite数据库在working directory
+    data_file = Path("pixiv_bot.db")
+    if not data_file.exists():
+        data_file = store.get_data_file("nonebot_plugin_pixivbot", "pixiv_bot.db")
+
+    return "sqlite+aiosqlite:///" + str(data_file)
+
+
 @context.register_singleton(**get_driver().config.dict())
 class Config(BaseSettings):
     @root_validator(pre=True, allow_reuse=True)
     def deprecated_config(cls, values):
         for name in {"blacklist", "pixiv_query_cooldown", "pixiv_no_query_cooldown_users"}:
             if name in values:
                 _deprecated_warn(name)
@@ -46,15 +60,15 @@
 
         values["pixiv_data_source"] = pixiv_data_source
         return values
 
     @root_validator(pre=True, allow_reuse=True)
     def default_sql_conn_url(cls, values):
         if "pixiv_sql_conn_url" not in values:
-            values["pixiv_sql_conn_url"] = "sqlite+aiosqlite:///pixiv_bot.db"
+            values["pixiv_sql_conn_url"] = _get_default_sql_conn_url()
         return values
 
     @root_validator(pre=True, allow_reuse=True)
     def detect_sql_dialect(cls, values):
         pixiv_data_source = values["pixiv_data_source"]
 
         if pixiv_data_source == DataSourceType.sql:
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/context.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,23 +3,14 @@
 
 from nonebot.log import logger
 
 T = TypeVar("T")
 T2 = TypeVar("T2")
 
 
-class Inject:
-    def __init__(self, key):
-        self._key = key
-
-    def __get__(self, instance, owner):
-        context = getattr(instance, "__context__")
-        return context.require(self._key)
-
-
 class Provider(ABC, Generic[T]):
     @abstractmethod
     def provide(self) -> T:
         raise NotImplementedError()
 
 
 class InstanceProvider(Provider[T], Generic[T]):
@@ -150,13 +141,9 @@
         if key in self._container:
             return True
         elif self._parent is not None:
             return self._parent.__contains__(key)
         else:
             return False
 
-    def inject(self, cls: Type[T]):
-        setattr(cls, "__context__", self)
-        return cls
-
 
-__all__ = ("Context", "Inject")
+__all__ = ("Context", )
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/interval_task_repo.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/interval_task_repo.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/local_tag/__init__.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,41 @@
-from typing import Optional, Protocol, Collection
+from typing import Protocol, Callable, Union, Awaitable, Any
 
 from nonebot_plugin_pixivbot.config import Config
+from nonebot_plugin_pixivbot.enums import DataSourceType
 from nonebot_plugin_pixivbot.global_context import context
-from nonebot_plugin_pixivbot.model import Tag, Illust
-from ...enums import DataSourceType
 
 
-class LocalTagRepo(Protocol):
-    async def find_by_name(self, name: str) -> Optional[Tag]:
+class DataSource(Protocol):
+    async def initialize(self):
         ...
 
-    async def find_by_translated_name(self, translated_name: str) -> Optional[Tag]:
+    async def close(self):
         ...
 
-    async def update_one(self, tag: Tag):
+    def on_initializing(self, func: Callable[[], Union[None, Awaitable[None]]]):
         ...
 
-    async def update_many(self, tags: Collection[Tag]):
+    def on_initialized(self, func: Callable[[], Union[None, Awaitable[None]]]):
         ...
 
-    async def update_from_illusts(self, illusts: Collection[Illust]):
+    def on_closing(self, func: Callable[[], Union[None, Awaitable[None]]]):
+        ...
+
+    def on_closed(self, func: Callable[[], Union[None, Awaitable[None]]]):
+        ...
+
+    def start_session(self) -> Any:
         ...
 
 
 conf = context.require(Config)
 if conf.pixiv_data_source == DataSourceType.mongo:
-    from .mongo import MongoLocalTagRepo
+    from .mongo import MongoDataSource
 
-    context.bind(LocalTagRepo, MongoLocalTagRepo)
+    context.bind(DataSource, MongoDataSource)
 else:
-    from .sql import SqlLocalTagRepo
+    from .sql import SqlDataSource
 
-    context.bind(LocalTagRepo, SqlLocalTagRepo)
+    context.bind(DataSource, SqlDataSource)
 
-__all__ = ("LocalTagRepo",)
+__all__ = ("DataSource",)
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/local_tag/mongo.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/local_tag/mongo.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 from typing import Optional, Collection
 
 from beanie.odm.operators.update.general import SetOnInsert
 from nonebot import logger
 from pymongo import *
 
-from nonebot_plugin_pixivbot.context import Inject
 from nonebot_plugin_pixivbot.global_context import context
 from nonebot_plugin_pixivbot.model import Tag, Illust
+from .base import LocalTagRepo
 from ..source.mongo import MongoDataSource, MongoDocument
 
 
 class LocalTag(Tag, MongoDocument):
     class Settings:
         name = "local_tags"
         indexes = [
             IndexModel([("name", 1)], unique=True),
             IndexModel([("translated_name", 1)])
         ]
 
 
-@context.inject
+data_source = context.require(MongoDataSource)
+
+
 @context.register_singleton()
-class MongoLocalTagRepo:
-    data_source: MongoDataSource = Inject(MongoDataSource)
+class MongoLocalTagRepo(LocalTagRepo):
 
     async def find_by_name(self, name: str) -> Optional[Tag]:
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             result = await LocalTag.find_one(LocalTag.name == name, session=session)
             return result
 
     async def find_by_translated_name(self, translated_name: str) -> Optional[Tag]:
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             result = await LocalTag.find_one(LocalTag.translated_name == translated_name, session=session)
             return result
 
     async def update_one(self, tag: Tag):
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             await LocalTag.find_one(LocalTag.name == tag.name, session=session).upsert(
                 SetOnInsert({LocalTag.translated_name: tag.translated_name}),
                 on_insert=LocalTag(**tag.dict()),
                 session=session
             )
 
     async def update_many(self, tags: Collection[Tag]):
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             # BulkWriter存在bug，upsert不生效
             # https://github.com/roman-right/beanie/issues/224
 
             opt = []
 
             for tag in tags:
                 opt.append(UpdateOne(
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/local_tag/sql.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/local_tag/sql.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,59 +1,60 @@
 from typing import Optional, Collection
 
 from nonebot import logger
 from sqlalchemy import select
 from sqlalchemy.orm import mapped_column, Mapped
 
-from nonebot_plugin_pixivbot.context import Inject
 from nonebot_plugin_pixivbot.data.source.sql import SqlDataSource
 from nonebot_plugin_pixivbot.data.utils.sql import insert
 from nonebot_plugin_pixivbot.global_context import context
 from nonebot_plugin_pixivbot.model import Tag, Illust
+from .base import LocalTagRepo
 
 
 @SqlDataSource.registry.mapped
 class LocalTag:
     __tablename__ = "local_tag"
 
     name: Mapped[str] = mapped_column(primary_key=True)
     translated_name: Mapped[str] = mapped_column(index=True)
 
 
-@context.inject
+data_source = context.require(SqlDataSource)
+
+
 @context.register_singleton()
-class SqlLocalTagRepo:
-    data_source: SqlDataSource = Inject(SqlDataSource)
+class SqlLocalTagRepo(LocalTagRepo):
 
     async def find_by_name(self, name: str) -> Optional[Tag]:
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             stmt = select(LocalTag).where(LocalTag.name == name).limit(1)
             local_tag = (await session.execute(stmt)).scalar_one_or_none()
             if local_tag is not None:
                 return Tag.from_orm(local_tag)
             else:
                 return None
 
     async def find_by_translated_name(self, translated_name: str) -> Optional[Tag]:
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             stmt = select(LocalTag).where(LocalTag.translated_name == translated_name).limit(1)
             local_tag = (await session.execute(stmt)).scalar_one_or_none()
             if local_tag is not None:
                 return Tag.from_orm(local_tag)
             else:
                 return None
 
     async def update_one(self, tag: Tag):
         await self.update_many([tag])
 
     async def update_many(self, tags: Collection[Tag]):
         if len(tags) == 0:
             return
 
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             stmt = insert(LocalTag).values([t.dict() for t in tags])
             stmt = stmt.on_conflict_do_update(index_elements=[LocalTag.name],
                                               set_={
                                                   LocalTag.translated_name: stmt.excluded.translated_name
                                               })
 
             await session.execute(stmt)
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/pixiv_binding/mongo.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_binding/mongo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 from typing import Optional, Any
 
 from beanie.odm.operators.update.general import Set
 from pymongo import IndexModel
 
 from nonebot_plugin_pixivbot.global_context import context
 from nonebot_plugin_pixivbot.model import PixivBinding, T_UID
+from .base import PixivBindingRepo
 from ..source.mongo import MongoDataSource, MongoDocument
-from ...context import Inject
 
 
 class PixivBindingDocument(PixivBinding[Any], MongoDocument):
     class Settings:
         name = "pixiv_binding"
         indexes = [
             IndexModel([("adapter", 1), ("user_id", 1)], unique=True)
         ]
 
 
-@context.inject
+data_source = context.require(MongoDataSource)
+
+
 @context.register_singleton()
-class MongoPixivBindingRepo:
-    data_source: MongoDataSource = Inject(MongoDataSource)
+class MongoPixivBindingRepo(PixivBindingRepo):
 
     async def get(self, adapter: str, user_id: T_UID) -> Optional[PixivBinding]:
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             result = await PixivBindingDocument.find_one(
                 PixivBindingDocument.adapter == adapter,
                 PixivBindingDocument.user_id == user_id,
                 session=session
             )
             return result
 
     async def update(self, binding: PixivBinding):
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             await PixivBindingDocument.find_one(
                 PixivBindingDocument.adapter == binding.adapter,
                 PixivBindingDocument.user_id == binding.user_id,
                 session=session
             ).upsert(
                 Set({PixivBindingDocument.pixiv_user_id: binding.pixiv_user_id}),
                 on_insert=PixivBindingDocument(**binding.dict()),
                 session=session
             )
 
     async def remove(self, adapter: str, user_id: T_UID) -> bool:
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             cnt = await PixivBindingDocument.find_one(
                 PixivBindingDocument.adapter == adapter,
                 PixivBindingDocument.user_id == user_id,
                 session=session
             ).delete(session=session)
             return cnt == 1
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/pixiv_binding/sql.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_binding/sql.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,62 +1,63 @@
 from typing import Optional
 
 from sqlalchemy import select, delete
 from sqlalchemy.orm import Mapped, mapped_column
 
-from nonebot_plugin_pixivbot.context import Inject
 from nonebot_plugin_pixivbot.data.source.sql import SqlDataSource
 from nonebot_plugin_pixivbot.data.utils.sql import insert
 from nonebot_plugin_pixivbot.global_context import context
 from nonebot_plugin_pixivbot.model import PixivBinding, T_UID
+from .base import PixivBindingRepo
 
 
 @SqlDataSource.registry.mapped
 class PixivBindingOrm:
     __tablename__ = "pixiv_binding"
 
     adapter: Mapped[str] = mapped_column(primary_key=True)
     user_id: Mapped[str] = mapped_column(primary_key=True)
     pixiv_user_id: Mapped[int]
 
 
-@context.inject
+data_source = context.require(SqlDataSource)
+
+
 @context.register_singleton()
-class SqlPixivBindingRepo:
-    data_source: SqlDataSource = Inject(SqlDataSource)
+class SqlPixivBindingRepo(PixivBindingRepo):
 
     async def get(self, adapter: str, user_id: T_UID) -> Optional[PixivBinding]:
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             stmt = (select(PixivBindingOrm)
                     .where(PixivBindingOrm.adapter == adapter,
                            PixivBindingOrm.user_id == str(user_id))
                     .limit(1))
             result = (await session.execute(stmt)).scalar_one_or_none()
             if result is not None:
                 return PixivBinding(adapter=result.adapter,
                                     user_id=type(user_id)(result.user_id),
                                     pixiv_user_id=result.pixiv_user_id)
             else:
                 return None
 
     async def update(self, binding: PixivBinding[T_UID]):
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             stmt = (insert(PixivBindingOrm)
                     .values(adapter=binding.adapter,
                             user_id=str(binding.user_id),
                             pixiv_user_id=binding.pixiv_user_id)
                     .on_conflict_do_update(index_elements=[PixivBindingOrm.adapter, PixivBindingOrm.user_id],
                                            set_={
                                                PixivBindingOrm.pixiv_user_id: binding.pixiv_user_id
                                            }))
             await session.execute(stmt)
             await session.commit()
 
     async def remove(self, adapter: str, user_id: T_UID) -> bool:
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             stmt = (delete(PixivBinding)
                     .where(PixivBindingOrm.adapter == adapter,
                            PixivBindingOrm.user_id == str(user_id)))
             result = await session.execute(stmt)
             await session.commit()
             return result.rowcount == 1
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/pixiv_repo/base.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/pixiv_repo/compressor.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/compressor.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,27 +3,26 @@
 import multiprocessing
 from concurrent.futures.thread import ThreadPoolExecutor
 from io import BytesIO
 
 from PIL import Image, ImageFile
 
 from nonebot_plugin_pixivbot.config import Config
-from nonebot_plugin_pixivbot.context import Inject
 from nonebot_plugin_pixivbot.global_context import context
 
+conf = context.require(Config)
+
 
-@context.inject
 @context.register_singleton()
 class Compressor:
-    _conf = Inject(Config)
 
     def __init__(self) -> None:
-        self.enabled = self._conf.pixiv_compression_enabled
-        self.max_size = self._conf.pixiv_compression_max_size
-        self.quantity = self._conf.pixiv_compression_quantity
+        self.enabled = conf.pixiv_compression_enabled
+        self.max_size = conf.pixiv_compression_max_size
+        self.quantity = conf.pixiv_compression_quantity
 
         if self.enabled:
             cpu_count = multiprocessing.cpu_count()
             self._executor = ThreadPoolExecutor(cpu_count, "compressor")
             # logger.info(f"A ThreadPool with {cpu_count} worker(s) was created for compression")
 
     async def compress(self, content: bytes) -> bytes:
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/pixiv_repo/lazy_illust.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/lazy_illust.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/__init__.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/base.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/dummy.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/dummy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from nonebot_plugin_pixivbot.data.pixiv_repo.errors import NoSuchItemError
 from nonebot_plugin_pixivbot.data.pixiv_repo.local_repo import LocalPixivRepo
 
 from nonebot_plugin_pixivbot.global_context import context
 
 
-@context.inject
 @context.register_singleton()
 class DummyPixivRepo(LocalPixivRepo):
     # ================ illust_detail ================
     async def illust_detail(self, *args, **kwargs):
         raise NoSuchItemError()
         yield None
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/mongo.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/mongo.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from beanie.odm.operators.update.array import AddToSet, Pull, Push
 from beanie.odm.operators.update.general import Set
 from nonebot import logger
 from pymongo import UpdateOne
 from pymongo.client_session import ClientSession
 
 from nonebot_plugin_pixivbot.config import Config
-from nonebot_plugin_pixivbot.context import Inject
 from nonebot_plugin_pixivbot.enums import RankingMode
 from nonebot_plugin_pixivbot.global_context import context
 from nonebot_plugin_pixivbot.model import Illust, User
 from .base import LocalPixivRepo
 from .mongo_models import UserDetailCache, PixivRepoCache, IllustDetailCache, IllustSetCache, UserSetCache, \
     SearchIllustCache, SearchUserCache, UserIllustsCache, UserBookmarksCache, OtherIllustCache, RelatedIllustsCache, \
     IllustRankingCache, DownloadCache
@@ -27,31 +26,32 @@
 
 
 def _handle_expires_in(metadata: PixivRepoMetadata, expires_in: int):
     if datetime.now(timezone.utc) - metadata.update_time >= timedelta(seconds=expires_in):
         raise CacheExpiredError(metadata)
 
 
-@context.inject
+conf = context.require(Config)
+data_source = context.require(MongoDataSource)
+local_tags = context.require(LocalTagRepo)
+
+
 @context.register_singleton()
 class MongoPixivRepo(LocalPixivRepo):
-    conf: Config = Inject(Config)
-    data_source: MongoDataSource = Inject(MongoDataSource)
-    local_tag_repo: LocalTagRepo = Inject(LocalTagRepo)
 
     async def _add_to_local_tags(self, illusts: List[Union[LazyIllust, Illust]]):
         li = []
         for x in illusts:
             if isinstance(x, LazyIllust):
                 if not x.loaded:
                     continue
                 x = x.content
             li.append(x)
 
-        await self.local_tag_repo.update_from_illusts(li)
+        await local_tags.update_from_illusts(li)
 
     async def _illusts_agen(self, session: ClientSession,
                             doc_type: Type[PixivRepoCache],
                             *criteria: Union[Mapping[str, Any], bool],
                             offset: int = 0) -> AsyncGenerator[LazyIllust, None]:
         aggregation = [
             {
@@ -99,15 +99,15 @@
                 total += 1
                 if "illust" in x and x["illust"] is not None:
                     yield LazyIllust(x["illust_id"], Illust.parse_obj(x["illust"]))
                 else:
                     yield LazyIllust(x["illust_id"])
                     broken += 1
         finally:
-            logger.info(f"[local] got {total} illusts, illust_detail of {broken} are missed")
+            logger.debug(f"[local] got {total} illusts, illust_detail of {broken} are missed")
 
     async def _users_agen(self, session: ClientSession,
                           doc_type: Type[PixivRepoCache],
                           *criteria: Union[Mapping[str, Any], bool],
                           offset: int = 0) -> AsyncGenerator[User, None]:
         aggregation = [
             {
@@ -152,15 +152,15 @@
             async for x in doc_type.aggregate(aggregation, session=session):
                 if "user" in x and x["user"] is not None:
                     yield User.parse_obj(x["user"])
                 else:
                     yield User(id=x["user_id"], name="", account="")
                 total += 1
         finally:
-            logger.info(f"[local] got {total} users")
+            logger.debug(f"[local] got {total} users")
 
     async def _get_illusts(self, session: ClientSession,
                            doc_type: Type[PixivRepoCache],
                            *criteria: Union[Mapping[str, Any], bool],
                            expired_in: int,
                            offset: int = 0) \
             -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], Any]:
@@ -288,15 +288,15 @@
                         "metadata": {"update_time": metadata.update_time}
                     }},
                     upsert=True
                 ))
         if len(opt) != 0:
             await IllustDetailCache.get_motor_collection().bulk_write(opt, ordered=False, session=session)
 
-        if self.conf.pixiv_tag_translation_enabled:
+        if conf.pixiv_tag_translation_enabled:
             await self._add_to_local_tags(content)
 
     async def _update_users(self, session: ClientSession,
                             doc_type: Type[UserSetCache],
                             *criteria: Union[Mapping[str, Any], bool],
                             content: List[User],
                             metadata: PixivRepoMetadata,
@@ -348,15 +348,15 @@
                 {"$set": {
                     "user": user.dict(exclude_none=True),
                     "metadata": {"update_time": metadata.update_time}
                 }},
                 upsert=True
             ))
         if len(opt) != 0:
-            await self.data_source.db.user_detail_cache.bulk_write(opt, ordered=False, session=session)
+            await data_source.db.user_detail_cache.bulk_write(opt, ordered=False, session=session)
 
     async def _append_and_check_illusts(self, session: ClientSession,
                                         doc_type: Type[IllustSetCache],
                                         *criteria: Union[Mapping[str, Any], bool],
                                         content: List[Union[Illust, LazyIllust]],
                                         metadata: PixivRepoMetadata,
                                         append_at_begin: bool = False):
@@ -373,63 +373,63 @@
         exists = await self._check_users_exists(session, doc_type, *criteria, user_id=[x.id for x in content])
         await self._update_users(session, doc_type, *criteria, content=content, metadata=metadata, append=True)
         return exists
 
     # ================ illust_detail ================
     async def illust_detail(self, illust_id: int) \
             -> AsyncGenerator[Union[Illust, PixivRepoMetadata], None]:
-        logger.info(f"[local] illust_detail {illust_id}")
-        async with self.data_source.start_session() as session:
+        logger.debug(f"[local] illust_detail {illust_id}")
+        async with data_source.start_session() as session:
             doc = await IllustDetailCache.find_one(IllustDetailCache.illust.id == illust_id, session=session)
             if doc is not None:
-                _handle_expires_in(doc.metadata, self.conf.pixiv_illust_detail_cache_expires_in)
+                _handle_expires_in(doc.metadata, conf.pixiv_illust_detail_cache_expires_in)
 
                 yield doc.metadata
                 yield doc.illust
             else:
                 raise NoSuchItemError()
 
     async def update_illust_detail(self, illust: Illust, metadata: PixivRepoMetadata):
-        logger.info(f"[local] update illust_detail {illust.id} {metadata}")
+        logger.debug(f"[local] update illust_detail {illust.id} {metadata}")
 
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             await IllustDetailCache.find_one(
                 IllustDetailCache.illust.id == illust.id,
                 session=session
             ).update(
                 Set({
                     IllustDetailCache.illust: illust,
                     IllustDetailCache.metadata: metadata
                 }),
                 upsert=True,
                 session=session
             )
 
-            if self.conf.pixiv_tag_translation_enabled:
+            if conf.pixiv_tag_translation_enabled:
                 await self._add_to_local_tags([illust])
 
     # ================ user_detail ================
     async def user_detail(self, user_id: int) \
             -> AsyncGenerator[Union[User, PixivRepoMetadata], None]:
-        logger.info(f"[local] user_detail {user_id}")
-        async with self.data_source.start_session() as session:
+        logger.debug(f"[local] user_detail {user_id}")
+        async with data_source.start_session() as session:
             doc: Optional[UserDetailCache] = await UserDetailCache.find_one(UserDetailCache.user.id == user_id,
                                                                             session=session)
             if doc is not None:
-                _handle_expires_in(doc.metadata, self.conf.pixiv_user_detail_cache_expires_in)
+                _handle_expires_in(doc.metadata, conf.pixiv_user_detail_cache_expires_in)
 
                 yield doc.metadata
                 yield doc.user
             else:
                 raise NoSuchItemError()
 
     async def update_user_detail(self, user: User, metadata: PixivRepoMetadata):
-        logger.info(f"[local] update user_detail {user.id} {metadata}")
+        logger.debug(f"[local] update user_detail {user.id} {metadata}")
 
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             if not metadata:
                 metadata = PixivRepoMetadata(update_time=datetime.now(timezone.utc))
 
             await UserDetailCache.find_one(
                 UserDetailCache.user.id == user.id,
                 session=session
             ).update(
@@ -440,229 +440,229 @@
                 upsert=True,
                 session=session
             )
 
     # ================ search_illust ================
     async def search_illust(self, word: str, *, offset: int = 0) \
             -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-        logger.info(f"[local] search_illust {word}")
-        async with self.data_source.start_session() as session:
+        logger.debug(f"[local] search_illust {word}")
+        async with data_source.start_session() as session:
             async for x in self._get_illusts(session, SearchIllustCache, SearchIllustCache.word == word,
-                                             expired_in=self.conf.pixiv_search_illust_cache_expires_in, offset=offset):
+                                             expired_in=conf.pixiv_search_illust_cache_expires_in, offset=offset):
                 yield x
 
     async def invalidate_search_illust(self, word: str):
-        logger.info(f"[local] invalidate search_illust {word}")
-        async with self.data_source.start_session() as session:
-            await self.data_source.db.search_illust_cache.delete_one({"word": word}, session=session)
+        logger.debug(f"[local] invalidate search_illust {word}")
+        async with data_source.start_session() as session:
+            await data_source.db.search_illust_cache.delete_one({"word": word}, session=session)
 
     async def append_search_illust(self, word: str, content: List[Union[Illust, LazyIllust]],
                                    metadata: PixivRepoMetadata) -> bool:
         # 返回值表示content中是否有已经存在于集合的文档，下同
-        logger.info(f"[local] append search_illust {word} "
+        logger.debug(f"[local] append search_illust {word} "
                     f"({len(content)} items) "
                     f"{metadata}")
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             return await self._append_and_check_illusts(session, SearchIllustCache, SearchIllustCache.word == word,
                                                         content=content, metadata=metadata)
 
     # ================ search_user ================
     async def search_user(self, word: str, *, offset: int = 0) \
             -> AsyncGenerator[Union[User, PixivRepoMetadata], None]:
-        logger.info(f"[local] search_user {word}")
-        async with self.data_source.start_session() as session:
+        logger.debug(f"[local] search_user {word}")
+        async with data_source.start_session() as session:
             async for x in self._get_users(session, SearchUserCache, SearchUserCache.word == word,
-                                           expired_in=self.conf.pixiv_search_user_cache_expires_in, offset=offset):
+                                           expired_in=conf.pixiv_search_user_cache_expires_in, offset=offset):
                 yield x
 
     async def invalidate_search_user(self, word: str):
-        logger.info(f"[local] invalidate search_user {word}")
-        async with self.data_source.start_session() as session:
+        logger.debug(f"[local] invalidate search_user {word}")
+        async with data_source.start_session() as session:
             await SearchUserCache.find_one(SearchUserCache.word == word, session=session).delete()
 
     async def append_search_user(self, word: str, content: List[User],
                                  metadata: PixivRepoMetadata) -> bool:
-        logger.info(f"[local] append search_user {word} "
+        logger.debug(f"[local] append search_user {word} "
                     f"({len(content)} items) "
                     f"{metadata}")
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             return await self._append_and_check_users(session, SearchUserCache, SearchUserCache.word == word,
                                                       content=content, metadata=metadata)
 
     # ================ user_illusts ================
     async def user_illusts(self, user_id: int, *, offset: int = 0) \
             -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-        logger.info(f"[local] user_illusts {user_id}")
-        async with self.data_source.start_session() as session:
+        logger.debug(f"[local] user_illusts {user_id}")
+        async with data_source.start_session() as session:
             async for x in self._get_illusts(session, UserIllustsCache, UserIllustsCache.user_id == user_id,
-                                             expired_in=self.conf.pixiv_user_illusts_cache_expires_in, offset=offset):
+                                             expired_in=conf.pixiv_user_illusts_cache_expires_in, offset=offset):
                 yield x
 
     async def invalidate_user_illusts(self, user_id: int):
-        logger.info(f"[local] invalidate user_illusts {user_id}")
-        async with self.data_source.start_session() as session:
+        logger.debug(f"[local] invalidate user_illusts {user_id}")
+        async with data_source.start_session() as session:
             await UserIllustsCache.find_one(UserIllustsCache.user_id == user_id, session=session).delete()
 
     async def append_user_illusts(self, user_id: int,
                                   content: List[Union[Illust, LazyIllust]],
                                   metadata: PixivRepoMetadata,
                                   append_at_begin: bool = False) -> bool:
-        logger.info(f"[local] append user_illusts {user_id} "
+        logger.debug(f"[local] append user_illusts {user_id} "
                     f"{'at begin ' if append_at_begin else ''}"
                     f"({len(content)} items) "
                     f"{metadata}")
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             return await self._append_and_check_illusts(session, UserIllustsCache, UserIllustsCache.user_id == user_id,
                                                         content=content, metadata=metadata,
                                                         append_at_begin=append_at_begin)
 
     # ================ user_bookmarks ================
     async def user_bookmarks(self, user_id: int = 0, *, offset: int = 0) \
             -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-        logger.info(f"[local] user_bookmarks {user_id}")
-        async with self.data_source.start_session() as session:
+        logger.debug(f"[local] user_bookmarks {user_id}")
+        async with data_source.start_session() as session:
             async for x in self._get_illusts(session, UserBookmarksCache, UserBookmarksCache.user_id == user_id,
-                                             expired_in=self.conf.pixiv_user_bookmarks_cache_expires_in, offset=offset):
+                                             expired_in=conf.pixiv_user_bookmarks_cache_expires_in, offset=offset):
                 yield x
 
     async def invalidate_user_bookmarks(self, user_id: int):
-        logger.info(f"[local] invalidate user_bookmarks {user_id}")
-        async with self.data_source.start_session() as session:
+        logger.debug(f"[local] invalidate user_bookmarks {user_id}")
+        async with data_source.start_session() as session:
             await UserBookmarksCache.find_one(UserBookmarksCache.user_id == user_id, session=session).delete()
 
     async def append_user_bookmarks(self, user_id: int,
                                     content: List[Union[Illust, LazyIllust]],
                                     metadata: PixivRepoMetadata,
                                     append_at_begin: bool = False) -> bool:
-        logger.info(f"[local] append user_bookmarks {user_id} "
+        logger.debug(f"[local] append user_bookmarks {user_id} "
                     f"{'at begin ' if append_at_begin else ''}"
                     f"({len(content)} items) "
                     f"{metadata}")
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             return await self._append_and_check_illusts(session, UserBookmarksCache,
                                                         UserBookmarksCache.user_id == user_id,
                                                         content=content, metadata=metadata,
                                                         append_at_begin=append_at_begin)
 
     # ================ recommended_illusts ================
     async def recommended_illusts(self, *, offset: int = 0) \
             -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-        logger.info(f"[local] recommended_illusts")
-        async with self.data_source.start_session() as session:
+        logger.debug(f"[local] recommended_illusts")
+        async with data_source.start_session() as session:
             async for x in self._get_illusts(session, OtherIllustCache, OtherIllustCache.type == "recommended_illusts",
-                                             expired_in=self.conf.pixiv_other_cache_expires_in, offset=offset):
+                                             expired_in=conf.pixiv_other_cache_expires_in, offset=offset):
                 yield x
 
     async def invalidate_recommended_illusts(self):
-        logger.info(f"[local] invalidate recommended_illusts")
-        async with self.data_source.start_session() as session:
+        logger.debug(f"[local] invalidate recommended_illusts")
+        async with data_source.start_session() as session:
             await OtherIllustCache.find_one(OtherIllustCache.type == "recommended_illusts",
                                             session=session).delete()
 
     async def append_recommended_illusts(self, content: List[Union[Illust, LazyIllust]],
                                          metadata: PixivRepoMetadata) -> bool:
-        logger.info(f"[local] append recommended_illusts "
+        logger.debug(f"[local] append recommended_illusts "
                     f"({len(content)} items) "
                     f"{metadata}")
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             return await self._append_and_check_illusts(session, OtherIllustCache,
                                                         OtherIllustCache.type == "recommended_illusts",
                                                         content=content, metadata=metadata)
 
     # ================ related_illusts ================
     async def related_illusts(self, illust_id: int, *, offset: int = 0) \
             -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-        logger.info(f"[local] related_illusts {illust_id}")
-        async with self.data_source.start_session() as session:
+        logger.debug(f"[local] related_illusts {illust_id}")
+        async with data_source.start_session() as session:
             async for x in self._get_illusts(session, RelatedIllustsCache,
                                              RelatedIllustsCache.original_illust_id == illust_id,
-                                             expired_in=self.conf.pixiv_related_illusts_cache_expires_in,
+                                             expired_in=conf.pixiv_related_illusts_cache_expires_in,
                                              offset=offset):
                 yield x
 
     async def invalidate_related_illusts(self, illust_id: int):
-        logger.info(f"[local] invalidate related_illusts")
-        async with self.data_source.start_session() as session:
+        logger.debug(f"[local] invalidate related_illusts")
+        async with data_source.start_session() as session:
             await RelatedIllustsCache.find_one(RelatedIllustsCache.original_illust_id == illust_id,
                                                session=session).delete()
 
     async def append_related_illusts(self, illust_id: int, content: List[Union[Illust, LazyIllust]],
                                      metadata: PixivRepoMetadata) -> bool:
-        logger.info(f"[local] append related_illusts {illust_id} "
+        logger.debug(f"[local] append related_illusts {illust_id} "
                     f"({len(content)} items) "
                     f"{metadata}")
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             return await self._append_and_check_illusts(session, RelatedIllustsCache,
                                                         RelatedIllustsCache.original_illust_id == illust_id,
                                                         content=content, metadata=metadata)
 
     # ================ illust_ranking ================
     async def illust_ranking(self, mode: Union[str, RankingMode], *, offset: int = 0) \
             -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
         if isinstance(mode, str):
             mode = RankingMode[mode]
 
-        logger.info(f"[local] illust_ranking {mode}")
+        logger.debug(f"[local] illust_ranking {mode}")
 
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             async for x in self._get_illusts(session, IllustRankingCache, IllustRankingCache.mode == mode,
-                                             expired_in=self.conf.pixiv_illust_ranking_cache_expires_in, offset=offset):
+                                             expired_in=conf.pixiv_illust_ranking_cache_expires_in, offset=offset):
                 yield x
 
     async def invalidate_illust_ranking(self, mode: RankingMode):
-        logger.info(f"[local] invalidate illust_ranking")
-        async with self.data_source.start_session() as session:
+        logger.debug(f"[local] invalidate illust_ranking")
+        async with data_source.start_session() as session:
             await IllustRankingCache.find_one(IllustRankingCache.mode == mode,
                                               session=session).delete()
 
     async def append_illust_ranking(self, mode: RankingMode, content: List[Union[Illust, LazyIllust]],
                                     metadata: PixivRepoMetadata) -> bool:
-        logger.info(f"[local] append illust_ranking {mode} "
+        logger.debug(f"[local] append illust_ranking {mode} "
                     f"({len(content)} items) "
                     f"{metadata}")
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             return await self._append_and_check_illusts(session, IllustRankingCache, IllustRankingCache.mode == mode,
                                                         content=content, metadata=metadata)
 
     # ================ image ================
     async def image(self, illust: Illust, page: int = 0) -> AsyncGenerator[Union[bytes, PixivRepoMetadata], None]:
-        logger.info(f"[local] image {illust.id}")
-        async with self.data_source.start_session() as session:
+        logger.debug(f"[local] image {illust.id}")
+        async with data_source.start_session() as session:
             doc = await DownloadCache.find_one(DownloadCache.illust_id == illust.id,
                                                DownloadCache.page == page,
                                                session=session)
             if doc is not None:
-                _handle_expires_in(doc.metadata, self.conf.pixiv_download_cache_expires_in)
+                _handle_expires_in(doc.metadata, conf.pixiv_download_cache_expires_in)
                 yield doc.metadata
                 yield doc.content
             else:
                 raise NoSuchItemError()
 
     async def update_image(self, illust_id: int, page: int,
                            content: bytes, metadata: PixivRepoMetadata):
-        logger.info(f"[local] update image {illust_id} "
+        logger.debug(f"[local] update image {illust_id} "
                     f"{metadata}")
 
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             await DownloadCache.find_one(
                 DownloadCache.illust_id == illust_id,
                 DownloadCache.page == page,
                 session=session
             ).update(
                 Set({
                     DownloadCache.content: bson.Binary(content),
                     DownloadCache.metadata: metadata
                 }),
                 upsert=True,
                 session=session
             )
 
     async def invalidate_all(self):
-        logger.info(f"[local] invalidate_all")
-        async with self.data_source.start_session() as session:
+        logger.debug(f"[local] invalidate_all")
+        async with data_source.start_session() as session:
             await DownloadCache.delete_all(session=session)
             await IllustDetailCache.delete_all(session=session)
             await UserDetailCache.delete_all(session=session)
             await IllustRankingCache.delete_all(session=session)
             await SearchIllustCache.delete_all(session=session)
             await SearchUserCache.delete_all(session=session)
             await UserIllustsCache.delete_all(session=session)
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/mongo_models.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/mongo_models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from apscheduler.triggers.interval import IntervalTrigger
 from nonebot import logger
 from nonebot_plugin_apscheduler import scheduler as apscheduler
 from sqlalchemy import select, delete, func, text
 from sqlalchemy.ext.asyncio import AsyncSession
 
 from nonebot_plugin_pixivbot.config import Config
-from nonebot_plugin_pixivbot.context import Inject
 from nonebot_plugin_pixivbot.enums import RankingMode
 from nonebot_plugin_pixivbot.global_context import context
 from nonebot_plugin_pixivbot.model import Illust, User
 from nonebot_plugin_pixivbot.utils.lifecycler import on_startup
 from .base import LocalPixivRepo
 from .sql_models import IllustDetailCache, UserDetailCache, DownloadCache, IllustSetCache, IllustSetCacheIllust, \
     UserSetCache, UserSetCacheUser
@@ -36,20 +35,21 @@
     if is_set_cache:
         metadata = PixivRepoMetadata(update_time=update_time, pages=cache.pages, next_qs=cache.next_qs)
     else:
         metadata = PixivRepoMetadata(update_time=update_time)
     return metadata
 
 
-@context.inject
+conf = context.require(Config)
+data_source = context.require(SqlDataSource)
+local_tags = context.require(LocalTagRepo)
+
+
 @context.register_singleton()
 class SqlPixivRepo(LocalPixivRepo):
-    conf: Config = Inject(Config)
-    data_source: SqlDataSource = Inject(SqlDataSource)
-    local_tag_repo: LocalTagRepo = Inject(LocalTagRepo)
 
     def __init__(self):
         on_startup(replay=True)(
             partial(
                 apscheduler.add_job,
                 self.clean_expired,
                 id='pixivbot_sql_pixiv_repo_clean_expired',
@@ -93,22 +93,22 @@
 
                 if illust is not None:
                     yield LazyIllust(illust.illust_id, Illust(**illust.illust))
                 else:
                     yield LazyIllust(cache_illust.illust_id)
                     broken += 1
         finally:
-            logger.info(f"[local] got {total} illusts, illust_detail of {broken} are missed")
+            logger.debug(f"[local] got {total} illusts, illust_detail of {broken} are missed")
 
         yield metadata
 
     async def _invalidate_illusts(self, session: AsyncSession,
                                   cache_type: str,
                                   key: dict):
-        if self.conf.pixiv_sql_dialect == 'sqlite':
+        if conf.pixiv_sql_dialect == 'sqlite':
             await session.execute(text("PRAGMA foreign_keys = ON;"))
 
         stmt = (delete(IllustSetCache)
                 .where(IllustSetCache.cache_type == cache_type,
                        IllustSetCache.key == key))
         await session.execute(stmt)
         await session.commit()
@@ -208,15 +208,15 @@
         li = []
         for x in content:
             if isinstance(x, LazyIllust):
                 if not x.loaded:
                     continue
                 x = x.content
             li.append(x)
-        await self.local_tag_repo.update_from_illusts(li)
+        await local_tags.update_from_illusts(li)
 
         return row_count != len(content)
 
     async def _get_users(self, session: AsyncSession,
                          cache_type: str,
                          key: dict,
                          expired_in: int,
@@ -243,22 +243,22 @@
             async for cache_user, user in await session.stream(stmt):
                 if user is not None:
                     yield User(**user.user)
                 else:
                     yield User(id=cache_user.user_id, name="", account="")
                 total += 1
         finally:
-            logger.info(f"[local] got {total} users")
+            logger.debug(f"[local] got {total} users")
 
         yield metadata
 
     async def _invalidate_users(self, session: AsyncSession,
                                 cache_type: str,
                                 key: dict):
-        if self.conf.pixiv_sql_dialect == 'sqlite':
+        if conf.pixiv_sql_dialect == 'sqlite':
             await session.execute(text("PRAGMA foreign_keys = ON;"))
 
         stmt = (delete(UserSetCache)
                 .where(UserSetCache.cache_type == cache_type,
                        UserSetCache.key == key))
         await session.execute(stmt)
         await session.commit()
@@ -314,103 +314,103 @@
             await session.commit()
 
         return row_count != len(content)
 
     # ================ illust_detail ================
     async def illust_detail(self, illust_id: int) \
             -> AsyncGenerator[Union[Illust, PixivRepoMetadata], None]:
-        logger.info(f"[local] illust_detail {illust_id}")
+        logger.debug(f"[local] illust_detail {illust_id}")
 
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             stmt = select(IllustDetailCache).where(IllustDetailCache.illust_id == illust_id).limit(1)
             cache = (await session.execute(stmt)).scalar_one_or_none()
 
             if cache is not None:
                 metadata = _extract_metadata(cache, False)
-                _handle_expires_in(metadata, self.conf.pixiv_illust_detail_cache_expires_in)
+                _handle_expires_in(metadata, conf.pixiv_illust_detail_cache_expires_in)
 
                 yield metadata
                 yield Illust(**cache.illust)
             else:
                 raise NoSuchItemError()
 
     async def update_illust_detail(self, illust: Illust, metadata: PixivRepoMetadata):
-        logger.info(f"[local] update illust_detail {illust.id} {metadata}")
+        logger.debug(f"[local] update illust_detail {illust.id} {metadata}")
 
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             stmt = (insert(IllustDetailCache)
                     .values(illust_id=illust.id, illust=illust.dict(), update_time=metadata.update_time))
             stmt = stmt.on_conflict_do_update(index_elements=[IllustDetailCache.illust_id],
                                               set_={
                                                   IllustDetailCache.illust: stmt.excluded.illust,
                                                   IllustDetailCache.update_time: stmt.excluded.update_time
                                               })
 
             await session.execute(stmt)
             await session.commit()
 
-            if self.conf.pixiv_tag_translation_enabled:
-                await self.local_tag_repo.update_from_illusts([illust])
+            if conf.pixiv_tag_translation_enabled:
+                await local_tags.update_from_illusts([illust])
 
     # ================ user_detail ================
     async def user_detail(self, user_id: int) \
             -> AsyncGenerator[Union[User, PixivRepoMetadata], None]:
-        logger.info(f"[local] user_detail {user_id}")
+        logger.debug(f"[local] user_detail {user_id}")
 
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             stmt = select(UserDetailCache).where(UserDetailCache.user_id == user_id).limit(1)
             cache = (await session.execute(stmt)).scalar_one_or_none()
 
             if cache is not None:
                 metadata = _extract_metadata(cache, False)
-                _handle_expires_in(metadata, self.conf.pixiv_user_detail_cache_expires_in)
+                _handle_expires_in(metadata, conf.pixiv_user_detail_cache_expires_in)
 
                 yield metadata
                 yield User(**cache.user)
             else:
                 raise NoSuchItemError()
 
     async def update_user_detail(self, user: User, metadata: PixivRepoMetadata):
-        logger.info(f"[local] update user_detail {user.id} {metadata}")
+        logger.debug(f"[local] update user_detail {user.id} {metadata}")
 
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             stmt = (insert(UserDetailCache)
                     .values(user_id=user.id, user=user.dict(), update_time=metadata.update_time))
             stmt = stmt.on_conflict_do_update(index_elements=[UserDetailCache.user_id],
                                               set_={
                                                   UserDetailCache.user: stmt.excluded.user,
                                                   UserDetailCache.update_time: stmt.excluded.update_time
                                               })
 
             await session.execute(stmt)
             await session.commit()
 
     # ================ image ================
     async def image(self, illust: Illust, page: int = 0) -> AsyncGenerator[Union[bytes, PixivRepoMetadata], None]:
-        logger.info(f"[local] image {illust.id}")
+        logger.debug(f"[local] image {illust.id}")
 
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             stmt = select(DownloadCache).where(DownloadCache.illust_id == illust.id,
                                                DownloadCache.page == page).limit(1)
             cache = (await session.execute(stmt)).scalar_one_or_none()
 
             if cache is not None:
                 metadata = _extract_metadata(cache, False)
-                _handle_expires_in(metadata, self.conf.pixiv_download_cache_expires_in)
+                _handle_expires_in(metadata, conf.pixiv_download_cache_expires_in)
 
                 yield metadata
                 yield cache.content
             else:
                 raise NoSuchItemError()
 
     async def update_image(self, illust_id: int, page: int,
                            content: bytes, metadata: PixivRepoMetadata):
-        logger.info(f"[local] update image {illust_id} {metadata}")
+        logger.debug(f"[local] update image {illust_id} {metadata}")
 
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             stmt = (insert(DownloadCache)
                     .values(illust_id=illust_id, page=page, content=content, update_time=metadata.update_time))
             stmt = stmt.on_conflict_do_update(index_elements=[DownloadCache.illust_id, DownloadCache.page],
                                               set_={
                                                   DownloadCache.content: stmt.excluded.content,
                                                   DownloadCache.update_time: stmt.excluded.update_time
                                               })
@@ -420,188 +420,188 @@
 
     # ================ illust_ranking ================
     async def illust_ranking(self, mode: Union[str, RankingMode], *, offset: int = 0) \
             -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
         if isinstance(mode, str):
             mode = RankingMode[mode]
 
-        logger.info(f"[local] illust_ranking {mode}")
+        logger.debug(f"[local] illust_ranking {mode}")
 
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             async for x in self._get_illusts(session, "illust_ranking", {"mode": mode},
-                                             expired_in=self.conf.pixiv_illust_ranking_cache_expires_in, offset=offset):
+                                             expired_in=conf.pixiv_illust_ranking_cache_expires_in, offset=offset):
                 yield x
 
     async def invalidate_illust_ranking(self, mode: RankingMode):
-        logger.info(f"[local] invalidate illust_ranking")
-        async with self.data_source.start_session() as session:
+        logger.debug(f"[local] invalidate illust_ranking")
+        async with data_source.start_session() as session:
             await self._invalidate_illusts(session, "illust_ranking", {"mode": mode})
 
     async def append_illust_ranking(self, mode: RankingMode, content: List[Union[Illust, LazyIllust]],
                                     metadata: PixivRepoMetadata) -> bool:
-        logger.info(f"[local] append illust_ranking {mode} "
+        logger.debug(f"[local] append illust_ranking {mode} "
                     f"({len(content)} items) "
                     f"{metadata}")
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             return await self._append_and_check_illusts(session, "illust_ranking", {"mode": mode},
                                                         content=content, metadata=metadata)
 
     # ================ search_illust ================
     async def search_illust(self, word: str, *, offset: int = 0) \
             -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-        logger.info(f"[local] search_illust {word}")
-        async with self.data_source.start_session() as session:
+        logger.debug(f"[local] search_illust {word}")
+        async with data_source.start_session() as session:
             async for x in self._get_illusts(session, "search_illust", {"word": word},
-                                             expired_in=self.conf.pixiv_search_illust_cache_expires_in, offset=offset):
+                                             expired_in=conf.pixiv_search_illust_cache_expires_in, offset=offset):
                 yield x
 
     async def invalidate_search_illust(self, word: str):
-        logger.info(f"[local] invalidate search_illust {word}")
-        async with self.data_source.start_session() as session:
+        logger.debug(f"[local] invalidate search_illust {word}")
+        async with data_source.start_session() as session:
             await self._invalidate_illusts(session, "search_illust", {"word": word})
 
     async def append_search_illust(self, word: str, content: List[Union[Illust, LazyIllust]],
                                    metadata: PixivRepoMetadata) -> bool:
         # 返回值表示content中是否有已经存在于集合的文档，下同
-        logger.info(f"[local] append search_illust {word} "
+        logger.debug(f"[local] append search_illust {word} "
                     f"({len(content)} items) "
                     f"{metadata}")
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             return await self._append_and_check_illusts(session, "search_illust", {"word": word},
                                                         content=content, metadata=metadata)
 
     # ================ user_illusts ================
     async def user_illusts(self, user_id: int, *, offset: int = 0) \
             -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-        logger.info(f"[local] user_illusts {user_id}")
-        async with self.data_source.start_session() as session:
+        logger.debug(f"[local] user_illusts {user_id}")
+        async with data_source.start_session() as session:
             async for x in self._get_illusts(session, "user_illusts", {"user_id": user_id},
-                                             expired_in=self.conf.pixiv_user_illusts_cache_expires_in, offset=offset):
+                                             expired_in=conf.pixiv_user_illusts_cache_expires_in, offset=offset):
                 yield x
 
     async def invalidate_user_illusts(self, user_id: int):
-        logger.info(f"[local] invalidate user_illusts {user_id}")
-        async with self.data_source.start_session() as session:
+        logger.debug(f"[local] invalidate user_illusts {user_id}")
+        async with data_source.start_session() as session:
             await self._invalidate_illusts(session, "user_illusts", {"user_id": user_id})
 
     async def append_user_illusts(self, user_id: int,
                                   content: List[Union[Illust, LazyIllust]],
                                   metadata: PixivRepoMetadata,
                                   append_at_begin: bool = False) -> bool:
-        logger.info(f"[local] append user_illusts {user_id} "
+        logger.debug(f"[local] append user_illusts {user_id} "
                     f"{'at begin ' if append_at_begin else ''}"
                     f"({len(content)} items) "
                     f"{metadata}")
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             return await self._append_and_check_illusts(session, "user_illusts", {"user_id": user_id},
                                                         content=content, metadata=metadata,
                                                         append_at_begin=append_at_begin)
 
     # ================ user_bookmarks ================
     async def user_bookmarks(self, user_id: int = 0, *, offset: int = 0) \
             -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-        logger.info(f"[local] user_bookmarks {user_id}")
-        async with self.data_source.start_session() as session:
+        logger.debug(f"[local] user_bookmarks {user_id}")
+        async with data_source.start_session() as session:
             async for x in self._get_illusts(session, "user_bookmarks", {"user_id": user_id},
-                                             expired_in=self.conf.pixiv_user_bookmarks_cache_expires_in, offset=offset):
+                                             expired_in=conf.pixiv_user_bookmarks_cache_expires_in, offset=offset):
                 yield x
 
     async def invalidate_user_bookmarks(self, user_id: int):
-        logger.info(f"[local] invalidate user_bookmarks {user_id}")
-        async with self.data_source.start_session() as session:
+        logger.debug(f"[local] invalidate user_bookmarks {user_id}")
+        async with data_source.start_session() as session:
             await self._invalidate_illusts(session, "user_bookmarks", {"user_id": user_id})
 
     async def append_user_bookmarks(self, user_id: int,
                                     content: List[Union[Illust, LazyIllust]],
                                     metadata: PixivRepoMetadata,
                                     append_at_begin: bool = False) -> bool:
-        logger.info(f"[local] append user_bookmarks {user_id} "
+        logger.debug(f"[local] append user_bookmarks {user_id} "
                     f"{'at begin ' if append_at_begin else ''} "
                     f"({len(content)} items) "
                     f"{metadata}")
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             return await self._append_and_check_illusts(session, "user_bookmarks", {"user_id": user_id},
                                                         content=content, metadata=metadata,
                                                         append_at_begin=append_at_begin)
 
     # ================ recommended_illusts ================
     async def recommended_illusts(self, *, offset: int = 0) \
             -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-        logger.info(f"[local] recommended_illusts")
-        async with self.data_source.start_session() as session:
+        logger.debug(f"[local] recommended_illusts")
+        async with data_source.start_session() as session:
             async for x in self._get_illusts(session, "other", {"type": "recommended_illusts"},
-                                             expired_in=self.conf.pixiv_other_cache_expires_in, offset=offset):
+                                             expired_in=conf.pixiv_other_cache_expires_in, offset=offset):
                 yield x
 
     async def invalidate_recommended_illusts(self):
-        logger.info(f"[local] invalidate recommended_illusts")
-        async with self.data_source.start_session() as session:
+        logger.debug(f"[local] invalidate recommended_illusts")
+        async with data_source.start_session() as session:
             await self._invalidate_illusts(session, "other", {"type": "recommended_illusts"})
 
     async def append_recommended_illusts(self, content: List[Union[Illust, LazyIllust]],
                                          metadata: PixivRepoMetadata) -> bool:
-        logger.info(f"[local] append recommended_illusts "
+        logger.debug(f"[local] append recommended_illusts "
                     f"({len(content)} items) "
                     f"{metadata}")
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             return await self._append_and_check_illusts(session, "other", {"type": "recommended_illusts"},
                                                         content=content, metadata=metadata)
 
     # ================ related_illusts ================
     async def related_illusts(self, illust_id: int, *, offset: int = 0) \
             -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-        logger.info(f"[local] related_illusts {illust_id}")
-        async with self.data_source.start_session() as session:
+        logger.debug(f"[local] related_illusts {illust_id}")
+        async with data_source.start_session() as session:
             async for x in self._get_illusts(session, "related_illusts", {"original_illust_id": illust_id},
-                                             expired_in=self.conf.pixiv_related_illusts_cache_expires_in,
+                                             expired_in=conf.pixiv_related_illusts_cache_expires_in,
                                              offset=offset):
                 yield x
 
     async def invalidate_related_illusts(self, illust_id: int):
-        logger.info(f"[local] invalidate related_illusts")
-        async with self.data_source.start_session() as session:
+        logger.debug(f"[local] invalidate related_illusts")
+        async with data_source.start_session() as session:
             await self._invalidate_illusts(session, "related_illusts", {"original_illust_id": illust_id})
 
     async def append_related_illusts(self, illust_id: int, content: List[Union[Illust, LazyIllust]],
                                      metadata: PixivRepoMetadata) -> bool:
-        logger.info(f"[local] append related_illusts {illust_id} "
+        logger.debug(f"[local] append related_illusts {illust_id} "
                     f"({len(content)} items) "
                     f"{metadata}")
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             return await self._append_and_check_illusts(session, "related_illusts", {"original_illust_id": illust_id},
                                                         content=content, metadata=metadata)
 
     # ================ search_user ================
     async def search_user(self, word: str, *, offset: int = 0) \
             -> AsyncGenerator[Union[User, PixivRepoMetadata], None]:
-        logger.info(f"[local] search_user {word}")
-        async with self.data_source.start_session() as session:
+        logger.debug(f"[local] search_user {word}")
+        async with data_source.start_session() as session:
             async for x in self._get_users(session, "search_user", {"word": word},
-                                           expired_in=self.conf.pixiv_search_user_cache_expires_in, offset=offset):
+                                           expired_in=conf.pixiv_search_user_cache_expires_in, offset=offset):
                 yield x
 
     async def invalidate_search_user(self, word: str):
-        logger.info(f"[local] invalidate search_user {word}")
-        async with self.data_source.start_session() as session:
+        logger.debug(f"[local] invalidate search_user {word}")
+        async with data_source.start_session() as session:
             await self._invalidate_users(session, "search_user", {"word": word})
 
     async def append_search_user(self, word: str, content: List[User],
                                  metadata: PixivRepoMetadata) -> bool:
-        logger.info(f"[local] append search_user {word} "
+        logger.debug(f"[local] append search_user {word} "
                     f"({len(content)} items) "
                     f"{metadata}")
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             return await self._append_and_check_users(session, "search_user", {"word": word},
                                                       content=content, metadata=metadata)
 
     async def invalidate_all(self):
-        logger.info(f"[local] invalidate_all")
+        logger.debug(f"[local] invalidate_all")
 
-        async with self.data_source.start_session() as session:
-            if self.conf.pixiv_sql_dialect == 'sqlite':
+        async with data_source.start_session() as session:
+            if conf.pixiv_sql_dialect == 'sqlite':
                 await session.execute(text("PRAGMA foreign_keys = ON;"))
 
             result = await session.execute(delete(IllustSetCache))
             logger.success(f"[local] deleted {result.rowcount} illust_set cache")
             result = await session.execute(delete(UserSetCache))
             logger.success(f"[local] deleted {result.rowcount} user_set cache")
             result = await session.execute(delete(IllustDetailCache))
@@ -609,82 +609,82 @@
             result = await session.execute(delete(UserDetailCache))
             logger.success(f"[local] deleted {result.rowcount} user_detail cache")
             result = await session.execute(delete(DownloadCache))
             logger.success(f"[local] deleted {result.rowcount} download cache")
             await session.commit()
 
     async def clean_expired(self):
-        logger.info(f"[local] clean_expired")
+        logger.debug(f"[local] clean_expired")
 
-        async with self.data_source.start_session() as session:
-            if self.conf.pixiv_sql_dialect == 'sqlite':
+        async with data_source.start_session() as session:
+            if conf.pixiv_sql_dialect == 'sqlite':
                 await session.execute(text("PRAGMA foreign_keys = ON;"))
 
             now = datetime.utcnow()
             stmt = delete(IllustDetailCache).where(
-                IllustDetailCache.update_time <= now - timedelta(seconds=self.conf.pixiv_illust_detail_cache_expires_in)
+                IllustDetailCache.update_time <= now - timedelta(seconds=conf.pixiv_illust_detail_cache_expires_in)
             )
             result = await session.execute(stmt)
             logger.success(f"[local] deleted {result.rowcount} illust_detail cache")
 
             stmt = delete(UserDetailCache).where(
-                UserDetailCache.update_time <= now - timedelta(seconds=self.conf.pixiv_user_detail_cache_expires_in)
+                UserDetailCache.update_time <= now - timedelta(seconds=conf.pixiv_user_detail_cache_expires_in)
             )
             result = await session.execute(stmt)
             logger.success(f"[local] deleted {result.rowcount} user_detail cache")
 
             stmt = delete(DownloadCache).where(
-                DownloadCache.update_time <= now - timedelta(seconds=self.conf.pixiv_download_cache_expires_in)
+                DownloadCache.update_time <= now - timedelta(seconds=conf.pixiv_download_cache_expires_in)
             )
             result = await session.execute(stmt)
             logger.success(f"[local] deleted {result.rowcount} download cache")
 
             stmt = delete(IllustSetCache).where(
                 IllustSetCache.cache_type == 'illust_ranking',
-                IllustSetCache.update_time <= now - timedelta(seconds=self.conf.pixiv_illust_ranking_cache_expires_in)
+                IllustSetCache.update_time <= now - timedelta(seconds=conf.pixiv_illust_ranking_cache_expires_in)
             )
             result = await session.execute(stmt)
             logger.success(f"[local] deleted {result.rowcount} illust_ranking cache")
 
             stmt = delete(IllustSetCache).where(
                 IllustSetCache.cache_type == 'search_illust',
-                IllustSetCache.update_time <= now - timedelta(seconds=self.conf.pixiv_search_illust_cache_delete_in)
+                IllustSetCache.update_time <= now - timedelta(seconds=conf.pixiv_search_illust_cache_delete_in)
             )
             result = await session.execute(stmt)
             logger.success(f"[local] deleted {result.rowcount} search_illust cache")
 
             stmt = delete(UserSetCache).where(
                 UserSetCache.cache_type == 'search_user',
-                UserSetCache.update_time <= now - timedelta(seconds=self.conf.pixiv_search_user_cache_delete_in)
+                UserSetCache.update_time <= now - timedelta(seconds=conf.pixiv_search_user_cache_delete_in)
             )
             result = await session.execute(stmt)
             logger.success(f"[local] deleted {result.rowcount} search_user cache")
 
             stmt = delete(IllustSetCache).where(
                 IllustSetCache.cache_type == 'user_illusts',
-                IllustSetCache.update_time <= now - timedelta(seconds=self.conf.pixiv_user_illusts_cache_delete_in)
+                IllustSetCache.update_time <= now - timedelta(seconds=conf.pixiv_user_illusts_cache_delete_in)
             )
             result = await session.execute(stmt)
             logger.success(f"[local] deleted {result.rowcount} user_illusts cache")
 
             stmt = delete(IllustSetCache).where(
                 IllustSetCache.cache_type == 'user_bookmarks',
-                IllustSetCache.update_time <= now - timedelta(seconds=self.conf.pixiv_user_bookmarks_cache_delete_in)
+                IllustSetCache.update_time <= now - timedelta(seconds=conf.pixiv_user_bookmarks_cache_delete_in)
             )
             result = await session.execute(stmt)
             logger.success(f"[local] deleted {result.rowcount} user_bookmarks cache")
 
             stmt = delete(IllustSetCache).where(
                 IllustSetCache.cache_type == 'related_illusts',
-                IllustSetCache.update_time <= now - timedelta(seconds=self.conf.pixiv_related_illusts_cache_expires_in)
+                IllustSetCache.update_time <= now - timedelta(seconds=conf.pixiv_related_illusts_cache_expires_in)
             )
             result = await session.execute(stmt)
             logger.success(f"[local] deleted {result.rowcount} related_illusts cache")
 
             stmt = delete(IllustSetCache).where(
                 IllustSetCache.cache_type == 'other',
-                IllustSetCache.update_time <= now - timedelta(seconds=self.conf.pixiv_other_cache_expires_in)
+                IllustSetCache.update_time <= now - timedelta(seconds=conf.pixiv_other_cache_expires_in)
             )
             result = await session.execute(stmt)
             logger.success(f"[local] deleted {result.rowcount} other cache")
 
             await session.commit()
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql_models.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql_models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator_repo.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator_repo.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,168 +2,203 @@
 from typing import Any, AsyncGenerator, Union
 
 from frozendict import frozendict
 from nonebot import logger
 from pydantic import BaseModel
 
 from nonebot_plugin_pixivbot.config import Config
-from nonebot_plugin_pixivbot.context import Inject
 from nonebot_plugin_pixivbot.enums import RankingMode
 from nonebot_plugin_pixivbot.global_context import context
 from nonebot_plugin_pixivbot.model import Illust, User, UserPreview
 from nonebot_plugin_pixivbot.utils.shared_agen import SharedAsyncGeneratorManager
 from .base import PixivRepo
 from .enums import PixivResType, CacheStrategy
 from .lazy_illust import LazyIllust
 from .local_repo import LocalPixivRepo
-from .mediator import mediate_single, mediate_many, mediate_append
+from .mediator import SingleMediator, AppendMediator, ManyMediator
 from .models import PixivRepoMetadata
 from .remote_repo import RemotePixivRepo
+from ...utils.format import format_kwargs
+
+conf = context.require(Config)
+local = context.require(LocalPixivRepo)
+remote = context.require(RemotePixivRepo)
 
 
 class SharedAgenIdentifier(BaseModel):
     type: PixivResType
     kwargs: frozendict[str, Any]
 
     def __init__(self, type: PixivResType, **kwargs):
         super().__init__(type=type, kwargs=frozendict(kwargs))
 
     def __str__(self):
-        return f"({self.type.name} {', '.join(map(lambda k: f'{k}={self.kwargs[k]}', {**self.kwargs}))})"
+        return f"({self.type.name} {format_kwargs(**self.kwargs)})"
 
     class Config:
         frozen = True
 
 
-@context.inject
-@context.register_singleton()
 class PixivSharedAsyncGeneratorManager(SharedAsyncGeneratorManager[SharedAgenIdentifier, Any]):
     log_tag = "pixiv_shared_agen"
 
-    conf = Inject(Config)
-    local = Inject(LocalPixivRepo)
-    remote = Inject(RemotePixivRepo)
+    mediators = {
+        "illust_detail": SingleMediator(
+            "illust_detail",
+            cache_factory=lambda kwargs: local.illust_detail(kwargs["illust_id"]),
+            remote_factory=lambda kwargs: remote.illust_detail(**kwargs),
+            cache_updater=lambda kwargs, data, meta: local.update_illust_detail(data, meta)
+        ),
+        "user_detail": SingleMediator(
+            "user_detail",
+            cache_factory=lambda kwargs: local.user_detail(kwargs["user_id"]),
+            remote_factory=lambda kwargs: remote.user_detail(**kwargs),
+            cache_updater=lambda kwargs, data, meta: local.update_user_detail(data, meta)
+        ),
+        "search_illust": AppendMediator(
+            "search_illust",
+            cache_factory=lambda kwargs: local.search_illust(kwargs["word"]),
+            remote_factory=lambda kwargs: remote.search_illust(**kwargs),
+            cache_invalidator=lambda kwargs: local.invalidate_search_illust(kwargs["word"]),
+            cache_appender=lambda kwargs, data, meta: local.append_search_illust(kwargs["word"], data, meta),
+            front_cache_appender=lambda kwargs, data, meta: local.append_search_illust(kwargs["word"], data, meta),
+        ),
+        "search_user": AppendMediator(
+            "search_user",
+            cache_factory=lambda kwargs: local.search_user(kwargs["word"]),
+            remote_factory=lambda kwargs: remote.search_user(**kwargs),
+            cache_invalidator=lambda kwargs: local.invalidate_search_user(kwargs["word"]),
+            cache_appender=lambda kwargs, data, meta: local.append_search_user(kwargs["word"], data, meta),
+            front_cache_appender=lambda kwargs, data, meta: local.append_search_user(kwargs["word"], data, meta),
+        ),
+        "user_illusts": AppendMediator(
+            "user_illusts",
+            cache_factory=lambda kwargs: local.user_illusts(kwargs["user_id"]),
+            remote_factory=lambda kwargs: remote.user_illusts(**kwargs),
+            cache_invalidator=lambda kwargs: local.invalidate_user_illusts(kwargs["user_id"]),
+            cache_appender=lambda kwargs, data, meta: local.append_user_illusts(kwargs["user_id"], data, meta),
+            front_cache_appender=lambda kwargs, data, meta: local.append_user_illusts(kwargs["user_id"], data, meta,
+                                                                                      append_at_begin=True),
+        ),
+        "user_bookmarks": AppendMediator(
+            "user_bookmarks",
+            cache_factory=lambda kwargs: local.user_bookmarks(kwargs["user_id"]),
+            remote_factory=lambda kwargs: remote.user_bookmarks(**kwargs),
+            cache_invalidator=lambda kwargs: local.invalidate_user_bookmarks(kwargs["user_id"]),
+            cache_appender=lambda kwargs, data, meta: local.append_user_bookmarks(kwargs["user_id"], data, meta),
+            front_cache_appender=lambda kwargs, data, meta: local.append_user_bookmarks(kwargs["user_id"], data, meta,
+                                                                                        append_at_begin=True),
+        ),
+        "recommended_illusts": ManyMediator(
+            "recommended_illusts",
+            cache_factory=lambda kwargs: local.recommended_illusts(),
+            remote_factory=lambda kwargs: remote.recommended_illusts(**kwargs),
+            cache_invalidator=lambda kwargs: local.invalidate_recommended_illusts(),
+            cache_appender=lambda kwargs, data, meta: local.append_recommended_illusts(data, meta),
+        ),
+        "related_illusts": ManyMediator(
+            "related_illusts",
+            cache_factory=lambda kwargs: local.related_illusts(kwargs["illust_id"]),
+            remote_factory=lambda kwargs: remote.related_illusts(**kwargs),
+            cache_invalidator=lambda kwargs: local.invalidate_related_illusts(kwargs["illust_id"]),
+            cache_appender=lambda kwargs, data, meta: local.append_related_illusts(kwargs["illust_id"], data, meta),
+        ),
+        "illust_ranking": ManyMediator(
+            "illust_ranking",
+            cache_factory=lambda kwargs: local.illust_ranking(kwargs["mode"]),
+            remote_factory=lambda kwargs: remote.illust_ranking(**kwargs),
+            cache_invalidator=lambda kwargs: local.invalidate_illust_ranking(kwargs["mode"]),
+            cache_appender=lambda kwargs, data, meta: local.append_illust_ranking(kwargs["mode"], data, meta),
+        ),
+        "image": SingleMediator(
+            "image",
+            cache_factory=lambda kwargs: local.image(kwargs["illust"], kwargs["page"]),
+            remote_factory=lambda kwargs: remote.image(**kwargs),
+            cache_updater=lambda kwargs, data, meta: local.update_image(kwargs["illust"].id, kwargs["page"], data, meta)
+        ),
+    }
 
     def illust_detail_factory(self, illust_id: int,
                               cache_strategy: CacheStrategy) -> AsyncGenerator[Illust, None]:
-        return mediate_single(
-            cache_factory=self.local.illust_detail,
-            remote_factory=self.remote.illust_detail,
-            query_kwargs={"illust_id": illust_id},
-            cache_updater=lambda data, metadata: self.local.update_illust_detail(data, metadata),
+        return self.mediators["illust_detail"].mediate(
+            {"illust_id": illust_id},
             force_expiration=cache_strategy == CacheStrategy.FORCE_EXPIRATION,
         )
 
     def user_detail_factory(self, user_id: int,
                             cache_strategy: CacheStrategy) -> AsyncGenerator[User, None]:
-        return mediate_single(
-            cache_factory=self.local.user_detail,
-            remote_factory=self.remote.user_detail,
+        return self.mediators["user_detail"].mediate(
             query_kwargs={"user_id": user_id},
-            cache_updater=lambda data, metadata: self.local.update_user_detail(data, metadata),
             force_expiration=cache_strategy == CacheStrategy.FORCE_EXPIRATION,
         )
 
     def search_illust_factory(self, word: str,
                               cache_strategy: CacheStrategy) -> AsyncGenerator[LazyIllust, None]:
-        return mediate_append(
-            cache_factory=self.local.search_illust,
-            remote_factory=self.remote.search_illust,
+        return self.mediators["search_illust"].mediate(
             query_kwargs={"word": word},
-            cache_appender=lambda data, metadata: self.local.append_search_illust(word, data, metadata),
-            front_cache_appender=lambda data, metadata: self.local.append_search_illust(word, data, metadata),
-            max_item=self.conf.pixiv_random_illust_max_item,
-            max_page=self.conf.pixiv_random_illust_max_page,
+            max_item=conf.pixiv_random_illust_max_item,
+            max_page=conf.pixiv_random_illust_max_page,
             force_expiration=cache_strategy == CacheStrategy.FORCE_EXPIRATION,
         )
 
     def search_user_factory(self, word: str,
                             cache_strategy: CacheStrategy) -> AsyncGenerator[User, None]:
-        return mediate_append(
-            cache_factory=self.local.search_user,
-            remote_factory=self.remote.search_user,
+        return self.mediators["search_user"].mediate(
             query_kwargs={"word": word},
-            cache_appender=lambda data, metadata: self.local.append_search_user(word, data, metadata),
-            front_cache_appender=lambda data, metadata: self.local.append_search_user(word, data, metadata),
             max_page=1,
             force_expiration=cache_strategy == CacheStrategy.FORCE_EXPIRATION,
         )
 
     def user_illusts_factory(self, user_id: int,
                              cache_strategy: CacheStrategy) -> AsyncGenerator[LazyIllust, None]:
-        return mediate_append(
-            cache_factory=self.local.user_illusts,
-            remote_factory=self.remote.user_illusts,
+        return self.mediators["user_illusts"].mediate(
             query_kwargs={"user_id": user_id},
-            cache_appender=lambda data, metadata: self.local.append_user_illusts(user_id, data, metadata),
-            front_cache_appender=lambda data, metadata: self.local.append_user_illusts(user_id, data, metadata,
-                                                                                       append_at_begin=True),
-            max_item=self.conf.pixiv_random_user_illust_max_item,
-            max_page=self.conf.pixiv_random_user_illust_max_page,
+            max_item=conf.pixiv_random_user_illust_max_item,
+            max_page=conf.pixiv_random_user_illust_max_page,
             force_expiration=cache_strategy == CacheStrategy.FORCE_EXPIRATION,
         )
 
     def user_bookmarks_factory(self, user_id: int,
                                cache_strategy: CacheStrategy) -> AsyncGenerator[LazyIllust, None]:
-        return mediate_append(
-            cache_factory=self.local.user_bookmarks,
-            remote_factory=self.remote.user_bookmarks,
+        return self.mediators["user_bookmarks"].mediate(
             query_kwargs={"user_id": user_id},
-            cache_appender=lambda data, metadata: self.local.append_user_bookmarks(user_id, data, metadata),
-            front_cache_appender=lambda data, metadata: self.local.append_user_bookmarks(user_id, data, metadata,
-                                                                                         append_at_begin=True),
-            max_item=self.conf.pixiv_random_bookmark_max_item,
-            max_page=self.conf.pixiv_random_bookmark_max_page,
+            max_item=conf.pixiv_random_bookmark_max_item,
+            max_page=conf.pixiv_random_bookmark_max_page,
             force_expiration=cache_strategy == CacheStrategy.FORCE_EXPIRATION,
         )
 
     def recommended_illusts_factory(self, cache_strategy: CacheStrategy) -> AsyncGenerator[LazyIllust, None]:
-        return mediate_many(
-            cache_factory=self.local.recommended_illusts,
-            remote_factory=self.remote.recommended_illusts,
+        return self.mediators["recommended_illusts"].mediate(
             query_kwargs={},
-            cache_invalidator=self.local.invalidate_recommended_illusts,
-            cache_appender=lambda data, metadata: self.local.append_recommended_illusts(data, metadata),
-            max_item=self.conf.pixiv_random_recommended_illust_max_item,
-            max_page=self.conf.pixiv_random_recommended_illust_max_page,
+            max_item=conf.pixiv_random_recommended_illust_max_item,
+            max_page=conf.pixiv_random_recommended_illust_max_page,
             force_expiration=cache_strategy == CacheStrategy.FORCE_EXPIRATION,
         )
 
     def related_illusts_factory(self, illust_id: int,
                                 cache_strategy: CacheStrategy) -> AsyncGenerator[LazyIllust, None]:
-        return mediate_many(
-            cache_factory=self.local.related_illusts,
-            remote_factory=self.remote.related_illusts,
+        return self.mediators["related_illusts"].mediate(
             query_kwargs={"illust_id": illust_id},
-            cache_invalidator=lambda: self.local.invalidate_related_illusts(illust_id),
-            cache_appender=lambda data, metadata: self.local.append_related_illusts(illust_id, data, metadata),
-            max_item=self.conf.pixiv_random_related_illust_max_item,
-            max_page=self.conf.pixiv_random_related_illust_max_page,
+            max_item=conf.pixiv_random_related_illust_max_item,
+            max_page=conf.pixiv_random_related_illust_max_page,
             force_expiration=cache_strategy == CacheStrategy.FORCE_EXPIRATION,
         )
 
     def illust_ranking_factory(self, mode: RankingMode,
                                cache_strategy: CacheStrategy) -> AsyncGenerator[LazyIllust, None]:
-        return mediate_many(
-            cache_factory=self.local.illust_ranking,
-            remote_factory=self.remote.illust_ranking,
+        return self.mediators["illust_ranking"].mediate(
             query_kwargs={"mode": mode},
-            cache_invalidator=lambda: self.local.invalidate_illust_ranking(mode),
-            cache_appender=lambda data, metadata: self.local.append_illust_ranking(mode, data, metadata),
-            max_item=self.conf.pixiv_ranking_fetch_item,
+            max_item=conf.pixiv_ranking_fetch_item,
             force_expiration=cache_strategy == CacheStrategy.FORCE_EXPIRATION,
         )
 
     def image_factory(self, illust_id: int, illust: Illust, page: int,
                       cache_strategy: CacheStrategy) -> AsyncGenerator[bytes, None]:
-        return mediate_single(
-            cache_factory=self.local.image,
-            remote_factory=self.remote.image,
+        return self.mediators["image"].mediate(
             query_kwargs={"illust": illust, "page": page},
-            cache_updater=lambda data, metadata: self.local.update_image(illust.id, page, data, metadata),
             force_expiration=cache_strategy == CacheStrategy.FORCE_EXPIRATION,
         )
 
     factories = {
         PixivResType.ILLUST_DETAIL: illust_detail_factory,
         PixivResType.USER_DETAIL: user_detail_factory,
         PixivResType.SEARCH_ILLUST: search_illust_factory,
@@ -207,91 +242,89 @@
     async def on_agen_next(self, identifier: SharedAgenIdentifier, item: Any):
         await super().on_agen_next(identifier, item)
         if isinstance(item, PixivRepoMetadata) and not self.get_expires_time(identifier):
             expires_time = self.calc_expires_time(identifier, item.update_time)
             await self.set_expires_time(identifier, expires_time.timestamp())
 
 
-@context.inject
 @context.root.register_singleton()
 class MediatorPixivRepo(PixivRepo):
-    _shared_agen_mgr: PixivSharedAsyncGeneratorManager = Inject(PixivSharedAsyncGeneratorManager)
-    _local: LocalPixivRepo = Inject(LocalPixivRepo)
-    _remote: RemotePixivRepo = Inject(RemotePixivRepo)
+    def __init__(self):
+        self.shared_agen_mgr = PixivSharedAsyncGeneratorManager()
 
     async def invalidate_cache(self):
-        await self._shared_agen_mgr.invalidate_all()
-        await self._local.invalidate_all()
+        await self.shared_agen_mgr.invalidate_all()
+        await local.invalidate_all()
 
     async def illust_detail(self, illust_id: int,
                             cache_strategy: CacheStrategy = CacheStrategy.NORMAL) -> AsyncGenerator[Illust, None]:
-        logger.info(f"[mediator] illust_detail {illust_id} "
-                    f"cache_strategy={cache_strategy.name}")
-        async with self._shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.ILLUST_DETAIL, illust_id=illust_id),
-                                             cache_strategy) as gen:
+        logger.debug(f"[mediator] illust_detail {illust_id} "
+                     f"cache_strategy={cache_strategy.name}")
+        async with self.shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.ILLUST_DETAIL, illust_id=illust_id),
+                                            cache_strategy) as gen:
             data = None
             async for x in gen:
                 if not isinstance(x, PixivRepoMetadata):
                     data = x
 
         # 保证shared_agen能正常结束
         if data is not None:
             yield data
 
     async def user_detail(self, user_id: int,
                           cache_strategy: CacheStrategy = CacheStrategy.NORMAL) -> AsyncGenerator[User, None]:
-        logger.info(f"[mediator] user_detail {user_id} "
-                    f"cache_strategy={cache_strategy.name}")
-        async with self._shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.USER_DETAIL, user_id=user_id),
-                                             cache_strategy) as gen:
+        logger.debug(f"[mediator] user_detail {user_id} "
+                     f"cache_strategy={cache_strategy.name}")
+        async with self.shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.USER_DETAIL, user_id=user_id),
+                                            cache_strategy) as gen:
             data = None
             async for x in gen:
                 if not isinstance(x, PixivRepoMetadata):
                     data = x
 
         # 保证shared_agen能正常结束
         if data is not None:
             yield data
 
     async def search_illust(self, word: str,
                             cache_strategy: CacheStrategy = CacheStrategy.NORMAL) -> AsyncGenerator[LazyIllust, None]:
-        logger.info(f"[mediator] search_illust {word} "
-                    f"cache_strategy={cache_strategy.name}")
-        async with self._shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.SEARCH_ILLUST, word=word),
-                                             cache_strategy) as gen:
+        logger.debug(f"[mediator] search_illust {word} "
+                     f"cache_strategy={cache_strategy.name}")
+        async with self.shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.SEARCH_ILLUST, word=word),
+                                            cache_strategy) as gen:
             async for x in gen:
                 if not isinstance(x, PixivRepoMetadata):
                     yield x
 
     async def search_user(self, word: str,
                           cache_strategy: CacheStrategy = CacheStrategy.NORMAL) -> AsyncGenerator[User, None]:
-        logger.info(f"[mediator] search_user {word} "
-                    f"cache_strategy={cache_strategy.name}")
-        async with self._shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.SEARCH_USER, word=word),
-                                             cache_strategy) as gen:
+        logger.debug(f"[mediator] search_user {word} "
+                     f"cache_strategy={cache_strategy.name}")
+        async with self.shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.SEARCH_USER, word=word),
+                                            cache_strategy) as gen:
             async for x in gen:
                 if not isinstance(x, PixivRepoMetadata):
                     yield x
 
     async def user_bookmarks(self, user_id: int = 0,
                              cache_strategy: CacheStrategy = CacheStrategy.NORMAL) -> AsyncGenerator[LazyIllust, None]:
-        logger.info(f"[mediator] user_bookmarks {user_id} "
-                    f"cache_strategy={cache_strategy.name}")
-        async with self._shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.USER_BOOKMARKS, user_id=user_id),
-                                             cache_strategy) as gen:
+        logger.debug(f"[mediator] user_bookmarks {user_id} "
+                     f"cache_strategy={cache_strategy.name}")
+        async with self.shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.USER_BOOKMARKS, user_id=user_id),
+                                            cache_strategy) as gen:
             async for x in gen:
                 if not isinstance(x, PixivRepoMetadata):
                     yield x
 
     async def user_illusts(self, user_id: int = 0,
                            cache_strategy: CacheStrategy = CacheStrategy.NORMAL) -> AsyncGenerator[LazyIllust, None]:
-        logger.info(f"[mediator] user_illusts {user_id} "
-                    f"cache_strategy={cache_strategy.name}")
-        async with self._shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.USER_ILLUSTS, user_id=user_id),
-                                             cache_strategy) as gen:
+        logger.debug(f"[mediator] user_illusts {user_id} "
+                     f"cache_strategy={cache_strategy.name}")
+        async with self.shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.USER_ILLUSTS, user_id=user_id),
+                                            cache_strategy) as gen:
             async for x in gen:
                 if not isinstance(x, PixivRepoMetadata):
                     yield x
 
     async def _contact_user_illusts_with_preview(self, user_preview: UserPreview,
                                                  cache_strategy: CacheStrategy = CacheStrategy.NORMAL) \
             -> AsyncGenerator[LazyIllust, None]:
@@ -306,22 +339,22 @@
             async for x in gen:
                 if x.id not in ids:
                     yield x
 
     async def user_following_illusts(self, user_id: int,
                                      cache_strategy: CacheStrategy = CacheStrategy.NORMAL) \
             -> AsyncGenerator[LazyIllust, None]:
-        logger.info(f"[mediator] user_following_illusts {user_id} "
-                    f"cache_strategy={cache_strategy.name}")
+        logger.debug(f"[mediator] user_following_illusts {user_id} "
+                     f"cache_strategy={cache_strategy.name}")
 
         n = 0
         gen = []
         peeked = []
 
-        async for user_preview in self._remote.user_following_with_preview(user_id):
+        async for user_preview in remote.user_following_with_preview(user_id):
             if not isinstance(user_preview, PixivRepoMetadata):
                 n += 1
                 gen.append(self._contact_user_illusts_with_preview(user_preview, cache_strategy))
                 peeked.append(None)
 
         try:
             while True:
@@ -343,51 +376,51 @@
                 peeked[select] = None
         except GeneratorExit:
             for gen in gen:
                 await gen.aclose()
 
     async def recommended_illusts(self, cache_strategy: CacheStrategy = CacheStrategy.NORMAL) \
             -> AsyncGenerator[LazyIllust, None]:
-        logger.info(f"[mediator] recommended_illusts "
-                    f"cache_strategy={cache_strategy.name}")
-        async with self._shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.RECOMMENDED_ILLUSTS),
-                                             cache_strategy) as gen:
+        logger.debug(f"[mediator] recommended_illusts "
+                     f"cache_strategy={cache_strategy.name}")
+        async with self.shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.RECOMMENDED_ILLUSTS),
+                                            cache_strategy) as gen:
             async for x in gen:
                 if not isinstance(x, PixivRepoMetadata):
                     yield x
 
     async def related_illusts(self, illust_id: int,
                               cache_strategy: CacheStrategy = CacheStrategy.NORMAL) -> AsyncGenerator[LazyIllust, None]:
-        logger.info(f"[mediator] related_illusts {illust_id} "
-                    f"cache_strategy={cache_strategy.name}")
-        async with self._shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.RELATED_ILLUSTS, illust_id=illust_id),
-                                             cache_strategy) as gen:
+        logger.debug(f"[mediator] related_illusts {illust_id} "
+                     f"cache_strategy={cache_strategy.name}")
+        async with self.shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.RELATED_ILLUSTS, illust_id=illust_id),
+                                            cache_strategy) as gen:
             async for x in gen:
                 if not isinstance(x, PixivRepoMetadata):
                     yield x
 
     async def illust_ranking(self, mode: Union[str, RankingMode],
                              cache_strategy: CacheStrategy = CacheStrategy.NORMAL) -> AsyncGenerator[LazyIllust, None]:
         if isinstance(mode, str):
             mode = RankingMode[mode]
 
-        logger.info(f"[mediator] illust_ranking {mode} "
-                    f"cache_strategy={cache_strategy.name}")
-        async with self._shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.ILLUST_RANKING, mode=mode),
-                                             cache_strategy) as gen:
+        logger.debug(f"[mediator] illust_ranking {mode} "
+                     f"cache_strategy={cache_strategy.name}")
+        async with self.shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.ILLUST_RANKING, mode=mode),
+                                            cache_strategy) as gen:
             async for x in gen:
                 if not isinstance(x, PixivRepoMetadata):
                     yield x
 
     async def image(self, illust: Illust, page: int = 0,
                     cache_strategy: CacheStrategy = CacheStrategy.NORMAL) -> AsyncGenerator[bytes, None]:
-        logger.info(f"[mediator] image {illust.id}[{page}] "
-                    f"cache_strategy={cache_strategy.name}")
-        async with self._shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.IMAGE, illust_id=illust.id, page=page),
-                                             cache_strategy, illust=illust) as gen:
+        logger.debug(f"[mediator] image {illust.id}[{page}] "
+                     f"cache_strategy={cache_strategy.name}")
+        async with self.shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.IMAGE, illust_id=illust.id, page=page),
+                                            cache_strategy, illust=illust) as gen:
             data = None
             async for x in gen:
                 if not isinstance(x, PixivRepoMetadata):
                     data = x
 
         # 保证shared_agen能正常退出
         if data is not None:
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/pixiv_repo/remote_repo.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/remote_repo.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,33 +5,32 @@
 from typing import TypeVar, Optional, Awaitable, List, Callable, Tuple, AsyncGenerator, Union
 
 from nonebot import logger
 from pixivpy_async import *
 from pixivpy_async.error import TokenError
 
 from nonebot_plugin_pixivbot.config import Config
-from nonebot_plugin_pixivbot.context import Inject
 from nonebot_plugin_pixivbot.enums import RankingMode
 from nonebot_plugin_pixivbot.global_context import context
 from nonebot_plugin_pixivbot.model import Illust, User, UserPreview
 from nonebot_plugin_pixivbot.utils.errors import QueryError, RateLimitError
 from nonebot_plugin_pixivbot.utils.lifecycler import on_startup, on_shutdown
 from .base import PixivRepo
 from .compressor import Compressor
 from .lazy_illust import LazyIllust
 from .models import PixivRepoMetadata
 
+_conf = context.require(Config)
+_compressor = context.require(Compressor)
+
 T = TypeVar("T")
 
 
-@context.inject
 @context.register_eager_singleton()
 class RemotePixivRepo(PixivRepo):
-    _conf: Config = Inject(Config)
-    _compressor: Compressor = Inject(Compressor)
 
     # noinspection PyTypeChecker
     def __init__(self):
         self._sema: Semaphore = None
         self._pclient: PixivClient = None
         self._papi: AppPixivAPI = None
         self._refresh_daemon: Task = None
@@ -48,15 +47,15 @@
         USER_AGENT = "PixivAndroidApp/5.0.234 (Android 11; Pixel 5)"
         # REDIRECT_URI = "https://app-api.pixiv.net/web/v1/users/auth/pixiv/callback"
         # LOGIN_URL = "https://app-api.pixiv.net/web/v1/login"
         AUTH_TOKEN_URL = "https://oauth.secure.pixiv.net/auth/token"
         CLIENT_ID = "MOBrBDS8blbauoSck0ZfDbtuzpyT"
         CLIENT_SECRET = "lsACyCD94FhDUtGTXi3QzcFE2uU1hqtDaKeqrdwj"
 
-        refresh_token = self._conf.pixiv_refresh_token
+        refresh_token = _conf.pixiv_refresh_token
 
         data = {
             "client_id": CLIENT_ID,
             "client_secret": CLIENT_SECRET,
             "grant_type": "refresh_token",
             "include_policy": "true",
             "refresh_token": refresh_token,
@@ -93,19 +92,19 @@
             except Exception as e:
                 logger.error(
                     "failed to refresh access token, will retry in 60s.")
                 logger.exception(e)
                 await sleep(60)
 
     def start(self):
-        self._pclient = PixivClient(proxy=self._conf.pixiv_proxy, timeout=self._conf.pixiv_query_timeout)
+        self._pclient = PixivClient(proxy=_conf.pixiv_proxy, timeout=_conf.pixiv_query_timeout)
         self._papi = AppPixivAPI(client=self._pclient.start())
         self._papi.set_additional_headers({'Accept-Language': 'zh-CN'})
         self._refresh_daemon = create_task(self._refresh_daemon_worker())
-        self._sema = Semaphore(self._conf.pixiv_simultaneous_query)
+        self._sema = Semaphore(_conf.pixiv_simultaneous_query)
 
     async def shutdown(self):
         await self._pclient.close()
         self._refresh_daemon.cancel()
 
     def _check_error_in_raw_result(self, raw_result: dict):
         if "error" in raw_result:
@@ -247,15 +246,15 @@
                     if "limit_unknown_360.png" in item.image_urls.large:
                         broken += 1
                         yield LazyIllust(item.id)
                     else:
                         yield LazyIllust(item.id, item)
                 yield metadata
         finally:
-            logger.info(f"[remote] got {total} illusts, illust_detail of {broken} are missed")
+            logger.debug(f"[remote] got {total} illusts, illust_detail of {broken} are missed")
 
     async def _get_user_previews(self, papi_search_func: Callable[[], Awaitable[dict]],
                                  *, block_tags: Optional[List[str]] = None,
                                  **kwargs) \
             -> AsyncGenerator[Union[PixivRepoMetadata, UserPreview], None]:
         yield PixivRepoMetadata(pages=0, next_qs=kwargs)
         async for page, metadata in self._load_many_pages(papi_search_func, "user_previews",
@@ -286,140 +285,140 @@
     async def _raw_illust_detail(self, illust_id: int, **kwargs) -> dict:
         async with self._query():
             raw_result = await self._papi.illust_detail(illust_id, **kwargs)
             self._check_error_in_raw_result(raw_result)
             return raw_result
 
     async def illust_detail(self, illust_id: int, **kwargs) -> AsyncGenerator[Illust, None]:
-        logger.info(f"[remote] illust_detail {illust_id}")
+        logger.debug(f"[remote] illust_detail {illust_id}")
         raw_result = await self._raw_illust_detail(illust_id, **kwargs)
         yield PixivRepoMetadata()
         yield Illust.parse_obj(raw_result["illust"])
 
     async def _raw_user_detail(self, user_id: int, **kwargs) -> dict:
         async with self._query():
             raw_result = await self._papi.user_detail(user_id, **kwargs)
             self._check_error_in_raw_result(raw_result)
             return raw_result
 
     async def user_detail(self, user_id: int, **kwargs) -> AsyncGenerator[User, None]:
-        logger.info(f"[remote] user_detail {user_id}")
+        logger.debug(f"[remote] user_detail {user_id}")
         raw_result = await self._raw_user_detail(user_id, **kwargs)
         yield PixivRepoMetadata()
         yield User.parse_obj(raw_result["user"])
 
     def search_illust(self, word: str, **kwargs) \
             -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-        logger.info(f"[remote] search_illust {word}")
+        logger.debug(f"[remote] search_illust {word}")
         return self._get_illusts(self._papi.search_illust,
-                                 block_tags=self._conf.pixiv_block_tags,
-                                 min_bookmark=self._conf.pixiv_random_illust_min_bookmark,
-                                 min_view=self._conf.pixiv_random_illust_min_view,
+                                 block_tags=_conf.pixiv_block_tags,
+                                 min_bookmark=_conf.pixiv_random_illust_min_bookmark,
+                                 min_view=_conf.pixiv_random_illust_min_view,
                                  word=word, **kwargs)
 
     def search_user(self, word: str, **kwargs) \
             -> AsyncGenerator[Union[User, PixivRepoMetadata], None]:
-        logger.info(f"[remote] search_user {word}")
+        logger.debug(f"[remote] search_user {word}")
         return self._get_users(self._papi.search_user,
                                word=word, **kwargs)
 
     def search_user_with_preview(self, word: str, **kwargs) \
             -> AsyncGenerator[Union[UserPreview, PixivRepoMetadata], None]:
-        logger.info(f"[remote] search_user {word}")
+        logger.debug(f"[remote] search_user {word}")
         return self._get_user_previews(self._papi.search_user,
-                                       block_tags=self._conf.pixiv_block_tags,
+                                       block_tags=_conf.pixiv_block_tags,
                                        word=word, **kwargs)
 
     def user_following(self, user_id: int, **kwargs) \
             -> AsyncGenerator[Union[User, PixivRepoMetadata], None]:
-        logger.info(f"[remote] following_users {user_id}")
+        logger.debug(f"[remote] following_users {user_id}")
         return self._get_users(self._papi.user_following,
                                user_id=user_id, **kwargs)
 
     def user_following_with_preview(self, user_id: int, **kwargs) \
             -> AsyncGenerator[Union[UserPreview, PixivRepoMetadata], None]:
-        logger.info(f"[remote] following_users {user_id}")
+        logger.debug(f"[remote] following_users {user_id}")
         return self._get_user_previews(self._papi.user_following,
-                                       block_tags=self._conf.pixiv_block_tags,
+                                       block_tags=_conf.pixiv_block_tags,
                                        user_id=user_id, **kwargs)
 
     def user_illusts(self, user_id: int, **kwargs) \
             -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-        logger.info(f"[remote] user_illusts {user_id}")
+        logger.debug(f"[remote] user_illusts {user_id}")
         return self._get_illusts(self._papi.user_illusts,
-                                 block_tags=self._conf.pixiv_block_tags,
-                                 min_bookmark=self._conf.pixiv_random_user_illust_min_bookmark,
-                                 min_view=self._conf.pixiv_random_user_illust_min_view,
+                                 block_tags=_conf.pixiv_block_tags,
+                                 min_bookmark=_conf.pixiv_random_user_illust_min_bookmark,
+                                 min_view=_conf.pixiv_random_user_illust_min_view,
                                  user_id=user_id, **kwargs)
 
     def user_bookmarks(self, user_id: int = 0, **kwargs) \
             -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
         if user_id == 0:
             user_id = self.user_id
 
-        logger.info(f"[remote] user_bookmarks {user_id}")
+        logger.debug(f"[remote] user_bookmarks {user_id}")
         return self._get_illusts(self._papi.user_bookmarks_illust,
-                                 block_tags=self._conf.pixiv_block_tags,
-                                 min_bookmark=self._conf.pixiv_random_bookmark_min_bookmark,
-                                 min_view=self._conf.pixiv_random_bookmark_min_view,
+                                 block_tags=_conf.pixiv_block_tags,
+                                 min_bookmark=_conf.pixiv_random_bookmark_min_bookmark,
+                                 min_view=_conf.pixiv_random_bookmark_min_view,
                                  user_id=user_id, **kwargs)
 
     # def following_illusts(self, **kwargs) \
     #         -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
     #     logger.debug(f"[remote] following_illusts")
     #     return self._get_illusts(self._papi.illust_follow,
-    #                              block_tags=self._conf.pixiv_block_tags,
-    #                              min_bookmark=self._conf.pixiv_random_following_illust_min_bookmark,
-    #                              min_view=self._conf.pixiv_random_following_illust_min_view,
+    #                              block_tags=_conf.pixiv_block_tags,
+    #                              min_bookmark=_conf.pixiv_random_following_illust_min_bookmark,
+    #                              min_view=_conf.pixiv_random_following_illust_min_view,
     #                              **kwargs)
 
     def recommended_illusts(self, **kwargs) \
             -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-        logger.info(f"[remote] recommended_illusts")
+        logger.debug(f"[remote] recommended_illusts")
         return self._get_illusts(self._papi.illust_recommended,
-                                 block_tags=self._conf.pixiv_block_tags,
-                                 min_bookmark=self._conf.pixiv_random_recommended_illust_min_bookmark,
-                                 min_view=self._conf.pixiv_random_recommended_illust_min_view,
+                                 block_tags=_conf.pixiv_block_tags,
+                                 min_bookmark=_conf.pixiv_random_recommended_illust_min_bookmark,
+                                 min_view=_conf.pixiv_random_recommended_illust_min_view,
                                  **kwargs)
 
     def related_illusts(self, illust_id: int, **kwargs) \
             -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-        logger.info(f"[remote] related_illusts {illust_id}")
+        logger.debug(f"[remote] related_illusts {illust_id}")
         return self._get_illusts(self._papi.illust_related,
-                                 block_tags=self._conf.pixiv_block_tags,
-                                 min_bookmark=self._conf.pixiv_random_related_illust_min_bookmark,
-                                 min_view=self._conf.pixiv_random_related_illust_min_view,
+                                 block_tags=_conf.pixiv_block_tags,
+                                 min_bookmark=_conf.pixiv_random_related_illust_min_bookmark,
+                                 min_view=_conf.pixiv_random_related_illust_min_view,
                                  illust_id=illust_id, **kwargs)
 
     def illust_ranking(self, mode: Union[str, RankingMode], **kwargs) \
             -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
         if isinstance(mode, str):
             mode = RankingMode[mode]
 
-        logger.info(f"[remote] illust_ranking {mode}")
+        logger.debug(f"[remote] illust_ranking {mode}")
         return self._get_illusts(self._papi.illust_ranking,
-                                 block_tags=self._conf.pixiv_block_tags,
+                                 block_tags=_conf.pixiv_block_tags,
                                  mode=mode.name, **kwargs)
 
     async def _raw_image(self, illust: Illust, page: int, **kwargs) -> bytes:
-        custom_domain = self._conf.pixiv_download_custom_domain
+        custom_domain = _conf.pixiv_download_custom_domain
 
         url = illust.page_image_url(page)
         if custom_domain is not None:
             url = url.replace("i.pximg.net", custom_domain)
 
         async with self._query():
             with BytesIO() as bio:
                 await self._papi.download(url, fname=bio, **kwargs)
                 content = bio.getvalue()
                 return content
 
     async def image(self, illust: Illust, page: int = 0, **kwargs) \
             -> AsyncGenerator[Union[bytes, PixivRepoMetadata], None]:
-        logger.info(f"[remote] image {illust.id}")
+        logger.debug(f"[remote] image {illust.id}")
         content = await self._raw_image(illust, page, **kwargs)
-        content = await self._compressor.compress(content)
+        content = await _compressor.compress(content)
         yield PixivRepoMetadata()
         yield content
 
 
 __all__ = ("RemotePixivRepo",)
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/source/lifecycle_mixin.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/lifecycle_mixin.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/source/migration_manager.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/migration_manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/source/mongo/__init__.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/mongo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,25 +7,24 @@
 from motor.motor_asyncio import AsyncIOMotorClient, AsyncIOMotorDatabase
 from nonebot import logger
 from pydantic.main import ModelMetaclass
 from pymongo import IndexModel
 from pymongo.errors import OperationFailure
 
 from nonebot_plugin_pixivbot.config import Config
-from nonebot_plugin_pixivbot.context import Inject
 from nonebot_plugin_pixivbot.data.errors import DataSourceNotReadyError
 from nonebot_plugin_pixivbot.enums import DataSourceType
 from nonebot_plugin_pixivbot.global_context import context
 from nonebot_plugin_pixivbot.utils.lifecycler import on_shutdown, on_startup
 from ..lifecycle_mixin import DataSourceLifecycleMixin
 
+conf = context.require(Config)
+
 
-@context.inject
 class MongoDataSource(DataSourceLifecycleMixin):
-    conf = Inject(Config)
     app_db_version = 7
 
     document_models: List[Type[Document]] = []
 
     def __init__(self):
         super().__init__()
 
@@ -85,17 +84,19 @@
                 f"Index in {coll_name}: expireAfterSeconds changed to {index.document['expireAfterSeconds']}")
 
     async def initialize(self):
         from .migration import MongoMigrationManager
 
         await self._fire_initializing()
 
-        client = AsyncIOMotorClient(self.conf.pixiv_mongo_conn_url)
+        logger.info("[data source] mongo conn url: " + conf.pixiv_mongo_conn_url)
+
+        client = AsyncIOMotorClient(conf.pixiv_mongo_conn_url)
         options = CodecOptions(tz_aware=True)
-        db = client[self.conf.pixiv_mongo_database_name].with_options(options)
+        db = client[conf.pixiv_mongo_database_name].with_options(options)
 
         # migrate
         mig_mgr = MongoMigrationManager(lambda prev, cur: self._raw_set_db_version(db, cur))
         db_version = await self._raw_get_db_version(db)
         await mig_mgr.perform_migration(db, db_version, self.app_db_version)
 
         # ensure ttl indexes (before init beanie)
@@ -151,12 +152,11 @@
         return cls
 
 
 class MongoDocument(Document, metaclass=MongoDocumentMeta):
     pass
 
 
-conf = context.require(Config)
 if conf.pixiv_data_source == DataSourceType.mongo:
     context.register_eager_singleton()(MongoDataSource)
 
 __all__ = ("MongoDataSource", "MongoDocument")
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/source/mongo/migration/__init__.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/mongo/migration/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v1_to_v2.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v1_to_v2.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v2_to_v3.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v2_to_v3.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v3_to_v4.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v3_to_v4.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v4_to_v5.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v4_to_v5.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v5_to_v6.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v5_to_v6.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/source/sql/__init__.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/sql/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,37 +6,35 @@
 from nonebot import get_driver, logger
 from sqlalchemy import select, inspect
 from sqlalchemy.ext.asyncio import create_async_engine, AsyncSession, AsyncEngine
 from sqlalchemy.orm import registry, sessionmaker
 from sqlalchemy.pool import StaticPool
 
 from nonebot_plugin_pixivbot.config import Config
-from nonebot_plugin_pixivbot.context import Inject
 from nonebot_plugin_pixivbot.enums import DataSourceType
 from nonebot_plugin_pixivbot.global_context import context
 from nonebot_plugin_pixivbot.utils.lifecycler import on_startup, on_shutdown
 from ..lifecycle_mixin import DataSourceLifecycleMixin
 from ...errors import DataSourceNotReadyError
 
+conf = context.require(Config)
+
 
 def default_dumps(obj):
     if isinstance(obj, (datetime, date)):
         return obj.isoformat()
 
     return None
 
 
 def json_serializer(obj):
     return json.dumps(obj, default=default_dumps)
 
 
-@context.inject
 class SqlDataSource(DataSourceLifecycleMixin):
-    conf: Config = Inject(Config)
-
     app_db_version = 4
     registry = registry()
 
     def __init__(self):
         super().__init__()
 
         self._engine = None
@@ -93,21 +91,22 @@
         params = {
             # 仅当TRACE模式时回显sql语句
             'echo': driver.config.log_level == 'TRACE',
             'future': True,
             'json_serializer': json_serializer
         }
 
-        if self.conf.detect_sql_dialect == 'sqlite':
+        if conf.detect_sql_dialect == 'sqlite':
             # 使用 SQLite 数据库时，如果在写入时遇到 (sqlite3.OperationalError) database is locked 错误。
             # 可尝试将 poolclass 设置为 StaticPool，保持有且仅有一个连接。
             # 不过这样设置之后，在程序运行期间，你的数据库文件都将被占用。
             params['poolclass'] = StaticPool
 
-        self._engine = create_async_engine(self.conf.pixiv_sql_conn_url, **params)
+        logger.info("[data source] sql conn url: " + conf.pixiv_sql_conn_url)
+        self._engine = create_async_engine(conf.pixiv_sql_conn_url, **params)
 
         async with self._engine.begin() as conn:
             from .migration import SqlMigrationManager
             from .meta_info import MetaInfo
 
             await conn.run_sync(lambda conn: MetaInfo.__table__.create(conn, checkfirst=True))
 
@@ -146,12 +145,11 @@
     @property
     def engine(self) -> AsyncEngine:
         if self._engine is None:
             raise DataSourceNotReadyError()
         return self._engine
 
 
-conf = context.require(Config)
 if conf.pixiv_data_source == DataSourceType.sql:
     context.register_eager_singleton()(SqlDataSource)
 
 __all__ = ("SqlDataSource",)
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v1_to_v2.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v1_to_v2.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v2_to_v3.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v2_to_v3.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/subscription/mongo.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/subscription/mongo.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,90 +1,92 @@
 from typing import Optional, Any, AsyncGenerator, Collection
 
 from pymongo import IndexModel, DeleteOne
 
-from nonebot_plugin_pixivbot.context import Inject
 from nonebot_plugin_pixivbot.global_context import context
 from nonebot_plugin_pixivbot.model import Subscription, PostIdentifier, T_UID, T_GID, UserIdentifier
+from .base import SubscriptionRepo
 from ..interval_task_repo import process_subscriber
 from ..source.mongo import MongoDataSource, MongoDocument
 from ..utils.shortuuid import gen_code
 
 
 class SubscriptionDocument(Subscription[Any, Any], MongoDocument):
     class Settings:
         name = "subscription"
         indexes = [
             IndexModel([("bot", 1), ("subscriber", 1), ("code", 1)], unique=True)
         ]
 
 
-@context.inject
+data_source = context.require(MongoDataSource)
+
+
 @context.register_singleton()
-class MongoSubscriptionRepo:
-    data_source: MongoDataSource = Inject(MongoDataSource)
+class MongoSubscriptionRepo(SubscriptionRepo):
 
     async def get_by_subscriber(self, bot: UserIdentifier[T_UID],
-                                subscriber: PostIdentifier[T_UID, T_GID]) -> AsyncGenerator[
-        Subscription[T_UID, T_GID], None]:
+                                subscriber: PostIdentifier[T_UID, T_GID]) \
+            -> AsyncGenerator[Subscription[T_UID, T_GID], None]:
         subscriber = process_subscriber(subscriber)
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             async for doc in SubscriptionDocument.find(
                     SubscriptionDocument.bot == bot,
                     SubscriptionDocument.subscriber == subscriber,
                     session=session):
                 yield doc
 
-    async def get_by_bot(self, bot: UserIdentifier[T_UID]) -> AsyncGenerator[Subscription[T_UID, T_GID], None]:
-        async with self.data_source.start_session() as session:
+    async def get_by_bot(self, bot: UserIdentifier[T_UID]) \
+            -> AsyncGenerator[Subscription[T_UID, T_GID], None]:
+        async with data_source.start_session() as session:
             async for doc in SubscriptionDocument.find(SubscriptionDocument.bot == bot,
                                                        session=session):
                 yield doc
 
     async def get_by_code(self, bot: UserIdentifier[T_UID],
                           subscriber: PostIdentifier[T_UID, T_GID],
                           code: str) -> Optional[Subscription[T_UID, T_GID]]:
         subscriber = process_subscriber(subscriber)
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             return await SubscriptionDocument.find_one(
                 SubscriptionDocument.bot == bot,
                 SubscriptionDocument.subscriber == subscriber,
                 SubscriptionDocument.code == code,
                 session=session)
 
     async def insert(self, item: Subscription[T_UID, T_GID]) -> bool:
         item.subscriber = process_subscriber(item.subscriber)
         item.code = gen_code()
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             await SubscriptionDocument.insert_one(SubscriptionDocument(**item.dict()), session=session)
         return True
 
     async def delete_one(self, bot: UserIdentifier[T_UID],
                          subscriber: PostIdentifier[T_UID, T_GID],
                          code: str) -> Optional[Subscription[T_UID, T_GID]]:
         # beanie不支持原子性的find_one_and_delete操作
         subscriber = process_subscriber(subscriber)
         query = {
             "bot": bot.dict(),
             "code": code,
             "subscriber": process_subscriber(subscriber).dict()
         }
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             result = await SubscriptionDocument.get_motor_collection().find_one_and_delete(query, session=session)
             if result:
                 return Subscription.parse_obj(result)
             else:
                 return None
 
     async def delete_many_by_subscriber(self, bot: UserIdentifier[T_UID],
                                         subscriber: PostIdentifier[T_UID, T_GID]) \
             -> Collection[Subscription[T_UID, T_GID]]:
         subscriber = process_subscriber(subscriber)
 
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             old_doc = await SubscriptionDocument.find(
                 SubscriptionDocument.bot == bot,
                 SubscriptionDocument.subscriber == subscriber,
                 session=session
             ).to_list()
 
             # BulkWriter存在bug，session不生效
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/subscription/sql.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/subscription/sql.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Optional, AsyncIterable, Collection
 
 import tzlocal
 from sqlalchemy import select, UniqueConstraint
 from sqlalchemy.orm import mapped_column, Mapped
 
-from nonebot_plugin_pixivbot.context import Inject
 from nonebot_plugin_pixivbot.global_context import context
 from nonebot_plugin_pixivbot.model import Subscription, PostIdentifier, ScheduleType, T_UID, T_GID, UserIdentifier
+from .base import SubscriptionRepo
 from ..interval_task_repo import process_subscriber
 from ..source.sql import SqlDataSource
 from ..utils.shortuuid import gen_code
 from ..utils.sql import insert, JSON
 
 
 @SqlDataSource.registry.mapped
@@ -38,45 +38,46 @@
                         type=item.type,
                         kwargs=item.kwargs,
                         bot=UserIdentifier(adapter, bot_id),
                         schedule=item.schedule,
                         tz=item.tz)
 
 
-@context.inject
+data_source = context.require(SqlDataSource)
+
+
 @context.register_singleton()
-class SqlSubscriptionRepo:
-    data_source: SqlDataSource = Inject(SqlDataSource)
+class SqlSubscriptionRepo(SubscriptionRepo):
 
     async def get_by_subscriber(self, bot: UserIdentifier[T_UID],
                                 subscriber: PostIdentifier[T_UID, T_GID]) -> AsyncIterable[Subscription]:
         subscriber = process_subscriber(subscriber)
 
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             stmt = (
                 select(SubscriptionOrm)
                 .where(SubscriptionOrm.bot == str(bot),
                        SubscriptionOrm.subscriber == subscriber.dict())
             )
             async for x in await session.stream_scalars(stmt):
                 yield _to_model(x)
 
     async def get_by_bot(self, bot: UserIdentifier[T_UID]) -> AsyncIterable[Subscription]:
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             stmt = (
                 select(SubscriptionOrm)
                 .where(SubscriptionOrm.bot == str(bot))
             )
             async for x in await session.stream_scalars(stmt):
                 yield _to_model(x)
 
     async def get_by_code(self, bot: UserIdentifier[T_UID],
                           subscriber: PostIdentifier[T_UID, T_GID],
                           code: str) -> Optional[Subscription]:
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             stmt = (
                 select(SubscriptionOrm)
                 .where(SubscriptionOrm.bot == str(bot),
                        SubscriptionOrm.subscriber == subscriber.dict(),
                        SubscriptionOrm.code == code)
             )
             x = (await session.execute(stmt)).scalar_one_or_none()
@@ -85,15 +86,15 @@
             else:
                 return None
 
     async def insert(self, item: Subscription[T_UID, T_GID]) -> bool:
         item.subscriber = process_subscriber(item.subscriber)
         item.code = gen_code()
 
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             stmt = (insert(SubscriptionOrm)
                     .values(subscriber=item.subscriber.dict(),
                             code=item.code,
                             type=item.type,
                             kwargs=item.kwargs,
                             bot=str(item.bot),
                             schedule=item.schedule,
@@ -103,15 +104,15 @@
         return True
 
     async def delete_one(self, bot: UserIdentifier[T_UID],
                          subscriber: PostIdentifier[T_UID, T_GID],
                          code: int) -> Optional[Subscription]:
         subscriber = process_subscriber(subscriber)
 
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             stmt = (select(SubscriptionOrm)
                     .where(SubscriptionOrm.bot == str(bot),
                            SubscriptionOrm.subscriber == subscriber.dict(),
                            SubscriptionOrm.code == code)
                     .limit(1))
             sub = (await session.execute(stmt)).scalar_one_or_none()
 
@@ -122,15 +123,15 @@
             await session.commit()
             return _to_model(sub)
 
     async def delete_many_by_subscriber(self, bot: UserIdentifier[T_UID],
                                         subscriber: PostIdentifier[T_UID, T_GID]) -> Collection[Subscription]:
         subscriber = process_subscriber(subscriber)
 
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             stmt = (select(SubscriptionOrm)
                     .where(SubscriptionOrm.bot == str(bot),
                            SubscriptionOrm.subscriber == subscriber.dict()))
             subs = (await session.execute(stmt)).scalars().all()
 
             for t in subs:
                 await session.delete(t)
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/utils/sql/__init__.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/utils/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/utils/sql/utc_datetime.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/utils/sql/utc_datetime.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/utils/sql.pyi` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/utils/sql.pyi`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/watch_task/__init__.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/watch_task/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,11 @@
 from nonebot_plugin_pixivbot.config import Config
 from nonebot_plugin_pixivbot.enums import DataSourceType
 from nonebot_plugin_pixivbot.global_context import context
-from nonebot_plugin_pixivbot.model import WatchTask
-from ..interval_task_repo import IntervalTaskRepo
-
-
-class WatchTaskRepo(IntervalTaskRepo[WatchTask]):
-    async def update(self, item: WatchTask) -> bool:
-        ...
-
+from .base import WatchTaskRepo
 
 conf = context.require(Config)
 if conf.pixiv_data_source == DataSourceType.mongo:
     from .mongo import MongoWatchTaskRepo
 
     context.bind(WatchTaskRepo, MongoWatchTaskRepo)
 else:
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/watch_task/mongo.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/watch_task/mongo.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,75 +1,76 @@
 from typing import AsyncGenerator, Optional, Any, Collection
 
 from pymongo import IndexModel, DeleteOne
 from pymongo.errors import DuplicateKeyError
 
-from nonebot_plugin_pixivbot.context import Inject
 from nonebot_plugin_pixivbot.global_context import context
 from nonebot_plugin_pixivbot.model import WatchTask, PostIdentifier, T_UID, T_GID, UserIdentifier
+from . import WatchTaskRepo
 from ..interval_task_repo import process_subscriber
 from ..source.mongo import MongoDataSource, MongoDocument
 from ..utils.shortuuid import gen_code
 
 
 class WatchTaskDocument(WatchTask[Any, Any], MongoDocument):
     class Settings:
         name = "watch_task"
         indexes = [
             IndexModel([("bot", 1), ("subscriber", 1), ("code", 1)], unique=True),
             IndexModel([("bot", 1), ("subscriber", 1), ("type", 1), ("kwargs", 1)], unique=True)
         ]
 
 
-@context.inject
+data_source = context.require(MongoDataSource)
+
+
 @context.register_singleton()
-class MongoWatchTaskRepo:
-    data_source = Inject(MongoDataSource)
+class MongoWatchTaskRepo(WatchTaskRepo):
 
     async def get_by_subscriber(self, bot: UserIdentifier[T_UID],
                                 subscriber: PostIdentifier[T_UID, T_GID]) -> AsyncGenerator[WatchTask, None]:
         subscriber = process_subscriber(subscriber)
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             async for doc in WatchTaskDocument.find(
                     WatchTaskDocument.bot == bot,
                     WatchTaskDocument.subscriber == subscriber,
                     session=session):
                 yield doc
 
     async def get_by_bot(self, bot: UserIdentifier[T_UID]) -> AsyncGenerator[WatchTask, None]:
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             async for doc in WatchTaskDocument.find(WatchTaskDocument.bot == bot,
                                                     session=session):
                 yield doc
 
     async def get_by_code(self, bot: UserIdentifier[T_UID],
                           subscriber: PostIdentifier[T_UID, T_GID],
                           code: int) -> Optional[WatchTask]:
         subscriber = process_subscriber(subscriber)
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             return await WatchTaskDocument.find_one(
                 WatchTaskDocument.bot == bot,
                 WatchTaskDocument.subscriber == subscriber,
                 WatchTaskDocument.code == code,
                 session=session)
 
     async def insert(self, item: WatchTask) -> bool:
         try:
-            async with self.data_source.start_session() as session:
+            async with data_source.start_session() as session:
                 item.subscriber = process_subscriber(item.subscriber)
                 item.code = gen_code()
                 doc = WatchTaskDocument(**item.dict())
                 await doc.save(session=session)
 
                 return True
         except DuplicateKeyError:
             return False
 
     async def update(self, item: WatchTask) -> bool:
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             if isinstance(item, WatchTaskDocument):
                 await item.save()
             else:
                 item.subscriber = process_subscriber(item.subscriber)
                 await WatchTaskDocument.find_one(
                     WatchTaskDocument.subscriber == item.subscriber,
                     WatchTaskDocument.code == item.code,
@@ -77,15 +78,15 @@
                 ).update(**item.dict(exclude={"subscriber", "code"}),
                          session=session)
             return True
 
     async def delete_one(self, bot: UserIdentifier[T_UID],
                          subscriber: PostIdentifier[T_UID, T_GID],
                          code: int) -> Optional[WatchTask]:
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             # beanie不支持原子性的find_one_and_delete操作
             subscriber = process_subscriber(subscriber)
             query = {
                 "bot": bot.dict(),
                 "code": code,
                 "subscriber": process_subscriber(subscriber).dict()
             }
@@ -93,15 +94,15 @@
             if result:
                 return WatchTask.parse_obj(result)
             else:
                 return None
 
     async def delete_many_by_subscriber(self, bot: UserIdentifier[T_UID],
                                         subscriber: PostIdentifier[T_UID, T_GID]) -> Collection[WatchTask]:
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             subscriber = process_subscriber(subscriber)
 
             old_doc = await WatchTaskDocument.find(
                 WatchTaskDocument.bot == bot,
                 WatchTaskDocument.subscriber == subscriber,
                 session=session
             ).to_list()
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/data/watch_task/sql.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/watch_task/sql.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from datetime import datetime
 from typing import Optional, AsyncIterable, Collection
 
 from pytz import utc
 from sqlalchemy import select, UniqueConstraint, update
 from sqlalchemy.orm import mapped_column, Mapped
 
-from nonebot_plugin_pixivbot.context import Inject
 from nonebot_plugin_pixivbot.global_context import context
 from nonebot_plugin_pixivbot.model import PostIdentifier, WatchType, WatchTask, T_UID, T_GID, UserIdentifier
+from .base import WatchTaskRepo
 from ..interval_task_repo import process_subscriber
 from ..source.sql import SqlDataSource
 from ..utils.shortuuid import gen_code
 from ..utils.sql import insert, JSON, UTCDateTime
 
 
 @SqlDataSource.registry.mapped
@@ -38,62 +38,63 @@
                      code=item.code,
                      type=item.type,
                      kwargs=item.kwargs,
                      bot=UserIdentifier(adapter, bot_id),
                      checkpoint=item.checkpoint)
 
 
-@context.inject
+data_source = context.require(SqlDataSource)
+
+
 @context.register_singleton()
-class SqlWatchTaskRepo:
-    data_source: SqlDataSource = Inject(SqlDataSource)
+class SqlWatchTaskRepo(WatchTaskRepo):
 
     async def get_by_subscriber(self, bot: UserIdentifier[T_UID],
                                 subscriber: PostIdentifier[T_UID, T_GID]) -> AsyncIterable[WatchTask[T_UID, T_GID]]:
         subscriber = process_subscriber(subscriber)
 
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             stmt = (
                 select(WatchTaskOrm)
                 .where(WatchTaskOrm.bot == str(bot),
                        WatchTaskOrm.subscriber == subscriber.dict())
             )
             async for x in await session.stream_scalars(stmt):
                 x.checkpoint = x.checkpoint.replace(tzinfo=utc)
                 yield _to_model(x)
 
     async def get_by_bot(self, bot: UserIdentifier[T_UID]) -> AsyncIterable[WatchTask[T_UID, T_GID]]:
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             stmt = (
                 select(WatchTaskOrm)
                 .where(WatchTaskOrm.bot == str(bot))
             )
             async for x in await session.stream_scalars(stmt):
                 x.checkpoint = x.checkpoint.replace(tzinfo=utc)
                 yield _to_model(x)
 
     async def get_by_code(self, bot: UserIdentifier[T_UID],
                           subscriber: PostIdentifier[T_UID, T_GID],
                           code: int) -> Optional[WatchTask[T_UID, T_GID]]:
         subscriber = process_subscriber(subscriber)
 
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             stmt = (select(WatchTaskOrm)
                     .where(WatchTaskOrm.bot == str(bot),
                            WatchTaskOrm.subscriber == subscriber.dict(),
                            WatchTaskOrm.code == code))
             result = (await session.execute(stmt)).scalar_one_or_none()
             result.checkpoint = result.checkpoint.replace(tzinfo=utc)
             return _to_model(result)
 
     async def insert(self, item: WatchTask[T_UID, T_GID]) -> bool:
         item.subscriber = process_subscriber(item.subscriber)
         item.code = gen_code()
 
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             stmt = (insert(WatchTaskOrm)
                     .values(subscriber=item.subscriber.dict(),
                             code=item.code,
                             type=item.type,
                             kwargs=item.kwargs,
                             bot=str(item.bot),
                             checkpoint=item.checkpoint))
@@ -102,15 +103,15 @@
             await session.commit()
 
             return result.rowcount == 1
 
     async def update(self, item: WatchTask[T_UID, T_GID]) -> bool:
         item.subscriber = process_subscriber(item.subscriber)
 
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             stmt = (update(WatchTaskOrm)
                     .values(type=item.type,
                             kwargs=item.kwargs,
                             bot=str(item.bot),
                             checkpoint=item.checkpoint)
                     .where(WatchTaskOrm.subscriber == item.subscriber.dict(),
                            WatchTaskOrm.code == item.code))
@@ -119,15 +120,15 @@
             return result.rowcount == 1
 
     async def delete_one(self, bot: UserIdentifier[T_UID],
                          subscriber: PostIdentifier[T_UID, T_GID],
                          code: int) -> Optional[WatchTask[T_UID, T_GID]]:
         subscriber = process_subscriber(subscriber)
 
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             stmt = (select(WatchTaskOrm)
                     .where(WatchTaskOrm.bot == str(bot),
                            WatchTaskOrm.subscriber == subscriber.dict(),
                            WatchTaskOrm.code == code)
                     .limit(1))
             task = (await session.execute(stmt)).scalar_one_or_none()
 
@@ -139,15 +140,15 @@
             return _to_model(task)
 
     async def delete_many_by_subscriber(self, bot: UserIdentifier[T_UID],
                                         subscriber: PostIdentifier[T_UID, T_GID]) \
             -> Collection[WatchTask[T_UID, T_GID]]:
         subscriber = process_subscriber(subscriber)
 
-        async with self.data_source.start_session() as session:
+        async with data_source.start_session() as session:
             stmt = (select(WatchTaskOrm)
                     .where(WatchTaskOrm.bot == str(bot),
                            WatchTaskOrm.subscriber == subscriber.dict()))
             tasks = (await session.execute(stmt)).scalars().all()
 
             for t in tasks:
                 await session.delete(t)
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/enums.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/enums.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/base.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from nonebot_plugin_pixivbot.model import Illust, T_UID, T_GID
 from nonebot_plugin_pixivbot.model.message import IllustMessagesModel
 from nonebot_plugin_pixivbot.protocol_dep.post_dest import PostDestination
 from nonebot_plugin_pixivbot.protocol_dep.postman import PostmanManager
 from .interceptor.base import Interceptor, DummyInterceptor
 from .interceptor.combined_interceptor import CombinedInterceptor
 from .interceptor.default_error_interceptor import DefaultErrorInterceptor
+from .interceptor.service_interceptor import ServiceInterceptor
 from .pkg_context import context
 from ..plugin_service import r18_service, r18g_service
 from ..utils.algorithm import as_unique
 
 conf = context.require(Config)
 
 
@@ -43,14 +44,26 @@
                     else:
                         interceptors.append(base_cls.interceptor)
 
         if "interceptors" in kwargs:
             interceptors.extend(kwargs["interceptors"])
             del kwargs["interceptors"]
 
+        if "service" in kwargs:
+            service = kwargs["service"]
+            del kwargs["service"]
+
+            if "service_interceptor_kwargs" in kwargs:
+                service_interceptor_kwargs = kwargs["service_interceptor_kwargs"]
+                del kwargs["service_interceptor_kwargs"]
+            else:
+                service_interceptor_kwargs = {}
+
+            interceptors.insert(0, ServiceInterceptor(service, **service_interceptor_kwargs))
+
         interceptors = as_unique(interceptors)
 
         cls = super().__new__(mcs, name, bases, namespace, **kwargs)
 
         if len(interceptors) == 0:
             cls.interceptor = DummyInterceptor()
         elif len(interceptors) == 1:
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/command/bind.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/command/bind.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from .subcommand import SubCommandHandler
 from ..interceptor.service_interceptor import ServiceInterceptor
 from ..pkg_context import context
 
 binder = context.require(PixivAccountBinder)
 
 
-class BindHandler(SubCommandHandler, subcommand='bind', interceptors=[ServiceInterceptor(bind_service)]):
+class BindHandler(SubCommandHandler, subcommand='bind', service=bind_service):
     @classmethod
     def type(cls) -> str:
         return "bind"
 
     async def parse_args(self, args: Sequence[str]) -> dict:
         if len(args) < 1:
             raise BadRequestError()
@@ -42,15 +42,15 @@
                     msg = f"当前绑定账号：{pixiv_user_id}\n"
                 else:
                     msg = "当前未绑定Pixiv账号\n"
                 msg += f"命令格式：{default_command_start}pixivbot bind <pixiv_user_id>"
                 await self.post_plain_text(message=msg)
 
 
-class UnbindHandler(SubCommandHandler, subcommand='unbind', interceptors=[ServiceInterceptor(bind_service)]):
+class UnbindHandler(SubCommandHandler, subcommand='unbind', service=bind_service):
     @classmethod
     def type(cls) -> str:
         return "unbind"
 
     # noinspection PyMethodOverriding
     async def actual_handle(self):
         result = await binder.unbind(self.post_dest.adapter, self.post_dest.user_id)
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/command/command.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/command/command.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/command/help.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/command/help.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,14 @@
 - {default_command_start}pixivbot help：查看本帮助
 - {default_command_start}pixivbot bind：绑定Pixiv账号
 
 更多功能：参见https://github.com/ssttkkl/nonebot-plugin-pixivbot
 """.strip()
 
 
-class HelpHandler(SubCommandHandler, subcommand='help', interceptors=[ServiceInterceptor(help_service)]):
+class HelpHandler(SubCommandHandler, subcommand='help', service=help_service):
     @classmethod
     def type(cls) -> str:
         return "help"
 
     async def actual_handle(self):
         await self.post_plain_text(help_text)
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/command/invalidate_cache.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/command/invalidate_cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 from ..interceptor.permission_interceptor import SuperuserInterceptor
 from ..interceptor.service_interceptor import ServiceInterceptor
 from ..pkg_context import context
 
 repo = context.require(PixivRepo)
 
 
-class InvalidateCacheHandler(SubCommandHandler, subcommand='invalidate_cache',
-                             interceptors=[context.require(SuperuserInterceptor),
-                                           ServiceInterceptor(invalidate_cache_service)]):
+class InvalidateCacheHandler(SubCommandHandler, subcommand='invalidate_cache', service=invalidate_cache_service,
+                             interceptors=[context.require(SuperuserInterceptor)]):
 
     @classmethod
     def type(cls) -> str:
         return "invalidate_cache"
 
     async def actual_handle(self):
         await repo.invalidate_cache()
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/command/schedule.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/command/schedule.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from nonebot_plugin_pixivbot.model import T_UID, T_GID
 from nonebot_plugin_pixivbot.plugin_service import manage_schedule_service
 from nonebot_plugin_pixivbot.protocol_dep.post_dest import PostDestination
 from nonebot_plugin_pixivbot.service.scheduler import Scheduler
 from nonebot_plugin_pixivbot.utils.errors import BadRequestError
 from nonebot_plugin_pixivbot.utils.nonebot import default_command_start
 from .subcommand import SubCommandHandler
-from ..interceptor.service_interceptor import ServiceInterceptor
 from ..pkg_context import context
 
 scheduler = context.require(Scheduler)
 
 
 async def build_subscriptions_msg(post_dest: PostDestination[T_UID, T_GID]):
     scheduler = context.require(Scheduler)
@@ -28,16 +27,15 @@
                     sio.write(f' ({args_text})')
                 sio.write('\n')
         else:
             sio.write('无\n')
         return sio.getvalue()
 
 
-class ScheduleHandler(SubCommandHandler, subcommand='schedule',
-                      interceptors=[ServiceInterceptor(manage_schedule_service)]):
+class ScheduleHandler(SubCommandHandler, subcommand='schedule', service=manage_schedule_service):
     @classmethod
     def type(cls) -> str:
         return "schedule"
 
     async def parse_args(self, args: Sequence[str]) -> dict:
         if len(args) < 2:
             raise BadRequestError()
@@ -69,28 +67,33 @@
                "random_user_illust, ranking\n" \
                "  <schedule>：格式为HH:mm（每日固定时间点推送）或HH:mm*x（间隔时间推送）\n" \
                "  [...args]：根据<type>不同需要提供不同的参数\n" \
                f"示例：{default_command_start}pixivbot schedule ranking 06:00*x day 1-5"
         await self.post_plain_text(message=msg)
 
 
-class UnscheduleHandler(SubCommandHandler, subcommand='unschedule',
-                        interceptors=[ServiceInterceptor(manage_schedule_service)]):
+class UnscheduleHandler(SubCommandHandler, subcommand='unschedule', service=manage_schedule_service):
     @classmethod
     def type(cls) -> str:
         return "unschedule"
 
     async def parse_args(self, args: Sequence[str]) -> dict:
         if len(args) == 0:
             raise BadRequestError()
         return {"code": args[0]}
 
     # noinspection PyMethodOverriding
     async def actual_handle(self, *, code: str):
-        if await scheduler.remove_task(self.post_dest, code):
+        if code != "all":
+            ok = await scheduler.remove_task(self.post_dest, code)
+        else:
+            await scheduler.remove_all_by_subscriber(self.post_dest)
+            ok = True
+
+        if ok:
             await self.post_plain_text(message="取消订阅成功")
         else:
             raise BadRequestError("取消订阅失败，不存在该订阅")
 
     async def actual_handle_bad_request(self, err: BadRequestError):
         msg = ""
         if err.message:
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/command/subcommand.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/command/subcommand.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/command/watch.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/command/watch.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from nonebot_plugin_pixivbot.plugin_service import manage_watch_service
 from nonebot_plugin_pixivbot.protocol_dep.post_dest import PostDestination
 from nonebot_plugin_pixivbot.service.pixiv_service import PixivService
 from nonebot_plugin_pixivbot.service.watchman import Watchman
 from nonebot_plugin_pixivbot.utils.errors import BadRequestError
 from nonebot_plugin_pixivbot.utils.nonebot import default_command_start
 from .subcommand import SubCommandHandler
-from ..interceptor.service_interceptor import ServiceInterceptor
 from ..pkg_context import context
 
 watchman = context.require(Watchman)
 pixiv = context.require(PixivService)
 
 
 async def parse_and_get_user(raw_user: str):
@@ -64,16 +63,15 @@
         watch_args = {"pixiv_user_id": 0,
                       "sender_user_id": post_dest.user_id}
         message = "关注者插画更新"
 
     return watch_args, message
 
 
-class WatchHandler(SubCommandHandler, subcommand='watch',
-                   interceptors=[ServiceInterceptor(manage_watch_service)]):
+class WatchHandler(SubCommandHandler, subcommand='watch', service=manage_watch_service):
 
     @classmethod
     def type(cls) -> str:
         return "watch"
 
     async def parse_args(self, args: Sequence[str]) -> dict:
         if len(args) == 0:
@@ -128,28 +126,33 @@
                "参数：\n" \
                "  <type>：可选值有user_illusts, following_illusts\n" \
                "  [...args]：根据<type>不同需要提供不同的参数\n" \
                f"示例：{default_command_start}pixivbot watch user_illusts <用户名>\n"
         await self.post_plain_text(message=msg)
 
 
-class UnwatchHandler(SubCommandHandler, subcommand='unwatch',
-                     interceptors=[ServiceInterceptor(manage_watch_service)]):
+class UnwatchHandler(SubCommandHandler, subcommand='unwatch', service=manage_watch_service):
     @classmethod
     def type(cls) -> str:
         return "unwatch"
 
     async def parse_args(self, args: Sequence[str]) -> dict:
         if len(args) == 0:
             raise BadRequestError()
         return {"code": args[0]}
 
     # noinspection PyMethodOverriding
     async def actual_handle(self, *, code: str):
-        if await watchman.remove_task(self.post_dest, code):
+        if code != "all":
+            ok = await watchman.remove_task(self.post_dest, code)
+        else:
+            await watchman.remove_all_by_subscriber(self.post_dest)
+            ok = True
+
+        if ok:
             await self.post_plain_text(message="取消订阅成功")
         else:
             raise BadRequestError("取消订阅失败，不存在该订阅")
 
     async def actual_handle_bad_request(self, err: BadRequestError):
         msg = ""
         if err.message:
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/common/__init__.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/common/base.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/common/illust.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/illust.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,27 +4,25 @@
 from nonebot.internal.params import Depends
 from nonebot.typing import T_State
 
 from nonebot_plugin_pixivbot.model import T_UID, T_GID
 from nonebot_plugin_pixivbot.plugin_service import illust_service
 from nonebot_plugin_pixivbot.utils.errors import BadRequestError
 from .base import CommonHandler
-from ..interceptor.default_error_interceptor import DefaultErrorInterceptor
-from ..interceptor.service_interceptor import ServiceInterceptor
 from ..pkg_context import context
 from ..utils import get_common_query_rule
 from ...config import Config
 from ...protocol_dep.post_dest import post_destination
 from ...service.pixiv_service import PixivService
 
 conf = context.require(Config)
 service = context.require(PixivService)
 
 
-class IllustHandler(CommonHandler, Generic[T_UID, T_GID]):
+class IllustHandler(CommonHandler, Generic[T_UID, T_GID], service=illust_service):
     @classmethod
     def type(cls) -> str:
         return "illust"
 
     @classmethod
     def enabled(cls) -> bool:
         return conf.pixiv_illust_query_enabled
@@ -37,16 +35,12 @@
 
     # noinspection PyMethodOverriding
     async def actual_handle(self, illust_id: int):
         illust = await service.illust_detail(illust_id)
         await self.post_illust(illust)
 
 
-IllustHandler.add_interceptor_after(ServiceInterceptor(illust_service),
-                                    after=context.require(DefaultErrorInterceptor))
-
-
 @on_regex(r"^看看图\s*([1-9][0-9]*)$", rule=get_common_query_rule(), priority=5).handle()
 async def on_match(state: T_State,
                    post_dest=Depends(post_destination)):
     illust_id = state["_matched_groups"][0]
     await IllustHandler(post_dest).handle(illust_id)
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/common/more.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/random_user_illust.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,52 @@
+from typing import Sequence
+from typing import Union
+
 from nonebot import on_regex
 from nonebot.internal.params import Depends
 from nonebot.typing import T_State
 
-from nonebot_plugin_pixivbot.plugin_service import more_service
+from nonebot_plugin_pixivbot.plugin_service import random_user_illust_service
 from nonebot_plugin_pixivbot.protocol_dep.post_dest import post_destination
-from nonebot_plugin_pixivbot.utils.errors import BadRequestError
-from .base import CommonHandler
-from ..interceptor.default_error_interceptor import DefaultErrorInterceptor
-from ..interceptor.service_interceptor import ServiceInterceptor
+from .base import RecordCommonHandler
 from ..pkg_context import context
-from ..recorder import Recorder
 from ..utils import get_common_query_rule, get_count
 from ...config import Config
+from ...service.pixiv_service import PixivService
 
-recorder = context.require(Recorder)
 conf = context.require(Config)
+service = context.require(PixivService)
 
 
-class MoreHandler(CommonHandler):
+class RandomUserIllustHandler(RecordCommonHandler, service=random_user_illust_service):
     @classmethod
     def type(cls) -> str:
-        return "more"
+        return "random_user_illust"
 
     @classmethod
     def enabled(cls) -> bool:
-        return conf.pixiv_more_enabled
-
-    async def actual_handle(self, count: int = 1):
-        req = recorder.get_req(self.post_dest.identifier)
-        if not req:
-            raise BadRequestError("你还没有发送过请求")
-
-        handler = req.handler_type(self.post_dest, silently=self.silently, disable_interceptors=True)
-        await handler.handle(*req.args, **{**req.kwargs, "count": count})
+        return conf.pixiv_random_user_illust_query_enabled
 
+    async def parse_args(self, args: Sequence[str]) -> dict:
+        try:
+            user_id = int(args[0])
+            return {"user": user_id}
+        except ValueError:
+            user = await service.get_user(args[0])
+            return {"user": user.id}
+
+    # noinspection PyMethodOverriding
+    async def actual_handle(self, *, user: Union[str, int],
+                            count: int = 1):
+        userinfo, illusts = await service.random_user_illust(user, count=count,
+                                                             exclude_r18=(not await self.is_r18_allowed()),
+                                                             exclude_r18g=(not await self.is_r18g_allowed()))
 
-MoreHandler.add_interceptor_after(ServiceInterceptor(more_service),
-                                  after=context.require(DefaultErrorInterceptor))
+        await self.post_illusts(illusts,
+                                header=f"这是您点的{userinfo.name}({userinfo.id})老师的图")
 
 
-@on_regex("^还要((.*)张)?$", rule=get_common_query_rule(), priority=1, block=True).handle()
+@on_regex("^来(.*)?张(.+)老师的图$", rule=get_common_query_rule(), priority=4, block=True).handle()
 async def on_match(state: T_State,
                    post_dest=Depends(post_destination)):
-    await MoreHandler(post_dest).handle(count=get_count(state, 1))
+    user = state["_matched_groups"][1]
+    await RandomUserIllustHandler(post_dest).handle(user, count=get_count(state))
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/common/random_bookmark.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/random_bookmark.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,26 @@
 from nonebot.typing import T_State
 
 from nonebot_plugin_pixivbot.model import T_UID
 from nonebot_plugin_pixivbot.plugin_service import random_bookmark_service
 from nonebot_plugin_pixivbot.service.pixiv_account_binder import PixivAccountBinder
 from nonebot_plugin_pixivbot.utils.errors import BadRequestError
 from .base import RecordCommonHandler
-from ..interceptor.default_error_interceptor import DefaultErrorInterceptor
-from ..interceptor.service_interceptor import ServiceInterceptor
 from ..pkg_context import context
 from ..utils import get_common_query_rule, get_count
 from ...config import Config
 from ...protocol_dep.post_dest import post_destination
 from ...service.pixiv_service import PixivService
 
 conf = context.require(Config)
 binder = context.require(PixivAccountBinder)
 service = context.require(PixivService)
 
 
-class RandomBookmarkHandler(RecordCommonHandler):
+class RandomBookmarkHandler(RecordCommonHandler, service=random_bookmark_service):
     @classmethod
     def type(cls) -> str:
         return "random_bookmark"
 
     @classmethod
     def enabled(cls) -> bool:
         return conf.pixiv_random_bookmark_query_enabled
@@ -61,15 +59,11 @@
                                                 exclude_r18=(not await self.is_r18_allowed()),
                                                 exclude_r18g=(not await self.is_r18g_allowed()))
 
         await self.post_illusts(illusts,
                                 header="这是您点的私家车")
 
 
-RandomBookmarkHandler.add_interceptor_after(ServiceInterceptor(random_bookmark_service),
-                                            after=context.require(DefaultErrorInterceptor))
-
-
 @on_regex("^来(.*)?张私家车$", rule=get_common_query_rule(), priority=5).handle()
 async def on_match(state: T_State,
                    post_dest=Depends(post_destination)):
     await RandomBookmarkHandler(post_dest).handle(count=get_count(state))
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/common/random_illust.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/random_illust.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,26 +3,24 @@
 from nonebot import on_regex
 from nonebot.internal.params import Depends
 from nonebot.typing import T_State
 
 from nonebot_plugin_pixivbot.plugin_service import random_illust_service
 from nonebot_plugin_pixivbot.protocol_dep.post_dest import post_destination
 from .base import RecordCommonHandler
-from ..interceptor.default_error_interceptor import DefaultErrorInterceptor
-from ..interceptor.service_interceptor import ServiceInterceptor
 from ..pkg_context import context
 from ..utils import get_common_query_rule, get_count
 from ...config import Config
 from ...service.pixiv_service import PixivService
 
 conf = context.require(Config)
 service = context.require(PixivService)
 
 
-class RandomIllustHandler(RecordCommonHandler):
+class RandomIllustHandler(RecordCommonHandler, service=random_illust_service):
     @classmethod
     def type(cls) -> str:
         return "random_illust"
 
     @classmethod
     def enabled(cls) -> bool:
         return conf.pixiv_random_illust_query_enabled
@@ -37,16 +35,12 @@
                                               exclude_r18=(not await self.is_r18_allowed()),
                                               exclude_r18g=(not await self.is_r18g_allowed()))
 
         await self.post_illusts(illusts,
                                 header=f"这是您点的{word}图")
 
 
-RandomIllustHandler.add_interceptor_after(ServiceInterceptor(random_illust_service),
-                                          after=context.require(DefaultErrorInterceptor))
-
-
 @on_regex("^来(.*)?张(.+)图$", rule=get_common_query_rule(), priority=5).handle()
 async def on_match(state: T_State,
                    post_dest=Depends(post_destination)):
     word = state["_matched_groups"][1]
     await RandomIllustHandler(post_dest).handle(word, count=get_count(state))
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/common/random_recommended_illust.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/random_recommended_illust.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 from nonebot import on_regex
 from nonebot.internal.params import Depends
 from nonebot.typing import T_State
 
 from nonebot_plugin_pixivbot.plugin_service import random_recommended_illust_service
 from nonebot_plugin_pixivbot.protocol_dep.post_dest import post_destination
 from .base import RecordCommonHandler
-from ..interceptor.default_error_interceptor import DefaultErrorInterceptor
-from ..interceptor.service_interceptor import ServiceInterceptor
 from ..pkg_context import context
 from ..utils import get_common_query_rule, get_count
 from ...config import Config
 from ...service.pixiv_service import PixivService
 
 conf = context.require(Config)
 service = context.require(PixivService)
 
 
-class RandomRecommendedIllustHandler(RecordCommonHandler):
+class RandomRecommendedIllustHandler(RecordCommonHandler, service=random_recommended_illust_service):
     @classmethod
     def type(cls) -> str:
         return "random_recommended_illust"
 
     @classmethod
     def enabled(cls) -> bool:
         return conf.pixiv_random_recommended_illust_query_enabled
@@ -30,15 +28,11 @@
                                                           exclude_r18=(not await self.is_r18_allowed()),
                                                           exclude_r18g=(not await self.is_r18g_allowed()))
 
         await self.post_illusts(illusts,
                                 header="这是您点的图")
 
 
-RandomRecommendedIllustHandler.add_interceptor_after(ServiceInterceptor(random_recommended_illust_service),
-                                                     after=context.require(DefaultErrorInterceptor))
-
-
 @on_regex("^来(.*)?张图$", rule=get_common_query_rule(), priority=3, block=True).handle()
 async def on_match(state: T_State,
                    post_dest=Depends(post_destination)):
     await RandomRecommendedIllustHandler(post_dest).handle(count=get_count(state))
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/common/random_related_illust.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/random_related_illust.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,28 +3,26 @@
 from nonebot import on_regex
 from nonebot.internal.params import Depends
 
 from nonebot_plugin_pixivbot.plugin_service import random_related_illust_service
 from nonebot_plugin_pixivbot.protocol_dep.post_dest import post_destination
 from nonebot_plugin_pixivbot.utils.errors import BadRequestError
 from .base import RecordCommonHandler
-from ..interceptor.default_error_interceptor import DefaultErrorInterceptor
-from ..interceptor.service_interceptor import ServiceInterceptor
 from ..pkg_context import context
 from ..recorder import Recorder
 from ..utils import get_common_query_rule
 from ...config import Config
 from ...service.pixiv_service import PixivService
 
 conf = context.require(Config)
 service = context.require(PixivService)
 recorder = context.require(Recorder)
 
 
-class RandomRelatedIllustHandler(RecordCommonHandler):
+class RandomRelatedIllustHandler(RecordCommonHandler, service=random_related_illust_service):
     @classmethod
     def type(cls) -> str:
         return "random_related_illust"
 
     @classmethod
     def enabled(cls) -> bool:
         return conf.pixiv_random_related_illust_query_enabled
@@ -42,14 +40,10 @@
                                                       exclude_r18=(not await self.is_r18_allowed()),
                                                       exclude_r18g=(not await self.is_r18g_allowed()))
 
         await self.post_illusts(illusts,
                                 header=f"这是您点的[{illust_id}]的相关图片")
 
 
-RandomRelatedIllustHandler.add_interceptor_after(ServiceInterceptor(random_related_illust_service),
-                                                 after=context.require(DefaultErrorInterceptor))
-
-
 @on_regex("^不够色$", rule=get_common_query_rule(), priority=1, block=True).handle()
 async def on_match(post_dest=Depends(post_destination)):
     await RandomRelatedIllustHandler(post_dest).handle()
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/common/ranking.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/ranking.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,27 +7,25 @@
 from nonebot.typing import T_State
 
 from nonebot_plugin_pixivbot.enums import RankingMode
 from nonebot_plugin_pixivbot.plugin_service import ranking_service
 from nonebot_plugin_pixivbot.utils.decode_integer import decode_integer
 from nonebot_plugin_pixivbot.utils.errors import BadRequestError
 from .base import CommonHandler
-from ..interceptor.default_error_interceptor import DefaultErrorInterceptor
-from ..interceptor.service_interceptor import ServiceInterceptor
 from ..pkg_context import context
 from ..utils import get_common_query_rule
 from ...config import Config
 from ...protocol_dep.post_dest import post_destination
 from ...service.pixiv_service import PixivService
 
 conf = context.require(Config)
 service = context.require(PixivService)
 
 
-class RankingHandler(CommonHandler):
+class RankingHandler(CommonHandler, service=ranking_service):
     @classmethod
     def type(cls) -> str:
         return "ranking"
 
     mode_mapping = {RankingMode.day: "日", RankingMode.week: "周", RankingMode.month: "月",
                     RankingMode.day_male: "男性", RankingMode.day_female: "女性", RankingMode.week_original: "原创",
                     RankingMode.week_rookie: "新人", RankingMode.day_manga: "漫画", RankingMode.day_ai: 'ai'}
@@ -95,18 +93,14 @@
         self.validate_range(range)
         illusts = await service.illust_ranking(mode, range)
         await self.post_illusts(illusts,
                                 header=f"这是您点的{self.mode_mapping[mode]}榜",
                                 number=range[0])
 
 
-RankingHandler.add_interceptor_after(ServiceInterceptor(ranking_service),
-                                     after=context.require(DefaultErrorInterceptor))
-
-
 @on_regex(r"^看看(.*)?榜\s*(.*)?$", rule=get_common_query_rule(), priority=4, block=True).handle()
 async def on_match(state: T_State,
                    post_dest=Depends(post_destination)):
     if "_matched_groups" in state:
         mode = state["_matched_groups"][0]
         num = state["_matched_groups"][1]
     else:
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/interceptor/base.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/interceptor/combined_interceptor.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/combined_interceptor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/interceptor/default_error_interceptor.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/default_error_interceptor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/interceptor/loading_prompt_interceptor.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/loading_prompt_interceptor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/interceptor/permission_interceptor.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/permission_interceptor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/interceptor/record_req_interceptor.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/record_req_interceptor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/interceptor/retry_interceptor.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/retry_interceptor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/interceptor/service_interceptor.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/service_interceptor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/interceptor/timeout_interceptor.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/timeout_interceptor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/recorder.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/recorder.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,16 +71,18 @@
             key = self._key_fallback(key)
             if key is not None:
                 return self.get_resp(key)
             else:
                 return None
 
 
-@context.inject
-@context.bind_singleton_to(PostmanManager, context.require(PostmanManager))
+origin_postman_mgr = context.require(PostmanManager)
+
+
+@context.bind_singleton_to(PostmanManager, origin_postman_mgr)
 class RecordPostmanManager:
     def __init__(self, delegation: PostmanManager):
         self.delegation = delegation
 
     async def send_illusts(self, model: IllustMessagesModel,
                            *, post_dest: PostDestination[T_UID, T_GID]):
         recorder = context.require(Recorder)
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/utils.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/watch/following_illusts.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/watch/following_illusts.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,26 +13,25 @@
 
 conf = context.require(Config)
 binder = context.require(PixivAccountBinder)
 pixiv = context.require(PixivRepo)
 
 
 # 因为要强制从远端获取，所以用这个shared_agen_mgr来缓存
-@context.register_singleton()
 class WatchFollowingIllustsSharedAsyncGeneratorManager(SharedAsyncGeneratorManager[int, Illust]):
     log_tag = "watch_following_illusts_shared_agen"
 
     async def agen(self, identifier: int, cache_strategy: CacheStrategy, **kwargs):
         await self.set_expires_time(identifier, time.time() + 30)  # 30s过期，保证每分钟的所有task都能共享
         async for x in pixiv.user_following_illusts(user_id=identifier,
                                                     cache_strategy=CacheStrategy.FORCE_EXPIRATION):
             yield await x.get()
 
 
-shared_agen_mgr = context.require(WatchFollowingIllustsSharedAsyncGeneratorManager)
+shared_agen_mgr = WatchFollowingIllustsSharedAsyncGeneratorManager()
 
 
 class WatchFollowingIllustsHandler(WatchTaskHandler):
     @classmethod
     def type(cls) -> str:
         return "watch_user_illusts"
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/handler/watch/user_illusts.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/watch/user_illusts.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,30 +11,27 @@
 from ..pkg_context import context
 
 pixiv = context.require(PixivRepo)
 remote_pixiv = context.require(RemotePixivRepo)
 
 
 # 因为要强制从远端获取，所以用这个shared_agen_mgr来缓存
-@context.register_singleton()
 class WatchUserIllustsSharedAsyncGeneratorManager(SharedAsyncGeneratorManager[int, Illust]):
     log_tag = "watch_user_illusts_shared_agen"
 
     async def agen(self, identifier: int, cache_strategy: CacheStrategy, **kwargs):
         await self.set_expires_time(identifier, time.time() + 30)  # 30s过期，保证每分钟的所有task都能共享
         async for x in pixiv.user_illusts(user_id=identifier,
                                           cache_strategy=CacheStrategy.FORCE_EXPIRATION):
             yield await x.get()
 
 
-shared_agen_mgr = context.require(WatchUserIllustsSharedAsyncGeneratorManager)
+shared_agen_mgr = WatchUserIllustsSharedAsyncGeneratorManager()
 
 
-@context.inject
-@context.root.register_singleton()
 class WatchUserIllustsHandler(WatchTaskHandler):
     @classmethod
     def type(cls) -> str:
         return "watch_user_illusts"
 
     # noinspection PyMethodOverriding
     async def actual_handle(self, *, task: WatchTask):
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/model/__init__.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/model/identifier.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/identifier.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/model/illust.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/illust.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/model/message/illust_message.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/message/illust_message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/model/message/illust_messages.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/message/illust_messages.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/model/old/subscription.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/old/subscription.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/model/subscription.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/subscription.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from enum import Enum
 from typing import Sequence, Dict, Any, Generic
 
 import tzlocal
 
 from . import T_UID, T_GID
 from .interval_task import IntervalTask
+from ..utils.format import format_kwargs
 
 
 class ScheduleType(str, Enum):
     random_bookmark = "random_bookmark"
     random_recommended_illust = "random_recommended_illust"
     random_illust = "random_illust"
     random_user_illust = "random_user_illust"
@@ -24,19 +25,20 @@
     @property
     def schedule_text(self) -> str:
         return f'{str(self.schedule[0]).zfill(2)}:{str(self.schedule[1]).zfill(2)}' \
                f'+{str(self.schedule[2]).zfill(2)}:{str(self.schedule[3]).zfill(2)}*x'
 
     @property
     def args_text(self) -> str:
-        args = list(filter(lambda kv: kv[1], self.kwargs.items()))
-        if len(args) != 0:
-            return ", ".join(map(lambda kv: f'{kv[0]}={kv[1]}', args))
-        else:
-            return ""
+        filtered_kwargs = {}
+        for k in self.kwargs:
+            if self.kwargs[k]:
+                filtered_kwargs[k] = self.kwargs[k]
+
+        return format_kwargs(**filtered_kwargs)
 
     def __repr__(self):
         text = f'[{self.code}] {self.type} on {self.schedule_text} by {self.subscriber}'
         if len(self.kwargs) != 0:
             text += f' ({self.args_text})'
         return text
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/plugin_service.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/plugin_service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/protocol_dep/authenticator.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/protocol_dep/authenticator.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/protocol_dep/post_dest.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/protocol_dep/post_dest.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/protocol_dep/postman.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/protocol_dep/postman.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/protocol_dep/protocol_dep.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/protocol_dep/protocol_dep.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/service/interval_task_worker.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/service/interval_task_worker.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,34 +3,36 @@
 from typing import Generic, TypeVar, AsyncIterable
 
 from apscheduler.triggers.base import BaseTrigger
 from nonebot import logger, Bot, get_bot
 from nonebot.exception import ActionFailed
 from nonebot_plugin_apscheduler import scheduler as apscheduler
 
-from nonebot_plugin_pixivbot.context import Inject
 from nonebot_plugin_pixivbot.data.interval_task_repo import IntervalTaskRepo
 from nonebot_plugin_pixivbot.global_context import context
 from nonebot_plugin_pixivbot.model import T_UID, T_GID
 from nonebot_plugin_pixivbot.model.interval_task import IntervalTask
 from nonebot_plugin_pixivbot.protocol_dep.authenticator import AuthenticatorManager
 from nonebot_plugin_pixivbot.protocol_dep.post_dest import PostDestinationFactoryManager, PostDestination
 from nonebot_plugin_pixivbot.utils.lifecycler import on_bot_connect, on_bot_disconnect
 from nonebot_plugin_pixivbot.utils.nonebot import get_bot_user_identifier
 
+pd_factory_mgr = context.require(PostDestinationFactoryManager)
+auth_mgr = context.require(AuthenticatorManager)
+
 T = TypeVar("T", bound=IntervalTask)
 
 
-@context.inject
 class IntervalTaskWorker(ABC, Generic[T]):
     tag: str = ""
-    repo: IntervalTaskRepo[T]
 
-    pd_factory_mgr: PostDestinationFactoryManager = Inject(PostDestinationFactoryManager)
-    auth_mgr: AuthenticatorManager = Inject(AuthenticatorManager)
+    @property
+    @abstractmethod
+    def repo(self) -> IntervalTaskRepo[T]:
+        raise NotImplementedError()
 
     def __init__(self):
         @on_bot_connect(replay=True)
         async def _(bot: Bot):
             async for task in self.repo.get_by_bot(get_bot_user_identifier(bot)):
                 try:
                     self._add_job(task)
@@ -55,28 +57,28 @@
     async def _handle_trigger(self, item: T, post_dest: PostDestination[T_UID, T_GID]):
         ...
 
     async def _on_trigger(self, item: T):
         logger.info(f"[{self.tag}] triggered \"{item}\"")
 
         bot = get_bot(item.bot.user_id)
-        post_dest = self.pd_factory_mgr.build(bot, item.subscriber.user_id, item.subscriber.group_id)
+        post_dest = pd_factory_mgr.build(bot, item.subscriber.user_id, item.subscriber.group_id)
 
         try:
             await self._handle_trigger(item, post_dest)
         except ActionFailed as e:
             logger.error(f"[{self.tag}] ActionFailed {e}")
 
-            available = self.auth_mgr.available(post_dest)
+            available = auth_mgr.available(post_dest)
             if isawaitable(available):
                 available = await available
 
             if not available:
                 logger.info(f"[{self.tag}] {post_dest} is no longer available, removing all his tasks...")
-                await self.unschedule_all_by_subscriber(post_dest)
+                await self.remove_all_by_subscriber(post_dest)
 
     @abstractmethod
     def _make_job_trigger(self, item: T) -> BaseTrigger:
         ...
 
     def _add_job(self, item: T):
         job_id = self._make_job_id(item)
@@ -116,15 +118,15 @@
         if item:
             logger.success(f"[{self.tag}] removed task \"{item}\"")
             self._remove_job(item)
             return True
         else:
             return False
 
-    async def unschedule_all_by_subscriber(self, post_dest: PostDestination[T_UID, T_GID]):
+    async def remove_all_by_subscriber(self, post_dest: PostDestination[T_UID, T_GID]):
         old = await self.repo.delete_many_by_subscriber(get_bot_user_identifier(post_dest.bot),
                                                         post_dest.identifier)
         for item in old:
             logger.success(f"[{self.tag}] removed task \"{item}\"")
             self._remove_job(item)
 
     async def get_by_subscriber(self, post_dest: PostDestination[T_UID, T_GID]) -> AsyncIterable[T]:
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/service/pixiv_account_binder.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/service/pixiv_account_binder.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from typing import Optional
 
-from nonebot_plugin_pixivbot.context import Inject
 from nonebot_plugin_pixivbot.data.pixiv_binding import PixivBindingRepo
 from nonebot_plugin_pixivbot.global_context import context
 from nonebot_plugin_pixivbot.model import T_UID
 from nonebot_plugin_pixivbot.model.pixiv_binding import PixivBinding
 
+repo = context.require(PixivBindingRepo)
+
 
-@context.inject
 @context.register_singleton()
 class PixivAccountBinder:
-    repo = Inject(PixivBindingRepo)
 
     async def bind(self, adapter: str, user_id: T_UID, pixiv_user_id: int):
         binding = PixivBinding(adapter=adapter, user_id=user_id, pixiv_user_id=pixiv_user_id)
-        await self.repo.update(binding)
+        await repo.update(binding)
 
     async def unbind(self, adapter: str, user_id: T_UID) -> bool:
-        return await self.repo.remove(adapter, user_id)
+        return await repo.remove(adapter, user_id)
 
     async def get_binding(self, adapter: str, user_id: T_UID) -> Optional[int]:
-        binding = await self.repo.get(adapter, user_id)
+        binding = await repo.get(adapter, user_id)
         if binding:
             return binding.pixiv_user_id
         else:
             return None
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/service/pixiv_service.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/service/pixiv_service.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from typing import List, Union, Tuple, Iterable, Sequence
 
 from nonebot import logger
 
 from nonebot_plugin_pixivbot.config import Config
-from nonebot_plugin_pixivbot.context import Inject
 from nonebot_plugin_pixivbot.data.local_tag import LocalTagRepo
 from nonebot_plugin_pixivbot.data.pixiv_repo import LazyIllust, PixivRepo
 from nonebot_plugin_pixivbot.enums import RandomIllustMethod, RankingMode
 from nonebot_plugin_pixivbot.global_context import context
 from nonebot_plugin_pixivbot.model import Illust, User
 from nonebot_plugin_pixivbot.service.roulette import roulette
 from nonebot_plugin_pixivbot.utils.errors import BadRequestError, QueryError
 
+conf = context.require(Config)
+repo = context.require(PixivRepo)
+local_tags = context.require(LocalTagRepo)
+
 
-@context.inject
 @context.register_singleton()
 class PixivService:
-    conf = Inject(Config)
-    repo = Inject(PixivRepo)
-    local_tag_repo = Inject(LocalTagRepo)
 
     @staticmethod
     def _handle_r18(illusts: Iterable[LazyIllust],
                     exclude_r18: bool = False,
                     exclude_r18g: bool = False) -> Iterable[LazyIllust]:
         if not exclude_r18 and not exclude_r18g:
             return illusts
@@ -39,97 +38,97 @@
 
             return _()
 
     async def _choice_and_load(self, illusts: Sequence[LazyIllust], random_method: RandomIllustMethod, count: int) \
             -> List[Illust]:
         if count <= 0:
             raise BadRequestError("不合法的请求数量")
-        if count > self.conf.pixiv_max_item_per_query:
+        if count > conf.pixiv_max_item_per_query:
             raise BadRequestError("数量超过单次请求上限")
         if count > len(illusts):
             raise QueryError("别看了，没有的。")
 
         winners = roulette(illusts, random_method, count)
         logger.info(f"[pixiv_service] choice {[x.id for x in winners]}")
         return [await x.get() for x in winners]
 
     async def illust_ranking(self, mode: RankingMode, range: Tuple[int, int]) -> List[Illust]:
         # range 下标从1开始 闭区间
         i = 1
         li = []
-        async for x in self.repo.illust_ranking(mode):
+        async for x in repo.illust_ranking(mode):
             if i > range[1]:
                 break
             elif i >= range[0]:
                 li.append(await x.get())
             i += 1
         return li
 
     async def illust_detail(self, illust: int) -> Illust:
-        async for x in self.repo.illust_detail(illust):
+        async for x in repo.illust_detail(illust):
             return x
 
     async def random_illust(self, word: str,
                             *, count: int = 1,
                             exclude_r18: bool = False,
                             exclude_r18g: bool = False) -> List[Illust]:
-        if self.conf.pixiv_tag_translation_enabled:
+        if conf.pixiv_tag_translation_enabled:
             # 只有原word不是标签时获取翻译（例子：唐可可）
-            tag = await self.local_tag_repo.find_by_name(word)
+            tag = await local_tags.find_by_name(word)
             if not tag:
-                tag = await self.local_tag_repo.find_by_translated_name(word)
+                tag = await local_tags.find_by_translated_name(word)
                 if tag:
                     logger.info(f"[pixiv_service] found translation {word} -> {tag.name}")
                     word = tag.name
 
-        illusts = [x async for x in self.repo.search_illust(word)]
+        illusts = [x async for x in repo.search_illust(word)]
         illusts = self._handle_r18(illusts, exclude_r18, exclude_r18g)
-        return await self._choice_and_load(list(illusts), self.conf.pixiv_random_illust_method, count)
+        return await self._choice_and_load(list(illusts), conf.pixiv_random_illust_method, count)
 
     async def get_user(self, user: Union[str, int]) -> User:
         if isinstance(user, str):
-            async for x in self.repo.search_user(user):
+            async for x in repo.search_user(user):
                 logger.info(f"[pixiv_service] select user {x.name}({x.id})")
                 return x
             raise QueryError("未找到用户")
         else:
-            async for x in self.repo.user_detail(user):
+            async for x in repo.user_detail(user):
                 return x
 
     async def random_user_illust(self, user: Union[str, int],
                                  *, count: int = 1,
                                  exclude_r18: bool = False,
                                  exclude_r18g: bool = False) -> Tuple[User, List[Illust]]:
         user = await self.get_user(user)
 
-        illusts = [x async for x in self.repo.user_illusts(user.id)]
+        illusts = [x async for x in repo.user_illusts(user.id)]
         illusts = self._handle_r18(illusts, exclude_r18, exclude_r18g)
-        illust = await self._choice_and_load(list(illusts), self.conf.pixiv_random_user_illust_method, count)
+        illust = await self._choice_and_load(list(illusts), conf.pixiv_random_user_illust_method, count)
         return user, illust
 
     async def random_recommended_illust(self, *, count: int = 1,
                                         exclude_r18: bool = False,
                                         exclude_r18g: bool = False) -> List[Illust]:
-        illusts = [x async for x in self.repo.recommended_illusts()]
-        return await self._choice_and_load(illusts, self.conf.pixiv_random_recommended_illust_method, count)
+        illusts = [x async for x in repo.recommended_illusts()]
+        return await self._choice_and_load(illusts, conf.pixiv_random_recommended_illust_method, count)
 
     async def random_bookmark(self, pixiv_user_id: int = 0,
                               *, count: int = 1,
                               exclude_r18: bool = False,
                               exclude_r18g: bool = False) -> List[Illust]:
-        illusts = [x async for x in self.repo.user_bookmarks(pixiv_user_id)]
+        illusts = [x async for x in repo.user_bookmarks(pixiv_user_id)]
         illusts = self._handle_r18(illusts, exclude_r18, exclude_r18g)
-        return await self._choice_and_load(list(illusts), self.conf.pixiv_random_bookmark_method, count)
+        return await self._choice_and_load(list(illusts), conf.pixiv_random_bookmark_method, count)
 
     async def random_related_illust(self, illust_id: int,
                                     *, count: int = 1,
                                     exclude_r18: bool = False,
                                     exclude_r18g: bool = False) -> List[Illust]:
         if illust_id == 0:
             raise BadRequestError("你还没有发送过请求")
 
-        illusts = [x async for x in self.repo.related_illusts(illust_id)]
+        illusts = [x async for x in repo.related_illusts(illust_id)]
         illusts = self._handle_r18(illusts, exclude_r18, exclude_r18g)
-        return await self._choice_and_load(list(illusts), self.conf.pixiv_random_related_illust_method, count)
+        return await self._choice_and_load(list(illusts), conf.pixiv_random_related_illust_method, count)
 
 
 __all__ = ("PixivService",)
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/service/roulette.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/service/roulette.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/service/scheduler.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/service/scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from datetime import datetime, timedelta
 from inspect import isawaitable
 from typing import Sequence, Union, TYPE_CHECKING, overload, Type
 
 import pytz
 from apscheduler.triggers.interval import IntervalTrigger
 
-from nonebot_plugin_pixivbot.context import Inject
 from nonebot_plugin_pixivbot.data.subscription import SubscriptionRepo
 from nonebot_plugin_pixivbot.global_context import context
 from nonebot_plugin_pixivbot.handler.schedule import SubscriptionRandomBookmarkHandler, \
     SubscriptionRandomRecommendedIllustHandler, SubscriptionRankingHandler, SubscriptionRandomIllustHandler, \
     SubscriptionRandomUserIllustHandler
 from nonebot_plugin_pixivbot.model import Subscription
 from nonebot_plugin_pixivbot.model import T_UID, T_GID
@@ -54,18 +53,20 @@
             or (interval_hour > 0 and interval_minute < 0) or (interval_hour == 0 and interval_minute <= 0):
         raise BadRequestError(f'{raw_schedule}不是合法的时间')
 
     return start_hour, start_minute, interval_hour, interval_minute
 
 
 @context.register_eager_singleton()
-@context.inject
 class Scheduler(IntervalTaskWorker[Subscription[T_UID, T_GID]]):
     tag = "scheduler"
-    repo: SubscriptionRepo = Inject(SubscriptionRepo)
+
+    @property
+    def repo(self) -> SubscriptionRepo:
+        return context.require(SubscriptionRepo)
 
     @classmethod
     def _get_handler_type(cls, type: ScheduleType) -> Type["Handler"]:
         if type == ScheduleType.random_bookmark:
             return SubscriptionRandomBookmarkHandler
         elif type == ScheduleType.random_recommended_illust:
             return SubscriptionRandomRecommendedIllustHandler
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/service/watchman.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/service/watchman.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 from datetime import datetime, timedelta, timezone
 from typing import Dict, Any, overload, Type
 
 from apscheduler.triggers.interval import IntervalTrigger
 
 from nonebot_plugin_pixivbot.config import Config
-from nonebot_plugin_pixivbot.context import Inject
 from nonebot_plugin_pixivbot.data.watch_task import WatchTaskRepo
 from nonebot_plugin_pixivbot.global_context import context
 from nonebot_plugin_pixivbot.handler.base import Handler
 from nonebot_plugin_pixivbot.handler.watch import WatchUserIllustsHandler, WatchFollowingIllustsHandler
 from nonebot_plugin_pixivbot.model import T_UID, T_GID
 from nonebot_plugin_pixivbot.model import WatchTask, WatchType
 from nonebot_plugin_pixivbot.protocol_dep.post_dest import PostDestination
-from nonebot_plugin_pixivbot.protocol_dep.postman import PostmanManager
 from nonebot_plugin_pixivbot.service.interval_task_worker import IntervalTaskWorker
-from nonebot_plugin_pixivbot.service.pixiv_account_binder import PixivAccountBinder
 from nonebot_plugin_pixivbot.utils.nonebot import get_bot_user_identifier
 
+conf = context.require(Config)
+
 
 @context.root.register_eager_singleton()
-@context.inject
 class Watchman(IntervalTaskWorker[WatchTask[T_UID, T_GID]]):
     tag = "watchman"
 
-    conf = Inject(Config)
-    binder = Inject(PixivAccountBinder)
-    postman_mgr = Inject(PostmanManager)
-    repo: WatchTaskRepo = Inject(WatchTaskRepo)
-
     _trigger_hasher_mapper = {
         WatchType.user_illusts: lambda args: args["user_id"],
         WatchType.following_illusts: lambda args: hash(args["sender_user_id"]),
     }
 
+    @property
+    def repo(self) -> WatchTaskRepo:
+        return context.require(WatchTaskRepo)
+
     @classmethod
     def _get_handler_type(cls, type: WatchType) -> Type["Handler"]:
         if type == WatchType.user_illusts:
             return WatchUserIllustsHandler
         elif type == WatchType.following_illusts:
             return WatchFollowingIllustsHandler
 
@@ -50,19 +47,19 @@
             # 保存checkpoint，避免一次异常后下一次重复推送
             # 但是会存在丢失推送的问题
             task.checkpoint = datetime.now(timezone.utc)
             await self.repo.update(task)
 
     def _make_job_trigger(self, item: WatchTask[T_UID, T_GID]) -> IntervalTrigger:
         hasher = self._trigger_hasher_mapper[item.type]
-        hash_sec = hasher(item.kwargs) % self.conf.pixiv_watch_interval
+        hash_sec = hasher(item.kwargs) % conf.pixiv_watch_interval
         yesterday = datetime.now(timezone.utc).replace(
             hour=0, minute=0, second=0, microsecond=0
         ) + timedelta(days=-1) + timedelta(seconds=hash_sec)
-        trigger = IntervalTrigger(seconds=self.conf.pixiv_watch_interval, start_date=yesterday)
+        trigger = IntervalTrigger(seconds=conf.pixiv_watch_interval, start_date=yesterday)
         return trigger
 
     async def _build_task(self, type_: WatchType,
                           kwargs: Dict[str, Any],
                           post_dest: PostDestination[T_UID, T_GID]) -> WatchTask:
         return WatchTask(type=type_, kwargs=kwargs,
                          subscriber=post_dest.identifier,
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/utils/decode_integer.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/utils/decode_integer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/utils/errors.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/utils/errors.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/utils/expires_lru_dict.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/utils/expires_lru_dict.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/utils/lifecycler.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/utils/lifecycler.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/utils/nonebot.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/utils/nonebot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot/utils/shared_agen.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/utils/shared_agen.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot_kook/config.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_kook/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot_kook/protocol_dep/authenticator.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_kook/protocol_dep/authenticator.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot_kook/protocol_dep/post_dest.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_kook/protocol_dep/post_dest.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot_kook/protocol_dep/postman.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_kook/protocol_dep/postman.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot_kook/utils/card_builder.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_kook/utils/card_builder.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot_kook/utils/illust_card.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_kook/utils/illust_card.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot_onebot_v11/config.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_onebot_v11/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot_onebot_v11/handler/poke.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_onebot_v11/handler/poke.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/authenticator.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/authenticator.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/post_dest.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/post_dest.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.1/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/postman.py` & `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/postman.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from io import StringIO
 
 from nonebot.adapters.onebot.v11 import Message, MessageSegment
 
-from nonebot_plugin_pixivbot.context import Inject
 from nonebot_plugin_pixivbot.enums import BlockAction
 from nonebot_plugin_pixivbot.global_context import context
 from nonebot_plugin_pixivbot.model.message import IllustMessageModel, IllustMessagesModel
 from nonebot_plugin_pixivbot.protocol_dep.postman import Postman as BasePostman, PostmanManager
 from nonebot_plugin_pixivbot_onebot_v11.config import OnebotV11Config
 from nonebot_plugin_pixivbot_onebot_v11.protocol_dep.post_dest import PostDestination
 
+conf = context.require(OnebotV11Config)
+
 
-@context.inject
 @context.register_singleton()
 class Postman(BasePostman[int, int], manager=PostmanManager):
-    conf: OnebotV11Config = Inject(OnebotV11Config)
-
     adapter = "onebot"
 
     def make_illust_msg(self, model: IllustMessageModel) -> Message:
         msg = Message()
 
         if model.block_action is not None:
             if model.block_action == BlockAction.no_image:
@@ -42,15 +40,15 @@
             sio.write(f"「{model.title}」")
             if model.total != 1:
                 sio.write(f"（{model.page + 1}/{model.total}）")
             sio.write("\n")
 
             sio.write(f"作者：{model.author}\n"
                       f"发布时间：{model.create_time}\n")
-            if self.conf.pixiv_onebot_with_link:
+            if conf.pixiv_onebot_with_link:
                 sio.write(model.link)
             else:
                 sio.write(f"Pixiv ID：{model.id}")
 
             msg.append(MessageSegment.text(sio.getvalue()))
         return msg
 
@@ -66,16 +64,16 @@
             message.append(MessageSegment.text(model.header + '\n'))
 
         message.extend(self.make_illust_msg(model))
         await post_dest.post(message)
 
     async def send_illusts(self, model: IllustMessagesModel,
                            *, post_dest: PostDestination):
-        if self.conf.pixiv_onebot_send_forward_message == 'never' or \
-                self.conf.pixiv_onebot_send_forward_message == 'auto' and len(model.messages) == 1:
+        if conf.pixiv_onebot_send_forward_message == 'never' or \
+                conf.pixiv_onebot_send_forward_message == 'auto' and len(model.messages) == 1:
             for x in model.flat():
                 await self.send_illust(x, post_dest=post_dest)
         else:
             messages = []
             if model.header:
                 messages.append(Message([MessageSegment.text(model.header)]))
             for sub_model in model.messages:
```

### Comparing `nonebot_plugin_pixivbot-1.8.1/PKG-INFO` & `nonebot_plugin_pixivbot-1.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pixivbot
-Version: 1.8.1
+Version: 1.8.2
 Summary: Nonebot Plugin PixivBot
 Home-page: https://github.com/ssttkkl/nonebot-plugin-pixivbot
 License: MIT
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -29,14 +29,15 @@
 Requires-Dist: frozendict (>=2.3.4,<3.0.0)
 Requires-Dist: lazy (>=1.4,<2.0)
 Requires-Dist: motor (>=3.0.0,<4.0.0) ; extra == "mongo"
 Requires-Dist: nonebot-adapter-kaiheila (>=0.2.0,<0.3.0) ; extra == "kook"
 Requires-Dist: nonebot-adapter-onebot (>=2.2.1,<3.0.0) ; extra == "onebot"
 Requires-Dist: nonebot-adapter-telegram (>=0.1.0b8,<0.2.0) ; extra == "telegram"
 Requires-Dist: nonebot-plugin-access-control (>=0.4.0,<0.5.0)
+Requires-Dist: nonebot-plugin-localstore (>=0.4.1,<0.5.0)
 Requires-Dist: nonebot2 (>=2.0.0rc2,<3.0.0)
 Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0)
 Requires-Dist: numpy (>=1.23.1,<2.0.0)
 Requires-Dist: shortuuid (>=1.0.9,<2.0.0)
 Requires-Dist: tzlocal (>=4.2,<5.0)
 Project-URL: Repository, https://github.com/ssttkkl/nonebot-plugin-pixivbot
 Description-Content-Type: text/markdown
@@ -303,15 +304,15 @@
 # OneBot平台（主要是gocq）配置
 pixiv_poke_action=random_recommended_illust  # 响应戳一戳动作，可选值：ranking, random_recommended_illust, random_bookmark, 什么都不填即忽略戳一戳动作
 pixiv_onebot_with_link=False  # 发图时是否带上链接（容易被tx盯上）
 pixiv_onebot_send_forward_message=auto  # 发图时是否使用转发消息的形式，可选值：always(永远使用), auto(仅在多张图片时使用), never(永远不使用)
 
 # 功能配置
 pixiv_more_enabled=True  # 启用重复上一次请求（还要）功能
-pixiv_query_expires_in=10*60  # 上一次请求的过期时间（单位：秒）
+pixiv_query_expires_in=600  # 上一次请求的过期时间（单位：秒）
 
 pixiv_illust_query_enabled=True  # 启用插画查询（看看图）功能
 
 pixiv_ranking_query_enabled=True  # 启用榜单查询（看看榜）功能
 pixiv_ranking_default_mode=day  # 默认查询的榜单，可选值：day, week, month, day_male, day_female, week_original, week_rookie, day_manga
 pixiv_ranking_default_range=[1, 3]  # 默认查询的榜单范围
 pixiv_ranking_fetch_item=150  # 每次从服务器获取的榜单项数（查询的榜单范围必须在这个数目内）
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-pixivbot Version: 1.8.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-pixivbot Version: 1.8.2 Summary:
 Nonebot Plugin PixivBot Home-page: https://github.com/ssttkkl/nonebot-plugin-
 pixivbot License: MIT Author: ssttkkl Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Provides-Extra: kook
 Provides-Extra: mongo Provides-Extra: onebot Provides-Extra: postgresql
@@ -14,19 +14,20 @@
 Dist: beanie (>=1.17.0,<2.0.0) ; extra == "mongo" Requires-Dist: cachetools
 (>=5.2.0,<6.0.0) Requires-Dist: frozendict (>=2.3.4,<3.0.0) Requires-Dist: lazy
 (>=1.4,<2.0) Requires-Dist: motor (>=3.0.0,<4.0.0) ; extra == "mongo" Requires-
 Dist: nonebot-adapter-kaiheila (>=0.2.0,<0.3.0) ; extra == "kook" Requires-
 Dist: nonebot-adapter-onebot (>=2.2.1,<3.0.0) ; extra == "onebot" Requires-
 Dist: nonebot-adapter-telegram (>=0.1.0b8,<0.2.0) ; extra == "telegram"
 Requires-Dist: nonebot-plugin-access-control (>=0.4.0,<0.5.0) Requires-Dist:
-nonebot2 (>=2.0.0rc2,<3.0.0) Requires-Dist: nonebot_plugin_apscheduler
-(>=0.2.0,<0.3.0) Requires-Dist: numpy (>=1.23.1,<2.0.0) Requires-Dist:
-shortuuid (>=1.0.9,<2.0.0) Requires-Dist: tzlocal (>=4.2,<5.0) Project-URL:
-Repository, https://github.com/ssttkkl/nonebot-plugin-pixivbot Description-
-Content-Type: text/markdown
+nonebot-plugin-localstore (>=0.4.1,<0.5.0) Requires-Dist: nonebot2
+(>=2.0.0rc2,<3.0.0) Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0)
+Requires-Dist: numpy (>=1.23.1,<2.0.0) Requires-Dist: shortuuid
+(>=1.0.9,<2.0.0) Requires-Dist: tzlocal (>=4.2,<5.0) Project-URL: Repository,
+https://github.com/ssttkkl/nonebot-plugin-pixivbot Description-Content-Type:
+text/markdown
                                    [nonebot]
                nonebot_plugin_pixivbot ===== _â¨ PixivBot â¨_
                            [license] [pypi] [python]
 NoneBotæä»¶ï¼æ¯æåééæºPixivæç»ãç»å¸æ´æ°æ¨éãå®æ¶è®¢éæ¨éâ¦â¦
 ## å¼å§ä½¿ç¨ ééåè®®ï¼ - [Onebot V11](https://
 onebot.adapters.nonebot.dev/) - [KOOK / å¼é»å¦](https://github.com/Tian-que/
 nonebot-adapter-kaiheila) - [Telegram](https://github.com/nonebot/adapter-
@@ -201,15 +202,15 @@
 random_bookmark, ä»ä¹é½ä¸å¡«å³å¿½ç¥æ³ä¸æ³å¨ä½
 pixiv_onebot_with_link=False #
 åå¾æ¶æ¯å¦å¸¦ä¸é¾æ¥ï¼å®¹æè¢«txç¯ä¸ï¼
 pixiv_onebot_send_forward_message=auto #
 åå¾æ¶æ¯å¦ä½¿ç¨è½¬åæ¶æ¯çå½¢å¼ï¼å¯éå¼ï¼always(æ°¸è¿ä½¿ç¨),
 auto(ä»å¨å¤å¼ å¾çæ¶ä½¿ç¨), never(æ°¸è¿ä¸ä½¿ç¨) # åè½éç½®
 pixiv_more_enabled=True # å¯ç¨éå¤ä¸ä¸æ¬¡è¯·æ±ï¼è¿è¦ï¼åè½
-pixiv_query_expires_in=10*60 # ä¸ä¸æ¬¡è¯·æ±çè¿ææ¶é´ï¼åä½ï¼ç§ï¼
+pixiv_query_expires_in=600 # ä¸ä¸æ¬¡è¯·æ±çè¿ææ¶é´ï¼åä½ï¼ç§ï¼
 pixiv_illust_query_enabled=True # å¯ç¨æç»æ¥è¯¢ï¼ççå¾ï¼åè½
 pixiv_ranking_query_enabled=True # å¯ç¨æ¦åæ¥è¯¢ï¼ççæ¦ï¼åè½
 pixiv_ranking_default_mode=day # é»è®¤æ¥è¯¢çæ¦åï¼å¯éå¼ï¼day, week,
 month, day_male, day_female, week_original, week_rookie, day_manga
 pixiv_ranking_default_range=[1, 3] # é»è®¤æ¥è¯¢çæ¦åèå´
 pixiv_ranking_fetch_item=150 #
 æ¯æ¬¡ä»æå¡å¨è·åçæ¦åé¡¹æ°ï¼æ¥è¯¢çæ¦åèå´å¿é¡»å¨è¿ä¸ªæ°ç®åï¼
```

