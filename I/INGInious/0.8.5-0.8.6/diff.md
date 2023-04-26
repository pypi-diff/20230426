# Comparing `tmp/INGInious-0.8.5.tar.gz` & `tmp/INGInious-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "INGInious-0.8.5.tar", last modified: Thu Mar 23 07:53:10 2023, max compression
+gzip compressed data, was "INGInious-0.8.6.tar", last modified: Wed Apr 26 10:06:31 2023, max compression
```

## Comparing `INGInious-0.8.5.tar` & `INGInious-0.8.6.tar`

### file list

```diff
@@ -1,1018 +1,1018 @@
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.068127 INGInious-0.8.5/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.920127 INGInious-0.8.5/.github/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.940127 INGInious-0.8.5/.github/workflows/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1850 2023-03-23 07:41:45.000000 INGInious-0.8.5/.github/workflows/ci.yml
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      422 2022-02-09 10:08:57.000000 INGInious-0.8.5/.gitignore
--rw-r--r--   0 anthony   (1000) anthony   (1000)       22 2018-11-16 12:58:08.000000 INGInious-0.8.5/.landscape.yml
--rw-r--r--   0 anthony   (1000) anthony   (1000)    10147 2018-11-16 12:58:08.000000 INGInious-0.8.5/.pylintrc
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      156 2021-06-10 10:07:01.000000 INGInious-0.8.5/.readthedocs.yaml
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1581 2018-11-16 12:58:08.000000 INGInious-0.8.5/.travis.yml
--rw-r--r--   0 anthony   (1000) anthony   (1000)      622 2023-03-14 08:45:50.000000 INGInious-0.8.5/COPYRIGHTS
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.941127 INGInious-0.8.5/INGInious.egg-info/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3124 2023-03-23 07:53:09.000000 INGInious-0.8.5/INGInious.egg-info/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)    40029 2023-03-23 07:53:09.000000 INGInious-0.8.5/INGInious.egg-info/SOURCES.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2023-03-23 07:53:09.000000 INGInious-0.8.5/INGInious.egg-info/dependency_links.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)      658 2023-03-23 07:53:09.000000 INGInious-0.8.5/INGInious.egg-info/requires.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       10 2023-03-23 07:53:09.000000 INGInious-0.8.5/INGInious.egg-info/top_level.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)    34764 2018-11-16 12:58:08.000000 INGInious-0.8.5/LICENSE
--rw-r--r--   0 anthony   (1000) anthony   (1000)      440 2018-11-16 12:58:08.000000 INGInious-0.8.5/MANIFEST.in
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3124 2023-03-23 07:53:10.068127 INGInious-0.8.5/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2688 2023-03-23 07:41:45.000000 INGInious-0.8.5/README.rst
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.921127 INGInious-0.8.5/base-containers/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.941127 INGInious-0.8.5/base-containers/base/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1927 2022-07-12 07:33:48.000000 INGInious-0.8.5/base-containers/base/Dockerfile
--rw-r--r--   0 anthony   (1000) anthony   (1000)      610 2018-11-16 12:58:08.000000 INGInious-0.8.5/base-containers/base/README.md
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.943127 INGInious-0.8.5/base-containers/base/bin/
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)    19095 2023-02-28 09:27:21.000000 INGInious-0.8.5/base-containers/base/bin/INGInious
--rwxrwxr-x   0 anthony   (1000) anthony   (1000)     5040 2022-03-18 07:57:30.000000 INGInious-0.8.5/base-containers/base/bin/_run_student_intern
--rwxrwxr-x   0 anthony   (1000) anthony   (1000)     1418 2021-04-26 06:37:40.000000 INGInious-0.8.5/base-containers/base/bin/archive
--rwxrwxr-x   0 anthony   (1000) anthony   (1000)     2830 2021-04-26 06:37:40.000000 INGInious-0.8.5/base-containers/base/bin/feedback
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1088 2021-04-26 06:37:40.000000 INGInious-0.8.5/base-containers/base/bin/feedback-custom
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      549 2021-04-26 06:37:40.000000 INGInious-0.8.5/base-containers/base/bin/feedback-grade
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1306 2021-04-26 06:37:40.000000 INGInious-0.8.5/base-containers/base/bin/feedback-msg
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1533 2021-04-26 06:37:40.000000 INGInious-0.8.5/base-containers/base/bin/feedback-msg-tpl
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      812 2021-04-26 06:37:40.000000 INGInious-0.8.5/base-containers/base/bin/feedback-result
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      569 2021-04-26 06:37:40.000000 INGInious-0.8.5/base-containers/base/bin/feedback-state
--rwxrwxr-x   0 anthony   (1000) anthony   (1000)     1180 2021-06-10 10:07:01.000000 INGInious-0.8.5/base-containers/base/bin/getinput
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1090 2022-02-08 16:02:58.000000 INGInious-0.8.5/base-containers/base/bin/inginious-ipython
--rwxrwxr-x   0 anthony   (1000) anthony   (1000)     1066 2021-04-26 06:37:40.000000 INGInious-0.8.5/base-containers/base/bin/parsetemplate
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1064 2021-04-26 06:37:40.000000 INGInious-0.8.5/base-containers/base/bin/rst-code
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      737 2021-04-26 06:37:40.000000 INGInious-0.8.5/base-containers/base/bin/rst-image
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1277 2021-04-26 06:37:40.000000 INGInious-0.8.5/base-containers/base/bin/rst-indent
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1223 2021-04-26 06:37:40.000000 INGInious-0.8.5/base-containers/base/bin/rst-msgblock
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)     2752 2023-02-28 09:27:21.000000 INGInious-0.8.5/base-containers/base/bin/run_student
--rwxrwxr-x   0 anthony   (1000) anthony   (1000)     2953 2022-02-09 08:29:26.000000 INGInious-0.8.5/base-containers/base/bin/ssh_student
--rwxrwxr-x   0 anthony   (1000) anthony   (1000)      491 2021-04-26 06:37:40.000000 INGInious-0.8.5/base-containers/base/bin/tag
--rwxrwxr-x   0 anthony   (1000) anthony   (1000)      623 2021-04-26 06:37:40.000000 INGInious-0.8.5/base-containers/base/bin/tag-set
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.944127 INGInious-0.8.5/base-containers/base/inginious_container_api/
--rwxrwxr-x   0 anthony   (1000) anthony   (1000)       30 2021-04-26 06:37:40.000000 INGInious-0.8.5/base-containers/base/inginious_container_api/__init__.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     6616 2022-02-09 10:08:57.000000 INGInious-0.8.5/base-containers/base/inginious_container_api/feedback.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3400 2021-06-10 10:07:01.000000 INGInious-0.8.5/base-containers/base/inginious_container_api/input.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      789 2021-04-26 06:37:40.000000 INGInious-0.8.5/base-containers/base/inginious_container_api/lang.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1704 2021-04-26 06:37:40.000000 INGInious-0.8.5/base-containers/base/inginious_container_api/rst.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    16470 2023-02-28 09:27:21.000000 INGInious-0.8.5/base-containers/base/inginious_container_api/run_student.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      466 2021-04-26 06:37:40.000000 INGInious-0.8.5/base-containers/base/inginious_container_api/run_types.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3065 2022-02-09 08:57:05.000000 INGInious-0.8.5/base-containers/base/inginious_container_api/ssh_student.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    13519 2022-03-30 06:18:20.000000 INGInious-0.8.5/base-containers/base/inginious_container_api/utils.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.945127 INGInious-0.8.5/base-containers/default/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      210 2021-02-12 07:54:48.000000 INGInious-0.8.5/base-containers/default/Dockerfile
--rw-r--r--   0 anthony   (1000) anthony   (1000)      378 2018-11-16 12:58:08.000000 INGInious-0.8.5/base-containers/default/README.md
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2068 2021-06-10 10:07:01.000000 INGInious-0.8.5/configuration.example.yaml
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.947127 INGInious-0.8.5/doc/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6910 2018-11-16 12:58:08.000000 INGInious-0.8.5/doc/Makefile
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.921127 INGInious-0.8.5/doc/admin_doc/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.949127 INGInious-0.8.5/doc/admin_doc/commands_doc/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2703 2022-02-09 10:08:57.000000 INGInious-0.8.5/doc/admin_doc/commands_doc/inginious-agent-docker.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      824 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/admin_doc/commands_doc/inginious-agent-mcq.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1192 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/admin_doc/commands_doc/inginious-autotest.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      881 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/admin_doc/commands_doc/inginious-backend.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      336 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/admin_doc/commands_doc/inginious-container-update.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      407 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/admin_doc/commands_doc/inginious-database-update.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      569 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/admin_doc/commands_doc/inginious-install.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1297 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/admin_doc/commands_doc/inginious-synchronize.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      980 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/admin_doc/commands_doc/inginious-webapp.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      980 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/admin_doc/commands_doc/inginious-webdav.rst
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.950127 INGInious-0.8.5/doc/admin_doc/install_doc/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    18632 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/admin_doc/install_doc/config_reference.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)     9220 2023-03-23 07:44:27.000000 INGInious-0.8.5/doc/admin_doc/install_doc/create_container.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)    21186 2023-03-23 07:41:45.000000 INGInious-0.8.5/doc/admin_doc/install_doc/installation.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2094 2022-02-09 08:57:05.000000 INGInious-0.8.5/doc/admin_doc/install_doc/other_oci_runtimes_support.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1350 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/admin_doc/install_doc/static_pages.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3847 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/admin_doc/install_doc/troubleshooting.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1342 2022-02-09 08:22:39.000000 INGInious-0.8.5/doc/admin_doc/install_doc/updating.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1172 2023-03-23 07:41:45.000000 INGInious-0.8.5/doc/admin_documentation.rst
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.952127 INGInious-0.8.5/doc/api_doc/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      506 2018-11-16 12:58:08.000000 INGInious-0.8.5/doc/api_doc/inginious.agent.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)      336 2018-11-16 12:58:08.000000 INGInious-0.8.5/doc/api_doc/inginious.backend.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)      715 2018-11-16 12:58:08.000000 INGInious-0.8.5/doc/api_doc/inginious.client.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      414 2022-03-18 07:57:30.000000 INGInious-0.8.5/doc/api_doc/inginious.common.filesystems.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1495 2022-03-18 07:57:30.000000 INGInious-0.8.5/doc/api_doc/inginious.common.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)      692 2018-11-16 12:58:08.000000 INGInious-0.8.5/doc/api_doc/inginious.common.task_file_readers.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      570 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/api_doc/inginious.common.tests.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1286 2018-11-16 12:58:08.000000 INGInious-0.8.5/doc/api_doc/inginious.frontend.pages.api.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2429 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/api_doc/inginious.frontend.pages.course_admin.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1474 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/api_doc/inginious.frontend.pages.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      664 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/api_doc/inginious.frontend.plugins.auth.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1146 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/api_doc/inginious.frontend.plugins.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)      212 2018-11-16 12:58:08.000000 INGInious-0.8.5/doc/api_doc/inginious.frontend.plugins.scoreboard.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3200 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/api_doc/inginious.frontend.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1483 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/api_doc/inginious.frontend.tests.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      324 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/api_doc/inginious.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)    10661 2023-03-14 08:45:50.000000 INGInious-0.8.5/doc/conf.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.921127 INGInious-0.8.5/doc/dev_doc/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.953127 INGInious-0.8.5/doc/dev_doc/extensions_doc/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1902 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/dev_doc/extensions_doc/how_to_extend.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      753 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/dev_doc/extensions_doc/i18n.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)    16600 2023-03-14 09:48:05.000000 INGInious-0.8.5/doc/dev_doc/extensions_doc/plugins.rst
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.956127 INGInious-0.8.5/doc/dev_doc/internals_doc/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2083 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/dev_doc/internals_doc/architectures.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2309 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/dev_doc/internals_doc/exercises.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1217 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/dev_doc/internals_doc/frontend.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)       37 2023-03-23 07:41:45.000000 INGInious-0.8.5/doc/dev_doc/internals_doc/groupes_audiences.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    71784 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/dev_doc/internals_doc/inginious_arch.png
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    97918 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/dev_doc/internals_doc/inginious_arch_docker.png
--rw-rw-r--   0 anthony   (1000) anthony   (1000)   119437 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/dev_doc/internals_doc/inginious_arch_full.png
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    20901 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/dev_doc/internals_doc/submission_evaluation_docker.png
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    51028 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/dev_doc/internals_doc/submission_workflow.png
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     5607 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/dev_doc/internals_doc/submissions.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3834 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/dev_doc/internals_doc/understand_inginious.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)      618 2023-03-23 07:41:45.000000 INGInious-0.8.5/doc/developer_documentation.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      297 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/index.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    11703 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/logo_rtd.svg
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6707 2018-11-16 12:58:08.000000 INGInious-0.8.5/doc/make.bat
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.960127 INGInious-0.8.5/doc/teacher_doc/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4806 2018-11-16 12:58:08.000000 INGInious-0.8.5/doc/teacher_doc/best_practices.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      952 2021-04-26 06:37:40.000000 INGInious-0.8.5/doc/teacher_doc/common.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)    11047 2023-03-23 07:41:45.000000 INGInious-0.8.5/doc/teacher_doc/course_admin.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     4106 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/teacher_doc/course_description.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1093 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/teacher_doc/course_tuto.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      921 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/teacher_doc/courses.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1168 2022-02-08 16:02:58.000000 INGInious-0.8.5/doc/teacher_doc/inginious_container_api.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3025 2022-03-18 07:57:30.000000 INGInious-0.8.5/doc/teacher_doc/lti.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1856 2021-04-26 06:37:40.000000 INGInious-0.8.5/doc/teacher_doc/random.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5807 2022-08-11 06:40:58.000000 INGInious-0.8.5/doc/teacher_doc/rst.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)    34270 2023-02-27 12:38:00.000000 INGInious-0.8.5/doc/teacher_doc/run_file.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)      764 2018-11-16 12:58:08.000000 INGInious-0.8.5/doc/teacher_doc/share_files.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)      975 2018-11-16 12:58:08.000000 INGInious-0.8.5/doc/teacher_doc/system_files.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     9474 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/teacher_doc/task_file.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     5397 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/teacher_doc/task_tuto.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      214 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/teacher_doc/tasks.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1676 2018-11-16 12:58:08.000000 INGInious-0.8.5/doc/teacher_doc/testing.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3060 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/teacher_doc/translating.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      197 2022-02-09 08:22:39.000000 INGInious-0.8.5/doc/teacher_documentation.rst
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     5111 2021-06-10 10:07:01.000000 INGInious-0.8.5/doc/what_is_inginious.rst
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.960127 INGInious-0.8.5/inginious/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      709 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/__init__.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.960127 INGInious-0.8.5/inginious/agent/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    12044 2022-08-30 07:08:17.000000 INGInious-0.8.5/inginious/agent/__init__.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.960127 INGInious-0.8.5/inginious/agent/docker_agent/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    50529 2023-03-23 07:43:59.000000 INGInious-0.8.5/inginious/agent/docker_agent/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    13345 2023-03-23 07:43:59.000000 INGInious-0.8.5/inginious/agent/docker_agent/_docker_interface.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)      858 2023-03-23 07:43:59.000000 INGInious-0.8.5/inginious/agent/docker_agent/_docker_runtime.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4597 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/agent/docker_agent/_timeout_watcher.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.961127 INGInious-0.8.5/inginious/agent/mcq_agent/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6721 2022-08-30 07:08:17.000000 INGInious-0.8.5/inginious/agent/mcq_agent/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)       42 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/agent/mcq_agent/babel.cfg
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.961127 INGInious-0.8.5/inginious/agent/mcq_agent/i18n/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.922127 INGInious-0.8.5/inginious/agent/mcq_agent/i18n/de/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.961127 INGInious-0.8.5/inginious/agent/mcq_agent/i18n/de/LC_MESSAGES/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1037 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/agent/mcq_agent/i18n/de/LC_MESSAGES/messages.mo
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1505 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/agent/mcq_agent/i18n/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.922127 INGInious-0.8.5/inginious/agent/mcq_agent/i18n/es/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.962127 INGInious-0.8.5/inginious/agent/mcq_agent/i18n/es/LC_MESSAGES/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1051 2022-02-09 10:08:57.000000 INGInious-0.8.5/inginious/agent/mcq_agent/i18n/es/LC_MESSAGES/messages.mo
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1525 2022-02-09 10:08:57.000000 INGInious-0.8.5/inginious/agent/mcq_agent/i18n/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.922127 INGInious-0.8.5/inginious/agent/mcq_agent/i18n/fr/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.962127 INGInious-0.8.5/inginious/agent/mcq_agent/i18n/fr/LC_MESSAGES/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1059 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/agent/mcq_agent/i18n/fr/LC_MESSAGES/messages.mo
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1530 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/agent/mcq_agent/i18n/fr/LC_MESSAGES/messages.po
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1109 2021-04-26 06:37:40.000000 INGInious-0.8.5/inginious/agent/mcq_agent/i18n/messages.pot
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.962127 INGInious-0.8.5/inginious/backend/
--rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/backend/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    22973 2023-02-27 12:38:00.000000 INGInious-0.8.5/inginious/backend/backend.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1894 2022-02-09 08:29:26.000000 INGInious-0.8.5/inginious/backend/topic_priority_queue.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.963127 INGInious-0.8.5/inginious/client/
--rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/client/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     9874 2023-02-23 07:55:28.000000 INGInious-0.8.5/inginious/client/_zeromq_client.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    16216 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/client/client.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2541 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/client/client_buffer.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1271 2021-04-26 06:37:40.000000 INGInious-0.8.5/inginious/client/client_sync.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.965127 INGInious-0.8.5/inginious/common/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      242 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/common/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2607 2023-02-23 07:55:28.000000 INGInious-0.8.5/inginious/common/asyncio_utils.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2458 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/common/babel.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     4805 2022-03-30 09:10:41.000000 INGInious-0.8.5/inginious/common/base.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3124 2021-04-26 06:37:40.000000 INGInious-0.8.5/inginious/common/custom_yaml.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4275 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/common/entrypoints.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      701 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/common/exceptions.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.965127 INGInious-0.8.5/inginious/common/filesystems/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     5291 2022-03-18 07:57:30.000000 INGInious-0.8.5/inginious/common/filesystems/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6096 2022-12-14 10:14:50.000000 INGInious-0.8.5/inginious/common/filesystems/local.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2131 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/common/log.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    14512 2022-08-30 07:08:17.000000 INGInious-0.8.5/inginious/common/messages.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2672 2021-04-26 06:37:40.000000 INGInious-0.8.5/inginious/common/tags.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.966127 INGInious-0.8.5/inginious/common/task_file_readers/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      224 2020-08-25 08:18:47.000000 INGInious-0.8.5/inginious/common/task_file_readers/__init__.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      755 2020-08-25 08:18:47.000000 INGInious-0.8.5/inginious/common/task_file_readers/abstract_reader.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      650 2020-08-25 08:18:47.000000 INGInious-0.8.5/inginious/common/task_file_readers/yaml_reader.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    14652 2023-03-23 07:44:31.000000 INGInious-0.8.5/inginious/common/tasks_problems.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.966127 INGInious-0.8.5/inginious/common/tests/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5009 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/common/tests/TestBase.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2823 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/common/tests/TestCustomYaml.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)      206 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/common/tests/__init__.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    12982 2022-02-09 10:08:57.000000 INGInious-0.8.5/inginious/common/tests/test_filesystem_local.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.970127 INGInious-0.8.5/inginious/frontend/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      214 2022-03-18 08:08:05.000000 INGInious-0.8.5/inginious/frontend/__init__.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     5943 2022-02-09 08:22:39.000000 INGInious-0.8.5/inginious/frontend/accessible_time.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    15300 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/app.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4770 2023-02-02 07:45:35.000000 INGInious-0.8.5/inginious/frontend/arch_helper.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      138 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/babel.cfg
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    10782 2022-03-18 08:08:05.000000 INGInious-0.8.5/inginious/frontend/course_factory.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    11693 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/courses.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.971127 INGInious-0.8.5/inginious/frontend/environment_types/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      859 2023-03-23 07:43:59.000000 INGInious-0.8.5/inginious/frontend/environment_types/__init__.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      361 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/environment_types/docker.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      920 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/environment_types/env_type.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2146 2023-02-28 09:27:21.000000 INGInious-0.8.5/inginious/frontend/environment_types/generic_docker_oci_runtime.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      287 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/environment_types/kata.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      408 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/environment_types/mcq.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)      288 2023-03-23 07:43:59.000000 INGInious-0.8.5/inginious/frontend/environment_types/nvidia.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.972127 INGInious-0.8.5/inginious/frontend/flask/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      157 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/flask/__init__.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)       43 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/flask/mail.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    11759 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/flask/mapping.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     5564 2022-02-09 10:08:57.000000 INGInious-0.8.5/inginious/frontend/flask/mongo_sessions.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.972127 INGInious-0.8.5/inginious/frontend/i18n/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.923127 INGInious-0.8.5/inginious/frontend/i18n/de/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.973127 INGInious-0.8.5/inginious/frontend/i18n/de/LC_MESSAGES/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    25694 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/i18n/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 anthony   (1000) anthony   (1000)   110889 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/i18n/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.923127 INGInious-0.8.5/inginious/frontend/i18n/el/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.973127 INGInious-0.8.5/inginious/frontend/i18n/el/LC_MESSAGES/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    29887 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/i18n/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 anthony   (1000) anthony   (1000)   119743 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/i18n/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.923127 INGInious-0.8.5/inginious/frontend/i18n/es/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.973127 INGInious-0.8.5/inginious/frontend/i18n/es/LC_MESSAGES/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    47593 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/i18n/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 anthony   (1000) anthony   (1000)   132063 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/i18n/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.923127 INGInious-0.8.5/inginious/frontend/i18n/fr/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.974127 INGInious-0.8.5/inginious/frontend/i18n/fr/LC_MESSAGES/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    60340 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/i18n/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 anthony   (1000) anthony   (1000)   127508 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/i18n/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.924127 INGInious-0.8.5/inginious/frontend/i18n/he/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.974127 INGInious-0.8.5/inginious/frontend/i18n/he/LC_MESSAGES/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    68397 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/i18n/he/LC_MESSAGES/messages.mo
--rw-r--r--   0 anthony   (1000) anthony   (1000)   130391 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/i18n/he/LC_MESSAGES/messages.po
--rw-r--r--   0 anthony   (1000) anthony   (1000)    99891 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/i18n/messages.pot
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.924127 INGInious-0.8.5/inginious/frontend/i18n/nl/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.974127 INGInious-0.8.5/inginious/frontend/i18n/nl/LC_MESSAGES/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4937 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/i18n/nl/LC_MESSAGES/messages.mo
--rw-r--r--   0 anthony   (1000) anthony   (1000)   102119 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/i18n/nl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.924127 INGInious-0.8.5/inginious/frontend/i18n/pt/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.975127 INGInious-0.8.5/inginious/frontend/i18n/pt/LC_MESSAGES/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    24190 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/i18n/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 anthony   (1000) anthony   (1000)   119920 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/i18n/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.924127 INGInious-0.8.5/inginious/frontend/i18n/pt_BR/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.975127 INGInious-0.8.5/inginious/frontend/i18n/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      530 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/i18n/pt_BR/LC_MESSAGES/messages.mo
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.924127 INGInious-0.8.5/inginious/frontend/i18n/vi/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.975127 INGInious-0.8.5/inginious/frontend/i18n/vi/LC_MESSAGES/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    34450 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/i18n/vi/LC_MESSAGES/messages.mo
--rw-r--r--   0 anthony   (1000) anthony   (1000)   118219 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/i18n/vi/LC_MESSAGES/messages.po
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.924127 INGInious-0.8.5/inginious/frontend/i18n/wa/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.976127 INGInious-0.8.5/inginious/frontend/i18n/wa/LC_MESSAGES/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2170 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/i18n/wa/LC_MESSAGES/messages.mo
--rw-rw-r--   0 anthony   (1000) anthony   (1000)   100743 2022-02-09 10:08:57.000000 INGInious-0.8.5/inginious/frontend/i18n/wa/LC_MESSAGES/messages.po
--rw-r--r--   0 anthony   (1000) anthony   (1000)    27989 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/installer.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      639 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/l10n_manager.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     4924 2021-02-19 11:28:54.000000 INGInious-0.8.5/inginious/frontend/lti_outcome_manager.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2061 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/lti_request_validator.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      777 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/lti_tool_provider.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3385 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/marketplace_courses.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.978127 INGInious-0.8.5/inginious/frontend/pages/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      196 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/pages/__init__.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.979127 INGInious-0.8.5/inginious/frontend/pages/admin/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      199 2022-03-30 09:10:41.000000 INGInious-0.8.5/inginious/frontend/pages/admin/__init__.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2944 2022-03-30 09:10:41.000000 INGInious-0.8.5/inginious/frontend/pages/admin/admin.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.980127 INGInious-0.8.5/inginious/frontend/pages/api/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      191 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/pages/api/__init__.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     6726 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/pages/api/_api_page.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1476 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/pages/api/auth_methods.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1615 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/pages/api/authentication.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2946 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/pages/api/courses.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8534 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/pages/api/submissions.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4517 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/pages/api/tasks.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4502 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/pages/course.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.982127 INGInious-0.8.5/inginious/frontend/pages/course_admin/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      189 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/pages/course_admin/__init__.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     5328 2022-02-09 10:08:57.000000 INGInious-0.8.5/inginious/frontend/pages/course_admin/audience_edit.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    10305 2022-03-30 09:10:41.000000 INGInious-0.8.5/inginious/frontend/pages/course_admin/danger_zone.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1425 2023-03-23 07:44:51.000000 INGInious-0.8.5/inginious/frontend/pages/course_admin/search_user.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5138 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/pages/course_admin/settings.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    13926 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/pages/course_admin/statistics.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2690 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/pages/course_admin/student_info.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    18777 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/pages/course_admin/student_list.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3489 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/pages/course_admin/submission.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    12967 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/pages/course_admin/submissions.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2377 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/pages/course_admin/tags.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    13627 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/pages/course_admin/task_edit.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    11817 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/pages/course_admin/task_edit_file.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5408 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/pages/course_admin/task_list.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    16859 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/pages/course_admin/utils.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1811 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/pages/course_register.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1240 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/pages/courselist.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     4503 2022-03-18 07:57:30.000000 INGInious-0.8.5/inginious/frontend/pages/group.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      813 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/pages/index.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    12033 2022-02-09 10:08:57.000000 INGInious-0.8.5/inginious/frontend/pages/lti.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      571 2021-07-15 06:35:04.000000 INGInious-0.8.5/inginious/frontend/pages/maintenance.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3957 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/pages/marketplace.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2326 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/pages/marketplace_course.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3020 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/pages/mycourses.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.983127 INGInious-0.8.5/inginious/frontend/pages/preferences/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      179 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/pages/preferences/__init__.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2090 2022-03-30 09:10:41.000000 INGInious-0.8.5/inginious/frontend/pages/preferences/bindings.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1950 2022-03-30 09:10:41.000000 INGInious-0.8.5/inginious/frontend/pages/preferences/delete.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     6131 2022-03-30 09:10:41.000000 INGInious-0.8.5/inginious/frontend/pages/preferences/profile.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1396 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/pages/preferences/utils.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      981 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/pages/queue.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     9157 2022-03-30 09:10:41.000000 INGInious-0.8.5/inginious/frontend/pages/register.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3533 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/pages/social.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    22133 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/pages/tasks.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    14567 2022-08-03 10:55:31.000000 INGInious-0.8.5/inginious/frontend/pages/utils.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    13757 2022-12-14 10:19:50.000000 INGInious-0.8.5/inginious/frontend/parsable_text.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4724 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/plugin_manager.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.983127 INGInious-0.8.5/inginious/frontend/plugins/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      203 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/plugins/__init__.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.984127 INGInious-0.8.5/inginious/frontend/plugins/auth/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      180 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/plugins/auth/__init__.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.987127 INGInious-0.8.5/inginious/frontend/plugins/auth/__pycache__/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      210 2022-01-01 20:58:44.000000 INGInious-0.8.5/inginious/frontend/plugins/auth/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 anthony   (1000) anthony   (1000)      200 2021-02-26 16:21:15.000000 INGInious-0.8.5/inginious/frontend/plugins/auth/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 anthony   (1000) anthony   (1000)      204 2021-02-26 10:55:03.000000 INGInious-0.8.5/inginious/frontend/plugins/auth/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 anthony   (1000) anthony   (1000)      208 2021-04-21 06:41:19.000000 INGInious-0.8.5/inginious/frontend/plugins/auth/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 anthony   (1000) anthony   (1000)      208 2021-02-26 10:50:17.000000 INGInious-0.8.5/inginious/frontend/plugins/auth/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3416 2022-01-01 20:58:44.000000 INGInious-0.8.5/inginious/frontend/plugins/auth/__pycache__/google_auth.cpython-310.pyc
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3372 2021-12-16 14:52:36.000000 INGInious-0.8.5/inginious/frontend/plugins/auth/__pycache__/google_auth.cpython-36.pyc
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3442 2023-02-28 09:13:57.000000 INGInious-0.8.5/inginious/frontend/plugins/auth/__pycache__/google_auth.cpython-38.pyc
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3426 2021-06-18 12:47:24.000000 INGInious-0.8.5/inginious/frontend/plugins/auth/__pycache__/google_auth.cpython-39.pyc
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6216 2022-02-09 08:43:21.000000 INGInious-0.8.5/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-310.pyc
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6129 2021-12-16 14:52:36.000000 INGInious-0.8.5/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-36.pyc
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     6096 2021-03-01 12:53:51.000000 INGInious-0.8.5/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-37.pyc
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6226 2023-02-28 09:14:23.000000 INGInious-0.8.5/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-38.pyc
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6232 2021-10-25 13:22:36.000000 INGInious-0.8.5/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-39.pyc
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6434 2022-01-01 20:58:44.000000 INGInious-0.8.5/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-310.pyc
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6394 2021-12-16 14:52:36.000000 INGInious-0.8.5/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-36.pyc
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     6389 2021-03-01 13:00:13.000000 INGInious-0.8.5/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-37.pyc
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6466 2023-02-28 09:13:57.000000 INGInious-0.8.5/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-38.pyc
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6464 2021-06-18 12:47:24.000000 INGInious-0.8.5/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-39.pyc
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1691 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/plugins/auth/custom_auth_form.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     4075 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/plugins/auth/facebook_auth.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2665 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/plugins/auth/github_auth.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2979 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/plugins/auth/google_auth.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     7358 2022-02-09 08:29:26.000000 INGInious-0.8.5/inginious/frontend/plugins/auth/ldap_auth.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3082 2022-06-13 06:34:05.000000 INGInious-0.8.5/inginious/frontend/plugins/auth/linkedin_auth.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     7053 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/plugins/auth/saml2_auth.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     4317 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/plugins/auth/twitter_auth.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.990127 INGInious-0.8.5/inginious/frontend/plugins/contests/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    11265 2023-03-14 09:48:05.000000 INGInious-0.8.5/inginious/frontend/plugins/contests/__init__.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.991127 INGInious-0.8.5/inginious/frontend/plugins/contests/__pycache__/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7900 2023-03-14 09:50:07.000000 INGInious-0.8.5/inginious/frontend/plugins/contests/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     7995 2021-03-01 12:53:52.000000 INGInious-0.8.5/inginious/frontend/plugins/contests/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7976 2023-02-28 09:13:57.000000 INGInious-0.8.5/inginious/frontend/plugins/contests/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     7930 2021-04-29 09:45:18.000000 INGInious-0.8.5/inginious/frontend/plugins/contests/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     5410 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/plugins/contests/admin.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1671 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/plugins/contests/course_menu.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     4223 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/plugins/contests/scoreboard.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.991127 INGInious-0.8.5/inginious/frontend/plugins/demo/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      583 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/plugins/demo/__init__.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.991127 INGInious-0.8.5/inginious/frontend/plugins/git_repo/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     4807 2020-08-25 08:18:47.000000 INGInious-0.8.5/inginious/frontend/plugins/git_repo/__init__.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.991127 INGInious-0.8.5/inginious/frontend/plugins/ltibestsubmission/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3438 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/plugins/ltibestsubmission/__init__.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.992127 INGInious-0.8.5/inginious/frontend/plugins/scoreboard/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     9753 2022-07-12 06:51:08.000000 INGInious-0.8.5/inginious/frontend/plugins/scoreboard/__init__.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.993127 INGInious-0.8.5/inginious/frontend/plugins/scoreboard/__pycache__/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     6649 2022-03-30 09:15:04.000000 INGInious-0.8.5/inginious/frontend/plugins/scoreboard/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     6798 2021-03-01 12:53:52.000000 INGInious-0.8.5/inginious/frontend/plugins/scoreboard/__pycache__/__init__.cpython-37.pyc
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     6738 2021-04-21 06:41:19.000000 INGInious-0.8.5/inginious/frontend/plugins/scoreboard/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     6731 2021-04-29 09:45:18.000000 INGInious-0.8.5/inginious/frontend/plugins/scoreboard/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      354 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/plugins/scoreboard/course_menu.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1220 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/plugins/scoreboard/main.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1418 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/plugins/scoreboard/scoreboard.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      425 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/plugins/scoreboard/task_menu.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.993127 INGInious-0.8.5/inginious/frontend/plugins/simple_grader/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     6106 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/plugins/simple_grader/__init__.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.993127 INGInious-0.8.5/inginious/frontend/plugins/task_editor_hook_example/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1363 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/plugins/task_editor_hook_example/__init__.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      816 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/plugins/task_editor_hook_example/example_tab_2.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.994127 INGInious-0.8.5/inginious/frontend/plugins/task_file_readers/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      212 2020-08-25 08:18:47.000000 INGInious-0.8.5/inginious/frontend/plugins/task_file_readers/__init__.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      976 2020-08-25 08:18:47.000000 INGInious-0.8.5/inginious/frontend/plugins/task_file_readers/json_reader.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.994127 INGInious-0.8.5/inginious/frontend/plugins/upcoming_tasks/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6301 2023-03-14 09:48:05.000000 INGInious-0.8.5/inginious/frontend/plugins/upcoming_tasks/__init__.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.995127 INGInious-0.8.5/inginious/frontend/plugins/upcoming_tasks/templates/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4945 2023-03-14 09:48:05.000000 INGInious-0.8.5/inginious/frontend/plugins/upcoming_tasks/templates/coming_tasks.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)      198 2023-03-14 09:48:05.000000 INGInious-0.8.5/inginious/frontend/plugins/upcoming_tasks/templates/main_menu.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)      358 2023-03-14 09:48:05.000000 INGInious-0.8.5/inginious/frontend/plugins/upcoming_tasks/templates/upcoming.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2803 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/plugins/upcoming_tasks/templates/upcoming_task_list.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.936127 INGInious-0.8.5/inginious/frontend/static/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.996127 INGInious-0.8.5/inginious/frontend/static/css/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    11071 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/static/css/INGInious.css
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3518 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/static/css/INGInious.less
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     9063 2021-04-26 06:37:40.000000 INGInious-0.8.5/inginious/frontend/static/css/bootstrap-datetimepicker.min.css
--rw-r--r--   0 anthony   (1000) anthony   (1000)   134084 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/static/css/bootstrap.min.css
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8217 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/css/codemirror.css
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     9044 2022-03-30 06:18:20.000000 INGInious-0.8.5/inginious/frontend/static/css/common.less
--rw-r--r--   0 anthony   (1000) anthony   (1000)    31000 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/css/font-awesome.min.css
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     7996 2021-06-18 12:47:19.000000 INGInious-0.8.5/inginious/frontend/static/css/lti.css
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      254 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/static/css/lti.less
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    11150 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/static/css/selectize.css
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.001127 INGInious-0.8.5/inginious/frontend/static/fonts/
--rw-r--r--   0 anthony   (1000) anthony   (1000)   134808 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/fonts/FontAwesome.otf
--rw-r--r--   0 anthony   (1000) anthony   (1000)   165742 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/fonts/fontawesome-webfont.eot
--rw-r--r--   0 anthony   (1000) anthony   (1000)   444379 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/fonts/fontawesome-webfont.svg
--rw-r--r--   0 anthony   (1000) anthony   (1000)   165548 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 anthony   (1000) anthony   (1000)    98024 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/fonts/fontawesome-webfont.woff
--rw-r--r--   0 anthony   (1000) anthony   (1000)    77160 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 anthony   (1000) anthony   (1000)    20127 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 anthony   (1000) anthony   (1000)   108738 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 anthony   (1000) anthony   (1000)    45404 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 anthony   (1000) anthony   (1000)    23424 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 anthony   (1000) anthony   (1000)    18028 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.006127 INGInious-0.8.5/inginious/frontend/static/icons/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1856 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/icons/apple-touch-icon-114x114.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1844 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/icons/apple-touch-icon-120x120.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2259 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/icons/apple-touch-icon-144x144.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2312 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/icons/apple-touch-icon-152x152.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1020 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/icons/apple-touch-icon-57x57.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1101 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/icons/apple-touch-icon-60x60.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1241 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/icons/apple-touch-icon-72x72.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1294 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/icons/apple-touch-icon-76x76.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2810 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/icons/apple-touch-icon-precomposed.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2312 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/icons/apple-touch-icon.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)      371 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/icons/browserconfig.xml
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3475 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/icons/favicon-160x160.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)      535 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/icons/favicon-16x16.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2870 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/icons/favicon-196x196.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)      928 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/icons/favicon-32x32.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2226 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/icons/favicon-96x96.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)    15086 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/icons/favicon.ico
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4358 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/icons/google-icon.svg
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3186 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/icons/mstile-144x144.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2135 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/icons/mstile-150x150.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1829 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/icons/mstile-310x150.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3819 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/icons/mstile-310x310.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1970 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/icons/mstile-70x70.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2531 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/icons/wb.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1573 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/icons/wb.svg
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.007127 INGInious-0.8.5/inginious/frontend/static/images/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5244 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/images/header.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6681 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/images/inginious_full.svg
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6531 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/images/inginious_full_logo_only.svg
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4730 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/images/inginious_horiz.svg
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4728 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/images/inginious_vert.svg
--rw-r--r--   0 anthony   (1000) anthony   (1000)    14493 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/images/logo.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)    13380 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/images/logo_maintenance.png
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.009127 INGInious-0.8.5/inginious/frontend/static/js/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2445 2022-03-30 09:10:41.000000 INGInious-0.8.5/inginious/frontend/static/js/admin.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)   638597 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/static/js/all-minified.js
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3828 2022-02-09 10:08:57.000000 INGInious-0.8.5/inginious/frontend/static/js/audiences.js
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2838 2021-04-26 06:37:40.000000 INGInious-0.8.5/inginious/frontend/static/js/checked-list-group.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.009127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1107 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/LICENSE
--rw-r--r--   0 anthony   (1000) anthony   (1000)   205623 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/codemirror.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.010127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.010127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/apl/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4736 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/apl/apl.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2179 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/apl/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.011127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/asciiarmor/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2378 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/asciiarmor/asciiarmor.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1289 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/asciiarmor/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.011127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/asn.1/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7735 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/asn.1/asn.1.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2222 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/asn.1/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.011127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/asterisk/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7437 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/asterisk/asterisk.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4591 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/asterisk/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.012127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/brainfuck/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2174 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/brainfuck/brainfuck.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3338 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/brainfuck/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.012127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/clike/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    31062 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/clike/clike.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)    10105 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/clike/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    28518 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/clike/scala.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.013127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/clojure/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    16005 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/clojure/clojure.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2550 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/clojure/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.013127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/cmake/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2600 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/cmake/cmake.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4152 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/cmake/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.013127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/cobol/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    10288 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/cobol/cobol.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8084 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/cobol/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.014127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/coffeescript/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     9884 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/coffeescript/coffeescript.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)    22402 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/coffeescript/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.014127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/commonlisp/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4569 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/commonlisp/commonlisp.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6691 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/commonlisp/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.014127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/crystal/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    12818 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/crystal/crystal.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2605 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/crystal/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.016127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/css/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    37613 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/css/css.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2780 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/css/gss.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)      460 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/css/gss_test.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1911 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/css/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4066 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/css/less.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1871 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/css/less_test.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2742 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/css/scss.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3124 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/css/scss_test.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.016127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/cypher/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6362 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/cypher/cypher.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1908 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/cypher/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.016127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/d/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7566 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/d/d.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6332 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/d/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.017127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/dart/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5124 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/dart/dart.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1627 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/dart/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.017127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/diff/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1138 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/diff/diff.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4409 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/diff/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.017127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/django/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    11791 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/django/django.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2077 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/django/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.018127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/dockerfile/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2221 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/dockerfile/dockerfile.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2267 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/dockerfile/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.018127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/dtd/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4814 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/dtd/dtd.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3337 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/dtd/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.018127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/dylan/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    10112 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/dylan/dylan.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)    13032 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/dylan/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.019127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/ebnf/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6085 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/ebnf/ebnf.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2450 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/ebnf/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.019127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/ecl/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8843 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/ecl/ecl.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1409 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/ecl/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.019127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/eiffel/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3744 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/eiffel/eiffel.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)    13198 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/eiffel/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.019127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/elm/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5552 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/elm/elm.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1640 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/elm/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.020127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/erlang/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    18887 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/erlang/erlang.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2168 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/erlang/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.020127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/factor/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3565 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/factor/factor.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2024 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/factor/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.020127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/fcl/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4703 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/fcl/fcl.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3091 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/fcl/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.021127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/forth/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5230 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/forth/forth.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1783 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/forth/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.021127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/fortran/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8686 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/fortran/fortran.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2492 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/fortran/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.021127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/gas/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8886 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/gas/gas.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1840 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/gas/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.022127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/gfm/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5103 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/gfm/gfm.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2583 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/gfm/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.022127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/gherkin/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    13257 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/gherkin/gherkin.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1566 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/gherkin/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.023127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/go/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6030 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/go/go.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2174 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/go/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.023127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/groovy/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7904 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/groovy/groovy.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2177 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/groovy/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.023127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/haml/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5353 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/haml/haml.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2071 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/haml/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.023127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/handlebars/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2172 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/handlebars/handlebars.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2196 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/handlebars/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.024127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/haskell/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8109 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/haskell/haskell.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2194 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/haskell/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.024127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/haskell-literate/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1390 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/haskell-literate/haskell-literate.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     9381 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/haskell-literate/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.024127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/haxe/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    17563 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/haxe/haxe.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2577 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/haxe/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.025127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/htmlembedded/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1417 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/htmlembedded/htmlembedded.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2086 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/htmlembedded/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.025127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/htmlmixed/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5611 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/htmlmixed/htmlmixed.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3434 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/htmlmixed/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.025127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/http/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2795 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/http/http.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1393 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/http/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.025127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/idl/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    14889 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/idl/idl.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1633 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/idl/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8286 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/index.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.026127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/javascript/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4193 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/javascript/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    31566 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/javascript/javascript.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2150 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/javascript/json-ld.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1557 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/javascript/typescript.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.026127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/jinja2/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1755 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/jinja2/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4279 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/jinja2/jinja2.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.027127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/jsx/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2410 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/jsx/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5195 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/jsx/jsx.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.027127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/julia/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2375 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/julia/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    12089 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/julia/julia.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.027127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/livescript/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     9843 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/livescript/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7668 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/livescript/livescript.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.028127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/lua/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2073 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/lua/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5950 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/lua/lua.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.028127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/markdown/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    10957 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/markdown/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    25671 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/markdown/markdown.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.028127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mathematica/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2254 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mathematica/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5612 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mathematica/mathematica.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.029127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mbox/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1293 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mbox/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3649 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mbox/mbox.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)    15098 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/meta.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.029127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mirc/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5798 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mirc/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    10077 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mirc/mirc.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.029127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mllike/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4436 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mllike/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5097 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mllike/mllike.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.030127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/modelica/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2007 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/modelica/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6930 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/modelica/modelica.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.030127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mscgen/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4310 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mscgen/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6820 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mscgen/mscgen.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3795 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mscgen/mscgen_test.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3255 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mscgen/msgenny_test.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4006 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mscgen/xu_test.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.031127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mumps/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2608 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mumps/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5354 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mumps/mumps.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.031127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/nginx/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5239 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/nginx/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    10164 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/nginx/nginx.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.031127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/nsis/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1764 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/nsis/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7642 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/nsis/nsis.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.032127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/ntriples/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1357 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/ntriples/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6643 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/ntriples/ntriples.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.032127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/octave/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1805 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/octave/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4522 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/octave/octave.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.032127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/oz/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1389 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/oz/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6665 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/oz/oz.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.033127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/pascal/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1440 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/pascal/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3055 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/pascal/pascal.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.033127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/pegjs/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1890 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/pegjs/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3577 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/pegjs/pegjs.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.033127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/perl/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1542 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/perl/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    56135 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/perl/perl.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.034127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/php/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1999 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/php/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    18224 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/php/php.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.034127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/pig/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1475 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/pig/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5810 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/pig/pig.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.034127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/powershell/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7372 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/powershell/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    12896 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/powershell/powershell.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.035127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/properties/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1555 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/properties/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2171 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/properties/properties.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.035127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/protobuf/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1680 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/protobuf/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2113 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/protobuf/protobuf.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.035127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/pug/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2489 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/pug/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    16046 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/pug/pug.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.036127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/puppet/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3260 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/puppet/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7568 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/puppet/puppet.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.036127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/python/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5950 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/python/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    12479 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/python/python.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.036127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/q/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8961 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/q/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6593 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/q/q.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.037127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/r/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2518 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/r/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6396 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/r/r.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.037127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/rpm/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.037127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/rpm/changes/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2180 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/rpm/changes/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4623 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/rpm/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3775 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/rpm/rpm.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.037127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/rst/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    17769 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/rst/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    17547 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/rst/rst.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.038127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/ruby/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5749 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/ruby/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    10516 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/ruby/ruby.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.038127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/rust/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1532 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/rust/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3025 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/rust/rust.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.039127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/sas/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1854 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/sas/index.html
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)    15424 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/sas/sas.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.039127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/sass/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1631 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/sass/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    11509 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/sass/sass.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.040127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/scheme/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2554 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/scheme/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    13437 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/scheme/scheme.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.040127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/shell/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1745 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/shell/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4002 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/shell/shell.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.040127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/sieve/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2335 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/sieve/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4284 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/sieve/sieve.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.040127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/slim/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2920 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/slim/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    18026 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/slim/slim.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.041127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/smalltalk/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1904 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/smalltalk/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4543 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/smalltalk/smalltalk.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.041127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/smarty/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3973 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/smarty/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6828 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/smarty/smarty.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.041127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/solr/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1365 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/solr/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2672 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/solr/solr.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.042127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/soy/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1939 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/soy/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    12239 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/soy/soy.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.042127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/sparql/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1773 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/sparql/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6335 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/sparql/sparql.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.042127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/spreadsheet/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1392 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/spreadsheet/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3139 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/spreadsheet/spreadsheet.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.043127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/sql/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2991 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/sql/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    37351 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/sql/sql.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.043127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/stex/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4132 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/stex/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6932 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/stex/stex.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.043127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/stylus/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2472 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/stylus/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    42256 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/stylus/stylus.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.044127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/swift/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2085 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/swift/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7168 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/swift/swift.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.044127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/tcl/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6297 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/tcl/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4920 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/tcl/tcl.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.044127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/textile/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4347 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/textile/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    13835 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/textile/textile.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.045127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/tiddlywiki/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4579 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/tiddlywiki/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)      220 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/tiddlywiki/tiddlywiki.css
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8510 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/tiddlywiki/tiddlywiki.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.045127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/tiki/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1745 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/tiki/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)      439 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/tiki/tiki.css
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8462 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/tiki/tiki.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.045127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/toml/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1840 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/toml/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2897 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/toml/toml.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.046127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/tornado/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1803 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/tornado/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2496 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/tornado/tornado.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.046127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/troff/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4465 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/troff/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2392 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/troff/troff.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.046127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/ttcn/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3490 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/ttcn/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    10155 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/ttcn/ttcn.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.047127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/ttcn-cfg/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3605 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/ttcn-cfg/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7857 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/ttcn-cfg/ttcn-cfg.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.047127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/turtle/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1470 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/turtle/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4849 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/turtle/turtle.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.047127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/twig/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1370 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/twig/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4565 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/twig/twig.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.048128 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/vb/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1500 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/vb/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8734 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/vb/vb.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.048128 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/vbscript/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1517 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/vbscript/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    13793 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/vbscript/vbscript.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.048128 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/velocity/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3300 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/velocity/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7098 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/velocity/velocity.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.048128 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/verilog/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2619 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/verilog/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    24588 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/verilog/verilog.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.049127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/vhdl/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2486 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/vhdl/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6704 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/vhdl/vhdl.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.049127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/vue/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2064 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/vue/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2544 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/vue/vue.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.049127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/webidl/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2171 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/webidl/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5784 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/webidl/webidl.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.050127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/xml/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2171 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/xml/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    12570 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/xml/xml.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.050127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/xquery/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8609 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/xquery/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    14470 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/xquery/xquery.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.050127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/yacas/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2176 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/yacas/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5424 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/yacas/yacas.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.051127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/yaml/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2098 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/yaml/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3693 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/yaml/yaml.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.051127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/yaml-frontmatter/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3072 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/yaml-frontmatter/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2292 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/yaml-frontmatter/yaml-frontmatter.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.051127 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/z80/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1406 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/z80/index.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3577 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/z80/z80.js
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     6370 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/static/js/common.js
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     7286 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/static/js/groups.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.053127 INGInious-0.8.5/inginious/frontend/static/js/libs/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    42997 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/static/js/libs/Sortable.min.js
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    56581 2021-04-26 06:37:40.000000 INGInious-0.8.5/inginious/frontend/static/js/libs/bootstrap-datetimepicker.min.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)    51039 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/static/js/libs/bootstrap.min.js
--rw-rw-r--   0 anthony   (1000) anthony   (1000)   158741 2021-04-26 06:37:40.000000 INGInious-0.8.5/inginious/frontend/static/js/libs/chart.min.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)    15252 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/js/libs/jquery.form.min.js
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    86926 2021-04-26 06:37:40.000000 INGInious-0.8.5/inginious/frontend/static/js/libs/jquery.min.js
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     6542 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/static/js/libs/jquery.twbsPagination.min.js
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    51679 2021-04-26 06:37:40.000000 INGInious-0.8.5/inginious/frontend/static/js/libs/moment.min.js
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    20535 2021-04-26 06:37:40.000000 INGInious-0.8.5/inginious/frontend/static/js/libs/popper.min.js
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    41501 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/static/js/libs/selectize.min.js
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    50945 2021-04-26 06:37:40.000000 INGInious-0.8.5/inginious/frontend/static/js/libs/sentry-io-bundle.min.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)    24394 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/static/js/studio.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)    30954 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/static/js/task.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)    16389 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/static/js/task_dispensers.js
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      727 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/static/js/webapp.js
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.936127 INGInious-0.8.5/inginious/frontend/static/plugins/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.054127 INGInious-0.8.5/inginious/frontend/static/plugins/contests/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1413 2023-03-14 09:48:05.000000 INGInious-0.8.5/inginious/frontend/static/plugins/contests/contests.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4566 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/plugins/contests/jquery.countdown.min.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)      996 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/static/plugins/contests/scoreboard.css
--rw-r--r--   0 anthony   (1000) anthony   (1000)    35823 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/submission_manager.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.054127 INGInious-0.8.5/inginious/frontend/task_dispensers/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2312 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/task_dispensers/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3324 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/task_dispensers/combinatory_test.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2957 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/task_dispensers/toc.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7041 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/task_dispensers/util.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    13648 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/task_factory.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     9078 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/task_problems.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    11661 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/tasks.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     6972 2022-02-09 08:21:51.000000 INGInious-0.8.5/inginious/frontend/template_helper.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.058127 INGInious-0.8.5/inginious/frontend/templates/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.058127 INGInious-0.8.5/inginious/frontend/templates/admin/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    12064 2022-03-30 09:10:41.000000 INGInious-0.8.5/inginious/frontend/templates/admin/admin_users.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2986 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/auth.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7753 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/templates/course.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.060127 INGInious-0.8.5/inginious/frontend/templates/course_admin/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     9319 2022-02-09 10:08:57.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/audience_edit.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    10121 2022-02-09 10:08:57.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/danger_zone.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.061128 INGInious-0.8.5/inginious/frontend/templates/course_admin/edit_tabs/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    14096 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/edit_tabs/basic.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3536 2023-02-28 09:27:21.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/edit_tabs/env_generic_docker_oci.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1846 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/edit_tabs/environment.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1776 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/edit_tabs/file_modals.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3675 2022-03-30 06:18:20.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/edit_tabs/files.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1085 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/edit_tabs/subproblems.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      913 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/menu.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    18882 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/settings.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    14180 2022-03-30 06:18:20.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/stats.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     6499 2022-02-09 10:08:57.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/student_info.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    28812 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/student_list.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     5905 2022-03-30 06:18:20.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/student_list_table.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7590 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/submission.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    12969 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/submissions.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    17267 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/submissions_query.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.061128 INGInious-0.8.5/inginious/frontend/templates/course_admin/subproblems/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2032 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/subproblems/code.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1332 2023-02-27 12:38:00.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/subproblems/file.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1050 2023-03-23 07:44:31.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/subproblems/match.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2826 2022-02-09 08:22:39.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/subproblems/multiple_choice.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2174 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/subproblems/multiple_choice_templates.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5141 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/tags.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.062127 INGInious-0.8.5/inginious/frontend/templates/course_admin/task_dispensers/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1698 2023-03-14 09:48:05.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/task_dispensers/combinatory_test.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1225 2023-01-11 09:03:30.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/task_dispensers/empty_section.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1795 2023-03-14 09:48:05.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/task_dispensers/section.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      894 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/task_dispensers/section_config.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1352 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/task_dispensers/section_menu.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1249 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/task_dispensers/task_buttons.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2322 2023-03-14 09:48:05.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/task_dispensers/task_list.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1003 2023-03-14 09:48:05.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/task_dispensers/toc.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4564 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/task_dispensers/util.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2481 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/task_dispensers/util_delete_modal.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     9608 2023-03-14 09:48:05.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/task_edit.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5346 2023-03-14 09:48:05.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/task_list.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      476 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/course_admin/user_selection_box.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2034 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/course_register.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1573 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/course_unavailable.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     4040 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/courselist.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      493 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/forbidden.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     8084 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/group.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      667 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/internalerror.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    13580 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/templates/layout.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2128 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/lti_bind.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1462 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/lti_login.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      572 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/maintenance.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     4826 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/marketplace.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2796 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/marketplace_course.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     5383 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/mycourses.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      492 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/notfound.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.063127 INGInious-0.8.5/inginious/frontend/templates/preferences/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3987 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/preferences/bindings.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2872 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/preferences/delete.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      469 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/preferences/menu.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     4723 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/preferences/profile.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     4845 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/queue.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     5245 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/register.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      539 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/signin_button.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      271 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/static.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    25388 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/templates/task.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.063127 INGInious-0.8.5/inginious/frontend/templates/task_dispensers/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3268 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/templates/task_dispensers/task_list.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1819 2023-03-21 11:59:59.000000 INGInious-0.8.5/inginious/frontend/templates/task_dispensers/toc.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      513 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/task_unavailable.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.064128 INGInious-0.8.5/inginious/frontend/templates/tasks/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      528 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/tasks/code.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1039 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/tasks/file.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      307 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/tasks/match.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      644 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/tasks/multiple_choice.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      640 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/tasks/single_line_code.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1430 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/templates/unregister_modal.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.065127 INGInious-0.8.5/inginious/frontend/tests/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    16896 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/tests/SeleniumFormatter.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6346 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/tests/SeleniumTest.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4326 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/tests/TestCourse.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3383 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/tests/TestLogin.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2639 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/tests/TestParsableText.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)      972 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/tests/TestPluginManager.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7381 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/tests/TestTask.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1841 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/tests/TestTaskDisplay.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1975 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/tests/TestTaskSubmission.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious/frontend/tests/__init__.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.937127 INGInious-0.8.5/inginious/frontend/tests/tasks/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.065127 INGInious-0.8.5/inginious/frontend/tests/tasks/invalid_course/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)       72 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/tests/tasks/invalid_course/course.yaml
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.065127 INGInious-0.8.5/inginious/frontend/tests/tasks/test/
--rw-r--r--   0 anthony   (1000) anthony   (1000)       73 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/tests/tasks/test/course.yaml
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.065127 INGInious-0.8.5/inginious/frontend/tests/tasks/test/task1/
--rwxrwxr-x   0 anthony   (1000) anthony   (1000)       41 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/tests/tasks/test/task1/run
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      573 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/tests/tasks/test/task1/task.yaml
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.066127 INGInious-0.8.5/inginious/frontend/tests/tasks/test/task2/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      320 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/tests/tasks/test/task2/task.yaml
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.066127 INGInious-0.8.5/inginious/frontend/tests/tasks/test/task3/
--rwxrwxr-x   0 anthony   (1000) anthony   (1000)       41 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/tests/tasks/test/task3/run
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      363 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/tests/tasks/test/task3/task.yaml
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.066127 INGInious-0.8.5/inginious/frontend/tests/tasks/test/task4/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      275 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/tests/tasks/test/task4/task.yaml
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.066127 INGInious-0.8.5/inginious/frontend/tests/tasks/test2/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)       79 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/tests/tasks/test2/course.yaml
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.066127 INGInious-0.8.5/inginious/frontend/tests/tasks/test2/task1/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      320 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/tests/tasks/test2/task1/task.yaml
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.066127 INGInious-0.8.5/inginious/frontend/tests/tasks/test2/task2/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      339 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/tests/tasks/test2/task2/task.yaml
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.067127 INGInious-0.8.5/inginious/frontend/tests/tasks/test2/task3/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      559 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/tests/tasks/test2/task3/task.yaml
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.067127 INGInious-0.8.5/inginious/frontend/tests/tasks/test2/task4/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      275 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/tests/tasks/test2/task4/task.yaml
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.067127 INGInious-0.8.5/inginious/frontend/tests/tasks/test3/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      122 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/tests/tasks/test3/course.json
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.067127 INGInious-0.8.5/inginious/frontend/tests/tasks/test3/invalid_task/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)       34 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/tests/tasks/test3/invalid_task/task.yaml
--rw-r--r--   0 anthony   (1000) anthony   (1000)    44783 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious/frontend/user_manager.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     9056 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious/frontend/webdav.py
--rwxrwxr-x   0 anthony   (1000) anthony   (1000)     6462 2022-02-09 10:08:57.000000 INGInious-0.8.5/inginious-agent-docker
--rwxrwxr-x   0 anthony   (1000) anthony   (1000)     3404 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious-agent-mcq
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)    12793 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious-autotest
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)     2162 2018-11-16 12:58:08.000000 INGInious-0.8.5/inginious-backend
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)      649 2023-03-23 07:41:45.000000 INGInious-0.8.5/inginious-install
--rwxrwxr-x   0 anthony   (1000) anthony   (1000)     3981 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious-webapp
--rwxrwxr-x   0 anthony   (1000) anthony   (1000)     3038 2021-06-10 10:07:01.000000 INGInious-0.8.5/inginious-webdav
--rw-r--r--   0 anthony   (1000) anthony   (1000)       38 2023-03-23 07:53:10.068127 INGInious-0.8.5/setup.cfg
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2441 2023-03-23 07:43:39.000000 INGInious-0.8.5/setup.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:09.937127 INGInious-0.8.5/utils/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.067127 INGInious-0.8.5/utils/container_update/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3199 2022-02-09 10:08:57.000000 INGInious-0.8.5/utils/container_update/inginious-container-update
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.067127 INGInious-0.8.5/utils/database_updater/
--rwxrwxr-x   0 anthony   (1000) anthony   (1000)     4682 2022-02-09 10:08:57.000000 INGInious-0.8.5/utils/database_updater/inginious-database-update
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.068127 INGInious-0.8.5/utils/minify/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2728 2023-03-23 07:41:45.000000 INGInious-0.8.5/utils/minify/Gruntfile.js
--rw-r--r--   0 anthony   (1000) anthony   (1000)      452 2023-03-23 07:41:45.000000 INGInious-0.8.5/utils/minify/package.json
--rw-r--r--   0 anthony   (1000) anthony   (1000)      936 2018-11-16 12:58:08.000000 INGInious-0.8.5/utils/minify/watchers.xml
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-03-23 07:53:10.068127 INGInious-0.8.5/utils/sync/
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)     3220 2018-11-16 12:58:08.000000 INGInious-0.8.5/utils/sync/inginious-synchronize
--rw-r--r--   0 anthony   (1000) anthony   (1000)      349 2018-11-16 12:58:08.000000 INGInious-0.8.5/utils/sync/synchronize.json.example
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.164087 INGInious-0.8.6/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.030087 INGInious-0.8.6/.github/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.042086 INGInious-0.8.6/.github/workflows/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1850 2023-04-26 09:42:50.000000 INGInious-0.8.6/.github/workflows/ci.yml
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      422 2022-02-09 10:08:57.000000 INGInious-0.8.6/.gitignore
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       22 2018-11-16 12:58:08.000000 INGInious-0.8.6/.landscape.yml
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    10147 2018-11-16 12:58:08.000000 INGInious-0.8.6/.pylintrc
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      156 2021-06-10 10:07:01.000000 INGInious-0.8.6/.readthedocs.yaml
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1581 2018-11-16 12:58:08.000000 INGInious-0.8.6/.travis.yml
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      622 2023-03-14 08:45:50.000000 INGInious-0.8.6/COPYRIGHTS
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.043087 INGInious-0.8.6/INGInious.egg-info/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3124 2023-04-26 10:06:30.000000 INGInious-0.8.6/INGInious.egg-info/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    40029 2023-04-26 10:06:31.000000 INGInious-0.8.6/INGInious.egg-info/SOURCES.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2023-04-26 10:06:30.000000 INGInious-0.8.6/INGInious.egg-info/dependency_links.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      658 2023-04-26 10:06:30.000000 INGInious-0.8.6/INGInious.egg-info/requires.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       10 2023-04-26 10:06:30.000000 INGInious-0.8.6/INGInious.egg-info/top_level.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    34764 2018-11-16 12:58:08.000000 INGInious-0.8.6/LICENSE
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      440 2018-11-16 12:58:08.000000 INGInious-0.8.6/MANIFEST.in
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3124 2023-04-26 10:06:31.163087 INGInious-0.8.6/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2688 2023-04-26 09:42:50.000000 INGInious-0.8.6/README.rst
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.030087 INGInious-0.8.6/base-containers/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.043087 INGInious-0.8.6/base-containers/base/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1927 2022-07-12 07:33:48.000000 INGInious-0.8.6/base-containers/base/Dockerfile
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      610 2018-11-16 12:58:08.000000 INGInious-0.8.6/base-containers/base/README.md
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.045086 INGInious-0.8.6/base-containers/base/bin/
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)    19095 2023-02-28 09:27:21.000000 INGInious-0.8.6/base-containers/base/bin/INGInious
+-rwxrwxr-x   0 anthony   (1000) anthony   (1000)     5040 2022-03-18 07:57:30.000000 INGInious-0.8.6/base-containers/base/bin/_run_student_intern
+-rwxrwxr-x   0 anthony   (1000) anthony   (1000)     1418 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/bin/archive
+-rwxrwxr-x   0 anthony   (1000) anthony   (1000)     2830 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/bin/feedback
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1088 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/bin/feedback-custom
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      549 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/bin/feedback-grade
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1306 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/bin/feedback-msg
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1533 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/bin/feedback-msg-tpl
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      812 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/bin/feedback-result
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      569 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/bin/feedback-state
+-rwxrwxr-x   0 anthony   (1000) anthony   (1000)     1180 2021-06-10 10:07:01.000000 INGInious-0.8.6/base-containers/base/bin/getinput
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1090 2022-02-08 16:02:58.000000 INGInious-0.8.6/base-containers/base/bin/inginious-ipython
+-rwxrwxr-x   0 anthony   (1000) anthony   (1000)     1066 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/bin/parsetemplate
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1064 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/bin/rst-code
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      737 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/bin/rst-image
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1277 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/bin/rst-indent
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1223 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/bin/rst-msgblock
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)     2752 2023-02-28 09:27:21.000000 INGInious-0.8.6/base-containers/base/bin/run_student
+-rwxrwxr-x   0 anthony   (1000) anthony   (1000)     2953 2022-02-09 08:29:26.000000 INGInious-0.8.6/base-containers/base/bin/ssh_student
+-rwxrwxr-x   0 anthony   (1000) anthony   (1000)      491 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/bin/tag
+-rwxrwxr-x   0 anthony   (1000) anthony   (1000)      623 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/bin/tag-set
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.047087 INGInious-0.8.6/base-containers/base/inginious_container_api/
+-rwxrwxr-x   0 anthony   (1000) anthony   (1000)       30 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/inginious_container_api/__init__.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     6616 2022-02-09 10:08:57.000000 INGInious-0.8.6/base-containers/base/inginious_container_api/feedback.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3400 2021-06-10 10:07:01.000000 INGInious-0.8.6/base-containers/base/inginious_container_api/input.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      789 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/inginious_container_api/lang.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1704 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/inginious_container_api/rst.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    16470 2023-02-28 09:27:21.000000 INGInious-0.8.6/base-containers/base/inginious_container_api/run_student.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      466 2021-04-26 06:37:40.000000 INGInious-0.8.6/base-containers/base/inginious_container_api/run_types.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3065 2022-02-09 08:57:05.000000 INGInious-0.8.6/base-containers/base/inginious_container_api/ssh_student.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    13519 2022-03-30 06:18:20.000000 INGInious-0.8.6/base-containers/base/inginious_container_api/utils.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.047087 INGInious-0.8.6/base-containers/default/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      210 2021-02-12 07:54:48.000000 INGInious-0.8.6/base-containers/default/Dockerfile
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      378 2018-11-16 12:58:08.000000 INGInious-0.8.6/base-containers/default/README.md
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2068 2021-06-10 10:07:01.000000 INGInious-0.8.6/configuration.example.yaml
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.049087 INGInious-0.8.6/doc/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6910 2018-11-16 12:58:08.000000 INGInious-0.8.6/doc/Makefile
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.031087 INGInious-0.8.6/doc/admin_doc/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.050087 INGInious-0.8.6/doc/admin_doc/commands_doc/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2703 2022-02-09 10:08:57.000000 INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-agent-docker.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      824 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-agent-mcq.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1192 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-autotest.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      881 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-backend.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      336 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-container-update.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      407 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-database-update.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      569 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-install.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1297 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-synchronize.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      980 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-webapp.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      980 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-webdav.rst
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.051087 INGInious-0.8.6/doc/admin_doc/install_doc/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    18632 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/admin_doc/install_doc/config_reference.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     9220 2023-03-28 13:39:50.000000 INGInious-0.8.6/doc/admin_doc/install_doc/create_container.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    21186 2023-04-26 09:42:50.000000 INGInious-0.8.6/doc/admin_doc/install_doc/installation.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2094 2022-02-09 08:57:05.000000 INGInious-0.8.6/doc/admin_doc/install_doc/other_oci_runtimes_support.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1350 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/admin_doc/install_doc/static_pages.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3847 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/admin_doc/install_doc/troubleshooting.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1342 2022-02-09 08:22:39.000000 INGInious-0.8.6/doc/admin_doc/install_doc/updating.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1172 2023-04-26 09:42:50.000000 INGInious-0.8.6/doc/admin_documentation.rst
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.054087 INGInious-0.8.6/doc/api_doc/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      506 2018-11-16 12:58:08.000000 INGInious-0.8.6/doc/api_doc/inginious.agent.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      336 2018-11-16 12:58:08.000000 INGInious-0.8.6/doc/api_doc/inginious.backend.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      715 2018-11-16 12:58:08.000000 INGInious-0.8.6/doc/api_doc/inginious.client.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      414 2022-03-18 07:57:30.000000 INGInious-0.8.6/doc/api_doc/inginious.common.filesystems.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1495 2022-03-18 07:57:30.000000 INGInious-0.8.6/doc/api_doc/inginious.common.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      692 2018-11-16 12:58:08.000000 INGInious-0.8.6/doc/api_doc/inginious.common.task_file_readers.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      570 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/api_doc/inginious.common.tests.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1286 2018-11-16 12:58:08.000000 INGInious-0.8.6/doc/api_doc/inginious.frontend.pages.api.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2429 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/api_doc/inginious.frontend.pages.course_admin.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1474 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/api_doc/inginious.frontend.pages.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      664 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/api_doc/inginious.frontend.plugins.auth.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1146 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/api_doc/inginious.frontend.plugins.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      212 2018-11-16 12:58:08.000000 INGInious-0.8.6/doc/api_doc/inginious.frontend.plugins.scoreboard.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3200 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/api_doc/inginious.frontend.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1483 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/api_doc/inginious.frontend.tests.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      324 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/api_doc/inginious.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    10661 2023-03-14 08:45:50.000000 INGInious-0.8.6/doc/conf.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.031087 INGInious-0.8.6/doc/dev_doc/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.054087 INGInious-0.8.6/doc/dev_doc/extensions_doc/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1902 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/dev_doc/extensions_doc/how_to_extend.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      753 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/dev_doc/extensions_doc/i18n.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    16600 2023-04-26 09:42:50.000000 INGInious-0.8.6/doc/dev_doc/extensions_doc/plugins.rst
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.057087 INGInious-0.8.6/doc/dev_doc/internals_doc/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2083 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/dev_doc/internals_doc/architectures.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2309 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/dev_doc/internals_doc/exercises.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1217 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/dev_doc/internals_doc/frontend.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       37 2023-04-26 09:42:50.000000 INGInious-0.8.6/doc/dev_doc/internals_doc/groupes_audiences.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    71784 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/dev_doc/internals_doc/inginious_arch.png
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    97918 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/dev_doc/internals_doc/inginious_arch_docker.png
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)   119437 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/dev_doc/internals_doc/inginious_arch_full.png
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    20901 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/dev_doc/internals_doc/submission_evaluation_docker.png
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    51028 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/dev_doc/internals_doc/submission_workflow.png
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     5607 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/dev_doc/internals_doc/submissions.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3834 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/dev_doc/internals_doc/understand_inginious.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      618 2023-04-26 09:42:50.000000 INGInious-0.8.6/doc/developer_documentation.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      297 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/index.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    11703 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/logo_rtd.svg
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6707 2018-11-16 12:58:08.000000 INGInious-0.8.6/doc/make.bat
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.060087 INGInious-0.8.6/doc/teacher_doc/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4806 2018-11-16 12:58:08.000000 INGInious-0.8.6/doc/teacher_doc/best_practices.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      952 2021-04-26 06:37:40.000000 INGInious-0.8.6/doc/teacher_doc/common.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    11047 2023-04-26 09:42:50.000000 INGInious-0.8.6/doc/teacher_doc/course_admin.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     4106 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/teacher_doc/course_description.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1093 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/teacher_doc/course_tuto.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      921 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/teacher_doc/courses.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1168 2022-02-08 16:02:58.000000 INGInious-0.8.6/doc/teacher_doc/inginious_container_api.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3025 2022-03-18 07:57:30.000000 INGInious-0.8.6/doc/teacher_doc/lti.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1856 2021-04-26 06:37:40.000000 INGInious-0.8.6/doc/teacher_doc/random.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5807 2022-08-11 06:40:58.000000 INGInious-0.8.6/doc/teacher_doc/rst.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    34270 2023-04-26 09:42:50.000000 INGInious-0.8.6/doc/teacher_doc/run_file.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      764 2018-11-16 12:58:08.000000 INGInious-0.8.6/doc/teacher_doc/share_files.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      975 2018-11-16 12:58:08.000000 INGInious-0.8.6/doc/teacher_doc/system_files.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     9474 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/teacher_doc/task_file.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     5397 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/teacher_doc/task_tuto.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      214 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/teacher_doc/tasks.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1676 2018-11-16 12:58:08.000000 INGInious-0.8.6/doc/teacher_doc/testing.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3060 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/teacher_doc/translating.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      197 2022-02-09 08:22:39.000000 INGInious-0.8.6/doc/teacher_documentation.rst
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     5111 2021-06-10 10:07:01.000000 INGInious-0.8.6/doc/what_is_inginious.rst
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.060087 INGInious-0.8.6/inginious/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      709 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/__init__.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.060087 INGInious-0.8.6/inginious/agent/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    11964 2023-04-26 09:44:11.000000 INGInious-0.8.6/inginious/agent/__init__.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.061087 INGInious-0.8.6/inginious/agent/docker_agent/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    50851 2023-04-26 09:44:11.000000 INGInious-0.8.6/inginious/agent/docker_agent/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    13345 2023-03-28 13:39:50.000000 INGInious-0.8.6/inginious/agent/docker_agent/_docker_interface.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      858 2023-03-28 13:39:50.000000 INGInious-0.8.6/inginious/agent/docker_agent/_docker_runtime.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4597 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/agent/docker_agent/_timeout_watcher.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.061087 INGInious-0.8.6/inginious/agent/mcq_agent/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6721 2022-08-30 07:08:17.000000 INGInious-0.8.6/inginious/agent/mcq_agent/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       42 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/agent/mcq_agent/babel.cfg
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.061087 INGInious-0.8.6/inginious/agent/mcq_agent/i18n/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.031087 INGInious-0.8.6/inginious/agent/mcq_agent/i18n/de/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.061087 INGInious-0.8.6/inginious/agent/mcq_agent/i18n/de/LC_MESSAGES/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1037 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/agent/mcq_agent/i18n/de/LC_MESSAGES/messages.mo
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1505 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/agent/mcq_agent/i18n/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.031087 INGInious-0.8.6/inginious/agent/mcq_agent/i18n/es/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.062087 INGInious-0.8.6/inginious/agent/mcq_agent/i18n/es/LC_MESSAGES/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1051 2022-02-09 10:08:57.000000 INGInious-0.8.6/inginious/agent/mcq_agent/i18n/es/LC_MESSAGES/messages.mo
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1525 2022-02-09 10:08:57.000000 INGInious-0.8.6/inginious/agent/mcq_agent/i18n/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.031087 INGInious-0.8.6/inginious/agent/mcq_agent/i18n/fr/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.062087 INGInious-0.8.6/inginious/agent/mcq_agent/i18n/fr/LC_MESSAGES/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1059 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/agent/mcq_agent/i18n/fr/LC_MESSAGES/messages.mo
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1530 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/agent/mcq_agent/i18n/fr/LC_MESSAGES/messages.po
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1109 2021-04-26 06:37:40.000000 INGInious-0.8.6/inginious/agent/mcq_agent/i18n/messages.pot
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.062087 INGInious-0.8.6/inginious/backend/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/backend/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    22389 2023-04-26 09:44:11.000000 INGInious-0.8.6/inginious/backend/backend.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1894 2022-02-09 08:29:26.000000 INGInious-0.8.6/inginious/backend/topic_priority_queue.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.063087 INGInious-0.8.6/inginious/client/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/client/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     9874 2023-02-23 07:55:28.000000 INGInious-0.8.6/inginious/client/_zeromq_client.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    16216 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/client/client.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2541 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/client/client_buffer.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1271 2021-04-26 06:37:40.000000 INGInious-0.8.6/inginious/client/client_sync.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.065087 INGInious-0.8.6/inginious/common/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      242 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/common/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2607 2023-02-23 07:55:28.000000 INGInious-0.8.6/inginious/common/asyncio_utils.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2458 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/common/babel.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     4805 2022-03-30 09:10:41.000000 INGInious-0.8.6/inginious/common/base.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3124 2021-04-26 06:37:40.000000 INGInious-0.8.6/inginious/common/custom_yaml.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4275 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/common/entrypoints.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      701 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/common/exceptions.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.065087 INGInious-0.8.6/inginious/common/filesystems/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     5291 2022-03-18 07:57:30.000000 INGInious-0.8.6/inginious/common/filesystems/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6096 2022-12-14 10:14:50.000000 INGInious-0.8.6/inginious/common/filesystems/local.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2131 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/common/log.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    14490 2023-04-26 09:44:11.000000 INGInious-0.8.6/inginious/common/messages.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2672 2021-04-26 06:37:40.000000 INGInious-0.8.6/inginious/common/tags.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.066087 INGInious-0.8.6/inginious/common/task_file_readers/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      224 2020-08-25 08:18:47.000000 INGInious-0.8.6/inginious/common/task_file_readers/__init__.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      755 2020-08-25 08:18:47.000000 INGInious-0.8.6/inginious/common/task_file_readers/abstract_reader.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      650 2020-08-25 08:18:47.000000 INGInious-0.8.6/inginious/common/task_file_readers/yaml_reader.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    14652 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/common/tasks_problems.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.066087 INGInious-0.8.6/inginious/common/tests/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5009 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/common/tests/TestBase.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2823 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/common/tests/TestCustomYaml.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      206 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/common/tests/__init__.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    12982 2022-02-09 10:08:57.000000 INGInious-0.8.6/inginious/common/tests/test_filesystem_local.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.069087 INGInious-0.8.6/inginious/frontend/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      214 2022-03-18 08:08:05.000000 INGInious-0.8.6/inginious/frontend/__init__.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     5943 2022-02-09 08:22:39.000000 INGInious-0.8.6/inginious/frontend/accessible_time.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    15300 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/app.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4770 2023-04-20 07:54:08.000000 INGInious-0.8.6/inginious/frontend/arch_helper.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      138 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/babel.cfg
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    10782 2022-03-18 08:08:05.000000 INGInious-0.8.6/inginious/frontend/course_factory.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    11693 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/courses.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.070087 INGInious-0.8.6/inginious/frontend/environment_types/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1022 2023-04-26 09:44:11.000000 INGInious-0.8.6/inginious/frontend/environment_types/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      447 2023-04-26 09:44:11.000000 INGInious-0.8.6/inginious/frontend/environment_types/docker.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      920 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/environment_types/env_type.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2067 2023-04-26 09:44:11.000000 INGInious-0.8.6/inginious/frontend/environment_types/generic_docker_oci_runtime.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      395 2023-04-26 09:44:11.000000 INGInious-0.8.6/inginious/frontend/environment_types/kata.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      408 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/environment_types/mcq.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      393 2023-04-26 09:44:11.000000 INGInious-0.8.6/inginious/frontend/environment_types/nvidia.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.071087 INGInious-0.8.6/inginious/frontend/flask/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      157 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/flask/__init__.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)       43 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/flask/mail.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    11759 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/flask/mapping.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     5564 2022-02-09 10:08:57.000000 INGInious-0.8.6/inginious/frontend/flask/mongo_sessions.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.071087 INGInious-0.8.6/inginious/frontend/i18n/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.032086 INGInious-0.8.6/inginious/frontend/i18n/de/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.071087 INGInious-0.8.6/inginious/frontend/i18n/de/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    25694 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   110889 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.032086 INGInious-0.8.6/inginious/frontend/i18n/el/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.071087 INGInious-0.8.6/inginious/frontend/i18n/el/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    29887 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   119743 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.032086 INGInious-0.8.6/inginious/frontend/i18n/es/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.072087 INGInious-0.8.6/inginious/frontend/i18n/es/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    47593 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   132063 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.032086 INGInious-0.8.6/inginious/frontend/i18n/fr/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.072087 INGInious-0.8.6/inginious/frontend/i18n/fr/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    60340 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   127508 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.032086 INGInious-0.8.6/inginious/frontend/i18n/he/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.072087 INGInious-0.8.6/inginious/frontend/i18n/he/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    68397 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/he/LC_MESSAGES/messages.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   130391 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/he/LC_MESSAGES/messages.po
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    99891 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/messages.pot
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.032086 INGInious-0.8.6/inginious/frontend/i18n/nl/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.073087 INGInious-0.8.6/inginious/frontend/i18n/nl/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4937 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/nl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   102119 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/nl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.032086 INGInious-0.8.6/inginious/frontend/i18n/pt/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.073087 INGInious-0.8.6/inginious/frontend/i18n/pt/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    24190 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   119920 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.032086 INGInious-0.8.6/inginious/frontend/i18n/pt_BR/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.073087 INGInious-0.8.6/inginious/frontend/i18n/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      530 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/i18n/pt_BR/LC_MESSAGES/messages.mo
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.032086 INGInious-0.8.6/inginious/frontend/i18n/vi/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.074087 INGInious-0.8.6/inginious/frontend/i18n/vi/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    34450 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/vi/LC_MESSAGES/messages.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   118219 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/vi/LC_MESSAGES/messages.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.032086 INGInious-0.8.6/inginious/frontend/i18n/wa/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.074087 INGInious-0.8.6/inginious/frontend/i18n/wa/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2170 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/wa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   100743 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/i18n/wa/LC_MESSAGES/messages.po
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    27989 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/installer.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      639 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/l10n_manager.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     4924 2021-02-19 11:28:54.000000 INGInious-0.8.6/inginious/frontend/lti_outcome_manager.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2061 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/lti_request_validator.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      777 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/lti_tool_provider.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3385 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/marketplace_courses.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.076087 INGInious-0.8.6/inginious/frontend/pages/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      196 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/pages/__init__.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.077087 INGInious-0.8.6/inginious/frontend/pages/admin/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      199 2022-03-30 09:10:41.000000 INGInious-0.8.6/inginious/frontend/pages/admin/__init__.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2944 2022-03-30 09:10:41.000000 INGInious-0.8.6/inginious/frontend/pages/admin/admin.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.078087 INGInious-0.8.6/inginious/frontend/pages/api/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      191 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/pages/api/__init__.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     6726 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/pages/api/_api_page.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1476 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/pages/api/auth_methods.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1615 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/pages/api/authentication.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2946 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/pages/api/courses.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     8534 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/pages/api/submissions.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4517 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/pages/api/tasks.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4502 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/pages/course.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.080087 INGInious-0.8.6/inginious/frontend/pages/course_admin/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      189 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/pages/course_admin/__init__.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     5328 2022-02-09 10:08:57.000000 INGInious-0.8.6/inginious/frontend/pages/course_admin/audience_edit.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    10305 2022-03-30 09:10:41.000000 INGInious-0.8.6/inginious/frontend/pages/course_admin/danger_zone.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1425 2023-03-23 10:48:36.000000 INGInious-0.8.6/inginious/frontend/pages/course_admin/search_user.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5138 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/pages/course_admin/settings.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    13926 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/pages/course_admin/statistics.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2690 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/pages/course_admin/student_info.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    18777 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/pages/course_admin/student_list.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3489 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/pages/course_admin/submission.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    12967 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/pages/course_admin/submissions.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2377 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/pages/course_admin/tags.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    13627 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/pages/course_admin/task_edit.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    11817 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/pages/course_admin/task_edit_file.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5408 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/pages/course_admin/task_list.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    16859 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/pages/course_admin/utils.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1811 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/pages/course_register.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1240 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/pages/courselist.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     4503 2022-03-18 07:57:30.000000 INGInious-0.8.6/inginious/frontend/pages/group.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      813 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/pages/index.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    12033 2022-02-09 10:08:57.000000 INGInious-0.8.6/inginious/frontend/pages/lti.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      571 2021-07-15 06:35:04.000000 INGInious-0.8.6/inginious/frontend/pages/maintenance.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3957 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/pages/marketplace.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2326 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/pages/marketplace_course.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3020 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/pages/mycourses.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.081086 INGInious-0.8.6/inginious/frontend/pages/preferences/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      179 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/pages/preferences/__init__.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2090 2022-03-30 09:10:41.000000 INGInious-0.8.6/inginious/frontend/pages/preferences/bindings.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1950 2022-03-30 09:10:41.000000 INGInious-0.8.6/inginious/frontend/pages/preferences/delete.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     6131 2022-03-30 09:10:41.000000 INGInious-0.8.6/inginious/frontend/pages/preferences/profile.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1396 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/pages/preferences/utils.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      981 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/pages/queue.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     9157 2022-03-30 09:10:41.000000 INGInious-0.8.6/inginious/frontend/pages/register.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3533 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/pages/social.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    22133 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/pages/tasks.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    14567 2022-08-03 10:55:31.000000 INGInious-0.8.6/inginious/frontend/pages/utils.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    13757 2022-12-14 10:19:50.000000 INGInious-0.8.6/inginious/frontend/parsable_text.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4724 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/plugin_manager.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.081086 INGInious-0.8.6/inginious/frontend/plugins/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      203 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/plugins/__init__.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.082087 INGInious-0.8.6/inginious/frontend/plugins/auth/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      180 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__init__.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.085087 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      210 2022-01-01 20:58:44.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      200 2021-02-26 16:21:15.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      204 2021-02-26 10:55:03.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      208 2021-04-21 06:41:19.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      208 2021-02-26 10:50:17.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3416 2023-04-26 09:46:50.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/google_auth.cpython-310.pyc
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3372 2021-12-16 14:52:36.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/google_auth.cpython-36.pyc
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3442 2023-02-28 09:13:57.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/google_auth.cpython-38.pyc
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3426 2021-06-18 12:47:24.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/google_auth.cpython-39.pyc
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6216 2023-04-26 09:46:50.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-310.pyc
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6129 2021-12-16 14:52:36.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-36.pyc
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     6096 2021-03-01 12:53:51.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-37.pyc
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6226 2023-02-28 09:14:23.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-38.pyc
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6232 2021-10-25 13:22:36.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-39.pyc
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6434 2023-04-26 09:46:50.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-310.pyc
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6394 2021-12-16 14:52:36.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-36.pyc
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     6389 2021-03-01 13:00:13.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-37.pyc
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6466 2023-02-28 09:13:57.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-38.pyc
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6464 2021-06-18 12:47:24.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-39.pyc
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1691 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/custom_auth_form.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4075 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/facebook_auth.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2665 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/github_auth.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2979 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/google_auth.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7358 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/ldap_auth.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3082 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/linkedin_auth.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7053 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/saml2_auth.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4317 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/plugins/auth/twitter_auth.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.086087 INGInious-0.8.6/inginious/frontend/plugins/contests/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    11265 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/plugins/contests/__init__.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.087087 INGInious-0.8.6/inginious/frontend/plugins/contests/__pycache__/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7900 2023-04-26 09:46:50.000000 INGInious-0.8.6/inginious/frontend/plugins/contests/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     7995 2021-03-01 12:53:52.000000 INGInious-0.8.6/inginious/frontend/plugins/contests/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7976 2023-02-28 09:13:57.000000 INGInious-0.8.6/inginious/frontend/plugins/contests/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     7930 2021-04-29 09:45:18.000000 INGInious-0.8.6/inginious/frontend/plugins/contests/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     5410 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/plugins/contests/admin.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1671 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/plugins/contests/course_menu.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     4223 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/plugins/contests/scoreboard.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.087087 INGInious-0.8.6/inginious/frontend/plugins/demo/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      583 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/plugins/demo/__init__.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.087087 INGInious-0.8.6/inginious/frontend/plugins/git_repo/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     4807 2020-08-25 08:18:47.000000 INGInious-0.8.6/inginious/frontend/plugins/git_repo/__init__.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.087087 INGInious-0.8.6/inginious/frontend/plugins/ltibestsubmission/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3438 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/plugins/ltibestsubmission/__init__.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.088087 INGInious-0.8.6/inginious/frontend/plugins/scoreboard/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     9753 2022-07-12 06:51:08.000000 INGInious-0.8.6/inginious/frontend/plugins/scoreboard/__init__.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.089087 INGInious-0.8.6/inginious/frontend/plugins/scoreboard/__pycache__/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     6649 2022-03-30 09:15:04.000000 INGInious-0.8.6/inginious/frontend/plugins/scoreboard/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     6798 2021-03-01 12:53:52.000000 INGInious-0.8.6/inginious/frontend/plugins/scoreboard/__pycache__/__init__.cpython-37.pyc
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     6738 2021-04-21 06:41:19.000000 INGInious-0.8.6/inginious/frontend/plugins/scoreboard/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     6731 2021-04-29 09:45:18.000000 INGInious-0.8.6/inginious/frontend/plugins/scoreboard/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      354 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/plugins/scoreboard/course_menu.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1220 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/plugins/scoreboard/main.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1418 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/plugins/scoreboard/scoreboard.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      425 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/plugins/scoreboard/task_menu.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.089087 INGInious-0.8.6/inginious/frontend/plugins/simple_grader/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     6106 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/plugins/simple_grader/__init__.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.089087 INGInious-0.8.6/inginious/frontend/plugins/task_editor_hook_example/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1363 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/plugins/task_editor_hook_example/__init__.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      816 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/plugins/task_editor_hook_example/example_tab_2.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.090087 INGInious-0.8.6/inginious/frontend/plugins/task_file_readers/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      212 2020-08-25 08:18:47.000000 INGInious-0.8.6/inginious/frontend/plugins/task_file_readers/__init__.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      976 2020-08-25 08:18:47.000000 INGInious-0.8.6/inginious/frontend/plugins/task_file_readers/json_reader.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.090087 INGInious-0.8.6/inginious/frontend/plugins/upcoming_tasks/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6301 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/plugins/upcoming_tasks/__init__.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.090087 INGInious-0.8.6/inginious/frontend/plugins/upcoming_tasks/templates/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4945 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/plugins/upcoming_tasks/templates/coming_tasks.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      198 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/plugins/upcoming_tasks/templates/main_menu.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      358 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/plugins/upcoming_tasks/templates/upcoming.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2803 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/plugins/upcoming_tasks/templates/upcoming_task_list.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.039086 INGInious-0.8.6/inginious/frontend/static/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.091087 INGInious-0.8.6/inginious/frontend/static/css/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    11071 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/static/css/INGInious.css
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3518 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/static/css/INGInious.less
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     9063 2021-04-26 06:37:40.000000 INGInious-0.8.6/inginious/frontend/static/css/bootstrap-datetimepicker.min.css
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   134084 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/static/css/bootstrap.min.css
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     8217 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/css/codemirror.css
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     9044 2022-03-30 06:18:20.000000 INGInious-0.8.6/inginious/frontend/static/css/common.less
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    31000 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/css/font-awesome.min.css
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     7996 2021-06-18 12:47:19.000000 INGInious-0.8.6/inginious/frontend/static/css/lti.css
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      254 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/static/css/lti.less
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    11150 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/static/css/selectize.css
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.096087 INGInious-0.8.6/inginious/frontend/static/fonts/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   134808 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/fonts/FontAwesome.otf
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   165742 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   444379 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   165548 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    98024 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    77160 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    20127 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   108738 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    45404 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    23424 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    18028 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.100087 INGInious-0.8.6/inginious/frontend/static/icons/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1856 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-114x114.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1844 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-120x120.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2259 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-144x144.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2312 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-152x152.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1020 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-57x57.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1101 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-60x60.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1241 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-72x72.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1294 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-76x76.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2810 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-precomposed.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2312 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      371 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/browserconfig.xml
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3475 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/favicon-160x160.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      535 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/favicon-16x16.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2870 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/favicon-196x196.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      928 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/favicon-32x32.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2226 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/favicon-96x96.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    15086 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/favicon.ico
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4358 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/google-icon.svg
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3186 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/mstile-144x144.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2135 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/mstile-150x150.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1829 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/mstile-310x150.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3819 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/mstile-310x310.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1970 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/mstile-70x70.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2531 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/wb.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1573 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/icons/wb.svg
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.101087 INGInious-0.8.6/inginious/frontend/static/images/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5244 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/images/header.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6681 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/images/inginious_full.svg
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6531 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/images/inginious_full_logo_only.svg
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4730 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/images/inginious_horiz.svg
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4728 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/images/inginious_vert.svg
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    14493 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/images/logo.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    13380 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/images/logo_maintenance.png
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.103087 INGInious-0.8.6/inginious/frontend/static/js/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2445 2022-03-30 09:10:41.000000 INGInious-0.8.6/inginious/frontend/static/js/admin.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   638597 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/static/js/all-minified.js
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3828 2022-02-09 10:08:57.000000 INGInious-0.8.6/inginious/frontend/static/js/audiences.js
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2838 2021-04-26 06:37:40.000000 INGInious-0.8.6/inginious/frontend/static/js/checked-list-group.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.103087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1107 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/LICENSE
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   205623 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/codemirror.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.104087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.104087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/apl/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4736 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/apl/apl.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2179 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/apl/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.104087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/asciiarmor/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2378 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/asciiarmor/asciiarmor.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1289 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/asciiarmor/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.105087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/asn.1/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7735 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/asn.1/asn.1.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2222 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/asn.1/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.105087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/asterisk/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7437 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/asterisk/asterisk.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4591 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/asterisk/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.105087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/brainfuck/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2174 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/brainfuck/brainfuck.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3338 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/brainfuck/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.106087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/clike/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    31062 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/clike/clike.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    10105 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/clike/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    28518 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/clike/scala.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.107087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/clojure/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    16005 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/clojure/clojure.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2550 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/clojure/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.107087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/cmake/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2600 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/cmake/cmake.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4152 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/cmake/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.107087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/cobol/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    10288 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/cobol/cobol.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     8084 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/cobol/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.108087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/coffeescript/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     9884 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/coffeescript/coffeescript.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    22402 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/coffeescript/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.108087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/commonlisp/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4569 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/commonlisp/commonlisp.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6691 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/commonlisp/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.108087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/crystal/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    12818 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/crystal/crystal.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2605 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/crystal/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.110087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/css/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    37613 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/css/css.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2780 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/css/gss.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      460 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/css/gss_test.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1911 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/css/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4066 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/css/less.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1871 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/css/less_test.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2742 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/css/scss.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3124 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/css/scss_test.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.110087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/cypher/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6362 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/cypher/cypher.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1908 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/cypher/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.110087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/d/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7566 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/d/d.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6332 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/d/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.111087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dart/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5124 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dart/dart.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1627 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dart/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.111087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/diff/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1138 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/diff/diff.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4409 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/diff/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.111087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/django/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    11791 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/django/django.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2077 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/django/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.112087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dockerfile/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2221 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dockerfile/dockerfile.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2267 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dockerfile/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.112087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dtd/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4814 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dtd/dtd.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3337 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dtd/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.112087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dylan/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    10112 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dylan/dylan.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    13032 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dylan/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.113087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ebnf/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6085 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ebnf/ebnf.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2450 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ebnf/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.114087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ecl/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     8843 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ecl/ecl.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1409 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ecl/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.114087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/eiffel/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3744 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/eiffel/eiffel.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    13198 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/eiffel/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.115087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/elm/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5552 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/elm/elm.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1640 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/elm/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.115087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/erlang/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    18887 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/erlang/erlang.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2168 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/erlang/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.115087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/factor/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3565 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/factor/factor.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2024 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/factor/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.116087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/fcl/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4703 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/fcl/fcl.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3091 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/fcl/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.116087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/forth/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5230 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/forth/forth.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1783 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/forth/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.116087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/fortran/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     8686 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/fortran/fortran.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2492 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/fortran/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.117087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/gas/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     8886 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/gas/gas.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1840 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/gas/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.117087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/gfm/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5103 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/gfm/gfm.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2583 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/gfm/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.117087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/gherkin/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    13257 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/gherkin/gherkin.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1566 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/gherkin/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.118087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/go/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6030 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/go/go.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2174 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/go/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.118087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/groovy/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7904 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/groovy/groovy.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2177 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/groovy/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.118087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haml/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5353 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haml/haml.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2071 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haml/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.118087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/handlebars/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2172 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/handlebars/handlebars.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2196 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/handlebars/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.119087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haskell/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     8109 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haskell/haskell.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2194 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haskell/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.119087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haskell-literate/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1390 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haskell-literate/haskell-literate.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     9381 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haskell-literate/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.119087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haxe/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    17563 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haxe/haxe.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2577 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haxe/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.120087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/htmlembedded/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1417 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/htmlembedded/htmlembedded.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2086 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/htmlembedded/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.120087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/htmlmixed/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5611 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/htmlmixed/htmlmixed.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3434 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/htmlmixed/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.120087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/http/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2795 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/http/http.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1393 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/http/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.121087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/idl/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    14889 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/idl/idl.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1633 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/idl/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     8286 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/index.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.121087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/javascript/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4193 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/javascript/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    31566 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/javascript/javascript.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2150 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/javascript/json-ld.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1557 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/javascript/typescript.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.122087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/jinja2/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1755 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/jinja2/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4279 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/jinja2/jinja2.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.122087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/jsx/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2410 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/jsx/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5195 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/jsx/jsx.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.122087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/julia/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2375 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/julia/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    12089 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/julia/julia.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.123087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/livescript/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     9843 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/livescript/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7668 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/livescript/livescript.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.123087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/lua/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2073 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/lua/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5950 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/lua/lua.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.123087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/markdown/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    10957 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/markdown/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    25671 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/markdown/markdown.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.124087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mathematica/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2254 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mathematica/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5612 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mathematica/mathematica.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.124087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mbox/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1293 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mbox/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3649 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mbox/mbox.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    15098 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/meta.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.124087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mirc/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5798 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mirc/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    10077 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mirc/mirc.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.125087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mllike/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4436 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mllike/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5097 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mllike/mllike.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.125087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/modelica/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2007 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/modelica/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6930 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/modelica/modelica.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.126087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mscgen/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4310 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mscgen/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6820 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mscgen/mscgen.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3795 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mscgen/mscgen_test.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3255 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mscgen/msgenny_test.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4006 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mscgen/xu_test.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.126087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mumps/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2608 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mumps/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5354 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mumps/mumps.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.126087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/nginx/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5239 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/nginx/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    10164 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/nginx/nginx.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.127087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/nsis/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1764 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/nsis/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7642 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/nsis/nsis.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.127087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ntriples/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1357 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ntriples/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6643 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ntriples/ntriples.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.127087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/octave/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1805 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/octave/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4522 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/octave/octave.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.128087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/oz/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1389 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/oz/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6665 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/oz/oz.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.128087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pascal/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1440 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pascal/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3055 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pascal/pascal.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.128087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pegjs/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1890 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pegjs/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3577 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pegjs/pegjs.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.128087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/perl/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1542 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/perl/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    56135 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/perl/perl.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.129087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/php/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1999 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/php/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    18224 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/php/php.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.129087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pig/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1475 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pig/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5810 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pig/pig.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.130087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/powershell/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7372 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/powershell/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    12896 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/powershell/powershell.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.130087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/properties/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1555 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/properties/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2171 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/properties/properties.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.130087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/protobuf/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1680 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/protobuf/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2113 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/protobuf/protobuf.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.131087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pug/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2489 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pug/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    16046 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pug/pug.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.131087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/puppet/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3260 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/puppet/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7568 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/puppet/puppet.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.131087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/python/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5950 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/python/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    12479 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/python/python.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.132087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/q/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     8961 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/q/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6593 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/q/q.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.132087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/r/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2518 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/r/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6396 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/r/r.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.132087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rpm/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.132087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rpm/changes/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2180 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rpm/changes/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4623 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rpm/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3775 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rpm/rpm.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.133087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rst/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    17769 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rst/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    17547 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rst/rst.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.133087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ruby/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5749 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ruby/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    10516 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ruby/ruby.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.133087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rust/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1532 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rust/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3025 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rust/rust.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.134087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sas/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1854 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sas/index.html
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)    15424 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sas/sas.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.134087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sass/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1631 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sass/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    11509 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sass/sass.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.134087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/scheme/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2554 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/scheme/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    13437 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/scheme/scheme.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.135087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/shell/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1745 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/shell/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4002 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/shell/shell.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.135087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sieve/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2335 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sieve/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4284 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sieve/sieve.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.135087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/slim/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2920 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/slim/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    18026 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/slim/slim.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.135087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/smalltalk/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1904 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/smalltalk/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4543 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/smalltalk/smalltalk.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.136087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/smarty/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3973 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/smarty/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6828 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/smarty/smarty.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.136087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/solr/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1365 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/solr/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2672 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/solr/solr.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.136087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/soy/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1939 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/soy/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    12239 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/soy/soy.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.137087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sparql/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1773 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sparql/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6335 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sparql/sparql.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.137087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/spreadsheet/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1392 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/spreadsheet/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3139 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/spreadsheet/spreadsheet.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.137087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sql/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2991 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sql/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    37351 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sql/sql.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.138087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/stex/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4132 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/stex/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6932 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/stex/stex.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.138087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/stylus/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2472 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/stylus/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    42256 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/stylus/stylus.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.138087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/swift/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2085 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/swift/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7168 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/swift/swift.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.139087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tcl/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6297 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tcl/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4920 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tcl/tcl.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.139087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/textile/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4347 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/textile/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    13835 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/textile/textile.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.139087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tiddlywiki/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4579 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tiddlywiki/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      220 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tiddlywiki/tiddlywiki.css
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     8510 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tiddlywiki/tiddlywiki.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.140087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tiki/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1745 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tiki/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      439 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tiki/tiki.css
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     8462 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tiki/tiki.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.140087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/toml/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1840 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/toml/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2897 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/toml/toml.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.140087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tornado/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1803 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tornado/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2496 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tornado/tornado.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.141087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/troff/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4465 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/troff/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2392 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/troff/troff.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.141087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ttcn/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3490 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ttcn/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    10155 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ttcn/ttcn.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.141087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ttcn-cfg/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3605 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ttcn-cfg/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7857 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ttcn-cfg/ttcn-cfg.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.142087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/turtle/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1470 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/turtle/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4849 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/turtle/turtle.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.142087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/twig/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1370 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/twig/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4565 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/twig/twig.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.142087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vb/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1500 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vb/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     8734 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vb/vb.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.143087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vbscript/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1517 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vbscript/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    13793 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vbscript/vbscript.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.143087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/velocity/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3300 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/velocity/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7098 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/velocity/velocity.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.143087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/verilog/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2619 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/verilog/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    24588 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/verilog/verilog.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.144087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vhdl/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2486 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vhdl/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6704 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vhdl/vhdl.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.144087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vue/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2064 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vue/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2544 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vue/vue.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.144087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/webidl/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2171 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/webidl/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5784 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/webidl/webidl.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.145087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/xml/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2171 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/xml/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    12570 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/xml/xml.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.145087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/xquery/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     8609 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/xquery/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    14470 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/xquery/xquery.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.145087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/yacas/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2176 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/yacas/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5424 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/yacas/yacas.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.146087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/yaml/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2098 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/yaml/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3693 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/yaml/yaml.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.146087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/yaml-frontmatter/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3072 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/yaml-frontmatter/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2292 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/yaml-frontmatter/yaml-frontmatter.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.147087 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/z80/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1406 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/z80/index.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3577 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/z80/z80.js
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     6370 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/static/js/common.js
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     7286 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/static/js/groups.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.149087 INGInious-0.8.6/inginious/frontend/static/js/libs/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    42997 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/static/js/libs/Sortable.min.js
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    56581 2021-04-26 06:37:40.000000 INGInious-0.8.6/inginious/frontend/static/js/libs/bootstrap-datetimepicker.min.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    51039 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/static/js/libs/bootstrap.min.js
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)   158741 2021-04-26 06:37:40.000000 INGInious-0.8.6/inginious/frontend/static/js/libs/chart.min.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    15252 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/js/libs/jquery.form.min.js
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    86926 2021-04-26 06:37:40.000000 INGInious-0.8.6/inginious/frontend/static/js/libs/jquery.min.js
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     6542 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/static/js/libs/jquery.twbsPagination.min.js
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    51679 2021-04-26 06:37:40.000000 INGInious-0.8.6/inginious/frontend/static/js/libs/moment.min.js
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    20535 2021-04-26 06:37:40.000000 INGInious-0.8.6/inginious/frontend/static/js/libs/popper.min.js
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    41501 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/static/js/libs/selectize.min.js
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    50945 2021-04-26 06:37:40.000000 INGInious-0.8.6/inginious/frontend/static/js/libs/sentry-io-bundle.min.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    24394 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/static/js/studio.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    30954 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/static/js/task.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    16389 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/static/js/task_dispensers.js
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      727 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/static/js/webapp.js
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.039086 INGInious-0.8.6/inginious/frontend/static/plugins/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.150087 INGInious-0.8.6/inginious/frontend/static/plugins/contests/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1413 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/static/plugins/contests/contests.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4566 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/plugins/contests/jquery.countdown.min.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      996 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/static/plugins/contests/scoreboard.css
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    36374 2023-04-26 09:57:12.000000 INGInious-0.8.6/inginious/frontend/submission_manager.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.150087 INGInious-0.8.6/inginious/frontend/task_dispensers/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2312 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/task_dispensers/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3324 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/task_dispensers/combinatory_test.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2957 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/task_dispensers/toc.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7041 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/task_dispensers/util.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    13648 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/task_factory.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     9078 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/task_problems.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    11846 2023-04-26 09:54:11.000000 INGInious-0.8.6/inginious/frontend/tasks.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     6972 2022-02-09 08:21:51.000000 INGInious-0.8.6/inginious/frontend/template_helper.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.154087 INGInious-0.8.6/inginious/frontend/templates/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.154087 INGInious-0.8.6/inginious/frontend/templates/admin/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    12064 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/admin/admin_users.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2986 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/auth.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7753 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.156087 INGInious-0.8.6/inginious/frontend/templates/course_admin/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     9319 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/audience_edit.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    10121 2022-02-09 10:08:57.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/danger_zone.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.156087 INGInious-0.8.6/inginious/frontend/templates/course_admin/edit_tabs/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    14096 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/edit_tabs/basic.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3102 2023-04-26 09:44:11.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/edit_tabs/env_generic_docker_oci.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1846 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/edit_tabs/environment.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1776 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/edit_tabs/file_modals.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3675 2022-03-30 06:18:20.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/edit_tabs/files.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1085 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/edit_tabs/subproblems.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      913 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/menu.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    18882 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/settings.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    14180 2022-03-30 06:18:20.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/stats.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6499 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/student_info.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    28812 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/student_list.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5905 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/student_list_table.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7590 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/submission.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    12969 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/submissions.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    17267 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/submissions_query.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.156087 INGInious-0.8.6/inginious/frontend/templates/course_admin/subproblems/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2032 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/subproblems/code.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1332 2023-02-27 12:38:00.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/subproblems/file.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1050 2023-03-23 10:48:36.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/subproblems/match.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2826 2022-02-09 08:22:39.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/subproblems/multiple_choice.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2174 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/subproblems/multiple_choice_templates.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5141 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/tags.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.157087 INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1698 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/combinatory_test.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1225 2023-01-11 09:03:30.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/empty_section.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1795 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/section.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      894 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/section_config.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1352 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/section_menu.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1249 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/task_buttons.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2322 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/task_list.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1003 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/toc.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4564 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/util.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2481 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/util_delete_modal.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     9608 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/task_edit.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5346 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/task_list.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      476 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/course_admin/user_selection_box.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2034 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/course_register.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1573 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/course_unavailable.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     4040 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/courselist.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      493 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/forbidden.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     8084 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/group.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      667 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/internalerror.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    13580 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/layout.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2128 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/lti_bind.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1462 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/lti_login.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      572 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/maintenance.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     4826 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/marketplace.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2796 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/marketplace_course.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     5383 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/mycourses.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      492 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/notfound.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.158087 INGInious-0.8.6/inginious/frontend/templates/preferences/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3987 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/preferences/bindings.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2872 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/preferences/delete.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      469 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/preferences/menu.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     4723 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/preferences/profile.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4845 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/queue.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     5245 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/register.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      539 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/signin_button.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      271 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/static.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    25388 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/task.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.158087 INGInious-0.8.6/inginious/frontend/templates/task_dispensers/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3268 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/task_dispensers/task_list.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1819 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/task_dispensers/toc.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      513 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/task_unavailable.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.159087 INGInious-0.8.6/inginious/frontend/templates/tasks/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      528 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/tasks/code.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1039 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/tasks/file.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      307 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/tasks/match.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      644 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/tasks/multiple_choice.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      640 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/templates/tasks/single_line_code.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1430 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/templates/unregister_modal.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.160087 INGInious-0.8.6/inginious/frontend/tests/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    16896 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/tests/SeleniumFormatter.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6346 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/tests/SeleniumTest.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4326 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/tests/TestCourse.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3383 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/tests/TestLogin.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2639 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/tests/TestParsableText.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      972 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/tests/TestPluginManager.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7381 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/tests/TestTask.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1841 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/tests/TestTaskDisplay.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1975 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/tests/TestTaskSubmission.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious/frontend/tests/__init__.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.040087 INGInious-0.8.6/inginious/frontend/tests/tasks/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.160087 INGInious-0.8.6/inginious/frontend/tests/tasks/invalid_course/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)       72 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/tests/tasks/invalid_course/course.yaml
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.160087 INGInious-0.8.6/inginious/frontend/tests/tasks/test/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       73 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/tests/tasks/test/course.yaml
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.160087 INGInious-0.8.6/inginious/frontend/tests/tasks/test/task1/
+-rwxrwxr-x   0 anthony   (1000) anthony   (1000)       41 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/tests/tasks/test/task1/run
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      573 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/tests/tasks/test/task1/task.yaml
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.161087 INGInious-0.8.6/inginious/frontend/tests/tasks/test/task2/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      320 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/tests/tasks/test/task2/task.yaml
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.161087 INGInious-0.8.6/inginious/frontend/tests/tasks/test/task3/
+-rwxrwxr-x   0 anthony   (1000) anthony   (1000)       41 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/tests/tasks/test/task3/run
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      363 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/tests/tasks/test/task3/task.yaml
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.161087 INGInious-0.8.6/inginious/frontend/tests/tasks/test/task4/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      275 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/tests/tasks/test/task4/task.yaml
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.161087 INGInious-0.8.6/inginious/frontend/tests/tasks/test2/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)       79 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/tests/tasks/test2/course.yaml
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.161087 INGInious-0.8.6/inginious/frontend/tests/tasks/test2/task1/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      320 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/tests/tasks/test2/task1/task.yaml
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.161087 INGInious-0.8.6/inginious/frontend/tests/tasks/test2/task2/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      339 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/tests/tasks/test2/task2/task.yaml
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.162087 INGInious-0.8.6/inginious/frontend/tests/tasks/test2/task3/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      559 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/tests/tasks/test2/task3/task.yaml
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.162087 INGInious-0.8.6/inginious/frontend/tests/tasks/test2/task4/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      275 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/tests/tasks/test2/task4/task.yaml
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.162087 INGInious-0.8.6/inginious/frontend/tests/tasks/test3/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      122 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/tests/tasks/test3/course.json
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.162087 INGInious-0.8.6/inginious/frontend/tests/tasks/test3/invalid_task/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)       34 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/tests/tasks/test3/invalid_task/task.yaml
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    44783 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious/frontend/user_manager.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     9056 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious/frontend/webdav.py
+-rwxrwxr-x   0 anthony   (1000) anthony   (1000)     6462 2022-02-09 10:08:57.000000 INGInious-0.8.6/inginious-agent-docker
+-rwxrwxr-x   0 anthony   (1000) anthony   (1000)     3404 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious-agent-mcq
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)    12793 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious-autotest
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)     2162 2018-11-16 12:58:08.000000 INGInious-0.8.6/inginious-backend
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)      649 2023-04-26 09:42:50.000000 INGInious-0.8.6/inginious-install
+-rwxrwxr-x   0 anthony   (1000) anthony   (1000)     3981 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious-webapp
+-rwxrwxr-x   0 anthony   (1000) anthony   (1000)     3038 2021-06-10 10:07:01.000000 INGInious-0.8.6/inginious-webdav
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       38 2023-04-26 10:06:31.164087 INGInious-0.8.6/setup.cfg
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2441 2023-04-26 09:42:50.000000 INGInious-0.8.6/setup.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.040087 INGInious-0.8.6/utils/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.162087 INGInious-0.8.6/utils/container_update/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3199 2022-02-09 10:08:57.000000 INGInious-0.8.6/utils/container_update/inginious-container-update
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.162087 INGInious-0.8.6/utils/database_updater/
+-rwxrwxr-x   0 anthony   (1000) anthony   (1000)     4682 2022-02-09 10:08:57.000000 INGInious-0.8.6/utils/database_updater/inginious-database-update
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.163087 INGInious-0.8.6/utils/minify/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2728 2023-04-26 09:42:50.000000 INGInious-0.8.6/utils/minify/Gruntfile.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      452 2023-04-26 09:42:50.000000 INGInious-0.8.6/utils/minify/package.json
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      936 2018-11-16 12:58:08.000000 INGInious-0.8.6/utils/minify/watchers.xml
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-04-26 10:06:31.163087 INGInious-0.8.6/utils/sync/
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)     3220 2018-11-16 12:58:08.000000 INGInious-0.8.6/utils/sync/inginious-synchronize
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      349 2018-11-16 12:58:08.000000 INGInious-0.8.6/utils/sync/synchronize.json.example
```

### Comparing `INGInious-0.8.5/.github/workflows/ci.yml` & `INGInious-0.8.6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/.pylintrc` & `INGInious-0.8.6/.pylintrc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/.travis.yml` & `INGInious-0.8.6/.travis.yml`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/COPYRIGHTS` & `INGInious-0.8.6/COPYRIGHTS`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/INGInious.egg-info/PKG-INFO` & `INGInious-0.8.6/INGInious.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: INGInious
-Version: 0.8.5
+Version: 0.8.6
 Summary: An intelligent grader that allows secured and automated testing of code made by students.
 Home-page: https://github.com/UCL-INGI/INGInious
 Author: INGInious contributors
 Author-email: inginious@info.ucl.ac.be
 License: AGPL 3
 Provides-Extra: cgi
 Provides-Extra: ldap
