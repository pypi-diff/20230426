# Comparing `tmp/djgentelella-0.3.8.tar.gz` & `tmp/djgentelella-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djgentelella-0.3.8.tar", last modified: Fri Jan  6 00:00:44 2023, max compression
+gzip compressed data, was "djgentelella-0.3.9.tar", last modified: Tue Jan 17 16:40:40 2023, max compression
```

## Comparing `djgentelella-0.3.8.tar` & `djgentelella-0.3.9.tar`

### file list

```diff
@@ -1,1048 +1,1052 @@
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.237464 djgentelella-0.3.8/
--rw-r--r--   0 luisza    (1000) luisza    (1000)    18047 2022-09-27 22:26:00.000000 djgentelella-0.3.8/LICENSE
--rw-r--r--   0 luisza    (1000) luisza    (1000)      206 2022-09-27 22:26:00.000000 djgentelella-0.3.8/MANIFEST.in
--rw-r--r--   0 luisza    (1000) luisza    (1000)     4911 2023-01-06 00:00:44.237464 djgentelella-0.3.8/PKG-INFO
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2883 2022-10-28 14:04:53.000000 djgentelella-0.3.8/Readme.rst
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.113464 djgentelella-0.3.8/djgentelella/
--rw-r--r--   0 luisza    (1000) luisza    (1000)       22 2023-01-05 16:27:54.000000 djgentelella-0.3.8/djgentelella/__init__.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1304 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/admin.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)      153 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/apps.py
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.113464 djgentelella-0.3.8/djgentelella/blog/
--rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/blog/__init__.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)       29 2022-12-21 20:53:40.000000 djgentelella-0.3.8/djgentelella/blog/admin.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)      150 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/blog/apps.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)      919 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/blog/forms.py
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.113464 djgentelella-0.3.8/djgentelella/blog/migrations/
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3175 2022-12-21 21:53:07.000000 djgentelella-0.3.8/djgentelella/blog/migrations/0001_initial.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/blog/migrations/__init__.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3796 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/blog/models.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)      483 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/blog/sitemaps.py
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.105464 djgentelella-0.3.8/djgentelella/blog/static/
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.113464 djgentelella-0.3.8/djgentelella/blog/static/images/
--rw-r--r--   0 luisza    (1000) luisza    (1000)    85355 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/blog/static/images/article.png
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.105464 djgentelella-0.3.8/djgentelella/blog/templates/
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.105464 djgentelella-0.3.8/djgentelella/blog/templates/gentelella/
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.113464 djgentelella-0.3.8/djgentelella/blog/templates/gentelella/blog/
--rw-r--r--   0 luisza    (1000) luisza    (1000)      123 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/blog/templates/gentelella/blog/category_add.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      688 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/blog/templates/gentelella/blog/entry_delete.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1976 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/blog/templates/gentelella/blog/entry_detail.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      806 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/blog/templates/gentelella/blog/entry_form.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)     5528 2022-11-08 16:55:36.000000 djgentelella-0.3.8/djgentelella/blog/templates/gentelella/blog/entry_list.html
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.113464 djgentelella-0.3.8/djgentelella/blog/templatetags/
--rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-12-21 21:56:51.000000 djgentelella-0.3.8/djgentelella/blog/templatetags/__init__.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)      621 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/blog/templatetags/blog_tags.py
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.117464 djgentelella-0.3.8/djgentelella/blog/tests/
--rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/blog/tests/__init__.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)      849 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/blog/tests/test_entry_detail.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1983 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/blog/tests/test_entry_forms.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1046 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/blog/tests/test_entry_listing.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     4147 2022-12-21 21:46:47.000000 djgentelella-0.3.8/djgentelella/blog/tests/test_models.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1299 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/blog/tests/test_sitemaps.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2105 2022-12-21 21:56:42.000000 djgentelella-0.3.8/djgentelella/blog/tests/test_templatetags.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)       26 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/blog/tests.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)      582 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/blog/urls.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     5761 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/blog/views.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     8572 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/chartjs.py
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.117464 djgentelella-0.3.8/djgentelella/chunked_upload/
--rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-10-08 03:13:40.000000 djgentelella-0.3.8/djgentelella/chunked_upload/__init__.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)      300 2022-10-08 03:13:40.000000 djgentelella-0.3.8/djgentelella/chunked_upload/constants.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2908 2022-12-21 21:32:15.000000 djgentelella-0.3.8/djgentelella/chunked_upload/models.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)      388 2022-10-08 03:13:40.000000 djgentelella-0.3.8/djgentelella/chunked_upload/response.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)    11110 2022-12-21 21:32:07.000000 djgentelella-0.3.8/djgentelella/chunked_upload/views.py
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.117464 djgentelella-0.3.8/djgentelella/cruds/
--rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/cruds/__init__.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)    28229 2022-12-21 21:44:14.000000 djgentelella-0.3.8/djgentelella/cruds/base.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2685 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/cruds/filter.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     9405 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/cruds/inline_crud.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3115 2022-12-21 21:31:25.000000 djgentelella-0.3.8/djgentelella/cruds/utils.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3340 2022-12-21 20:53:40.000000 djgentelella-0.3.8/djgentelella/elements.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)      262 2022-10-08 03:13:40.000000 djgentelella-0.3.8/djgentelella/exceptions.py
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.117464 djgentelella-0.3.8/djgentelella/fields/
--rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/fields/__init__.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2551 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/fields/catalog.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1880 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/fields/drfdatetime.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2209 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/fields/tree.py
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.117464 djgentelella-0.3.8/djgentelella/forms/
--rw-r--r--   0 luisza    (1000) luisza    (1000)       84 2022-12-21 20:53:40.000000 djgentelella-0.3.8/djgentelella/forms/__init__.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2340 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/forms/decorators.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3092 2022-12-21 21:06:39.000000 djgentelella-0.3.8/djgentelella/forms/forms.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)      397 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/forms/models.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)      415 2022-12-21 20:53:40.000000 djgentelella-0.3.8/djgentelella/groute.py
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.105464 djgentelella-0.3.8/djgentelella/locale/
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.105464 djgentelella-0.3.8/djgentelella/locale/es/
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.117464 djgentelella-0.3.8/djgentelella/locale/es/LC_MESSAGES/
--rw-r--r--   0 luisza    (1000) luisza    (1000)     8099 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 luisza    (1000) luisza    (1000)    15549 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.117464 djgentelella-0.3.8/djgentelella/management/
--rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/management/__init__.py
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.117464 djgentelella-0.3.8/djgentelella/management/commands/
--rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/management/commands/__init__.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1508 2022-12-21 20:53:40.000000 djgentelella-0.3.8/djgentelella/management/commands/createbasejs.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1716 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/management/commands/delete_expired_uploads.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)    26879 2022-12-21 21:14:46.000000 djgentelella-0.3.8/djgentelella/management/commands/loaddevstatic.py
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.117464 djgentelella-0.3.8/djgentelella/menu_widgets/
--rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/menu_widgets/__init__.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2253 2022-12-21 21:07:10.000000 djgentelella-0.3.8/djgentelella/menu_widgets/palette.py
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.121464 djgentelella-0.3.8/djgentelella/migrations/
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2868 2022-12-21 21:52:13.000000 djgentelella-0.3.8/djgentelella/migrations/0001_initial.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     8975 2022-12-21 21:56:12.000000 djgentelella-0.3.8/djgentelella/migrations/0001_squashed_new_initial.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)      424 2023-01-05 22:09:21.000000 djgentelella-0.3.8/djgentelella/migrations/0002_alter_permissionscategorymanagement_options.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)      993 2022-12-21 21:59:13.000000 djgentelella-0.3.8/djgentelella/migrations/0002_auto_20200214_2038.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)      988 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/migrations/0003_help.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)      582 2022-12-21 20:53:40.000000 djgentelella-0.3.8/djgentelella/migrations/0004_loadsettings.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1921 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/migrations/0005_notification.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1073 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/migrations/0006_permissionscategorymanagement.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)      660 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/migrations/0007_edit_footer.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)      479 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/migrations/0008_defaulttheme.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1855 2022-12-21 21:52:28.000000 djgentelella-0.3.8/djgentelella/migrations/0009_chunkedupload.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)      707 2022-12-21 20:53:40.000000 djgentelella-0.3.8/djgentelella/migrations/0010_menuitem_position.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1077 2022-12-21 20:53:40.000000 djgentelella-0.3.8/djgentelella/migrations/0011_remove_menuitem_level_remove_menuitem_lft_and_more.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/migrations/__init__.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     4560 2023-01-05 22:06:57.000000 djgentelella-0.3.8/djgentelella/models.py
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.121464 djgentelella-0.3.8/djgentelella/notification/
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3585 2023-01-05 21:42:42.000000 djgentelella-0.3.8/djgentelella/notification/__init__.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1672 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/notification/base.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)      557 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/notification/serializer.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1752 2022-12-21 20:53:40.000000 djgentelella-0.3.8/djgentelella/notification/widgets.py
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.121464 djgentelella-0.3.8/djgentelella/permission_management/
--rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/permission_management/__init__.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1562 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/permission_management/forms.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     4926 2022-12-21 21:59:57.000000 djgentelella-0.3.8/djgentelella/permission_management/objinterface.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2117 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/permission_management/views.py
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.121464 djgentelella-0.3.8/djgentelella/serializers/
--rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/serializers/__init__.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3461 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/serializers/calendar.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)      248 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/serializers/helper.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1255 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/serializers/storyline.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2777 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/serializers/storymap.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2132 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/serializers/timeline.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2917 2022-12-21 21:38:13.000000 djgentelella-0.3.8/djgentelella/settings.py
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.105464 djgentelella-0.3.8/djgentelella/static/
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.105464 djgentelella-0.3.8/djgentelella/static/django_ajax/
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.121464 djgentelella-0.3.8/djgentelella/static/django_ajax/js/
--rw-r--r--   0 luisza    (1000) luisza    (1000)     8403 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/static/django_ajax/js/jquery.ajax-plugin.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3030 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/static/django_ajax/js/jquery.ajax-plugin.min.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)     6684 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/static/django_ajax/js/jquery.ajax.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3460 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/static/django_ajax/js/jquery.ajax.min.js
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.105464 djgentelella-0.3.8/djgentelella/static/gentelella/
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.125464 djgentelella-0.3.8/djgentelella/static/gentelella/css/
--rwxr-xr-x   0 luisza    (1000) luisza    (1000)    89690 2022-11-03 22:29:50.000000 djgentelella-0.3.8/djgentelella/static/gentelella/css/custom.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)    81514 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/static/gentelella/css/modern.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)    81715 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/static/gentelella/css/modern_black_white.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)    81264 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/static/gentelella/css/style_black_and_white.css
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.125464 djgentelella-0.3.8/djgentelella/static/gentelella/images/
--rwxr-xr-x   0 luisza    (1000) luisza    (1000)     1361 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/static/gentelella/images/back_disabled.png
--rwxr-xr-x   0 luisza    (1000) luisza    (1000)     1379 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/static/gentelella/images/back_enabled.png
--rwxr-xr-x   0 luisza    (1000) luisza    (1000)     1375 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/static/gentelella/images/back_enabled_hover.png
--rwxr-xr-x   0 luisza    (1000) luisza    (1000)     1363 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/static/gentelella/images/forward_disabled.png
--rwxr-xr-x   0 luisza    (1000) luisza    (1000)     1380 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/static/gentelella/images/forward_enabled.png
--rwxr-xr-x   0 luisza    (1000) luisza    (1000)     1379 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/static/gentelella/images/forward_enabled_hover.png
--rwxr-xr-x   0 luisza    (1000) luisza    (1000)    30269 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/static/gentelella/images/loading.gif
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.129464 djgentelella-0.3.8/djgentelella/static/gentelella/js/
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.129464 djgentelella-0.3.8/djgentelella/static/gentelella/js/base/
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1216 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/static/gentelella/js/base/autocompleteSelect2.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1056 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/static/gentelella/js/base/booleanFields.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)      772 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/static/gentelella/js/base/calendar.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1567 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/static/gentelella/js/base/chart.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)     5533 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/static/gentelella/js/base/custom.widgets.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)     5617 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/static/gentelella/js/base/dateranges_gridslider.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1118 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/static/gentelella/js/base/editorTinymce.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)     4319 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/static/gentelella/js/base/fileupload.widget.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)     7693 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/static/gentelella/js/base/formset.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)      627 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/static/gentelella/js/base/gigapixel_storymap.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)    10836 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/static/gentelella/js/base/helper_widget.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)      542 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/static/gentelella/js/base/mapbased_storymap.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)     4688 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/static/gentelella/js/base/notifications.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)      332 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/static/gentelella/js/base/select2_wrap.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)     4540 2022-11-01 23:08:45.000000 djgentelella-0.3.8/djgentelella/static/gentelella/js/base/select2related.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)      867 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/static/gentelella/js/base/storyline.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)      788 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/static/gentelella/js/base/timeline.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)      405 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/static/gentelella/js/base/wysiwyg.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)    52577 2023-01-06 00:00:43.000000 djgentelella-0.3.8/djgentelella/static/gentelella/js/base.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)    14885 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/static/gentelella/js/custom.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)     9310 2022-12-17 20:23:41.000000 djgentelella-0.3.8/djgentelella/static/gentelella/js/datatables.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)  3898127 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/static/gentelella/js/gentelella-bundle.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)     8211 2022-11-06 19:51:25.000000 djgentelella-0.3.8/djgentelella/static/gentelella/js/permissionmanagement.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)    12575 2022-10-28 14:04:53.000000 djgentelella-0.3.8/djgentelella/static/gentelella/js/widgets.js
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.109464 djgentelella-0.3.8/djgentelella/static/vendors/
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.129464 djgentelella-0.3.8/djgentelella/static/vendors/autosize/
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3274 2023-01-05 23:59:18.000000 djgentelella-0.3.8/djgentelella/static/vendors/autosize/autosize.min.js
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.133464 djgentelella-0.3.8/djgentelella/static/vendors/bootstrap/
--rw-r--r--   0 luisza    (1000) luisza    (1000)    79790 2023-01-05 23:59:11.000000 djgentelella-0.3.8/djgentelella/static/vendors/bootstrap/bootstrap.bundle.min.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)   194699 2023-01-05 23:59:10.000000 djgentelella-0.3.8/djgentelella/static/vendors/bootstrap/bootstrap.min.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)    60104 2023-01-05 23:59:10.000000 djgentelella-0.3.8/djgentelella/static/vendors/bootstrap/bootstrap.min.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)    19766 2023-01-05 23:59:11.000000 djgentelella-0.3.8/djgentelella/static/vendors/bootstrap/popper.min.js
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.133464 djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-colorpicker/
--rw-r--r--   0 luisza    (1000) luisza    (1000)     4002 2023-01-06 00:00:30.000000 djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-colorpicker/bootstrap-colorpicker.min.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)    18689 2023-01-06 00:00:30.000000 djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-colorpicker/bootstrap-colorpicker.min.js
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.133464 djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-daterangepicker/
--rw-r--r--   0 luisza    (1000) luisza    (1000)     6430 2023-01-05 23:59:13.000000 djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-daterangepicker/daterangepicker.min.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2876 2023-01-05 23:59:13.000000 djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-daterangepicker/daterangepicker.min.css.map
--rw-r--r--   0 luisza    (1000) luisza    (1000)    32018 2023-01-05 23:59:12.000000 djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-daterangepicker/daterangepicker.min.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)    32527 2023-01-05 23:59:13.000000 djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-daterangepicker/daterangepicker.min.js.map
--rw-r--r--   0 luisza    (1000) luisza    (1000)    53324 2023-01-05 23:59:13.000000 djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-daterangepicker/moment.min.js
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.133464 djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-datetimepicker/
--rw-r--r--   0 luisza    (1000) luisza    (1000)     7785 2023-01-05 23:59:13.000000 djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-datetimepicker/bootstrap-datetimepicker.min.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)      146 2023-01-05 23:59:13.000000 djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-datetimepicker/bootstrap-datetimepicker.min.css.map
--rw-r--r--   0 luisza    (1000) luisza    (1000)    38510 2023-01-05 23:59:13.000000 djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-datetimepicker/bootstrap-datetimepicker.min.js
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.133464 djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-maxlength/
--rw-r--r--   0 luisza    (1000) luisza    (1000)     4821 2023-01-05 23:59:18.000000 djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-maxlength/bootstrap-maxlength.min.js
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.133464 djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-progressbar/
--rw-r--r--   0 luisza    (1000) luisza    (1000)     5014 2023-01-05 23:59:16.000000 djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-progressbar/bootstrap-progressbar-3.3.4.min.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2333 2023-01-05 23:59:16.000000 djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-progressbar/bootstrap-progressbar.min.js
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.133464 djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-tree/
--rw-r--r--   0 luisza    (1000) luisza    (1000)      521 2023-01-06 00:00:32.000000 djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-tree/bootstrap-treeview.min.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)    27547 2023-01-06 00:00:32.000000 djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-tree/bootstrap-treeview.min.js
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.133464 djgentelella-0.3.8/djgentelella/static/vendors/chartjs/
--rw-r--r--   0 luisza    (1000) luisza    (1000)      521 2023-01-06 00:00:30.000000 djgentelella-0.3.8/djgentelella/static/vendors/chartjs/Chart.min.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)   172812 2023-01-06 00:00:30.000000 djgentelella-0.3.8/djgentelella/static/vendors/chartjs/Chart.min.js
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.105464 djgentelella-0.3.8/djgentelella/static/vendors/css/
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.133464 djgentelella-0.3.8/djgentelella/static/vendors/css/icons/
--rw-r--r--   0 luisza    (1000) luisza    (1000)    14472 2023-01-06 00:00:30.000000 djgentelella-0.3.8/djgentelella/static/vendors/css/icons/vco-icons.ttf
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.133464 djgentelella-0.3.8/djgentelella/static/vendors/datatables/
--rw-r--r--   0 luisza    (1000) luisza    (1000)    62157 2023-01-06 00:00:27.000000 djgentelella-0.3.8/djgentelella/static/vendors/datatables/datatables.min.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)   590996 2023-01-06 00:00:27.000000 djgentelella-0.3.8/djgentelella/static/vendors/datatables/datatables.min.js
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.133464 djgentelella-0.3.8/djgentelella/static/vendors/fileupload/
--rw-r--r--   0 luisza    (1000) luisza    (1000)    18782 2023-01-06 00:00:27.000000 djgentelella-0.3.8/djgentelella/static/vendors/fileupload/jquery.fileupload.min.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2292 2023-01-06 00:00:28.000000 djgentelella-0.3.8/djgentelella/static/vendors/fileupload/jquery.iframe-transport.min.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)     8398 2023-01-06 00:00:28.000000 djgentelella-0.3.8/djgentelella/static/vendors/fileupload/jquery.ui.widget.min.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)    10158 2023-01-06 00:00:28.000000 djgentelella-0.3.8/djgentelella/static/vendors/fileupload/spark-md5.min.js
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.133464 djgentelella-0.3.8/djgentelella/static/vendors/flag-icon-css/
--rw-r--r--   0 luisza    (1000) luisza    (1000)    27398 2023-01-05 23:59:18.000000 djgentelella-0.3.8/djgentelella/static/vendors/flag-icon-css/flag-icons.min.css
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.105464 djgentelella-0.3.8/djgentelella/static/vendors/flags/
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.169464 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/
--rw-r--r--   0 luisza    (1000) luisza    (1000)    32253 2023-01-05 23:59:18.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ad.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      262 2023-01-05 23:59:18.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ae.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    20928 2023-01-05 23:59:18.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/af.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      761 2023-01-05 23:59:18.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ag.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    48199 2023-01-05 23:59:18.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ai.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3205 2023-01-05 23:59:18.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/al.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      231 2023-01-05 23:59:18.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/am.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1588 2023-01-05 23:59:19.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ao.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     5958 2023-01-05 23:59:19.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/aq.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3473 2023-01-05 23:59:19.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ar.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     7828 2023-01-05 23:59:19.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/as.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      242 2023-01-05 23:59:19.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/at.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1483 2023-01-05 23:59:19.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/au.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    12084 2023-01-05 23:59:19.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/aw.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      541 2023-01-05 23:59:19.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ax.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      498 2023-01-05 23:59:19.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/az.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1242 2023-01-05 23:59:20.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ba.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      609 2023-01-05 23:59:20.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/bb.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      192 2023-01-05 23:59:20.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/bd.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      290 2023-01-05 23:59:20.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/be.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      383 2023-01-05 23:59:20.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/bf.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      294 2023-01-05 23:59:20.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/bg.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      538 2023-01-05 23:59:20.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/bh.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1042 2023-01-05 23:59:20.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/bi.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      499 2023-01-05 23:59:20.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/bj.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-05 23:59:20.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/bl.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    22270 2023-01-05 23:59:21.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/bm.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    14359 2023-01-05 23:59:21.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/bn.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)   118659 2023-01-05 23:59:21.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/bo.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      228 2023-01-05 23:59:21.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/bq.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     7686 2023-01-05 23:59:21.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/br.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      568 2023-01-05 23:59:21.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/bs.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    25045 2023-01-05 23:59:21.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/bt.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      582 2023-01-05 23:59:21.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/bv.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      254 2023-01-05 23:59:21.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/bw.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     6086 2023-01-05 23:59:22.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/by.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    46678 2023-01-05 23:59:22.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/bz.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      708 2023-01-05 23:59:22.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ca.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3083 2023-01-05 23:59:22.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/cc.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      507 2023-01-05 23:59:22.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/cd.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      632 2023-01-05 23:59:22.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/cf.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      469 2023-01-05 23:59:22.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/cg.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      295 2023-01-05 23:59:22.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ch.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      283 2023-01-05 23:59:23.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ci.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2020 2023-01-05 23:59:23.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ck.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      574 2023-01-05 23:59:23.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/cl.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      824 2023-01-05 23:59:23.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/cm.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      743 2023-01-05 23:59:23.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/cn.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      289 2023-01-05 23:59:23.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/co.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      293 2023-01-05 23:59:24.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/cr.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      573 2023-01-05 23:59:24.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/cu.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1357 2023-01-05 23:59:24.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/cv.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      682 2023-01-05 23:59:24.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/cw.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2496 2023-01-05 23:59:24.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/cx.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     5955 2023-01-05 23:59:24.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/cy.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      480 2023-01-05 23:59:25.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/cz.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      221 2023-01-05 23:59:25.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/de.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      585 2023-01-05 23:59:25.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/dj.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      235 2023-01-05 23:59:25.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/dk.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    16457 2023-01-05 23:59:25.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/dm.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)   391369 2023-01-05 23:59:25.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/do.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      305 2023-01-05 23:59:25.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/dz.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    29875 2023-01-05 23:59:26.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ec.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      352 2023-01-05 23:59:26.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ee.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     9913 2023-01-05 23:59:26.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/eg.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      817 2023-01-05 23:59:26.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/eh.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3371 2023-01-05 23:59:26.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/er.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      257 2023-01-05 23:59:26.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/es-ca.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    92546 2023-01-05 23:59:26.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/es.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1226 2023-01-05 23:59:26.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/et.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1250 2023-01-05 23:59:27.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/eu.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      240 2023-01-05 23:59:27.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/fi.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    27518 2023-01-05 23:59:27.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/fj.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    31798 2023-01-05 23:59:27.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/fk.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      759 2023-01-05 23:59:27.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/fm.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      534 2023-01-05 23:59:27.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/fo.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-05 23:59:27.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/fr.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      278 2023-01-05 23:59:27.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ga.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      232 2023-01-05 23:59:27.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/gb-eng.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    26487 2023-01-05 23:59:28.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/gb-nir.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      239 2023-01-05 23:59:28.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/gb-sct.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     9055 2023-01-05 23:59:28.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/gb-wls.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      541 2023-01-05 23:59:28.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/gb.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1828 2023-01-05 23:59:28.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/gd.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1541 2023-01-05 23:59:28.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ge.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-05 23:59:28.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/gf.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      625 2023-01-05 23:59:28.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/gg.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      296 2023-01-05 23:59:28.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/gh.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2930 2023-01-05 23:59:29.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/gi.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      237 2023-01-05 23:59:29.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/gl.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      382 2023-01-05 23:59:29.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/gm.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      295 2023-01-05 23:59:29.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/gn.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-05 23:59:29.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/gp.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     5273 2023-01-05 23:59:29.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/gq.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1085 2023-01-05 23:59:29.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/gr.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    35061 2023-01-05 23:59:29.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/gs.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    37255 2023-01-05 23:59:29.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/gt.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     4614 2023-01-05 23:59:30.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/gu.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      889 2023-01-05 23:59:30.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/gw.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      481 2023-01-05 23:59:30.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/gy.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3529 2023-01-05 23:59:30.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/hk.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1308 2023-01-05 23:59:30.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/hm.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1116 2023-01-05 23:59:30.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/hn.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    40852 2023-01-05 23:59:30.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/hr.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    15094 2023-01-05 23:59:31.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ht.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      276 2023-01-05 23:59:31.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/hu.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      239 2023-01-05 23:59:31.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/id.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-05 23:59:31.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ie.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      848 2023-01-05 23:59:31.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/il.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    10197 2023-01-05 23:59:31.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/im.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1088 2023-01-05 23:59:31.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/in.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    27357 2023-01-05 23:59:31.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/io.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1475 2023-01-05 23:59:31.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/iq.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    15356 2023-01-05 23:59:32.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ir.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      526 2023-01-05 23:59:32.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/is.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-05 23:59:32.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/it.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     4675 2023-01-05 23:59:32.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/je.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      389 2023-01-05 23:59:32.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/jm.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      691 2023-01-05 23:59:32.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/jo.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      484 2023-01-05 23:59:32.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/jp.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1485 2023-01-05 23:59:32.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ke.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3316 2023-01-05 23:59:33.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/kg.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     7262 2023-01-05 23:59:33.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/kh.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     5941 2023-01-05 23:59:33.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ki.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1037 2023-01-05 23:59:33.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/km.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      817 2023-01-05 23:59:33.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/kn.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      852 2023-01-05 23:59:33.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/kp.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1719 2023-01-05 23:59:33.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/kr.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      507 2023-01-05 23:59:33.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/kw.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    22357 2023-01-05 23:59:34.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ky.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    11415 2023-01-05 23:59:34.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/kz.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      501 2023-01-05 23:59:34.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/la.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2747 2023-01-05 23:59:34.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/lb.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      370 2023-01-05 23:59:34.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/lc.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     8291 2023-01-05 23:59:34.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/li.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    11254 2023-01-05 23:59:34.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/lk.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      694 2023-01-05 23:59:34.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/lr.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1242 2023-01-05 23:59:34.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ls.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      442 2023-01-05 23:59:35.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/lt.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      232 2023-01-05 23:59:35.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/lu.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      237 2023-01-05 23:59:35.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/lv.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      526 2023-01-05 23:59:35.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ly.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      250 2023-01-05 23:59:35.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ma.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      237 2023-01-05 23:59:35.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/mc.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    11337 2023-01-05 23:59:35.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/md.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    63354 2023-01-05 23:59:36.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/me.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-05 23:59:36.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/mf.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      302 2023-01-05 23:59:36.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/mg.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      763 2023-01-05 23:59:36.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/mh.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      410 2023-01-05 23:59:36.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/mk.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      279 2023-01-05 23:59:36.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ml.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      865 2023-01-05 23:59:36.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/mm.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1251 2023-01-05 23:59:36.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/mn.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1495 2023-01-05 23:59:37.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/mo.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    23628 2023-01-05 23:59:37.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/mp.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-05 23:59:37.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/mq.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      431 2023-01-05 23:59:37.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/mr.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    12140 2023-01-05 23:59:37.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ms.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    10422 2023-01-05 23:59:37.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/mt.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      319 2023-01-05 23:59:37.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/mu.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      307 2023-01-05 23:59:37.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/mv.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3797 2023-01-05 23:59:38.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/mw.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    90505 2023-01-05 23:59:38.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/mx.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1262 2023-01-05 23:59:38.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/my.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2597 2023-01-05 23:59:38.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/mz.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      977 2023-01-05 23:59:38.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/na.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1387 2023-01-05 23:59:38.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/nc.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      282 2023-01-05 23:59:38.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ne.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     5591 2023-01-05 23:59:38.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/nf.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      260 2023-01-05 23:59:39.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ng.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    18463 2023-01-05 23:59:39.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ni.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      228 2023-01-05 23:59:39.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/nl.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      321 2023-01-05 23:59:39.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/no.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1193 2023-01-05 23:59:39.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/np.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      668 2023-01-05 23:59:39.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/nr.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1727 2023-01-05 23:59:39.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/nu.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2999 2023-01-05 23:59:39.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/nz.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    22614 2023-01-05 23:59:40.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/om.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      659 2023-01-05 23:59:40.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/pa.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    72907 2023-01-05 23:59:40.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/pe.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     4229 2023-01-05 23:59:40.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/pf.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2095 2023-01-05 23:59:40.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/pg.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1510 2023-01-05 23:59:40.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ph.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      684 2023-01-05 23:59:40.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/pk.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      222 2023-01-05 23:59:40.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/pl.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-05 23:59:41.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/pm.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     8517 2023-01-05 23:59:41.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/pn.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      619 2023-01-05 23:59:41.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/pr.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      541 2023-01-05 23:59:41.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ps.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     8661 2023-01-05 23:59:41.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/pt.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      507 2023-01-05 23:59:41.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/pw.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    17246 2023-01-05 23:59:41.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/py.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      356 2023-01-05 23:59:42.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/qa.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-05 23:59:42.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/re.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      305 2023-01-05 23:59:42.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ro.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)   186989 2023-01-05 23:59:42.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/rs.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      290 2023-01-05 23:59:43.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ru.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      748 2023-01-05 23:59:43.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/rw.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    10179 2023-01-05 23:59:43.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/sa.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      952 2023-01-05 23:59:43.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/sb.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      570 2023-01-05 23:59:44.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/sc.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      493 2023-01-05 23:59:44.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/sd.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      698 2023-01-05 23:59:44.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/se.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      948 2023-01-05 23:59:45.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/sg.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    30113 2023-01-05 23:59:45.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/sh.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2065 2023-01-05 23:59:45.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/si.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      321 2023-01-05 23:59:45.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/sj.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1173 2023-01-05 23:59:45.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/sk.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      438 2023-01-05 23:59:45.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/sl.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    15729 2023-01-05 23:59:45.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/sm.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      414 2023-01-05 23:59:45.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/sn.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      498 2023-01-05 23:59:46.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/so.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      320 2023-01-05 23:59:46.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/sr.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      397 2023-01-05 23:59:46.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ss.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      920 2023-01-05 23:59:46.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/st.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    83238 2023-01-05 23:59:46.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/sv.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    12992 2023-01-05 23:59:46.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/sx.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      579 2023-01-05 23:59:46.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/sy.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     6689 2023-01-05 23:59:46.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/sz.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    14756 2023-01-05 23:59:46.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/tc.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      279 2023-01-05 23:59:47.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/td.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1196 2023-01-05 23:59:47.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/tf.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      733 2023-01-05 23:59:47.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/tg.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      288 2023-01-05 23:59:47.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/th.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1767 2023-01-05 23:59:47.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/tj.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      778 2023-01-05 23:59:47.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/tk.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      577 2023-01-05 23:59:47.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/tl.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    31566 2023-01-05 23:59:47.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/tm.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      733 2023-01-05 23:59:48.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/tn.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      361 2023-01-05 23:59:48.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/to.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      575 2023-01-05 23:59:48.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/tr.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      320 2023-01-05 23:59:48.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/tt.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1716 2023-01-05 23:59:48.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/tv.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      954 2023-01-05 23:59:48.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/tw.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      602 2023-01-05 23:59:48.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/tz.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      238 2023-01-05 23:59:49.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ua.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     4024 2023-01-05 23:59:49.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ug.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3972 2023-01-05 23:59:49.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/um.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    20185 2023-01-05 23:59:49.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/un.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3921 2023-01-05 23:59:49.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/us.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1715 2023-01-05 23:59:49.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/uy.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1454 2023-01-05 23:59:49.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/uz.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    90711 2023-01-05 23:59:49.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/va.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      498 2023-01-05 23:59:49.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/vc.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1188 2023-01-05 23:59:50.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ve.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    24814 2023-01-05 23:59:50.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/vg.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     8697 2023-01-05 23:59:50.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/vi.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      498 2023-01-05 23:59:50.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/vn.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3732 2023-01-05 23:59:50.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/vu.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-05 23:59:50.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/wf.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      706 2023-01-05 23:59:50.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ws.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     8963 2023-01-05 23:59:51.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/xk.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      275 2023-01-05 23:59:51.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ye.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-05 23:59:51.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/yt.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      872 2023-01-05 23:59:51.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/za.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     5401 2023-01-05 23:59:51.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/zm.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     6614 2023-01-05 23:59:51.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/zw.svg
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.201464 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/
--rw-r--r--   0 luisza    (1000) luisza    (1000)    33473 2023-01-05 23:59:51.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ad.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      254 2023-01-05 23:59:51.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ae.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    21066 2023-01-05 23:59:52.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/af.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      749 2023-01-05 23:59:52.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ag.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    48259 2023-01-05 23:59:52.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ai.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3206 2023-01-05 23:59:52.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/al.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      223 2023-01-05 23:59:52.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/am.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1588 2023-01-05 23:59:52.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ao.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     6143 2023-01-05 23:59:52.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/aq.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3402 2023-01-05 23:59:52.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ar.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     8068 2023-01-05 23:59:53.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/as.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      240 2023-01-05 23:59:53.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/at.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1546 2023-01-05 23:59:53.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/au.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     9951 2023-01-05 23:59:53.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/aw.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      559 2023-01-05 23:59:54.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ax.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      512 2023-01-05 23:59:54.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/az.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1310 2023-01-05 23:59:54.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ba.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      609 2023-01-05 23:59:54.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/bb.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      190 2023-01-05 23:59:54.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/bd.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      290 2023-01-05 23:59:54.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/be.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      357 2023-01-05 23:59:54.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/bf.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      286 2023-01-05 23:59:54.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/bg.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      517 2023-01-05 23:59:55.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/bh.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1074 2023-01-05 23:59:55.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/bi.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      502 2023-01-05 23:59:55.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/bj.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-05 23:59:55.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/bl.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    22569 2023-01-05 23:59:55.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/bm.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    14213 2023-01-05 23:59:55.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/bn.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)   117062 2023-01-05 23:59:55.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/bo.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      224 2023-01-05 23:59:55.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/bq.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     8097 2023-01-05 23:59:56.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/br.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      552 2023-01-05 23:59:56.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/bs.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    25227 2023-01-05 23:59:56.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/bt.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      585 2023-01-05 23:59:56.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/bv.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      252 2023-01-05 23:59:56.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/bw.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     5962 2023-01-05 23:59:56.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/by.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    46427 2023-01-05 23:59:56.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/bz.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      728 2023-01-05 23:59:56.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ca.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3123 2023-01-05 23:59:57.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/cc.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      349 2023-01-05 23:59:57.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/cd.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      691 2023-01-05 23:59:57.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/cf.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      487 2023-01-05 23:59:57.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/cg.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      297 2023-01-05 23:59:57.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ch.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      280 2023-01-05 23:59:57.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ci.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2097 2023-01-05 23:59:57.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ck.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      563 2023-01-05 23:59:57.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/cl.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      824 2023-01-05 23:59:58.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/cm.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      801 2023-01-05 23:59:58.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/cn.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      289 2023-01-05 23:59:58.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/co.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      293 2023-01-05 23:59:58.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/cr.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      622 2023-01-05 23:59:58.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/cu.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1415 2023-01-05 23:59:58.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/cv.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      681 2023-01-05 23:59:58.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/cw.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2455 2023-01-05 23:59:58.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/cx.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     5866 2023-01-05 23:59:58.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/cy.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      484 2023-01-05 23:59:59.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/cz.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      213 2023-01-05 23:59:59.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/de.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      591 2023-01-05 23:59:59.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/dj.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      239 2023-01-05 23:59:59.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/dk.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    15975 2023-01-05 23:59:59.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/dm.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)   393849 2023-01-05 23:59:59.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/do.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      294 2023-01-05 23:59:59.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/dz.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    29320 2023-01-05 23:59:59.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ec.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      321 2023-01-06 00:00:00.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ee.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     9899 2023-01-06 00:00:00.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/eg.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      873 2023-01-06 00:00:00.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/eh.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3187 2023-01-06 00:00:00.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/er.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      258 2023-01-06 00:00:00.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/es-ca.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    90819 2023-01-06 00:00:00.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/es.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1233 2023-01-06 00:00:00.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/et.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1249 2023-01-06 00:00:01.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/eu.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      237 2023-01-06 00:00:01.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/fi.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    27237 2023-01-06 00:00:01.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/fj.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    31973 2023-01-06 00:00:01.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/fk.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      776 2023-01-06 00:00:01.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/fm.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      570 2023-01-06 00:00:01.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/fo.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-06 00:00:01.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/fr.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      274 2023-01-06 00:00:01.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ga.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      242 2023-01-06 00:00:02.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/gb-eng.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    25061 2023-01-06 00:00:02.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/gb-nir.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      231 2023-01-06 00:00:02.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/gb-sct.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     9161 2023-01-06 00:00:02.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/gb-wls.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      538 2023-01-06 00:00:02.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/gb.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1681 2023-01-06 00:00:02.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/gd.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1397 2023-01-06 00:00:02.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ge.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-06 00:00:02.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/gf.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      595 2023-01-06 00:00:02.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/gg.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      281 2023-01-06 00:00:03.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/gh.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2938 2023-01-06 00:00:03.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/gi.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      223 2023-01-06 00:00:03.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/gl.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      546 2023-01-06 00:00:03.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/gm.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      295 2023-01-06 00:00:03.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/gn.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-06 00:00:03.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/gp.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     5182 2023-01-06 00:00:03.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/gq.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1096 2023-01-06 00:00:03.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/gr.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    34568 2023-01-06 00:00:04.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/gs.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    37255 2023-01-06 00:00:04.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/gt.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     4840 2023-01-06 00:00:04.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/gu.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      813 2023-01-06 00:00:04.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/gw.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      488 2023-01-06 00:00:04.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/gy.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3494 2023-01-06 00:00:04.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/hk.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1324 2023-01-06 00:00:04.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/hm.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1112 2023-01-06 00:00:04.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/hn.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    40615 2023-01-06 00:00:05.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/hr.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    15005 2023-01-06 00:00:05.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ht.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      274 2023-01-06 00:00:05.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/hu.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      237 2023-01-06 00:00:05.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/id.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-06 00:00:05.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ie.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      901 2023-01-06 00:00:05.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/il.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     9870 2023-01-06 00:00:05.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/im.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1074 2023-01-06 00:00:05.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/in.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    27341 2023-01-06 00:00:06.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/io.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1470 2023-01-06 00:00:06.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/iq.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    15451 2023-01-06 00:00:06.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ir.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      524 2023-01-06 00:00:06.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/is.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-06 00:00:06.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/it.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     4700 2023-01-06 00:00:06.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/je.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      389 2023-01-06 00:00:07.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/jm.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      720 2023-01-06 00:00:07.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/jo.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      474 2023-01-06 00:00:07.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/jp.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1379 2023-01-06 00:00:07.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ke.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3374 2023-01-06 00:00:07.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/kg.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     7261 2023-01-06 00:00:07.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/kh.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     5813 2023-01-06 00:00:07.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ki.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1064 2023-01-06 00:00:08.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/km.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      819 2023-01-06 00:00:08.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/kn.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      795 2023-01-06 00:00:08.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/kp.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1822 2023-01-06 00:00:08.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/kr.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      509 2023-01-06 00:00:08.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/kw.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    21724 2023-01-06 00:00:08.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ky.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    11327 2023-01-06 00:00:08.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/kz.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      457 2023-01-06 00:00:08.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/la.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2816 2023-01-06 00:00:09.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/lb.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      370 2023-01-06 00:00:09.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/lc.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     8268 2023-01-06 00:00:09.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/li.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    11242 2023-01-06 00:00:09.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/lk.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      727 2023-01-06 00:00:09.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/lr.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1219 2023-01-06 00:00:09.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ls.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      442 2023-01-06 00:00:09.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/lt.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      228 2023-01-06 00:00:09.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/lu.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      233 2023-01-06 00:00:10.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/lv.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      533 2023-01-06 00:00:10.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ly.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      250 2023-01-06 00:00:10.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ma.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      237 2023-01-06 00:00:10.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/mc.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    11237 2023-01-06 00:00:10.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/md.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    62373 2023-01-06 00:00:10.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/me.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-06 00:00:10.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/mf.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      302 2023-01-06 00:00:10.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/mg.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      741 2023-01-06 00:00:11.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/mh.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      382 2023-01-06 00:00:11.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/mk.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      276 2023-01-06 00:00:11.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ml.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      848 2023-01-06 00:00:11.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/mm.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1245 2023-01-06 00:00:11.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/mn.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1461 2023-01-06 00:00:11.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/mo.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    23398 2023-01-06 00:00:11.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/mp.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-06 00:00:12.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/mq.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      442 2023-01-06 00:00:12.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/mr.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     9279 2023-01-06 00:00:12.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ms.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     8733 2023-01-06 00:00:12.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/mt.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      319 2023-01-06 00:00:12.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/mu.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      289 2023-01-06 00:00:12.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/mv.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3652 2023-01-06 00:00:12.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/mw.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    94979 2023-01-06 00:00:12.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/mx.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1270 2023-01-06 00:00:13.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/my.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2622 2023-01-06 00:00:13.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/mz.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1005 2023-01-06 00:00:13.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/na.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1380 2023-01-06 00:00:13.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/nc.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      276 2023-01-06 00:00:13.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ne.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     5837 2023-01-06 00:00:13.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/nf.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      260 2023-01-06 00:00:13.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ng.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    18408 2023-01-06 00:00:13.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ni.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      224 2023-01-06 00:00:14.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/nl.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      321 2023-01-06 00:00:14.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/no.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1061 2023-01-06 00:00:14.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/np.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      651 2023-01-06 00:00:14.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/nr.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1745 2023-01-06 00:00:14.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/nu.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2989 2023-01-06 00:00:14.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/nz.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    22636 2023-01-06 00:00:14.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/om.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      749 2023-01-06 00:00:14.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/pa.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    73609 2023-01-06 00:00:15.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/pe.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     4290 2023-01-06 00:00:15.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/pf.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1661 2023-01-06 00:00:15.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/pg.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1565 2023-01-06 00:00:15.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ph.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      739 2023-01-06 00:00:15.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/pk.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      222 2023-01-06 00:00:15.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/pl.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-06 00:00:15.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/pm.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    10878 2023-01-06 00:00:15.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/pn.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      637 2023-01-06 00:00:16.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/pr.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      561 2023-01-06 00:00:16.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ps.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     8280 2023-01-06 00:00:16.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/pt.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      467 2023-01-06 00:00:16.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/pw.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    17097 2023-01-06 00:00:16.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/py.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      359 2023-01-06 00:00:16.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/qa.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-06 00:00:16.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/re.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      305 2023-01-06 00:00:16.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ro.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)   187134 2023-01-06 00:00:16.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/rs.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      286 2023-01-06 00:00:17.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ru.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      747 2023-01-06 00:00:17.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/rw.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    10238 2023-01-06 00:00:17.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/sa.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      953 2023-01-06 00:00:17.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/sb.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      571 2023-01-06 00:00:17.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/sc.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      497 2023-01-06 00:00:17.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/sd.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      691 2023-01-06 00:00:18.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/se.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      887 2023-01-06 00:00:18.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/sg.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    29501 2023-01-06 00:00:18.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/sh.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2053 2023-01-06 00:00:18.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/si.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      321 2023-01-06 00:00:18.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/sj.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1202 2023-01-06 00:00:19.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/sk.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      275 2023-01-06 00:00:19.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/sl.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    15801 2023-01-06 00:00:19.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/sm.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      424 2023-01-06 00:00:19.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/sn.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      497 2023-01-06 00:00:19.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/so.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      315 2023-01-06 00:00:19.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/sr.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      386 2023-01-06 00:00:19.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ss.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      916 2023-01-06 00:00:19.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/st.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    82697 2023-01-06 00:00:20.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/sv.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    13209 2023-01-06 00:00:20.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/sx.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      565 2023-01-06 00:00:20.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/sy.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     6742 2023-01-06 00:00:20.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/sz.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    14497 2023-01-06 00:00:20.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/tc.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      267 2023-01-06 00:00:20.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/td.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1088 2023-01-06 00:00:20.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/tf.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      728 2023-01-06 00:00:20.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/tg.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      287 2023-01-06 00:00:21.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/th.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1812 2023-01-06 00:00:21.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/tj.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      788 2023-01-06 00:00:21.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/tk.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      603 2023-01-06 00:00:21.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/tl.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    32287 2023-01-06 00:00:21.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/tm.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      751 2023-01-06 00:00:21.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/tn.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      355 2023-01-06 00:00:22.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/to.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      554 2023-01-06 00:00:22.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/tr.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      315 2023-01-06 00:00:22.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/tt.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1783 2023-01-06 00:00:22.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/tv.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      945 2023-01-06 00:00:22.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/tw.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      549 2023-01-06 00:00:22.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/tz.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      238 2023-01-06 00:00:22.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ua.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3951 2023-01-06 00:00:23.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ug.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     4523 2023-01-06 00:00:23.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/um.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    19935 2023-01-06 00:00:23.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/un.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     4461 2023-01-06 00:00:23.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/us.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1718 2023-01-06 00:00:23.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/uy.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1454 2023-01-06 00:00:23.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/uz.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    91076 2023-01-06 00:00:23.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/va.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      451 2023-01-06 00:00:23.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/vc.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1168 2023-01-06 00:00:24.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ve.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    24640 2023-01-06 00:00:24.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/vg.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     8742 2023-01-06 00:00:24.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/vi.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      494 2023-01-06 00:00:24.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/vn.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3772 2023-01-06 00:00:24.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/vu.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-06 00:00:24.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/wf.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      693 2023-01-06 00:00:24.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ws.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     9643 2023-01-06 00:00:24.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/xk.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      275 2023-01-06 00:00:25.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ye.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-06 00:00:25.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/yt.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)      859 2023-01-06 00:00:25.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/za.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     5497 2023-01-06 00:00:25.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/zm.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     6641 2023-01-06 00:00:26.000000 djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/zw.svg
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.201464 djgentelella-0.3.8/djgentelella/static/vendors/font-awesome/
--rw-r--r--   0 luisza    (1000) luisza    (1000)    21778 2023-01-05 23:59:12.000000 djgentelella-0.3.8/djgentelella/static/vendors/font-awesome/font-awesome.css.map
--rw-r--r--   0 luisza    (1000) luisza    (1000)    31000 2023-01-05 23:59:12.000000 djgentelella-0.3.8/djgentelella/static/vendors/font-awesome/font-awesome.min.css
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.201464 djgentelella-0.3.8/djgentelella/static/vendors/fonts/
--rw-r--r--   0 luisza    (1000) luisza    (1000)   134808 2023-01-05 23:59:12.000000 djgentelella-0.3.8/djgentelella/static/vendors/fonts/FontAwesome.otf
--rw-r--r--   0 luisza    (1000) luisza    (1000)   165742 2023-01-05 23:59:12.000000 djgentelella-0.3.8/djgentelella/static/vendors/fonts/fontawesome-webfont.eot
--rw-r--r--   0 luisza    (1000) luisza    (1000)   444379 2023-01-05 23:59:12.000000 djgentelella-0.3.8/djgentelella/static/vendors/fonts/fontawesome-webfont.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)   165548 2023-01-05 23:59:12.000000 djgentelella-0.3.8/djgentelella/static/vendors/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 luisza    (1000) luisza    (1000)    98024 2023-01-05 23:59:12.000000 djgentelella-0.3.8/djgentelella/static/vendors/fonts/fontawesome-webfont.woff
--rw-r--r--   0 luisza    (1000) luisza    (1000)    77160 2023-01-05 23:59:12.000000 djgentelella-0.3.8/djgentelella/static/vendors/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 luisza    (1000) luisza    (1000)    20127 2023-01-05 23:59:11.000000 djgentelella-0.3.8/djgentelella/static/vendors/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 luisza    (1000) luisza    (1000)   108738 2023-01-05 23:59:11.000000 djgentelella-0.3.8/djgentelella/static/vendors/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    45404 2023-01-05 23:59:11.000000 djgentelella-0.3.8/djgentelella/static/vendors/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 luisza    (1000) luisza    (1000)    23424 2023-01-05 23:59:11.000000 djgentelella-0.3.8/djgentelella/static/vendors/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 luisza    (1000) luisza    (1000)    18028 2023-01-05 23:59:11.000000 djgentelella-0.3.8/djgentelella/static/vendors/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.205464 djgentelella-0.3.8/djgentelella/static/vendors/fullcalendar/
--rw-r--r--   0 luisza    (1000) luisza    (1000)    46228 2023-01-06 00:00:28.000000 djgentelella-0.3.8/djgentelella/static/vendors/fullcalendar/locales-all.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)    25839 2023-01-06 00:00:29.000000 djgentelella-0.3.8/djgentelella/static/vendors/fullcalendar/main.min.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)   269560 2023-01-06 00:00:28.000000 djgentelella-0.3.8/djgentelella/static/vendors/fullcalendar/main.min.js
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.205464 djgentelella-0.3.8/djgentelella/static/vendors/grid-slider/
--rw-r--r--   0 luisza    (1000) luisza    (1000)    11084 2023-01-06 00:00:33.000000 djgentelella-0.3.8/djgentelella/static/vendors/grid-slider/ion.rangeSlider.min.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)    41171 2023-01-06 00:00:33.000000 djgentelella-0.3.8/djgentelella/static/vendors/grid-slider/ion.rangeSlider.min.js
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.205464 djgentelella-0.3.8/djgentelella/static/vendors/iCheck/
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1302 2023-01-05 23:59:14.000000 djgentelella-0.3.8/djgentelella/static/vendors/iCheck/aero.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1302 2023-01-05 23:59:15.000000 djgentelella-0.3.8/djgentelella/static/vendors/iCheck/aero.png
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3021 2023-01-05 23:59:16.000000 djgentelella-0.3.8/djgentelella/static/vendors/iCheck/aero@2x.png
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1302 2023-01-05 23:59:14.000000 djgentelella-0.3.8/djgentelella/static/vendors/iCheck/blue.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1298 2023-01-05 23:59:15.000000 djgentelella-0.3.8/djgentelella/static/vendors/iCheck/blue.png
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3022 2023-01-05 23:59:15.000000 djgentelella-0.3.8/djgentelella/static/vendors/iCheck/blue@2x.png
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1317 2023-01-05 23:59:14.000000 djgentelella-0.3.8/djgentelella/static/vendors/iCheck/green.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1299 2023-01-05 23:59:15.000000 djgentelella-0.3.8/djgentelella/static/vendors/iCheck/green.png
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3022 2023-01-05 23:59:15.000000 djgentelella-0.3.8/djgentelella/static/vendors/iCheck/green@2x.png
--rw-r--r--   0 luisza    (1000) luisza    (1000)     4931 2023-01-05 23:59:14.000000 djgentelella-0.3.8/djgentelella/static/vendors/iCheck/icheck.min.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1332 2023-01-05 23:59:15.000000 djgentelella-0.3.8/djgentelella/static/vendors/iCheck/orange.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1299 2023-01-05 23:59:15.000000 djgentelella-0.3.8/djgentelella/static/vendors/iCheck/orange.png
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3022 2023-01-05 23:59:16.000000 djgentelella-0.3.8/djgentelella/static/vendors/iCheck/orange@2x.png
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1332 2023-01-05 23:59:14.000000 djgentelella-0.3.8/djgentelella/static/vendors/iCheck/yellow.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1303 2023-01-05 23:59:15.000000 djgentelella-0.3.8/djgentelella/static/vendors/iCheck/yellow.png
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3021 2023-01-05 23:59:16.000000 djgentelella-0.3.8/djgentelella/static/vendors/iCheck/yellow@2x.png
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.109464 djgentelella-0.3.8/djgentelella/static/vendors/img/
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.205464 djgentelella-0.3.8/djgentelella/static/vendors/img/bootstrap-colorpicker/
--rw-r--r--   0 luisza    (1000) luisza    (1000)      557 2023-01-06 00:00:31.000000 djgentelella-0.3.8/djgentelella/static/vendors/img/bootstrap-colorpicker/alpha-horizontal.png
--rw-r--r--   0 luisza    (1000) luisza    (1000)      468 2023-01-06 00:00:31.000000 djgentelella-0.3.8/djgentelella/static/vendors/img/bootstrap-colorpicker/alpha.png
--rw-r--r--   0 luisza    (1000) luisza    (1000)      444 2023-01-06 00:00:31.000000 djgentelella-0.3.8/djgentelella/static/vendors/img/bootstrap-colorpicker/hue-horizontal.png
--rw-r--r--   0 luisza    (1000) luisza    (1000)      459 2023-01-06 00:00:31.000000 djgentelella-0.3.8/djgentelella/static/vendors/img/bootstrap-colorpicker/hue.png
--rw-r--r--   0 luisza    (1000) luisza    (1000)    52321 2023-01-06 00:00:31.000000 djgentelella-0.3.8/djgentelella/static/vendors/img/bootstrap-colorpicker/saturation-horizontal.png
--rw-r--r--   0 luisza    (1000) luisza    (1000)     4143 2023-01-06 00:00:31.000000 djgentelella-0.3.8/djgentelella/static/vendors/img/bootstrap-colorpicker/saturation.png
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.205464 djgentelella-0.3.8/djgentelella/static/vendors/inputmask/
--rw-r--r--   0 luisza    (1000) luisza    (1000)    51226 2023-01-05 23:59:17.000000 djgentelella-0.3.8/djgentelella/static/vendors/inputmask/inputmask.min.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1662 2023-01-05 23:59:17.000000 djgentelella-0.3.8/djgentelella/static/vendors/inputmask/jquery.inputmask.min.js
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.205464 djgentelella-0.3.8/djgentelella/static/vendors/interact/
--rw-r--r--   0 luisza    (1000) luisza    (1000)   130770 2023-01-06 00:00:29.000000 djgentelella-0.3.8/djgentelella/static/vendors/interact/interact.min.js
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.209464 djgentelella-0.3.8/djgentelella/static/vendors/jquery/
--rw-r--r--   0 luisza    (1000) luisza    (1000)    89664 2023-01-05 23:59:17.000000 djgentelella-0.3.8/djgentelella/static/vendors/jquery/jquery.min.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)   138161 2023-01-05 23:59:17.000000 djgentelella-0.3.8/djgentelella/static/vendors/jquery/jquery.min.map
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.209464 djgentelella-0.3.8/djgentelella/static/vendors/jquery-knob/
--rw-r--r--   0 luisza    (1000) luisza    (1000)    10804 2023-01-05 23:59:17.000000 djgentelella-0.3.8/djgentelella/static/vendors/jquery-knob/jquery.knob.min.js
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.209464 djgentelella-0.3.8/djgentelella/static/vendors/jquery-ui/
--rw-r--r--   0 luisza    (1000) luisza    (1000)    31340 2023-01-05 23:59:17.000000 djgentelella-0.3.8/djgentelella/static/vendors/jquery-ui/jquery-ui.min.css
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.209464 djgentelella-0.3.8/djgentelella/static/vendors/moment/
--rw-r--r--   0 luisza    (1000) luisza    (1000)   206984 2023-01-05 23:59:17.000000 djgentelella-0.3.8/djgentelella/static/vendors/moment/moment-with-locales.min.js
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.209464 djgentelella-0.3.8/djgentelella/static/vendors/nprogress/
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1100 2023-01-05 23:59:16.000000 djgentelella-0.3.8/djgentelella/static/vendors/nprogress/nprogress.min.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)     4114 2023-01-05 23:59:16.000000 djgentelella-0.3.8/djgentelella/static/vendors/nprogress/nprogress.min.js
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.209464 djgentelella-0.3.8/djgentelella/static/vendors/parsleyjs/
--rw-r--r--   0 luisza    (1000) luisza    (1000)    40946 2023-01-05 23:59:17.000000 djgentelella-0.3.8/djgentelella/static/vendors/parsleyjs/parsley.min.js
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.209464 djgentelella-0.3.8/djgentelella/static/vendors/select2/
--rw-r--r--   0 luisza    (1000) luisza    (1000)    31223 2023-01-05 23:59:14.000000 djgentelella-0.3.8/djgentelella/static/vendors/select2/select2-bootstrap-5-theme.min.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)    16264 2023-01-05 23:59:13.000000 djgentelella-0.3.8/djgentelella/static/vendors/select2/select2.min.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)    73163 2023-01-05 23:59:13.000000 djgentelella-0.3.8/djgentelella/static/vendors/select2/select2.min.js
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.209464 djgentelella-0.3.8/djgentelella/static/vendors/storylinejs/
--rw-r--r--   0 luisza    (1000) luisza    (1000)    16975 2023-01-06 00:00:36.000000 djgentelella-0.3.8/djgentelella/static/vendors/storylinejs/storyline.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)  3283887 2023-01-06 00:00:37.000000 djgentelella-0.3.8/djgentelella/static/vendors/storylinejs/storyline.js
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.213464 djgentelella-0.3.8/djgentelella/static/vendors/storymapjs/
--rw-r--r--   0 luisza    (1000) luisza    (1000)    89683 2023-01-06 00:00:30.000000 djgentelella-0.3.8/djgentelella/static/vendors/storymapjs/storymap.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)   255419 2023-01-06 00:00:30.000000 djgentelella-0.3.8/djgentelella/static/vendors/storymapjs/storymap.js
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.213464 djgentelella-0.3.8/djgentelella/static/vendors/summernote/
--rw-r--r--   0 luisza    (1000) luisza    (1000)    30447 2023-01-06 00:00:34.000000 djgentelella-0.3.8/djgentelella/static/vendors/summernote/summernote-lite.min.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)   163197 2023-01-06 00:00:34.000000 djgentelella-0.3.8/djgentelella/static/vendors/summernote/summernote-lite.min.js
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.213464 djgentelella-0.3.8/djgentelella/static/vendors/sweetalert2/
--rw-r--r--   0 luisza    (1000) luisza    (1000)    69578 2023-01-06 00:00:33.000000 djgentelella-0.3.8/djgentelella/static/vendors/sweetalert2/sweetalert2.all.min.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)    24444 2023-01-06 00:00:33.000000 djgentelella-0.3.8/djgentelella/static/vendors/sweetalert2/sweetalert2.min.css
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.213464 djgentelella-0.3.8/djgentelella/static/vendors/switchery/
--rw-r--r--   0 luisza    (1000) luisza    (1000)      682 2023-01-05 23:59:14.000000 djgentelella-0.3.8/djgentelella/static/vendors/switchery/switchery.min.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)    24502 2023-01-05 23:59:14.000000 djgentelella-0.3.8/djgentelella/static/vendors/switchery/switchery.min.js
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.213464 djgentelella-0.3.8/djgentelella/static/vendors/tagify/
--rw-r--r--   0 luisza    (1000) luisza    (1000)    45904 2023-01-06 00:00:32.000000 djgentelella-0.3.8/djgentelella/static/vendors/tagify/jQuery.tagify.min.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)     9528 2023-01-06 00:00:33.000000 djgentelella-0.3.8/djgentelella/static/vendors/tagify/tagify.min.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)    45259 2023-01-06 00:00:32.000000 djgentelella-0.3.8/djgentelella/static/vendors/tagify/tagify.min.js
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.109464 djgentelella-0.3.8/djgentelella/static/vendors/timeline/
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.217464 djgentelella-0.3.8/djgentelella/static/vendors/timeline/css/
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.217464 djgentelella-0.3.8/djgentelella/static/vendors/timeline/css/icons/
--rw-r--r--   0 luisza    (1000) luisza    (1000)    13172 2023-01-06 00:00:29.000000 djgentelella-0.3.8/djgentelella/static/vendors/timeline/css/icons/tl-icons.eot
--rw-r--r--   0 luisza    (1000) luisza    (1000)    41332 2023-01-06 00:00:29.000000 djgentelella-0.3.8/djgentelella/static/vendors/timeline/css/icons/tl-icons.svg
--rw-r--r--   0 luisza    (1000) luisza    (1000)    13008 2023-01-06 00:00:29.000000 djgentelella-0.3.8/djgentelella/static/vendors/timeline/css/icons/tl-icons.ttf
--rw-r--r--   0 luisza    (1000) luisza    (1000)    91644 2023-01-06 00:00:29.000000 djgentelella-0.3.8/djgentelella/static/vendors/timeline/css/timeline.css
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.217464 djgentelella-0.3.8/djgentelella/static/vendors/timeline/js/
--rw-r--r--   0 luisza    (1000) luisza    (1000)   207822 2023-01-06 00:00:29.000000 djgentelella-0.3.8/djgentelella/static/vendors/timeline/js/timeline.js
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.217464 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/
--rw-r--r--   0 luisza    (1000) luisza    (1000)     6671 2023-01-06 00:00:34.000000 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/jquery.tinymce.min.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)    60883 2023-01-06 00:00:43.000000 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skin.min.css
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.109464 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.109464 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/content/
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.217464 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/content/dark/
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1469 2023-01-06 00:00:34.000000 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/content/dark/content.min.css
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.217464 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/content/default/
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1399 2023-01-06 00:00:35.000000 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/content/default/content.min.css
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.217464 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/content/document/
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1498 2023-01-06 00:00:35.000000 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/content/document/content.min.css
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.217464 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/content/writer/
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1420 2023-01-06 00:00:35.000000 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/content/writer/content.min.css
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.109464 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/ui/
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.217464 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/ui/oxide/
--rw-r--r--   0 luisza    (1000) luisza    (1000)    21708 2023-01-06 00:00:36.000000 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/ui/oxide/content.inline.min.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)    21767 2023-01-06 00:00:36.000000 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/ui/oxide/content.min.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)      544 2023-01-06 00:00:36.000000 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/ui/oxide/content.mobile.min.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)    60882 2023-01-06 00:00:36.000000 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/ui/oxide/skin.min.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)    21004 2023-01-06 00:00:36.000000 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/ui/oxide/skin.mobile.min.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)      735 2023-01-06 00:00:36.000000 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/ui/oxide/skin.shadowdom.min.css
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.221464 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/ui/oxide-dark/
--rw-r--r--   0 luisza    (1000) luisza    (1000)    21708 2023-01-06 00:00:35.000000 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/ui/oxide-dark/content.inline.min.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)    21384 2023-01-06 00:00:35.000000 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/ui/oxide-dark/content.min.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)      544 2023-01-06 00:00:35.000000 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/ui/oxide-dark/content.mobile.min.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)    60766 2023-01-06 00:00:35.000000 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/ui/oxide-dark/skin.min.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)    21004 2023-01-06 00:00:35.000000 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/ui/oxide-dark/skin.mobile.min.css
--rw-r--r--   0 luisza    (1000) luisza    (1000)      735 2023-01-06 00:00:36.000000 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/ui/oxide-dark/skin.shadowdom.min.css
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.109464 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/themes/
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.221464 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/themes/mobile/
--rw-r--r--   0 luisza    (1000) luisza    (1000)   171088 2023-01-06 00:00:34.000000 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/themes/mobile/theme.min.js
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.221464 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/themes/silver/
--rw-r--r--   0 luisza    (1000) luisza    (1000)   411481 2023-01-06 00:00:34.000000 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/themes/silver/theme.min.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)   736670 2023-01-06 00:00:43.000000 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/tinymce-all.js
--rw-r--r--   0 luisza    (1000) luisza    (1000)   395541 2023-01-06 00:00:34.000000 djgentelella-0.3.8/djgentelella/static/vendors/tinymce/tinymce.min.js
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.109464 djgentelella-0.3.8/djgentelella/templates/
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.109464 djgentelella-0.3.8/djgentelella/templates/cruds/
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.221464 djgentelella-0.3.8/djgentelella/templates/cruds/ajax/
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1639 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/cruds/ajax/_form.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      417 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/cruds/ajax/create.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1325 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/cruds/ajax/delete.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3219 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/cruds/ajax/list.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      412 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/cruds/ajax/update.html
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.221464 djgentelella-0.3.8/djgentelella/templates/gentelella/
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.221464 djgentelella-0.3.8/djgentelella/templates/gentelella/app/
--rw-r--r--   0 luisza    (1000) luisza    (1000)      207 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/app/footer.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2755 2022-11-04 01:21:36.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/app/messages.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      668 2022-10-28 14:04:53.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/app/sidebar.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1407 2023-01-05 22:10:06.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/app/top_navigation.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)    11361 2023-01-05 22:27:05.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/base.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)       36 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/base_site.html
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.221464 djgentelella-0.3.8/djgentelella/templates/gentelella/blocks/
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1229 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/blocks/box.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1497 2022-11-04 01:33:58.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/blocks/crud_list.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      312 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/blocks/helper_prototype.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2043 2022-11-03 23:12:02.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/blocks/permissions_management.html
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.225464 djgentelella-0.3.8/djgentelella/templates/gentelella/cruds/
--rw-r--r--   0 luisza    (1000) luisza    (1000)      334 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/cruds/403.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      970 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/cruds/_form.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1221 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/cruds/create.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      195 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/cruds/crud_fields.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1803 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/cruds/delete.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2148 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/cruds/detail.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)     6362 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/cruds/list.html
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.225464 djgentelella-0.3.8/djgentelella/templates/gentelella/cruds/pagination/
--rw-r--r--   0 luisza    (1000) luisza    (1000)      337 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/cruds/pagination/enumeration.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      731 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/cruds/pagination/prev_next.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3862 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/cruds/update.html
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.225464 djgentelella-0.3.8/djgentelella/templates/gentelella/email/
--rw-r--r--   0 luisza    (1000) luisza    (1000)       55 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/email/base.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      287 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/email/notification.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1125 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/index.html
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.225464 djgentelella-0.3.8/djgentelella/templates/gentelella/menu/
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1659 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/menu/notificacion.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2531 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/menu/notification_list.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1675 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/menu/palette.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2290 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/menu/palette_modal.html
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.225464 djgentelella-0.3.8/djgentelella/templates/gentelella/permission_management/
--rw-r--r--   0 luisza    (1000) luisza    (1000)      549 2022-10-28 14:04:53.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/permission_management/permissionmanagement_list.html
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.225464 djgentelella-0.3.8/djgentelella/templates/gentelella/registration/
--rw-r--r--   0 luisza    (1000) luisza    (1000)      410 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/registration/activate.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      434 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/registration/activation_complete.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      223 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/registration/activation_email.txt
--rw-r--r--   0 luisza    (1000) luisza    (1000)       67 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/registration/activation_email_subject.txt
--rw-r--r--   0 luisza    (1000) luisza    (1000)      886 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/registration/email_base.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/registration/email_footer.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/registration/email_header.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      209 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/registration/footer.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2195 2022-11-08 16:55:36.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/registration/login.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      694 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/registration/logout.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      693 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/registration/new_user.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      404 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/registration/password_change_done.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      524 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/registration/password_change_form.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      485 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/registration/password_reset_complete.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      679 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/registration/password_reset_confirm.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      634 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/registration/password_reset_done.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      618 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/registration/password_reset_email.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/registration/password_reset_email.txt
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1544 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/registration/password_reset_form.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      125 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/registration/password_reset_subject.txt
--rw-r--r--   0 luisza    (1000) luisza    (1000)      422 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/registration/registration_closed.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      433 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/registration/registration_complete.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      525 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/registration/registration_form.html
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.233464 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1480 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/addselect.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1413 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/addtreeselect.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      173 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/attrs.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      409 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/autocomplete_select.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      307 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/calendar.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      165 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/chart.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      109 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/chartjs.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)       53 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/checkbox.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)       53 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/checkbox_option.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)       54 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/checkbox_select.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      103 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/checkyesno.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1517 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/chunkedupload.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      459 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/clearable_file_input.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      111 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/color_default.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      162 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/color_inline.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      389 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/color_style.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)       93 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/credit_card_input_mask.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      258 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/custom_input.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)       94 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/custom_input_mask.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      243 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/date.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)       94 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/date_input_mask.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      242 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/daterange.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)       97 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/daterangetime.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      201 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/datetime.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)       94 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/datetime_input_mask.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)       46 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/email.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)       94 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/email_input_mask.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1337 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/file.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)       46 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/hidden.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)       94 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/identification_card_input_mask.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      187 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/input.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)       94 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/input_mask.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      216 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/input_option.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)       52 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/multiple_hidden.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      461 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/multiple_input.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      116 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/multiwidget.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)       45 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/number.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      161 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/number_knob_input.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)       45 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/password.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)       94 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/phone_number_input_mask.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      630 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/radio.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      216 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/radio_input_option.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)       52 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/radio_option.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)       54 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/radio_select.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      383 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/select.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)       52 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/select_date.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      124 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/select_option.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)       94 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/serial_number_input_mask.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)       51 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/splitdatetime.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)       52 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/splithiddendatetime.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)       58 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/storyline.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      122 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/storymap_gigapixel.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      101 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/storymap_mapbased.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)       46 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/tagging.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)       94 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/taxid_input_mask.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)       46 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/text.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      143 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/textarea.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      200 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/time.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)       82 2022-10-28 05:40:35.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/timeline.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      387 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/tree_select.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      211 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/tree_select_option.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)       45 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/url.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)      249 2022-10-28 14:04:53.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/wysiwyg.html
--rw-r--r--   0 luisza    (1000) luisza    (1000)       48 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/wysiwygtwo.html
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.233464 djgentelella-0.3.8/djgentelella/templatetags/
--rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/templatetags/__init__.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1855 2022-12-21 20:53:40.000000 djgentelella-0.3.8/djgentelella/templatetags/_utils.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     6328 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/templatetags/crud_tags.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     7675 2022-12-21 21:47:19.000000 djgentelella-0.3.8/djgentelella/templatetags/gentelellamenu.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1440 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/templatetags/gtsettings.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)      476 2022-12-21 20:53:40.000000 djgentelella-0.3.8/djgentelella/templatetags/timejs.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)       59 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/templatetags/tree_tags.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1945 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/templatetags/urlname_tags.py
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.233464 djgentelella-0.3.8/djgentelella/tests/
--rw-r--r--   0 luisza    (1000) luisza    (1000)     5219 2022-12-21 20:53:40.000000 djgentelella-0.3.8/djgentelella/tests/Calendar_Test.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     8523 2022-12-21 20:53:40.000000 djgentelella-0.3.8/djgentelella/tests/StoryLine_Test.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     4031 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/tests/StoryMap_Test.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3540 2022-12-21 20:53:40.000000 djgentelella-0.3.8/djgentelella/tests/TimeLine_Test.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)      117 2022-12-21 20:53:40.000000 djgentelella-0.3.8/djgentelella/tests/__init__.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     4246 2022-12-21 21:50:47.000000 djgentelella-0.3.8/djgentelella/urls.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)      825 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/utils.py
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.237464 djgentelella-0.3.8/djgentelella/views/
--rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/views/__init__.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)       97 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/views/auth.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     4415 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/views/select2autocomplete.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2793 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/views/storyline.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1025 2022-12-21 20:53:40.000000 djgentelella-0.3.8/djgentelella/views/storymap.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)      786 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/views/timeline.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-12-21 21:30:55.000000 djgentelella-0.3.8/djgentelella/views/upload.py
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.237464 djgentelella-0.3.8/djgentelella/widgets/
--rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/widgets/__init__.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1459 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/widgets/calendar.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1895 2022-12-21 21:43:38.000000 djgentelella-0.3.8/djgentelella/widgets/color.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)    19465 2022-12-21 21:27:48.000000 djgentelella-0.3.8/djgentelella/widgets/core.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1348 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/widgets/files.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)      826 2022-12-21 20:53:40.000000 djgentelella-0.3.8/djgentelella/widgets/helper.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)      407 2022-12-21 20:53:40.000000 djgentelella-0.3.8/djgentelella/widgets/numberknobinput.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     3191 2023-01-05 16:23:19.000000 djgentelella-0.3.8/djgentelella/widgets/selects.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1155 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/widgets/storyline.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2350 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/widgets/storymap.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1110 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/widgets/tagging.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1204 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/widgets/timeline.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)      607 2022-12-21 20:53:41.000000 djgentelella-0.3.8/djgentelella/widgets/tinymce.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     2212 2022-12-21 20:53:40.000000 djgentelella-0.3.8/djgentelella/widgets/trees.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)      609 2022-12-21 20:53:40.000000 djgentelella-0.3.8/djgentelella/widgets/wysiwyg.py
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.237464 djgentelella-0.3.8/djgentelella/wysiwyg/
--rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.8/djgentelella/wysiwyg/__init__.py
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1159 2022-12-21 21:31:09.000000 djgentelella-0.3.8/djgentelella/wysiwyg/views.py
-drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-06 00:00:44.113464 djgentelella-0.3.8/djgentelella.egg-info/
--rw-r--r--   0 luisza    (1000) luisza    (1000)     4911 2023-01-06 00:00:44.000000 djgentelella-0.3.8/djgentelella.egg-info/PKG-INFO
--rw-r--r--   0 luisza    (1000) luisza    (1000)    45216 2023-01-06 00:00:44.000000 djgentelella-0.3.8/djgentelella.egg-info/SOURCES.txt
--rw-r--r--   0 luisza    (1000) luisza    (1000)        1 2023-01-06 00:00:44.000000 djgentelella-0.3.8/djgentelella.egg-info/dependency_links.txt
--rw-r--r--   0 luisza    (1000) luisza    (1000)        1 2023-01-06 00:00:44.000000 djgentelella-0.3.8/djgentelella.egg-info/not-zip-safe
--rw-r--r--   0 luisza    (1000) luisza    (1000)      141 2023-01-06 00:00:44.000000 djgentelella-0.3.8/djgentelella.egg-info/requires.txt
--rw-r--r--   0 luisza    (1000) luisza    (1000)       13 2023-01-06 00:00:44.000000 djgentelella-0.3.8/djgentelella.egg-info/top_level.txt
--rw-r--r--   0 luisza    (1000) luisza    (1000)      148 2022-10-28 14:04:53.000000 djgentelella-0.3.8/requirements.txt
--rw-r--r--   0 luisza    (1000) luisza    (1000)       38 2023-01-06 00:00:44.237464 djgentelella-0.3.8/setup.cfg
--rw-r--r--   0 luisza    (1000) luisza    (1000)     1604 2023-01-05 16:27:45.000000 djgentelella-0.3.8/setup.py
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.630876 djgentelella-0.3.9/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    18047 2022-09-27 22:26:00.000000 djgentelella-0.3.9/LICENSE
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      206 2022-09-27 22:26:00.000000 djgentelella-0.3.9/MANIFEST.in
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     4911 2023-01-17 16:40:40.630876 djgentelella-0.3.9/PKG-INFO
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2883 2022-10-28 14:04:53.000000 djgentelella-0.3.9/Readme.rst
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.502875 djgentelella-0.3.9/djgentelella/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       22 2023-01-17 16:25:15.000000 djgentelella-0.3.9/djgentelella/__init__.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1304 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/admin.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      153 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/apps.py
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.506875 djgentelella-0.3.9/djgentelella/blog/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/blog/__init__.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       29 2022-12-21 20:53:40.000000 djgentelella-0.3.9/djgentelella/blog/admin.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      150 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/blog/apps.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      919 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/blog/forms.py
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.506875 djgentelella-0.3.9/djgentelella/blog/migrations/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3175 2022-12-21 21:53:07.000000 djgentelella-0.3.9/djgentelella/blog/migrations/0001_initial.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/blog/migrations/__init__.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3796 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/blog/models.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      483 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/blog/sitemaps.py
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.494876 djgentelella-0.3.9/djgentelella/blog/static/
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.506875 djgentelella-0.3.9/djgentelella/blog/static/images/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    85355 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/blog/static/images/article.png
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.494876 djgentelella-0.3.9/djgentelella/blog/templates/
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.494876 djgentelella-0.3.9/djgentelella/blog/templates/gentelella/
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.506875 djgentelella-0.3.9/djgentelella/blog/templates/gentelella/blog/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      123 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/blog/templates/gentelella/blog/category_add.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      688 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/blog/templates/gentelella/blog/entry_delete.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1976 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/blog/templates/gentelella/blog/entry_detail.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      806 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/blog/templates/gentelella/blog/entry_form.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     5528 2022-11-08 16:55:36.000000 djgentelella-0.3.9/djgentelella/blog/templates/gentelella/blog/entry_list.html
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.506875 djgentelella-0.3.9/djgentelella/blog/templatetags/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-12-21 21:56:51.000000 djgentelella-0.3.9/djgentelella/blog/templatetags/__init__.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      621 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/blog/templatetags/blog_tags.py
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.506875 djgentelella-0.3.9/djgentelella/blog/tests/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/blog/tests/__init__.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      849 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/blog/tests/test_entry_detail.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1983 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/blog/tests/test_entry_forms.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1046 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/blog/tests/test_entry_listing.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     4147 2022-12-21 21:46:47.000000 djgentelella-0.3.9/djgentelella/blog/tests/test_models.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1299 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/blog/tests/test_sitemaps.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2105 2022-12-21 21:56:42.000000 djgentelella-0.3.9/djgentelella/blog/tests/test_templatetags.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       26 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/blog/tests.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      582 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/blog/urls.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     5761 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/blog/views.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     8572 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/chartjs.py
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.506875 djgentelella-0.3.9/djgentelella/chunked_upload/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-10-08 03:13:40.000000 djgentelella-0.3.9/djgentelella/chunked_upload/__init__.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      300 2022-10-08 03:13:40.000000 djgentelella-0.3.9/djgentelella/chunked_upload/constants.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2908 2022-12-21 21:32:15.000000 djgentelella-0.3.9/djgentelella/chunked_upload/models.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      388 2022-10-08 03:13:40.000000 djgentelella-0.3.9/djgentelella/chunked_upload/response.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    11110 2022-12-21 21:32:07.000000 djgentelella-0.3.9/djgentelella/chunked_upload/views.py
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.506875 djgentelella-0.3.9/djgentelella/cruds/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/cruds/__init__.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    28229 2022-12-21 21:44:14.000000 djgentelella-0.3.9/djgentelella/cruds/base.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2685 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/cruds/filter.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     9405 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/cruds/inline_crud.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3115 2022-12-21 21:31:25.000000 djgentelella-0.3.9/djgentelella/cruds/utils.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3340 2022-12-21 20:53:40.000000 djgentelella-0.3.9/djgentelella/elements.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      262 2022-10-08 03:13:40.000000 djgentelella-0.3.9/djgentelella/exceptions.py
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.506875 djgentelella-0.3.9/djgentelella/fields/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/fields/__init__.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2551 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/fields/catalog.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1880 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/fields/drfdatetime.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2209 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/fields/tree.py
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.510875 djgentelella-0.3.9/djgentelella/forms/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       84 2022-12-21 20:53:40.000000 djgentelella-0.3.9/djgentelella/forms/__init__.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2340 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/forms/decorators.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3092 2022-12-21 21:06:39.000000 djgentelella-0.3.9/djgentelella/forms/forms.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      397 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/forms/models.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      415 2022-12-21 20:53:40.000000 djgentelella-0.3.9/djgentelella/groute.py
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.494876 djgentelella-0.3.9/djgentelella/locale/
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.494876 djgentelella-0.3.9/djgentelella/locale/es/
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.510875 djgentelella-0.3.9/djgentelella/locale/es/LC_MESSAGES/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     8099 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    15549 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.510875 djgentelella-0.3.9/djgentelella/management/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/management/__init__.py
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.510875 djgentelella-0.3.9/djgentelella/management/commands/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/management/commands/__init__.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1538 2023-01-07 04:37:27.000000 djgentelella-0.3.9/djgentelella/management/commands/createbasejs.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1716 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/management/commands/delete_expired_uploads.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    28021 2023-01-17 16:38:14.000000 djgentelella-0.3.9/djgentelella/management/commands/loaddevstatic.py
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.510875 djgentelella-0.3.9/djgentelella/menu_widgets/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/menu_widgets/__init__.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2253 2022-12-21 21:07:10.000000 djgentelella-0.3.9/djgentelella/menu_widgets/palette.py
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.510875 djgentelella-0.3.9/djgentelella/migrations/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2868 2022-12-21 21:52:13.000000 djgentelella-0.3.9/djgentelella/migrations/0001_initial.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     8975 2022-12-21 21:56:12.000000 djgentelella-0.3.9/djgentelella/migrations/0001_squashed_new_initial.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      424 2023-01-05 22:09:21.000000 djgentelella-0.3.9/djgentelella/migrations/0002_alter_permissionscategorymanagement_options.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      993 2022-12-21 21:59:13.000000 djgentelella-0.3.9/djgentelella/migrations/0002_auto_20200214_2038.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      988 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/migrations/0003_help.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      582 2022-12-21 20:53:40.000000 djgentelella-0.3.9/djgentelella/migrations/0004_loadsettings.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1921 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/migrations/0005_notification.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1073 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/migrations/0006_permissionscategorymanagement.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      660 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/migrations/0007_edit_footer.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      479 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/migrations/0008_defaulttheme.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1855 2022-12-21 21:52:28.000000 djgentelella-0.3.9/djgentelella/migrations/0009_chunkedupload.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      707 2022-12-21 20:53:40.000000 djgentelella-0.3.9/djgentelella/migrations/0010_menuitem_position.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1077 2022-12-21 20:53:40.000000 djgentelella-0.3.9/djgentelella/migrations/0011_remove_menuitem_level_remove_menuitem_lft_and_more.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/migrations/__init__.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     4560 2023-01-05 22:06:57.000000 djgentelella-0.3.9/djgentelella/models.py
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.510875 djgentelella-0.3.9/djgentelella/notification/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3585 2023-01-05 21:42:42.000000 djgentelella-0.3.9/djgentelella/notification/__init__.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1672 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/notification/base.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      557 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/notification/serializer.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1752 2022-12-21 20:53:40.000000 djgentelella-0.3.9/djgentelella/notification/widgets.py
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.510875 djgentelella-0.3.9/djgentelella/permission_management/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/permission_management/__init__.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1562 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/permission_management/forms.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     4926 2022-12-21 21:59:57.000000 djgentelella-0.3.9/djgentelella/permission_management/objinterface.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2104 2023-01-17 16:25:15.000000 djgentelella-0.3.9/djgentelella/permission_management/views.py
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.514876 djgentelella-0.3.9/djgentelella/serializers/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/serializers/__init__.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3461 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/serializers/calendar.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      248 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/serializers/helper.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1255 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/serializers/storyline.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2777 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/serializers/storymap.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2132 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/serializers/timeline.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2917 2022-12-21 21:38:13.000000 djgentelella-0.3.9/djgentelella/settings.py
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.498875 djgentelella-0.3.9/djgentelella/static/
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.498875 djgentelella-0.3.9/djgentelella/static/django_ajax/
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.514876 djgentelella-0.3.9/djgentelella/static/django_ajax/js/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     8403 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/static/django_ajax/js/jquery.ajax-plugin.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3030 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/static/django_ajax/js/jquery.ajax-plugin.min.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     6684 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/static/django_ajax/js/jquery.ajax.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3460 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/static/django_ajax/js/jquery.ajax.min.js
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.498875 djgentelella-0.3.9/djgentelella/static/gentelella/
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.514876 djgentelella-0.3.9/djgentelella/static/gentelella/css/
+-rwxr-xr-x   0 luisza    (1000) luisza    (1000)    89690 2022-11-03 22:29:50.000000 djgentelella-0.3.9/djgentelella/static/gentelella/css/custom.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    81514 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/static/gentelella/css/modern.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    81715 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/static/gentelella/css/modern_black_white.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    81264 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/static/gentelella/css/style_black_and_white.css
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.514876 djgentelella-0.3.9/djgentelella/static/gentelella/images/
+-rwxr-xr-x   0 luisza    (1000) luisza    (1000)     1361 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/static/gentelella/images/back_disabled.png
+-rwxr-xr-x   0 luisza    (1000) luisza    (1000)     1379 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/static/gentelella/images/back_enabled.png
+-rwxr-xr-x   0 luisza    (1000) luisza    (1000)     1375 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/static/gentelella/images/back_enabled_hover.png
+-rwxr-xr-x   0 luisza    (1000) luisza    (1000)     1363 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/static/gentelella/images/forward_disabled.png
+-rwxr-xr-x   0 luisza    (1000) luisza    (1000)     1380 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/static/gentelella/images/forward_enabled.png
+-rwxr-xr-x   0 luisza    (1000) luisza    (1000)     1379 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/static/gentelella/images/forward_enabled_hover.png
+-rwxr-xr-x   0 luisza    (1000) luisza    (1000)    30269 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/static/gentelella/images/loading.gif
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.518875 djgentelella-0.3.9/djgentelella/static/gentelella/js/
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.518875 djgentelella-0.3.9/djgentelella/static/gentelella/js/base/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1216 2023-01-17 16:25:15.000000 djgentelella-0.3.9/djgentelella/static/gentelella/js/base/autocompleteSelect2.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1056 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/static/gentelella/js/base/booleanFields.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      772 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/static/gentelella/js/base/calendar.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1567 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/static/gentelella/js/base/chart.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     5533 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/static/gentelella/js/base/custom.widgets.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     5617 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/static/gentelella/js/base/dateranges_gridslider.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1118 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/static/gentelella/js/base/editorTinymce.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     4319 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/static/gentelella/js/base/fileupload.widget.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     7693 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/static/gentelella/js/base/formset.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      627 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/static/gentelella/js/base/gigapixel_storymap.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    10836 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/static/gentelella/js/base/helper_widget.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      542 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/static/gentelella/js/base/mapbased_storymap.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    12381 2023-01-07 04:35:05.000000 djgentelella-0.3.9/djgentelella/static/gentelella/js/base/mediarecord.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     4688 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/static/gentelella/js/base/notifications.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      332 2023-01-17 16:25:15.000000 djgentelella-0.3.9/djgentelella/static/gentelella/js/base/select2_wrap.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     4540 2023-01-17 16:25:15.000000 djgentelella-0.3.9/djgentelella/static/gentelella/js/base/select2related.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      867 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/static/gentelella/js/base/storyline.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      788 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/static/gentelella/js/base/timeline.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      405 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/static/gentelella/js/base/wysiwyg.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    64960 2023-01-17 16:40:40.000000 djgentelella-0.3.9/djgentelella/static/gentelella/js/base.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    14885 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/static/gentelella/js/custom.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     9310 2022-12-17 20:23:41.000000 djgentelella-0.3.9/djgentelella/static/gentelella/js/datatables.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)  3898127 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/static/gentelella/js/gentelella-bundle.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     8211 2022-11-06 19:51:25.000000 djgentelella-0.3.9/djgentelella/static/gentelella/js/permissionmanagement.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    12999 2023-01-17 16:25:15.000000 djgentelella-0.3.9/djgentelella/static/gentelella/js/widgets.js
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.498875 djgentelella-0.3.9/djgentelella/static/vendors/
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.522875 djgentelella-0.3.9/djgentelella/static/vendors/autosize/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3274 2023-01-17 16:40:39.000000 djgentelella-0.3.9/djgentelella/static/vendors/autosize/autosize.min.js
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.522875 djgentelella-0.3.9/djgentelella/static/vendors/bootstrap/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    79790 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/bootstrap/bootstrap.bundle.min.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)   194699 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/bootstrap/bootstrap.min.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    60104 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/bootstrap/bootstrap.min.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    19766 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/bootstrap/popper.min.js
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.522875 djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-colorpicker/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     4002 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-colorpicker/bootstrap-colorpicker.min.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    18689 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-colorpicker/bootstrap-colorpicker.min.js
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.522875 djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-daterangepicker/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     6430 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-daterangepicker/daterangepicker.min.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2876 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-daterangepicker/daterangepicker.min.css.map
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    32018 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-daterangepicker/daterangepicker.min.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    32527 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-daterangepicker/daterangepicker.min.js.map
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    53324 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-daterangepicker/moment.min.js
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.522875 djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-datetimepicker/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     7785 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-datetimepicker/bootstrap-datetimepicker.min.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      146 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-datetimepicker/bootstrap-datetimepicker.min.css.map
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    38510 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-datetimepicker/bootstrap-datetimepicker.min.js
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.522875 djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-maxlength/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     4821 2023-01-17 16:40:39.000000 djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-maxlength/bootstrap-maxlength.min.js
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.522875 djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-progressbar/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     5014 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-progressbar/bootstrap-progressbar-3.3.4.min.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2333 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-progressbar/bootstrap-progressbar.min.js
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.522875 djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-tree/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      521 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-tree/bootstrap-treeview.min.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    27547 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-tree/bootstrap-treeview.min.js
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.522875 djgentelella-0.3.9/djgentelella/static/vendors/chartjs/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      521 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/chartjs/Chart.min.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)   172812 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/chartjs/Chart.min.js
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.498875 djgentelella-0.3.9/djgentelella/static/vendors/css/
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.522875 djgentelella-0.3.9/djgentelella/static/vendors/css/icons/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    14472 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/css/icons/vco-icons.ttf
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.522875 djgentelella-0.3.9/djgentelella/static/vendors/datatables/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    62157 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/datatables/datatables.min.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)   590996 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/datatables/datatables.min.js
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.526875 djgentelella-0.3.9/djgentelella/static/vendors/fileupload/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    18782 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/fileupload/jquery.fileupload.min.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2292 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/fileupload/jquery.iframe-transport.min.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     8398 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/fileupload/jquery.ui.widget.min.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    10158 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/fileupload/spark-md5.min.js
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.526875 djgentelella-0.3.9/djgentelella/static/vendors/flag-icon-css/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    27398 2023-01-17 16:40:39.000000 djgentelella-0.3.9/djgentelella/static/vendors/flag-icon-css/flag-icons.min.css
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.498875 djgentelella-0.3.9/djgentelella/static/vendors/flags/
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.554875 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    32253 2023-01-17 16:40:39.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ad.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      262 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ae.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    20928 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/af.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      761 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ag.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    48199 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ai.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3205 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/al.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      231 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/am.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1588 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ao.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     5958 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/aq.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3473 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ar.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     7828 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/as.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      242 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/at.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1483 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/au.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    12084 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/aw.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      541 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ax.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      498 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/az.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1242 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ba.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      609 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/bb.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      192 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/bd.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      290 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/be.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      383 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/bf.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      294 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/bg.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      538 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/bh.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1042 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/bi.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      499 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/bj.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/bl.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    22270 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/bm.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    14359 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/bn.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)   118659 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/bo.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      228 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/bq.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     7686 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/br.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      568 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/bs.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    25045 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/bt.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      582 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/bv.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      254 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/bw.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     6086 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/by.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    46678 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/bz.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      708 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ca.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3083 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/cc.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      507 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/cd.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      632 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/cf.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      469 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/cg.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      295 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ch.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      283 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ci.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2020 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ck.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      574 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/cl.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      824 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/cm.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      743 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/cn.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      289 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/co.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      293 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/cr.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      573 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/cu.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1357 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/cv.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      682 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/cw.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2496 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/cx.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     5955 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/cy.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      480 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/cz.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      221 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/de.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      585 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/dj.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      235 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/dk.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    16457 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/dm.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)   391369 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/do.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      305 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/dz.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    29875 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ec.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      352 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ee.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     9913 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/eg.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      817 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/eh.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3371 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/er.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      257 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/es-ca.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    92546 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/es.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1226 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/et.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1250 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/eu.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      240 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/fi.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    27518 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/fj.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    31798 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/fk.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      759 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/fm.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      534 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/fo.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/fr.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      278 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ga.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      232 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/gb-eng.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    26487 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/gb-nir.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      239 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/gb-sct.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     9055 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/gb-wls.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      541 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/gb.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1828 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/gd.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1541 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ge.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/gf.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      625 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/gg.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      296 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/gh.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2930 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/gi.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      237 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/gl.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      382 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/gm.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      295 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/gn.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/gp.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     5273 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/gq.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1085 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/gr.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    35061 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/gs.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    37255 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/gt.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     4614 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/gu.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      889 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/gw.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      481 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/gy.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3529 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/hk.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1308 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/hm.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1116 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/hn.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    40852 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/hr.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    15094 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ht.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      276 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/hu.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      239 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/id.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ie.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      848 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/il.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    10197 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/im.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1088 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/in.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    27357 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/io.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1475 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/iq.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    15356 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ir.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      526 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/is.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/it.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     4675 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/je.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      389 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/jm.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      691 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/jo.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      484 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/jp.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1485 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ke.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3316 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/kg.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     7262 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/kh.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     5941 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ki.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1037 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/km.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      817 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/kn.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      852 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/kp.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1719 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/kr.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      507 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/kw.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    22357 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ky.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    11415 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/kz.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      501 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/la.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2747 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/lb.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      370 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/lc.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     8291 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/li.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    11254 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/lk.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      694 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/lr.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1242 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ls.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      442 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/lt.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      232 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/lu.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      237 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/lv.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      526 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ly.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      250 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ma.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      237 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/mc.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    11337 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/md.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    63354 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/me.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/mf.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      302 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/mg.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      763 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/mh.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      410 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/mk.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      279 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ml.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      865 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/mm.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1251 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/mn.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1495 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/mo.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    23628 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/mp.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/mq.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      431 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/mr.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    12140 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ms.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    10422 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/mt.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      319 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/mu.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      307 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/mv.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3797 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/mw.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    90505 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/mx.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1262 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/my.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2597 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/mz.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      977 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/na.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1387 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/nc.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      282 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ne.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     5591 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/nf.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      260 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ng.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    18463 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ni.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      228 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/nl.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      321 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/no.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1193 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/np.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      668 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/nr.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1727 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/nu.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2999 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/nz.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    22614 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/om.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      659 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/pa.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    72907 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/pe.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     4229 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/pf.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2095 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/pg.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1510 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ph.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      684 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/pk.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      222 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/pl.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/pm.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     8517 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/pn.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      619 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/pr.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      541 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ps.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     8661 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/pt.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      507 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/pw.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    17246 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/py.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      356 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/qa.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/re.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      305 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ro.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)   186989 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/rs.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      290 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ru.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      748 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/rw.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    10179 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/sa.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      952 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/sb.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      570 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/sc.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      493 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/sd.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      698 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/se.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      948 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/sg.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    30113 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/sh.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2065 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/si.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      321 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/sj.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1173 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/sk.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      438 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/sl.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    15729 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/sm.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      414 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/sn.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      498 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/so.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      320 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/sr.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      397 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ss.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      920 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/st.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    83238 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/sv.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    12992 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/sx.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      579 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/sy.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     6689 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/sz.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    14756 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/tc.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      279 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/td.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1196 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/tf.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      733 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/tg.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      288 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/th.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1767 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/tj.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      778 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/tk.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      577 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/tl.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    31566 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/tm.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      733 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/tn.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      361 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/to.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      575 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/tr.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      320 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/tt.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1716 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/tv.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      954 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/tw.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      602 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/tz.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      238 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ua.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     4024 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ug.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3972 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/um.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    20185 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/un.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3921 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/us.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1715 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/uy.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1454 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/uz.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    90711 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/va.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      498 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/vc.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1188 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ve.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    24814 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/vg.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     8697 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/vi.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      498 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/vn.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3732 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/vu.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/wf.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      706 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ws.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     8963 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/xk.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      275 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ye.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/yt.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      872 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/za.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     5401 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/zm.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     6614 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/zw.svg
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.590875 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    33473 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ad.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      254 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ae.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    21066 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/af.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      749 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ag.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    48259 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ai.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3206 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/al.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      223 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/am.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1588 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ao.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     6143 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/aq.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3402 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ar.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     8068 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/as.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      240 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/at.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1546 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/au.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     9951 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/aw.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      559 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ax.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      512 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/az.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1310 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ba.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      609 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/bb.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      190 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/bd.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      290 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/be.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      357 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/bf.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      286 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/bg.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      517 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/bh.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1074 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/bi.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      502 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/bj.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/bl.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    22569 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/bm.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    14213 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/bn.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)   117062 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/bo.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      224 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/bq.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     8097 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/br.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      552 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/bs.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    25227 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/bt.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      585 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/bv.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      252 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/bw.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     5962 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/by.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    46427 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/bz.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      728 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ca.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3123 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/cc.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      349 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/cd.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      691 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/cf.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      487 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/cg.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      297 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ch.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      280 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ci.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2097 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ck.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      563 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/cl.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      824 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/cm.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      801 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/cn.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      289 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/co.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      293 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/cr.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      622 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/cu.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1415 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/cv.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      681 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/cw.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2455 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/cx.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     5866 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/cy.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      484 2023-01-17 16:40:39.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/cz.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      213 2023-01-17 16:40:39.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/de.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      591 2023-01-17 16:40:39.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/dj.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      239 2023-01-17 16:40:39.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/dk.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    15975 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/dm.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)   393849 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/do.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      294 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/dz.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    29320 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ec.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      321 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ee.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     9899 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/eg.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      873 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/eh.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3187 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/er.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      258 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/es-ca.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    90819 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/es.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1233 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/et.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1249 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/eu.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      237 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/fi.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    27237 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/fj.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    31973 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/fk.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      776 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/fm.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      570 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/fo.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/fr.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      274 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ga.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      242 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/gb-eng.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    25061 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/gb-nir.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      231 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/gb-sct.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     9161 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/gb-wls.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      538 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/gb.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1681 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/gd.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1397 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ge.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/gf.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      595 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/gg.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      281 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/gh.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2938 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/gi.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      223 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/gl.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      546 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/gm.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      295 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/gn.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/gp.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     5182 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/gq.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1096 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/gr.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    34568 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/gs.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    37255 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/gt.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     4840 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/gu.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      813 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/gw.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      488 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/gy.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3494 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/hk.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1324 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/hm.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1112 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/hn.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    40615 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/hr.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    15005 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ht.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      274 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/hu.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      237 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/id.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ie.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      901 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/il.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     9870 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/im.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1074 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/in.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    27341 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/io.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1470 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/iq.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    15451 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ir.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      524 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/is.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/it.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     4700 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/je.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      389 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/jm.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      720 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/jo.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      474 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/jp.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1379 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ke.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3374 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/kg.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     7261 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/kh.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     5813 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ki.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1064 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/km.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      819 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/kn.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      795 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/kp.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1822 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/kr.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      509 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/kw.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    21724 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ky.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    11327 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/kz.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      457 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/la.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2816 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/lb.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      370 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/lc.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     8268 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/li.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    11242 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/lk.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      727 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/lr.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1219 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ls.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      442 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/lt.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      228 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/lu.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      233 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/lv.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      533 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ly.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      250 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ma.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      237 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/mc.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    11237 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/md.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    62373 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/me.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/mf.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      302 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/mg.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      741 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/mh.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      382 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/mk.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      276 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ml.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      848 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/mm.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1245 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/mn.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1461 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/mo.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    23398 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/mp.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/mq.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      442 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/mr.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     9279 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ms.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     8733 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/mt.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      319 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/mu.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      289 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/mv.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3652 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/mw.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    94979 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/mx.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1270 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/my.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2622 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/mz.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1005 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/na.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1380 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/nc.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      276 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ne.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     5837 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/nf.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      260 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ng.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    18408 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ni.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      224 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/nl.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      321 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/no.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1061 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/np.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      651 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/nr.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1745 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/nu.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2989 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/nz.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    22636 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/om.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      749 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/pa.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    73609 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/pe.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     4290 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/pf.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1661 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/pg.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1565 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ph.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      739 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/pk.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      222 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/pl.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/pm.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    10878 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/pn.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      637 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/pr.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      561 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ps.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     8280 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/pt.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      467 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/pw.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    17097 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/py.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      359 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/qa.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/re.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      305 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ro.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)   187134 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/rs.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      286 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ru.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      747 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/rw.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    10238 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/sa.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      953 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/sb.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      571 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/sc.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      497 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/sd.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      691 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/se.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      887 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/sg.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    29501 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/sh.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2053 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/si.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      321 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/sj.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1202 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/sk.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      275 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/sl.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    15801 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/sm.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      424 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/sn.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      497 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/so.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      315 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/sr.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      386 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ss.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      916 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/st.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    82697 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/sv.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    13209 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/sx.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      565 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/sy.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     6742 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/sz.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    14497 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/tc.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      267 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/td.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1088 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/tf.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      728 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/tg.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      287 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/th.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1812 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/tj.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      788 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/tk.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      603 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/tl.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    32287 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/tm.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      751 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/tn.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      355 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/to.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      554 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/tr.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      315 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/tt.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1783 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/tv.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      945 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/tw.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      549 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/tz.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      238 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ua.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3951 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ug.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     4523 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/um.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    19935 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/un.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     4461 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/us.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1718 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/uy.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1454 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/uz.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    91076 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/va.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      451 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/vc.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1168 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ve.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    24640 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/vg.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     8742 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/vi.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      494 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/vn.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3772 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/vu.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/wf.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      693 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ws.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     9643 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/xk.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      275 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ye.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      292 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/yt.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      859 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/za.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     5497 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/zm.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     6641 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/zw.svg
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.594876 djgentelella-0.3.9/djgentelella/static/vendors/font-awesome/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    21778 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/font-awesome/font-awesome.css.map
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    31000 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/font-awesome/font-awesome.min.css
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.594876 djgentelella-0.3.9/djgentelella/static/vendors/fonts/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)   134808 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/fonts/FontAwesome.otf
+-rw-r--r--   0 luisza    (1000) luisza    (1000)   165742 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 luisza    (1000) luisza    (1000)   444379 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)   165548 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    98024 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    77160 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    20127 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 luisza    (1000) luisza    (1000)   108738 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    45404 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    23424 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    18028 2023-01-17 16:40:29.000000 djgentelella-0.3.9/djgentelella/static/vendors/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.594876 djgentelella-0.3.9/djgentelella/static/vendors/fullcalendar/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    46228 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/fullcalendar/locales-all.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    25839 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/fullcalendar/main.min.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)   269560 2023-01-17 16:40:30.000000 djgentelella-0.3.9/djgentelella/static/vendors/fullcalendar/main.min.js
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.594876 djgentelella-0.3.9/djgentelella/static/vendors/grid-slider/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    11084 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/grid-slider/ion.rangeSlider.min.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    41171 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/grid-slider/ion.rangeSlider.min.js
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.598876 djgentelella-0.3.9/djgentelella/static/vendors/iCheck/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1302 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/iCheck/aero.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1302 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/iCheck/aero.png
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3021 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/iCheck/aero@2x.png
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1302 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/iCheck/blue.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1298 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/iCheck/blue.png
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3022 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/iCheck/blue@2x.png
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1317 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/iCheck/green.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1299 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/iCheck/green.png
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3022 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/iCheck/green@2x.png
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     4931 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/iCheck/icheck.min.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1332 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/iCheck/orange.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1299 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/iCheck/orange.png
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3022 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/iCheck/orange@2x.png
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1332 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/iCheck/yellow.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1303 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/iCheck/yellow.png
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3021 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/iCheck/yellow@2x.png
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.498875 djgentelella-0.3.9/djgentelella/static/vendors/img/
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.598876 djgentelella-0.3.9/djgentelella/static/vendors/img/bootstrap-colorpicker/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      557 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/img/bootstrap-colorpicker/alpha-horizontal.png
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      468 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/img/bootstrap-colorpicker/alpha.png
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      444 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/img/bootstrap-colorpicker/hue-horizontal.png
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      459 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/img/bootstrap-colorpicker/hue.png
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    52447 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/img/bootstrap-colorpicker/saturation-horizontal.png
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     4143 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/img/bootstrap-colorpicker/saturation.png
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.598876 djgentelella-0.3.9/djgentelella/static/vendors/inputmask/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    51226 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/inputmask/inputmask.min.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1662 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/inputmask/jquery.inputmask.min.js
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.598876 djgentelella-0.3.9/djgentelella/static/vendors/interact/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)   130770 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/interact/interact.min.js
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.598876 djgentelella-0.3.9/djgentelella/static/vendors/jquery/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    89664 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/jquery/jquery.min.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)   138161 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/jquery/jquery.min.map
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.598876 djgentelella-0.3.9/djgentelella/static/vendors/jquery-knob/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    10804 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/jquery-knob/jquery.knob.min.js
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.598876 djgentelella-0.3.9/djgentelella/static/vendors/jquery-ui/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    31340 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/jquery-ui/jquery-ui.min.css
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.598876 djgentelella-0.3.9/djgentelella/static/vendors/moment/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)   206984 2023-01-17 16:40:39.000000 djgentelella-0.3.9/djgentelella/static/vendors/moment/moment-with-locales.min.js
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.598876 djgentelella-0.3.9/djgentelella/static/vendors/nprogress/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1100 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/nprogress/nprogress.min.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     4114 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/nprogress/nprogress.min.js
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.602876 djgentelella-0.3.9/djgentelella/static/vendors/parsleyjs/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    40946 2023-01-17 16:40:39.000000 djgentelella-0.3.9/djgentelella/static/vendors/parsleyjs/parsley.min.js
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.602876 djgentelella-0.3.9/djgentelella/static/vendors/select2/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    31223 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/select2/select2-bootstrap-5-theme.min.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    16264 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/select2/select2.min.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    73163 2023-01-17 16:40:33.000000 djgentelella-0.3.9/djgentelella/static/vendors/select2/select2.min.js
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.602876 djgentelella-0.3.9/djgentelella/static/vendors/storylinejs/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    16975 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/storylinejs/storyline.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)  3283887 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/storylinejs/storyline.js
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.606876 djgentelella-0.3.9/djgentelella/static/vendors/storymapjs/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    89683 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/storymapjs/storymap.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)   255419 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/storymapjs/storymap.js
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.606876 djgentelella-0.3.9/djgentelella/static/vendors/summernote/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    30447 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/summernote/summernote-lite.min.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)   163197 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/summernote/summernote-lite.min.js
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.606876 djgentelella-0.3.9/djgentelella/static/vendors/sweetalert2/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    69578 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/sweetalert2/sweetalert2.all.min.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    24444 2023-01-17 16:40:36.000000 djgentelella-0.3.9/djgentelella/static/vendors/sweetalert2/sweetalert2.min.css
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.606876 djgentelella-0.3.9/djgentelella/static/vendors/switchery/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      682 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/switchery/switchery.min.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    24502 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/switchery/switchery.min.js
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.606876 djgentelella-0.3.9/djgentelella/static/vendors/tagify/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    45904 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/tagify/jQuery.tagify.min.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     9528 2023-01-17 16:40:35.000000 djgentelella-0.3.9/djgentelella/static/vendors/tagify/tagify.min.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    45259 2023-01-17 16:40:34.000000 djgentelella-0.3.9/djgentelella/static/vendors/tagify/tagify.min.js
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.498875 djgentelella-0.3.9/djgentelella/static/vendors/timeline/
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.606876 djgentelella-0.3.9/djgentelella/static/vendors/timeline/css/
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.610876 djgentelella-0.3.9/djgentelella/static/vendors/timeline/css/icons/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    13172 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/timeline/css/icons/tl-icons.eot
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    41332 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/timeline/css/icons/tl-icons.svg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    13008 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/timeline/css/icons/tl-icons.ttf
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    91644 2023-01-17 16:40:31.000000 djgentelella-0.3.9/djgentelella/static/vendors/timeline/css/timeline.css
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.610876 djgentelella-0.3.9/djgentelella/static/vendors/timeline/js/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)   207822 2023-01-17 16:40:32.000000 djgentelella-0.3.9/djgentelella/static/vendors/timeline/js/timeline.js
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.610876 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     6671 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/jquery.tinymce.min.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    60883 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skin.min.css
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.498875 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.498875 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/content/
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.610876 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/content/dark/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1469 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/content/dark/content.min.css
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.610876 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/content/default/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1399 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/content/default/content.min.css
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.610876 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/content/document/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1498 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/content/document/content.min.css
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.610876 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/content/writer/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1420 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/content/writer/content.min.css
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.498875 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/ui/
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.614876 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/ui/oxide/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    21708 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/ui/oxide/content.inline.min.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    21767 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/ui/oxide/content.min.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      544 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/ui/oxide/content.mobile.min.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    60882 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/ui/oxide/skin.min.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    21004 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/ui/oxide/skin.mobile.min.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      735 2023-01-17 16:40:28.000000 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/ui/oxide/skin.shadowdom.min.css
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.614876 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/ui/oxide-dark/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    21708 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/ui/oxide-dark/content.inline.min.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    21384 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/ui/oxide-dark/content.min.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      544 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/ui/oxide-dark/content.mobile.min.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    60766 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/ui/oxide-dark/skin.min.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    21004 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/ui/oxide-dark/skin.mobile.min.css
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      735 2023-01-17 16:40:38.000000 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/ui/oxide-dark/skin.shadowdom.min.css
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.498875 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/themes/
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.614876 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/themes/mobile/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)   171088 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/themes/mobile/theme.min.js
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.614876 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/themes/silver/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)   411481 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/themes/silver/theme.min.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)   736670 2023-01-17 16:40:27.000000 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/tinymce-all.js
+-rw-r--r--   0 luisza    (1000) luisza    (1000)   395541 2023-01-17 16:40:37.000000 djgentelella-0.3.9/djgentelella/static/vendors/tinymce/tinymce.min.js
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.502875 djgentelella-0.3.9/djgentelella/templates/
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.502875 djgentelella-0.3.9/djgentelella/templates/cruds/
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.614876 djgentelella-0.3.9/djgentelella/templates/cruds/ajax/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1639 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/cruds/ajax/_form.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      417 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/cruds/ajax/create.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1325 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/cruds/ajax/delete.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3219 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/cruds/ajax/list.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      412 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/cruds/ajax/update.html
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.614876 djgentelella-0.3.9/djgentelella/templates/gentelella/
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.614876 djgentelella-0.3.9/djgentelella/templates/gentelella/app/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      207 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/app/footer.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2755 2022-11-04 01:21:36.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/app/messages.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      668 2022-10-28 14:04:53.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/app/sidebar.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1407 2023-01-05 22:10:06.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/app/top_navigation.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    11367 2023-01-17 16:25:15.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/base.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       36 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/base_site.html
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.614876 djgentelella-0.3.9/djgentelella/templates/gentelella/blocks/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1229 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/blocks/box.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1497 2022-11-04 01:33:58.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/blocks/crud_list.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      312 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/blocks/helper_prototype.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2043 2022-11-03 23:12:02.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/blocks/permissions_management.html
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.618876 djgentelella-0.3.9/djgentelella/templates/gentelella/cruds/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      334 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/cruds/403.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      970 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/cruds/_form.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1221 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/cruds/create.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      195 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/cruds/crud_fields.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1803 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/cruds/delete.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2148 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/cruds/detail.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     6362 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/cruds/list.html
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.618876 djgentelella-0.3.9/djgentelella/templates/gentelella/cruds/pagination/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      337 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/cruds/pagination/enumeration.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      731 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/cruds/pagination/prev_next.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3862 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/cruds/update.html
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.618876 djgentelella-0.3.9/djgentelella/templates/gentelella/email/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       55 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/email/base.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      287 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/email/notification.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1065 2023-01-06 05:35:49.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/index.html
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.618876 djgentelella-0.3.9/djgentelella/templates/gentelella/menu/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1659 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/menu/notificacion.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2531 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/menu/notification_list.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1675 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/menu/palette.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2290 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/menu/palette_modal.html
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.618876 djgentelella-0.3.9/djgentelella/templates/gentelella/permission_management/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      549 2022-10-28 14:04:53.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/permission_management/permissionmanagement_list.html
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.622876 djgentelella-0.3.9/djgentelella/templates/gentelella/registration/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      410 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/registration/activate.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      434 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/registration/activation_complete.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      223 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/registration/activation_email.txt
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       67 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/registration/activation_email_subject.txt
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      886 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/registration/email_base.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/registration/email_footer.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/registration/email_header.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      209 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/registration/footer.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2195 2022-11-08 16:55:36.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/registration/login.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      694 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/registration/logout.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      693 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/registration/new_user.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      404 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/registration/password_change_done.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      524 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/registration/password_change_form.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      485 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/registration/password_reset_complete.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      679 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/registration/password_reset_confirm.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      634 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/registration/password_reset_done.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      618 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/registration/password_reset_email.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/registration/password_reset_email.txt
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1544 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/registration/password_reset_form.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      125 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/registration/password_reset_subject.txt
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      422 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/registration/registration_closed.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      433 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/registration/registration_complete.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      525 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/registration/registration_form.html
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.630876 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1480 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/addselect.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1413 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/addtreeselect.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      173 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/attrs.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      409 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/autocomplete_select.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      307 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/calendar.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      165 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/chart.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      109 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/chartjs.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       53 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/checkbox.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       53 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/checkbox_option.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       54 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/checkbox_select.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      103 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/checkyesno.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1517 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/chunkedupload.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      459 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/clearable_file_input.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      111 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/color_default.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      162 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/color_inline.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      389 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/color_style.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       93 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/credit_card_input_mask.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      258 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/custom_input.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       94 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/custom_input_mask.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      243 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/date.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       94 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/date_input_mask.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      242 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/daterange.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       97 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/daterangetime.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      201 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/datetime.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       94 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/datetime_input_mask.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       46 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/email.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       94 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/email_input_mask.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1337 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/file.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       46 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/hidden.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       94 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/identification_card_input_mask.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      187 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/input.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       94 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/input_mask.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      216 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/input_option.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       52 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/multiple_hidden.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      461 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/multiple_input.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      116 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/multiwidget.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       45 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/number.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      161 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/number_knob_input.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       45 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/password.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       94 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/phone_number_input_mask.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      630 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/radio.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      216 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/radio_input_option.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       52 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/radio_option.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       54 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/radio_select.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      554 2023-01-07 00:00:42.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/record_audio.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      722 2023-01-06 03:44:55.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/record_photo.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      647 2023-01-07 00:12:07.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/record_video.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      383 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/select.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       52 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/select_date.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      124 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/select_option.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       94 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/serial_number_input_mask.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       51 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/splitdatetime.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       52 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/splithiddendatetime.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       58 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/storyline.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      122 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/storymap_gigapixel.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      101 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/storymap_mapbased.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       46 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/tagging.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       94 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/taxid_input_mask.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       46 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/text.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      143 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/textarea.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      200 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/time.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       82 2022-10-28 05:40:35.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/timeline.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      387 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/tree_select.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      211 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/tree_select_option.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       45 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/url.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      249 2022-10-28 14:04:53.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/wysiwyg.html
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       48 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/wysiwygtwo.html
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.630876 djgentelella-0.3.9/djgentelella/templatetags/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/templatetags/__init__.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1855 2022-12-21 20:53:40.000000 djgentelella-0.3.9/djgentelella/templatetags/_utils.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     6328 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/templatetags/crud_tags.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     7675 2022-12-21 21:47:19.000000 djgentelella-0.3.9/djgentelella/templatetags/gentelellamenu.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1440 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/templatetags/gtsettings.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      476 2022-12-21 20:53:40.000000 djgentelella-0.3.9/djgentelella/templatetags/timejs.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       59 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/templatetags/tree_tags.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1945 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/templatetags/urlname_tags.py
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.630876 djgentelella-0.3.9/djgentelella/tests/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     5219 2022-12-21 20:53:40.000000 djgentelella-0.3.9/djgentelella/tests/Calendar_Test.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     8523 2022-12-21 20:53:40.000000 djgentelella-0.3.9/djgentelella/tests/StoryLine_Test.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     4031 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/tests/StoryMap_Test.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3540 2022-12-21 20:53:40.000000 djgentelella-0.3.9/djgentelella/tests/TimeLine_Test.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      117 2022-12-21 20:53:40.000000 djgentelella-0.3.9/djgentelella/tests/__init__.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     4246 2023-01-17 16:25:15.000000 djgentelella-0.3.9/djgentelella/urls.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      825 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/utils.py
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.630876 djgentelella-0.3.9/djgentelella/views/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/views/__init__.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       97 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/views/auth.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     4415 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/views/select2autocomplete.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2793 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/views/storyline.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1025 2022-12-21 20:53:40.000000 djgentelella-0.3.9/djgentelella/views/storymap.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      786 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/views/timeline.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-12-21 21:30:55.000000 djgentelella-0.3.9/djgentelella/views/upload.py
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.630876 djgentelella-0.3.9/djgentelella/widgets/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/widgets/__init__.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1459 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/widgets/calendar.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1895 2022-12-21 21:43:38.000000 djgentelella-0.3.9/djgentelella/widgets/color.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    20838 2023-01-17 16:25:15.000000 djgentelella-0.3.9/djgentelella/widgets/core.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1348 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/widgets/files.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      826 2022-12-21 20:53:40.000000 djgentelella-0.3.9/djgentelella/widgets/helper.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      407 2022-12-21 20:53:40.000000 djgentelella-0.3.9/djgentelella/widgets/numberknobinput.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     3191 2023-01-05 16:23:19.000000 djgentelella-0.3.9/djgentelella/widgets/selects.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1155 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/widgets/storyline.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2350 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/widgets/storymap.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1110 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/widgets/tagging.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1204 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/widgets/timeline.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      607 2022-12-21 20:53:41.000000 djgentelella-0.3.9/djgentelella/widgets/tinymce.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     2212 2022-12-21 20:53:40.000000 djgentelella-0.3.9/djgentelella/widgets/trees.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      609 2022-12-21 20:53:40.000000 djgentelella-0.3.9/djgentelella/widgets/wysiwyg.py
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.630876 djgentelella-0.3.9/djgentelella/wysiwyg/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)        0 2022-09-27 22:26:00.000000 djgentelella-0.3.9/djgentelella/wysiwyg/__init__.py
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1159 2022-12-21 21:31:09.000000 djgentelella-0.3.9/djgentelella/wysiwyg/views.py
+drwxr-xr-x   0 luisza    (1000) luisza    (1000)        0 2023-01-17 16:40:40.502875 djgentelella-0.3.9/djgentelella.egg-info/
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     4911 2023-01-17 16:40:40.000000 djgentelella-0.3.9/djgentelella.egg-info/PKG-INFO
+-rw-r--r--   0 luisza    (1000) luisza    (1000)    45450 2023-01-17 16:40:40.000000 djgentelella-0.3.9/djgentelella.egg-info/SOURCES.txt
+-rw-r--r--   0 luisza    (1000) luisza    (1000)        1 2023-01-17 16:40:40.000000 djgentelella-0.3.9/djgentelella.egg-info/dependency_links.txt
+-rw-r--r--   0 luisza    (1000) luisza    (1000)        1 2023-01-17 16:40:40.000000 djgentelella-0.3.9/djgentelella.egg-info/not-zip-safe
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      141 2023-01-17 16:40:40.000000 djgentelella-0.3.9/djgentelella.egg-info/requires.txt
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       13 2023-01-17 16:40:40.000000 djgentelella-0.3.9/djgentelella.egg-info/top_level.txt
+-rw-r--r--   0 luisza    (1000) luisza    (1000)      148 2022-10-28 14:04:53.000000 djgentelella-0.3.9/requirements.txt
+-rw-r--r--   0 luisza    (1000) luisza    (1000)       38 2023-01-17 16:40:40.634876 djgentelella-0.3.9/setup.cfg
+-rw-r--r--   0 luisza    (1000) luisza    (1000)     1605 2023-01-17 16:25:15.000000 djgentelella-0.3.9/setup.py
```

### Comparing `djgentelella-0.3.8/LICENSE` & `djgentelella-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/PKG-INFO` & `djgentelella-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: djgentelella
-Version: 0.3.8
+Version: 0.3.9
 Summary: Extra widgets for django using gentelella.
 Home-page: https://solvosoft.com
 Author: Luis Zarate Montero
 Author-email: luis.zarate@solvosoft.com
 License: GNU General Public License
 Description: Django Gentelella widgets
         ############################
