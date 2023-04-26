# Comparing `tmp/protean-0.9.0.tar.gz` & `tmp/protean-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protean-0.9.0.tar", last modified: Fri Feb 18 03:09:35 2022, max compression
+gzip compressed data, was "protean-0.9.1.tar", last modified: Wed Feb 23 21:38:05 2022, max compression
```

## Comparing `protean-0.9.0.tar` & `protean-0.9.1.tar`

### file list

```diff
@@ -1,499 +1,499 @@
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.780026 protean-0.9.0/
--rw-r--r--   0 subhashb   (501) staff       (20)      169 2022-02-18 02:30:54.000000 protean-0.9.0/.bumpversion.cfg
--rw-r--r--   0 subhashb   (501) staff       (20)     2043 2019-04-06 03:53:33.000000 protean-0.9.0/.cookiecutterrc
--rw-r--r--   0 subhashb   (501) staff       (20)      284 2019-04-06 03:53:33.000000 protean-0.9.0/.coveragerc
--rw-r--r--   0 subhashb   (501) staff       (20)      314 2020-09-22 16:40:24.000000 protean-0.9.0/.editorconfig
--rw-r--r--   0 subhashb   (501) staff       (20)       71 2020-09-22 16:40:24.000000 protean-0.9.0/.git-blame-ignore-revs
--rw-r--r--   0 subhashb   (501) staff       (20)      575 2022-02-12 19:48:13.000000 protean-0.9.0/.pre-commit-config.yaml
--rw-r--r--   0 subhashb   (501) staff       (20)    12859 2022-02-18 02:54:18.000000 protean-0.9.0/CHANGELOG.rst
--rw-r--r--   0 subhashb   (501) staff       (20)      658 2021-08-09 21:35:32.000000 protean-0.9.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 subhashb   (501) staff       (20)     6755 2021-08-09 21:32:40.000000 protean-0.9.0/CONTRIBUTING.rst
--rw-r--r--   0 subhashb   (501) staff       (20)     1516 2020-04-06 01:30:35.000000 protean-0.9.0/LICENSE
--rw-r--r--   0 subhashb   (501) staff       (20)      505 2020-09-22 16:40:24.000000 protean-0.9.0/MANIFEST.in
--rw-r--r--   0 subhashb   (501) staff       (20)      413 2022-02-12 19:48:13.000000 protean-0.9.0/Makefile
--rw-r--r--   0 subhashb   (501) staff       (20)    16337 2022-02-18 03:09:35.780384 protean-0.9.0/PKG-INFO
--rw-r--r--   0 subhashb   (501) staff       (20)     2157 2021-10-07 17:14:25.000000 protean-0.9.0/README.rst
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.491952 protean-0.9.0/ci/
--rwxr-xr-x   0 subhashb   (501) staff       (20)     2063 2022-02-12 19:48:13.000000 protean-0.9.0/ci/bootstrap.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1066 2022-02-12 19:48:13.000000 protean-0.9.0/docker-compose.yml
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.496335 protean-0.9.0/docs/
--rw-r--r--   0 subhashb   (501) staff       (20)      636 2021-08-06 23:09:47.000000 protean-0.9.0/docs/Makefile
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.497248 protean-0.9.0/docs/adapters/
--rw-r--r--   0 subhashb   (501) staff       (20)     1834 2022-02-12 19:48:13.000000 protean-0.9.0/docs/adapters/database.rst
--rw-r--r--   0 subhashb   (501) staff       (20)      485 2021-08-17 17:25:27.000000 protean-0.9.0/docs/api.rst
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.500223 protean-0.9.0/docs/community/
--rw-r--r--   0 subhashb   (501) staff       (20)       33 2021-08-09 17:30:41.000000 protean-0.9.0/docs/community/changelog.rst
--rw-r--r--   0 subhashb   (501) staff       (20)       39 2021-08-09 21:30:16.000000 protean-0.9.0/docs/community/code-of-conduct.rst
--rw-r--r--   0 subhashb   (501) staff       (20)       36 2021-08-09 21:30:37.000000 protean-0.9.0/docs/community/contributing.rst
--rw-r--r--   0 subhashb   (501) staff       (20)     1872 2022-02-18 02:30:54.000000 protean-0.9.0/docs/conf.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.502272 protean-0.9.0/docs/images/
--rw-r--r--   0 subhashb   (501) staff       (20)    32963 2021-08-16 21:03:49.000000 protean-0.9.0/docs/images/consuming-events.jpg
--rw-r--r--   0 subhashb   (501) staff       (20)    45503 2021-08-16 21:06:33.000000 protean-0.9.0/docs/images/raising-events.jpg
--rw-r--r--   0 subhashb   (501) staff       (20)     3473 2021-10-07 17:14:25.000000 protean-0.9.0/docs/index.rst
--rw-r--r--   0 subhashb   (501) staff       (20)      797 2021-08-06 23:09:47.000000 protean-0.9.0/docs/make.bat
--rw-r--r--   0 subhashb   (501) staff       (20)       11 2021-08-06 23:08:58.000000 protean-0.9.0/docs/requirements.txt
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.504613 protean-0.9.0/docs/static/
--rw-r--r--   0 subhashb   (501) staff       (20)       37 2021-08-16 19:58:19.000000 protean-0.9.0/docs/static/custom.css
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.516219 protean-0.9.0/docs/user/
--rw-r--r--   0 subhashb   (501) staff       (20)     2564 2021-08-12 17:19:36.000000 protean-0.9.0/docs/user/cli.rst
--rw-r--r--   0 subhashb   (501) staff       (20)     3814 2021-08-10 22:37:09.000000 protean-0.9.0/docs/user/composing-a-domain.rst
--rw-r--r--   0 subhashb   (501) staff       (20)    12237 2021-08-16 23:56:42.000000 protean-0.9.0/docs/user/config.rst
--rw-r--r--   0 subhashb   (501) staff       (20)    18905 2021-08-17 17:46:28.000000 protean-0.9.0/docs/user/domain-definition.rst
--rw-r--r--   0 subhashb   (501) staff       (20)    13694 2021-08-18 19:54:10.000000 protean-0.9.0/docs/user/entities-and-vos.rst
--rw-r--r--   0 subhashb   (501) staff       (20)    10510 2021-08-16 23:56:38.000000 protean-0.9.0/docs/user/eventing.rst
--rw-r--r--   0 subhashb   (501) staff       (20)    14638 2021-08-17 20:16:34.000000 protean-0.9.0/docs/user/fields.rst
--rw-r--r--   0 subhashb   (501) staff       (20)     2884 2021-08-09 18:46:28.000000 protean-0.9.0/docs/user/foreword.rst
--rw-r--r--   0 subhashb   (501) staff       (20)     2692 2021-08-10 17:21:01.000000 protean-0.9.0/docs/user/installation.rst
--rw-r--r--   0 subhashb   (501) staff       (20)     9088 2021-08-24 08:06:25.000000 protean-0.9.0/docs/user/persistence.rst
--rw-r--r--   0 subhashb   (501) staff       (20)     6060 2021-08-09 21:28:20.000000 protean-0.9.0/docs/user/quickstart.rst
--rw-r--r--   0 subhashb   (501) staff       (20)     1831 2021-08-31 16:03:14.000000 protean-0.9.0/docs/user/services.rst
--rw-r--r--   0 subhashb   (501) staff       (20)     1134 2022-02-18 03:09:35.781444 protean-0.9.0/setup.cfg
--rw-r--r--   0 subhashb   (501) staff       (20)     4293 2022-02-18 02:30:54.000000 protean-0.9.0/setup.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.459105 protean-0.9.0/src/
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.521586 protean-0.9.0/src/protean/
--rw-r--r--   0 subhashb   (501) staff       (20)      974 2022-02-18 02:30:54.000000 protean-0.9.0/src/protean/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)      361 2021-07-16 18:23:52.000000 protean-0.9.0/src/protean/__main__.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.525610 protean-0.9.0/src/protean/adapters/
--rw-r--r--   0 subhashb   (501) staff       (20)      647 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/adapters/__init__.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.527260 protean-0.9.0/src/protean/adapters/broker/
--rw-r--r--   0 subhashb   (501) staff       (20)     3438 2022-02-17 03:12:21.000000 protean-0.9.0/src/protean/adapters/broker/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)     4095 2022-02-18 00:49:21.000000 protean-0.9.0/src/protean/adapters/broker/celery.py
--rw-r--r--   0 subhashb   (501) staff       (20)      898 2022-02-17 03:17:46.000000 protean-0.9.0/src/protean/adapters/broker/inline.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1026 2022-02-17 03:17:46.000000 protean-0.9.0/src/protean/adapters/broker/redis.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.528956 protean-0.9.0/src/protean/adapters/cache/
--rw-r--r--   0 subhashb   (501) staff       (20)     2955 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/adapters/cache/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)     5457 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/adapters/cache/memory.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2859 2021-09-23 17:39:41.000000 protean-0.9.0/src/protean/adapters/cache/redis.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.530616 protean-0.9.0/src/protean/adapters/email/
--rw-r--r--   0 subhashb   (501) staff       (20)     2068 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/adapters/email/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)      507 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/adapters/email/dummy.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1658 2022-02-18 02:27:14.000000 protean-0.9.0/src/protean/adapters/email/sendgrid.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.532277 protean-0.9.0/src/protean/adapters/event_store/
--rw-r--r--   0 subhashb   (501) staff       (20)     4790 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/adapters/event_store/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)     3968 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/adapters/event_store/memory.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2320 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/adapters/event_store/message_db.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.534165 protean-0.9.0/src/protean/adapters/repository/
--rw-r--r--   0 subhashb   (501) staff       (20)     6539 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/adapters/repository/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)    21821 2022-02-18 02:14:54.000000 protean-0.9.0/src/protean/adapters/repository/elasticsearch.py
--rw-r--r--   0 subhashb   (501) staff       (20)    22123 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/adapters/repository/memory.py
--rw-r--r--   0 subhashb   (501) staff       (20)    27412 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/adapters/repository/sqlalchemy.py
--rw-r--r--   0 subhashb   (501) staff       (20)     8108 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/cli.py
--rw-r--r--   0 subhashb   (501) staff       (20)    12182 2022-02-18 02:24:17.000000 protean-0.9.0/src/protean/container.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.544057 protean-0.9.0/src/protean/core/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2021-09-23 17:39:41.000000 protean-0.9.0/src/protean/core/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2105 2022-02-18 02:23:17.000000 protean-0.9.0/src/protean/core/aggregate.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1375 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/core/application_service.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1932 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/core/command.py
--rw-r--r--   0 subhashb   (501) staff       (20)     3102 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/core/command_handler.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1003 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/core/domain_service.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2454 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/core/email.py
--rw-r--r--   0 subhashb   (501) staff       (20)    17436 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/core/entity.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1690 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/core/event.py
--rw-r--r--   0 subhashb   (501) staff       (20)     3317 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/core/event_handler.py
--rw-r--r--   0 subhashb   (501) staff       (20)     6805 2022-02-18 02:23:17.000000 protean-0.9.0/src/protean/core/event_sourced_aggregate.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2606 2022-02-18 02:24:26.000000 protean-0.9.0/src/protean/core/event_sourced_repository.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2311 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/core/model.py
--rw-r--r--   0 subhashb   (501) staff       (20)    11988 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/core/queryset.py
--rw-r--r--   0 subhashb   (501) staff       (20)    10028 2022-02-18 02:24:52.000000 protean-0.9.0/src/protean/core/repository.py
--rw-r--r--   0 subhashb   (501) staff       (20)     7222 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/core/serializer.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1735 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/core/subscriber.py
--rw-r--r--   0 subhashb   (501) staff       (20)     5792 2022-02-18 02:24:59.000000 protean-0.9.0/src/protean/core/unit_of_work.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1376 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/core/value_object.py
--rw-r--r--   0 subhashb   (501) staff       (20)     4687 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/core/view.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.546452 protean-0.9.0/src/protean/domain/
--rw-r--r--   0 subhashb   (501) staff       (20)    30182 2022-02-17 02:58:02.000000 protean-0.9.0/src/protean/domain/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)    10890 2021-08-11 01:11:51.000000 protean-0.9.0/src/protean/domain/config.py
--rw-r--r--   0 subhashb   (501) staff       (20)     3782 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/domain/context.py
--rw-r--r--   0 subhashb   (501) staff       (20)     3339 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/domain/helpers.py
--rw-r--r--   0 subhashb   (501) staff       (20)     4116 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/domain/registry.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2569 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/exceptions.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.550312 protean-0.9.0/src/protean/fields/
--rw-r--r--   0 subhashb   (501) staff       (20)      322 2021-12-02 17:46:40.000000 protean-0.9.0/src/protean/fields/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)    17211 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/fields/association.py
--rw-r--r--   0 subhashb   (501) staff       (20)     7702 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/fields/base.py
--rw-r--r--   0 subhashb   (501) staff       (20)    12545 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/fields/basic.py
--rw-r--r--   0 subhashb   (501) staff       (20)     6391 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/fields/embedded.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2292 2021-09-23 17:39:41.000000 protean-0.9.0/src/protean/fields/mixins.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2892 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/fields/validators.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1084 2021-08-24 17:57:24.000000 protean-0.9.0/src/protean/globals.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.553614 protean-0.9.0/src/protean/port/
--rw-r--r--   0 subhashb   (501) staff       (20)      160 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/port/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2597 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/port/broker.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2549 2021-08-12 17:03:37.000000 protean-0.9.0/src/protean/port/cache.py
--rw-r--r--   0 subhashb   (501) staff       (20)    24789 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/port/dao.py
--rw-r--r--   0 subhashb   (501) staff       (20)     5924 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/port/event_store.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2814 2021-07-16 18:24:42.000000 protean-0.9.0/src/protean/port/provider.py
--rw-r--r--   0 subhashb   (501) staff       (20)     3165 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/reflection.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.554856 protean-0.9.0/src/protean/server/
--rw-r--r--   0 subhashb   (501) staff       (20)       27 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/server/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)     4713 2022-02-18 02:25:30.000000 protean-0.9.0/src/protean/server/engine.py
--rw-r--r--   0 subhashb   (501) staff       (20)     4525 2022-02-18 02:25:06.000000 protean-0.9.0/src/protean/server/subscription.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.556757 protean-0.9.0/src/protean/utils/
--rw-r--r--   0 subhashb   (501) staff       (20)     4893 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/utils/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1153 2021-08-03 23:51:36.000000 protean-0.9.0/src/protean/utils/importlib.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2882 2021-07-16 18:24:42.000000 protean-0.9.0/src/protean/utils/inflection.py
--rw-r--r--   0 subhashb   (501) staff       (20)     9397 2022-02-18 02:30:01.000000 protean-0.9.0/src/protean/utils/mixins.py
--rw-r--r--   0 subhashb   (501) staff       (20)     8983 2022-02-12 19:48:13.000000 protean-0.9.0/src/protean/utils/query.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.525241 protean-0.9.0/src/protean.egg-info/
--rw-r--r--   0 subhashb   (501) staff       (20)    16337 2022-02-18 03:09:35.000000 protean-0.9.0/src/protean.egg-info/PKG-INFO
--rw-r--r--   0 subhashb   (501) staff       (20)    15852 2022-02-18 03:09:35.000000 protean-0.9.0/src/protean.egg-info/SOURCES.txt
--rw-r--r--   0 subhashb   (501) staff       (20)        1 2022-02-18 03:09:35.000000 protean-0.9.0/src/protean.egg-info/dependency_links.txt
--rw-r--r--   0 subhashb   (501) staff       (20)       46 2022-02-18 03:09:35.000000 protean-0.9.0/src/protean.egg-info/entry_points.txt
--rw-r--r--   0 subhashb   (501) staff       (20)        1 2022-02-18 03:09:35.000000 protean-0.9.0/src/protean.egg-info/not-zip-safe
--rw-r--r--   0 subhashb   (501) staff       (20)     2887 2022-02-18 03:09:35.000000 protean-0.9.0/src/protean.egg-info/requires.txt
--rw-r--r--   0 subhashb   (501) staff       (20)        8 2022-02-18 03:09:35.000000 protean-0.9.0/src/protean.egg-info/top_level.txt
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.562867 protean-0.9.0/tests/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-04-06 03:53:33.000000 protean-0.9.0/tests/__init__.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.563407 protean-0.9.0/tests/adapters/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2020-09-28 21:08:18.000000 protean-0.9.0/tests/adapters/__init__.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.462613 protean-0.9.0/tests/adapters/broker/
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.566684 protean-0.9.0/tests/adapters/broker/celery_broker/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2020-09-22 16:41:47.000000 protean-0.9.0/tests/adapters/broker/celery_broker/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1867 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/broker/celery_broker/config.py
--rw-r--r--   0 subhashb   (501) staff       (20)      809 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/broker/celery_broker/conftest.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1529 2021-09-23 17:39:41.000000 protean-0.9.0/tests/adapters/broker/celery_broker/elements.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1334 2021-08-10 16:05:35.000000 protean-0.9.0/tests/adapters/broker/celery_broker/test_subscriber.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1177 2021-08-10 16:05:35.000000 protean-0.9.0/tests/adapters/broker/celery_broker/tests.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.569059 protean-0.9.0/tests/adapters/broker/redis_broker/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2021-08-03 23:51:36.000000 protean-0.9.0/tests/adapters/broker/redis_broker/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1663 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/broker/redis_broker/config.py
--rw-r--r--   0 subhashb   (501) staff       (20)      700 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/broker/redis_broker/conftest.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1577 2022-02-17 02:25:28.000000 protean-0.9.0/tests/adapters/broker/redis_broker/elements.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2845 2022-02-17 03:17:46.000000 protean-0.9.0/tests/adapters/broker/redis_broker/tests.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.462953 protean-0.9.0/tests/adapters/cache/
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.570999 protean-0.9.0/tests/adapters/cache/redis_cache/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2021-04-21 23:33:04.000000 protean-0.9.0/tests/adapters/cache/redis_cache/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)      755 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/cache/redis_cache/config.py
--rw-r--r--   0 subhashb   (501) staff       (20)      540 2021-07-16 18:31:32.000000 protean-0.9.0/tests/adapters/cache/redis_cache/conftest.py
--rw-r--r--   0 subhashb   (501) staff       (20)     7555 2021-09-23 17:39:41.000000 protean-0.9.0/tests/adapters/cache/redis_cache/tests.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.463236 protean-0.9.0/tests/adapters/email/
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.573330 protean-0.9.0/tests/adapters/email/sendgrid_email/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2020-09-22 16:41:47.000000 protean-0.9.0/tests/adapters/email/sendgrid_email/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1361 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/email/sendgrid_email/config.py
--rw-r--r--   0 subhashb   (501) staff       (20)      550 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/email/sendgrid_email/conftest.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2010 2021-09-23 17:39:41.000000 protean-0.9.0/tests/adapters/email/sendgrid_email/elements.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1292 2021-08-10 16:05:35.000000 protean-0.9.0/tests/adapters/email/sendgrid_email/tests.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.463911 protean-0.9.0/tests/adapters/event_store/
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.575841 protean-0.9.0/tests/adapters/event_store/memory_event_store/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/event_store/memory_event_store/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)      361 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/event_store/memory_event_store/test_data_reset.py
--rw-r--r--   0 subhashb   (501) staff       (20)      420 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/event_store/memory_event_store/test_initialization.py
--rw-r--r--   0 subhashb   (501) staff       (20)      427 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/event_store/memory_event_store/test_memory_message_repository.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2450 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/event_store/memory_event_store/test_reading_from_memory_event_store.py
--rw-r--r--   0 subhashb   (501) staff       (20)      977 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/event_store/memory_event_store/test_writing_to_memory_event_store.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.578303 protean-0.9.0/tests/adapters/event_store/message_db_event_store/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/event_store/message_db_event_store/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)      620 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/event_store/message_db_event_store/config.py
--rw-r--r--   0 subhashb   (501) staff       (20)      530 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/event_store/message_db_event_store/conftest.py
--rw-r--r--   0 subhashb   (501) staff       (20)     4457 2022-02-18 02:28:10.000000 protean-0.9.0/tests/adapters/event_store/message_db_event_store/tests.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.465262 protean-0.9.0/tests/adapters/model/
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.579724 protean-0.9.0/tests/adapters/model/dict_model/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2020-09-22 16:41:47.000000 protean-0.9.0/tests/adapters/model/dict_model/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1499 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/model/dict_model/elements.py
--rw-r--r--   0 subhashb   (501) staff       (20)     4104 2022-01-14 02:23:09.000000 protean-0.9.0/tests/adapters/model/dict_model/tests.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.582307 protean-0.9.0/tests/adapters/model/elasticsearch_model/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2020-09-22 16:41:47.000000 protean-0.9.0/tests/adapters/model/elasticsearch_model/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)      738 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/model/elasticsearch_model/config.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1252 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/model/elasticsearch_model/conftest.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1752 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/model/elasticsearch_model/elements.py
--rw-r--r--   0 subhashb   (501) staff       (20)    13709 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/model/elasticsearch_model/tests.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.582721 protean-0.9.0/tests/adapters/model/sqlalchemy_model/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2020-09-22 16:41:47.000000 protean-0.9.0/tests/adapters/model/sqlalchemy_model/__init__.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.587491 protean-0.9.0/tests/adapters/model/sqlalchemy_model/postgresql/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2020-09-22 16:41:47.000000 protean-0.9.0/tests/adapters/model/sqlalchemy_model/postgresql/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)      764 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/model/sqlalchemy_model/postgresql/config.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2144 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/model/sqlalchemy_model/postgresql/conftest.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1737 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/model/sqlalchemy_model/postgresql/elements.py
--rw-r--r--   0 subhashb   (501) staff       (20)     4809 2022-01-14 02:23:09.000000 protean-0.9.0/tests/adapters/model/sqlalchemy_model/postgresql/test_array_datatype.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2464 2022-01-14 02:23:09.000000 protean-0.9.0/tests/adapters/model/sqlalchemy_model/postgresql/test_json_datatype.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2528 2022-01-14 02:23:09.000000 protean-0.9.0/tests/adapters/model/sqlalchemy_model/postgresql/test_list_datatype.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1946 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/model/sqlalchemy_model/postgresql/test_lookups.py
--rw-r--r--   0 subhashb   (501) staff       (20)     4486 2022-01-14 02:23:09.000000 protean-0.9.0/tests/adapters/model/sqlalchemy_model/postgresql/test_model.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.591442 protean-0.9.0/tests/adapters/model/sqlalchemy_model/sqlite/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2020-09-22 16:41:47.000000 protean-0.9.0/tests/adapters/model/sqlalchemy_model/sqlite/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)      725 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/model/sqlalchemy_model/sqlite/config.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1704 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/model/sqlalchemy_model/sqlite/conftest.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1438 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/model/sqlalchemy_model/sqlite/elements.py
--rw-r--r--   0 subhashb   (501) staff       (20)     3091 2022-01-14 02:23:09.000000 protean-0.9.0/tests/adapters/model/sqlalchemy_model/sqlite/test_array_datatype.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1057 2022-01-14 02:23:09.000000 protean-0.9.0/tests/adapters/model/sqlalchemy_model/sqlite/test_json_datatype.py
--rw-r--r--   0 subhashb   (501) staff       (20)     4408 2022-01-14 02:23:09.000000 protean-0.9.0/tests/adapters/model/sqlalchemy_model/sqlite/test_model.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.592106 protean-0.9.0/tests/adapters/repository/
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.599167 protean-0.9.0/tests/adapters/repository/elasticsearch_repo/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2020-09-22 16:41:47.000000 protean-0.9.0/tests/adapters/repository/elasticsearch_repo/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)      738 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/repository/elasticsearch_repo/config.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1031 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/repository/elasticsearch_repo/conftest.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1336 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/repository/elasticsearch_repo/elements.py
--rw-r--r--   0 subhashb   (501) staff       (20)    36663 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/repository/elasticsearch_repo/test_dao.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1861 2021-07-16 18:24:10.000000 protean-0.9.0/tests/adapters/repository/elasticsearch_repo/test_lookup.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2951 2022-01-14 02:23:09.000000 protean-0.9.0/tests/adapters/repository/elasticsearch_repo/test_provider.py
--rw-r--r--   0 subhashb   (501) staff       (20)     3008 2022-01-14 02:23:09.000000 protean-0.9.0/tests/adapters/repository/elasticsearch_repo/test_query.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1293 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/repository/elasticsearch_repo/test_repo.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.601164 protean-0.9.0/tests/adapters/repository/memory/
--rw-r--r--   0 subhashb   (501) staff       (20)     1223 2022-01-14 02:23:09.000000 protean-0.9.0/tests/adapters/repository/memory/test_any_operator.py
--rw-r--r--   0 subhashb   (501) staff       (20)      822 2022-01-14 02:23:09.000000 protean-0.9.0/tests/adapters/repository/memory/test_in_operator.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1420 2021-07-16 18:35:06.000000 protean-0.9.0/tests/adapters/repository/memory/test_lookups.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1929 2022-01-14 02:23:09.000000 protean-0.9.0/tests/adapters/repository/memory/test_sorting_on_none_values.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.601704 protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2020-09-22 16:41:47.000000 protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/__init__.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.607570 protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/postgresql/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2020-09-22 16:41:47.000000 protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/postgresql/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)      765 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/postgresql/config.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1661 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/postgresql/conftest.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1374 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/postgresql/elements.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1639 2022-01-14 02:23:09.000000 protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/postgresql/test_associations.py
--rw-r--r--   0 subhashb   (501) staff       (20)    36584 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/postgresql/test_dao.py
--rw-r--r--   0 subhashb   (501) staff       (20)      798 2022-01-14 02:23:09.000000 protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/postgresql/test_persistence.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2961 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/postgresql/test_provider.py
--rw-r--r--   0 subhashb   (501) staff       (20)     6405 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/postgresql/test_transactions.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.612027 protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/sqlite/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2020-09-22 16:41:47.000000 protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/sqlite/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)      725 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/sqlite/config.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1274 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/sqlite/conftest.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1336 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/sqlite/elements.py
--rw-r--r--   0 subhashb   (501) staff       (20)    34775 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/sqlite/test_dao.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2987 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/sqlite/test_provider.py
--rw-r--r--   0 subhashb   (501) staff       (20)     6632 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/sqlite/test_transactions.py
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2020-09-22 16:41:47.000000 protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/sqlite/tests.py
--rw-r--r--   0 subhashb   (501) staff       (20)     4143 2022-02-12 19:48:13.000000 protean-0.9.0/tests/adapters/repository/test_generic.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.623890 protean-0.9.0/tests/aggregate/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-05-30 19:04:30.000000 protean-0.9.0/tests/aggregate/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)      866 2021-09-23 17:39:41.000000 protean-0.9.0/tests/aggregate/aggregate_elements.py
--rw-r--r--   0 subhashb   (501) staff       (20)      467 2021-09-23 17:39:41.000000 protean-0.9.0/tests/aggregate/aggregate_elements_with_value_objects.py
--rw-r--r--   0 subhashb   (501) staff       (20)     5301 2021-09-23 17:39:41.000000 protean-0.9.0/tests/aggregate/elements.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1506 2022-02-12 19:48:13.000000 protean-0.9.0/tests/aggregate/test_aggregate_abstraction.py
--rw-r--r--   0 subhashb   (501) staff       (20)     9500 2022-02-12 19:48:13.000000 protean-0.9.0/tests/aggregate/test_aggregate_association.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2024 2022-02-12 19:48:13.000000 protean-0.9.0/tests/aggregate/test_aggregate_events.py
--rw-r--r--   0 subhashb   (501) staff       (20)     6236 2022-02-12 19:48:13.000000 protean-0.9.0/tests/aggregate/test_aggregate_initialization.py
--rw-r--r--   0 subhashb   (501) staff       (20)     5602 2022-02-12 19:48:13.000000 protean-0.9.0/tests/aggregate/test_aggregate_properties.py
--rw-r--r--   0 subhashb   (501) staff       (20)    10102 2022-02-12 19:48:13.000000 protean-0.9.0/tests/aggregate/test_aggregate_reference_field.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1135 2021-09-23 17:39:41.000000 protean-0.9.0/tests/aggregate/test_aggregate_registration.py
--rw-r--r--   0 subhashb   (501) staff       (20)     4093 2022-01-14 02:23:09.000000 protean-0.9.0/tests/aggregate/test_aggregate_state.py
--rw-r--r--   0 subhashb   (501) staff       (20)     3945 2022-01-14 02:23:09.000000 protean-0.9.0/tests/aggregate/test_aggregates_with_entities.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1726 2021-07-16 18:27:32.000000 protean-0.9.0/tests/aggregate/test_aggregates_with_value_objects.py
--rw-r--r--   0 subhashb   (501) staff       (20)     5378 2022-02-12 19:48:13.000000 protean-0.9.0/tests/aggregate/test_as_dict.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.627524 protean-0.9.0/tests/application_service/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-06-25 14:29:25.000000 protean-0.9.0/tests/application_service/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)      189 2021-09-23 17:39:41.000000 protean-0.9.0/tests/application_service/elements.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1224 2021-09-23 17:39:41.000000 protean-0.9.0/tests/application_service/tests.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.628478 protean-0.9.0/tests/cache/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2021-04-21 23:33:04.000000 protean-0.9.0/tests/cache/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)     7503 2021-10-02 16:15:04.000000 protean-0.9.0/tests/cache/tests.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.630574 protean-0.9.0/tests/command/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2022-02-12 19:48:13.000000 protean-0.9.0/tests/command/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2755 2022-02-18 02:28:05.000000 protean-0.9.0/tests/command/test_automatic_stream_association.py
--rw-r--r--   0 subhashb   (501) staff       (20)      636 2022-02-12 19:48:13.000000 protean-0.9.0/tests/command/test_command_identity.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2422 2022-02-18 02:28:47.000000 protean-0.9.0/tests/command/test_command_meta.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.634749 protean-0.9.0/tests/command_handler/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2022-02-12 19:48:13.000000 protean-0.9.0/tests/command_handler/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1046 2022-02-12 19:48:13.000000 protean-0.9.0/tests/command_handler/test_command_handler_options.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1167 2022-02-12 19:48:13.000000 protean-0.9.0/tests/command_handler/test_command_handler_registration.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2717 2022-02-12 19:48:13.000000 protean-0.9.0/tests/command_handler/test_handle_decorator_in_command_handlers.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1432 2022-02-17 03:03:33.000000 protean-0.9.0/tests/command_handler/test_inline_command_processing.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2456 2022-02-12 19:48:13.000000 protean-0.9.0/tests/command_handler/test_retrieving_handlers_by_command.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1246 2022-02-12 19:48:13.000000 protean-0.9.0/tests/command_handler/test_uow_around_command_handlers.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2104 2022-02-12 19:48:13.000000 protean-0.9.0/tests/config.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.637117 protean-0.9.0/tests/configuration/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-06-08 01:24:59.000000 protean-0.9.0/tests/configuration/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)       54 2019-06-08 01:24:59.000000 protean-0.9.0/tests/configuration/config.json
--rw-r--r--   0 subhashb   (501) staff       (20)     6056 2022-02-12 19:48:13.000000 protean-0.9.0/tests/configuration/tests.py
--rw-r--r--   0 subhashb   (501) staff       (20)     6778 2022-02-12 19:48:13.000000 protean-0.9.0/tests/conftest.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.637611 protean-0.9.0/tests/container/
--rw-r--r--   0 subhashb   (501) staff       (20)     1370 2022-02-12 19:48:13.000000 protean-0.9.0/tests/container/test_options.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.640523 protean-0.9.0/tests/context/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-06-08 01:24:59.000000 protean-0.9.0/tests/context/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)     4253 2022-02-12 19:48:13.000000 protean-0.9.0/tests/context/tests.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.645684 protean-0.9.0/tests/dao/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-05-30 19:04:30.000000 protean-0.9.0/tests/dao/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)      653 2021-09-23 17:39:41.000000 protean-0.9.0/tests/dao/elements.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2322 2022-01-14 02:23:09.000000 protean-0.9.0/tests/dao/test_basics.py
--rw-r--r--   0 subhashb   (501) staff       (20)     5943 2022-02-12 19:48:13.000000 protean-0.9.0/tests/dao/test_delete.py
--rw-r--r--   0 subhashb   (501) staff       (20)      105 2019-09-27 16:08:17.000000 protean-0.9.0/tests/dao/test_lookup.py
--rw-r--r--   0 subhashb   (501) staff       (20)    14830 2022-02-12 19:48:13.000000 protean-0.9.0/tests/dao/test_retrieval.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1767 2022-02-12 19:48:13.000000 protean-0.9.0/tests/dao/test_save.py
--rw-r--r--   0 subhashb   (501) staff       (20)     7248 2022-02-12 19:48:13.000000 protean-0.9.0/tests/dao/test_update.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2245 2022-02-12 19:48:13.000000 protean-0.9.0/tests/dao/test_validations.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.650733 protean-0.9.0/tests/domain/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-05-30 19:04:30.000000 protean-0.9.0/tests/domain/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)      495 2021-09-23 17:39:41.000000 protean-0.9.0/tests/domain/elements.py
--rw-r--r--   0 subhashb   (501) staff       (20)      529 2022-02-12 19:48:13.000000 protean-0.9.0/tests/domain/test_config_immutability.py
--rw-r--r--   0 subhashb   (501) staff       (20)     9543 2022-02-12 19:48:13.000000 protean-0.9.0/tests/domain/tests.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.652272 protean-0.9.0/tests/domain_service/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-06-25 18:11:26.000000 protean-0.9.0/tests/domain_service/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)      166 2021-09-23 17:39:41.000000 protean-0.9.0/tests/domain_service/elements.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1125 2021-09-23 17:39:41.000000 protean-0.9.0/tests/domain_service/tests.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.657359 protean-0.9.0/tests/email_provider/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2020-01-10 17:02:21.000000 protean-0.9.0/tests/email_provider/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2083 2021-09-23 17:39:41.000000 protean-0.9.0/tests/email_provider/elements.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1856 2022-02-12 19:48:13.000000 protean-0.9.0/tests/email_provider/tests.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.661507 protean-0.9.0/tests/entity/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-05-30 19:04:30.000000 protean-0.9.0/tests/entity/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2756 2021-09-23 17:39:41.000000 protean-0.9.0/tests/entity/elements.py
--rw-r--r--   0 subhashb   (501) staff       (20)     5848 2022-02-12 19:48:13.000000 protean-0.9.0/tests/entity/test_entity.py
--rw-r--r--   0 subhashb   (501) staff       (20)     3459 2022-02-12 19:48:13.000000 protean-0.9.0/tests/entity/test_entity_meta.py
--rw-r--r--   0 subhashb   (501) staff       (20)     5965 2022-02-12 19:48:13.000000 protean-0.9.0/tests/entity/test_entity_properties.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1841 2021-09-23 17:39:41.000000 protean-0.9.0/tests/entity/test_entity_registration.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1440 2021-09-23 17:39:41.000000 protean-0.9.0/tests/entity/test_fields.py
--rw-r--r--   0 subhashb   (501) staff       (20)      700 2021-08-03 23:51:36.000000 protean-0.9.0/tests/entity/test_lifecycle_methods.py
--rw-r--r--   0 subhashb   (501) staff       (20)      555 2021-09-23 17:39:41.000000 protean-0.9.0/tests/entity/test_temp.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.666360 protean-0.9.0/tests/event/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-07-01 16:19:36.000000 protean-0.9.0/tests/event/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1508 2021-09-23 17:39:41.000000 protean-0.9.0/tests/event/elements.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2883 2022-02-18 02:28:05.000000 protean-0.9.0/tests/event/test_automatic_stream_association.py
--rw-r--r--   0 subhashb   (501) staff       (20)      636 2022-02-12 19:48:13.000000 protean-0.9.0/tests/event/test_event_identity.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1597 2022-02-18 02:29:20.000000 protean-0.9.0/tests/event/test_event_meta.py
--rw-r--r--   0 subhashb   (501) staff       (20)      814 2022-02-12 19:48:13.000000 protean-0.9.0/tests/event/test_raising_events.py
--rw-r--r--   0 subhashb   (501) staff       (20)      872 2021-08-10 16:05:35.000000 protean-0.9.0/tests/event/test_serialization.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2585 2022-02-17 00:23:17.000000 protean-0.9.0/tests/event/tests.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.678396 protean-0.9.0/tests/event_handler/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2022-02-12 19:48:13.000000 protean-0.9.0/tests/event_handler/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1023 2022-02-12 19:48:13.000000 protean-0.9.0/tests/event_handler/test_any_event_handler.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2401 2022-02-12 19:48:13.000000 protean-0.9.0/tests/event_handler/test_event_handler_options.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1124 2022-02-12 19:48:13.000000 protean-0.9.0/tests/event_handler/test_event_handler_registration.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2935 2022-02-12 19:48:13.000000 protean-0.9.0/tests/event_handler/test_handle_decorator_in_event_handlers.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2834 2022-02-12 19:48:13.000000 protean-0.9.0/tests/event_handler/test_retrieving_handlers_by_event.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1258 2022-02-12 19:48:13.000000 protean-0.9.0/tests/event_handler/test_uow_around_event_handlers.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.683756 protean-0.9.0/tests/event_sourced_aggregates/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2022-02-12 19:48:13.000000 protean-0.9.0/tests/event_sourced_aggregates/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)     3063 2022-02-18 02:28:16.000000 protean-0.9.0/tests/event_sourced_aggregates/test_applying_events.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2533 2022-02-12 19:48:13.000000 protean-0.9.0/tests/event_sourced_aggregates/test_event_association_with_aggregate.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1551 2022-02-12 19:48:13.000000 protean-0.9.0/tests/event_sourced_aggregates/test_event_sourced_aggregate_options.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1095 2022-02-12 19:48:13.000000 protean-0.9.0/tests/event_sourced_aggregates/test_event_sourced_aggregate_registration.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2487 2022-02-12 19:48:13.000000 protean-0.9.0/tests/event_sourced_aggregates/test_expected_version_error.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2295 2022-02-12 19:48:13.000000 protean-0.9.0/tests/event_sourced_aggregates/test_raising_events_from_within_aggregates.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.685905 protean-0.9.0/tests/event_sourced_repository/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2022-02-12 19:48:13.000000 protean-0.9.0/tests/event_sourced_repository/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)     4841 2022-02-12 19:48:13.000000 protean-0.9.0/tests/event_sourced_repository/test_loading_aggregates.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1009 2022-02-12 19:48:13.000000 protean-0.9.0/tests/event_sourced_repository/test_retrieving_event_sourced_repository.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.695250 protean-0.9.0/tests/event_store/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2022-02-12 19:48:13.000000 protean-0.9.0/tests/event_store/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2334 2022-02-12 19:48:13.000000 protean-0.9.0/tests/event_store/test_appending_aggregate_events.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1517 2022-02-18 02:28:29.000000 protean-0.9.0/tests/event_store/test_appending_commands.py
--rw-r--r--   0 subhashb   (501) staff       (20)      840 2022-02-12 19:48:13.000000 protean-0.9.0/tests/event_store/test_appending_events.py
--rw-r--r--   0 subhashb   (501) staff       (20)      507 2022-02-12 19:48:13.000000 protean-0.9.0/tests/event_store/test_deriving_category.py
--rw-r--r--   0 subhashb   (501) staff       (20)      495 2022-02-12 19:48:13.000000 protean-0.9.0/tests/event_store/test_event_store_adapter_initialization.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2211 2022-02-12 19:48:13.000000 protean-0.9.0/tests/event_store/test_reading_all_streams.py
--rw-r--r--   0 subhashb   (501) staff       (20)     5178 2022-02-12 19:48:13.000000 protean-0.9.0/tests/event_store/test_reading_messages.py
--rw-r--r--   0 subhashb   (501) staff       (20)     5091 2022-02-12 19:48:13.000000 protean-0.9.0/tests/event_store/test_snapshotting.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2005 2022-02-12 19:48:13.000000 protean-0.9.0/tests/event_store/test_streams_initialization.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.702715 protean-0.9.0/tests/field/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-05-31 17:44:59.000000 protean-0.9.0/tests/field/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)      750 2021-09-23 17:39:41.000000 protean-0.9.0/tests/field/elements.py
--rw-r--r--   0 subhashb   (501) staff       (20)      865 2022-02-12 19:48:13.000000 protean-0.9.0/tests/field/test_associations.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2473 2022-02-18 02:28:05.000000 protean-0.9.0/tests/field/test_auto.py
--rw-r--r--   0 subhashb   (501) staff       (20)    11247 2022-02-18 02:28:05.000000 protean-0.9.0/tests/field/test_field_types.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2554 2021-09-23 17:39:41.000000 protean-0.9.0/tests/field/test_field_validators.py
--rw-r--r--   0 subhashb   (501) staff       (20)      525 2022-02-12 19:48:13.000000 protean-0.9.0/tests/field/test_identifier.py
--rw-r--r--   0 subhashb   (501) staff       (20)      751 2022-02-12 19:48:13.000000 protean-0.9.0/tests/field/test_reference.py
--rw-r--r--   0 subhashb   (501) staff       (20)     3745 2022-02-12 19:48:13.000000 protean-0.9.0/tests/field/tests.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.708256 protean-0.9.0/tests/identity/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-09-04 22:52:17.000000 protean-0.9.0/tests/identity/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)      742 2022-02-12 19:48:13.000000 protean-0.9.0/tests/identity/config_int.py
--rw-r--r--   0 subhashb   (501) staff       (20)      760 2022-02-12 19:48:13.000000 protean-0.9.0/tests/identity/config_string.py
--rw-r--r--   0 subhashb   (501) staff       (20)      758 2022-02-12 19:48:13.000000 protean-0.9.0/tests/identity/config_uuid.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1335 2022-02-12 19:48:13.000000 protean-0.9.0/tests/identity/conftest.py
--rw-r--r--   0 subhashb   (501) staff       (20)      245 2021-09-23 17:39:41.000000 protean-0.9.0/tests/identity/elements.py
--rw-r--r--   0 subhashb   (501) staff       (20)      792 2021-07-16 18:27:32.000000 protean-0.9.0/tests/identity/tests.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.710448 protean-0.9.0/tests/message/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2022-02-12 19:48:13.000000 protean-0.9.0/tests/message/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2007 2022-02-12 19:48:13.000000 protean-0.9.0/tests/message/test_message_to_object.py
--rw-r--r--   0 subhashb   (501) staff       (20)     5169 2022-02-16 22:46:36.000000 protean-0.9.0/tests/message/test_object_to_message.py
--rw-r--r--   0 subhashb   (501) staff       (20)     3721 2022-02-18 02:27:37.000000 protean-0.9.0/tests/message/test_origin_stream_name_in_metadata.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.711801 protean-0.9.0/tests/provider/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-05-31 17:44:59.000000 protean-0.9.0/tests/provider/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)      412 2021-09-23 17:39:41.000000 protean-0.9.0/tests/provider/elements.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2858 2022-01-14 02:23:09.000000 protean-0.9.0/tests/provider/tests.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.718323 protean-0.9.0/tests/query/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-05-31 17:44:59.000000 protean-0.9.0/tests/query/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)      245 2021-09-23 17:39:41.000000 protean-0.9.0/tests/query/elements.py
--rw-r--r--   0 subhashb   (501) staff       (20)     4261 2022-01-14 02:23:09.000000 protean-0.9.0/tests/query/test_conjunctions.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2101 2022-02-12 19:48:13.000000 protean-0.9.0/tests/query/test_q.py
--rw-r--r--   0 subhashb   (501) staff       (20)    26398 2022-02-18 02:29:12.000000 protean-0.9.0/tests/query/test_queryset.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.719425 protean-0.9.0/tests/reflection/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2022-02-12 19:48:13.000000 protean-0.9.0/tests/reflection/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)      873 2022-02-12 19:48:13.000000 protean-0.9.0/tests/reflection/test_has_id_field.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.730614 protean-0.9.0/tests/repository/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-05-30 19:04:30.000000 protean-0.9.0/tests/repository/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)      865 2021-09-23 17:39:41.000000 protean-0.9.0/tests/repository/child_entities.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1200 2022-02-12 19:48:13.000000 protean-0.9.0/tests/repository/elements.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1947 2022-02-12 19:48:13.000000 protean-0.9.0/tests/repository/test_aggregate_persistence.py
--rw-r--r--   0 subhashb   (501) staff       (20)     5572 2022-01-14 02:23:09.000000 protean-0.9.0/tests/repository/test_child_persistence.py
--rw-r--r--   0 subhashb   (501) staff       (20)     4641 2022-01-14 02:23:09.000000 protean-0.9.0/tests/repository/test_providers.py
--rw-r--r--   0 subhashb   (501) staff       (20)     5739 2022-01-14 02:23:09.000000 protean-0.9.0/tests/repository/test_repository_registration.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1661 2022-01-14 02:23:09.000000 protean-0.9.0/tests/repository/test_resultset.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1604 2022-02-12 19:48:13.000000 protean-0.9.0/tests/repository/test_tracking_seen_objects.py
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2022-02-12 19:48:13.000000 protean-0.9.0/tests/repository/test_writing_events_in_seen_objects.py
--rw-r--r--   0 subhashb   (501) staff       (20)      880 2022-02-12 19:48:13.000000 protean-0.9.0/tests/repository/tests.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.732597 protean-0.9.0/tests/serializer/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-07-13 06:22:37.000000 protean-0.9.0/tests/serializer/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)      336 2021-09-23 17:39:41.000000 protean-0.9.0/tests/serializer/elements.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1706 2022-02-12 19:48:13.000000 protean-0.9.0/tests/serializer/tests.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.743855 protean-0.9.0/tests/server/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2022-02-12 19:48:13.000000 protean-0.9.0/tests/server/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1073 2022-02-12 19:48:13.000000 protean-0.9.0/tests/server/dummy_domain.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1582 2022-02-12 19:48:13.000000 protean-0.9.0/tests/server/test_any_event_handler.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1281 2022-02-12 19:48:13.000000 protean-0.9.0/tests/server/test_command_handler_subscription.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1481 2022-02-12 19:48:13.000000 protean-0.9.0/tests/server/test_command_handling.py
--rw-r--r--   0 subhashb   (501) staff       (20)      719 2022-02-12 19:48:13.000000 protean-0.9.0/tests/server/test_engine_initialization.py
--rw-r--r--   0 subhashb   (501) staff       (20)      281 2022-02-12 19:48:13.000000 protean-0.9.0/tests/server/test_engine_run.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2475 2022-02-12 19:48:13.000000 protean-0.9.0/tests/server/test_event_handler_subscription.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1538 2022-02-12 19:48:13.000000 protean-0.9.0/tests/server/test_event_handling.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2241 2022-02-12 19:48:13.000000 protean-0.9.0/tests/server/test_handling_all_events.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.749178 protean-0.9.0/tests/subscription/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2022-02-12 19:48:13.000000 protean-0.9.0/tests/subscription/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)     3071 2022-02-12 19:48:13.000000 protean-0.9.0/tests/subscription/test_message_filtering_with_origin_stream.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1952 2022-02-12 19:48:13.000000 protean-0.9.0/tests/subscription/test_message_handover_to_engine.py
--rw-r--r--   0 subhashb   (501) staff       (20)     3039 2022-02-12 19:48:13.000000 protean-0.9.0/tests/subscription/test_no_message_filtering.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.749705 protean-0.9.0/tests/support/
--rw-r--r--   0 subhashb   (501) staff       (20)       54 2021-08-10 23:12:38.000000 protean-0.9.0/tests/support/config.json
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.477514 protean-0.9.0/tests/support/test_domains/
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.755559 protean-0.9.0/tests/support/test_domains/test1/
--rw-r--r--   0 subhashb   (501) staff       (20)       53 2021-08-12 14:57:06.000000 protean-0.9.0/tests/support/test_domains/test1/basic.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.476696 protean-0.9.0/tests/support/test_domains/test2/
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.756262 protean-0.9.0/tests/support/test_domains/test2/src/
--rw-r--r--   0 subhashb   (501) staff       (20)       54 2021-08-12 14:54:33.000000 protean-0.9.0/tests/support/test_domains/test2/src/folder.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.756995 protean-0.9.0/tests/support/test_domains/test3/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2021-08-11 22:02:46.000000 protean-0.9.0/tests/support/test_domains/test3/__init__.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.757413 protean-0.9.0/tests/support/test_domains/test3/nested/
--rw-r--r--   0 subhashb   (501) staff       (20)       51 2021-08-12 14:54:27.000000 protean-0.9.0/tests/support/test_domains/test3/nested/web.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.760441 protean-0.9.0/tests/support/test_domains/test4/
--rw-r--r--   0 subhashb   (501) staff       (20)       54 2021-08-12 14:54:22.000000 protean-0.9.0/tests/support/test_domains/test4/instance.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.760954 protean-0.9.0/tests/support/test_domains/test5/
--rw-r--r--   0 subhashb   (501) staff       (20)       10 2021-08-12 14:57:13.000000 protean-0.9.0/tests/support/test_domains/test5/dummy.py
--rw-r--r--   0 subhashb   (501) staff       (20)     3575 2022-02-12 19:48:13.000000 protean-0.9.0/tests/test_aggregates.py
--rw-r--r--   0 subhashb   (501) staff       (20)     8030 2022-02-18 02:27:21.000000 protean-0.9.0/tests/test_brokers.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2571 2021-08-24 17:58:32.000000 protean-0.9.0/tests/test_cli.py
--rw-r--r--   0 subhashb   (501) staff       (20)     5014 2022-02-12 19:48:13.000000 protean-0.9.0/tests/test_commands.py
--rw-r--r--   0 subhashb   (501) staff       (20)     5442 2021-08-24 17:58:32.000000 protean-0.9.0/tests/test_config.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2229 2022-02-12 19:48:13.000000 protean-0.9.0/tests/test_containers.py
--rw-r--r--   0 subhashb   (501) staff       (20)      287 2021-09-23 18:06:55.000000 protean-0.9.0/tests/test_exceptions.py
--rw-r--r--   0 subhashb   (501) staff       (20)      737 2022-02-12 19:48:13.000000 protean-0.9.0/tests/test_other.py
--rw-r--r--   0 subhashb   (501) staff       (20)      343 2021-08-10 16:05:35.000000 protean-0.9.0/tests/test_protean_cli.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2975 2022-02-12 19:48:13.000000 protean-0.9.0/tests/test_registry.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1624 2022-02-04 17:31:40.000000 protean-0.9.0/tests/test_subscribers.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.770299 protean-0.9.0/tests/unit_of_work/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-05-30 19:04:30.000000 protean-0.9.0/tests/unit_of_work/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)      937 2021-09-23 17:39:41.000000 protean-0.9.0/tests/unit_of_work/aggregate_elements.py
--rw-r--r--   0 subhashb   (501) staff       (20)      312 2021-09-23 17:39:41.000000 protean-0.9.0/tests/unit_of_work/elements.py
--rw-r--r--   0 subhashb   (501) staff       (20)     3019 2022-01-14 02:23:09.000000 protean-0.9.0/tests/unit_of_work/test_child_object_persistence.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2591 2022-02-12 19:48:13.000000 protean-0.9.0/tests/unit_of_work/test_inline_event_processing.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2683 2022-02-12 19:48:13.000000 protean-0.9.0/tests/unit_of_work/test_nested_inline_event_processing.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1912 2022-02-12 19:48:13.000000 protean-0.9.0/tests/unit_of_work/test_storing_events_on_commit.py
--rw-r--r--   0 subhashb   (501) staff       (20)     6425 2022-02-12 19:48:13.000000 protean-0.9.0/tests/unit_of_work/test_uow_transactions.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1109 2021-09-23 17:39:41.000000 protean-0.9.0/tests/unit_of_work/tests.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.771228 protean-0.9.0/tests/utils/
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.771726 protean-0.9.0/tests/utils/support/
--rw-r--r--   0 subhashb   (501) staff       (20)       76 2021-08-10 16:05:35.000000 protean-0.9.0/tests/utils/support/domain.py
--rw-r--r--   0 subhashb   (501) staff       (20)      158 2021-08-07 21:10:38.000000 protean-0.9.0/tests/utils/test_get_version.py
--rw-r--r--   0 subhashb   (501) staff       (20)      468 2021-08-03 23:51:36.000000 protean-0.9.0/tests/utils/test_import_from_full_path.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.776493 protean-0.9.0/tests/value_object/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-05-30 19:04:30.000000 protean-0.9.0/tests/value_object/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)     3112 2022-02-12 19:48:13.000000 protean-0.9.0/tests/value_object/elements.py
--rw-r--r--   0 subhashb   (501) staff       (20)      700 2021-08-03 23:51:36.000000 protean-0.9.0/tests/value_object/test_lifecycle_methods.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1456 2022-01-14 02:23:09.000000 protean-0.9.0/tests/value_object/test_to_dict.py
--rw-r--r--   0 subhashb   (501) staff       (20)     9756 2022-02-12 19:48:13.000000 protean-0.9.0/tests/value_object/tests.py
-drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-18 03:09:35.779605 protean-0.9.0/tests/views/
--rw-r--r--   0 subhashb   (501) staff       (20)        0 2020-11-10 19:35:58.000000 protean-0.9.0/tests/views/__init__.py
--rw-r--r--   0 subhashb   (501) staff       (20)     1800 2021-09-23 17:39:41.000000 protean-0.9.0/tests/views/test_view_validations_for_fields.py
--rw-r--r--   0 subhashb   (501) staff       (20)      276 2021-09-23 17:39:41.000000 protean-0.9.0/tests/views/test_view_with_redis.py
--rw-r--r--   0 subhashb   (501) staff       (20)    13164 2022-02-12 19:48:13.000000 protean-0.9.0/tests/views/tests.py
--rw-r--r--   0 subhashb   (501) staff       (20)     2376 2021-07-16 18:19:34.000000 protean-0.9.0/tox.ini
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.902251 protean-0.9.1/
+-rw-r--r--   0 subhashb   (501) staff       (20)      169 2022-02-23 21:37:25.000000 protean-0.9.1/.bumpversion.cfg
+-rw-r--r--   0 subhashb   (501) staff       (20)     2043 2019-04-06 03:53:33.000000 protean-0.9.1/.cookiecutterrc
+-rw-r--r--   0 subhashb   (501) staff       (20)      284 2019-04-06 03:53:33.000000 protean-0.9.1/.coveragerc
+-rw-r--r--   0 subhashb   (501) staff       (20)      314 2020-09-22 16:40:24.000000 protean-0.9.1/.editorconfig
+-rw-r--r--   0 subhashb   (501) staff       (20)       71 2020-09-22 16:40:24.000000 protean-0.9.1/.git-blame-ignore-revs
+-rw-r--r--   0 subhashb   (501) staff       (20)      575 2022-02-12 19:48:13.000000 protean-0.9.1/.pre-commit-config.yaml
+-rw-r--r--   0 subhashb   (501) staff       (20)    12963 2022-02-23 21:24:14.000000 protean-0.9.1/CHANGELOG.rst
+-rw-r--r--   0 subhashb   (501) staff       (20)      658 2021-08-09 21:35:32.000000 protean-0.9.1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 subhashb   (501) staff       (20)     6755 2021-08-09 21:32:40.000000 protean-0.9.1/CONTRIBUTING.rst
+-rw-r--r--   0 subhashb   (501) staff       (20)     1516 2020-04-06 01:30:35.000000 protean-0.9.1/LICENSE
+-rw-r--r--   0 subhashb   (501) staff       (20)      505 2020-09-22 16:40:24.000000 protean-0.9.1/MANIFEST.in
+-rw-r--r--   0 subhashb   (501) staff       (20)      413 2022-02-12 19:48:13.000000 protean-0.9.1/Makefile
+-rw-r--r--   0 subhashb   (501) staff       (20)    16441 2022-02-23 21:38:05.902682 protean-0.9.1/PKG-INFO
+-rw-r--r--   0 subhashb   (501) staff       (20)     2157 2021-10-07 17:14:25.000000 protean-0.9.1/README.rst
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.291957 protean-0.9.1/ci/
+-rwxr-xr-x   0 subhashb   (501) staff       (20)     2063 2022-02-12 19:48:13.000000 protean-0.9.1/ci/bootstrap.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1066 2022-02-18 17:21:44.000000 protean-0.9.1/docker-compose.yml
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.299324 protean-0.9.1/docs/
+-rw-r--r--   0 subhashb   (501) staff       (20)      636 2021-08-06 23:09:47.000000 protean-0.9.1/docs/Makefile
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.300395 protean-0.9.1/docs/adapters/
+-rw-r--r--   0 subhashb   (501) staff       (20)     1834 2022-02-12 19:48:13.000000 protean-0.9.1/docs/adapters/database.rst
+-rw-r--r--   0 subhashb   (501) staff       (20)      485 2021-08-17 17:25:27.000000 protean-0.9.1/docs/api.rst
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.303340 protean-0.9.1/docs/community/
+-rw-r--r--   0 subhashb   (501) staff       (20)       33 2021-08-09 17:30:41.000000 protean-0.9.1/docs/community/changelog.rst
+-rw-r--r--   0 subhashb   (501) staff       (20)       39 2021-08-09 21:30:16.000000 protean-0.9.1/docs/community/code-of-conduct.rst
+-rw-r--r--   0 subhashb   (501) staff       (20)       36 2021-08-09 21:30:37.000000 protean-0.9.1/docs/community/contributing.rst
+-rw-r--r--   0 subhashb   (501) staff       (20)     1872 2022-02-23 21:37:25.000000 protean-0.9.1/docs/conf.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.305616 protean-0.9.1/docs/images/
+-rw-r--r--   0 subhashb   (501) staff       (20)    32963 2021-08-16 21:03:49.000000 protean-0.9.1/docs/images/consuming-events.jpg
+-rw-r--r--   0 subhashb   (501) staff       (20)    45503 2021-08-16 21:06:33.000000 protean-0.9.1/docs/images/raising-events.jpg
+-rw-r--r--   0 subhashb   (501) staff       (20)     3473 2021-10-07 17:14:25.000000 protean-0.9.1/docs/index.rst
+-rw-r--r--   0 subhashb   (501) staff       (20)      797 2021-08-06 23:09:47.000000 protean-0.9.1/docs/make.bat
+-rw-r--r--   0 subhashb   (501) staff       (20)       11 2021-08-06 23:08:58.000000 protean-0.9.1/docs/requirements.txt
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.306972 protean-0.9.1/docs/static/
+-rw-r--r--   0 subhashb   (501) staff       (20)       37 2021-08-16 19:58:19.000000 protean-0.9.1/docs/static/custom.css
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.340731 protean-0.9.1/docs/user/
+-rw-r--r--   0 subhashb   (501) staff       (20)     2564 2021-08-12 17:19:36.000000 protean-0.9.1/docs/user/cli.rst
+-rw-r--r--   0 subhashb   (501) staff       (20)     3814 2021-08-10 22:37:09.000000 protean-0.9.1/docs/user/composing-a-domain.rst
+-rw-r--r--   0 subhashb   (501) staff       (20)    12237 2021-08-16 23:56:42.000000 protean-0.9.1/docs/user/config.rst
+-rw-r--r--   0 subhashb   (501) staff       (20)    18905 2021-08-17 17:46:28.000000 protean-0.9.1/docs/user/domain-definition.rst
+-rw-r--r--   0 subhashb   (501) staff       (20)    13694 2021-08-18 19:54:10.000000 protean-0.9.1/docs/user/entities-and-vos.rst
+-rw-r--r--   0 subhashb   (501) staff       (20)    10510 2021-08-16 23:56:38.000000 protean-0.9.1/docs/user/eventing.rst
+-rw-r--r--   0 subhashb   (501) staff       (20)    14638 2021-08-17 20:16:34.000000 protean-0.9.1/docs/user/fields.rst
+-rw-r--r--   0 subhashb   (501) staff       (20)     2884 2021-08-09 18:46:28.000000 protean-0.9.1/docs/user/foreword.rst
+-rw-r--r--   0 subhashb   (501) staff       (20)     2692 2021-08-10 17:21:01.000000 protean-0.9.1/docs/user/installation.rst
+-rw-r--r--   0 subhashb   (501) staff       (20)     9088 2021-08-24 08:06:25.000000 protean-0.9.1/docs/user/persistence.rst
+-rw-r--r--   0 subhashb   (501) staff       (20)     6060 2021-08-09 21:28:20.000000 protean-0.9.1/docs/user/quickstart.rst
+-rw-r--r--   0 subhashb   (501) staff       (20)     1831 2021-08-31 16:03:14.000000 protean-0.9.1/docs/user/services.rst
+-rw-r--r--   0 subhashb   (501) staff       (20)     1134 2022-02-23 21:38:05.904347 protean-0.9.1/setup.cfg
+-rw-r--r--   0 subhashb   (501) staff       (20)     4293 2022-02-23 21:37:25.000000 protean-0.9.1/setup.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.239501 protean-0.9.1/src/
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.347842 protean-0.9.1/src/protean/
+-rw-r--r--   0 subhashb   (501) staff       (20)      974 2022-02-23 21:37:25.000000 protean-0.9.1/src/protean/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      361 2021-07-16 18:23:52.000000 protean-0.9.1/src/protean/__main__.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.352735 protean-0.9.1/src/protean/adapters/
+-rw-r--r--   0 subhashb   (501) staff       (20)      647 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/adapters/__init__.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.356976 protean-0.9.1/src/protean/adapters/broker/
+-rw-r--r--   0 subhashb   (501) staff       (20)     3438 2022-02-17 03:12:21.000000 protean-0.9.1/src/protean/adapters/broker/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     4095 2022-02-18 00:49:21.000000 protean-0.9.1/src/protean/adapters/broker/celery.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      898 2022-02-17 03:17:46.000000 protean-0.9.1/src/protean/adapters/broker/inline.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1026 2022-02-17 03:17:46.000000 protean-0.9.1/src/protean/adapters/broker/redis.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.358944 protean-0.9.1/src/protean/adapters/cache/
+-rw-r--r--   0 subhashb   (501) staff       (20)     2955 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/adapters/cache/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     5457 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/adapters/cache/memory.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2859 2021-09-23 17:39:41.000000 protean-0.9.1/src/protean/adapters/cache/redis.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.360819 protean-0.9.1/src/protean/adapters/email/
+-rw-r--r--   0 subhashb   (501) staff       (20)     2068 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/adapters/email/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      507 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/adapters/email/dummy.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1658 2022-02-18 02:27:14.000000 protean-0.9.1/src/protean/adapters/email/sendgrid.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.364770 protean-0.9.1/src/protean/adapters/event_store/
+-rw-r--r--   0 subhashb   (501) staff       (20)     4790 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/adapters/event_store/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     3968 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/adapters/event_store/memory.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2482 2022-02-23 21:25:10.000000 protean-0.9.1/src/protean/adapters/event_store/message_db.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.399497 protean-0.9.1/src/protean/adapters/repository/
+-rw-r--r--   0 subhashb   (501) staff       (20)     6539 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/adapters/repository/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)    21821 2022-02-18 02:14:54.000000 protean-0.9.1/src/protean/adapters/repository/elasticsearch.py
+-rw-r--r--   0 subhashb   (501) staff       (20)    22123 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/adapters/repository/memory.py
+-rw-r--r--   0 subhashb   (501) staff       (20)    27412 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/adapters/repository/sqlalchemy.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     8108 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/cli.py
+-rw-r--r--   0 subhashb   (501) staff       (20)    12182 2022-02-18 02:24:17.000000 protean-0.9.1/src/protean/container.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.441546 protean-0.9.1/src/protean/core/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2021-09-23 17:39:41.000000 protean-0.9.1/src/protean/core/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2105 2022-02-18 02:23:17.000000 protean-0.9.1/src/protean/core/aggregate.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1375 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/core/application_service.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1932 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/core/command.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     3102 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/core/command_handler.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1003 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/core/domain_service.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2454 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/core/email.py
+-rw-r--r--   0 subhashb   (501) staff       (20)    17436 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/core/entity.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1690 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/core/event.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     3317 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/core/event_handler.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     6805 2022-02-18 02:23:17.000000 protean-0.9.1/src/protean/core/event_sourced_aggregate.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2606 2022-02-18 02:24:26.000000 protean-0.9.1/src/protean/core/event_sourced_repository.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2311 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/core/model.py
+-rw-r--r--   0 subhashb   (501) staff       (20)    11988 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/core/queryset.py
+-rw-r--r--   0 subhashb   (501) staff       (20)    10028 2022-02-18 02:24:52.000000 protean-0.9.1/src/protean/core/repository.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     7222 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/core/serializer.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1735 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/core/subscriber.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     5792 2022-02-18 02:24:59.000000 protean-0.9.1/src/protean/core/unit_of_work.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1376 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/core/value_object.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     4687 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/core/view.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.447919 protean-0.9.1/src/protean/domain/
+-rw-r--r--   0 subhashb   (501) staff       (20)    30182 2022-02-17 02:58:02.000000 protean-0.9.1/src/protean/domain/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)    10890 2021-08-11 01:11:51.000000 protean-0.9.1/src/protean/domain/config.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     3782 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/domain/context.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     3339 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/domain/helpers.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     4116 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/domain/registry.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2569 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/exceptions.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.454253 protean-0.9.1/src/protean/fields/
+-rw-r--r--   0 subhashb   (501) staff       (20)      322 2021-12-02 17:46:40.000000 protean-0.9.1/src/protean/fields/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)    17211 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/fields/association.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     7702 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/fields/base.py
+-rw-r--r--   0 subhashb   (501) staff       (20)    12545 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/fields/basic.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     6391 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/fields/embedded.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2292 2021-09-23 17:39:41.000000 protean-0.9.1/src/protean/fields/mixins.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2892 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/fields/validators.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1084 2021-08-24 17:57:24.000000 protean-0.9.1/src/protean/globals.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.463093 protean-0.9.1/src/protean/port/
+-rw-r--r--   0 subhashb   (501) staff       (20)      160 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/port/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2597 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/port/broker.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2549 2021-08-12 17:03:37.000000 protean-0.9.1/src/protean/port/cache.py
+-rw-r--r--   0 subhashb   (501) staff       (20)    24789 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/port/dao.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     5924 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/port/event_store.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2814 2021-07-16 18:24:42.000000 protean-0.9.1/src/protean/port/provider.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     3165 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/reflection.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.465385 protean-0.9.1/src/protean/server/
+-rw-r--r--   0 subhashb   (501) staff       (20)       27 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/server/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     4713 2022-02-18 02:25:30.000000 protean-0.9.1/src/protean/server/engine.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     4525 2022-02-18 02:25:06.000000 protean-0.9.1/src/protean/server/subscription.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.469213 protean-0.9.1/src/protean/utils/
+-rw-r--r--   0 subhashb   (501) staff       (20)     4893 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/utils/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1153 2021-08-03 23:51:36.000000 protean-0.9.1/src/protean/utils/importlib.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2882 2021-07-16 18:24:42.000000 protean-0.9.1/src/protean/utils/inflection.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     9397 2022-02-18 02:30:01.000000 protean-0.9.1/src/protean/utils/mixins.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     8983 2022-02-12 19:48:13.000000 protean-0.9.1/src/protean/utils/query.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.352248 protean-0.9.1/src/protean.egg-info/
+-rw-r--r--   0 subhashb   (501) staff       (20)    16441 2022-02-23 21:38:04.000000 protean-0.9.1/src/protean.egg-info/PKG-INFO
+-rw-r--r--   0 subhashb   (501) staff       (20)    15852 2022-02-23 21:38:05.000000 protean-0.9.1/src/protean.egg-info/SOURCES.txt
+-rw-r--r--   0 subhashb   (501) staff       (20)        1 2022-02-23 21:38:04.000000 protean-0.9.1/src/protean.egg-info/dependency_links.txt
+-rw-r--r--   0 subhashb   (501) staff       (20)       46 2022-02-23 21:38:04.000000 protean-0.9.1/src/protean.egg-info/entry_points.txt
+-rw-r--r--   0 subhashb   (501) staff       (20)        1 2022-02-23 21:38:04.000000 protean-0.9.1/src/protean.egg-info/not-zip-safe
+-rw-r--r--   0 subhashb   (501) staff       (20)     2887 2022-02-23 21:38:04.000000 protean-0.9.1/src/protean.egg-info/requires.txt
+-rw-r--r--   0 subhashb   (501) staff       (20)        8 2022-02-23 21:38:04.000000 protean-0.9.1/src/protean.egg-info/top_level.txt
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.483541 protean-0.9.1/tests/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-04-06 03:53:33.000000 protean-0.9.1/tests/__init__.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.484337 protean-0.9.1/tests/adapters/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2020-09-28 21:08:18.000000 protean-0.9.1/tests/adapters/__init__.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.249190 protean-0.9.1/tests/adapters/broker/
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.488254 protean-0.9.1/tests/adapters/broker/celery_broker/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2020-09-22 16:41:47.000000 protean-0.9.1/tests/adapters/broker/celery_broker/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1867 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/broker/celery_broker/config.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      809 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/broker/celery_broker/conftest.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1529 2021-09-23 17:39:41.000000 protean-0.9.1/tests/adapters/broker/celery_broker/elements.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1334 2021-08-10 16:05:35.000000 protean-0.9.1/tests/adapters/broker/celery_broker/test_subscriber.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1177 2021-08-10 16:05:35.000000 protean-0.9.1/tests/adapters/broker/celery_broker/tests.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.495468 protean-0.9.1/tests/adapters/broker/redis_broker/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2021-08-03 23:51:36.000000 protean-0.9.1/tests/adapters/broker/redis_broker/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1663 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/broker/redis_broker/config.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      700 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/broker/redis_broker/conftest.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1577 2022-02-17 02:25:28.000000 protean-0.9.1/tests/adapters/broker/redis_broker/elements.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2845 2022-02-17 03:17:46.000000 protean-0.9.1/tests/adapters/broker/redis_broker/tests.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.249694 protean-0.9.1/tests/adapters/cache/
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.499358 protean-0.9.1/tests/adapters/cache/redis_cache/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2021-04-21 23:33:04.000000 protean-0.9.1/tests/adapters/cache/redis_cache/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      755 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/cache/redis_cache/config.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      540 2021-07-16 18:31:32.000000 protean-0.9.1/tests/adapters/cache/redis_cache/conftest.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     7555 2021-09-23 17:39:41.000000 protean-0.9.1/tests/adapters/cache/redis_cache/tests.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.250171 protean-0.9.1/tests/adapters/email/
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.502194 protean-0.9.1/tests/adapters/email/sendgrid_email/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2020-09-22 16:41:47.000000 protean-0.9.1/tests/adapters/email/sendgrid_email/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1361 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/email/sendgrid_email/config.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      550 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/email/sendgrid_email/conftest.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2010 2021-09-23 17:39:41.000000 protean-0.9.1/tests/adapters/email/sendgrid_email/elements.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1292 2021-08-10 16:05:35.000000 protean-0.9.1/tests/adapters/email/sendgrid_email/tests.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.250795 protean-0.9.1/tests/adapters/event_store/
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.507692 protean-0.9.1/tests/adapters/event_store/memory_event_store/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/event_store/memory_event_store/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      361 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/event_store/memory_event_store/test_data_reset.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      420 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/event_store/memory_event_store/test_initialization.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      427 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/event_store/memory_event_store/test_memory_message_repository.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2450 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/event_store/memory_event_store/test_reading_from_memory_event_store.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      977 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/event_store/memory_event_store/test_writing_to_memory_event_store.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.511271 protean-0.9.1/tests/adapters/event_store/message_db_event_store/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/event_store/message_db_event_store/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      620 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/event_store/message_db_event_store/config.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      530 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/event_store/message_db_event_store/conftest.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     4457 2022-02-18 02:28:10.000000 protean-0.9.1/tests/adapters/event_store/message_db_event_store/tests.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.252007 protean-0.9.1/tests/adapters/model/
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.516211 protean-0.9.1/tests/adapters/model/dict_model/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2020-09-22 16:41:47.000000 protean-0.9.1/tests/adapters/model/dict_model/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1499 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/model/dict_model/elements.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     4104 2022-01-14 02:23:09.000000 protean-0.9.1/tests/adapters/model/dict_model/tests.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.521375 protean-0.9.1/tests/adapters/model/elasticsearch_model/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2020-09-22 16:41:47.000000 protean-0.9.1/tests/adapters/model/elasticsearch_model/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      738 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/model/elasticsearch_model/config.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1252 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/model/elasticsearch_model/conftest.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1752 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/model/elasticsearch_model/elements.py
+-rw-r--r--   0 subhashb   (501) staff       (20)    13709 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/model/elasticsearch_model/tests.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.522251 protean-0.9.1/tests/adapters/model/sqlalchemy_model/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2020-09-22 16:41:47.000000 protean-0.9.1/tests/adapters/model/sqlalchemy_model/__init__.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.548416 protean-0.9.1/tests/adapters/model/sqlalchemy_model/postgresql/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2020-09-22 16:41:47.000000 protean-0.9.1/tests/adapters/model/sqlalchemy_model/postgresql/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      764 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/model/sqlalchemy_model/postgresql/config.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2144 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/model/sqlalchemy_model/postgresql/conftest.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1737 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/model/sqlalchemy_model/postgresql/elements.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     4809 2022-01-14 02:23:09.000000 protean-0.9.1/tests/adapters/model/sqlalchemy_model/postgresql/test_array_datatype.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2464 2022-01-14 02:23:09.000000 protean-0.9.1/tests/adapters/model/sqlalchemy_model/postgresql/test_json_datatype.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2528 2022-01-14 02:23:09.000000 protean-0.9.1/tests/adapters/model/sqlalchemy_model/postgresql/test_list_datatype.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1946 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/model/sqlalchemy_model/postgresql/test_lookups.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     4486 2022-01-14 02:23:09.000000 protean-0.9.1/tests/adapters/model/sqlalchemy_model/postgresql/test_model.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.553646 protean-0.9.1/tests/adapters/model/sqlalchemy_model/sqlite/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2020-09-22 16:41:47.000000 protean-0.9.1/tests/adapters/model/sqlalchemy_model/sqlite/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      725 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/model/sqlalchemy_model/sqlite/config.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1704 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/model/sqlalchemy_model/sqlite/conftest.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1438 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/model/sqlalchemy_model/sqlite/elements.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     3091 2022-01-14 02:23:09.000000 protean-0.9.1/tests/adapters/model/sqlalchemy_model/sqlite/test_array_datatype.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1057 2022-01-14 02:23:09.000000 protean-0.9.1/tests/adapters/model/sqlalchemy_model/sqlite/test_json_datatype.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     4408 2022-01-14 02:23:09.000000 protean-0.9.1/tests/adapters/model/sqlalchemy_model/sqlite/test_model.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.554185 protean-0.9.1/tests/adapters/repository/
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.564864 protean-0.9.1/tests/adapters/repository/elasticsearch_repo/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2020-09-22 16:41:47.000000 protean-0.9.1/tests/adapters/repository/elasticsearch_repo/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      738 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/repository/elasticsearch_repo/config.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1031 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/repository/elasticsearch_repo/conftest.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1336 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/repository/elasticsearch_repo/elements.py
+-rw-r--r--   0 subhashb   (501) staff       (20)    36663 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/repository/elasticsearch_repo/test_dao.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1861 2021-07-16 18:24:10.000000 protean-0.9.1/tests/adapters/repository/elasticsearch_repo/test_lookup.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2951 2022-01-14 02:23:09.000000 protean-0.9.1/tests/adapters/repository/elasticsearch_repo/test_provider.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     3008 2022-01-14 02:23:09.000000 protean-0.9.1/tests/adapters/repository/elasticsearch_repo/test_query.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1293 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/repository/elasticsearch_repo/test_repo.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.567186 protean-0.9.1/tests/adapters/repository/memory/
+-rw-r--r--   0 subhashb   (501) staff       (20)     1223 2022-01-14 02:23:09.000000 protean-0.9.1/tests/adapters/repository/memory/test_any_operator.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      822 2022-01-14 02:23:09.000000 protean-0.9.1/tests/adapters/repository/memory/test_in_operator.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1420 2021-07-16 18:35:06.000000 protean-0.9.1/tests/adapters/repository/memory/test_lookups.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1929 2022-01-14 02:23:09.000000 protean-0.9.1/tests/adapters/repository/memory/test_sorting_on_none_values.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.567761 protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2020-09-22 16:41:47.000000 protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/__init__.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.572826 protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/postgresql/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2020-09-22 16:41:47.000000 protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/postgresql/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      765 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/postgresql/config.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1661 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/postgresql/conftest.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1374 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/postgresql/elements.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1639 2022-01-14 02:23:09.000000 protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/postgresql/test_associations.py
+-rw-r--r--   0 subhashb   (501) staff       (20)    36584 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/postgresql/test_dao.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      798 2022-01-14 02:23:09.000000 protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/postgresql/test_persistence.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2961 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/postgresql/test_provider.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     6405 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/postgresql/test_transactions.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.579830 protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/sqlite/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2020-09-22 16:41:47.000000 protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/sqlite/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      725 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/sqlite/config.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1274 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/sqlite/conftest.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1336 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/sqlite/elements.py
+-rw-r--r--   0 subhashb   (501) staff       (20)    34775 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/sqlite/test_dao.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2987 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/sqlite/test_provider.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     6632 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/sqlite/test_transactions.py
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2020-09-22 16:41:47.000000 protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/sqlite/tests.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     4143 2022-02-12 19:48:13.000000 protean-0.9.1/tests/adapters/repository/test_generic.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.594110 protean-0.9.1/tests/aggregate/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-05-30 19:04:30.000000 protean-0.9.1/tests/aggregate/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      866 2021-09-23 17:39:41.000000 protean-0.9.1/tests/aggregate/aggregate_elements.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      467 2021-09-23 17:39:41.000000 protean-0.9.1/tests/aggregate/aggregate_elements_with_value_objects.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     5301 2021-09-23 17:39:41.000000 protean-0.9.1/tests/aggregate/elements.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1506 2022-02-12 19:48:13.000000 protean-0.9.1/tests/aggregate/test_aggregate_abstraction.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     9500 2022-02-12 19:48:13.000000 protean-0.9.1/tests/aggregate/test_aggregate_association.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2024 2022-02-12 19:48:13.000000 protean-0.9.1/tests/aggregate/test_aggregate_events.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     6236 2022-02-12 19:48:13.000000 protean-0.9.1/tests/aggregate/test_aggregate_initialization.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     5602 2022-02-12 19:48:13.000000 protean-0.9.1/tests/aggregate/test_aggregate_properties.py
+-rw-r--r--   0 subhashb   (501) staff       (20)    10102 2022-02-12 19:48:13.000000 protean-0.9.1/tests/aggregate/test_aggregate_reference_field.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1135 2021-09-23 17:39:41.000000 protean-0.9.1/tests/aggregate/test_aggregate_registration.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     4093 2022-01-14 02:23:09.000000 protean-0.9.1/tests/aggregate/test_aggregate_state.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     3945 2022-01-14 02:23:09.000000 protean-0.9.1/tests/aggregate/test_aggregates_with_entities.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1726 2021-07-16 18:27:32.000000 protean-0.9.1/tests/aggregate/test_aggregates_with_value_objects.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     5378 2022-02-12 19:48:13.000000 protean-0.9.1/tests/aggregate/test_as_dict.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.597483 protean-0.9.1/tests/application_service/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-06-25 14:29:25.000000 protean-0.9.1/tests/application_service/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      189 2021-09-23 17:39:41.000000 protean-0.9.1/tests/application_service/elements.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1224 2021-09-23 17:39:41.000000 protean-0.9.1/tests/application_service/tests.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.599355 protean-0.9.1/tests/cache/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2021-04-21 23:33:04.000000 protean-0.9.1/tests/cache/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     7503 2021-10-02 16:15:04.000000 protean-0.9.1/tests/cache/tests.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.603253 protean-0.9.1/tests/command/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2022-02-12 19:48:13.000000 protean-0.9.1/tests/command/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2755 2022-02-18 02:28:05.000000 protean-0.9.1/tests/command/test_automatic_stream_association.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      636 2022-02-12 19:48:13.000000 protean-0.9.1/tests/command/test_command_identity.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2422 2022-02-18 02:28:47.000000 protean-0.9.1/tests/command/test_command_meta.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.611371 protean-0.9.1/tests/command_handler/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2022-02-12 19:48:13.000000 protean-0.9.1/tests/command_handler/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1046 2022-02-12 19:48:13.000000 protean-0.9.1/tests/command_handler/test_command_handler_options.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1167 2022-02-12 19:48:13.000000 protean-0.9.1/tests/command_handler/test_command_handler_registration.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2717 2022-02-12 19:48:13.000000 protean-0.9.1/tests/command_handler/test_handle_decorator_in_command_handlers.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1432 2022-02-17 03:03:33.000000 protean-0.9.1/tests/command_handler/test_inline_command_processing.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2456 2022-02-12 19:48:13.000000 protean-0.9.1/tests/command_handler/test_retrieving_handlers_by_command.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1246 2022-02-12 19:48:13.000000 protean-0.9.1/tests/command_handler/test_uow_around_command_handlers.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2104 2022-02-12 19:48:13.000000 protean-0.9.1/tests/config.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.616968 protean-0.9.1/tests/configuration/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-06-08 01:24:59.000000 protean-0.9.1/tests/configuration/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)       54 2019-06-08 01:24:59.000000 protean-0.9.1/tests/configuration/config.json
+-rw-r--r--   0 subhashb   (501) staff       (20)     6056 2022-02-12 19:48:13.000000 protean-0.9.1/tests/configuration/tests.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     6778 2022-02-12 19:48:13.000000 protean-0.9.1/tests/conftest.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.618219 protean-0.9.1/tests/container/
+-rw-r--r--   0 subhashb   (501) staff       (20)     1370 2022-02-12 19:48:13.000000 protean-0.9.1/tests/container/test_options.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.619830 protean-0.9.1/tests/context/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-06-08 01:24:59.000000 protean-0.9.1/tests/context/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     4253 2022-02-12 19:48:13.000000 protean-0.9.1/tests/context/tests.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.631315 protean-0.9.1/tests/dao/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-05-30 19:04:30.000000 protean-0.9.1/tests/dao/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      653 2021-09-23 17:39:41.000000 protean-0.9.1/tests/dao/elements.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2322 2022-01-14 02:23:09.000000 protean-0.9.1/tests/dao/test_basics.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     5943 2022-02-12 19:48:13.000000 protean-0.9.1/tests/dao/test_delete.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      105 2019-09-27 16:08:17.000000 protean-0.9.1/tests/dao/test_lookup.py
+-rw-r--r--   0 subhashb   (501) staff       (20)    14830 2022-02-12 19:48:13.000000 protean-0.9.1/tests/dao/test_retrieval.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1767 2022-02-12 19:48:13.000000 protean-0.9.1/tests/dao/test_save.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     7248 2022-02-12 19:48:13.000000 protean-0.9.1/tests/dao/test_update.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2245 2022-02-12 19:48:13.000000 protean-0.9.1/tests/dao/test_validations.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.636097 protean-0.9.1/tests/domain/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-05-30 19:04:30.000000 protean-0.9.1/tests/domain/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      495 2021-09-23 17:39:41.000000 protean-0.9.1/tests/domain/elements.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      529 2022-02-12 19:48:13.000000 protean-0.9.1/tests/domain/test_config_immutability.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     9543 2022-02-12 19:48:13.000000 protean-0.9.1/tests/domain/tests.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.638338 protean-0.9.1/tests/domain_service/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-06-25 18:11:26.000000 protean-0.9.1/tests/domain_service/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      166 2021-09-23 17:39:41.000000 protean-0.9.1/tests/domain_service/elements.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1125 2021-09-23 17:39:41.000000 protean-0.9.1/tests/domain_service/tests.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.648912 protean-0.9.1/tests/email_provider/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2020-01-10 17:02:21.000000 protean-0.9.1/tests/email_provider/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2083 2021-09-23 17:39:41.000000 protean-0.9.1/tests/email_provider/elements.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1856 2022-02-12 19:48:13.000000 protean-0.9.1/tests/email_provider/tests.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.716513 protean-0.9.1/tests/entity/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-05-30 19:04:30.000000 protean-0.9.1/tests/entity/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2756 2021-09-23 17:39:41.000000 protean-0.9.1/tests/entity/elements.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     5848 2022-02-12 19:48:13.000000 protean-0.9.1/tests/entity/test_entity.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     3459 2022-02-12 19:48:13.000000 protean-0.9.1/tests/entity/test_entity_meta.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     5965 2022-02-12 19:48:13.000000 protean-0.9.1/tests/entity/test_entity_properties.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1841 2021-09-23 17:39:41.000000 protean-0.9.1/tests/entity/test_entity_registration.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1440 2021-09-23 17:39:41.000000 protean-0.9.1/tests/entity/test_fields.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      700 2021-08-03 23:51:36.000000 protean-0.9.1/tests/entity/test_lifecycle_methods.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      555 2021-09-23 17:39:41.000000 protean-0.9.1/tests/entity/test_temp.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.734775 protean-0.9.1/tests/event/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-07-01 16:19:36.000000 protean-0.9.1/tests/event/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1508 2021-09-23 17:39:41.000000 protean-0.9.1/tests/event/elements.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2883 2022-02-18 02:28:05.000000 protean-0.9.1/tests/event/test_automatic_stream_association.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      636 2022-02-12 19:48:13.000000 protean-0.9.1/tests/event/test_event_identity.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1597 2022-02-18 02:29:20.000000 protean-0.9.1/tests/event/test_event_meta.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      814 2022-02-12 19:48:13.000000 protean-0.9.1/tests/event/test_raising_events.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      872 2021-08-10 16:05:35.000000 protean-0.9.1/tests/event/test_serialization.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2585 2022-02-17 00:23:17.000000 protean-0.9.1/tests/event/tests.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.764799 protean-0.9.1/tests/event_handler/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2022-02-12 19:48:13.000000 protean-0.9.1/tests/event_handler/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1023 2022-02-12 19:48:13.000000 protean-0.9.1/tests/event_handler/test_any_event_handler.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2401 2022-02-12 19:48:13.000000 protean-0.9.1/tests/event_handler/test_event_handler_options.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1124 2022-02-12 19:48:13.000000 protean-0.9.1/tests/event_handler/test_event_handler_registration.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2935 2022-02-12 19:48:13.000000 protean-0.9.1/tests/event_handler/test_handle_decorator_in_event_handlers.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2834 2022-02-12 19:48:13.000000 protean-0.9.1/tests/event_handler/test_retrieving_handlers_by_event.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1258 2022-02-12 19:48:13.000000 protean-0.9.1/tests/event_handler/test_uow_around_event_handlers.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.771464 protean-0.9.1/tests/event_sourced_aggregates/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2022-02-12 19:48:13.000000 protean-0.9.1/tests/event_sourced_aggregates/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     3063 2022-02-18 02:28:16.000000 protean-0.9.1/tests/event_sourced_aggregates/test_applying_events.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2533 2022-02-12 19:48:13.000000 protean-0.9.1/tests/event_sourced_aggregates/test_event_association_with_aggregate.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1551 2022-02-12 19:48:13.000000 protean-0.9.1/tests/event_sourced_aggregates/test_event_sourced_aggregate_options.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1095 2022-02-12 19:48:13.000000 protean-0.9.1/tests/event_sourced_aggregates/test_event_sourced_aggregate_registration.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2487 2022-02-12 19:48:13.000000 protean-0.9.1/tests/event_sourced_aggregates/test_expected_version_error.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2295 2022-02-12 19:48:13.000000 protean-0.9.1/tests/event_sourced_aggregates/test_raising_events_from_within_aggregates.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.776744 protean-0.9.1/tests/event_sourced_repository/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2022-02-12 19:48:13.000000 protean-0.9.1/tests/event_sourced_repository/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     4841 2022-02-12 19:48:13.000000 protean-0.9.1/tests/event_sourced_repository/test_loading_aggregates.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1009 2022-02-12 19:48:13.000000 protean-0.9.1/tests/event_sourced_repository/test_retrieving_event_sourced_repository.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.785101 protean-0.9.1/tests/event_store/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2022-02-12 19:48:13.000000 protean-0.9.1/tests/event_store/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2334 2022-02-12 19:48:13.000000 protean-0.9.1/tests/event_store/test_appending_aggregate_events.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1517 2022-02-18 02:28:29.000000 protean-0.9.1/tests/event_store/test_appending_commands.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      840 2022-02-12 19:48:13.000000 protean-0.9.1/tests/event_store/test_appending_events.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      507 2022-02-12 19:48:13.000000 protean-0.9.1/tests/event_store/test_deriving_category.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      495 2022-02-12 19:48:13.000000 protean-0.9.1/tests/event_store/test_event_store_adapter_initialization.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2211 2022-02-12 19:48:13.000000 protean-0.9.1/tests/event_store/test_reading_all_streams.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     5178 2022-02-12 19:48:13.000000 protean-0.9.1/tests/event_store/test_reading_messages.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     5091 2022-02-12 19:48:13.000000 protean-0.9.1/tests/event_store/test_snapshotting.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2005 2022-02-12 19:48:13.000000 protean-0.9.1/tests/event_store/test_streams_initialization.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.792913 protean-0.9.1/tests/field/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-05-31 17:44:59.000000 protean-0.9.1/tests/field/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      750 2021-09-23 17:39:41.000000 protean-0.9.1/tests/field/elements.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      865 2022-02-12 19:48:13.000000 protean-0.9.1/tests/field/test_associations.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2473 2022-02-18 02:28:05.000000 protean-0.9.1/tests/field/test_auto.py
+-rw-r--r--   0 subhashb   (501) staff       (20)    11247 2022-02-18 02:28:05.000000 protean-0.9.1/tests/field/test_field_types.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2554 2021-09-23 17:39:41.000000 protean-0.9.1/tests/field/test_field_validators.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      525 2022-02-12 19:48:13.000000 protean-0.9.1/tests/field/test_identifier.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      751 2022-02-12 19:48:13.000000 protean-0.9.1/tests/field/test_reference.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     3745 2022-02-12 19:48:13.000000 protean-0.9.1/tests/field/tests.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.831932 protean-0.9.1/tests/identity/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-09-04 22:52:17.000000 protean-0.9.1/tests/identity/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      742 2022-02-12 19:48:13.000000 protean-0.9.1/tests/identity/config_int.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      760 2022-02-12 19:48:13.000000 protean-0.9.1/tests/identity/config_string.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      758 2022-02-12 19:48:13.000000 protean-0.9.1/tests/identity/config_uuid.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1335 2022-02-12 19:48:13.000000 protean-0.9.1/tests/identity/conftest.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      245 2021-09-23 17:39:41.000000 protean-0.9.1/tests/identity/elements.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      792 2021-07-16 18:27:32.000000 protean-0.9.1/tests/identity/tests.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.847192 protean-0.9.1/tests/message/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2022-02-12 19:48:13.000000 protean-0.9.1/tests/message/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2007 2022-02-12 19:48:13.000000 protean-0.9.1/tests/message/test_message_to_object.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     5169 2022-02-16 22:46:36.000000 protean-0.9.1/tests/message/test_object_to_message.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     3721 2022-02-18 02:27:37.000000 protean-0.9.1/tests/message/test_origin_stream_name_in_metadata.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.850441 protean-0.9.1/tests/provider/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-05-31 17:44:59.000000 protean-0.9.1/tests/provider/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      412 2021-09-23 17:39:41.000000 protean-0.9.1/tests/provider/elements.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2858 2022-01-14 02:23:09.000000 protean-0.9.1/tests/provider/tests.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.856596 protean-0.9.1/tests/query/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-05-31 17:44:59.000000 protean-0.9.1/tests/query/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      245 2021-09-23 17:39:41.000000 protean-0.9.1/tests/query/elements.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     4261 2022-01-14 02:23:09.000000 protean-0.9.1/tests/query/test_conjunctions.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2101 2022-02-12 19:48:13.000000 protean-0.9.1/tests/query/test_q.py
+-rw-r--r--   0 subhashb   (501) staff       (20)    26398 2022-02-18 02:29:12.000000 protean-0.9.1/tests/query/test_queryset.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.857977 protean-0.9.1/tests/reflection/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2022-02-12 19:48:13.000000 protean-0.9.1/tests/reflection/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      873 2022-02-12 19:48:13.000000 protean-0.9.1/tests/reflection/test_has_id_field.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.868183 protean-0.9.1/tests/repository/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-05-30 19:04:30.000000 protean-0.9.1/tests/repository/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      865 2021-09-23 17:39:41.000000 protean-0.9.1/tests/repository/child_entities.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1200 2022-02-12 19:48:13.000000 protean-0.9.1/tests/repository/elements.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1947 2022-02-12 19:48:13.000000 protean-0.9.1/tests/repository/test_aggregate_persistence.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     5572 2022-01-14 02:23:09.000000 protean-0.9.1/tests/repository/test_child_persistence.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     4641 2022-01-14 02:23:09.000000 protean-0.9.1/tests/repository/test_providers.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     5739 2022-01-14 02:23:09.000000 protean-0.9.1/tests/repository/test_repository_registration.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1661 2022-01-14 02:23:09.000000 protean-0.9.1/tests/repository/test_resultset.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1604 2022-02-12 19:48:13.000000 protean-0.9.1/tests/repository/test_tracking_seen_objects.py
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2022-02-12 19:48:13.000000 protean-0.9.1/tests/repository/test_writing_events_in_seen_objects.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      880 2022-02-12 19:48:13.000000 protean-0.9.1/tests/repository/tests.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.870115 protean-0.9.1/tests/serializer/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-07-13 06:22:37.000000 protean-0.9.1/tests/serializer/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      336 2021-09-23 17:39:41.000000 protean-0.9.1/tests/serializer/elements.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1706 2022-02-12 19:48:13.000000 protean-0.9.1/tests/serializer/tests.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.877683 protean-0.9.1/tests/server/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2022-02-12 19:48:13.000000 protean-0.9.1/tests/server/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1073 2022-02-12 19:48:13.000000 protean-0.9.1/tests/server/dummy_domain.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1582 2022-02-12 19:48:13.000000 protean-0.9.1/tests/server/test_any_event_handler.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1281 2022-02-12 19:48:13.000000 protean-0.9.1/tests/server/test_command_handler_subscription.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1481 2022-02-12 19:48:13.000000 protean-0.9.1/tests/server/test_command_handling.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      719 2022-02-12 19:48:13.000000 protean-0.9.1/tests/server/test_engine_initialization.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      281 2022-02-12 19:48:13.000000 protean-0.9.1/tests/server/test_engine_run.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2475 2022-02-12 19:48:13.000000 protean-0.9.1/tests/server/test_event_handler_subscription.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1538 2022-02-12 19:48:13.000000 protean-0.9.1/tests/server/test_event_handling.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2241 2022-02-12 19:48:13.000000 protean-0.9.1/tests/server/test_handling_all_events.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.882663 protean-0.9.1/tests/subscription/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2022-02-12 19:48:13.000000 protean-0.9.1/tests/subscription/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     3071 2022-02-12 19:48:13.000000 protean-0.9.1/tests/subscription/test_message_filtering_with_origin_stream.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1952 2022-02-12 19:48:13.000000 protean-0.9.1/tests/subscription/test_message_handover_to_engine.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     3039 2022-02-12 19:48:13.000000 protean-0.9.1/tests/subscription/test_no_message_filtering.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.883347 protean-0.9.1/tests/support/
+-rw-r--r--   0 subhashb   (501) staff       (20)       54 2021-08-10 23:12:38.000000 protean-0.9.1/tests/support/config.json
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.267761 protean-0.9.1/tests/support/test_domains/
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.884094 protean-0.9.1/tests/support/test_domains/test1/
+-rw-r--r--   0 subhashb   (501) staff       (20)       53 2021-08-12 14:57:06.000000 protean-0.9.1/tests/support/test_domains/test1/basic.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.265969 protean-0.9.1/tests/support/test_domains/test2/
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.884594 protean-0.9.1/tests/support/test_domains/test2/src/
+-rw-r--r--   0 subhashb   (501) staff       (20)       54 2021-08-12 14:54:33.000000 protean-0.9.1/tests/support/test_domains/test2/src/folder.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.885104 protean-0.9.1/tests/support/test_domains/test3/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2021-08-11 22:02:46.000000 protean-0.9.1/tests/support/test_domains/test3/__init__.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.885558 protean-0.9.1/tests/support/test_domains/test3/nested/
+-rw-r--r--   0 subhashb   (501) staff       (20)       51 2021-08-12 14:54:27.000000 protean-0.9.1/tests/support/test_domains/test3/nested/web.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.886112 protean-0.9.1/tests/support/test_domains/test4/
+-rw-r--r--   0 subhashb   (501) staff       (20)       54 2021-08-12 14:54:22.000000 protean-0.9.1/tests/support/test_domains/test4/instance.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.886692 protean-0.9.1/tests/support/test_domains/test5/
+-rw-r--r--   0 subhashb   (501) staff       (20)       10 2021-08-12 14:57:13.000000 protean-0.9.1/tests/support/test_domains/test5/dummy.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     3575 2022-02-12 19:48:13.000000 protean-0.9.1/tests/test_aggregates.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     8030 2022-02-18 02:27:21.000000 protean-0.9.1/tests/test_brokers.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2571 2021-08-24 17:58:32.000000 protean-0.9.1/tests/test_cli.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     5014 2022-02-12 19:48:13.000000 protean-0.9.1/tests/test_commands.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     5442 2021-08-24 17:58:32.000000 protean-0.9.1/tests/test_config.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2229 2022-02-12 19:48:13.000000 protean-0.9.1/tests/test_containers.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      287 2021-09-23 18:06:55.000000 protean-0.9.1/tests/test_exceptions.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      737 2022-02-12 19:48:13.000000 protean-0.9.1/tests/test_other.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      343 2021-08-10 16:05:35.000000 protean-0.9.1/tests/test_protean_cli.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2975 2022-02-12 19:48:13.000000 protean-0.9.1/tests/test_registry.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1624 2022-02-04 17:31:40.000000 protean-0.9.1/tests/test_subscribers.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.892695 protean-0.9.1/tests/unit_of_work/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-05-30 19:04:30.000000 protean-0.9.1/tests/unit_of_work/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      937 2021-09-23 17:39:41.000000 protean-0.9.1/tests/unit_of_work/aggregate_elements.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      312 2021-09-23 17:39:41.000000 protean-0.9.1/tests/unit_of_work/elements.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     3019 2022-01-14 02:23:09.000000 protean-0.9.1/tests/unit_of_work/test_child_object_persistence.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2591 2022-02-12 19:48:13.000000 protean-0.9.1/tests/unit_of_work/test_inline_event_processing.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2683 2022-02-12 19:48:13.000000 protean-0.9.1/tests/unit_of_work/test_nested_inline_event_processing.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1912 2022-02-12 19:48:13.000000 protean-0.9.1/tests/unit_of_work/test_storing_events_on_commit.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     6425 2022-02-12 19:48:13.000000 protean-0.9.1/tests/unit_of_work/test_uow_transactions.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1109 2021-09-23 17:39:41.000000 protean-0.9.1/tests/unit_of_work/tests.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.894011 protean-0.9.1/tests/utils/
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.894700 protean-0.9.1/tests/utils/support/
+-rw-r--r--   0 subhashb   (501) staff       (20)       76 2021-08-10 16:05:35.000000 protean-0.9.1/tests/utils/support/domain.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      158 2021-08-07 21:10:38.000000 protean-0.9.1/tests/utils/test_get_version.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      468 2021-08-03 23:51:36.000000 protean-0.9.1/tests/utils/test_import_from_full_path.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.898037 protean-0.9.1/tests/value_object/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2019-05-30 19:04:30.000000 protean-0.9.1/tests/value_object/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     3112 2022-02-12 19:48:13.000000 protean-0.9.1/tests/value_object/elements.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      700 2021-08-03 23:51:36.000000 protean-0.9.1/tests/value_object/test_lifecycle_methods.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1456 2022-01-14 02:23:09.000000 protean-0.9.1/tests/value_object/test_to_dict.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     9756 2022-02-12 19:48:13.000000 protean-0.9.1/tests/value_object/tests.py
+drwxr-xr-x   0 subhashb   (501) staff       (20)        0 2022-02-23 21:38:05.901611 protean-0.9.1/tests/views/
+-rw-r--r--   0 subhashb   (501) staff       (20)        0 2020-11-10 19:35:58.000000 protean-0.9.1/tests/views/__init__.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     1800 2021-09-23 17:39:41.000000 protean-0.9.1/tests/views/test_view_validations_for_fields.py
+-rw-r--r--   0 subhashb   (501) staff       (20)      276 2021-09-23 17:39:41.000000 protean-0.9.1/tests/views/test_view_with_redis.py
+-rw-r--r--   0 subhashb   (501) staff       (20)    13164 2022-02-12 19:48:13.000000 protean-0.9.1/tests/views/tests.py
+-rw-r--r--   0 subhashb   (501) staff       (20)     2376 2021-07-16 18:19:34.000000 protean-0.9.1/tox.ini
```

### Comparing `protean-0.9.0/.cookiecutterrc` & `protean-0.9.1/.cookiecutterrc`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/.pre-commit-config.yaml` & `protean-0.9.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/CHANGELOG.rst` & `protean-0.9.1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 ===============
 
 DEV
 ---
 
 
 
+0.9.1
+-----
+
+* Bugfix - Use Domain's EventStore connection details for clearing events after test runs
+
 0.9.0
 -----
 
 * Output VO values as nested dicts instead of a forced flat structure
 * Enclose DAOs within repositories to encourage DB interaction solely through repos
 * Remove `remove` method from repository to discourage hard deletes
 * Manage concurrency with Aggregate versions
```