```

### Comparing `INGInious-0.8.5/INGInious.egg-info/SOURCES.txt` & `INGInious-0.8.6/INGInious.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/INGInious.egg-info/requires.txt` & `INGInious-0.8.6/INGInious.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/LICENSE` & `INGInious-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/PKG-INFO` & `INGInious-0.8.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: INGInious
-Version: 0.8.5
+Version: 0.8.6
 Summary: An intelligent grader that allows secured and automated testing of code made by students.
 Home-page: https://github.com/UCL-INGI/INGInious
 Author: INGInious contributors
 Author-email: inginious@info.ucl.ac.be
 License: AGPL 3
 Provides-Extra: cgi
 Provides-Extra: ldap
```

### Comparing `INGInious-0.8.5/README.rst` & `INGInious-0.8.6/README.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/base-containers/base/Dockerfile` & `INGInious-0.8.6/base-containers/base/Dockerfile`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/base-containers/base/README.md` & `INGInious-0.8.6/base-containers/base/README.md`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/base-containers/base/bin/INGInious` & `INGInious-0.8.6/base-containers/base/bin/INGInious`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/base-containers/base/bin/_run_student_intern` & `INGInious-0.8.6/base-containers/base/bin/_run_student_intern`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/base-containers/base/bin/archive` & `INGInious-0.8.6/base-containers/base/bin/archive`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/base-containers/base/bin/feedback` & `INGInious-0.8.6/base-containers/base/bin/feedback`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/base-containers/base/bin/feedback-custom` & `INGInious-0.8.6/base-containers/base/bin/feedback-custom`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/base-containers/base/bin/feedback-grade` & `INGInious-0.8.6/base-containers/base/bin/feedback-grade`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/base-containers/base/bin/feedback-msg` & `INGInious-0.8.6/base-containers/base/bin/feedback-msg`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/base-containers/base/bin/feedback-msg-tpl` & `INGInious-0.8.6/base-containers/base/bin/feedback-msg-tpl`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/base-containers/base/bin/feedback-result` & `INGInious-0.8.6/base-containers/base/bin/feedback-result`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/base-containers/base/bin/feedback-state` & `INGInious-0.8.6/base-containers/base/bin/feedback-state`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/base-containers/base/bin/getinput` & `INGInious-0.8.6/base-containers/base/bin/getinput`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/base-containers/base/bin/inginious-ipython` & `INGInious-0.8.6/base-containers/base/bin/inginious-ipython`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/base-containers/base/bin/parsetemplate` & `INGInious-0.8.6/base-containers/base/bin/parsetemplate`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/base-containers/base/bin/rst-code` & `INGInious-0.8.6/base-containers/base/bin/rst-code`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/base-containers/base/bin/rst-image` & `INGInious-0.8.6/base-containers/base/bin/rst-image`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/base-containers/base/bin/rst-indent` & `INGInious-0.8.6/base-containers/base/bin/rst-indent`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/base-containers/base/bin/rst-msgblock` & `INGInious-0.8.6/base-containers/base/bin/rst-msgblock`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/base-containers/base/bin/run_student` & `INGInious-0.8.6/base-containers/base/bin/run_student`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/base-containers/base/bin/ssh_student` & `INGInious-0.8.6/base-containers/base/bin/ssh_student`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/base-containers/base/bin/tag-set` & `INGInious-0.8.6/base-containers/base/bin/tag-set`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/base-containers/base/inginious_container_api/feedback.py` & `INGInious-0.8.6/base-containers/base/inginious_container_api/feedback.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/base-containers/base/inginious_container_api/input.py` & `INGInious-0.8.6/base-containers/base/inginious_container_api/input.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/base-containers/base/inginious_container_api/lang.py` & `INGInious-0.8.6/base-containers/base/inginious_container_api/lang.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/base-containers/base/inginious_container_api/rst.py` & `INGInious-0.8.6/base-containers/base/inginious_container_api/rst.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/base-containers/base/inginious_container_api/run_student.py` & `INGInious-0.8.6/base-containers/base/inginious_container_api/run_student.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/base-containers/base/inginious_container_api/ssh_student.py` & `INGInious-0.8.6/base-containers/base/inginious_container_api/ssh_student.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/base-containers/base/inginious_container_api/utils.py` & `INGInious-0.8.6/base-containers/base/inginious_container_api/utils.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/configuration.example.yaml` & `INGInious-0.8.6/configuration.example.yaml`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/Makefile` & `INGInious-0.8.6/doc/Makefile`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/admin_doc/commands_doc/inginious-agent-docker.rst` & `INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-agent-docker.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/admin_doc/commands_doc/inginious-agent-mcq.rst` & `INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-agent-mcq.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/admin_doc/commands_doc/inginious-autotest.rst` & `INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-autotest.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/admin_doc/commands_doc/inginious-backend.rst` & `INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-backend.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/admin_doc/commands_doc/inginious-install.rst` & `INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-install.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/admin_doc/commands_doc/inginious-synchronize.rst` & `INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-synchronize.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/admin_doc/commands_doc/inginious-webapp.rst` & `INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-webapp.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/admin_doc/commands_doc/inginious-webdav.rst` & `INGInious-0.8.6/doc/admin_doc/commands_doc/inginious-webdav.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/admin_doc/install_doc/config_reference.rst` & `INGInious-0.8.6/doc/admin_doc/install_doc/config_reference.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/admin_doc/install_doc/create_container.rst` & `INGInious-0.8.6/doc/admin_doc/install_doc/create_container.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/admin_doc/install_doc/installation.rst` & `INGInious-0.8.6/doc/admin_doc/install_doc/installation.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/admin_doc/install_doc/other_oci_runtimes_support.rst` & `INGInious-0.8.6/doc/admin_doc/install_doc/other_oci_runtimes_support.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/admin_doc/install_doc/static_pages.rst` & `INGInious-0.8.6/doc/admin_doc/install_doc/static_pages.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/admin_doc/install_doc/troubleshooting.rst` & `INGInious-0.8.6/doc/admin_doc/install_doc/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/admin_doc/install_doc/updating.rst` & `INGInious-0.8.6/doc/admin_doc/install_doc/updating.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/admin_documentation.rst` & `INGInious-0.8.6/doc/admin_documentation.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/api_doc/inginious.client.rst` & `INGInious-0.8.6/doc/api_doc/inginious.client.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/api_doc/inginious.common.rst` & `INGInious-0.8.6/doc/api_doc/inginious.common.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/api_doc/inginious.common.task_file_readers.rst` & `INGInious-0.8.6/doc/api_doc/inginious.common.task_file_readers.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/api_doc/inginious.common.tests.rst` & `INGInious-0.8.6/doc/api_doc/inginious.common.tests.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/api_doc/inginious.frontend.pages.api.rst` & `INGInious-0.8.6/doc/api_doc/inginious.frontend.pages.api.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/api_doc/inginious.frontend.pages.course_admin.rst` & `INGInious-0.8.6/doc/api_doc/inginious.frontend.pages.course_admin.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/api_doc/inginious.frontend.pages.rst` & `INGInious-0.8.6/doc/api_doc/inginious.frontend.pages.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/api_doc/inginious.frontend.plugins.auth.rst` & `INGInious-0.8.6/doc/api_doc/inginious.frontend.plugins.auth.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/api_doc/inginious.frontend.plugins.rst` & `INGInious-0.8.6/doc/api_doc/inginious.frontend.plugins.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/api_doc/inginious.frontend.rst` & `INGInious-0.8.6/doc/api_doc/inginious.frontend.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/api_doc/inginious.frontend.tests.rst` & `INGInious-0.8.6/doc/api_doc/inginious.frontend.tests.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/conf.py` & `INGInious-0.8.6/doc/conf.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/dev_doc/extensions_doc/how_to_extend.rst` & `INGInious-0.8.6/doc/dev_doc/extensions_doc/how_to_extend.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/dev_doc/extensions_doc/i18n.rst` & `INGInious-0.8.6/doc/dev_doc/extensions_doc/i18n.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/dev_doc/extensions_doc/plugins.rst` & `INGInious-0.8.6/doc/dev_doc/extensions_doc/plugins.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/dev_doc/internals_doc/architectures.rst` & `INGInious-0.8.6/doc/dev_doc/internals_doc/architectures.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/dev_doc/internals_doc/exercises.rst` & `INGInious-0.8.6/doc/dev_doc/internals_doc/exercises.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/dev_doc/internals_doc/frontend.rst` & `INGInious-0.8.6/doc/dev_doc/internals_doc/frontend.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/dev_doc/internals_doc/inginious_arch.png` & `INGInious-0.8.6/doc/dev_doc/internals_doc/inginious_arch.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/dev_doc/internals_doc/inginious_arch_docker.png` & `INGInious-0.8.6/doc/dev_doc/internals_doc/inginious_arch_docker.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/dev_doc/internals_doc/inginious_arch_full.png` & `INGInious-0.8.6/doc/dev_doc/internals_doc/inginious_arch_full.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/dev_doc/internals_doc/submission_evaluation_docker.png` & `INGInious-0.8.6/doc/dev_doc/internals_doc/submission_evaluation_docker.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/dev_doc/internals_doc/submission_workflow.png` & `INGInious-0.8.6/doc/dev_doc/internals_doc/submission_workflow.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/dev_doc/internals_doc/submissions.rst` & `INGInious-0.8.6/doc/dev_doc/internals_doc/submissions.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/dev_doc/internals_doc/understand_inginious.rst` & `INGInious-0.8.6/doc/dev_doc/internals_doc/understand_inginious.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/developer_documentation.rst` & `INGInious-0.8.6/doc/developer_documentation.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/logo_rtd.svg` & `INGInious-0.8.6/doc/logo_rtd.svg`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/make.bat` & `INGInious-0.8.6/doc/make.bat`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/teacher_doc/best_practices.rst` & `INGInious-0.8.6/doc/teacher_doc/best_practices.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/teacher_doc/common.rst` & `INGInious-0.8.6/doc/teacher_doc/common.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/teacher_doc/course_admin.rst` & `INGInious-0.8.6/doc/teacher_doc/course_admin.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/teacher_doc/course_description.rst` & `INGInious-0.8.6/doc/teacher_doc/course_description.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/teacher_doc/course_tuto.rst` & `INGInious-0.8.6/doc/teacher_doc/course_tuto.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/teacher_doc/courses.rst` & `INGInious-0.8.6/doc/teacher_doc/courses.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/teacher_doc/inginious_container_api.rst` & `INGInious-0.8.6/doc/teacher_doc/inginious_container_api.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/teacher_doc/lti.rst` & `INGInious-0.8.6/doc/teacher_doc/lti.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/teacher_doc/random.rst` & `INGInious-0.8.6/doc/teacher_doc/random.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/teacher_doc/rst.rst` & `INGInious-0.8.6/doc/teacher_doc/rst.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/teacher_doc/run_file.rst` & `INGInious-0.8.6/doc/teacher_doc/run_file.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/teacher_doc/share_files.rst` & `INGInious-0.8.6/doc/teacher_doc/share_files.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/teacher_doc/system_files.rst` & `INGInious-0.8.6/doc/teacher_doc/system_files.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/teacher_doc/task_file.rst` & `INGInious-0.8.6/doc/teacher_doc/task_file.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/teacher_doc/task_tuto.rst` & `INGInious-0.8.6/doc/teacher_doc/task_tuto.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/teacher_doc/testing.rst` & `INGInious-0.8.6/doc/teacher_doc/testing.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/teacher_doc/translating.rst` & `INGInious-0.8.6/doc/teacher_doc/translating.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/doc/what_is_inginious.rst` & `INGInious-0.8.6/doc/what_is_inginious.rst`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/__init__.py` & `INGInious-0.8.6/inginious/__init__.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/agent/__init__.py` & `INGInious-0.8.6/inginious/agent/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 
 class Agent(object, metaclass=ABCMeta):
     """
     An INGInious agent, that grades specific kinds of jobs, and interacts with a Backend.
     """
 
-    def __init__(self, context, backend_addr, friendly_name, concurrency, filesystem, ssh_allowed=False):
+    def __init__(self, context, backend_addr, friendly_name, concurrency, filesystem):
         """
         :param context: a ZMQ context to which the agent will be linked
         :param backend_addr: address of the backend to which the agent should connect. The format is the same as ZMQ
         :param concurrency: number of simultaneous jobs that can be run by this agent
         :param filesystem: filesystem for the tasks
         """
         # These fields can be read/modified/overridden in subclasses
@@ -62,15 +62,14 @@
 
         # These fields should not be read/modified/overridden in subclasses
         self.__concurrency = concurrency
 
         self.__backend_addr = backend_addr
         self.__context = context
         self.__friendly_name = friendly_name
-        self.__ssh_allowed = ssh_allowed
         self.__backend_socket = self.__context.socket(zmq.DEALER)
         self.__backend_socket.ipv6 = True
 
         self.__running_job = {}
         self.__running_batch_job = set()
 
         self.__backend_last_seen_time = None
@@ -108,15 +107,15 @@
         May raise an asyncio.CancelledError, in which case the agent should clean itself and restart completely.
         """
         self._logger.info("Agent started")
         self.__backend_socket.connect(self.__backend_addr)
 
         # Tell the backend we are up and have `concurrency` threads available
         self._logger.info("Saying hello to the backend")
-        await ZMQUtils.send(self.__backend_socket, AgentHello(self.__friendly_name, self.__concurrency, self.environments, self.__ssh_allowed))
+        await ZMQUtils.send(self.__backend_socket, AgentHello(self.__friendly_name, self.__concurrency, self.environments))
         self.__backend_last_seen_time = time.time()
 
         run_listen = self._loop.create_task(self.__run_listen())
 
         self._loop.call_later(1, self._create_safe_task, self.__check_last_ping(run_listen))
 
         await run_listen
```