```

### Comparing `djgentelella-0.3.8/Readme.rst` & `djgentelella-0.3.9/Readme.rst`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/admin.py` & `djgentelella-0.3.9/djgentelella/admin.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/blog/forms.py` & `djgentelella-0.3.9/djgentelella/blog/forms.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/blog/migrations/0001_initial.py` & `djgentelella-0.3.9/djgentelella/blog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/blog/models.py` & `djgentelella-0.3.9/djgentelella/blog/models.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/blog/static/images/article.png` & `djgentelella-0.3.9/djgentelella/blog/static/images/article.png`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/blog/templates/gentelella/blog/entry_delete.html` & `djgentelella-0.3.9/djgentelella/blog/templates/gentelella/blog/entry_delete.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/blog/templates/gentelella/blog/entry_detail.html` & `djgentelella-0.3.9/djgentelella/blog/templates/gentelella/blog/entry_detail.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/blog/templates/gentelella/blog/entry_form.html` & `djgentelella-0.3.9/djgentelella/blog/templates/gentelella/blog/entry_form.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/blog/templates/gentelella/blog/entry_list.html` & `djgentelella-0.3.9/djgentelella/blog/templates/gentelella/blog/entry_list.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/blog/templatetags/blog_tags.py` & `djgentelella-0.3.9/djgentelella/blog/templatetags/blog_tags.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/blog/tests/test_entry_detail.py` & `djgentelella-0.3.9/djgentelella/blog/tests/test_entry_detail.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/blog/tests/test_entry_forms.py` & `djgentelella-0.3.9/djgentelella/blog/tests/test_entry_forms.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/blog/tests/test_entry_listing.py` & `djgentelella-0.3.9/djgentelella/blog/tests/test_entry_listing.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/blog/tests/test_models.py` & `djgentelella-0.3.9/djgentelella/blog/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/blog/tests/test_sitemaps.py` & `djgentelella-0.3.9/djgentelella/blog/tests/test_sitemaps.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/blog/tests/test_templatetags.py` & `djgentelella-0.3.9/djgentelella/blog/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/blog/urls.py` & `djgentelella-0.3.9/djgentelella/blog/urls.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/blog/views.py` & `djgentelella-0.3.9/djgentelella/blog/views.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/chartjs.py` & `djgentelella-0.3.9/djgentelella/chartjs.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/chunked_upload/models.py` & `djgentelella-0.3.9/djgentelella/chunked_upload/models.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/chunked_upload/views.py` & `djgentelella-0.3.9/djgentelella/chunked_upload/views.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/cruds/base.py` & `djgentelella-0.3.9/djgentelella/cruds/base.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/cruds/filter.py` & `djgentelella-0.3.9/djgentelella/cruds/filter.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/cruds/inline_crud.py` & `djgentelella-0.3.9/djgentelella/cruds/inline_crud.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/cruds/utils.py` & `djgentelella-0.3.9/djgentelella/cruds/utils.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/elements.py` & `djgentelella-0.3.9/djgentelella/elements.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/fields/catalog.py` & `djgentelella-0.3.9/djgentelella/fields/catalog.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/fields/drfdatetime.py` & `djgentelella-0.3.9/djgentelella/fields/drfdatetime.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/fields/tree.py` & `djgentelella-0.3.9/djgentelella/fields/tree.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/forms/decorators.py` & `djgentelella-0.3.9/djgentelella/forms/decorators.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/forms/forms.py` & `djgentelella-0.3.9/djgentelella/forms/forms.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/locale/es/LC_MESSAGES/django.mo` & `djgentelella-0.3.9/djgentelella/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/locale/es/LC_MESSAGES/django.po` & `djgentelella-0.3.9/djgentelella/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/management/commands/createbasejs.py` & `djgentelella-0.3.9/djgentelella/management/commands/createbasejs.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,16 @@
             'booleanFields.js',
             'editorTinymce.js',
             'wysiwyg.js',
             'gigapixel_storymap.js',
             'mapbased_storymap.js',
             'storyline.js',
             'calendar.js',