### Comparing `protean-0.9.0/CODE_OF_CONDUCT.rst` & `protean-0.9.1/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/CONTRIBUTING.rst` & `protean-0.9.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/LICENSE` & `protean-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/PKG-INFO` & `protean-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protean
-Version: 0.9.0
+Version: 0.9.1
 Summary: Protean Application Framework
 Home-page: https://github.com/proteanhq/protean
 Author: Subhash Bhushan C
 Author-email: subhash@team8solutions.com
 License: BSD 3-Clause License
 Keywords: domain-driven design,ddd,cqrs,cqs,ports and adapters
 Platform: UNKNOWN
@@ -92,14 +92,19 @@
 ===============
 
 DEV
 ---
 
 
 
+0.9.1
+-----
+
+* Bugfix - Use Domain's EventStore connection details for clearing events after test runs
+
 0.9.0
 -----
 
 * Output VO values as nested dicts instead of a forced flat structure
 * Enclose DAOs within repositories to encourage DB interaction solely through repos
 * Remove `remove` method from repository to discourage hard deletes
 * Manage concurrency with Aggregate versions
```

### Comparing `protean-0.9.0/README.rst` & `protean-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/ci/bootstrap.py` & `protean-0.9.1/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/docker-compose.yml` & `protean-0.9.1/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/docs/Makefile` & `protean-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/docs/adapters/database.rst` & `protean-0.9.1/docs/adapters/database.rst`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/docs/conf.py` & `protean-0.9.1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 source_suffix = ".rst"
 master_doc = "index"
 project = "Protean"
 year = "2021"
 author = "Subhash Bhushan C"
 copyright = "{0}, {1}".format(year, author)
-version = release = "0.9.0"
+version = release = "0.9.1"
 
 pygments_style = "autumn"
 templates_path = ["."]
 extlinks = {
     "issue": ("https://github.com/proteanhq/protean/issues/%s", "#"),
     "pr": ("https://github.com/proteanhq/protean/pull/%s", "PR #"),
 }
```

