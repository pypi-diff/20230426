# Comparing `tmp/air_drf_relation-0.5.6.tar.gz` & `tmp/air_drf_relation-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "air_drf_relation-0.5.6.tar", last modified: Tue Apr 18 16:00:51 2023, max compression
+gzip compressed data, was "air_drf_relation-0.5.7.tar", last modified: Tue Apr 25 22:12:23 2023, max compression
```

## Comparing `air_drf_relation-0.5.6.tar` & `air_drf_relation-0.5.7.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-18 16:00:51.264019 air_drf_relation-0.5.6/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1074 2021-06-27 18:03:44.000000 air_drf_relation-0.5.6/LICENSE
--rw-r--r--   0 kirillcelisev   (501) staff       (20)       87 2021-06-27 19:16:11.000000 air_drf_relation-0.5.6/MANIFEST.in
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     8696 2023-04-18 16:00:51.264165 air_drf_relation-0.5.6/PKG-INFO
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     6483 2022-05-26 10:52:59.000000 air_drf_relation-0.5.6/README.md
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-18 16:00:51.250992 air_drf_relation-0.5.6/air_drf_relation/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      346 2022-05-26 10:45:07.000000 air_drf_relation-0.5.6/air_drf_relation/__init__.py
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-18 16:00:51.255461 air_drf_relation-0.5.6/air_drf_relation/__pycache__/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      492 2022-05-26 10:48:51.000000 air_drf_relation-0.5.6/air_drf_relation/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1452 2022-05-04 08:27:13.000000 air_drf_relation-0.5.6/air_drf_relation/__pycache__/context_builder.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      885 2022-05-04 08:28:39.000000 air_drf_relation-0.5.6/air_drf_relation/__pycache__/decorators.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     3466 2022-03-03 07:13:47.000000 air_drf_relation-0.5.6/air_drf_relation/__pycache__/extra_kwargs.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     2441 2022-05-26 11:22:49.000000 air_drf_relation-0.5.6/air_drf_relation/__pycache__/fields.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1236 2022-05-04 08:27:13.000000 air_drf_relation-0.5.6/air_drf_relation/__pycache__/filters.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1662 2023-04-18 14:12:35.000000 air_drf_relation-0.5.6/air_drf_relation/__pycache__/model_fields.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     5012 2023-02-11 11:33:06.000000 air_drf_relation-0.5.6/air_drf_relation/__pycache__/preload_objects_manager.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     3021 2023-02-08 21:41:02.000000 air_drf_relation-0.5.6/air_drf_relation/__pycache__/queryset_optimization.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)    11176 2023-04-18 15:58:49.000000 air_drf_relation-0.5.6/air_drf_relation/__pycache__/serializers.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      332 2022-05-26 10:48:51.000000 air_drf_relation-0.5.6/air_drf_relation/__pycache__/settings.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1157 2023-04-18 15:58:32.000000 air_drf_relation-0.5.6/air_drf_relation/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      832 2022-05-04 08:26:21.000000 air_drf_relation-0.5.6/air_drf_relation/context_builder.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      696 2022-05-04 07:31:58.000000 air_drf_relation-0.5.6/air_drf_relation/decorators.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     4316 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/air_drf_relation/extra_kwargs.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1855 2022-05-26 11:22:46.000000 air_drf_relation-0.5.6/air_drf_relation/fields.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      690 2022-05-04 07:35:13.000000 air_drf_relation-0.5.6/air_drf_relation/filters.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1137 2023-04-18 14:12:13.000000 air_drf_relation-0.5.6/air_drf_relation/model_fields.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     5763 2023-02-11 11:19:46.000000 air_drf_relation-0.5.6/air_drf_relation/preload_objects_manager.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     3103 2023-02-08 21:41:00.000000 air_drf_relation-0.5.6/air_drf_relation/queryset_optimization.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)    11007 2023-04-18 15:58:48.000000 air_drf_relation-0.5.6/air_drf_relation/serializers.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      240 2022-05-26 10:47:07.000000 air_drf_relation-0.5.6/air_drf_relation/settings.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      786 2023-04-18 15:58:31.000000 air_drf_relation-0.5.6/air_drf_relation/utils.py
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-18 16:00:51.252097 air_drf_relation-0.5.6/air_drf_relation.egg-info/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     8696 2023-04-18 16:00:51.000000 air_drf_relation-0.5.6/air_drf_relation.egg-info/PKG-INFO
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     2343 2023-04-18 16:00:51.000000 air_drf_relation-0.5.6/air_drf_relation.egg-info/SOURCES.txt
--rw-r--r--   0 kirillcelisev   (501) staff       (20)        1 2023-04-18 16:00:51.000000 air_drf_relation-0.5.6/air_drf_relation.egg-info/dependency_links.txt
--rw-r--r--   0 kirillcelisev   (501) staff       (20)        1 2023-02-08 22:24:16.000000 air_drf_relation-0.5.6/air_drf_relation.egg-info/not-zip-safe
--rw-r--r--   0 kirillcelisev   (501) staff       (20)       41 2023-04-18 16:00:51.000000 air_drf_relation-0.5.6/air_drf_relation.egg-info/requires.txt
--rw-r--r--   0 kirillcelisev   (501) staff       (20)       50 2023-04-18 16:00:51.000000 air_drf_relation-0.5.6/air_drf_relation.egg-info/top_level.txt
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-18 16:00:51.256624 air_drf_relation-0.5.6/device/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/device/__init__.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/device/admin.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      144 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/device/apps.py
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-18 16:00:51.257058 air_drf_relation-0.5.6/device/migrations/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      698 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/device/migrations/0001_initial.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      371 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/device/migrations/0002_alter_device_code.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/device/migrations/__init__.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      251 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/device/models.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      888 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/device/serializers.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     2505 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/device/tests.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/device/views.py
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-18 16:00:51.258708 air_drf_relation-0.5.6/film/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2023-02-08 21:16:41.000000 air_drf_relation-0.5.6/film/__init__.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2023-02-08 21:16:41.000000 air_drf_relation-0.5.6/film/admin.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      140 2023-02-08 21:16:41.000000 air_drf_relation-0.5.6/film/apps.py
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-18 16:00:51.259171 air_drf_relation-0.5.6/film/migrations/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1093 2023-02-08 22:30:35.000000 air_drf_relation-0.5.6/film/migrations/0001_initial.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2023-02-08 21:16:41.000000 air_drf_relation-0.5.6/film/migrations/__init__.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      586 2023-02-11 10:43:36.000000 air_drf_relation-0.5.6/film/models.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      877 2023-02-08 22:29:38.000000 air_drf_relation-0.5.6/film/serializers.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1845 2023-04-18 14:12:56.000000 air_drf_relation-0.5.6/film/tests.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      163 2023-02-08 23:17:50.000000 air_drf_relation-0.5.6/film/urls.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      217 2023-02-08 23:17:39.000000 air_drf_relation-0.5.6/film/views.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)       73 2023-04-18 16:00:51.264977 air_drf_relation-0.5.6/setup.cfg
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      886 2023-04-18 16:00:49.000000 air_drf_relation-0.5.6/setup.py
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-18 16:00:51.260650 air_drf_relation-0.5.6/table/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-05-13 12:51:44.000000 air_drf_relation-0.5.6/table/__init__.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2022-05-13 12:51:44.000000 air_drf_relation-0.5.6/table/admin.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      142 2022-05-13 12:51:44.000000 air_drf_relation-0.5.6/table/apps.py
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-18 16:00:51.261823 air_drf_relation-0.5.6/table/migrations/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      885 2022-05-13 12:54:15.000000 air_drf_relation-0.5.6/table/migrations/0001_initial.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      417 2022-05-13 12:58:02.000000 air_drf_relation-0.5.6/table/migrations/0002_table_name.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1820 2022-05-13 15:42:11.000000 air_drf_relation-0.5.6/table/migrations/0003_auto_20220513_1542.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      545 2022-05-13 15:43:10.000000 air_drf_relation-0.5.6/table/migrations/0004_material_company.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-05-13 12:51:44.000000 air_drf_relation-0.5.6/table/migrations/__init__.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      916 2022-05-13 15:43:05.000000 air_drf_relation-0.5.6/table/models.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1342 2023-02-11 11:37:09.000000 air_drf_relation-0.5.6/table/serializers.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     5277 2023-04-18 14:13:22.000000 air_drf_relation-0.5.6/table/tests.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2022-05-13 12:51:44.000000 air_drf_relation-0.5.6/table/views.py
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-18 16:00:51.263100 air_drf_relation-0.5.6/task/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/task/__init__.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/task/admin.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      140 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/task/apps.py
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-18 16:00:51.263920 air_drf_relation-0.5.6/task/migrations/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      558 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/task/migrations/0001_initial.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      387 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/task/migrations/0002_alter_task_image.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      598 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/task/migrations/0003_tag.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      512 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/task/migrations/0004_tag_task.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/task/migrations/__init__.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      391 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/task/models.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      462 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/task/serializers.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1346 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/task/tests.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      163 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/task/urls.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      935 2022-03-03 07:12:43.000000 air_drf_relation-0.5.6/task/views.py
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-25 22:12:23.996384 air_drf_relation-0.5.7/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1074 2021-06-27 18:03:44.000000 air_drf_relation-0.5.7/LICENSE
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)       87 2021-06-27 19:16:11.000000 air_drf_relation-0.5.7/MANIFEST.in
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     8696 2023-04-25 22:12:23.996544 air_drf_relation-0.5.7/PKG-INFO
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     6483 2022-05-26 10:52:59.000000 air_drf_relation-0.5.7/README.md
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-25 22:12:23.978676 air_drf_relation-0.5.7/air_drf_relation/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      346 2022-05-26 10:45:07.000000 air_drf_relation-0.5.7/air_drf_relation/__init__.py
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-25 22:12:23.984017 air_drf_relation-0.5.7/air_drf_relation/__pycache__/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      492 2022-05-26 10:48:51.000000 air_drf_relation-0.5.7/air_drf_relation/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1452 2022-05-04 08:27:13.000000 air_drf_relation-0.5.7/air_drf_relation/__pycache__/context_builder.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      885 2022-05-04 08:28:39.000000 air_drf_relation-0.5.7/air_drf_relation/__pycache__/decorators.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     3466 2022-03-03 07:13:47.000000 air_drf_relation-0.5.7/air_drf_relation/__pycache__/extra_kwargs.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     2441 2022-05-26 11:22:49.000000 air_drf_relation-0.5.7/air_drf_relation/__pycache__/fields.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1236 2022-05-04 08:27:13.000000 air_drf_relation-0.5.7/air_drf_relation/__pycache__/filters.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1662 2023-04-18 14:12:35.000000 air_drf_relation-0.5.7/air_drf_relation/__pycache__/model_fields.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     5012 2023-02-11 11:33:06.000000 air_drf_relation-0.5.7/air_drf_relation/__pycache__/preload_objects_manager.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     3021 2023-02-08 21:41:02.000000 air_drf_relation-0.5.7/air_drf_relation/__pycache__/queryset_optimization.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)    11176 2023-04-18 15:58:49.000000 air_drf_relation-0.5.7/air_drf_relation/__pycache__/serializers.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      332 2022-05-26 10:48:51.000000 air_drf_relation-0.5.7/air_drf_relation/__pycache__/settings.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1157 2023-04-18 15:58:32.000000 air_drf_relation-0.5.7/air_drf_relation/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      832 2022-05-04 08:26:21.000000 air_drf_relation-0.5.7/air_drf_relation/context_builder.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      696 2022-05-04 07:31:58.000000 air_drf_relation-0.5.7/air_drf_relation/decorators.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     4316 2022-03-03 07:12:43.000000 air_drf_relation-0.5.7/air_drf_relation/extra_kwargs.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1855 2022-05-26 11:22:46.000000 air_drf_relation-0.5.7/air_drf_relation/fields.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      690 2022-05-04 07:35:13.000000 air_drf_relation-0.5.7/air_drf_relation/filters.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1137 2023-04-18 14:12:13.000000 air_drf_relation-0.5.7/air_drf_relation/model_fields.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     5763 2023-02-11 11:19:46.000000 air_drf_relation-0.5.7/air_drf_relation/preload_objects_manager.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     3103 2023-02-08 21:41:00.000000 air_drf_relation-0.5.7/air_drf_relation/queryset_optimization.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)    11007 2023-04-18 15:58:48.000000 air_drf_relation-0.5.7/air_drf_relation/serializers.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      240 2022-05-26 10:47:07.000000 air_drf_relation-0.5.7/air_drf_relation/settings.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      873 2023-04-25 22:09:43.000000 air_drf_relation-0.5.7/air_drf_relation/utils.py
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-25 22:12:23.979917 air_drf_relation-0.5.7/air_drf_relation.egg-info/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     8696 2023-04-25 22:12:23.000000 air_drf_relation-0.5.7/air_drf_relation.egg-info/PKG-INFO
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     2343 2023-04-25 22:12:23.000000 air_drf_relation-0.5.7/air_drf_relation.egg-info/SOURCES.txt
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)        1 2023-04-25 22:12:23.000000 air_drf_relation-0.5.7/air_drf_relation.egg-info/dependency_links.txt
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)        1 2023-02-08 22:24:16.000000 air_drf_relation-0.5.7/air_drf_relation.egg-info/not-zip-safe
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)       80 2023-04-25 22:12:23.000000 air_drf_relation-0.5.7/air_drf_relation.egg-info/requires.txt
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)       50 2023-04-25 22:12:23.000000 air_drf_relation-0.5.7/air_drf_relation.egg-info/top_level.txt
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-25 22:12:23.986058 air_drf_relation-0.5.7/device/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-03-03 07:12:43.000000 air_drf_relation-0.5.7/device/__init__.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2022-03-03 07:12:43.000000 air_drf_relation-0.5.7/device/admin.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      144 2022-03-03 07:12:43.000000 air_drf_relation-0.5.7/device/apps.py
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-25 22:12:23.986793 air_drf_relation-0.5.7/device/migrations/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      698 2022-03-03 07:12:43.000000 air_drf_relation-0.5.7/device/migrations/0001_initial.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      371 2022-03-03 07:12:43.000000 air_drf_relation-0.5.7/device/migrations/0002_alter_device_code.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-03-03 07:12:43.000000 air_drf_relation-0.5.7/device/migrations/__init__.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      251 2022-03-03 07:12:43.000000 air_drf_relation-0.5.7/device/models.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      888 2022-03-03 07:12:43.000000 air_drf_relation-0.5.7/device/serializers.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     2505 2022-03-03 07:12:43.000000 air_drf_relation-0.5.7/device/tests.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2022-03-03 07:12:43.000000 air_drf_relation-0.5.7/device/views.py
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-25 22:12:23.989406 air_drf_relation-0.5.7/film/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2023-02-08 21:16:41.000000 air_drf_relation-0.5.7/film/__init__.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2023-02-08 21:16:41.000000 air_drf_relation-0.5.7/film/admin.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      140 2023-02-08 21:16:41.000000 air_drf_relation-0.5.7/film/apps.py
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-25 22:12:23.989961 air_drf_relation-0.5.7/film/migrations/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1093 2023-02-08 22:30:35.000000 air_drf_relation-0.5.7/film/migrations/0001_initial.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2023-02-08 21:16:41.000000 air_drf_relation-0.5.7/film/migrations/__init__.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      586 2023-02-11 10:43:36.000000 air_drf_relation-0.5.7/film/models.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      877 2023-02-08 22:29:38.000000 air_drf_relation-0.5.7/film/serializers.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1845 2023-04-18 14:12:56.000000 air_drf_relation-0.5.7/film/tests.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      163 2023-02-08 23:17:50.000000 air_drf_relation-0.5.7/film/urls.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      217 2023-02-08 23:17:39.000000 air_drf_relation-0.5.7/film/views.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)       73 2023-04-25 22:12:23.997182 air_drf_relation-0.5.7/setup.cfg
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      951 2023-04-25 22:11:20.000000 air_drf_relation-0.5.7/setup.py
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-25 22:12:23.991922 air_drf_relation-0.5.7/table/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-05-13 12:51:44.000000 air_drf_relation-0.5.7/table/__init__.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2022-05-13 12:51:44.000000 air_drf_relation-0.5.7/table/admin.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      142 2022-05-13 12:51:44.000000 air_drf_relation-0.5.7/table/apps.py
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-25 22:12:23.993739 air_drf_relation-0.5.7/table/migrations/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      885 2022-05-13 12:54:15.000000 air_drf_relation-0.5.7/table/migrations/0001_initial.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      417 2022-05-13 12:58:02.000000 air_drf_relation-0.5.7/table/migrations/0002_table_name.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1820 2022-05-13 15:42:11.000000 air_drf_relation-0.5.7/table/migrations/0003_auto_20220513_1542.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      545 2022-05-13 15:43:10.000000 air_drf_relation-0.5.7/table/migrations/0004_material_company.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-05-13 12:51:44.000000 air_drf_relation-0.5.7/table/migrations/__init__.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      916 2022-05-13 15:43:05.000000 air_drf_relation-0.5.7/table/models.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1342 2023-02-11 11:37:09.000000 air_drf_relation-0.5.7/table/serializers.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     5277 2023-04-18 14:13:22.000000 air_drf_relation-0.5.7/table/tests.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2022-05-13 12:51:44.000000 air_drf_relation-0.5.7/table/views.py
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-25 22:12:23.995305 air_drf_relation-0.5.7/task/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-03-03 07:12:43.000000 air_drf_relation-0.5.7/task/__init__.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2022-03-03 07:12:43.000000 air_drf_relation-0.5.7/task/admin.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      140 2022-03-03 07:12:43.000000 air_drf_relation-0.5.7/task/apps.py
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-04-25 22:12:23.996268 air_drf_relation-0.5.7/task/migrations/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      558 2022-03-03 07:12:43.000000 air_drf_relation-0.5.7/task/migrations/0001_initial.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      387 2022-03-03 07:12:43.000000 air_drf_relation-0.5.7/task/migrations/0002_alter_task_image.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      598 2022-03-03 07:12:43.000000 air_drf_relation-0.5.7/task/migrations/0003_tag.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      512 2022-03-03 07:12:43.000000 air_drf_relation-0.5.7/task/migrations/0004_tag_task.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-03-03 07:12:43.000000 air_drf_relation-0.5.7/task/migrations/__init__.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      391 2022-03-03 07:12:43.000000 air_drf_relation-0.5.7/task/models.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      462 2022-03-03 07:12:43.000000 air_drf_relation-0.5.7/task/serializers.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1346 2022-03-03 07:12:43.000000 air_drf_relation-0.5.7/task/tests.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      163 2022-03-03 07:12:43.000000 air_drf_relation-0.5.7/task/urls.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      935 2022-03-03 07:12:43.000000 air_drf_relation-0.5.7/task/views.py
```

### Comparing `air_drf_relation-0.5.6/LICENSE` & `air_drf_relation-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/PKG-INFO` & `air_drf_relation-0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: air_drf_relation
-Version: 0.5.6
+Version: 0.5.7
 Summary: Improved interaction with DRF relations.
 Home-page: https://github.com/bubaley/air-drf-relation
 Author: bubaley
 Author-email: bubaley.fu@gmail.com
 License: MIT
 Description: **AIR-DRF-RELATION**