-            'timeline.js'
+            'timeline.js',
+            'mediarecord.js'
         ]
         jquery_plugins = [
             'notifications.js',
             'chart.js',
             'custom.widgets.js',
             'fileupload.widget.js',
             'select2related.js',
```

### Comparing `djgentelella-0.3.8/djgentelella/management/commands/delete_expired_uploads.py` & `djgentelella-0.3.9/djgentelella/management/commands/delete_expired_uploads.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/management/commands/loaddevstatic.py` & `djgentelella-0.3.9/djgentelella/management/commands/loaddevstatic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 import os
 import shutil
 from pathlib import Path
+from threading import Thread, current_thread
 
 from django.contrib.staticfiles import finders
 from django.core.management import BaseCommand
 
+try:
+    import requests
+except BaseException:
+    print("Requests is required try pip install requests")
+    exit(1)
+
 FLAGS = ['ad', 'ae', 'af', 'ag', 'ai', 'al', 'am', 'ao', 'aq', 'ar', 'as', 'at', 'au',
          'aw', 'ax', 'az', 'ba', 'bb', 'bd', 'be', 'bf', 'bg', 'bh', 'bi', 'bj', 'bl',
          'bm', 'bn', 'bo', 'bq', 'br', 'bs', 'bt', 'bv', 'bw', 'by', 'bz', 'ca', 'cc',
          'cd', 'cf', 'cg', 'ch', 'ci', 'ck', 'cl', 'cm', 'cn', 'co', 'cr', 'cu', 'cv',
          'cw', 'cx', 'cy', 'cz', 'de', 'dj', 'dk', 'dm', 'do', 'dz', 'ec', 'ee', 'eg',
          'eh', 'er', 'es-ca', 'es', 'et', 'eu', 'fi', 'fj', 'fk', 'fm', 'fo', 'fr',
          'ga', 'gb-eng', 'gb-nir', 'gb-sct', 'gb-wls', 'gb', 'gd', 'ge', 'gf', 'gg',
@@ -24,48 +31,84 @@
          'sh', 'si', 'sj', 'sk', 'sl', 'sm', 'sn', 'so', 'sr', 'ss', 'st', 'sv', 'sx',
          'sy', 'sz', 'tc', 'td', 'tf', 'tg', 'th', 'tj', 'tk', 'tl', 'tm', 'tn', 'to',
          'tr', 'tt', 'tv', 'tw', 'tz', 'ua', 'ug', 'um', 'un', 'us', 'uy', 'uz', 'va',
          'vc', 've', 'vg', 'vi', 'vn', 'vu', 'wf', 'ws', 'xk', 'ye', 'yt', 'za', 'zm',
          'zw']
 
 
+def download(urls):
+    thread = current_thread()
+    for url in urls:
+        download_url = url[0]
+        filename = url[1]
+        print("%s) Downloading %s --> %s" % (thread.name, download_url, filename))
+        r = requests.get(download_url)
+        with open(filename, 'wb') as arch:
+            arch.write(r.content)
+
+
 class Command(BaseCommand):
     help = "Load static files for development command"
+    urls = []
+    threads_count = 10
+
+    def get_urls_list(self, urls):
+        if self.threads_count == 1:
+            yield urls[:]
+            return
+
+        trunk_len = len(urls) // self.threads_count
+        start = 0
+        nextt = trunk_len
+        end = len(urls)
+        while nextt != end:
+            yield urls[start:nextt]
+            start = nextt
+            nextt += trunk_len
+            if nextt > end:
+                yield urls[start:]
+                nextt = end
+
+    def download_urls(self):
+        threads = []
+        for urls_trunk in self.get_urls_list(self.urls):
+            t = Thread(target=download, args=[urls_trunk])
+            t.start()
+            threads.append(t)
 
-    def get_static_file(self, requests, url, basepath):
+        for t in threads:
+            t.join()
+
+    def get_static_file(self, url, basepath):
         name = url.split('/')[-1]
         if not os.path.exists(basepath / name):
-            print("Downloading %s --> %s" % (url, basepath / name))
-            r = requests.get(url)
-            with open(basepath / name, 'wb') as arch:
-                arch.write(r.content)
+            self.urls.append(
+                (url, basepath / name)
+            )
 
-    def get_static_list_file(self, requests, files, basepath):
+    def get_static_list_file(self, files, basepath):
         if not os.path.exists(basepath):
             print("Downloading %s " % (basepath,))
             with open(basepath, 'wb') as arch:
                 for url in files:
                     r = requests.get(url)
                     arch.write(r.content)
                     arch.write(b'\n')
 
     def add_arguments(self, parser):
         parser.add_argument(
             '--delete',
             action='store_true',
             help='Delete delete before start',
         )
+        parser.add_argument('--threads', type=int, default=10,
+                            help='Number of downloading threads')
 
     def handle(self, *args, **options):
-        try:
-            import requests
-        except BaseException:
-            print("Requests is required try pip install requests")
-            exit(1)
-
+        self.threads_count = options['threads']
         result = finders.find(Path('gentelella/css/custom.css'))
         if result is None:
             print('No static folder found')
             exit(1)
 
         basepath = Path(result.replace(
             str(Path('gentelella/css/custom.css')), 'vendors/'))
@@ -382,15 +425,16 @@
         if not os.path.exists(basepath / 'flags'):
             (basepath / 'flags').mkdir(parents=True)
         for lib in libs:
             currentbasepath = basepath / lib
             if not os.path.exists(currentbasepath):
                 os.makedirs(currentbasepath)
             for staticfile in libs[lib]:
-                self.get_static_file(requests, staticfile, currentbasepath)
+                self.get_static_file(staticfile, currentbasepath)
 
         for files in compressed:
             for name in compressed[files]:
                 currentbasepath = basepath / files
                 currentbasepath = currentbasepath / name
-                self.get_static_list_file(requests, compressed[files][name],
+                self.get_static_list_file(compressed[files][name],
                                           currentbasepath)
+        self.download_urls()
```

### Comparing `djgentelella-0.3.8/djgentelella/menu_widgets/palette.py` & `djgentelella-0.3.9/djgentelella/menu_widgets/palette.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/migrations/0001_initial.py` & `djgentelella-0.3.9/djgentelella/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/migrations/0001_squashed_new_initial.py` & `djgentelella-0.3.9/djgentelella/migrations/0001_squashed_new_initial.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/migrations/0002_auto_20200214_2038.py` & `djgentelella-0.3.9/djgentelella/migrations/0002_auto_20200214_2038.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/migrations/0003_help.py` & `djgentelella-0.3.9/djgentelella/migrations/0003_help.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/migrations/0004_loadsettings.py` & `djgentelella-0.3.9/djgentelella/migrations/0004_loadsettings.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/migrations/0005_notification.py` & `djgentelella-0.3.9/djgentelella/migrations/0005_notification.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/migrations/0006_permissionscategorymanagement.py` & `djgentelella-0.3.9/djgentelella/migrations/0006_permissionscategorymanagement.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/migrations/0007_edit_footer.py` & `djgentelella-0.3.9/djgentelella/migrations/0007_edit_footer.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/migrations/0009_chunkedupload.py` & `djgentelella-0.3.9/djgentelella/migrations/0009_chunkedupload.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/migrations/0010_menuitem_position.py` & `djgentelella-0.3.9/djgentelella/migrations/0010_menuitem_position.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/migrations/0011_remove_menuitem_level_remove_menuitem_lft_and_more.py` & `djgentelella-0.3.9/djgentelella/migrations/0011_remove_menuitem_level_remove_menuitem_lft_and_more.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/models.py` & `djgentelella-0.3.9/djgentelella/models.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/notification/__init__.py` & `djgentelella-0.3.9/djgentelella/notification/__init__.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/notification/base.py` & `djgentelella-0.3.9/djgentelella/notification/base.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/notification/serializer.py` & `djgentelella-0.3.9/djgentelella/notification/serializer.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/notification/widgets.py` & `djgentelella-0.3.9/djgentelella/notification/widgets.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/permission_management/forms.py` & `djgentelella-0.3.9/djgentelella/permission_management/forms.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/permission_management/objinterface.py` & `djgentelella-0.3.9/djgentelella/permission_management/objinterface.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/serializers/calendar.py` & `djgentelella-0.3.9/djgentelella/serializers/calendar.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/serializers/storyline.py` & `djgentelella-0.3.9/djgentelella/serializers/storyline.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/serializers/storymap.py` & `djgentelella-0.3.9/djgentelella/serializers/storymap.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/serializers/timeline.py` & `djgentelella-0.3.9/djgentelella/serializers/timeline.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/settings.py` & `djgentelella-0.3.9/djgentelella/settings.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/django_ajax/js/jquery.ajax-plugin.js` & `djgentelella-0.3.9/djgentelella/static/django_ajax/js/jquery.ajax-plugin.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/django_ajax/js/jquery.ajax-plugin.min.js` & `djgentelella-0.3.9/djgentelella/static/django_ajax/js/jquery.ajax-plugin.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/django_ajax/js/jquery.ajax.js` & `djgentelella-0.3.9/djgentelella/static/django_ajax/js/jquery.ajax.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/django_ajax/js/jquery.ajax.min.js` & `djgentelella-0.3.9/djgentelella/static/django_ajax/js/jquery.ajax.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/gentelella/css/custom.css` & `djgentelella-0.3.9/djgentelella/static/gentelella/css/custom.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/gentelella/css/modern.css` & `djgentelella-0.3.9/djgentelella/static/gentelella/css/modern.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/gentelella/css/modern_black_white.css` & `djgentelella-0.3.9/djgentelella/static/gentelella/css/modern_black_white.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/gentelella/css/style_black_and_white.css` & `djgentelella-0.3.9/djgentelella/static/gentelella/css/style_black_and_white.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/gentelella/images/back_disabled.png` & `djgentelella-0.3.9/djgentelella/static/gentelella/images/back_disabled.png`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/gentelella/images/back_enabled.png` & `djgentelella-0.3.9/djgentelella/static/gentelella/images/back_enabled.png`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/gentelella/images/back_enabled_hover.png` & `djgentelella-0.3.9/djgentelella/static/gentelella/images/back_enabled_hover.png`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/gentelella/images/forward_disabled.png` & `djgentelella-0.3.9/djgentelella/static/gentelella/images/forward_disabled.png`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/gentelella/images/forward_enabled.png` & `djgentelella-0.3.9/djgentelella/static/gentelella/images/forward_enabled.png`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/gentelella/images/forward_enabled_hover.png` & `djgentelella-0.3.9/djgentelella/static/gentelella/images/forward_enabled_hover.png`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/gentelella/images/loading.gif` & `djgentelella-0.3.9/djgentelella/static/gentelella/images/loading.gif`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/gentelella/js/base/autocompleteSelect2.js` & `djgentelella-0.3.9/djgentelella/static/gentelella/js/base/autocompleteSelect2.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/gentelella/js/base/booleanFields.js` & `djgentelella-0.3.9/djgentelella/static/gentelella/js/base/booleanFields.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/gentelella/js/base/calendar.js` & `djgentelella-0.3.9/djgentelella/static/gentelella/js/base/calendar.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/gentelella/js/base/chart.js` & `djgentelella-0.3.9/djgentelella/static/gentelella/js/base/chart.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/gentelella/js/base/custom.widgets.js` & `djgentelella-0.3.9/djgentelella/static/gentelella/js/base/custom.widgets.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/gentelella/js/base/dateranges_gridslider.js` & `djgentelella-0.3.9/djgentelella/static/gentelella/js/base/dateranges_gridslider.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/gentelella/js/base/editorTinymce.js` & `djgentelella-0.3.9/djgentelella/static/gentelella/js/base/editorTinymce.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/gentelella/js/base/fileupload.widget.js` & `djgentelella-0.3.9/djgentelella/static/gentelella/js/base/fileupload.widget.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/gentelella/js/base/formset.js` & `djgentelella-0.3.9/djgentelella/static/gentelella/js/base/formset.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/gentelella/js/base/gigapixel_storymap.js` & `djgentelella-0.3.9/djgentelella/static/gentelella/js/base/gigapixel_storymap.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/gentelella/js/base/helper_widget.js` & `djgentelella-0.3.9/djgentelella/static/gentelella/js/base/helper_widget.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/gentelella/js/base/mapbased_storymap.js` & `djgentelella-0.3.9/djgentelella/static/gentelella/js/base/mapbased_storymap.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/gentelella/js/base/notifications.js` & `djgentelella-0.3.9/djgentelella/static/gentelella/js/base/notifications.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/gentelella/js/base/select2related.js` & `djgentelella-0.3.9/djgentelella/static/gentelella/js/base/select2related.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/gentelella/js/base/storyline.js` & `djgentelella-0.3.9/djgentelella/static/gentelella/js/base/storyline.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/gentelella/js/base/timeline.js` & `djgentelella-0.3.9/djgentelella/static/gentelella/js/base/timeline.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/gentelella/js/base.js` & `djgentelella-0.3.9/djgentelella/static/gentelella/js/base.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1518,8 +1518,382 @@
         timeline = new TL.Timeline(instanceid, instance.data('url'), options);
         window.addEventListener('resize', function() {
             var embed = document.getElementById(instanceid);
             embed.style.height = getComputedStyle(document.body).height;
             timeline.updateDisplay();
         })
     });
+}
+
+function show_errors_media_record(error) {
+    Swal.fire({
+        icon: 'error',
+        title: 'Sorry, there is a problem',
+        text: 'Media device is not available',
+    })
+}
+
+function getPhotoRecord(element) {
+    let id = element.id
+    let media = {
+        tag: 'video',
+        type: 'image/png',
+        ext: '.png',
+        gUM: {
+            video: true
+        }
+    }
+
+    let v = {
+        id: id,
+        canvas: $("#" + id + "_canvas"),
+        video: $("#" + id + "_video"),
+        btn_control: $("#" + id + "_btn"),
+        btn_cancel: $("#" + id + "_cancel"),
+        width: $("#" + id).data('width') || '320px',
+        height: $("#" + id).data('height') || '240px',
+        recorder: null,
+        media: media,
+        status: 0,
+        initialize: function() {
+            this.btn_control.on('click', this.callClick(this));
+            this.btn_cancel.on('click', this.callCancel(this));
+            this.btn_cancel.hide();
+            this.canvas.hide();
+            this.video.hide();
+            this.canvas[0].style.width = this.width;
+            this.canvas[0].style.height = this.height;
+            this.video[0].style.width = this.width;
+            this.video[0].style.height = this.height;
+            $(window).on('cancelMedia', this.callCancel(this, trigger = true));
+
+        },
+        clickEvent: function() {
+            var video = this.video[0];
+            var parent = this;
+            if (this.status == 0) {
+                navigator.mediaDevices.getUserMedia(this.media.gUM).then(_stream => {
+                    video.srcObject = _stream;
+                    parent.tracks = _stream.getTracks();
+                }).catch(show_errors_media_record);
+                this.video.show();
+                this.canvas.hide();
+            } else if (this.status == 1) {
+                let canvas = this.canvas[0];
+                this.video.hide();
+                canvas.getContext('2d').drawImage(this.video[0], 0, 0, canvas.width, canvas.height);
+                this.canvas.show();
+            } else {
+                this.status = -1;
+                this.save_media();
+                if (this.tracks) this.tracks.forEach(track => track.stop());
+            }
+            this.status = this.status + 1;
+            this.presentbutton();
+        },
+        presentbutton: function() {
+            if (this.status == 0) {
+                this.btn_cancel.hide();
+                $("#" + this.id + "_btn i").attr('class', 'fa fa-video-camera');
+                $("#" + this.id + "_btn span").text('Start');
+            } else {
+                this.btn_cancel.show();
+            }
+            if (this.status == 1) {
+                $("#" + this.id + "_btn i").attr('class', 'fa fa-camera');
+                $("#" + this.id + "_btn span").text('Capture');
+            }
+            if (this.status == 2) {
+                $("#" + this.id + "_btn i").attr('class', 'fa fa-check');
+                $("#" + this.id + "_btn span").text('Save');
+            }
+        },
+        cancel: function(trigger) {
+            this.status = 0;
+            if (this.recorder != null) this.recorder.stop();
+            if (this.tracks) this.tracks.forEach(track => track.stop());
+            this.btn_cancel.hide();
+            this.canvas.hide();
+            this.video.hide();
+            this.presentbutton();
+            if (!trigger) $(window).trigger('cancelMedia');
+
+        },
+
+        callCancel: function(instance, trigger = false) {
+            return () => {
+                instance.cancel(trigger)
+            };
+        },
+        callClick: function(instance) {
+            return () => {
+                instance.clickEvent()
+            };
+        },
+        save_media: function() {
+            var parent = this;
+            this.canvas[0].toBlob((blob) => {
+                let file = new File([blob], "photo" + parent.media.ext, {
+                    type: parent.media.type
+                })
+                let container = new DataTransfer();
+                container.items.add(file);
+                $("#" + parent.id)[0].files = container.files;
+            }, parent.media.type);
+        }
+    }
+
+    v.initialize()
+    return v;
+}
+
+
+function getVideoRecord(element) {
+    let id = element.id
+    let media = {
+        tag: 'video',
+        type: 'video/webm',
+        ext: '.mp4',
+        gUM: {
+            video: true,
+            audio: true
+        }
+    }
+    let v = {
+        id: id,
+        canvas: $("#" + id + "_canvas"),
+        video: $("#" + id + "_video"),
+        btn_control: $("#" + id + "_btn"),
+        btn_cancel: $("#" + id + "_cancel"),
+        width: $("#" + id).data('width') || '320px',
+        height: $("#" + id).data('height') || '240px',
+        chunks: [],
+        recorder: null,
+        media: media,
+        status: 0,
+        initialize: function() {
+            this.btn_control.on('click', this.callClick(this));
+            this.btn_cancel.on('click', this.callCancel(this));
+            this.btn_cancel.hide();
+            this.video[0].style.width = this.width;
+            this.video[0].style.height = this.height;
+            this.video.hide();
+            $(window).on('cancelMedia', this.callCancel(this, trigger = true));
+
+        },
+        clickEvent: function() {
+            var video = this.video[0];
+            var parent = this;
+            if (this.status == 0) {
+                navigator.mediaDevices.getUserMedia(this.media.gUM).then(_stream => {
+                    video.srcObject = _stream;
+                    parent.tracks = _stream.getTracks();
+                    parent.recorder = new MediaRecorder(_stream);
+                    parent.recorder.ondataavailable = e => {
+                        parent.chunks.push(e.data);
+                        if (parent.recorder.state == 'inactive') parent.save_media();
+                    };
+                }).catch(show_errors_media_record);
+                this.video.show();
+
+            } else if (this.status == 1) {
+                this.chunks = [];
+                if (this.recorder) this.recorder.start();
+            } else {
+                if (this.recorder != null && this.recorder.state == 'inactive') this.recorder.stop();
+                this.cancel(true)
+                this.status = -1;
+            }
+            this.status = this.status + 1;
+            this.presentbutton();
+        },
+        presentbutton: function() {
+            if (this.status == 0) {
+                this.btn_cancel.hide();
+                $("#" + this.id + "_btn i").attr('class', 'fa fa-video-camera');
+                $("#" + this.id + "_btn span").text('Start');
+
+            } else {
+                this.btn_cancel.show();
+            }
+            if (this.status == 1) {
+                $("#" + this.id + "_btn i").attr('class', 'fa fa-play');
+                $("#" + this.id + "_btn span").text('Record');
+                $("#" + this.id + "_container .mediareproductor").remove();
+            }
+            if (this.status == 2) {
+                $("#" + this.id + "_btn i").attr('class', 'fa fa-pause');
+                $("#" + this.id + "_btn span").text('Recording...');
+            }
+        },
+        cancel: function(trigger) {
+            this.status = 0;
+            if (this.recorder != null && this.recorder.state != 'inactive') this.recorder.stop();
+            if (this.tracks) this.tracks.forEach(track => track.stop());
+            this.btn_cancel.hide();
+            this.video.hide();
+            this.presentbutton();
+            if (!trigger) $(window).trigger('cancelMedia');
+
+        },
+
+        callCancel: function(instance, trigger = false) {
+            return () => {
+                instance.cancel(trigger)
+            };
+        },
+        callClick: function(instance) {
+            return () => {
+                instance.clickEvent()
+            };
+        },
+        save_media: function() {
+            let file = new File(this.chunks, "record" + this.media.ext, {
+                type: this.media.type,
+                lastModified: new Date().getTime()
+            });
+            let container = new DataTransfer();
+            container.items.add(file);
+            $("#" + this.id)[0].files = container.files;
+            let blob = new Blob(this.chunks, {
+                type: this.media.type
+            })
+            let url = URL.createObjectURL(blob)
+            mt = document.createElement(this.media.tag)
+            mt.controls = true;
+            mt.src = url;
+            mt.className = "mediareproductor"
+            mt.style.width = this.width;
+            mt.style.height = this.height;
+            $("#" + this.id + "_container").append(mt);
+        }
+    }
+
+    v.initialize()
+    return v;
+}
+
+
+function getAudioRecord(element) {
+    let id = element.id
+    let media = {
+        tag: 'audio',
+        type: 'audio/ogg',
+        ext: '.ogg',
+        gUM: {
+            video: false,
+            audio: true
+        }
+    }
+    let v = {
+        id: id,
+        canvas: $("#" + id + "_canvas"),
+        btn_control: $("#" + id + "_btn"),
+        btn_cancel: $("#" + id + "_cancel"),
+        chunks: [],
+        recorder: null,
+        media: media,
+        status: 0,
+        initialize: function() {
+            this.btn_control.on('click', this.callClick(this));
+            this.btn_cancel.on('click', this.callCancel(this));
+            this.btn_cancel.hide();
+            $(window).on('cancelMedia', this.callCancel(this, trigger = true));
+
+        },
+        clickEvent: function() {
+            var parent = this;
+            if (this.status == 0) {
+                navigator.mediaDevices.getUserMedia(this.media.gUM).then(_stream => {
+                    parent.tracks = _stream.getTracks();
+                    parent.recorder = new MediaRecorder(_stream);
+                    parent.recorder.ondataavailable = e => {
+                        parent.chunks.push(e.data);
+                        if (parent.recorder.state == 'inactive') parent.save_media();
+                    };
+                }).catch(show_errors_media_record);
+            } else if (this.status == 1) {
+                this.chunks = [];
+                if (this.recorder) this.recorder.start();
+            } else {
+                if (this.recorder != null && this.recorder.state == 'inactive') this.recorder.stop();
+                this.cancel(true)
+                this.status = -1;
+            }
+            this.status = this.status + 1;
+            this.presentbutton();
+        },
+        presentbutton: function() {
+            if (this.status == 0) {
+                this.btn_cancel.hide();
+                $("#" + this.id + "_btn i").attr('class', 'fa fa-video-camera');
+                $("#" + this.id + "_btn span").text('Start');
+                $("#" + this.id + "_container .mediareproductor").remove();
+            } else {
+                this.btn_cancel.show();
+            }
+            if (this.status == 1) {
+                $("#" + this.id + "_btn i").attr('class', 'fa fa-play');
+                $("#" + this.id + "_btn span").text('Record');
+            }
+            if (this.status == 2) {
+                $("#" + this.id + "_btn i").attr('class', 'fa fa-pause');
+                $("#" + this.id + "_btn span").text('Recording...');
+            }
+        },
+        cancel: function(trigger) {
+            this.status = 0;
+            if (this.recorder != null && this.recorder.state == 'inactive') this.recorder.stop();
+            if (this.tracks) this.tracks.forEach(track => track.stop());
+            this.btn_cancel.hide();
+            this.presentbutton();
+            if (!trigger) $(window).trigger('cancelMedia');
+
+        },
+
+        callCancel: function(instance, trigger = false) {
+            return () => {
+                instance.cancel(trigger)
+            };
+        },
+        callClick: function(instance) {
+            return () => {
+                instance.clickEvent()
+            };
+        },
+        save_media: function() {
+            let file = new File(this.chunks, "record" + this.media.ext, {
+                type: this.media.type,
+                lastModified: new Date().getTime()
+            });
+            let container = new DataTransfer();
+            container.items.add(file);
+            $("#" + this.id)[0].files = container.files;
+            let blob = new Blob(this.chunks, {
+                type: this.media.type
+            })
+            let url = URL.createObjectURL(blob)
+            mt = document.createElement(this.media.tag)
+            mt.controls = true;
+            mt.src = url;
+            mt.className = "mediareproductor"
+            $("#" + this.id + "_container").append(mt);
+        }
+    }
+
+    v.initialize()
+    return v;
+}
+
+
+
+function getMediaRecord(element, mediatype) {
+    if (mediatype == 'photo') {
+        return getPhotoRecord(element);
+    }
+    if (mediatype == 'video') {
+        return getVideoRecord(element);
+    }
+    if (mediatype === "audio") {
+        return getAudioRecord(element)
+    }
 }
```

### Comparing `djgentelella-0.3.8/djgentelella/static/gentelella/js/custom.js` & `djgentelella-0.3.9/djgentelella/static/gentelella/js/custom.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/gentelella/js/datatables.js` & `djgentelella-0.3.9/djgentelella/static/gentelella/js/datatables.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/gentelella/js/gentelella-bundle.js` & `djgentelella-0.3.9/djgentelella/static/gentelella/js/gentelella-bundle.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/gentelella/js/permissionmanagement.js` & `djgentelella-0.3.9/djgentelella/static/gentelella/js/permissionmanagement.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/gentelella/js/widgets.js` & `djgentelella-0.3.9/djgentelella/static/gentelella/js/widgets.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,9 +1,24 @@
 document.formset = [];
 document.gtwidgets = {
+    ImageRecordInput: function(instance) {
+        instance.each(function(i, e) {
+            getMediaRecord(e, 'photo');
+        });
+    },
+    VideoRecordInput: function(instance) {
+        instance.each(function(i, e) {
+            getMediaRecord(e, 'video');
+        });
+    },
+    AudioRecordInput: function(instance) {
+        instance.each(function(i, e) {
+            getMediaRecord(e, 'audio');
+        });
+    },
     Select: function(instance) {
         instance.each(function(i, e) {
             let s2instance = $(e);
             let contexts2 = {};
             extract_select2_context(contexts2, s2instance);
             s2instance.select2(contexts2);
         });
```

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/autosize/autosize.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/autosize/autosize.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/bootstrap/bootstrap.bundle.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/bootstrap/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/bootstrap/bootstrap.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/bootstrap/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/bootstrap/bootstrap.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/bootstrap/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/bootstrap/popper.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/bootstrap/popper.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-colorpicker/bootstrap-colorpicker.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-colorpicker/bootstrap-colorpicker.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-colorpicker/bootstrap-colorpicker.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-colorpicker/bootstrap-colorpicker.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-daterangepicker/daterangepicker.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-daterangepicker/daterangepicker.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-daterangepicker/daterangepicker.min.css.map` & `djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-daterangepicker/daterangepicker.min.css.map`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-daterangepicker/daterangepicker.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-daterangepicker/daterangepicker.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-daterangepicker/daterangepicker.min.js.map` & `djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-daterangepicker/daterangepicker.min.js.map`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-daterangepicker/moment.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-daterangepicker/moment.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-datetimepicker/bootstrap-datetimepicker.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-datetimepicker/bootstrap-datetimepicker.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-datetimepicker/bootstrap-datetimepicker.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-datetimepicker/bootstrap-datetimepicker.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-maxlength/bootstrap-maxlength.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-maxlength/bootstrap-maxlength.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-progressbar/bootstrap-progressbar-3.3.4.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-progressbar/bootstrap-progressbar-3.3.4.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-progressbar/bootstrap-progressbar.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-progressbar/bootstrap-progressbar.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-tree/bootstrap-treeview.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-tree/bootstrap-treeview.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/bootstrap-tree/bootstrap-treeview.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/bootstrap-tree/bootstrap-treeview.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/chartjs/Chart.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/chartjs/Chart.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/chartjs/Chart.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/chartjs/Chart.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/css/icons/vco-icons.ttf` & `djgentelella-0.3.9/djgentelella/static/vendors/css/icons/vco-icons.ttf`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/datatables/datatables.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/datatables/datatables.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/datatables/datatables.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/datatables/datatables.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/fileupload/jquery.fileupload.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/fileupload/jquery.fileupload.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/fileupload/jquery.iframe-transport.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/fileupload/jquery.iframe-transport.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/fileupload/jquery.ui.widget.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/fileupload/jquery.ui.widget.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/fileupload/spark-md5.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/fileupload/spark-md5.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flag-icon-css/flag-icons.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/flag-icon-css/flag-icons.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ad.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ad.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/af.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/af.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ag.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ag.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ai.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ai.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/al.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/al.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ao.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ao.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/aq.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/aq.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ar.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ar.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/as.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/as.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/au.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/au.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/aw.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/aw.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ax.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ax.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ba.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ba.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/bb.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/bb.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/bh.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/bh.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/bi.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/bi.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/bm.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/bm.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/bn.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/bn.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/bo.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/bo.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/br.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/br.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/bs.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/bs.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/bt.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/bt.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/bv.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/bv.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/by.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/by.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/bz.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/bz.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ca.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ca.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/cc.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/cc.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/cf.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/cf.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ck.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ck.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/cl.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/cl.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/cm.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/cm.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/cn.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/cn.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/cu.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/cu.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/cv.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/cv.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/cw.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/cw.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/cx.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/cx.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/cy.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/cy.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/dj.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/dj.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/dm.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/dm.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/do.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/do.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ec.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ec.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/eg.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/eg.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/eh.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/eh.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/er.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/er.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/es.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/es.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/et.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/et.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/eu.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/eu.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/fj.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/fj.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/fk.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/fk.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/fm.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/fm.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/fo.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/fo.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/gb-nir.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/gb-nir.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/gb-wls.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/gb-wls.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/gb.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/gb.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/gd.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/gd.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ge.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ge.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/gg.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/gg.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/gi.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/gi.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/gq.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/gq.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/gr.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/gr.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/gs.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/gs.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/gt.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/gt.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/gu.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/gu.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/gw.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/gw.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/hk.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/hk.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/hm.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/hm.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/hn.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/hn.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/hr.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/hr.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ht.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ht.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/il.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/il.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/im.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/im.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/in.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/in.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/io.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/io.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/iq.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/iq.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ir.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ir.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/is.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/is.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/je.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/je.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/jo.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/jo.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ke.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ke.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/kg.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/kg.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/kh.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/kh.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ki.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ki.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/km.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/km.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/kn.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/kn.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/kp.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/kp.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/kr.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/kr.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ky.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ky.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/kz.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/kz.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/lb.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/lb.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/li.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/li.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/lk.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/lk.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/lr.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/lr.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ls.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ls.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ly.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ly.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/md.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/md.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/me.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/me.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/mh.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/mh.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/mm.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/mm.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/mn.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/mn.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/mo.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/mo.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/mp.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/mp.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ms.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ms.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/mt.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/mt.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/mw.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/mw.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/mx.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/mx.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/my.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/my.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/mz.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/mz.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/na.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/na.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/nc.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/nc.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/nf.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/nf.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ni.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ni.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/np.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/np.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/nr.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/nr.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/nu.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/nu.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/nz.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/nz.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/om.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/om.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/pa.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/pa.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/pe.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/pe.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/pf.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/pf.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/pg.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/pg.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ph.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ph.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/pk.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/pk.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/pn.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/pn.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/pr.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/pr.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ps.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ps.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/pt.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/pt.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/py.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/py.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/rs.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/rs.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/rw.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/rw.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/sa.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/sa.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/sb.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/sb.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/sc.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/sc.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/se.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/se.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/sg.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/sg.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/sh.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/sh.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/si.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/si.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/sk.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/sk.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/sm.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/sm.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/st.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/st.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/sv.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/sv.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/sx.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/sx.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/sy.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/sy.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/sz.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/sz.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/tc.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/tc.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/tf.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/tf.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/tg.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/tg.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/tj.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/tj.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/tk.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/tk.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/tl.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/tl.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/tm.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/tm.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/tn.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/tn.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/tr.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/tr.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/tv.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/tv.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/tw.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/tw.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/tz.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/tz.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ug.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ug.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/um.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/um.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/un.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/un.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/us.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/us.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/uy.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/uy.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/uz.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/uz.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/va.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/va.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ve.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ve.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/vg.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/vg.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/vi.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/vi.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/vu.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/vu.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/ws.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/ws.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/xk.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/xk.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/za.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/za.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/zm.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/zm.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/1x1/zw.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/1x1/zw.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ad.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ad.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/af.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/af.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ag.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ag.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ai.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ai.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/al.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/al.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ao.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ao.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/aq.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/aq.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ar.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ar.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/as.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/as.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/au.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/au.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/aw.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/aw.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ax.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ax.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/az.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/az.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ba.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ba.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/bb.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/bb.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/bh.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/bh.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/bi.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/bi.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/bm.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/bm.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/bn.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/bn.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/bo.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/bo.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/br.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/br.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/bs.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/bs.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/bt.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/bt.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/bv.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/bv.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/by.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/by.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/bz.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/bz.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ca.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ca.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/cc.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/cc.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/cf.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/cf.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ck.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ck.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/cl.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/cl.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/cm.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/cm.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/cn.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/cn.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/cu.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/cu.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/cv.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/cv.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/cw.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/cw.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/cx.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/cx.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/cy.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/cy.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/dj.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/dj.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/dm.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/dm.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/do.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/do.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ec.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ec.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/eg.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/eg.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/eh.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/eh.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/er.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/er.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/es.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/es.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/et.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/et.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/eu.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/eu.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/fj.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/fj.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/fk.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/fk.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/fm.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/fm.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/fo.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/fo.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/gb-nir.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/gb-nir.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/gb-wls.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/gb-wls.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/gb.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/gb.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/gd.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/gd.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ge.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ge.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/gg.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/gg.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/gi.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/gi.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/gm.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/gm.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/gq.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/gq.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/gr.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/gr.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/gs.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/gs.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/gt.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/gt.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/gu.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/gu.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/gw.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/gw.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/hk.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/hk.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/hm.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/hm.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/hn.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/hn.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/hr.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/hr.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ht.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ht.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/il.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/il.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/im.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/im.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/in.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/in.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/io.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/io.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/iq.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/iq.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ir.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ir.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/is.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/is.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/je.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/je.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/jo.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/jo.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ke.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ke.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/kg.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/kg.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/kh.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/kh.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ki.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ki.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/km.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/km.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/kn.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/kn.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/kp.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/kp.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/kr.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/kr.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ky.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ky.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/kz.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/kz.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/lb.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/lb.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/li.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/li.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/lk.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/lk.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/lr.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/lr.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ls.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ls.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ly.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ly.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/md.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/md.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/me.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/me.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/mh.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/mh.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/mm.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/mm.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/mn.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/mn.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/mo.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/mo.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/mp.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/mp.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ms.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ms.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/mt.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/mt.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/mw.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/mw.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/mx.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/mx.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/my.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/my.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/mz.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/mz.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/na.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/na.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/nc.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/nc.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/nf.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/nf.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ni.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ni.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/np.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/np.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/nr.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/nr.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/nu.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/nu.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/nz.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/nz.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/om.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/om.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/pa.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/pa.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/pe.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/pe.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/pf.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/pf.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/pg.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/pg.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ph.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ph.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/pk.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/pk.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/pn.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/pn.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/pr.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/pr.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ps.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ps.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/pt.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/pt.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/py.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/py.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/rs.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/rs.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/rw.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/rw.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/sa.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/sa.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/sb.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/sb.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/sc.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/sc.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/se.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/se.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/sg.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/sg.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/sh.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/sh.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/si.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/si.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/sk.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/sk.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/sm.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/sm.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/st.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/st.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/sv.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/sv.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/sx.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/sx.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/sy.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/sy.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/sz.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/sz.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/tc.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/tc.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/tf.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/tf.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/tg.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/tg.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/tj.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/tj.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/tk.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/tk.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/tl.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/tl.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/tm.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/tm.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/tn.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/tn.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/tr.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/tr.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/tv.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/tv.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/tw.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/tw.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/tz.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/tz.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ug.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ug.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/um.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/um.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/un.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/un.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/us.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/us.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/uy.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/uy.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/uz.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/uz.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/va.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/va.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ve.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ve.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/vg.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/vg.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/vi.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/vi.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/vu.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/vu.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/ws.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/ws.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/xk.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/xk.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/za.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/za.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/zm.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/zm.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/flags/4x3/zw.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/flags/4x3/zw.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/font-awesome/font-awesome.css.map` & `djgentelella-0.3.9/djgentelella/static/vendors/font-awesome/font-awesome.css.map`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/font-awesome/font-awesome.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/font-awesome/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/fonts/FontAwesome.otf` & `djgentelella-0.3.9/djgentelella/static/vendors/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/fonts/fontawesome-webfont.eot` & `djgentelella-0.3.9/djgentelella/static/vendors/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/fonts/fontawesome-webfont.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/fonts/fontawesome-webfont.ttf` & `djgentelella-0.3.9/djgentelella/static/vendors/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/fonts/fontawesome-webfont.woff` & `djgentelella-0.3.9/djgentelella/static/vendors/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/fonts/fontawesome-webfont.woff2` & `djgentelella-0.3.9/djgentelella/static/vendors/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/fonts/glyphicons-halflings-regular.eot` & `djgentelella-0.3.9/djgentelella/static/vendors/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/fonts/glyphicons-halflings-regular.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/fonts/glyphicons-halflings-regular.ttf` & `djgentelella-0.3.9/djgentelella/static/vendors/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/fonts/glyphicons-halflings-regular.woff` & `djgentelella-0.3.9/djgentelella/static/vendors/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/fonts/glyphicons-halflings-regular.woff2` & `djgentelella-0.3.9/djgentelella/static/vendors/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/fullcalendar/locales-all.js` & `djgentelella-0.3.9/djgentelella/static/vendors/fullcalendar/locales-all.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/fullcalendar/main.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/fullcalendar/main.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/fullcalendar/main.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/fullcalendar/main.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/grid-slider/ion.rangeSlider.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/grid-slider/ion.rangeSlider.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/grid-slider/ion.rangeSlider.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/grid-slider/ion.rangeSlider.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/iCheck/aero.css` & `djgentelella-0.3.9/djgentelella/static/vendors/iCheck/aero.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/iCheck/aero.png` & `djgentelella-0.3.9/djgentelella/static/vendors/iCheck/aero.png`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/iCheck/aero@2x.png` & `djgentelella-0.3.9/djgentelella/static/vendors/iCheck/aero@2x.png`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/iCheck/blue.css` & `djgentelella-0.3.9/djgentelella/static/vendors/iCheck/blue.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/iCheck/blue.png` & `djgentelella-0.3.9/djgentelella/static/vendors/iCheck/blue.png`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/iCheck/blue@2x.png` & `djgentelella-0.3.9/djgentelella/static/vendors/iCheck/blue@2x.png`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/iCheck/green.css` & `djgentelella-0.3.9/djgentelella/static/vendors/iCheck/green.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/iCheck/green.png` & `djgentelella-0.3.9/djgentelella/static/vendors/iCheck/green.png`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/iCheck/green@2x.png` & `djgentelella-0.3.9/djgentelella/static/vendors/iCheck/green@2x.png`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/iCheck/icheck.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/iCheck/icheck.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/iCheck/orange.css` & `djgentelella-0.3.9/djgentelella/static/vendors/iCheck/orange.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/iCheck/orange.png` & `djgentelella-0.3.9/djgentelella/static/vendors/iCheck/orange.png`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/iCheck/orange@2x.png` & `djgentelella-0.3.9/djgentelella/static/vendors/iCheck/orange@2x.png`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/iCheck/yellow.css` & `djgentelella-0.3.9/djgentelella/static/vendors/iCheck/yellow.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/iCheck/yellow.png` & `djgentelella-0.3.9/djgentelella/static/vendors/iCheck/yellow.png`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/iCheck/yellow@2x.png` & `djgentelella-0.3.9/djgentelella/static/vendors/iCheck/yellow@2x.png`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/img/bootstrap-colorpicker/alpha-horizontal.png` & `djgentelella-0.3.9/djgentelella/static/vendors/img/bootstrap-colorpicker/alpha-horizontal.png`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/img/bootstrap-colorpicker/saturation-horizontal.png` & `djgentelella-0.3.9/djgentelella/static/vendors/img/bootstrap-colorpicker/saturation-horizontal.png`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 <html class="no-js ie9" lang="en-US"> <![endif]--><!--[if gt IE 9]><!--><html class="no-js" lang="en-US"> <!--<![endif]-->
 <head>
 <meta charset="UTF-8">
 <meta name="viewport" content="width=device-width, initial-scale=1">
 <meta name="theme-color" content="">
 <link rel="profile" href="https://gmpg.org/xfn/11">
 <meta name="robots" content="noindex, follow">
-<meta name="dlm-version" content="4.7.71">
+<meta name="dlm-version" content="4.7.73">
 
 <title>Page Not Found - Colorlib</title>
 <meta property="og:locale" content="en_US">
 <meta property="og:title" content="Page Not Found - Colorlib">
 <meta property="og:site_name" content="Colorlib">
 <script type="application/ld+json" class="yoast-schema-graph">{"@context":"https://schema.org","@graph":[{"@type":"WebSite","@id":"https://colorlib.com/#website","url":"https://colorlib.com/","name":"Colorlib","description":"Free WordPress Themes","potentialAction":[{"@type":"SearchAction","target":{"@type":"EntryPoint","urlTemplate":"https://colorlib.com/?s={search_term_string}"},"query-input":"required name=search_term_string"}],"inLanguage":"en-US"}]}</script>
 
@@ -81,15 +81,15 @@
 <script type="text/javascript" src="https://colorlib.com/wp-includes/js/jquery/jquery-migrate.min.js?ver=3.3.2" id="jquery-migrate-js"></script>
 <script type="text/javascript" src="https://colorlib.com/wp-content/themes/sparkling/assets/js/vendor/bootstrap.min.js?ver=18a1ebc44d97" id="sparkling-bootstrapjs-js"></script>
 <script type="text/javascript" src="https://colorlib.com/wp-content/themes/sparkling/assets/js/functions.js?ver=90724b2ee937" id="sparkling-functions-js"></script>
 <link rel="https://api.w.org/" href="https://colorlib.com/wp-json/">
 <link rel="EditURI" type="application/rsd+xml" title="RSD" href="https://colorlib.com/xmlrpc.php?rsd">
 <link rel="wlwmanifest" type="application/wlwmanifest+xml" href="https://colorlib.com/wp-includes/wlwmanifest.xml">
 <style>img{height:auto}</style>
-<meta name="generator" content="Easy Digital Downloads v3.1.0.3">
+<meta name="generator" content="Easy Digital Downloads v3.1.0.4">
 <style type="text/css">body, .entry-content {color:#6B6B6B}.entry-content {font-family: Open Sans;}.entry-content {font-size:14px}.entry-content {font-weight:normal}</style>
 <style type="text/css">.recentcomments a{display:inline !important;padding:0 !important;margin:0 !important;}</style>
 <meta name="generator" content="Powered by WPBakery Page Builder - drag and drop page builder for WordPress.">
 <style type="text/css">
 				.navbar > .container .navbar-brand {
 			color: #dadada;
 		}
@@ -284,42 +284,42 @@
 </script>
 <script type="text/javascript" src="https://colorlib.com/wp-content/plugins/contact-form-7/includes/js/index.js?ver=f57435a927d4" id="contact-form-7-js"></script>
 <script type="text/javascript" id="edd-ajax-js-extra">
 /* <![CDATA[ */
 var edd_scripts = {"ajaxurl":"https:\/\/colorlib.com\/wp-admin\/admin-ajax.php","position_in_cart":"-1","has_purchase_links":"","already_in_cart_message":"You have already added this item to your cart","empty_cart_message":"Your cart is empty","loading":"Loading","select_option":"Please select an option","is_checkout":"0","default_gateway":"stripe","redirect_to_checkout":"1","checkout_page":"https:\/\/colorlib.com\/checkout\/","permalinks":"1","quantities_enabled":"","taxes_enabled":"1","current_page":""};
 /* ]]> */
 </script>
-<script type="text/javascript" src="https://colorlib.com/wp-content/plugins/easy-digital-downloads/assets/js/edd-ajax.js?ver=c22eb8f5ecc7" id="edd-ajax-js"></script>
+<script type="text/javascript" src="https://colorlib.com/wp-content/plugins/easy-digital-downloads/assets/js/edd-ajax.js?ver=74d18a0b8807" id="edd-ajax-js"></script>
 <script type="text/javascript" id="dlm-xhr-js-extra">
 /* <![CDATA[ */
 var dlmXHRtranslations = {"error":"An error occurred while trying to download the file. Please try again."};
 /* ]]> */
 </script>
 <script type="text/javascript" id="dlm-xhr-js-before">
-const dlmXHR = {"xhr_links":{"class":["download-link","download-button"]},"prevent_duplicates":true,"ajaxUrl":"https:\/\/colorlib.com\/wp-admin\/admin-ajax.php","nonce":"ee710c523b"}; dlmXHRinstance = {};
+const dlmXHR = {"xhr_links":{"class":["download-link","download-button"]},"prevent_duplicates":true,"ajaxUrl":"https:\/\/colorlib.com\/wp-admin\/admin-ajax.php","nonce":"5f52f7f1b7"}; dlmXHRinstance = {}; const dlmXHRGlobalLinks = "https://colorlib.com/download/"; dlmXHRgif = "https://colorlib.com/wp-includes/images/spinner.gif"
 </script>
-<script type="text/javascript" src="https://colorlib.com/wp-content/plugins/download-monitor/assets/js/dlm-xhr.min.js?ver=ab6a9a875a1d" id="dlm-xhr-js"></script>
+<script type="text/javascript" src="https://colorlib.com/wp-content/plugins/download-monitor/assets/js/dlm-xhr.min.js?ver=0600925864be" id="dlm-xhr-js"></script>
 <script type="text/javascript" src="https://colorlib.com/wp-content/plugins/edd-free-downloads/assets/js/isMobile.min.js?ver=5f371f16343f" id="edd-free-downloads-mobile-js"></script>
 <script type="text/javascript" id="edd-free-downloads-js-extra">
 /* <![CDATA[ */
 var edd_free_downloads_vars = {"close_button":"overlay","user_registration":"false","require_name":"true","download_loading":"Please Wait... ","download_label":"Download Now","modal_download_label":"Download Now","has_ajax":"1","ajaxurl":"https:\/\/colorlib.com\/wp-admin\/admin-ajax.php","mobile_url":"\/polygon\/vendors\/mjolnic-bootstrap-colorpicker\/dist\/img\/bootstrap-colorpicker\/saturation-horizontal.png?edd-free-download=true","form_class":"edd_purchase_submit_wrapper","bypass_logged_in":"false","is_download":"false","edd_is_mobile":"","success_page":"https:\/\/colorlib.com\/checkout\/purchase-confirmation\/","guest_checkout_disabled":"","email_verification":"1","on_complete_handler":"default","on_complete_delay":"2000"};
 /* ]]> */
 </script>
 <script type="text/javascript" src="https://colorlib.com/wp-content/plugins/edd-free-downloads/assets/js/edd-free-downloads.min.js?ver=08cb641a0696" id="edd-free-downloads-js"></script>
 <script type="text/javascript" src="https://colorlib.com/wp-content/themes/sparkling/assets/js/skip-link-focus-fix.min.js?ver=f5b80e59fc74" id="sparkling-skip-link-focus-fix-js"></script>
 <script type="text/javascript" src="https://colorlib.com/wp-content/plugins/jilt-for-edd/assets/js/lib/jquery-blockui/jquery.blockUI.min.js?ver=969879fd894a" id="jquery-block-ui-js"></script>
 <script type="text/javascript" id="edd-jilt-subscribe-form-js-extra">
 /* <![CDATA[ */
-var edd_jilt_subscribe = {"nonce":"419c9c8e04","loader":"https:\/\/colorlib.com\/wp-content\/plugins\/jilt-for-edd\/assets\/img\/ajax-loader.gif"};
+var edd_jilt_subscribe = {"nonce":"b3fb2b86c5","loader":"https:\/\/colorlib.com\/wp-content\/plugins\/jilt-for-edd\/assets\/img\/ajax-loader.gif"};
 /* ]]> */
 </script>
 <script type="text/javascript" src="https://colorlib.com/wp-content/plugins/jilt-for-edd/assets/js/frontend/edd-jilt-subscribe-form.min.js?ver=adf58a385c30" id="edd-jilt-subscribe-form-js"></script>
 <script type="text/javascript" id="edd-jilt-js-extra">
 /* <![CDATA[ */
-var jiltStorefrontParams = {"public_key":"pk_7c26fe596dfb4dc822c0ea3798973692","payment_field_mapping":{"edd_email":"email","edd_first":"first_name","edd_last":"last_name","card_address":"address1","card_address_2":"address2","card_city":"city","card_state":"state_code","card_zip":"postal_code","billing_country":"country_code"},"address_field_mapping":{"card_address":"line1","card_address_2":"line2","card_city":"city","card_state":"state","card_zip":"zip","billing_country":"country"},"cart_hash":"3da2b1d828997364c7a792ab6585d8dd","cart_token":"86e447a2-c67f-46af-a015-b74ce656ba2e","ajax_url":"https:\/\/colorlib.com\/wp-admin\/admin-ajax.php","nonce":"c90c13fe31","log_threshold":"900","x_jilt_shop_domain":"colorlib.com","shop_uuid":"460d09fa-cabc-42ae-b7d4-398bed00c92b","show_email_usage_notice":"","popover_dismiss_message":"No thanks, I'll enter my email later.","platform":"edd","api_url":"https:\/\/api.jilt.com","billing_needs_attention":"","signup_form":"","capture_email_on_add_to_cart":""};
+var jiltStorefrontParams = {"public_key":"pk_7c26fe596dfb4dc822c0ea3798973692","payment_field_mapping":{"edd_email":"email","edd_first":"first_name","edd_last":"last_name","card_address":"address1","card_address_2":"address2","card_city":"city","card_state":"state_code","card_zip":"postal_code","billing_country":"country_code"},"address_field_mapping":{"card_address":"line1","card_address_2":"line2","card_city":"city","card_state":"state","card_zip":"zip","billing_country":"country"},"cart_hash":"39ac19493c9070623dbbd757a17ba388","cart_token":"1629951c-7781-44d5-b743-abfb839b73b2","ajax_url":"https:\/\/colorlib.com\/wp-admin\/admin-ajax.php","nonce":"112b9342fe","log_threshold":"900","x_jilt_shop_domain":"colorlib.com","shop_uuid":"460d09fa-cabc-42ae-b7d4-398bed00c92b","show_email_usage_notice":"","popover_dismiss_message":"No thanks, I'll enter my email later.","platform":"edd","api_url":"https:\/\/api.jilt.com","billing_needs_attention":"","signup_form":"","capture_email_on_add_to_cart":""};
 /* ]]> */
 </script>
 <script type="text/javascript" src="https://js.jilt.com/storefront/v1/jilt.js?ver=1.5.4" id="edd-jilt-js"></script>
 <script type="text/javascript">
 			(function() {
 			var t   = document.createElement( 'script' );
 			t.type  = 'text/javascript';
@@ -329,10 +329,10 @@
 			t.src = '//secure.gaug.es/track.js';
 			var s = document.getElementsByTagName( 'script' )[0];
 			s.parentNode.insertBefore( t, s );
 			})();
 		</script>
 </div>
 <script>(function(){const dpi=window.devicePixelRatio>1?2:1;const images=document.querySelectorAll("img[data-origin-src]");images.forEach(function(image){const image_width=image.offsetWidth*dpi;const render_width=Math.ceil(image_width/100)*100;const origin_src=image.getAttribute("data-origin-src");image.src=`${origin_src}?width=${render_width}`})})();(function(){const events=["mouseover","keydown","touchstart","touchmove","wheel"];const elements=document.querySelectorAll("[data-lazy-method='interaction']");if(!elements.length)return;function load_elements(){clearTimeout(timeout);events.forEach(function(event){window.removeEventListener(event,load_elements,{passive:true})});elements.forEach(function(element){element.getAttribute("data-lazy-attributes").split(",").forEach(function(attribute){const value=element.getAttribute("data-lazy-".concat(attribute));element.setAttribute(attribute,value)})})}const timeout=setTimeout(load_elements,1e4);events.forEach(function(event){window.addEventListener(event,load_elements,{passive:true})})})();(function(){const observer=new IntersectionObserver(function(elements){elements.forEach(function(element){if(element.isIntersecting){observer.unobserve(element.target);element.target.getAttribute("data-lazy-attributes").split(",").forEach(function(attribute){const value=element.target.getAttribute("data-lazy-".concat(attribute));element.target.setAttribute(attribute,value)})}})},{rootMargin:"300px"});document.querySelectorAll("[data-lazy-method='viewport']").forEach(function(element){observer.observe(element)})})();</script>
-<script defer src="https://static.cloudflareinsights.com/beacon.min.js/vaafb692b2aea4879b33c060e79fe94621666317369993" integrity="sha512-0ahDYl866UMhKuYcW078ScMalXqtFJggm7TmlUtp0UlD4eQk0Ixfnm5ykXKvGJNFjLMoortdseTfsRT8oCfgGA==" data-cf-beacon='{"rayId":"78502c86894592fc","token":"cd0b4b3a733644fc843ef0b185f98241","version":"2022.11.3","si":100}' crossorigin="anonymous"></script>
+<script defer src="https://static.cloudflareinsights.com/beacon.min.js/vaafb692b2aea4879b33c060e79fe94621666317369993" integrity="sha512-0ahDYl866UMhKuYcW078ScMalXqtFJggm7TmlUtp0UlD4eQk0Ixfnm5ykXKvGJNFjLMoortdseTfsRT8oCfgGA==" data-cf-beacon='{"rayId":"78b0888bbf2e2b05","token":"cd0b4b3a733644fc843ef0b185f98241","version":"2022.11.3","si":100}' crossorigin="anonymous"></script>
 </body>
 </html>
```

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/img/bootstrap-colorpicker/saturation.png` & `djgentelella-0.3.9/djgentelella/static/vendors/img/bootstrap-colorpicker/saturation.png`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/inputmask/inputmask.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/inputmask/inputmask.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/inputmask/jquery.inputmask.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/inputmask/jquery.inputmask.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/interact/interact.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/interact/interact.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/jquery/jquery.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/jquery/jquery.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/jquery/jquery.min.map` & `djgentelella-0.3.9/djgentelella/static/vendors/jquery/jquery.min.map`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/jquery-knob/jquery.knob.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/jquery-knob/jquery.knob.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/jquery-ui/jquery-ui.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/jquery-ui/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/moment/moment-with-locales.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/moment/moment-with-locales.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/nprogress/nprogress.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/nprogress/nprogress.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/nprogress/nprogress.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/nprogress/nprogress.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/parsleyjs/parsley.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/parsleyjs/parsley.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/select2/select2-bootstrap-5-theme.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/select2/select2-bootstrap-5-theme.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/select2/select2.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/select2/select2.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/select2/select2.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/select2/select2.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/storylinejs/storyline.css` & `djgentelella-0.3.9/djgentelella/static/vendors/storylinejs/storyline.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/storylinejs/storyline.js` & `djgentelella-0.3.9/djgentelella/static/vendors/storylinejs/storyline.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/storymapjs/storymap.css` & `djgentelella-0.3.9/djgentelella/static/vendors/storymapjs/storymap.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/storymapjs/storymap.js` & `djgentelella-0.3.9/djgentelella/static/vendors/storymapjs/storymap.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/summernote/summernote-lite.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/summernote/summernote-lite.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/summernote/summernote-lite.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/summernote/summernote-lite.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/sweetalert2/sweetalert2.all.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/sweetalert2/sweetalert2.all.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/sweetalert2/sweetalert2.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/sweetalert2/sweetalert2.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/switchery/switchery.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/switchery/switchery.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/switchery/switchery.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/switchery/switchery.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/tagify/jQuery.tagify.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/tagify/jQuery.tagify.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/tagify/tagify.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/tagify/tagify.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/tagify/tagify.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/tagify/tagify.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/timeline/css/icons/tl-icons.eot` & `djgentelella-0.3.9/djgentelella/static/vendors/timeline/css/icons/tl-icons.eot`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/timeline/css/icons/tl-icons.svg` & `djgentelella-0.3.9/djgentelella/static/vendors/timeline/css/icons/tl-icons.svg`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/timeline/css/icons/tl-icons.ttf` & `djgentelella-0.3.9/djgentelella/static/vendors/timeline/css/icons/tl-icons.ttf`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/timeline/css/timeline.css` & `djgentelella-0.3.9/djgentelella/static/vendors/timeline/css/timeline.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/timeline/js/timeline.js` & `djgentelella-0.3.9/djgentelella/static/vendors/timeline/js/timeline.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/tinymce/jquery.tinymce.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/tinymce/jquery.tinymce.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skin.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skin.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/content/dark/content.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/content/dark/content.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/content/default/content.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/content/default/content.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/content/document/content.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/content/document/content.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/content/writer/content.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/content/writer/content.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/ui/oxide/content.inline.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/ui/oxide/content.inline.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/ui/oxide/content.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/ui/oxide/content.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/ui/oxide/content.mobile.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/ui/oxide/content.mobile.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/ui/oxide/skin.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/ui/oxide/skin.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/ui/oxide/skin.mobile.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/ui/oxide/skin.mobile.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/ui/oxide/skin.shadowdom.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/ui/oxide/skin.shadowdom.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/ui/oxide-dark/content.inline.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/ui/oxide-dark/content.inline.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/ui/oxide-dark/content.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/ui/oxide-dark/content.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/ui/oxide-dark/content.mobile.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/ui/oxide-dark/content.mobile.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/ui/oxide-dark/skin.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/ui/oxide-dark/skin.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/ui/oxide-dark/skin.mobile.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/ui/oxide-dark/skin.mobile.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/tinymce/skins/ui/oxide-dark/skin.shadowdom.min.css` & `djgentelella-0.3.9/djgentelella/static/vendors/tinymce/skins/ui/oxide-dark/skin.shadowdom.min.css`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/tinymce/themes/mobile/theme.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/tinymce/themes/mobile/theme.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/tinymce/themes/silver/theme.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/tinymce/themes/silver/theme.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/tinymce/tinymce-all.js` & `djgentelella-0.3.9/djgentelella/static/vendors/tinymce/tinymce-all.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/static/vendors/tinymce/tinymce.min.js` & `djgentelella-0.3.9/djgentelella/static/vendors/tinymce/tinymce.min.js`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/cruds/ajax/_form.html` & `djgentelella-0.3.9/djgentelella/templates/cruds/ajax/_form.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/cruds/ajax/delete.html` & `djgentelella-0.3.9/djgentelella/templates/cruds/ajax/delete.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/cruds/ajax/list.html` & `djgentelella-0.3.9/djgentelella/templates/cruds/ajax/list.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/app/messages.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/app/messages.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/app/sidebar.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/app/sidebar.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/app/top_navigation.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/app/top_navigation.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/base.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/base.html`

 * *Files 0% similar despite different names*

```diff
@@ -81,14 +81,17 @@
                     break;
                 }
             }
         }
         return cookieValue;
     }
 
+
+
+
   </script>
   {% block extra_head %}{% endblock %}
 </head>
 
 <body class="{% block body_class %}nav-md {% endblock body_class %}">
 {% block body %}
 <div class="body">
@@ -218,14 +221,17 @@
               'not_found_permissions_label': "{% trans 'This view has not permissions associated.' %}",
               'not_select_valid_option': "{% trans 'You have not selected a valid option.' %}",
               'save_messages': "{% trans 'Permission have been successfully saved.' %}",
               'error': "{% trans 'An error occurred while saving.' %}",
           };
 
 
+
+
+
 </script>
 <script src="{% static 'gentelella/js/permissionmanagement.js' %}?v={% get_version %}"></script>
 {% endif %}
 {% endif %}
 {% render_menu_js_widget %}
 {% endblock %}
```

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/blocks/box.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/blocks/box.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/blocks/crud_list.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/blocks/crud_list.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/blocks/permissions_management.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/blocks/permissions_management.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/cruds/_form.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/cruds/_form.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/cruds/create.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/cruds/create.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/cruds/delete.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/cruds/delete.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/cruds/detail.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/cruds/detail.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/cruds/list.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/cruds/list.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/cruds/pagination/prev_next.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/cruds/pagination/prev_next.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/cruds/update.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/cruds/update.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/index.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/index.html`

 * *Files 8% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 {% define_urlname_action 'pgroup-add'%}
 {% define_urlname_action 'pgroup-edit'%}
 {% define_urlname_action 'abcde-add'%}
 {% define_urlname_action 'abcde-edit'%}
 {% endblock%}
 <div class="row">
 
-<div class='col-sm-12 col-md-12 col-lg-12'>
-     <div class="card">
-            <div class="card-body">
-                <div class="card-title titles">
-                    <h2> A form  </h2>
-                </div>
-                   <form action="" method="POST">
-                    {% csrf_token %}
-                    {{form.as_inline}}
-                    <input class="btn btn-success" type="submit"  value="Save"/>
-                </form>
+  <div class='col-sm-12 col-md-12 col-lg-12'>
+    <div class="card">
+      <div class="card-body">
+        <div class="card-title titles">
+          <h2> A form </h2>
+        </div>
+        <form action="" method="POST" enctype="multipart/form-data">
+          {% csrf_token %}
+          {{form.as_inline}}
+          <input class="btn btn-success" type="submit" value="Save"/>
+        </form>
 
-            </div>
+      </div>
 
-        </div>
-</div>
+    </div>
+  </div>
 </div>
 {% endblock %}
 {% block js %} {{ form.media }} {% endblock %}
```

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/menu/notificacion.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/menu/notificacion.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/menu/notification_list.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/menu/notification_list.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/menu/palette.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/menu/palette.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/menu/palette_modal.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/menu/palette_modal.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/permission_management/permissionmanagement_list.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/permission_management/permissionmanagement_list.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/registration/email_base.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/registration/email_base.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/registration/login.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/registration/login.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/registration/logout.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/registration/logout.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/registration/new_user.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/registration/new_user.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/registration/password_change_form.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/registration/password_reset_confirm.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/registration/password_reset_done.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/registration/password_reset_email.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/registration/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/registration/password_reset_form.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/registration/registration_form.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/registration/registration_form.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/addselect.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/addselect.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/addtreeselect.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/addtreeselect.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/chunkedupload.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/chunkedupload.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/file.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/file.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templates/gentelella/widgets/radio.html` & `djgentelella-0.3.9/djgentelella/templates/gentelella/widgets/radio.html`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templatetags/_utils.py` & `djgentelella-0.3.9/djgentelella/templatetags/_utils.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templatetags/crud_tags.py` & `djgentelella-0.3.9/djgentelella/templatetags/crud_tags.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templatetags/gentelellamenu.py` & `djgentelella-0.3.9/djgentelella/templatetags/gentelellamenu.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templatetags/gtsettings.py` & `djgentelella-0.3.9/djgentelella/templatetags/gtsettings.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/templatetags/urlname_tags.py` & `djgentelella-0.3.9/djgentelella/templatetags/urlname_tags.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/tests/Calendar_Test.py` & `djgentelella-0.3.9/djgentelella/tests/Calendar_Test.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/tests/StoryLine_Test.py` & `djgentelella-0.3.9/djgentelella/tests/StoryLine_Test.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/tests/StoryMap_Test.py` & `djgentelella-0.3.9/djgentelella/tests/StoryMap_Test.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/tests/TimeLine_Test.py` & `djgentelella-0.3.9/djgentelella/tests/TimeLine_Test.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/urls.py` & `djgentelella-0.3.9/djgentelella/urls.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/utils.py` & `djgentelella-0.3.9/djgentelella/utils.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/views/select2autocomplete.py` & `djgentelella-0.3.9/djgentelella/views/select2autocomplete.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/views/storyline.py` & `djgentelella-0.3.9/djgentelella/views/storyline.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/views/storymap.py` & `djgentelella-0.3.9/djgentelella/views/storymap.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/views/timeline.py` & `djgentelella-0.3.9/djgentelella/views/timeline.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/widgets/calendar.py` & `djgentelella-0.3.9/djgentelella/widgets/calendar.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/widgets/color.py` & `djgentelella-0.3.9/djgentelella/widgets/color.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/widgets/core.py` & `djgentelella-0.3.9/djgentelella/widgets/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,14 +160,61 @@
         if 'data-href' not in attrs:
             attrs.update({'data-href': reverse_lazy('upload_file_view')})
         if 'data-done' not in attrs:
             attrs['data-done'] = reverse_lazy('upload_file_done')
         super().__init__(attrs)
 
 
+class ImageRecordInput(DJFileInput):
+    """
+    You can set the preview size using data-width and data-height.
+    """
+    needs_multipart_form = True
+    template_name = 'gentelella/widgets/record_photo.html'
+
+    def __init__(self, attrs=None, extraskwargs=True):
+        if extraskwargs:
+            attrs = update_kwargs(
+                attrs,
+                self.__class__.__name__,
+                base_class='d-none')
+        super().__init__(attrs)
+
+
+class VideoRecordInput(DJFileInput):
+    """
+    You can set the preview size using data-width and data-height.
+
+    .. note:: Size of video depends on camera default configuration.
+    """
+    needs_multipart_form = True
+    template_name = 'gentelella/widgets/record_video.html'
+
+    def __init__(self, attrs=None, extraskwargs=True):
+        if extraskwargs:
+            attrs = update_kwargs(
+                attrs,
+                self.__class__.__name__,
+                base_class='d-none')
+        super().__init__(attrs)
+
+
+class AudioRecordInput(DJFileInput):
+    needs_multipart_form = True
+    template_name = 'gentelella/widgets/record_audio.html'
+
+    def __init__(self, attrs=None, extraskwargs=True):
+        if extraskwargs:
+            attrs = update_kwargs(
+                attrs,
+                self.__class__.__name__,
+                base_class='d-none')
+        super().__init__(attrs)
+
+
 class ClearableFileInput(DJClearableFileInput):
     template_name = 'gentelella/widgets/file.html'
 
     def __init__(self, attrs=None, extraskwargs=True):
         if extraskwargs:
             attrs = update_kwargs(attrs, self.__class__.__name__)
         super().__init__(attrs)
```

### Comparing `djgentelella-0.3.8/djgentelella/widgets/files.py` & `djgentelella-0.3.9/djgentelella/widgets/files.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/widgets/helper.py` & `djgentelella-0.3.9/djgentelella/widgets/helper.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/widgets/selects.py` & `djgentelella-0.3.9/djgentelella/widgets/selects.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/widgets/storyline.py` & `djgentelella-0.3.9/djgentelella/widgets/storyline.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/widgets/storymap.py` & `djgentelella-0.3.9/djgentelella/widgets/storymap.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/widgets/tagging.py` & `djgentelella-0.3.9/djgentelella/widgets/tagging.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/widgets/timeline.py` & `djgentelella-0.3.9/djgentelella/widgets/timeline.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/widgets/tinymce.py` & `djgentelella-0.3.9/djgentelella/widgets/tinymce.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/widgets/trees.py` & `djgentelella-0.3.9/djgentelella/widgets/trees.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/widgets/wysiwyg.py` & `djgentelella-0.3.9/djgentelella/widgets/wysiwyg.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella/wysiwyg/views.py` & `djgentelella-0.3.9/djgentelella/wysiwyg/views.py`

 * *Files identical despite different names*

### Comparing `djgentelella-0.3.8/djgentelella.egg-info/PKG-INFO` & `djgentelella-0.3.9/djgentelella.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: djgentelella
-Version: 0.3.8
+Version: 0.3.9
 Summary: Extra widgets for django using gentelella.
 Home-page: https://solvosoft.com
 Author: Luis Zarate Montero
 Author-email: luis.zarate@solvosoft.com
 License: GNU General Public License
 Description: Django Gentelella widgets
         ############################
```

### Comparing `djgentelella-0.3.8/djgentelella.egg-info/SOURCES.txt` & `djgentelella-0.3.9/djgentelella.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -130,14 +130,15 @@
 djgentelella/static/gentelella/js/base/dateranges_gridslider.js
 djgentelella/static/gentelella/js/base/editorTinymce.js
 djgentelella/static/gentelella/js/base/fileupload.widget.js
 djgentelella/static/gentelella/js/base/formset.js
 djgentelella/static/gentelella/js/base/gigapixel_storymap.js
 djgentelella/static/gentelella/js/base/helper_widget.js
 djgentelella/static/gentelella/js/base/mapbased_storymap.js
+djgentelella/static/gentelella/js/base/mediarecord.js
 djgentelella/static/gentelella/js/base/notifications.js
 djgentelella/static/gentelella/js/base/select2_wrap.js
 djgentelella/static/gentelella/js/base/select2related.js
 djgentelella/static/gentelella/js/base/storyline.js
 djgentelella/static/gentelella/js/base/timeline.js
 djgentelella/static/gentelella/js/base/wysiwyg.js
 djgentelella/static/vendors/autosize/autosize.min.js
@@ -874,14 +875,17 @@
 djgentelella/templates/gentelella/widgets/number_knob_input.html
 djgentelella/templates/gentelella/widgets/password.html
 djgentelella/templates/gentelella/widgets/phone_number_input_mask.html
 djgentelella/templates/gentelella/widgets/radio.html
 djgentelella/templates/gentelella/widgets/radio_input_option.html
 djgentelella/templates/gentelella/widgets/radio_option.html
 djgentelella/templates/gentelella/widgets/radio_select.html
+djgentelella/templates/gentelella/widgets/record_audio.html
+djgentelella/templates/gentelella/widgets/record_photo.html
+djgentelella/templates/gentelella/widgets/record_video.html
 djgentelella/templates/gentelella/widgets/select.html
 djgentelella/templates/gentelella/widgets/select_date.html
 djgentelella/templates/gentelella/widgets/select_option.html
 djgentelella/templates/gentelella/widgets/serial_number_input_mask.html
 djgentelella/templates/gentelella/widgets/splitdatetime.html
 djgentelella/templates/gentelella/widgets/splithiddendatetime.html
 djgentelella/templates/gentelella/widgets/storyline.html
```

### Comparing `djgentelella-0.3.8/setup.py` & `djgentelella-0.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 '''
 Created on 12/02/2020
 
 @author: luisza
 '''
 
-from setuptools import setup, find_packages
 import os
 
+from setuptools import setup, find_packages
+
 CLASSIFIERS = [
     'Environment :: Web Environment',
     'Framework :: Django',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
     'Operating System :: OS Independent',
     'Programming Language :: Python',
@@ -23,15 +24,15 @@
 ]
 
 README = open(os.path.join(os.path.dirname(__file__), 'Readme.rst')).read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
-version = '0.3.8'
+version = '0.3.9'
 
 setup(
     author='Luis Zarate Montero',
     author_email='luis.zarate@solvosoft.com',
     name='djgentelella',
     version=version,
     description='Extra widgets for django using gentelella.',
```