### Comparing `INGInious-0.8.5/inginious/agent/docker_agent/__init__.py` & `INGInious-0.8.6/inginious/agent/docker_agent/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     student_path: str
     systemfiles_path: str
     course_common_student_path: str
     run_cmd: str
     assigned_external_ports: List[int]
     student_containers: Set[str]  # container ids of student containers
     enable_network: bool
-    ssh_allowed: bool
 
 
 @dataclass
 class DockerRunningStudentContainer:
     container_id: str
     parent_info: DockerRunningJob
     socket_id: str
@@ -76,16 +75,15 @@
         :param address_host: hostname/ip/... to which external client should connect to access to the docker
         :param external_ports: iterable containing ports to which the docker instance can bind internal ports
         :param tmp_dir: temp dir that is used by the agent to start new containers
         :param type: type of the container ("docker" or "kata")
         :param runtime: runtime used by docker (the defaults are "runc" with docker or "kata-runtime" with kata)
         :param ssh_allowed: boolean to make this agent accept tasks with ssh or not
         """
-        super(DockerAgent, self).__init__(context, backend_addr, friendly_name, concurrency, tasks_fs,
-                                          ssh_allowed=ssh_allowed)
+        super(DockerAgent, self).__init__(context, backend_addr, friendly_name, concurrency, tasks_fs)
 
         self._runtimes = {x.envtype: x for x in runtimes} if runtimes is not None else None
 
         self._logger = logging.getLogger("inginious.agent.docker")
 
         self._concurrency = concurrency
 
@@ -98,14 +96,17 @@
         self._address_host = address_host
         self._external_ports = set(external_ports) if external_ports is not None else set()
 
         # Async proxy to os
         self._aos = AsyncProxy(os)
         self._ashutil = AsyncProxy(shutil)
 
+        # Does this agent allow ssh_student ?
+        self._ssh_allowed = ssh_allowed
+
     async def _init_clean(self):
         """ Must be called when the agent is starting """
         # Data about running containers
         self._containers_running: Dict[str, DockerRunningJob] = {}  # container_id -> info
         self._container_for_job: Dict[str, str] = {}  # job id -> container_id
 
         self._student_containers_running: Dict[str, DockerRunningStudentContainer] = {}
@@ -277,15 +278,14 @@
 
         debug = message.debug
         environment_type = message.environment_type
         environment_name = message.environment
 
         try:
             enable_network = message.environment_parameters.get("network_grading", False)
-            ssh_allowed = message.environment_parameters.get("ssh_allowed", False)
             limits = message.environment_parameters.get("limits", {})
             time_limit = int(limits.get("time", 30))
             hard_time_limit = int(limits.get("hard_time", None) or time_limit * 3)
             mem_limit = int(limits.get("memory", 200))
             run_cmd = message.environment_parameters.get("run_cmd", '')
         except:
             raise CannotCreateJobException('The agent is unable to parse the parameters')
@@ -409,16 +409,15 @@
             sockets_path=sockets_path,
             student_path=student_path,
             systemfiles_path=systemfiles_path,
             course_common_student_path=course_common_student_path,
             run_cmd=run_cmd,
             assigned_external_ports=list(ports.values()),
             student_containers=set(),
-            enable_network=enable_network,
-            ssh_allowed=ssh_allowed
+            enable_network=enable_network
         )
 
         self._containers_running[container_id] = info
         self._container_for_job[message.job_id] = container_id
 
         try:
             # Start the container
@@ -671,15 +670,15 @@
                             time_limit = min(msg["time_limit"] or info.time_limit, info.time_limit)
                             hard_time_limit = min(msg["hard_time_limit"] or info.hard_time_limit, info.hard_time_limit)
                             share_network = msg["share_network"]
                             socket_id = msg["socket_id"]
                             ssh = msg["ssh"]
                             run_as_root = msg["run_as_root"]
                             assert "/" not in socket_id  # ensure task creator do not try to break the agent :-(
-                            if ssh and not (info.enable_network and info.ssh_allowed):
+                            if ssh and not (info.enable_network and "ssh" in info.environment_type and self._ssh_allowed):
                                 self._logger.error(
                                     "Exception: ssh for student requires to allow ssh and internet access in the task %s environment configuration tab",
                                     info.job_id)
                                 self._create_safe_task(self.handle_job_closing(info.container_id, -1,
                                                                                manual_feedback="ssh for student requires to allow ssh and internet access in the task environment configuration tab!"))
                             else:
                                 self._create_safe_task(
@@ -976,26 +975,31 @@
             await super(DockerAgent, self).run()
         except:
             await self._end_clean()
             raise
 
     def _detect_runtimes(self) -> Dict[str, DockerRuntime]:
         heuristic = [
-            ("runc", lambda x: DockerRuntime(runtime=x, run_as_root=False, enables_gpu=False, shared_kernel=True, envtype="docker")),
-            ("crun", lambda x: DockerRuntime(runtime=x, run_as_root=False, enables_gpu=False, shared_kernel=True, envtype="docker")),
-            ("kata", lambda x: DockerRuntime(runtime=x, run_as_root=True, enables_gpu=False, shared_kernel=False, envtype="kata")),
-            ("nvidia", lambda x: DockerRuntime(runtime=x, run_as_root=False, enables_gpu=True, shared_kernel=True, envtype="nvidia"))
+            ("runc", lambda x, y: DockerRuntime(runtime=x, run_as_root=False, enables_gpu=False,
+                                                shared_kernel=True, envtype="docker-ssh" if y else "docker")),
+            ("crun", lambda x, y: DockerRuntime(runtime=x, run_as_root=False, enables_gpu=False,
+                                                shared_kernel=True, envtype="docker-ssh" if y else "docker")),
+            ("kata", lambda x, y: DockerRuntime(runtime=x, run_as_root=True, enables_gpu=False,
+                                                shared_kernel=False, envtype="kata-ssh" if y else "kata")),
+            ("nvidia", lambda x, y: DockerRuntime(runtime=x, run_as_root=False, enables_gpu=True,
+                                                  shared_kernel=True, envtype="nvidia-ssh" if y else "nvidia"))
         ]
         retval = {}
 
         for runtime in self._docker.sync.list_runtimes().keys():
             for h_runtime, f in heuristic:
                 if h_runtime in runtime:
-                    v = f(runtime)
-                    if v.envtype not in retval:
-                        self._logger.info("Using %s as runtime with parameters %s", runtime, str(v))
-                        retval[v.envtype] = v
-                    else:
-                        self._logger.warning(
-                            "%s was detected as a runtime; it would duplicate another one, so we ignore it. %s",
-                            runtime, str(v))
+                    for ssh_allowed in {self._ssh_allowed, False}:
+                        v = f(runtime, ssh_allowed)
+                        if v.envtype not in retval:
+                            self._logger.info("Using %s as runtime with parameters %s", runtime, str(v))
+                            retval[v.envtype] = v
+                        else:
+                            self._logger.warning(
+                                "%s was detected as a runtime; it would duplicate another one, so we ignore it. %s",
+                                runtime, str(v))
         return retval
```

### Comparing `INGInious-0.8.5/inginious/agent/docker_agent/_docker_interface.py` & `INGInious-0.8.6/inginious/agent/docker_agent/_docker_interface.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/agent/docker_agent/_docker_runtime.py` & `INGInious-0.8.6/inginious/agent/docker_agent/_docker_runtime.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/agent/docker_agent/_timeout_watcher.py` & `INGInious-0.8.6/inginious/agent/docker_agent/_timeout_watcher.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/agent/mcq_agent/__init__.py` & `INGInious-0.8.6/inginious/agent/mcq_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/agent/mcq_agent/i18n/de/LC_MESSAGES/messages.mo` & `INGInious-0.8.6/inginious/agent/mcq_agent/i18n/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/agent/mcq_agent/i18n/de/LC_MESSAGES/messages.po` & `INGInious-0.8.6/inginious/agent/mcq_agent/i18n/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/agent/mcq_agent/i18n/es/LC_MESSAGES/messages.mo` & `INGInious-0.8.6/inginious/agent/mcq_agent/i18n/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/agent/mcq_agent/i18n/es/LC_MESSAGES/messages.po` & `INGInious-0.8.6/inginious/agent/mcq_agent/i18n/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/agent/mcq_agent/i18n/fr/LC_MESSAGES/messages.mo` & `INGInious-0.8.6/inginious/agent/mcq_agent/i18n/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/agent/mcq_agent/i18n/fr/LC_MESSAGES/messages.po` & `INGInious-0.8.6/inginious/agent/mcq_agent/i18n/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/agent/mcq_agent/i18n/messages.pot` & `INGInious-0.8.6/inginious/agent/mcq_agent/i18n/messages.pot`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/backend/backend.py` & `INGInious-0.8.6/inginious/backend/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # This will be pushed inside a TopicPriorityQueue that uses natural ordering (smallest element has the highest priority)
 # priority and time_received must thus be the two first element of the tuples.
 # a tuple with a small priority value will actually be processed first.
 WaitingJob = namedtuple('WaitingJob', ['priority', 'time_received', 'client_addr', 'job_id', 'msg'])
 
 RunningJob = namedtuple('RunningJob', ['agent_addr', 'client_addr', 'msg', 'time_started'])
 EnvironmentInfo = namedtuple('EnvironmentInfo', ['last_id', 'created_last', 'agents', 'type'])
-AgentInfo = namedtuple('AgentInfo', ['name', 'environments', 'ssh_allowed'])  # environments is a list of tuple (type, environment)
+AgentInfo = namedtuple('AgentInfo', ['name', 'environments'])  # environments is a list of tuple (type, environment)
 
 class Backend(object):
     """
         Backend. Central point of the architecture, manages communication between clients (frontends) and agents.
         Schedule jobs on agents.
     """
 
@@ -134,15 +134,15 @@
                                           BackendJobDone(message.job_id, ("crash", "Duplicate job id"),
                                                          0.0, {}, {}, {}, "", None, "", ""))
             return
 
         self._logger.info("Adding a new job %s %s to the queue", client_addr, message.job_id)
         job = WaitingJob(message.priority, time.time(), client_addr, message.job_id, message)
         self._waiting_jobs[message.job_id] = job
-        self._waiting_jobs_pq.put((message.environment_type, message.environment, self._get_ssh_allowed(message)), job)
+        self._waiting_jobs_pq.put((message.environment_type, message.environment), job)
 
         await self.update_queue()
 
     async def handle_client_kill_job(self, client_addr, message: ClientKillJob):
         """ Handle an ClientKillJob message. Remove a job from the waiting list or send the kill message to the right agent. """
         # Check if the job is not in the waiting list
         if message.job_id in self._waiting_jobs:
@@ -192,18 +192,15 @@
             if self._waiting_jobs_pq.empty():
                 break  # nothing to do
 
             try:
                 job = None
                 while job is None:
                     # keep the object, do not unzip it directly! It's sometimes modified when a job is killed.
-
-                    topics = [(*env, False) for env in self._registered_agents[agent_addr].environments]
-                    if self._registered_agents[agent_addr].ssh_allowed:
-                        topics += [(*env, True) for env in self._registered_agents[agent_addr].environments]
+                    topics = self._registered_agents[agent_addr].environments
 
                     job = self._waiting_jobs_pq.get(topics)
                     priority, insert_time, client_addr, job_id, job_msg = job
 
                     # Ensure the job has not been removed (killed)
                     if job_id not in self._waiting_jobs:
                         job = None  # repeat the while loop. we need a job
@@ -234,15 +231,15 @@
 
         if agent_addr in self._registered_agents:
             # Delete previous instance of this agent, if any
             await self._delete_agent(agent_addr)
 
         self._registered_agents[agent_addr] = AgentInfo(message.friendly_name,
                                                         [(etype, env) for etype, envs in
-                                                         message.available_environments.items() for env in envs], message.ssh_allowed)
+                                                         message.available_environments.items() for env in envs])
         self._available_agents.extend([agent_addr for _ in range(0, message.available_job_slots)])
         self._ping_count[agent_addr] = 0
 
         # update information about available environments
         for environment_type, environments in message.available_environments.items():
             if environment_type not in self._environments:
                 self._environments[environment_type] = {}
@@ -403,15 +400,8 @@
         """
             Returns an estimate of the time taken by a given job, if available in the environment_parameters.
             For this to work, ["limits"]["time"] must be a parameter of the environment.
         """
         try:
             return int(job_info.environment_parameters["limits"]["time"])
         except:
-            return -1 # unknown
-
-    def _get_ssh_allowed(self, job_info: ClientNewJob):
-        """
-            Returns if the job requires that the agent allows ssh
-            For this to work, ["ssh_allowed"] must be a parameter of the environment.
-        """
-        return job_info.environment_parameters.get("ssh_allowed", False)
+            return -1 # unknown
```

### Comparing `INGInious-0.8.5/inginious/backend/topic_priority_queue.py` & `INGInious-0.8.6/inginious/backend/topic_priority_queue.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/client/_zeromq_client.py` & `INGInious-0.8.6/inginious/client/_zeromq_client.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/client/client.py` & `INGInious-0.8.6/inginious/client/client.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/client/client_buffer.py` & `INGInious-0.8.6/inginious/client/client_buffer.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/client/client_sync.py` & `INGInious-0.8.6/inginious/client/client_sync.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/common/asyncio_utils.py` & `INGInious-0.8.6/inginious/common/asyncio_utils.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/common/babel.py` & `INGInious-0.8.6/inginious/common/babel.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/common/base.py` & `INGInious-0.8.6/inginious/common/base.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/common/custom_yaml.py` & `INGInious-0.8.6/inginious/common/custom_yaml.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/common/entrypoints.py` & `INGInious-0.8.6/inginious/common/entrypoints.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/common/exceptions.py` & `INGInious-0.8.6/inginious/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/common/filesystems/__init__.py` & `INGInious-0.8.6/inginious/common/filesystems/__init__.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/common/filesystems/local.py` & `INGInious-0.8.6/inginious/common/filesystems/local.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/common/log.py` & `INGInious-0.8.6/inginious/common/log.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/common/messages.py` & `INGInious-0.8.6/inginious/common/messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,14 @@
 
 @dataclass(frozen=True)
 class AgentHello:
     """ Let the agent say hello and announce which environments it has available """
     friendly_name: str  # a string containing a friendly name to identify agent
     available_job_slots: int  # an integer giving the number of concurrent
     available_environments: Dict[str, Dict[str, Dict[str, Any]]]  # dict of available environments:
-    ssh_allowed: bool
     # {
     #     "type": {
     #         "name": {                 #  for example, "default"
     #             "id": "env img id",   # "sha256:715c5cb5575cdb2641956e42af4a53e69edf763ce701006b2c6e0f4f39b68dd3"
     #             "created": 12345678,  # create date
     #             "ports": [22, 434],   # list of ports needed
     #         }
```

### Comparing `INGInious-0.8.5/inginious/common/tags.py` & `INGInious-0.8.6/inginious/common/tags.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/common/task_file_readers/abstract_reader.py` & `INGInious-0.8.6/inginious/common/task_file_readers/abstract_reader.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/common/task_file_readers/yaml_reader.py` & `INGInious-0.8.6/inginious/common/task_file_readers/yaml_reader.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/common/tasks_problems.py` & `INGInious-0.8.6/inginious/common/tasks_problems.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/common/tests/TestBase.py` & `INGInious-0.8.6/inginious/common/tests/TestBase.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/common/tests/TestCustomYaml.py` & `INGInious-0.8.6/inginious/common/tests/TestCustomYaml.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/common/tests/test_filesystem_local.py` & `INGInious-0.8.6/inginious/common/tests/test_filesystem_local.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/accessible_time.py` & `INGInious-0.8.6/inginious/frontend/accessible_time.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/app.py` & `INGInious-0.8.6/inginious/frontend/app.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/arch_helper.py` & `INGInious-0.8.6/inginious/frontend/arch_helper.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/course_factory.py` & `INGInious-0.8.6/inginious/frontend/course_factory.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/courses.py` & `INGInious-0.8.6/inginious/frontend/courses.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/environment_types/__init__.py` & `INGInious-0.8.6/inginious/frontend/environment_types/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,10 +21,13 @@
     """ env_obj is an instance of FrontendEnvType """
     __env_types[env_obj.id] = env_obj
 
 
 def register_base_env_types():
     # register standard env types here
     register_env_type(DockerEnvType())
+    register_env_type(DockerEnvType(ssh_allowed=True))
     register_env_type(NvidiaEnvType())
+    register_env_type(NvidiaEnvType(ssh_allowed=True))
     register_env_type(KataEnvType())
+    register_env_type(KataEnvType(ssh_allowed=True))
     register_env_type(MCQEnvType())
```

### Comparing `INGInious-0.8.5/inginious/frontend/environment_types/env_type.py` & `INGInious-0.8.6/inginious/frontend/environment_types/env_type.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/environment_types/generic_docker_oci_runtime.py` & `INGInious-0.8.6/inginious/frontend/environment_types/generic_docker_oci_runtime.py`

 * *Files 24% similar despite different names*

```diff
@@ -24,19 +24,14 @@
 
         # Response is HTML
         out["response_is_html"] = data.get("response_is_html", False)
 
         # Network access in grading container?
         out["network_grading"] = data.get("network_grading", False)
 
-        # SSH allowed ?
-        out["ssh_allowed"] = data.get("ssh_allowed", False)
-        if out["ssh_allowed"] == 'on':
-            out["ssh_allowed"] = True
-
         # Limits
         limits = {"time": 20, "memory": 1024, "disk": 1024}
         if "limits" in data:
             try:
                 limits['time'] = int(data["limits"].get("time", 20))
                 hard_time = data["limits"].get("hard_time", '')
                 if str(hard_time).strip() == '':
@@ -55,7 +50,10 @@
         out["limits"] = limits
 
         return out
 
     def studio_env_template(self, templator, task, allow_html: bool):
         return templator.render("course_admin/edit_tabs/env_generic_docker_oci.html", env_params=task.get("environment_parameters", {}),
                                 content_is_html=allow_html, env_id=self.id)
+
+    def __init__(self, ssh_allowed=False):
+        self._ssh_allowed = ssh_allowed
```

### Comparing `INGInious-0.8.5/inginious/frontend/flask/mapping.py` & `INGInious-0.8.6/inginious/frontend/flask/mapping.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/flask/mongo_sessions.py` & `INGInious-0.8.6/inginious/frontend/flask/mongo_sessions.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/i18n/de/LC_MESSAGES/messages.mo` & `INGInious-0.8.6/inginious/frontend/i18n/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/i18n/de/LC_MESSAGES/messages.po` & `INGInious-0.8.6/inginious/frontend/i18n/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/i18n/el/LC_MESSAGES/messages.mo` & `INGInious-0.8.6/inginious/frontend/i18n/el/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/i18n/el/LC_MESSAGES/messages.po` & `INGInious-0.8.6/inginious/frontend/i18n/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/i18n/es/LC_MESSAGES/messages.mo` & `INGInious-0.8.6/inginious/frontend/i18n/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/i18n/es/LC_MESSAGES/messages.po` & `INGInious-0.8.6/inginious/frontend/i18n/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/i18n/fr/LC_MESSAGES/messages.mo` & `INGInious-0.8.6/inginious/frontend/i18n/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/i18n/fr/LC_MESSAGES/messages.po` & `INGInious-0.8.6/inginious/frontend/i18n/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/i18n/he/LC_MESSAGES/messages.mo` & `INGInious-0.8.6/inginious/frontend/i18n/he/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/i18n/he/LC_MESSAGES/messages.po` & `INGInious-0.8.6/inginious/frontend/i18n/he/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/i18n/messages.pot` & `INGInious-0.8.6/inginious/frontend/i18n/messages.pot`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/i18n/nl/LC_MESSAGES/messages.mo` & `INGInious-0.8.6/inginious/frontend/i18n/nl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/i18n/nl/LC_MESSAGES/messages.po` & `INGInious-0.8.6/inginious/frontend/i18n/nl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/i18n/pt/LC_MESSAGES/messages.mo` & `INGInious-0.8.6/inginious/frontend/i18n/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/i18n/pt/LC_MESSAGES/messages.po` & `INGInious-0.8.6/inginious/frontend/i18n/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/i18n/pt_BR/LC_MESSAGES/messages.mo` & `INGInious-0.8.6/inginious/frontend/i18n/pt_BR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/i18n/vi/LC_MESSAGES/messages.mo` & `INGInious-0.8.6/inginious/frontend/i18n/vi/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/i18n/vi/LC_MESSAGES/messages.po` & `INGInious-0.8.6/inginious/frontend/i18n/vi/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/i18n/wa/LC_MESSAGES/messages.mo` & `INGInious-0.8.6/inginious/frontend/i18n/wa/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/i18n/wa/LC_MESSAGES/messages.po` & `INGInious-0.8.6/inginious/frontend/i18n/wa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/installer.py` & `INGInious-0.8.6/inginious/frontend/installer.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/l10n_manager.py` & `INGInious-0.8.6/inginious/frontend/l10n_manager.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/lti_outcome_manager.py` & `INGInious-0.8.6/inginious/frontend/lti_outcome_manager.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/lti_request_validator.py` & `INGInious-0.8.6/inginious/frontend/lti_request_validator.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/lti_tool_provider.py` & `INGInious-0.8.6/inginious/frontend/lti_tool_provider.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/marketplace_courses.py` & `INGInious-0.8.6/inginious/frontend/marketplace_courses.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/admin/admin.py` & `INGInious-0.8.6/inginious/frontend/pages/admin/admin.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/api/_api_page.py` & `INGInious-0.8.6/inginious/frontend/pages/api/_api_page.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/api/auth_methods.py` & `INGInious-0.8.6/inginious/frontend/pages/api/auth_methods.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/api/authentication.py` & `INGInious-0.8.6/inginious/frontend/pages/api/authentication.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/api/courses.py` & `INGInious-0.8.6/inginious/frontend/pages/api/courses.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/api/submissions.py` & `INGInious-0.8.6/inginious/frontend/pages/api/submissions.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/api/tasks.py` & `INGInious-0.8.6/inginious/frontend/pages/api/tasks.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/course.py` & `INGInious-0.8.6/inginious/frontend/pages/course.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/course_admin/audience_edit.py` & `INGInious-0.8.6/inginious/frontend/pages/course_admin/audience_edit.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/course_admin/danger_zone.py` & `INGInious-0.8.6/inginious/frontend/pages/course_admin/danger_zone.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/course_admin/search_user.py` & `INGInious-0.8.6/inginious/frontend/pages/course_admin/search_user.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/course_admin/settings.py` & `INGInious-0.8.6/inginious/frontend/pages/course_admin/settings.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/course_admin/statistics.py` & `INGInious-0.8.6/inginious/frontend/pages/course_admin/statistics.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/course_admin/student_info.py` & `INGInious-0.8.6/inginious/frontend/pages/course_admin/student_info.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/course_admin/student_list.py` & `INGInious-0.8.6/inginious/frontend/pages/course_admin/student_list.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/course_admin/submission.py` & `INGInious-0.8.6/inginious/frontend/pages/course_admin/submission.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/course_admin/submissions.py` & `INGInious-0.8.6/inginious/frontend/pages/course_admin/submissions.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/course_admin/tags.py` & `INGInious-0.8.6/inginious/frontend/pages/course_admin/tags.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/course_admin/task_edit.py` & `INGInious-0.8.6/inginious/frontend/pages/course_admin/task_edit.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/course_admin/task_edit_file.py` & `INGInious-0.8.6/inginious/frontend/pages/course_admin/task_edit_file.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/course_admin/task_list.py` & `INGInious-0.8.6/inginious/frontend/pages/course_admin/task_list.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/course_admin/utils.py` & `INGInious-0.8.6/inginious/frontend/pages/course_admin/utils.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/course_register.py` & `INGInious-0.8.6/inginious/frontend/pages/course_register.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/courselist.py` & `INGInious-0.8.6/inginious/frontend/pages/courselist.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/group.py` & `INGInious-0.8.6/inginious/frontend/pages/group.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/index.py` & `INGInious-0.8.6/inginious/frontend/pages/index.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/lti.py` & `INGInious-0.8.6/inginious/frontend/pages/lti.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/maintenance.py` & `INGInious-0.8.6/inginious/frontend/pages/maintenance.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/marketplace.py` & `INGInious-0.8.6/inginious/frontend/pages/marketplace.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/marketplace_course.py` & `INGInious-0.8.6/inginious/frontend/pages/marketplace_course.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/mycourses.py` & `INGInious-0.8.6/inginious/frontend/pages/mycourses.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/preferences/bindings.py` & `INGInious-0.8.6/inginious/frontend/pages/preferences/bindings.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/preferences/delete.py` & `INGInious-0.8.6/inginious/frontend/pages/preferences/delete.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/preferences/profile.py` & `INGInious-0.8.6/inginious/frontend/pages/preferences/profile.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/preferences/utils.py` & `INGInious-0.8.6/inginious/frontend/pages/preferences/utils.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/queue.py` & `INGInious-0.8.6/inginious/frontend/pages/queue.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/register.py` & `INGInious-0.8.6/inginious/frontend/pages/register.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/social.py` & `INGInious-0.8.6/inginious/frontend/pages/social.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/tasks.py` & `INGInious-0.8.6/inginious/frontend/pages/tasks.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/pages/utils.py` & `INGInious-0.8.6/inginious/frontend/pages/utils.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/parsable_text.py` & `INGInious-0.8.6/inginious/frontend/parsable_text.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugin_manager.py` & `INGInious-0.8.6/inginious/frontend/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/auth/__pycache__/google_auth.cpython-310.pyc` & `INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/google_auth.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun 10 10:07:01 2021 UTC, .py size: 2979 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 45e4 c160 a30b 0000  o.......E..`....
+00000000: 6f0d 0d0a 0000 0000 1af2 4864 a30b 0000  o.........Hd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6c00 0000 6400  .....@...sl...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c03  Z.d.d.l.Z.d.d.l.
 00000050: 6d04 5a04 0100 6401 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c07 6d08 5a08 0100 6406  ..d.d.l.m.Z...d.
 00000070: 5a09 6407 5a0a 6700 6408 a201 5a0b 4700  Z.d.Z.g.d...Z.G.
```

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/auth/__pycache__/google_auth.cpython-36.pyc` & `INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/google_auth.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/auth/__pycache__/google_auth.cpython-38.pyc` & `INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/google_auth.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/auth/__pycache__/google_auth.cpython-39.pyc` & `INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/google_auth.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-310.pyc` & `INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Feb  9 08:29:26 2022 UTC, .py size: 7358 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 667b 0362 be1c 0000  o.......f{.b....
+00000000: 6f0d 0d0a 0000 0000 1af2 4864 be1c 0000  o.........Hd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8e00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c03  Z.d.d.l.Z.d.d.l.
 00000050: 6d04 5a04 0100 6401 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c07 6d08 5a08 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6406 6c09 6d0a 5a0a 0100 6401 6407 6c0b  d.l.m.Z...d.d.l.
```

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-36.pyc` & `INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-37.pyc` & `INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-38.pyc` & `INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-39.pyc` & `INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/ldap_auth.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-310.pyc` & `INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun 10 10:07:01 2021 UTC, .py size: 7053 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 45e4 c160 8d1b 0000  o.......E..`....
+00000000: 6f0d 0d0a 0000 0000 1af2 4864 8d1b 0000  o.........Hd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 bc00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6403 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 6d07 5a07 0100 6401 6404 6c05 6d08 5a08  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6405 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
```

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-36.pyc` & `INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-37.pyc` & `INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-38.pyc` & `INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-39.pyc` & `INGInious-0.8.6/inginious/frontend/plugins/auth/__pycache__/saml2_auth.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/auth/custom_auth_form.html` & `INGInious-0.8.6/inginious/frontend/plugins/auth/custom_auth_form.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/auth/facebook_auth.py` & `INGInious-0.8.6/inginious/frontend/plugins/auth/facebook_auth.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/auth/github_auth.py` & `INGInious-0.8.6/inginious/frontend/plugins/auth/github_auth.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/auth/google_auth.py` & `INGInious-0.8.6/inginious/frontend/plugins/auth/google_auth.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/auth/ldap_auth.py` & `INGInious-0.8.6/inginious/frontend/plugins/auth/ldap_auth.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/auth/linkedin_auth.py` & `INGInious-0.8.6/inginious/frontend/plugins/auth/linkedin_auth.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/auth/saml2_auth.py` & `INGInious-0.8.6/inginious/frontend/plugins/auth/saml2_auth.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/auth/twitter_auth.py` & `INGInious-0.8.6/inginious/frontend/plugins/auth/twitter_auth.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/contests/__init__.py` & `INGInious-0.8.6/inginious/frontend/plugins/contests/__init__.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/contests/__pycache__/__init__.cpython-310.pyc` & `INGInious-0.8.6/inginious/frontend/plugins/contests/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Mar 14 09:48:05 2023 UTC, .py size: 11265 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 d542 1064 012c 0000  o........B.d.,..
+00000000: 6f0d 0d0a 0000 0000 1af2 4864 012c 0000  o.........Hd.,..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 bc00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 6d05 5a05 0100 6401 6402 6c06 5a06 6401  m.Z...d.d.l.Z.d.
 00000060: 6402 6c07 5a07 6401 6405 6c08 6d09 5a09  d.l.Z.d.d.l.m.Z.
 00000070: 0100 6401 6406 6c0a 6d0b 5a0b 0100 6401  ..d.d.l.m.Z...d.
```

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/contests/__pycache__/__init__.cpython-37.pyc` & `INGInious-0.8.6/inginious/frontend/plugins/contests/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/contests/__pycache__/__init__.cpython-38.pyc` & `INGInious-0.8.6/inginious/frontend/plugins/contests/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/contests/__pycache__/__init__.cpython-39.pyc` & `INGInious-0.8.6/inginious/frontend/plugins/contests/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/contests/admin.html` & `INGInious-0.8.6/inginious/frontend/plugins/contests/admin.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/contests/course_menu.html` & `INGInious-0.8.6/inginious/frontend/plugins/contests/course_menu.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/contests/scoreboard.html` & `INGInious-0.8.6/inginious/frontend/plugins/contests/scoreboard.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/demo/__init__.py` & `INGInious-0.8.6/inginious/frontend/plugins/demo/__init__.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/git_repo/__init__.py` & `INGInious-0.8.6/inginious/frontend/plugins/git_repo/__init__.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/ltibestsubmission/__init__.py` & `INGInious-0.8.6/inginious/frontend/plugins/ltibestsubmission/__init__.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/scoreboard/__init__.py` & `INGInious-0.8.6/inginious/frontend/plugins/scoreboard/__init__.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/scoreboard/__pycache__/__init__.cpython-310.pyc` & `INGInious-0.8.6/inginious/frontend/plugins/scoreboard/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/scoreboard/__pycache__/__init__.cpython-37.pyc` & `INGInious-0.8.6/inginious/frontend/plugins/scoreboard/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/scoreboard/__pycache__/__init__.cpython-38.pyc` & `INGInious-0.8.6/inginious/frontend/plugins/scoreboard/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/scoreboard/__pycache__/__init__.cpython-39.pyc` & `INGInious-0.8.6/inginious/frontend/plugins/scoreboard/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/scoreboard/main.html` & `INGInious-0.8.6/inginious/frontend/plugins/scoreboard/main.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/scoreboard/scoreboard.html` & `INGInious-0.8.6/inginious/frontend/plugins/scoreboard/scoreboard.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/simple_grader/__init__.py` & `INGInious-0.8.6/inginious/frontend/plugins/simple_grader/__init__.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/task_editor_hook_example/__init__.py` & `INGInious-0.8.6/inginious/frontend/plugins/task_editor_hook_example/__init__.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/task_editor_hook_example/example_tab_2.html` & `INGInious-0.8.6/inginious/frontend/plugins/task_editor_hook_example/example_tab_2.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/task_file_readers/json_reader.py` & `INGInious-0.8.6/inginious/frontend/plugins/task_file_readers/json_reader.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/upcoming_tasks/__init__.py` & `INGInious-0.8.6/inginious/frontend/plugins/upcoming_tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/upcoming_tasks/templates/coming_tasks.html` & `INGInious-0.8.6/inginious/frontend/plugins/upcoming_tasks/templates/coming_tasks.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/plugins/upcoming_tasks/templates/upcoming_task_list.html` & `INGInious-0.8.6/inginious/frontend/plugins/upcoming_tasks/templates/upcoming_task_list.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/css/INGInious.css` & `INGInious-0.8.6/inginious/frontend/static/css/INGInious.css`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/css/INGInious.less` & `INGInious-0.8.6/inginious/frontend/static/css/INGInious.less`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/css/bootstrap-datetimepicker.min.css` & `INGInious-0.8.6/inginious/frontend/static/css/bootstrap-datetimepicker.min.css`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/css/bootstrap.min.css` & `INGInious-0.8.6/inginious/frontend/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/css/codemirror.css` & `INGInious-0.8.6/inginious/frontend/static/css/codemirror.css`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/css/common.less` & `INGInious-0.8.6/inginious/frontend/static/css/common.less`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/css/font-awesome.min.css` & `INGInious-0.8.6/inginious/frontend/static/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/css/lti.css` & `INGInious-0.8.6/inginious/frontend/static/css/lti.css`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/css/selectize.css` & `INGInious-0.8.6/inginious/frontend/static/css/selectize.css`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/fonts/FontAwesome.otf` & `INGInious-0.8.6/inginious/frontend/static/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/fonts/fontawesome-webfont.eot` & `INGInious-0.8.6/inginious/frontend/static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/fonts/fontawesome-webfont.svg` & `INGInious-0.8.6/inginious/frontend/static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/fonts/fontawesome-webfont.ttf` & `INGInious-0.8.6/inginious/frontend/static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/fonts/fontawesome-webfont.woff` & `INGInious-0.8.6/inginious/frontend/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/fonts/fontawesome-webfont.woff2` & `INGInious-0.8.6/inginious/frontend/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/fonts/glyphicons-halflings-regular.eot` & `INGInious-0.8.6/inginious/frontend/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/fonts/glyphicons-halflings-regular.svg` & `INGInious-0.8.6/inginious/frontend/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/fonts/glyphicons-halflings-regular.ttf` & `INGInious-0.8.6/inginious/frontend/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/fonts/glyphicons-halflings-regular.woff` & `INGInious-0.8.6/inginious/frontend/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/fonts/glyphicons-halflings-regular.woff2` & `INGInious-0.8.6/inginious/frontend/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/icons/apple-touch-icon-114x114.png` & `INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-114x114.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/icons/apple-touch-icon-120x120.png` & `INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-120x120.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/icons/apple-touch-icon-144x144.png` & `INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/icons/apple-touch-icon-152x152.png` & `INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-152x152.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/icons/apple-touch-icon-57x57.png` & `INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-57x57.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/icons/apple-touch-icon-60x60.png` & `INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-60x60.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/icons/apple-touch-icon-72x72.png` & `INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/icons/apple-touch-icon-76x76.png` & `INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-76x76.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/icons/apple-touch-icon-precomposed.png` & `INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon-precomposed.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/icons/apple-touch-icon.png` & `INGInious-0.8.6/inginious/frontend/static/icons/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/icons/favicon-160x160.png` & `INGInious-0.8.6/inginious/frontend/static/icons/favicon-160x160.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/icons/favicon-16x16.png` & `INGInious-0.8.6/inginious/frontend/static/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/icons/favicon-196x196.png` & `INGInious-0.8.6/inginious/frontend/static/icons/favicon-196x196.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/icons/favicon-32x32.png` & `INGInious-0.8.6/inginious/frontend/static/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/icons/favicon-96x96.png` & `INGInious-0.8.6/inginious/frontend/static/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/icons/favicon.ico` & `INGInious-0.8.6/inginious/frontend/static/icons/favicon.ico`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/icons/google-icon.svg` & `INGInious-0.8.6/inginious/frontend/static/icons/google-icon.svg`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/icons/mstile-144x144.png` & `INGInious-0.8.6/inginious/frontend/static/icons/mstile-144x144.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/icons/mstile-150x150.png` & `INGInious-0.8.6/inginious/frontend/static/icons/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/icons/mstile-310x150.png` & `INGInious-0.8.6/inginious/frontend/static/icons/mstile-310x150.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/icons/mstile-310x310.png` & `INGInious-0.8.6/inginious/frontend/static/icons/mstile-310x310.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/icons/mstile-70x70.png` & `INGInious-0.8.6/inginious/frontend/static/icons/mstile-70x70.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/icons/wb.png` & `INGInious-0.8.6/inginious/frontend/static/icons/wb.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/icons/wb.svg` & `INGInious-0.8.6/inginious/frontend/static/icons/wb.svg`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/images/header.png` & `INGInious-0.8.6/inginious/frontend/static/images/header.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/images/inginious_full.svg` & `INGInious-0.8.6/inginious/frontend/static/images/inginious_full.svg`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/images/inginious_full_logo_only.svg` & `INGInious-0.8.6/inginious/frontend/static/images/inginious_full_logo_only.svg`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/images/inginious_horiz.svg` & `INGInious-0.8.6/inginious/frontend/static/images/inginious_horiz.svg`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/images/inginious_vert.svg` & `INGInious-0.8.6/inginious/frontend/static/images/inginious_vert.svg`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/images/logo.png` & `INGInious-0.8.6/inginious/frontend/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/images/logo_maintenance.png` & `INGInious-0.8.6/inginious/frontend/static/images/logo_maintenance.png`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/admin.js` & `INGInious-0.8.6/inginious/frontend/static/js/admin.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/all-minified.js` & `INGInious-0.8.6/inginious/frontend/static/js/all-minified.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/audiences.js` & `INGInious-0.8.6/inginious/frontend/static/js/audiences.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/checked-list-group.js` & `INGInious-0.8.6/inginious/frontend/static/js/checked-list-group.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/LICENSE` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/LICENSE`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/codemirror.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/codemirror.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/apl/apl.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/apl/apl.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/apl/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/apl/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/asciiarmor/asciiarmor.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/asciiarmor/asciiarmor.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/asciiarmor/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/asciiarmor/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/asn.1/asn.1.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/asn.1/asn.1.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/asn.1/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/asn.1/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/asterisk/asterisk.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/asterisk/asterisk.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/asterisk/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/asterisk/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/brainfuck/brainfuck.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/brainfuck/brainfuck.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/brainfuck/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/brainfuck/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/clike/clike.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/clike/clike.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/clike/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/clike/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/clike/scala.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/clike/scala.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/clojure/clojure.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/clojure/clojure.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/clojure/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/clojure/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/cmake/cmake.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/cmake/cmake.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/cmake/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/cmake/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/cobol/cobol.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/cobol/cobol.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/cobol/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/cobol/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/coffeescript/coffeescript.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/coffeescript/coffeescript.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/coffeescript/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/coffeescript/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/commonlisp/commonlisp.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/commonlisp/commonlisp.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/commonlisp/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/commonlisp/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/crystal/crystal.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/crystal/crystal.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/crystal/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/crystal/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/css/css.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/css/css.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/css/gss.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/css/gss.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/css/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/css/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/css/less.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/css/less.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/css/less_test.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/css/less_test.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/css/scss.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/css/scss.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/css/scss_test.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/css/scss_test.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/cypher/cypher.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/cypher/cypher.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/cypher/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/cypher/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/d/d.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/d/d.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/d/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/d/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/dart/dart.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dart/dart.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/dart/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dart/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/diff/diff.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/diff/diff.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/diff/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/diff/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/django/django.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/django/django.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/django/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/django/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/dockerfile/dockerfile.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dockerfile/dockerfile.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/dockerfile/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dockerfile/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/dtd/dtd.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dtd/dtd.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/dtd/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dtd/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/dylan/dylan.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dylan/dylan.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/dylan/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/dylan/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/ebnf/ebnf.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ebnf/ebnf.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/ebnf/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ebnf/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/ecl/ecl.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ecl/ecl.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/ecl/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ecl/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/eiffel/eiffel.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/eiffel/eiffel.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/eiffel/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/eiffel/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/elm/elm.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/elm/elm.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/elm/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/elm/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/erlang/erlang.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/erlang/erlang.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/erlang/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/erlang/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/factor/factor.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/factor/factor.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/factor/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/factor/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/fcl/fcl.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/fcl/fcl.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/fcl/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/fcl/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/forth/forth.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/forth/forth.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/forth/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/forth/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/fortran/fortran.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/fortran/fortran.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/fortran/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/fortran/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/gas/gas.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/gas/gas.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/gas/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/gas/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/gfm/gfm.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/gfm/gfm.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/gfm/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/gfm/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/gherkin/gherkin.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/gherkin/gherkin.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/gherkin/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/gherkin/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/go/go.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/go/go.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/go/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/go/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/groovy/groovy.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/groovy/groovy.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/groovy/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/groovy/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/haml/haml.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haml/haml.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/haml/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haml/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/handlebars/handlebars.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/handlebars/handlebars.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/handlebars/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/handlebars/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/haskell/haskell.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haskell/haskell.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/haskell/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haskell/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/haskell-literate/haskell-literate.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haskell-literate/haskell-literate.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/haskell-literate/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haskell-literate/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/haxe/haxe.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haxe/haxe.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/haxe/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/haxe/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/htmlembedded/htmlembedded.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/htmlembedded/htmlembedded.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/htmlembedded/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/htmlembedded/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/htmlmixed/htmlmixed.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/htmlmixed/htmlmixed.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/htmlmixed/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/htmlmixed/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/http/http.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/http/http.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/http/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/http/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/idl/idl.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/idl/idl.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/idl/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/idl/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/javascript/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/javascript/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/javascript/javascript.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/javascript/javascript.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/javascript/json-ld.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/javascript/json-ld.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/javascript/typescript.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/javascript/typescript.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/jinja2/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/jinja2/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/jinja2/jinja2.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/jinja2/jinja2.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/jsx/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/jsx/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/jsx/jsx.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/jsx/jsx.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/julia/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/julia/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/julia/julia.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/julia/julia.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/livescript/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/livescript/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/livescript/livescript.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/livescript/livescript.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/lua/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/lua/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/lua/lua.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/lua/lua.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/markdown/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/markdown/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/markdown/markdown.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/markdown/markdown.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mathematica/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mathematica/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mathematica/mathematica.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mathematica/mathematica.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mbox/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mbox/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mbox/mbox.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mbox/mbox.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/meta.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/meta.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mirc/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mirc/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mirc/mirc.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mirc/mirc.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mllike/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mllike/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mllike/mllike.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mllike/mllike.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/modelica/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/modelica/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/modelica/modelica.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/modelica/modelica.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mscgen/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mscgen/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mscgen/mscgen.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mscgen/mscgen.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mscgen/mscgen_test.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mscgen/mscgen_test.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mscgen/msgenny_test.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mscgen/msgenny_test.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mscgen/xu_test.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mscgen/xu_test.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mumps/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mumps/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/mumps/mumps.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/mumps/mumps.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/nginx/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/nginx/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/nginx/nginx.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/nginx/nginx.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/nsis/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/nsis/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/nsis/nsis.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/nsis/nsis.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/ntriples/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ntriples/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/ntriples/ntriples.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ntriples/ntriples.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/octave/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/octave/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/octave/octave.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/octave/octave.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/oz/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/oz/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/oz/oz.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/oz/oz.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/pascal/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pascal/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/pascal/pascal.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pascal/pascal.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/pegjs/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pegjs/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/pegjs/pegjs.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pegjs/pegjs.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/perl/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/perl/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/perl/perl.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/perl/perl.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/php/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/php/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/php/php.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/php/php.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/pig/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pig/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/pig/pig.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pig/pig.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/powershell/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/powershell/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/powershell/powershell.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/powershell/powershell.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/properties/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/properties/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/properties/properties.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/properties/properties.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/protobuf/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/protobuf/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/protobuf/protobuf.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/protobuf/protobuf.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/pug/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pug/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/pug/pug.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/pug/pug.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/puppet/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/puppet/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/puppet/puppet.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/puppet/puppet.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/python/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/python/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/python/python.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/python/python.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/q/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/q/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/q/q.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/q/q.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/r/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/r/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/r/r.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/r/r.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/rpm/changes/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rpm/changes/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/rpm/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rpm/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/rpm/rpm.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rpm/rpm.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/rst/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rst/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/rst/rst.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rst/rst.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/ruby/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ruby/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/ruby/ruby.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ruby/ruby.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/rust/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rust/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/rust/rust.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/rust/rust.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/sas/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sas/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/sas/sas.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sas/sas.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/sass/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sass/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/sass/sass.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sass/sass.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/scheme/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/scheme/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/scheme/scheme.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/scheme/scheme.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/shell/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/shell/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/shell/shell.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/shell/shell.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/sieve/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sieve/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/sieve/sieve.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sieve/sieve.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/slim/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/slim/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/slim/slim.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/slim/slim.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/smalltalk/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/smalltalk/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/smalltalk/smalltalk.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/smalltalk/smalltalk.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/smarty/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/smarty/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/smarty/smarty.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/smarty/smarty.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/solr/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/solr/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/solr/solr.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/solr/solr.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/soy/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/soy/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/soy/soy.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/soy/soy.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/sparql/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sparql/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/sparql/sparql.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sparql/sparql.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/spreadsheet/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/spreadsheet/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/spreadsheet/spreadsheet.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/spreadsheet/spreadsheet.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/sql/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sql/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/sql/sql.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/sql/sql.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/stex/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/stex/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/stex/stex.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/stex/stex.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/stylus/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/stylus/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/stylus/stylus.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/stylus/stylus.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/swift/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/swift/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/swift/swift.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/swift/swift.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/tcl/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tcl/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/tcl/tcl.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tcl/tcl.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/textile/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/textile/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/textile/textile.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/textile/textile.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/tiddlywiki/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tiddlywiki/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/tiddlywiki/tiddlywiki.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tiddlywiki/tiddlywiki.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/tiki/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tiki/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/tiki/tiki.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tiki/tiki.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/toml/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/toml/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/toml/toml.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/toml/toml.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/tornado/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tornado/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/tornado/tornado.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/tornado/tornado.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/troff/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/troff/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/troff/troff.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/troff/troff.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/ttcn/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ttcn/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/ttcn/ttcn.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ttcn/ttcn.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/ttcn-cfg/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ttcn-cfg/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/ttcn-cfg/ttcn-cfg.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/ttcn-cfg/ttcn-cfg.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/turtle/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/turtle/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/turtle/turtle.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/turtle/turtle.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/twig/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/twig/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/twig/twig.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/twig/twig.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/vb/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vb/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/vb/vb.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vb/vb.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/vbscript/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vbscript/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/vbscript/vbscript.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vbscript/vbscript.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/velocity/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/velocity/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/velocity/velocity.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/velocity/velocity.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/verilog/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/verilog/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/verilog/verilog.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/verilog/verilog.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/vhdl/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vhdl/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/vhdl/vhdl.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vhdl/vhdl.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/vue/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vue/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/vue/vue.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/vue/vue.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/webidl/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/webidl/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/webidl/webidl.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/webidl/webidl.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/xml/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/xml/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/xml/xml.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/xml/xml.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/xquery/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/xquery/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/xquery/xquery.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/xquery/xquery.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/yacas/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/yacas/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/yacas/yacas.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/yacas/yacas.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/yaml/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/yaml/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/yaml/yaml.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/yaml/yaml.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/yaml-frontmatter/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/yaml-frontmatter/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/yaml-frontmatter/yaml-frontmatter.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/yaml-frontmatter/yaml-frontmatter.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/z80/index.html` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/z80/index.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/codemirror/mode/z80/z80.js` & `INGInious-0.8.6/inginious/frontend/static/js/codemirror/mode/z80/z80.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/common.js` & `INGInious-0.8.6/inginious/frontend/static/js/common.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/groups.js` & `INGInious-0.8.6/inginious/frontend/static/js/groups.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/libs/Sortable.min.js` & `INGInious-0.8.6/inginious/frontend/static/js/libs/Sortable.min.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/libs/bootstrap-datetimepicker.min.js` & `INGInious-0.8.6/inginious/frontend/static/js/libs/bootstrap-datetimepicker.min.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/libs/bootstrap.min.js` & `INGInious-0.8.6/inginious/frontend/static/js/libs/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/libs/chart.min.js` & `INGInious-0.8.6/inginious/frontend/static/js/libs/chart.min.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/libs/jquery.form.min.js` & `INGInious-0.8.6/inginious/frontend/static/js/libs/jquery.form.min.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/libs/jquery.min.js` & `INGInious-0.8.6/inginious/frontend/static/js/libs/jquery.min.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/libs/jquery.twbsPagination.min.js` & `INGInious-0.8.6/inginious/frontend/static/js/libs/jquery.twbsPagination.min.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/libs/moment.min.js` & `INGInious-0.8.6/inginious/frontend/static/js/libs/moment.min.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/libs/popper.min.js` & `INGInious-0.8.6/inginious/frontend/static/js/libs/popper.min.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/libs/selectize.min.js` & `INGInious-0.8.6/inginious/frontend/static/js/libs/selectize.min.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/libs/sentry-io-bundle.min.js` & `INGInious-0.8.6/inginious/frontend/static/js/libs/sentry-io-bundle.min.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/studio.js` & `INGInious-0.8.6/inginious/frontend/static/js/studio.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/task.js` & `INGInious-0.8.6/inginious/frontend/static/js/task.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/task_dispensers.js` & `INGInious-0.8.6/inginious/frontend/static/js/task_dispensers.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/js/webapp.js` & `INGInious-0.8.6/inginious/frontend/static/js/webapp.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/plugins/contests/contests.js` & `INGInious-0.8.6/inginious/frontend/static/plugins/contests/contests.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/plugins/contests/jquery.countdown.min.js` & `INGInious-0.8.6/inginious/frontend/static/plugins/contests/jquery.countdown.min.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/static/plugins/contests/scoreboard.css` & `INGInious-0.8.6/inginious/frontend/static/plugins/contests/scoreboard.css`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/submission_manager.py` & `INGInious-0.8.6/inginious/frontend/submission_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,24 +72,34 @@
             "ssh_host": "",
             "ssh_port": "",
             "ssh_user": "",
             "ssh_password": ""
         }
 
         # Save submission to database
-        submission = self._database.submissions.find_one_and_update(
-            {"_id": submission["_id"]},
-            {"$set": data, "$unset": unset_obj},
-            return_document=ReturnDocument.AFTER
-        )
+        try:
+            submission = self._database.submissions.find_one_and_update(
+                {"_id": submission["_id"]},
+                {"$set": data, "$unset": unset_obj},
+                return_document=ReturnDocument.AFTER
+            )
 
-        self._plugin_manager.call_hook("submission_done", submission=submission, archive=archive, newsub=newsub)
+            for username in submission["username"]:
+                self._user_manager.update_user_stats(username, task, submission, result[0], grade, state, newsub)
 
-        for username in submission["username"]:
-            self._user_manager.update_user_stats(username, task, submission, result[0], grade, state, newsub)
+        # Check for size as it also takes the MongoDB command into consideration
+        except pymongo.errors.DocumentTooLarge:
+            data = {"status": "error", "text": _("Maximum submission size exceeded. Check feedback, stdout, stderr and state."), "grade": 0.0}
+            submission = self._database.submissions.find_one_and_update(
+                {"_id": submission["_id"]},
+                {"$set": data, "$unset": unset_obj},
+                return_document=ReturnDocument.AFTER
+            )
+
+        self._plugin_manager.call_hook("submission_done", submission=submission, archive=archive, newsub=newsub)
 
         if "outcome_service_url" in submission and "outcome_result_id" in submission and "outcome_consumer_key" in submission:
             for username in submission["username"]:
                 self._lti_outcome_manager.add(username,
                                               submission["courseid"],
                                               submission["taskid"],
                                               submission["outcome_consumer_key"],
```

### Comparing `INGInious-0.8.5/inginious/frontend/task_dispensers/__init__.py` & `INGInious-0.8.6/inginious/frontend/task_dispensers/__init__.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/task_dispensers/combinatory_test.py` & `INGInious-0.8.6/inginious/frontend/task_dispensers/combinatory_test.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/task_dispensers/toc.py` & `INGInious-0.8.6/inginious/frontend/task_dispensers/toc.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/task_dispensers/util.py` & `INGInious-0.8.6/inginious/frontend/task_dispensers/util.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/task_factory.py` & `INGInious-0.8.6/inginious/frontend/task_factory.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/task_problems.py` & `INGInious-0.8.6/inginious/frontend/task_problems.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/tasks.py` & `INGInious-0.8.6/inginious/frontend/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,19 @@
         content["environment_id"] = content["environment"]
         content["environment_type"] = "docker" if content["environment_id"] != "mcq" else "mcq"
         del content["environment"]
         content["environment_parameters"] = {"limits": content.get("limits", {}),
                                              "run_cmd": content.get("run_cmd", ''),
                                              "network_grading": content.get("network_grading", False),
                                              "response_is_html": content.get('responseIsHTML', False)}
+
+    # Retrocompatibility v0.8.5
+    if content.get("environment_parameters", {}).get("ssh_allowed", False):
+        content["environment_type"] = content["environment_type"] + "-ssh"
+
     return content
 
 
 class Task(object):
     """ A task that stores additional context information, specific to the web app """
 
     def __init__(self, course, taskid, content, filesystem, plugin_manager, task_problem_types):
```

### Comparing `INGInious-0.8.5/inginious/frontend/template_helper.py` & `INGInious-0.8.6/inginious/frontend/template_helper.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/admin/admin_users.html` & `INGInious-0.8.6/inginious/frontend/templates/admin/admin_users.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/auth.html` & `INGInious-0.8.6/inginious/frontend/templates/auth.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course.html` & `INGInious-0.8.6/inginious/frontend/templates/course.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/audience_edit.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/audience_edit.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/danger_zone.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/danger_zone.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/edit_tabs/basic.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/edit_tabs/basic.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/edit_tabs/env_generic_docker_oci.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/edit_tabs/env_generic_docker_oci.html`

 * *Files 9% similar despite different names*

```diff
@@ -26,24 +26,14 @@
     <div class="col-sm-8">
         <div class="checkbox"><label>
             <input type="checkbox" id="{{env_id}}-network-grading" name="envparams[{{env_id}}][network_grading]"
                    {{'checked="checked"' if env_params.get('network_grading',False) }} />&nbsp;
         </label></div>
     </div>
 </div>
-<div class="form-group row">
-    <label for="{{env_id}}-ssh-allowed" class="col-sm-4 control-label">{{ _("Allow ssh?") }}</label>
-
-    <div class="col-sm-8">
-        <div class="checkbox"><label>
-            <input type="checkbox" id="{{env_id}}-ssh-allowed" name="envparams[{{env_id}}][ssh_allowed]"
-                   {{'checked="checked"' if env_params.get('ssh_allowed',False) }} />&nbsp;
-        </label></div>
-    </div>
-</div>
 
 <div class="form-group row">
     <label for="{{env_id}}-run-cmd" class="col-sm-4 control-label">{{ _("Custom command to be run in container <small>(instead of running the run script)</small>") | safe}}</label>
 
     <div class="col-sm-8">
         <input type="text" class="form-control" id="{{env_id}}-run-cmd" name="envparams[{{env_id}}][run_cmd]" placeholder="{{ _('Optional') }}" value="{{env_params.get('run_cmd','')}}"/>
     </div>
```

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/edit_tabs/environment.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/edit_tabs/environment.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/edit_tabs/file_modals.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/edit_tabs/file_modals.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/edit_tabs/files.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/edit_tabs/files.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/edit_tabs/subproblems.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/edit_tabs/subproblems.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/menu.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/menu.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/settings.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/settings.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/stats.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/stats.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/student_info.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/student_info.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/student_list.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/student_list.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/student_list_table.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/student_list_table.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/submission.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/submission.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/submissions.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/submissions.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/submissions_query.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/submissions_query.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/subproblems/code.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/subproblems/code.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/subproblems/file.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/subproblems/file.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/subproblems/match.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/subproblems/match.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/subproblems/multiple_choice.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/subproblems/multiple_choice.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/subproblems/multiple_choice_templates.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/subproblems/multiple_choice_templates.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/tags.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/tags.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/task_dispensers/combinatory_test.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/combinatory_test.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/task_dispensers/empty_section.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/empty_section.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/task_dispensers/section.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/section.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/task_dispensers/section_config.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/section_config.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/task_dispensers/section_menu.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/section_menu.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/task_dispensers/task_buttons.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/task_buttons.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/task_dispensers/task_list.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/task_list.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/task_dispensers/toc.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/toc.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/task_dispensers/util.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/util.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/task_dispensers/util_delete_modal.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/task_dispensers/util_delete_modal.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/task_edit.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/task_edit.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_admin/task_list.html` & `INGInious-0.8.6/inginious/frontend/templates/course_admin/task_list.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_register.html` & `INGInious-0.8.6/inginious/frontend/templates/course_register.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/course_unavailable.html` & `INGInious-0.8.6/inginious/frontend/templates/course_unavailable.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/courselist.html` & `INGInious-0.8.6/inginious/frontend/templates/courselist.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/group.html` & `INGInious-0.8.6/inginious/frontend/templates/group.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/internalerror.html` & `INGInious-0.8.6/inginious/frontend/templates/internalerror.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/layout.html` & `INGInious-0.8.6/inginious/frontend/templates/layout.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/lti_bind.html` & `INGInious-0.8.6/inginious/frontend/templates/lti_bind.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/lti_login.html` & `INGInious-0.8.6/inginious/frontend/templates/lti_login.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/maintenance.html` & `INGInious-0.8.6/inginious/frontend/templates/maintenance.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/marketplace.html` & `INGInious-0.8.6/inginious/frontend/templates/marketplace.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/marketplace_course.html` & `INGInious-0.8.6/inginious/frontend/templates/marketplace_course.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/mycourses.html` & `INGInious-0.8.6/inginious/frontend/templates/mycourses.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/preferences/bindings.html` & `INGInious-0.8.6/inginious/frontend/templates/preferences/bindings.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/preferences/delete.html` & `INGInious-0.8.6/inginious/frontend/templates/preferences/delete.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/preferences/profile.html` & `INGInious-0.8.6/inginious/frontend/templates/preferences/profile.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/queue.html` & `INGInious-0.8.6/inginious/frontend/templates/queue.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/register.html` & `INGInious-0.8.6/inginious/frontend/templates/register.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/signin_button.html` & `INGInious-0.8.6/inginious/frontend/templates/signin_button.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/task.html` & `INGInious-0.8.6/inginious/frontend/templates/task.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/task_dispensers/task_list.html` & `INGInious-0.8.6/inginious/frontend/templates/task_dispensers/task_list.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/task_dispensers/toc.html` & `INGInious-0.8.6/inginious/frontend/templates/task_dispensers/toc.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/task_unavailable.html` & `INGInious-0.8.6/inginious/frontend/templates/task_unavailable.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/tasks/code.html` & `INGInious-0.8.6/inginious/frontend/templates/tasks/code.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/tasks/file.html` & `INGInious-0.8.6/inginious/frontend/templates/tasks/file.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/tasks/multiple_choice.html` & `INGInious-0.8.6/inginious/frontend/templates/tasks/multiple_choice.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/tasks/single_line_code.html` & `INGInious-0.8.6/inginious/frontend/templates/tasks/single_line_code.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/templates/unregister_modal.html` & `INGInious-0.8.6/inginious/frontend/templates/unregister_modal.html`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/tests/SeleniumFormatter.js` & `INGInious-0.8.6/inginious/frontend/tests/SeleniumFormatter.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/tests/SeleniumTest.py` & `INGInious-0.8.6/inginious/frontend/tests/SeleniumTest.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/tests/TestCourse.py` & `INGInious-0.8.6/inginious/frontend/tests/TestCourse.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/tests/TestLogin.py` & `INGInious-0.8.6/inginious/frontend/tests/TestLogin.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/tests/TestParsableText.py` & `INGInious-0.8.6/inginious/frontend/tests/TestParsableText.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/tests/TestPluginManager.py` & `INGInious-0.8.6/inginious/frontend/tests/TestPluginManager.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/tests/TestTask.py` & `INGInious-0.8.6/inginious/frontend/tests/TestTask.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/tests/TestTaskDisplay.py` & `INGInious-0.8.6/inginious/frontend/tests/TestTaskDisplay.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/tests/TestTaskSubmission.py` & `INGInious-0.8.6/inginious/frontend/tests/TestTaskSubmission.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/tests/tasks/test/task1/task.yaml` & `INGInious-0.8.6/inginious/frontend/tests/tasks/test/task1/task.yaml`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/tests/tasks/test2/task3/task.yaml` & `INGInious-0.8.6/inginious/frontend/tests/tasks/test2/task3/task.yaml`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/user_manager.py` & `INGInious-0.8.6/inginious/frontend/user_manager.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious/frontend/webdav.py` & `INGInious-0.8.6/inginious/frontend/webdav.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious-agent-docker` & `INGInious-0.8.6/inginious-agent-docker`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious-agent-mcq` & `INGInious-0.8.6/inginious-agent-mcq`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious-autotest` & `INGInious-0.8.6/inginious-autotest`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious-backend` & `INGInious-0.8.6/inginious-backend`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious-install` & `INGInious-0.8.6/inginious-install`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious-webapp` & `INGInious-0.8.6/inginious-webapp`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/inginious-webdav` & `INGInious-0.8.6/inginious-webdav`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/setup.py` & `INGInious-0.8.6/setup.py`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/utils/container_update/inginious-container-update` & `INGInious-0.8.6/utils/container_update/inginious-container-update`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/utils/database_updater/inginious-database-update` & `INGInious-0.8.6/utils/database_updater/inginious-database-update`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/utils/minify/Gruntfile.js` & `INGInious-0.8.6/utils/minify/Gruntfile.js`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/utils/minify/watchers.xml` & `INGInious-0.8.6/utils/minify/watchers.xml`

 * *Files identical despite different names*

### Comparing `INGInious-0.8.5/utils/sync/inginious-synchronize` & `INGInious-0.8.6/utils/sync/inginious-synchronize`

 * *Files identical despite different names*