```

### Comparing `air_drf_relation-0.5.6/README.md` & `air_drf_relation-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/air_drf_relation/__pycache__/context_builder.cpython-39.pyc` & `air_drf_relation-0.5.7/air_drf_relation/__pycache__/context_builder.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/air_drf_relation/__pycache__/decorators.cpython-39.pyc` & `air_drf_relation-0.5.7/air_drf_relation/__pycache__/decorators.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/air_drf_relation/__pycache__/extra_kwargs.cpython-39.pyc` & `air_drf_relation-0.5.7/air_drf_relation/__pycache__/extra_kwargs.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/air_drf_relation/__pycache__/fields.cpython-39.pyc` & `air_drf_relation-0.5.7/air_drf_relation/__pycache__/fields.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/air_drf_relation/__pycache__/filters.cpython-39.pyc` & `air_drf_relation-0.5.7/air_drf_relation/__pycache__/filters.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/air_drf_relation/__pycache__/model_fields.cpython-39.pyc` & `air_drf_relation-0.5.7/air_drf_relation/__pycache__/model_fields.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/air_drf_relation/__pycache__/preload_objects_manager.cpython-39.pyc` & `air_drf_relation-0.5.7/air_drf_relation/__pycache__/preload_objects_manager.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/air_drf_relation/__pycache__/queryset_optimization.cpython-39.pyc` & `air_drf_relation-0.5.7/air_drf_relation/__pycache__/queryset_optimization.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/air_drf_relation/__pycache__/serializers.cpython-39.pyc` & `air_drf_relation-0.5.7/air_drf_relation/__pycache__/serializers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/air_drf_relation/__pycache__/utils.cpython-39.pyc` & `air_drf_relation-0.5.7/air_drf_relation/__pycache__/utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/air_drf_relation/context_builder.py` & `air_drf_relation-0.5.7/air_drf_relation/context_builder.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/air_drf_relation/decorators.py` & `air_drf_relation-0.5.7/air_drf_relation/decorators.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/air_drf_relation/extra_kwargs.py` & `air_drf_relation-0.5.7/air_drf_relation/extra_kwargs.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/air_drf_relation/fields.py` & `air_drf_relation-0.5.7/air_drf_relation/fields.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/air_drf_relation/filters.py` & `air_drf_relation-0.5.7/air_drf_relation/filters.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/air_drf_relation/model_fields.py` & `air_drf_relation-0.5.7/air_drf_relation/model_fields.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/air_drf_relation/preload_objects_manager.py` & `air_drf_relation-0.5.7/air_drf_relation/preload_objects_manager.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/air_drf_relation/queryset_optimization.py` & `air_drf_relation-0.5.7/air_drf_relation/queryset_optimization.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/air_drf_relation/serializers.py` & `air_drf_relation-0.5.7/air_drf_relation/serializers.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/air_drf_relation/utils.py` & `air_drf_relation-0.5.7/air_drf_relation/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import uuid
-from collections.abc import Mapping, Sequence
 
 
 def get_pk_from_data(data, pk_name):
     if type(data) in [list, tuple]:
         return [v.get(pk_name) if type(v) == dict else v for v in data]
     return data.get(pk_name) if type(data) == dict else data
 