### Comparing `protean-0.9.0/docs/images/consuming-events.jpg` & `protean-0.9.1/docs/images/consuming-events.jpg`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/docs/images/raising-events.jpg` & `protean-0.9.1/docs/images/raising-events.jpg`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/docs/index.rst` & `protean-0.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/docs/make.bat` & `protean-0.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/docs/user/cli.rst` & `protean-0.9.1/docs/user/cli.rst`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/docs/user/composing-a-domain.rst` & `protean-0.9.1/docs/user/composing-a-domain.rst`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/docs/user/config.rst` & `protean-0.9.1/docs/user/config.rst`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/docs/user/domain-definition.rst` & `protean-0.9.1/docs/user/domain-definition.rst`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/docs/user/entities-and-vos.rst` & `protean-0.9.1/docs/user/entities-and-vos.rst`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/docs/user/eventing.rst` & `protean-0.9.1/docs/user/eventing.rst`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/docs/user/fields.rst` & `protean-0.9.1/docs/user/fields.rst`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/docs/user/foreword.rst` & `protean-0.9.1/docs/user/foreword.rst`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/docs/user/installation.rst` & `protean-0.9.1/docs/user/installation.rst`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/docs/user/persistence.rst` & `protean-0.9.1/docs/user/persistence.rst`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/docs/user/quickstart.rst` & `protean-0.9.1/docs/user/quickstart.rst`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/docs/user/services.rst` & `protean-0.9.1/docs/user/services.rst`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/setup.cfg` & `protean-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/setup.py` & `protean-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         "tox==3.15.0",
         "twine==3.1.1",
     ]
 )
 
 setup(
     name="protean",
-    version="0.9.0",
+    version="0.9.1",
     license="BSD 3-Clause License",
     description="Protean Application Framework",
     long_description="%s\n%s"
     % (
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub(
             "", read("README.rst")
         ),
```

### Comparing `protean-0.9.0/src/protean/__init__.py` & `protean-0.9.1/src/protean/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 
 from .core.aggregate import BaseAggregate
 from .core.application_service import BaseApplicationService
 from .core.command import BaseCommand
 from .core.command_handler import BaseCommandHandler
 from .core.domain_service import BaseDomainService
 from .core.email import BaseEmail
```

### Comparing `protean-0.9.0/src/protean/adapters/__init__.py` & `protean-0.9.1/src/protean/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/adapters/broker/__init__.py` & `protean-0.9.1/src/protean/adapters/broker/__init__.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/adapters/broker/celery.py` & `protean-0.9.1/src/protean/adapters/broker/celery.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/adapters/broker/inline.py` & `protean-0.9.1/src/protean/adapters/broker/inline.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/adapters/broker/redis.py` & `protean-0.9.1/src/protean/adapters/broker/redis.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/adapters/cache/__init__.py` & `protean-0.9.1/src/protean/adapters/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/adapters/cache/memory.py` & `protean-0.9.1/src/protean/adapters/cache/memory.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/adapters/cache/redis.py` & `protean-0.9.1/src/protean/adapters/cache/redis.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/adapters/email/__init__.py` & `protean-0.9.1/src/protean/adapters/email/__init__.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/adapters/email/sendgrid.py` & `protean-0.9.1/src/protean/adapters/email/sendgrid.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/adapters/event_store/__init__.py` & `protean-0.9.1/src/protean/adapters/event_store/__init__.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/adapters/event_store/memory.py` & `protean-0.9.1/src/protean/adapters/event_store/memory.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/adapters/event_store/message_db.py` & `protean-0.9.1/src/protean/adapters/event_store/message_db.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Any, Dict, List
+from urllib.parse import urlparse
 
 import psycopg2
 
 from message_db.client import MessageDB
 
 from protean.exceptions import ConfigurationError
 from protean.port.event_store import BaseEventStore
@@ -51,22 +52,26 @@
 
     def _read_last_message(self, stream_name) -> Dict[str, Any]:
         return self.client.read_last_message(stream_name)
 
     def _data_reset(self):
         """Utility function to empty messages, to be used only by test harness.
 
-        This method is designed to work only with the postgres instance run in the configured docker container:
-        Port is locked to 5433 and it is assumed that the default user does not have a password, both of which
+        This method is designed to work only with the postgres instance running in the configured docker container:
+        User is locked to `postgres` and it is assumed that the default user does not have a password, both of which
         should not be the configuration in production.
 
-        Any changes to docker configuration will need to updated here.
+        Any changes to configuration will need to updated here.
         """
+        parsed = urlparse(self.domain.config["EVENT_STORE"]["DATABASE_URI"])
         conn = psycopg2.connect(
-            dbname="message_store", user="postgres", port=5433, host="localhost"
+            dbname=parsed.path[1:],
+            user="postgres",
+            port=parsed.port,
+            host=parsed.hostname,
         )
 
         cursor = conn.cursor()
         cursor.execute("TRUNCATE message_store.messages RESTART IDENTITY;")
 
         conn.commit()  # Apparently, psycopg2 requires a `commit` even if its a `TRUNCATE` command
         cursor.close()
```

### Comparing `protean-0.9.0/src/protean/adapters/repository/__init__.py` & `protean-0.9.1/src/protean/adapters/repository/__init__.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/adapters/repository/elasticsearch.py` & `protean-0.9.1/src/protean/adapters/repository/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/adapters/repository/memory.py` & `protean-0.9.1/src/protean/adapters/repository/memory.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/adapters/repository/sqlalchemy.py` & `protean-0.9.1/src/protean/adapters/repository/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/cli.py` & `protean-0.9.1/src/protean/cli.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/container.py` & `protean-0.9.1/src/protean/container.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/core/aggregate.py` & `protean-0.9.1/src/protean/core/aggregate.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/core/application_service.py` & `protean-0.9.1/src/protean/core/application_service.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/core/command.py` & `protean-0.9.1/src/protean/core/command.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/core/command_handler.py` & `protean-0.9.1/src/protean/core/command_handler.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/core/domain_service.py` & `protean-0.9.1/src/protean/core/domain_service.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/core/email.py` & `protean-0.9.1/src/protean/core/email.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/core/entity.py` & `protean-0.9.1/src/protean/core/entity.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/core/event.py` & `protean-0.9.1/src/protean/core/event.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/core/event_handler.py` & `protean-0.9.1/src/protean/core/event_handler.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/core/event_sourced_aggregate.py` & `protean-0.9.1/src/protean/core/event_sourced_aggregate.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/core/event_sourced_repository.py` & `protean-0.9.1/src/protean/core/event_sourced_repository.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/core/model.py` & `protean-0.9.1/src/protean/core/model.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/core/queryset.py` & `protean-0.9.1/src/protean/core/queryset.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/core/repository.py` & `protean-0.9.1/src/protean/core/repository.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/core/serializer.py` & `protean-0.9.1/src/protean/core/serializer.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/core/subscriber.py` & `protean-0.9.1/src/protean/core/subscriber.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/core/unit_of_work.py` & `protean-0.9.1/src/protean/core/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/core/value_object.py` & `protean-0.9.1/src/protean/core/value_object.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/core/view.py` & `protean-0.9.1/src/protean/core/view.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/domain/__init__.py` & `protean-0.9.1/src/protean/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/domain/config.py` & `protean-0.9.1/src/protean/domain/config.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/domain/context.py` & `protean-0.9.1/src/protean/domain/context.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/domain/helpers.py` & `protean-0.9.1/src/protean/domain/helpers.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/domain/registry.py` & `protean-0.9.1/src/protean/domain/registry.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/exceptions.py` & `protean-0.9.1/src/protean/exceptions.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/fields/association.py` & `protean-0.9.1/src/protean/fields/association.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/fields/base.py` & `protean-0.9.1/src/protean/fields/base.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/fields/basic.py` & `protean-0.9.1/src/protean/fields/basic.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/fields/embedded.py` & `protean-0.9.1/src/protean/fields/embedded.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/fields/mixins.py` & `protean-0.9.1/src/protean/fields/mixins.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/fields/validators.py` & `protean-0.9.1/src/protean/fields/validators.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/globals.py` & `protean-0.9.1/src/protean/globals.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/port/broker.py` & `protean-0.9.1/src/protean/port/broker.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/port/cache.py` & `protean-0.9.1/src/protean/port/cache.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/port/dao.py` & `protean-0.9.1/src/protean/port/dao.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/port/event_store.py` & `protean-0.9.1/src/protean/port/event_store.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/port/provider.py` & `protean-0.9.1/src/protean/port/provider.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/reflection.py` & `protean-0.9.1/src/protean/reflection.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/server/engine.py` & `protean-0.9.1/src/protean/server/engine.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/server/subscription.py` & `protean-0.9.1/src/protean/server/subscription.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/utils/__init__.py` & `protean-0.9.1/src/protean/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/utils/importlib.py` & `protean-0.9.1/src/protean/utils/importlib.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/utils/inflection.py` & `protean-0.9.1/src/protean/utils/inflection.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/utils/mixins.py` & `protean-0.9.1/src/protean/utils/mixins.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean/utils/query.py` & `protean-0.9.1/src/protean/utils/query.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean.egg-info/PKG-INFO` & `protean-0.9.1/src/protean.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protean
-Version: 0.9.0
+Version: 0.9.1
 Summary: Protean Application Framework
 Home-page: https://github.com/proteanhq/protean
 Author: Subhash Bhushan C
 Author-email: subhash@team8solutions.com
 License: BSD 3-Clause License
 Keywords: domain-driven design,ddd,cqrs,cqs,ports and adapters
 Platform: UNKNOWN
@@ -92,14 +92,19 @@
 ===============
 
 DEV
 ---
 
 
 
+0.9.1
+-----
+
+* Bugfix - Use Domain's EventStore connection details for clearing events after test runs
+
 0.9.0
 -----
 
 * Output VO values as nested dicts instead of a forced flat structure
 * Enclose DAOs within repositories to encourage DB interaction solely through repos
 * Remove `remove` method from repository to discourage hard deletes
 * Manage concurrency with Aggregate versions
```

### Comparing `protean-0.9.0/src/protean.egg-info/SOURCES.txt` & `protean-0.9.1/src/protean.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/src/protean.egg-info/requires.txt` & `protean-0.9.1/src/protean.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/broker/celery_broker/config.py` & `protean-0.9.1/tests/adapters/broker/celery_broker/config.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/broker/celery_broker/conftest.py` & `protean-0.9.1/tests/adapters/broker/celery_broker/conftest.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/broker/celery_broker/elements.py` & `protean-0.9.1/tests/adapters/broker/celery_broker/elements.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/broker/celery_broker/test_subscriber.py` & `protean-0.9.1/tests/adapters/broker/celery_broker/test_subscriber.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/broker/celery_broker/tests.py` & `protean-0.9.1/tests/adapters/broker/celery_broker/tests.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/broker/redis_broker/config.py` & `protean-0.9.1/tests/adapters/broker/redis_broker/config.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/broker/redis_broker/conftest.py` & `protean-0.9.1/tests/adapters/broker/redis_broker/conftest.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/broker/redis_broker/elements.py` & `protean-0.9.1/tests/adapters/broker/redis_broker/elements.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/broker/redis_broker/tests.py` & `protean-0.9.1/tests/adapters/broker/redis_broker/tests.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/cache/redis_cache/config.py` & `protean-0.9.1/tests/adapters/cache/redis_cache/config.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/cache/redis_cache/conftest.py` & `protean-0.9.1/tests/adapters/cache/redis_cache/conftest.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/cache/redis_cache/tests.py` & `protean-0.9.1/tests/adapters/cache/redis_cache/tests.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/email/sendgrid_email/config.py` & `protean-0.9.1/tests/adapters/email/sendgrid_email/config.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/email/sendgrid_email/conftest.py` & `protean-0.9.1/tests/adapters/email/sendgrid_email/conftest.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/email/sendgrid_email/elements.py` & `protean-0.9.1/tests/adapters/email/sendgrid_email/elements.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/email/sendgrid_email/tests.py` & `protean-0.9.1/tests/adapters/email/sendgrid_email/tests.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/event_store/memory_event_store/test_reading_from_memory_event_store.py` & `protean-0.9.1/tests/adapters/event_store/memory_event_store/test_reading_from_memory_event_store.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/event_store/memory_event_store/test_writing_to_memory_event_store.py` & `protean-0.9.1/tests/adapters/event_store/memory_event_store/test_writing_to_memory_event_store.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/event_store/message_db_event_store/config.py` & `protean-0.9.1/tests/adapters/event_store/message_db_event_store/config.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/event_store/message_db_event_store/conftest.py` & `protean-0.9.1/tests/adapters/event_store/message_db_event_store/conftest.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/event_store/message_db_event_store/tests.py` & `protean-0.9.1/tests/adapters/event_store/message_db_event_store/tests.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/model/dict_model/elements.py` & `protean-0.9.1/tests/adapters/model/dict_model/elements.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/model/dict_model/tests.py` & `protean-0.9.1/tests/adapters/model/dict_model/tests.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/model/elasticsearch_model/config.py` & `protean-0.9.1/tests/adapters/model/elasticsearch_model/config.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/model/elasticsearch_model/conftest.py` & `protean-0.9.1/tests/adapters/model/elasticsearch_model/conftest.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/model/elasticsearch_model/elements.py` & `protean-0.9.1/tests/adapters/model/elasticsearch_model/elements.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/model/elasticsearch_model/tests.py` & `protean-0.9.1/tests/adapters/model/elasticsearch_model/tests.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/model/sqlalchemy_model/postgresql/config.py` & `protean-0.9.1/tests/adapters/model/sqlalchemy_model/postgresql/config.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/model/sqlalchemy_model/postgresql/conftest.py` & `protean-0.9.1/tests/adapters/model/sqlalchemy_model/postgresql/conftest.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/model/sqlalchemy_model/postgresql/elements.py` & `protean-0.9.1/tests/adapters/model/sqlalchemy_model/postgresql/elements.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/model/sqlalchemy_model/postgresql/test_array_datatype.py` & `protean-0.9.1/tests/adapters/model/sqlalchemy_model/postgresql/test_array_datatype.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/model/sqlalchemy_model/postgresql/test_json_datatype.py` & `protean-0.9.1/tests/adapters/model/sqlalchemy_model/postgresql/test_json_datatype.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/model/sqlalchemy_model/postgresql/test_list_datatype.py` & `protean-0.9.1/tests/adapters/model/sqlalchemy_model/postgresql/test_list_datatype.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/model/sqlalchemy_model/postgresql/test_lookups.py` & `protean-0.9.1/tests/adapters/model/sqlalchemy_model/postgresql/test_lookups.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/model/sqlalchemy_model/postgresql/test_model.py` & `protean-0.9.1/tests/adapters/model/sqlalchemy_model/postgresql/test_model.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/model/sqlalchemy_model/sqlite/config.py` & `protean-0.9.1/tests/adapters/model/sqlalchemy_model/sqlite/config.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/model/sqlalchemy_model/sqlite/conftest.py` & `protean-0.9.1/tests/adapters/model/sqlalchemy_model/sqlite/conftest.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/model/sqlalchemy_model/sqlite/elements.py` & `protean-0.9.1/tests/adapters/model/sqlalchemy_model/sqlite/elements.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/model/sqlalchemy_model/sqlite/test_array_datatype.py` & `protean-0.9.1/tests/adapters/model/sqlalchemy_model/sqlite/test_array_datatype.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/model/sqlalchemy_model/sqlite/test_json_datatype.py` & `protean-0.9.1/tests/adapters/model/sqlalchemy_model/sqlite/test_json_datatype.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/model/sqlalchemy_model/sqlite/test_model.py` & `protean-0.9.1/tests/adapters/model/sqlalchemy_model/sqlite/test_model.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/repository/elasticsearch_repo/config.py` & `protean-0.9.1/tests/adapters/repository/elasticsearch_repo/config.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/repository/elasticsearch_repo/conftest.py` & `protean-0.9.1/tests/adapters/repository/elasticsearch_repo/conftest.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/repository/elasticsearch_repo/elements.py` & `protean-0.9.1/tests/adapters/repository/elasticsearch_repo/elements.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/repository/elasticsearch_repo/test_dao.py` & `protean-0.9.1/tests/adapters/repository/elasticsearch_repo/test_dao.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/repository/elasticsearch_repo/test_lookup.py` & `protean-0.9.1/tests/adapters/repository/elasticsearch_repo/test_lookup.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/repository/elasticsearch_repo/test_provider.py` & `protean-0.9.1/tests/adapters/repository/elasticsearch_repo/test_provider.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/repository/elasticsearch_repo/test_query.py` & `protean-0.9.1/tests/adapters/repository/elasticsearch_repo/test_query.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/repository/elasticsearch_repo/test_repo.py` & `protean-0.9.1/tests/adapters/repository/elasticsearch_repo/test_repo.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/repository/memory/test_any_operator.py` & `protean-0.9.1/tests/adapters/repository/memory/test_any_operator.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/repository/memory/test_in_operator.py` & `protean-0.9.1/tests/adapters/repository/memory/test_in_operator.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/repository/memory/test_lookups.py` & `protean-0.9.1/tests/adapters/repository/memory/test_lookups.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/repository/memory/test_sorting_on_none_values.py` & `protean-0.9.1/tests/adapters/repository/memory/test_sorting_on_none_values.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/postgresql/config.py` & `protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/postgresql/config.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/postgresql/conftest.py` & `protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/postgresql/conftest.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/postgresql/elements.py` & `protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/postgresql/elements.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/postgresql/test_associations.py` & `protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/postgresql/test_associations.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/postgresql/test_dao.py` & `protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/postgresql/test_dao.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/postgresql/test_persistence.py` & `protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/postgresql/test_persistence.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/postgresql/test_provider.py` & `protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/postgresql/test_provider.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/postgresql/test_transactions.py` & `protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/postgresql/test_transactions.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/sqlite/config.py` & `protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/sqlite/config.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/sqlite/conftest.py` & `protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/sqlite/conftest.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/sqlite/elements.py` & `protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/sqlite/elements.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/sqlite/test_dao.py` & `protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/sqlite/test_dao.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/sqlite/test_provider.py` & `protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/sqlite/test_provider.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/repository/sqlalchemy_repo/sqlite/test_transactions.py` & `protean-0.9.1/tests/adapters/repository/sqlalchemy_repo/sqlite/test_transactions.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/adapters/repository/test_generic.py` & `protean-0.9.1/tests/adapters/repository/test_generic.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/aggregate/aggregate_elements.py` & `protean-0.9.1/tests/aggregate/aggregate_elements.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/aggregate/elements.py` & `protean-0.9.1/tests/aggregate/elements.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/aggregate/test_aggregate_abstraction.py` & `protean-0.9.1/tests/aggregate/test_aggregate_abstraction.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/aggregate/test_aggregate_association.py` & `protean-0.9.1/tests/aggregate/test_aggregate_association.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/aggregate/test_aggregate_events.py` & `protean-0.9.1/tests/aggregate/test_aggregate_events.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/aggregate/test_aggregate_initialization.py` & `protean-0.9.1/tests/aggregate/test_aggregate_initialization.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/aggregate/test_aggregate_properties.py` & `protean-0.9.1/tests/aggregate/test_aggregate_properties.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/aggregate/test_aggregate_reference_field.py` & `protean-0.9.1/tests/aggregate/test_aggregate_reference_field.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/aggregate/test_aggregate_registration.py` & `protean-0.9.1/tests/aggregate/test_aggregate_registration.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/aggregate/test_aggregate_state.py` & `protean-0.9.1/tests/aggregate/test_aggregate_state.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/aggregate/test_aggregates_with_entities.py` & `protean-0.9.1/tests/aggregate/test_aggregates_with_entities.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/aggregate/test_aggregates_with_value_objects.py` & `protean-0.9.1/tests/aggregate/test_aggregates_with_value_objects.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/aggregate/test_as_dict.py` & `protean-0.9.1/tests/aggregate/test_as_dict.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/application_service/tests.py` & `protean-0.9.1/tests/application_service/tests.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/cache/tests.py` & `protean-0.9.1/tests/cache/tests.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/command/test_automatic_stream_association.py` & `protean-0.9.1/tests/command/test_automatic_stream_association.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/command/test_command_identity.py` & `protean-0.9.1/tests/command/test_command_identity.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/command/test_command_meta.py` & `protean-0.9.1/tests/command/test_command_meta.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/command_handler/test_command_handler_options.py` & `protean-0.9.1/tests/command_handler/test_command_handler_options.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/command_handler/test_command_handler_registration.py` & `protean-0.9.1/tests/command_handler/test_command_handler_registration.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/command_handler/test_handle_decorator_in_command_handlers.py` & `protean-0.9.1/tests/command_handler/test_handle_decorator_in_command_handlers.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/command_handler/test_inline_command_processing.py` & `protean-0.9.1/tests/command_handler/test_inline_command_processing.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/command_handler/test_retrieving_handlers_by_command.py` & `protean-0.9.1/tests/command_handler/test_retrieving_handlers_by_command.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/command_handler/test_uow_around_command_handlers.py` & `protean-0.9.1/tests/command_handler/test_uow_around_command_handlers.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/config.py` & `protean-0.9.1/tests/config.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/configuration/tests.py` & `protean-0.9.1/tests/configuration/tests.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/conftest.py` & `protean-0.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/container/test_options.py` & `protean-0.9.1/tests/container/test_options.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/context/tests.py` & `protean-0.9.1/tests/context/tests.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/dao/elements.py` & `protean-0.9.1/tests/dao/elements.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/dao/test_basics.py` & `protean-0.9.1/tests/dao/test_basics.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/dao/test_delete.py` & `protean-0.9.1/tests/dao/test_delete.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/dao/test_retrieval.py` & `protean-0.9.1/tests/dao/test_retrieval.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/dao/test_save.py` & `protean-0.9.1/tests/dao/test_save.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/dao/test_update.py` & `protean-0.9.1/tests/dao/test_update.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/dao/test_validations.py` & `protean-0.9.1/tests/dao/test_validations.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/domain/test_config_immutability.py` & `protean-0.9.1/tests/domain/test_config_immutability.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/domain/tests.py` & `protean-0.9.1/tests/domain/tests.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/domain_service/tests.py` & `protean-0.9.1/tests/domain_service/tests.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/email_provider/elements.py` & `protean-0.9.1/tests/email_provider/elements.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/email_provider/tests.py` & `protean-0.9.1/tests/email_provider/tests.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/entity/elements.py` & `protean-0.9.1/tests/entity/elements.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/entity/test_entity.py` & `protean-0.9.1/tests/entity/test_entity.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/entity/test_entity_meta.py` & `protean-0.9.1/tests/entity/test_entity_meta.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/entity/test_entity_properties.py` & `protean-0.9.1/tests/entity/test_entity_properties.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/entity/test_entity_registration.py` & `protean-0.9.1/tests/entity/test_entity_registration.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/entity/test_fields.py` & `protean-0.9.1/tests/entity/test_fields.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/entity/test_lifecycle_methods.py` & `protean-0.9.1/tests/entity/test_lifecycle_methods.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/entity/test_temp.py` & `protean-0.9.1/tests/entity/test_temp.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/event/elements.py` & `protean-0.9.1/tests/event/elements.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/event/test_automatic_stream_association.py` & `protean-0.9.1/tests/event/test_automatic_stream_association.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/event/test_event_identity.py` & `protean-0.9.1/tests/event/test_event_identity.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/event/test_event_meta.py` & `protean-0.9.1/tests/event/test_event_meta.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/event/test_raising_events.py` & `protean-0.9.1/tests/event/test_raising_events.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/event/test_serialization.py` & `protean-0.9.1/tests/event/test_serialization.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/event/tests.py` & `protean-0.9.1/tests/event/tests.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/event_handler/test_any_event_handler.py` & `protean-0.9.1/tests/event_handler/test_any_event_handler.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/event_handler/test_event_handler_options.py` & `protean-0.9.1/tests/event_handler/test_event_handler_options.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/event_handler/test_event_handler_registration.py` & `protean-0.9.1/tests/event_handler/test_event_handler_registration.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/event_handler/test_handle_decorator_in_event_handlers.py` & `protean-0.9.1/tests/event_handler/test_handle_decorator_in_event_handlers.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/event_handler/test_retrieving_handlers_by_event.py` & `protean-0.9.1/tests/event_handler/test_retrieving_handlers_by_event.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/event_handler/test_uow_around_event_handlers.py` & `protean-0.9.1/tests/event_handler/test_uow_around_event_handlers.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/event_sourced_aggregates/test_applying_events.py` & `protean-0.9.1/tests/event_sourced_aggregates/test_applying_events.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/event_sourced_aggregates/test_event_association_with_aggregate.py` & `protean-0.9.1/tests/event_sourced_aggregates/test_event_association_with_aggregate.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/event_sourced_aggregates/test_event_sourced_aggregate_options.py` & `protean-0.9.1/tests/event_sourced_aggregates/test_event_sourced_aggregate_options.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/event_sourced_aggregates/test_event_sourced_aggregate_registration.py` & `protean-0.9.1/tests/event_sourced_aggregates/test_event_sourced_aggregate_registration.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/event_sourced_aggregates/test_expected_version_error.py` & `protean-0.9.1/tests/event_sourced_aggregates/test_expected_version_error.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/event_sourced_aggregates/test_raising_events_from_within_aggregates.py` & `protean-0.9.1/tests/event_sourced_aggregates/test_raising_events_from_within_aggregates.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/event_sourced_repository/test_loading_aggregates.py` & `protean-0.9.1/tests/event_sourced_repository/test_loading_aggregates.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/event_sourced_repository/test_retrieving_event_sourced_repository.py` & `protean-0.9.1/tests/event_sourced_repository/test_retrieving_event_sourced_repository.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/event_store/test_appending_aggregate_events.py` & `protean-0.9.1/tests/event_store/test_appending_aggregate_events.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/event_store/test_appending_commands.py` & `protean-0.9.1/tests/event_store/test_appending_commands.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/event_store/test_appending_events.py` & `protean-0.9.1/tests/event_store/test_appending_events.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/event_store/test_reading_all_streams.py` & `protean-0.9.1/tests/event_store/test_reading_all_streams.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/event_store/test_reading_messages.py` & `protean-0.9.1/tests/event_store/test_reading_messages.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/event_store/test_snapshotting.py` & `protean-0.9.1/tests/event_store/test_snapshotting.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/event_store/test_streams_initialization.py` & `protean-0.9.1/tests/event_store/test_streams_initialization.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/field/elements.py` & `protean-0.9.1/tests/field/elements.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/field/test_associations.py` & `protean-0.9.1/tests/field/test_associations.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/field/test_auto.py` & `protean-0.9.1/tests/field/test_auto.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/field/test_field_types.py` & `protean-0.9.1/tests/field/test_field_types.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/field/test_field_validators.py` & `protean-0.9.1/tests/field/test_field_validators.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/field/test_identifier.py` & `protean-0.9.1/tests/field/test_identifier.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/field/test_reference.py` & `protean-0.9.1/tests/field/test_reference.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/field/tests.py` & `protean-0.9.1/tests/field/tests.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/identity/config_int.py` & `protean-0.9.1/tests/identity/config_int.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/identity/config_string.py` & `protean-0.9.1/tests/identity/config_string.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/identity/config_uuid.py` & `protean-0.9.1/tests/identity/config_uuid.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/identity/conftest.py` & `protean-0.9.1/tests/identity/conftest.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/identity/tests.py` & `protean-0.9.1/tests/identity/tests.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/message/test_message_to_object.py` & `protean-0.9.1/tests/message/test_message_to_object.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/message/test_object_to_message.py` & `protean-0.9.1/tests/message/test_object_to_message.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/message/test_origin_stream_name_in_metadata.py` & `protean-0.9.1/tests/message/test_origin_stream_name_in_metadata.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/provider/tests.py` & `protean-0.9.1/tests/provider/tests.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/query/test_conjunctions.py` & `protean-0.9.1/tests/query/test_conjunctions.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/query/test_q.py` & `protean-0.9.1/tests/query/test_q.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/query/test_queryset.py` & `protean-0.9.1/tests/query/test_queryset.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/reflection/test_has_id_field.py` & `protean-0.9.1/tests/reflection/test_has_id_field.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/repository/child_entities.py` & `protean-0.9.1/tests/repository/child_entities.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/repository/elements.py` & `protean-0.9.1/tests/repository/elements.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/repository/test_aggregate_persistence.py` & `protean-0.9.1/tests/repository/test_aggregate_persistence.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/repository/test_child_persistence.py` & `protean-0.9.1/tests/repository/test_child_persistence.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/repository/test_providers.py` & `protean-0.9.1/tests/repository/test_providers.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/repository/test_repository_registration.py` & `protean-0.9.1/tests/repository/test_repository_registration.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/repository/test_resultset.py` & `protean-0.9.1/tests/repository/test_resultset.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/repository/test_tracking_seen_objects.py` & `protean-0.9.1/tests/repository/test_tracking_seen_objects.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/repository/tests.py` & `protean-0.9.1/tests/repository/tests.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/serializer/tests.py` & `protean-0.9.1/tests/serializer/tests.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/server/dummy_domain.py` & `protean-0.9.1/tests/server/dummy_domain.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/server/test_any_event_handler.py` & `protean-0.9.1/tests/server/test_any_event_handler.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/server/test_command_handler_subscription.py` & `protean-0.9.1/tests/server/test_command_handler_subscription.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/server/test_command_handling.py` & `protean-0.9.1/tests/server/test_command_handling.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/server/test_engine_initialization.py` & `protean-0.9.1/tests/server/test_engine_initialization.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/server/test_event_handler_subscription.py` & `protean-0.9.1/tests/server/test_event_handler_subscription.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/server/test_event_handling.py` & `protean-0.9.1/tests/server/test_event_handling.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/server/test_handling_all_events.py` & `protean-0.9.1/tests/server/test_handling_all_events.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/subscription/test_message_filtering_with_origin_stream.py` & `protean-0.9.1/tests/subscription/test_message_filtering_with_origin_stream.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/subscription/test_message_handover_to_engine.py` & `protean-0.9.1/tests/subscription/test_message_handover_to_engine.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/subscription/test_no_message_filtering.py` & `protean-0.9.1/tests/subscription/test_no_message_filtering.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/test_aggregates.py` & `protean-0.9.1/tests/test_aggregates.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/test_brokers.py` & `protean-0.9.1/tests/test_brokers.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/test_cli.py` & `protean-0.9.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/test_commands.py` & `protean-0.9.1/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/test_config.py` & `protean-0.9.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/test_containers.py` & `protean-0.9.1/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/test_other.py` & `protean-0.9.1/tests/test_other.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/test_registry.py` & `protean-0.9.1/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/test_subscribers.py` & `protean-0.9.1/tests/test_subscribers.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/unit_of_work/aggregate_elements.py` & `protean-0.9.1/tests/unit_of_work/aggregate_elements.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/unit_of_work/test_child_object_persistence.py` & `protean-0.9.1/tests/unit_of_work/test_child_object_persistence.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/unit_of_work/test_inline_event_processing.py` & `protean-0.9.1/tests/unit_of_work/test_inline_event_processing.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/unit_of_work/test_nested_inline_event_processing.py` & `protean-0.9.1/tests/unit_of_work/test_nested_inline_event_processing.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/unit_of_work/test_storing_events_on_commit.py` & `protean-0.9.1/tests/unit_of_work/test_storing_events_on_commit.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/unit_of_work/test_uow_transactions.py` & `protean-0.9.1/tests/unit_of_work/test_uow_transactions.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/unit_of_work/tests.py` & `protean-0.9.1/tests/unit_of_work/tests.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/value_object/elements.py` & `protean-0.9.1/tests/value_object/elements.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/value_object/test_lifecycle_methods.py` & `protean-0.9.1/tests/value_object/test_lifecycle_methods.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/value_object/test_to_dict.py` & `protean-0.9.1/tests/value_object/test_to_dict.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/value_object/tests.py` & `protean-0.9.1/tests/value_object/tests.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/views/test_view_validations_for_fields.py` & `protean-0.9.1/tests/views/test_view_validations_for_fields.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tests/views/tests.py` & `protean-0.9.1/tests/views/tests.py`

 * *Files identical despite different names*

### Comparing `protean-0.9.0/tox.ini` & `protean-0.9.1/tox.ini`

 * *Files identical despite different names*