@@ -21,7 +20,15 @@
             value[k] = stringify_uuids(value[k])
     elif isinstance(value, list) and not isinstance(value, str):
         for i, v in enumerate(value):
             value[i] = stringify_uuids(v)
     elif isinstance(value, uuid.UUID):
         return str(value)
     return value
+
+
+def is_uuid(value: str) -> bool:
+    try:
+        uuid.UUID(value)
+        return True
+    except ValueError:
+        return False
```

### Comparing `air_drf_relation-0.5.6/air_drf_relation.egg-info/PKG-INFO` & `air_drf_relation-0.5.7/air_drf_relation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: air-drf-relation
-Version: 0.5.6
+Version: 0.5.7
 Summary: Improved interaction with DRF relations.
 Home-page: https://github.com/bubaley/air-drf-relation
 Author: bubaley
 Author-email: bubaley.fu@gmail.com
 License: MIT
 Description: **AIR-DRF-RELATION**
```

### Comparing `air_drf_relation-0.5.6/air_drf_relation.egg-info/SOURCES.txt` & `air_drf_relation-0.5.7/air_drf_relation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/device/migrations/0001_initial.py` & `air_drf_relation-0.5.7/device/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/device/serializers.py` & `air_drf_relation-0.5.7/device/serializers.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/device/tests.py` & `air_drf_relation-0.5.7/device/tests.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/film/migrations/0001_initial.py` & `air_drf_relation-0.5.7/film/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/film/models.py` & `air_drf_relation-0.5.7/film/models.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/film/serializers.py` & `air_drf_relation-0.5.7/film/serializers.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/film/tests.py` & `air_drf_relation-0.5.7/film/tests.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/setup.py` & `air_drf_relation-0.5.7/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,24 +4,26 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='air_drf_relation',
-      version='0.5.6',
+      version='0.5.7',
       description='Improved interaction with DRF relations.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       keywords='django rest relation nested pk primary object',
       url='https://github.com/bubaley/air-drf-relation',
       author='bubaley',
       author_email='bubaley.fu@gmail.com',
       license='MIT',
       packages=find_packages(),
       install_requires=[
           'djangorestframework',
           'django-filter',
-          'django'
+          'django',
+          'dacite',
+          'djangorestframework-dataclasses'
       ],
       include_package_data=True,
       zip_safe=False)
```

### Comparing `air_drf_relation-0.5.6/table/migrations/0001_initial.py` & `air_drf_relation-0.5.7/table/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/table/migrations/0003_auto_20220513_1542.py` & `air_drf_relation-0.5.7/table/migrations/0003_auto_20220513_1542.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/table/migrations/0004_material_company.py` & `air_drf_relation-0.5.7/table/migrations/0004_material_company.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/table/models.py` & `air_drf_relation-0.5.7/table/models.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/table/serializers.py` & `air_drf_relation-0.5.7/table/serializers.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/table/tests.py` & `air_drf_relation-0.5.7/table/tests.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/task/migrations/0001_initial.py` & `air_drf_relation-0.5.7/task/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/task/migrations/0003_tag.py` & `air_drf_relation-0.5.7/task/migrations/0003_tag.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/task/migrations/0004_tag_task.py` & `air_drf_relation-0.5.7/task/migrations/0004_tag_task.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/task/tests.py` & `air_drf_relation-0.5.7/task/tests.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.5.6/task/views.py` & `air_drf_relation-0.5.7/task/views.py`

 * *Files identical despite different names*

