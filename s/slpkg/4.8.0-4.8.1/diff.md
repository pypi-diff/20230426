# Comparing `tmp/slpkg-4.8.0.tar.gz` & `tmp/slpkg-4.8.1.tar.gz`

## Comparing `slpkg-4.8.0.tar` & `slpkg-4.8.1.tar`

### file list

```diff
@@ -1,98 +1,101 @@
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-21 14:30:41.000000 slpkg-4.8.0/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/filelists/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/filelists/multilib/
--rw-r--r--   0 dslackw   (1000) users      (100)    15477 2023-04-21 14:24:01.000000 slpkg-4.8.0/filelists/multilib/README.ERIC
--rw-r--r--   0 dslackw   (1000) users      (100)      250 2023-04-21 14:24:01.000000 slpkg-4.8.0/filelists/multilib/glibc_packages.pkgs
--rw-r--r--   0 dslackw   (1000) users      (100)      831 2023-04-21 14:24:01.000000 slpkg-4.8.0/filelists/multilib/README
--rw-r--r--   0 dslackw   (1000) users      (100)     4508 2023-04-21 14:24:01.000000 slpkg-4.8.0/filelists/multilib/compat32.pkgs
--rw-r--r--   0 dslackw   (1000) users      (100)       88 2023-04-21 14:24:01.000000 slpkg-4.8.0/filelists/README
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/slackbuild/
--rw-r--r--   0 dslackw   (1000) users      (100)      941 2023-04-21 14:24:01.000000 slpkg-4.8.0/slackbuild/slack-desc
--rw-r--r--   0 dslackw   (1000) users      (100)      432 2023-04-21 14:24:01.000000 slpkg-4.8.0/slackbuild/doinst.sh
--rw-r--r--   0 dslackw   (1000) users      (100)      304 2023-04-21 14:24:01.000000 slpkg-4.8.0/slackbuild/README
--rwxr-xr-x   0 dslackw   (1000) users      (100)     4280 2023-04-21 14:24:01.000000 slpkg-4.8.0/slackbuild/slpkg.SlackBuild
--rwxr-xr-x   0 dslackw   (1000) users      (100)       70 2023-04-21 14:24:01.000000 slpkg-4.8.0/setup.py
--rw-r--r--   0 dslackw   (1000) users      (100)     7920 2023-04-21 14:30:35.000000 slpkg-4.8.0/README.rst
--rw-r--r--   0 dslackw   (1000) users      (100)       84 2023-04-21 14:24:01.000000 slpkg-4.8.0/requirements.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/configs/
--rw-r--r--   0 dslackw   (1000) users      (100)     9164 2023-04-21 14:24:01.000000 slpkg-4.8.0/configs/repositories.toml
--rw-r--r--   0 dslackw   (1000) users      (100)      483 2023-04-21 14:24:01.000000 slpkg-4.8.0/configs/blacklist.toml
--rw-r--r--   0 dslackw   (1000) users      (100)     3634 2023-04-21 14:24:01.000000 slpkg-4.8.0/configs/slpkg.toml
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/tests/
--rw-r--r--   0 dslackw   (1000) users      (100)     2340 2023-04-21 14:24:01.000000 slpkg-4.8.0/tests/test_configs.py
--rw-r--r--   0 dslackw   (1000) users      (100)      770 2023-04-21 14:24:01.000000 slpkg-4.8.0/tests/test_checks.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1891 2023-04-21 14:24:01.000000 slpkg-4.8.0/tests/test_utilities.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1455 2023-04-21 14:24:01.000000 slpkg-4.8.0/tests/test_sbo_queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)      255 2023-04-21 14:24:01.000000 slpkg-4.8.0/tests/test_blacklist.py
--rw-r--r--   0 dslackw   (1000) users      (100)      588 2023-04-21 14:24:01.000000 slpkg-4.8.0/tests/test_colors.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1567 2023-04-21 14:24:01.000000 slpkg-4.8.0/tests/test_upgrade.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1787 2023-04-21 14:24:01.000000 slpkg-4.8.0/tests/test_bin_queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1076 2023-04-21 14:24:01.000000 slpkg-4.8.0/LICENSE
--rwxr-xr-x   0 dslackw   (1000) users      (100)     1773 2023-04-21 14:24:01.000000 slpkg-4.8.0/install.sh
--rw-r--r--   0 dslackw   (1000) users      (100)    45268 2023-04-21 14:24:01.000000 slpkg-4.8.0/ChangeLog.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/man/
--rw-r--r--   0 dslackw   (1000) users      (100)     8987 2023-04-21 14:24:01.000000 slpkg-4.8.0/man/slpkg.1
--rw-r--r--   0 dslackw   (1000) users      (100)     9918 2023-04-21 14:24:01.000000 slpkg-4.8.0/man/slpkg-fr.1
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/completion/
--rw-r--r--   0 dslackw   (1000) users      (100)      910 2023-04-21 14:24:01.000000 slpkg-4.8.0/completion/slpkg
--rw-r--r--   0 dslackw   (1000) users      (100)       93 2023-04-21 14:24:01.000000 slpkg-4.8.0/.gitignore
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/
--rw-r--r--   0 dslackw   (1000) users      (100)     3983 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/dialog_configs.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/binaries/
--rw-r--r--   0 dslackw   (1000) users      (100)     1574 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/binaries/required.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2110 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/binaries/queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/binaries/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     9605 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/binaries/install.py
--rw-r--r--   0 dslackw   (1000) users      (100)    63573 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/install_data.py
--rw-r--r--   0 dslackw   (1000) users      (100)    27456 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/repositories.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2463 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/repo_info.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/sbos/
--rw-r--r--   0 dslackw   (1000) users      (100)     1368 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/sbos/queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)    14873 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/sbos/slackbuild.py
--rw-r--r--   0 dslackw   (1000) users      (100)      924 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/sbos/dependencies.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/sbos/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)    34184 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/update_repository.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1791 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/progress_bar.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2391 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/downloader.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/models/
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/models/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2630 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/models/models.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/views/
--rw-r--r--   0 dslackw   (1000) users      (100)     7070 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/views/view_package.py
--rw-r--r--   0 dslackw   (1000) users      (100)      629 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/views/version.py
--rw-r--r--   0 dslackw   (1000) users      (100)     6319 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/views/cli_menu.py
--rw-r--r--   0 dslackw   (1000) users      (100)     5553 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/views/ascii.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4043 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/views/help_commands.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/views/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     9827 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/views/views.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3029 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/checks.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1344 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/checksum.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2196 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/dialog_box.py
--rw-r--r--   0 dslackw   (1000) users      (100)     5193 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/configs.py
--rw-r--r--   0 dslackw   (1000) users      (100)      902 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/clean_logs.py
--rw-r--r--   0 dslackw   (1000) users      (100)     7000 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/utilities.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3970 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/dependees.py
--rw-r--r--   0 dslackw   (1000) users      (100)    11207 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/check_updates.py
--rw-r--r--   0 dslackw   (1000) users      (100)     5690 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/remove_packages.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1521 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/blacklist.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2603 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/download_only.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3043 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/tracking.py
--rw-r--r--   0 dslackw   (1000) users      (100)      245 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/logging_config.py
--rw-r--r--   0 dslackw   (1000) users      (100)    29938 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/main.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1423 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/find_installed.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3206 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/upgrade.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2872 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/search.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1354 2023-04-21 14:24:01.000000 slpkg-4.8.0/setup.cfg
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-21 14:29:47.000000 slpkg-4.8.0/slpkg.egg-info/
--rw-r--r--   0 dslackw   (1000) users      (100)        1 2023-04-21 14:29:47.000000 slpkg-4.8.0/slpkg.egg-info/dependency_links.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     1107 2023-04-21 14:29:47.000000 slpkg-4.8.0/slpkg.egg-info/SOURCES.txt
--rw-r--r--   0 dslackw   (1000) users      (100)        6 2023-04-21 14:29:47.000000 slpkg-4.8.0/slpkg.egg-info/top_level.txt
--rw-r--r--   0 dslackw   (1000) users      (100)       77 2023-04-21 14:29:47.000000 slpkg-4.8.0/slpkg.egg-info/requires.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     1262 2023-04-21 14:29:47.000000 slpkg-4.8.0/slpkg.egg-info/PKG-INFO
--rw-r--r--   0 dslackw   (1000) users      (100)     8453 2023-04-21 14:24:01.000000 slpkg-4.8.0/README.md
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/tools/
--rwxr-xr-x   0 dslackw   (1000) users      (100)      787 2023-04-21 14:24:01.000000 slpkg-4.8.0/tools/gen_sbo_txt.sh
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/bin/
--rwxr-xr-x   0 dslackw   (1000) users      (100)    11470 2023-04-21 14:24:01.000000 slpkg-4.8.0/bin/slpkg_new-configs
--rwxr-xr-x   0 dslackw   (1000) users      (100)      184 2023-04-21 14:24:01.000000 slpkg-4.8.0/bin/slpkg
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-25 15:26:51.000000 slpkg-4.8.1/
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/filelists/
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/filelists/multilib/
+-rw-r--r--   0 dslackw   (1000) users      (100)    15477 2023-04-25 15:23:48.000000 slpkg-4.8.1/filelists/multilib/README.ERIC
+-rw-r--r--   0 dslackw   (1000) users      (100)      250 2023-04-25 15:23:48.000000 slpkg-4.8.1/filelists/multilib/glibc_packages.pkgs
+-rw-r--r--   0 dslackw   (1000) users      (100)      831 2023-04-25 15:23:48.000000 slpkg-4.8.1/filelists/multilib/README
+-rw-r--r--   0 dslackw   (1000) users      (100)     4508 2023-04-25 15:23:48.000000 slpkg-4.8.1/filelists/multilib/compat32.pkgs
+-rw-r--r--   0 dslackw   (1000) users      (100)       88 2023-04-25 15:23:48.000000 slpkg-4.8.1/filelists/README
+-rw-r--r--   0 dslackw   (1000) users      (100)     1189 2023-04-25 15:23:48.000000 slpkg-4.8.1/repositories.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/slackbuild/
+-rw-r--r--   0 dslackw   (1000) users      (100)      941 2023-04-25 15:23:48.000000 slpkg-4.8.1/slackbuild/slack-desc
+-rw-r--r--   0 dslackw   (1000) users      (100)      432 2023-04-25 15:23:48.000000 slpkg-4.8.1/slackbuild/doinst.sh
+-rw-r--r--   0 dslackw   (1000) users      (100)      304 2023-04-25 15:23:48.000000 slpkg-4.8.1/slackbuild/README
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     4297 2023-04-25 15:23:48.000000 slpkg-4.8.1/slackbuild/slpkg.SlackBuild
+-rwxr-xr-x   0 dslackw   (1000) users      (100)       70 2023-04-25 15:23:48.000000 slpkg-4.8.1/setup.py
+-rw-r--r--   0 dslackw   (1000) users      (100)       84 2023-04-25 15:23:48.000000 slpkg-4.8.1/requirements.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/configs/
+-rw-r--r--   0 dslackw   (1000) users      (100)     8285 2023-04-25 15:23:48.000000 slpkg-4.8.1/configs/repositories.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)      483 2023-04-25 15:23:48.000000 slpkg-4.8.1/configs/blacklist.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)     3731 2023-04-25 15:23:48.000000 slpkg-4.8.1/configs/slpkg.toml
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/tests/
+-rw-r--r--   0 dslackw   (1000) users      (100)     2340 2023-04-25 15:23:48.000000 slpkg-4.8.1/tests/test_configs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      770 2023-04-25 15:23:48.000000 slpkg-4.8.1/tests/test_checks.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1891 2023-04-25 15:23:48.000000 slpkg-4.8.1/tests/test_utilities.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1455 2023-04-25 15:23:48.000000 slpkg-4.8.1/tests/test_sbo_queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      255 2023-04-25 15:23:48.000000 slpkg-4.8.1/tests/test_blacklist.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      898 2023-04-25 15:23:48.000000 slpkg-4.8.1/tests/test_colors.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      890 2023-04-25 15:23:48.000000 slpkg-4.8.1/tests/check_updates_test.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1567 2023-04-25 15:23:48.000000 slpkg-4.8.1/tests/test_upgrade.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1787 2023-04-25 15:23:48.000000 slpkg-4.8.1/tests/test_bin_queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1076 2023-04-25 15:23:48.000000 slpkg-4.8.1/LICENSE
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     1773 2023-04-25 15:23:48.000000 slpkg-4.8.1/install.sh
+-rw-r--r--   0 dslackw   (1000) users      (100)    45524 2023-04-25 15:23:48.000000 slpkg-4.8.1/ChangeLog.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/man/
+-rw-r--r--   0 dslackw   (1000) users      (100)     8987 2023-04-25 15:23:48.000000 slpkg-4.8.1/man/slpkg.1
+-rw-r--r--   0 dslackw   (1000) users      (100)     9918 2023-04-25 15:23:48.000000 slpkg-4.8.1/man/slpkg-fr.1
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/completion/
+-rw-r--r--   0 dslackw   (1000) users      (100)      910 2023-04-25 15:23:48.000000 slpkg-4.8.1/completion/slpkg
+-rw-r--r--   0 dslackw   (1000) users      (100)       93 2023-04-25 15:23:48.000000 slpkg-4.8.1/.gitignore
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/
+-rw-r--r--   0 dslackw   (1000) users      (100)     4007 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/dialog_configs.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/binaries/
+-rw-r--r--   0 dslackw   (1000) users      (100)     1623 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/binaries/required.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2110 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/binaries/queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/binaries/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     9345 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/binaries/install.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    63301 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/install_data.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    26741 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/repositories.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2016 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/repo_info.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/sbos/
+-rw-r--r--   0 dslackw   (1000) users      (100)     1368 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/sbos/queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    14622 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/sbos/slackbuild.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      974 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/sbos/dependencies.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/sbos/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    30467 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/update_repository.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1395 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/progress_bar.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2476 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/downloader.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/models/
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/models/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2630 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/models/models.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/views/
+-rw-r--r--   0 dslackw   (1000) users      (100)     6721 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/views/view_package.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      629 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/views/version.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     6096 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/views/cli_menu.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     5053 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/views/ascii.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3810 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/views/help_commands.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/views/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     9528 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/views/views.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      387 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/error_messages.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3386 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/checks.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1416 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/checksum.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2196 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/dialog_box.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4324 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/configs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      902 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/clean_logs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     6462 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/utilities.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3607 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/dependees.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      587 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/toml_error_message.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4815 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/check_updates.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     5384 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/remove_packages.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      939 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/blacklist.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2603 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/download_only.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2828 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/tracking.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      245 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/logging_config.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    29954 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/main.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1117 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/find_installed.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3206 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/upgrade.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2610 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/search.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1354 2023-04-25 15:23:48.000000 slpkg-4.8.1/setup.cfg
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-25 15:26:48.000000 slpkg-4.8.1/slpkg.egg-info/
+-rw-r--r--   0 dslackw   (1000) users      (100)        1 2023-04-25 15:26:48.000000 slpkg-4.8.1/slpkg.egg-info/dependency_links.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     1159 2023-04-25 15:26:48.000000 slpkg-4.8.1/slpkg.egg-info/SOURCES.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)        6 2023-04-25 15:26:48.000000 slpkg-4.8.1/slpkg.egg-info/top_level.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)       77 2023-04-25 15:26:48.000000 slpkg-4.8.1/slpkg.egg-info/requires.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     1262 2023-04-25 15:26:48.000000 slpkg-4.8.1/slpkg.egg-info/PKG-INFO
+-rw-r--r--   0 dslackw   (1000) users      (100)     8518 2023-04-25 15:23:48.000000 slpkg-4.8.1/README.md
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/tools/
+-rwxr-xr-x   0 dslackw   (1000) users      (100)      787 2023-04-25 15:23:48.000000 slpkg-4.8.1/tools/gen_sbo_txt.sh
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/bin/
+-rwxr-xr-x   0 dslackw   (1000) users      (100)    11352 2023-04-25 15:23:48.000000 slpkg-4.8.1/bin/slpkg_new-configs
+-rwxr-xr-x   0 dslackw   (1000) users      (100)      184 2023-04-25 15:23:48.000000 slpkg-4.8.1/bin/slpkg
```

### Comparing `slpkg-4.8.0/filelists/multilib/README.ERIC` & `slpkg-4.8.1/filelists/multilib/README.ERIC`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.0/filelists/multilib/README` & `slpkg-4.8.1/filelists/multilib/README`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.0/filelists/multilib/compat32.pkgs` & `slpkg-4.8.1/filelists/multilib/compat32.pkgs`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.0/slackbuild/slack-desc` & `slpkg-4.8.1/slackbuild/slack-desc`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.0/slackbuild/slpkg.SlackBuild` & `slpkg-4.8.1/slackbuild/slpkg.SlackBuild`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 cp man/slpkg.1 $PKG/usr/man/man1
 cp man/slpkg-fr.1 $PKG/usr/man/fr/man1/slpkg.1
 
 find $PKG/usr/man -type f -exec gzip -9 {} \;
 for i in $( find $PKG/usr/man -type l ) ; do ln -s $( readlink $i ).gz $i.gz; rm $i ; done
 
 mkdir -p $PKG/usr/doc/$PRGNAM-$VERSION
-cp -a README.md ChangeLog.txt LICENSE requirements.txt $PKG/usr/doc/$PRGNAM-$VERSION
+cp -a README.md ChangeLog.txt LICENSE requirements.txt repositories.txt $PKG/usr/doc/$PRGNAM-$VERSION
 cat $CWD/$PRGNAM.SlackBuild > $PKG/usr/doc/$PRGNAM-$VERSION/$PRGNAM.SlackBuild
 
 mkdir -p $PKG/install
 cat $CWD/slack-desc > $PKG/install/slack-desc
 cat $CWD/doinst.sh > $PKG/install/doinst.sh
 
 cd $PKG
```

### Comparing `slpkg-4.8.0/configs/repositories.toml` & `slpkg-4.8.1/configs/repositories.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,34 @@
-################# REPOSITORIES CONFIGURATION FILE ######################
-# The philosophy behind this is to have two repositories for           #
-# Slackbuilds one for the Slackware stable and one for the -current    #
-# and many binaries for all versions.                                  #
-# Set 'true' to 'PONCE_REPO' to switch with the ponce repository.      #
-# Set 'true' to the binaries repositories you want to enable.          #
-# Default is the 'sbo' Slackbuilds.org repository.                     #
-########################################################################
-
-########################################################################
-# If you are going to use a local repository, set the mirror:          #
-# Example: ["file:///path/to/alien/repository/" ,"15.0/", "x86_64/"]   #
-#                                                                      #
-# A binary local repository will must contain the files:               #
-# ChangeLog.txt, PACKAGES.TXT and CHECKSUMS.md5                        #
-# A SlackBuilds repository will must contain the files:                #
-# SLACKBUILDS.TXT and ChangeLog.txt                                    #
-# Note: ponce repository needs the 'gen_sbo_txt.sh' tool from          #
-# the 'slpkg/tools/' folder, if the SLACKBUILDS.TXT missing.           #
-#                                                                      #
-# After the mirror changed, you should update the database:            #
-# slpkg update or apply the option --bin-repo=<repo_name> for          #
-# binaries repositories.                                               #
-########################################################################
-
-########################################################################
-# Note: Before using a repository, make sure you have read about it.   #
-#       Some repositories are for -current only. Change the mirror if  #
-#       it is necessary. The mirror should end with a slash '/'.       #
-########################################################################
+# This is the general repositories configuration file of slpkg:
+# /etc/slpkg/repositories.toml
+# Date: 24/04/2023, Version: 4.8.1
+
+# The philosophy behind this is to have two repositories for
+# Slackbuilds one for the Slackware stable and one for the -current
+# and many binaries for all versions.
+# Set 'true' to 'PONCE_REPO' to switch with the ponce repository.
+# Set 'true' to the binary repositories you want to enable.
+# Default is the 'sbo' Slackbuilds.org repository.
+
+# If you are going to use a local repository, set the mirror:
+# Example: ["file:///path/to/alien/repository/" ,"15.0/", "x86_64/"]
+# A binary local repository will must contain the files:
+# ChangeLog.txt, PACKAGES.TXT and CHECKSUMS.md5
+# A SlackBuilds repository will must contain the files:
+# SLACKBUILDS.TXT and ChangeLog.txt
+# Note: ponce repository needs the 'gen_sbo_txt.sh' tool from
+# the 'slpkg/tools/' folder, if the SLACKBUILDS.TXT missing.
+
+# After the mirror changed, you should update the database:
+# slpkg update or apply the option --bin-repo=<repo_name> for
+# binary repositories.
+
+# Note: Before using a repository, make sure you have read about it.
+#       Some repositories are for -current only. Change the mirror if
+#       it is necessary. The mirror should end with a slash '/'.
 
 [REPOSITORIES]
 
 # SBo Repository for Slackware 15.0 stable.
 SBO_REPO_NAME = "sbo"
 SBO_REPO_MIRROR = ["https://slackbuilds.org/slackbuilds/15.0/"]
 SBO_REPO_SLACKBUILDS = "SLACKBUILDS.TXT"
@@ -68,16 +65,14 @@
 SLACK_EXTRA_REPO_MIRROR = ["https://slackware.uk/slackware/slackware64-15.0/", "extra/"]
 SLACK_EXTRA_REPO_PACKAGES = "PACKAGES.TXT"
 SLACK_EXTRA_REPO_CHECKSUMS = "CHECKSUMS.md5"
 SLACK_EXTRA_REPO_CHANGELOG = "ChangeLog.txt"
 SLACK_EXTRA_REPO_TAG = ""
 
 # Official repository for Slackware patches x86_64 15.0 stable.
-# For Slackware patches x86_64 -current:
-# ["https://slackware.uk/slackware/slackware64-current/", "patches/"]
 SLACK_PATCHES_REPO = false
 SLACK_PATCHES_REPO_NAME = "slack_patches"
 SLACK_PATCHES_REPO_MIRROR = ["https://slackware.uk/slackware/slackware64-15.0/", "patches/"]
 SLACK_PATCHES_REPO_PACKAGES = "PACKAGES.TXT"
 SLACK_PATCHES_REPO_CHECKSUMS = "CHECKSUMS.md5"
 SLACK_PATCHES_REPO_CHANGELOG = "ChangeLog.txt"
 SLACK_PATCHES_REPO_TAG = ""
```

### Comparing `slpkg-4.8.0/configs/slpkg.toml` & `slpkg-4.8.1/configs/slpkg.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# This is the general configuration file of slpkg:
+# /etc/slpkg/slpkg.toml
+# Date: 24/04/2023, Version: 4.8.1
+
 [CONFIGS]
 
 # OS architecture by default.
 OS_ARCH = "x86_64"
 
 # Where the packages download.
 # This path working only with the command download.
@@ -57,15 +61,15 @@
 INSTALLPKG = "upgradepkg --install-new"
 
 # Slackware command to reinstall packages.
 # Upgradepkg usually skips packages if the exact same package (matching name,
 # version, arch, and build number) is already installed on the system. Use
 # the --reinstall option if you want to upgrade all packages even if the same
 # version is already installed. See: $ man upgradepkg.
-REINSTALL = "upgradepkg --install-new --reinstall"
+REINSTALL = "upgradepkg --reinstall"
 
 # Slackware command to remove packages.
 #removepkg removes a previously installed Slackware package, while writing
 # a progress report to the standard output.  A package may be specified either
 # by the full package name (as you'd see listed in /var/lib/pkgtools/packages/),
 # or by the base package name. See: $ man removepkg.
 REMOVEPKG = "removepkg"
```

### Comparing `slpkg-4.8.0/tests/test_configs.py` & `slpkg-4.8.1/tests/test_configs.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.0/tests/test_checks.py` & `slpkg-4.8.1/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.0/tests/test_utilities.py` & `slpkg-4.8.1/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.0/tests/test_sbo_queries.py` & `slpkg-4.8.1/tests/test_sbo_queries.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,27 +13,27 @@
         self.assertTrue(True, self.data[self.name])
 
     def test_location(self):
         self.assertEqual('system', self.data[self.name][0])
 
     def test_sources_x86(self):
         self.assertEqual(['https://gitlab.com/dslackw/slpkg/-/archive'
-                         '/4.7.8/slpkg-4.7.8.tar.gz'], self.data[self.name][3].split())
+                         '/4.8.0/slpkg-4.8.0.tar.gz'], self.data[self.name][3].split())
 
     def test_sources_x86_64(self):
         self.assertEqual([], self.data[self.name][4].split())
 
     def test_requires(self):
         self.assertEqual(['SQLAlchemy', 'python3-pythondialog', 'python3-progress'], self.data[self.name][7].split())
 
     def test_version(self):
-        self.assertEqual('4.7.8', self.data[self.name][2])
+        self.assertEqual('4.8.0', self.data[self.name][2])
 
     def test_checksum_x86(self):
-        self.assertListEqual(['d0ba1c826dc691ceec1ad12603e51330'], self.data[self.name][5].split())
+        self.assertListEqual(['75af7a43379407b8428dc6053fac470c'], self.data[self.name][5].split())
 
     def test_checksum_x86_64(self):
         self.assertListEqual([], self.data[self.name][6].split())
 
     def test_files(self):
         self.assertEqual(5, len(self.data[self.name][1].split()))
```

### Comparing `slpkg-4.8.0/tests/test_upgrade.py` & `slpkg-4.8.1/tests/test_upgrade.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.0/tests/test_bin_queries.py` & `slpkg-4.8.1/tests/test_bin_queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.0/LICENSE` & `slpkg-4.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.0/install.sh` & `slpkg-4.8.1/install.sh`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.0/ChangeLog.txt` & `slpkg-4.8.1/ChangeLog.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+4.8.1 - 21/04/2023
+Updated:
+- For error messages
+- For repository updates (Thanks to rizitis)
+- For reinstall slackware command
+Fixed:
+- Double packages as main and as dependency for binaries repos
+- View packages for ponce repository (Thanks to rizitis)
+
 4.8.0 - 19/04/2023
 Fixed:
 - Counting dependencies for tracking and blacklist packages
 - Resolving dependencies when are blacklisted or not included in the repository
 
 4.7.9 - 15/04/2023
 Updated:
```

### Comparing `slpkg-4.8.0/man/slpkg.1` & `slpkg-4.8.1/man/slpkg.1`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.0/man/slpkg-fr.1` & `slpkg-4.8.1/man/slpkg-fr.1`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.0/completion/slpkg` & `slpkg-4.8.1/completion/slpkg`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.0/slpkg/dialog_configs.py` & `slpkg-4.8.1/slpkg/dialog_configs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 import os
 from pathlib import Path
 
-from slpkg.configs import Load
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.dialog_box import DialogBox
+from slpkg.error_messages import Errors
 
 
 class FormConfigs(Configs):
 
     def __init__(self):
         super(Configs).__init__()
-        self.load_configs = Load()
         self.dialogbox = DialogBox()
+        self.errors = Errors()
         self.utils = Utilities()
 
         self.orig_configs: list = []
-        self.config_file = Path(self.etc_path, f'{self.prog_name}.toml')
+        self.config_file: Path = Path(self.etc_path, f'{self.prog_name}.toml')
 
     def is_dialog_enabled(self) -> None:
         """ Checking if the dialog box is enabled by the user. """
         if not self.dialog:
-            self.utils.raise_error_message(f"You should enable the dialog "
-                                           f"in the '{self.etc_path}/{self.prog_name}.toml' file")
+            self.errors.raise_error_message(f"You should enable the dialog in the "
+                                            f"'{self.etc_path}/{self.prog_name}.toml' file")
 
     def edit(self) -> None:
         """ Read and write the configuration file. """
         self.is_dialog_enabled()
         elements: list = []
         height: int = 30
         width: int = 74
@@ -90,15 +90,15 @@
                 return False
 
         return True
 
     def read_configs(self) -> None:
         """ Read the original config file. """
         with open(self.config_file, 'r') as toml_file:
-            self.orig_configs = toml_file.readlines()
+            self.orig_configs: list = toml_file.readlines()
 
     def write_file(self, tags: list) -> None:
         """ Write the new values to the config file. """
         self.read_configs()
 
         with open(self.config_file, 'w') as patch_toml:
 
@@ -112,10 +112,10 @@
 
                             ('COLORS =', 'DIALOG =',
                              'SILENT_MODE =',
                              'ASCII_CHARACTERS =',
                              'ASK_QUESTION =',
                              'PARALLEL_DOWNLOADS =')
                     ):
-                        line = line.replace('"', '')
+                        line: str = line.replace('"', '')
 
                 patch_toml.write(line)
```

### Comparing `slpkg-4.8.0/slpkg/binaries/required.py` & `slpkg-4.8.1/slpkg/binaries/required.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+from typing import Generator
+
 from slpkg.repositories import Repositories
 
 
 class Required:
     """ Creates a list of dependencies with
     the right order to install. """
 
@@ -39,12 +41,12 @@
                 sub_required: list[str] = list(self.remove_deps(self.data[req][6].split()))
                 for sub in sub_required:
                     required.append(sub)
 
         required.reverse()
         return list(dict.fromkeys(required))
 
-    def remove_deps(self, requires):
+    def remove_deps(self, requires: list) -> Generator:
         """ Remove requires that not in the repository or blacklisted. """
         for dep in requires:
             if dep in list(self.data.keys()):
                 yield dep
```

### Comparing `slpkg-4.8.0/slpkg/binaries/queries.py` & `slpkg-4.8.1/slpkg/binaries/queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.0/slpkg/binaries/install.py` & `slpkg-4.8.1/slpkg/binaries/install.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,33 +28,24 @@
         super(Configs, self).__init__()
         self.data: dict = data
         self.packages: list = packages
         self.flags: list = flags
         self.mode: str = mode
 
         self.progress = ProgressBar()
-        self.color = self.colour()
         self.utils = Utilities()
         self.repos = Repositories()
         self.dialogbox = DialogBox()
         self.upgrade = Upgrade(self.flags, self.data)
         self.view_message = ViewMessage(self.flags, self.data)
         self.session = Session
 
-        self.output: int = 0
         self.stderr = None
         self.stdout = None
         self.process_message: str = ''
-        self.bold: str = self.color['bold']
-        self.cyan: str = self.color['cyan']
-        self.red: str = self.color['red']
-        self.yellow: str = self.color['yellow']
-        self.endc: str = self.color['endc']
-        self.byellow: str = f'{self.bold}{self.yellow}'
-        self.bred: str = f'{self.bold}{self.red}'
 
         self.packages_requires: list = []
         self.install_order: list = []
         self.binary_packages: list = []
 
         self.option_for_reinstall: bool = self.utils.is_option(
             ['-r', '--reinstall'], self.flags)
@@ -98,14 +89,19 @@
 
             # Clean dependencies from the dependencies list if already added with main packages.
             requires = list(OrderedDict.fromkeys(self.packages_requires))
 
             if requires:
                 self.packages_requires = self.choose_dependencies(requires)
 
+        # Clean up the main packages if they were selected for dependencies.
+        for dep in self.packages_requires:
+            if dep in self.packages:
+                self.packages.remove(dep)
+
         self.install_order = [*self.packages_requires, *self.packages]
 
     def download(self) -> None:
         """ Download packages from the repositories. """
         pkg_urls: list = []
 
         for pkg in self.install_order:
@@ -198,28 +194,27 @@
 
             done: str = f' {self.byellow} Done{self.endc}'
             self.stderr = subprocess.DEVNULL
             self.stdout = subprocess.DEVNULL
 
             # Starting multiprocessing
             p1 = Process(target=self.utils.process, args=(command, self.stderr, self.stdout))
-            p2 = Process(target=self.progress.bar, args=(f'[{message}]', filename))
+            p2 = Process(target=self.progress.bar, args=(f'{message}:', filename))
 
             p1.start()
             p2.start()
 
             # Wait until process 1 finish
             p1.join()
 
             # Terminate process 2 if process 1 finished
             if not p1.is_alive():
 
                 if p1.exitcode != 0:
                     done: str = f'{self.bred}Failed: {self.endc}{self.process_message}.'
-                    self.output: int = p1.exitcode  # type: ignore
 
                 print(f'{self.endc}{done}', end='')
                 p2.terminate()
 
             # Wait until process 2 finish
             p2.join()
```

### Comparing `slpkg-4.8.0/slpkg/install_data.py` & `slpkg-4.8.1/slpkg/install_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,21 +14,14 @@
 class InstallData(Configs):
 
     def __init__(self):
         super(Configs, self).__init__()
         self.session = Session
         self.utils = Utilities()
         self.repos = Repositories()
-        self.color = self.colour()
-
-        self.bold: str = self.color['bold']
-        self.yellow: str = self.color['yellow']
-        self.cyan: str = self.color['cyan']
-        self.byellow: str = f'{self.bold}{self.yellow}'
-        self.endc: str = self.color['endc']
 
     def last_updated(self, repo_file: Path) -> str:
         """ Reads the first date of the changelog file."""
         lines: list = self.utils.read_file(repo_file)
         days = ('Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun')
         for line in lines:
             if line.startswith(days):
```

### Comparing `slpkg-4.8.0/slpkg/repositories.py` & `slpkg-4.8.1/slpkg/repositories.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,33 +3,27 @@
 
 
 import tomli
 from pathlib import Path
 from dataclasses import dataclass
 
 from slpkg.configs import Configs
+from slpkg.toml_error_message import TomlErrors
 
 
 @dataclass
 class Repositories:
     configs = Configs
-    color = configs.colour()
-    bold: str = color['bold']
-    red: str = color['red']
-    cyan: str = color['cyan']
-    endc: str = color['endc']
-    bred: str = f'{bold}{red}'
+    errors = TomlErrors()
 
     repositories_toml_file: Path = Path(configs.etc_path, 'repositories.toml')
     repositories_path: Path = Path(configs.lib_path, 'repositories')
 
     repos_config = {}
     repositories = {}
-    bin_repos_name = []
-    bin_enabled_repos = []
 
     sbo_repo: bool = True
     sbo_repo_name: str = 'sbo'
     sbo_repo_path: Path = Path(repositories_path, sbo_repo_name)
     sbo_repo_mirror = ['https://slackbuilds.org/slackbuilds/15.0/']
     sbo_repo_slackbuilds: str = 'SLACKBUILDS.TXT'
     sbo_repo_changelog: str = 'ChangeLog.txt'
@@ -372,19 +366,15 @@
             slint_repo_checksums: str = repos_config['SLINT_REPO_CHECKSUMS']
             slint_repo_changelog: str = repos_config['SLINT_REPO_CHANGELOG']
             slint_repo_tag: str = repos_config['SLINT_REPO_TAG']
             if slint_repo_mirror[0].startswith('file'):
                 slint_repo_path: str = slint_repo_mirror[0][7:]
 
     except (tomli.TOMLDecodeError, KeyError) as error:
-        raise SystemExit(f'\n{configs.prog_name} {bred}Error{endc}: {error}: in the configuration file '
-                         f"'{repositories_toml_file}'.\n"
-                         f"\nIf you have upgraded the '{configs.prog_name}' probably you need to run:\n"
-                         f"'mv {repositories_toml_file}.new {repositories_toml_file}'.\n"
-                         f"or '{cyan}slpkg_new-configs{endc}' command.\n")
+        errors.raise_toml_error_message(error, repositories_toml_file)
 
     # Default sbo repository configs.
     repo_tag: str = sbo_repo_tag
     patch_repo_tag: str = sbo_repo_patch_tag
     sbo_enabled_repo_name: str = sbo_repo_name
     if ponce_repo:
         sbo_enabled_repo_name: str = ponce_repo_name
@@ -535,13 +525,7 @@
                           slint_repo_path,
                           slint_repo_mirror,
                           slint_repo_packages,
                           slint_repo_checksums,
                           slint_repo_changelog,
                           slint_repo_tag]
     }
-
-    # All the binary repositories names.
-    bin_repos_names = list(repositories.keys())[2:]
-
-    # All the enabled binary repositories names.
-    bin_enabled_repos = list(repositories.keys())[2:]
```

### Comparing `slpkg-4.8.0/slpkg/repo_info.py` & `slpkg-4.8.1/slpkg/repo_info.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,41 +11,30 @@
 
 
 class RepoInfo(Configs):
 
     def __init__(self):
         super(Configs, self).__init__()
 
+        self.session = Session
         self.utils = Utilities()
         self.repos = Repositories()
-        self.color = self.colour()
         self.columns, self.rows = shutil.get_terminal_size()
-        self.session = Session
-
-        self.bold: str = self.color['bold']
-        self.green: str = self.color['green']
-        self.red: str = self.color['red']
-        self.cyan: str = self.color['cyan']
-        self.grey: str = self.color['grey']
-        self.yellow: str = self.color['yellow']
-        self.byellow: str = f'{self.bold}{self.yellow}'
-        self.endc: str = self.color['endc']
 
     def info(self):
         """ Prints information about repositories. """
         total_packages: int = 0
         enabled: int = 0
 
         print('Repositories Information:')
         print('=' * self.columns)
         print(f"{'Name:':<18}{'Status:':<15}{'Last Updated:':<35}{'Packages:':>12}")
         print('=' * self.columns)
 
         for repo, value in self.repos.repositories.items():
-            count: int = 0
             status: str = 'Disabled'
             color: str = self.red
 
             last: str = self.session.query(
                 LastRepoUpdated.date).where(
                 LastRepoUpdated.repo == repo).first()
 
@@ -53,18 +42,18 @@
                 last: tuple = ('',)
 
             if value[0]:
                 enabled += 1
                 status: str = 'Enabled'
                 color: str = self.green
 
-                if repo in [self.repos.sbo_repo_name, self.repos.ponce_repo_name]:
-                    count = self.session.query(SBoTable.id).count()
-                else:
-                    count = self.session.query(BinariesTable).where(BinariesTable.repo == repo).count()
+            if repo in [self.repos.sbo_repo_name, self.repos.ponce_repo_name]:
+                count = self.session.query(SBoTable.id).count()
+            else:
+                count = self.session.query(BinariesTable).where(BinariesTable.repo == repo).count()
 
             total_packages += count
 
             print(f"{self.cyan}{repo:<18}{self.endc}{color}{status:<15}{self.endc}{last[0]:<35}"
                   f"{self.yellow}{count:>12}{self.endc}")
 
         print('=' * self.columns)
```

### Comparing `slpkg-4.8.0/slpkg/sbos/queries.py` & `slpkg-4.8.1/slpkg/sbos/queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.0/slpkg/sbos/slackbuild.py` & `slpkg-4.8.1/slpkg/sbos/slackbuild.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 from slpkg.checksum import Md5sum
 from slpkg.configs import Configs
 from slpkg.upgrade import Upgrade
 from slpkg.utilities import Utilities
 from slpkg.dialog_box import DialogBox
 from slpkg.downloader import Downloader
+from slpkg.error_messages import Errors
 from slpkg.views.views import ViewMessage
 from slpkg.progress_bar import ProgressBar
 from slpkg.repositories import Repositories
 from slpkg.sbos.dependencies import Requires
 from slpkg.models.models import LogsDependencies
 from slpkg.models.models import session as Session
 
@@ -32,35 +33,28 @@
         super(Configs, self).__init__()
         self.data = data
         self.slackbuilds: list = slackbuilds
         self.flags: list = flags
         self.mode: str = mode
 
         self.session = Session
+        self.errors = Errors()
         self.repos = Repositories()
         self.utils = Utilities()
         self.progress = ProgressBar()
         self.dialogbox = DialogBox()
         self.upgrade = Upgrade(self.flags, data)
         self.view_message = ViewMessage(self.flags, data)
-        self.color = self.colour()
 
         self.stderr = None
         self.stdout = None
         self.sbos: dict = {}
         self.install_order: list = []
         self.dependencies: list = []
         self.process_message: str = ''
-        self.bold: str = self.color['bold']
-        self.cyan: str = self.color['cyan']
-        self.red: str = self.color['red']
-        self.yellow: str = self.color['yellow']
-        self.endc: str = self.color['endc']
-        self.byellow: str = f'{self.bold}{self.yellow}'
-        self.bred: str = f'{self.bold}{self.red}'
 
         self.option_for_reinstall: bool = self.utils.is_option(
             ['-r', '--reinstall'], self.flags)
 
         self.option_for_skip_installed: bool = self.utils.is_option(
             ['-k', '--skip-installed'], self.flags)
 
@@ -112,15 +106,15 @@
 
                 self.dependencies.append(dep)
 
         # Remove duplicate packages and keeps the order.
         dependencies = list(OrderedDict.fromkeys(self.dependencies))
 
         if dependencies:
-            self.dependencies = self.choose_dependencies(dependencies)
+            self.dependencies: list = self.choose_dependencies(dependencies)
 
             # Clean up the main packages if they were selected for dependencies.
             for dep in self.dependencies:
                 if dep in self.slackbuilds:
                     self.slackbuilds.remove(dep)
 
         self.install_order.extend(self.dependencies)
@@ -237,30 +231,30 @@
             else:
                 package: str = self.utils.is_package_installed(sbo)
                 version: str = self.utils.split_binary_pkg(package)[1]
                 self.view_message.view_skipping_packages(sbo, version)
 
     def patch_sbo_tag(self, sbo: str) -> None:
         """ Patching SBo TAG from the configuration file. """
-        sbo_script = Path(self.build_path, sbo, f'{sbo}.SlackBuild')
+        sbo_script: Path = Path(self.build_path, sbo, f'{sbo}.SlackBuild')
 
         if sbo_script.is_file() and self.repos.patch_repo_tag:
 
             with open(sbo_script, 'r', encoding='utf-8') as f:
                 lines = f.readlines()
 
             with open(sbo_script, 'w') as script:
                 for line in lines:
                     if line.startswith('TAG=$'):
                         line: str = f'TAG=${{TAG:-{self.repos.patch_repo_tag}}}\n'
                     script.write(line)
 
     def logging_installed_dependencies(self, name: str) -> None:
         """ Logging installed dependencies and used for remove. """
-        exist = self.session.query(LogsDependencies.name).filter(
+        exist: tuple = self.session.query(LogsDependencies.name).filter(
             LogsDependencies.name == name).first()
 
         requires: list = Requires(self.data, name).resolve()
 
         # Update the dependencies if exist else create it.
         if exist:
             self.session.query(
@@ -294,21 +288,21 @@
 
     def package_for_install(self, name: str) -> str:
         """ Returns the package for install. """
         package: str = ''
         version: str = self.data[name][2]
         pattern: str = f'{name}-{version}*{self.repos.repo_tag}*'
 
-        tmp = Path(self.tmp_path)
+        tmp: Path = Path(self.tmp_path)
         packages: list = [file.name for file in tmp.glob(pattern)]
 
         try:
             package: str = max(packages)
         except ValueError:
-            self.utils.raise_error_message(f"Package '{name}' not found for install")
+            self.errors.raise_error_message(f"Package '{name}' not found for install")
 
         return package
 
     def build_the_script(self, path: Path, name: str) -> None:
         """ Run the .SlackBuild script. """
         folder: str = f'{Path(path, name)}/'
         execute: str = f'{folder}./{name}.SlackBuild'
@@ -317,15 +311,15 @@
         os.chown(folder, 0, 0)
         for file in os.listdir(folder):
             os.chown(f'{folder}{file}', 0, 0)
 
         if self.option_for_jobs:
             self.set_makeflags()
 
-        name = f'{name}.SlackBuild'
+        name: str = f'{name}.SlackBuild'
         message: str = f'{self.red}Build{self.endc}'
         self.process_message: str = f"package '{name}' to build"
 
         self.multi_process(execute, name, message)
 
     @staticmethod
     def set_makeflags() -> None:
@@ -338,15 +332,15 @@
 
             done: str = f' {self.byellow} Done{self.endc}'
             self.stderr = subprocess.DEVNULL
             self.stdout = subprocess.DEVNULL
 
             # Starting multiprocessing
             p1 = Process(target=self.utils.process, args=(command, self.stderr, self.stdout))
-            p2 = Process(target=self.progress.bar, args=(f'[{message}]', filename))
+            p2 = Process(target=self.progress.bar, args=(f'{self.bold}{message}:', filename))
 
             p1.start()
             p2.start()
 
             # Wait until process 1 finish
             p1.join()
```

### Comparing `slpkg-4.8.0/slpkg/sbos/dependencies.py` & `slpkg-4.8.1/slpkg/sbos/dependencies.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+from typing import Generator
+
+
 class Requires:
     """ Creates a list of dependencies with
     the right order to install. """
 
     def __init__(self, data: dict, name: str):
         __slots__ = 'data', 'name'
         self.data: dict = data
@@ -19,12 +22,12 @@
             for sub in sub_requires:
                 requires.append(sub)
 
         requires.reverse()
 
         return list(dict.fromkeys(requires))
 
-    def remove_deps(self, requires):
+    def remove_deps(self, requires: list) -> Generator:
         """ Remove requires that not in the repository or blacklisted. """
         for dep in requires:
             if dep in list(self.data.keys()):
                 yield dep
```

### Comparing `slpkg-4.8.0/slpkg/update_repository.py` & `slpkg-4.8.1/slpkg/update_repository.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,44 +24,36 @@
     """ Deletes and install the data. """
 
     def __init__(self, flags: list, repo: str):
         __slots__ = 'flags', 'repo'
         super(Configs, self).__init__()
         self.flags: list = flags
         self.repo: str = repo
+
         self.session = Session
         self.view = ViewMessage(self.flags)
-
         self.repos = Repositories()
         self.progress = ProgressBar()
         self.utils = Utilities()
-        self.color = self.colour()
         self.data = InstallData()
+
         self.check_updates = CheckUpdates(
             self.flags, self.repo
         )
 
-        if not self.repo:
-            self.repo = self.repos.sbo_enabled_repo_name
-
         self.repos_for_update: dict = {}
-        self.bold: str = self.color['bold']
-        self.green: str = self.color['green']
-        self.red: str = self.color['red']
-        self.yellow: str = self.color['yellow']
-        self.bgreen: str = f'{self.bold}{self.green}'
-        self.bred: str = f'{self.bold}{self.red}'
-        self.endc: str = self.color['endc']
-        self.flag_generate: list = ['-G', '--generate-only']
+
+        self.option_for_generate: bool = self.utils.is_option(
+            ['-G', '--generate-only'], self.flags)
 
         self.option_for_binaries: bool = self.utils.is_option(
             ['-B', '--bin-repo='], self.flags)
 
     def update_the_repositories(self) -> None:
-        if not self.repos_for_update.values() or self.repo not in self.repos_for_update.keys():
+        if not any(list(self.repos_for_update.values())) or self.repo == '*':
             self.view.question()
         else:
             print()
 
         bin_repositories: dict = {
             self.repos.slack_repo_name: self.slack_repository,
             self.repos.slack_extra_repo_name: self.slack_extra_repository,
@@ -80,498 +72,434 @@
             self.repos.slackel_repo_name: self.slackel_repository,
             self.repos.slint_repo_name: self.slint_repository
         }
 
         if self.option_for_binaries:
 
             for repo in bin_repositories.keys():
+                if self.repos.repositories[repo][0]:
 
-                if repo == self.repo:
-                    bin_repositories[repo]()
-                    break
+                    if repo == self.repo:
+                        bin_repositories[repo]()
+                        break
 
-                if self.repo == '*':
-                    bin_repositories[repo]()
+                    if self.repo == '*':
+                        bin_repositories[repo]()
         else:
             self.slackbuild_repositories()
         print()
 
     def slack_repository(self):
-        if self.repos.slack_repo:
-
-            if not self.repos.slack_repo_mirror[0].startswith('file'):
-                print(f"Downloading the '{self.green}{self.repos.slack_repo_name}{self.endc}"
-                      f"' repository, please wait...\n")
-                urls: list = []
-                self.make_dirs(self.repos.slack_repo_name)
-
-                urls.append(f'{self.repos.slack_repo_mirror[0]}{self.repos.slack_repo_packages}')
-                urls.append(f'{self.repos.slack_repo_mirror[0]}{self.repos.slack_repo_changelog}')
-                urls.append(f'{self.repos.slack_repo_mirror[0]}{self.repos.slack_repo_checksums}')
-
-                self.utils.remove_file_if_exists(self.repos.slack_repo_path, self.repos.slack_repo_packages)
-                self.utils.remove_file_if_exists(self.repos.slack_repo_path, self.repos.slack_repo_changelog)
-                self.utils.remove_file_if_exists(self.repos.slack_repo_path, self.repos.slack_repo_checksums)
-
-                down = Downloader(self.repos.slack_repo_path, urls, self.flags)
-                down.download()
-                print()
-
-            self.delete_bin_database_data(self.repos.slack_repo_name)
-            self.delete_last_updated(self.repos.slack_repo_name)
-            self.data.install_slack_data()
-            print()
-        else:
-            self.not_enabled_message(self.repos.slack_repo_name)
+        if not self.repos.slack_repo_mirror[0].startswith('file'):
+            print(f"Downloading the '{self.green}{self.repos.slack_repo_name}{self.endc}"
+                  f"' repository, please wait...\n")
+            urls: list = []
+            self.make_dirs(self.repos.slack_repo_name)
+
+            urls.append(f'{self.repos.slack_repo_mirror[0]}{self.repos.slack_repo_packages}')
+            urls.append(f'{self.repos.slack_repo_mirror[0]}{self.repos.slack_repo_changelog}')
+            urls.append(f'{self.repos.slack_repo_mirror[0]}{self.repos.slack_repo_checksums}')
+
+            self.utils.remove_file_if_exists(self.repos.slack_repo_path, self.repos.slack_repo_packages)
+            self.utils.remove_file_if_exists(self.repos.slack_repo_path, self.repos.slack_repo_changelog)
+            self.utils.remove_file_if_exists(self.repos.slack_repo_path, self.repos.slack_repo_checksums)
+
+            down = Downloader(self.repos.slack_repo_path, urls, self.flags)
+            down.download()
+            print()
+
+        self.delete_bin_database_data(self.repos.slack_repo_name)
+        self.delete_last_updated(self.repos.slack_repo_name)
+        self.data.install_slack_data()
+        print()
 
     def slack_extra_repository(self):
-        if self.repos.slack_extra_repo:
-
-            if not self.repos.slack_extra_repo_mirror[0].startswith('file'):
-                print(f"Downloading the '{self.green}{self.repos.slack_extra_repo_name}{self.endc}"
-                      f"' repository, please wait...\n")
-                urls: list = []
-                self.make_dirs(self.repos.slack_extra_repo_name)
-
-                urls.append(f'{"".join(self.repos.slack_extra_repo_mirror)}{self.repos.slack_extra_repo_packages}')
-                urls.append(f'{self.repos.slack_extra_repo_mirror[0]}{self.repos.slack_extra_repo_changelog}')
-                urls.append(f'{self.repos.slack_extra_repo_mirror[0]}{self.repos.slack_extra_repo_checksums}')
-
-                self.utils.remove_file_if_exists(self.repos.slack_extra_repo_path,
-                                                 self.repos.slack_extra_repo_packages)
-                self.utils.remove_file_if_exists(self.repos.slack_extra_repo_path,
-                                                 self.repos.slack_extra_repo_changelog)
-                self.utils.remove_file_if_exists(self.repos.slack_extra_repo_path,
-                                                 self.repos.slack_extra_repo_checksums)
-
-                down = Downloader(self.repos.slack_extra_repo_path, urls, self.flags)
-                down.download()
-                print()
-
-            self.delete_bin_database_data(self.repos.slack_extra_repo_name)
-            self.delete_last_updated(self.repos.slack_extra_repo_name)
-            self.data.install_slack_extra_data()
-            print()
-        else:
-            self.not_enabled_message(self.repos.slack_extra_repo_name)
+        if not self.repos.slack_extra_repo_mirror[0].startswith('file'):
+            print(f"Downloading the '{self.green}{self.repos.slack_extra_repo_name}{self.endc}"
+                  f"' repository, please wait...\n")
+            urls: list = []
+            self.make_dirs(self.repos.slack_extra_repo_name)
+
+            urls.append(f'{"".join(self.repos.slack_extra_repo_mirror)}{self.repos.slack_extra_repo_packages}')
+            urls.append(f'{self.repos.slack_extra_repo_mirror[0]}{self.repos.slack_extra_repo_changelog}')
+            urls.append(f'{self.repos.slack_extra_repo_mirror[0]}{self.repos.slack_extra_repo_checksums}')
+
+            self.utils.remove_file_if_exists(self.repos.slack_extra_repo_path,
+                                             self.repos.slack_extra_repo_packages)
+            self.utils.remove_file_if_exists(self.repos.slack_extra_repo_path,
+                                             self.repos.slack_extra_repo_changelog)
+            self.utils.remove_file_if_exists(self.repos.slack_extra_repo_path,
+                                             self.repos.slack_extra_repo_checksums)
+
+            down = Downloader(self.repos.slack_extra_repo_path, urls, self.flags)
+            down.download()
+            print()
+
+        self.delete_bin_database_data(self.repos.slack_extra_repo_name)
+        self.delete_last_updated(self.repos.slack_extra_repo_name)
+        self.data.install_slack_extra_data()
+        print()
 
     def slack_patches_repository(self):
-        if self.repos.slack_patches_repo:
-
-            if not self.repos.slack_patches_repo_mirror[0].startswith('file'):
-                print(f"Downloading the '{self.green}{self.repos.slack_patches_repo_name}{self.endc}"
-                      f"' repository, please wait...\n")
-                urls: list = []
-                self.make_dirs(self.repos.slack_patches_repo_name)
-
-                urls.append(f'{"".join(self.repos.slack_patches_repo_mirror)}{self.repos.slack_patches_repo_packages}')
-                urls.append(f'{self.repos.slack_patches_repo_mirror[0]}{self.repos.slack_patches_repo_changelog}')
-                urls.append(f'{self.repos.slack_patches_repo_mirror[0]}{self.repos.slack_patches_repo_checksums}')
-
-                self.utils.remove_file_if_exists(self.repos.slack_patches_repo_path,
-                                                 self.repos.slack_patches_repo_packages)
-                self.utils.remove_file_if_exists(self.repos.slack_patches_repo_path,
-                                                 self.repos.slack_patches_repo_changelog)
-                self.utils.remove_file_if_exists(self.repos.slack_patches_repo_path,
-                                                 self.repos.slack_patches_repo_checksums)
-
-                down = Downloader(self.repos.slack_patches_repo_path, urls, self.flags)
-                down.download()
-                print()
-
-            self.delete_bin_database_data(self.repos.slack_patches_repo_name)
-            self.delete_last_updated(self.repos.slack_patches_repo_name)
-            self.data.install_slack_patches_data()
-            print()
-        else:
-            self.not_enabled_message(self.repos.slack_patches_repo_name)
+        if not self.repos.slack_patches_repo_mirror[0].startswith('file'):
+            print(f"Downloading the '{self.green}{self.repos.slack_patches_repo_name}{self.endc}"
+                  f"' repository, please wait...\n")
+            urls: list = []
+            self.make_dirs(self.repos.slack_patches_repo_name)
+
+            urls.append(f'{"".join(self.repos.slack_patches_repo_mirror)}{self.repos.slack_patches_repo_packages}')
+            urls.append(f'{self.repos.slack_patches_repo_mirror[0]}{self.repos.slack_patches_repo_changelog}')
+            urls.append(f'{self.repos.slack_patches_repo_mirror[0]}{self.repos.slack_patches_repo_checksums}')
+
+            self.utils.remove_file_if_exists(self.repos.slack_patches_repo_path,
+                                             self.repos.slack_patches_repo_packages)
+            self.utils.remove_file_if_exists(self.repos.slack_patches_repo_path,
+                                             self.repos.slack_patches_repo_changelog)
+            self.utils.remove_file_if_exists(self.repos.slack_patches_repo_path,
+                                             self.repos.slack_patches_repo_checksums)
+
+            down = Downloader(self.repos.slack_patches_repo_path, urls, self.flags)
+            down.download()
+            print()
+
+        self.delete_bin_database_data(self.repos.slack_patches_repo_name)
+        self.delete_last_updated(self.repos.slack_patches_repo_name)
+        self.data.install_slack_patches_data()
+        print()
 
     def alien_repository(self):
-        if self.repos.alien_repo:
-
-            if not self.repos.alien_repo_mirror[0].startswith('file'):
-                print(f"Downloading the '{self.green}{self.repos.alien_repo_name}{self.endc}' "
-                      f"repository, please wait...\n")
-                urls: list = []
-                self.make_dirs(self.repos.alien_repo_name)
-
-                urls.append(f'{"".join(self.repos.alien_repo_mirror)}{self.repos.alien_repo_packages}')
-                urls.append(f'{self.repos.alien_repo_mirror[0]}{self.repos.alien_repo_changelog}')
-                urls.append(f'{"".join(self.repos.alien_repo_mirror)}{self.repos.alien_repo_checksums}')
-
-                self.utils.remove_file_if_exists(self.repos.alien_repo_path, self.repos.alien_repo_packages)
-                self.utils.remove_file_if_exists(self.repos.alien_repo_path, self.repos.alien_repo_changelog)
-                self.utils.remove_file_if_exists(self.repos.alien_repo_path, self.repos.alien_repo_checksums)
-
-                down = Downloader(self.repos.alien_repo_path, urls, self.flags)
-                down.download()
-                print()
-
-            self.delete_bin_database_data(self.repos.alien_repo_name)
-            self.delete_last_updated(self.repos.alien_repo_name)
-            self.data.install_alien_data()
-            print()
-        else:
-            self.not_enabled_message(self.repos.alien_repo_name)
+        if not self.repos.alien_repo_mirror[0].startswith('file'):
+            print(f"Downloading the '{self.green}{self.repos.alien_repo_name}{self.endc}' "
+                  f"repository, please wait...\n")
+            urls: list = []
+            self.make_dirs(self.repos.alien_repo_name)
+
+            urls.append(f'{"".join(self.repos.alien_repo_mirror)}{self.repos.alien_repo_packages}')
+            urls.append(f'{self.repos.alien_repo_mirror[0]}{self.repos.alien_repo_changelog}')
+            urls.append(f'{"".join(self.repos.alien_repo_mirror)}{self.repos.alien_repo_checksums}')
+
+            self.utils.remove_file_if_exists(self.repos.alien_repo_path, self.repos.alien_repo_packages)
+            self.utils.remove_file_if_exists(self.repos.alien_repo_path, self.repos.alien_repo_changelog)
+            self.utils.remove_file_if_exists(self.repos.alien_repo_path, self.repos.alien_repo_checksums)
+
+            down = Downloader(self.repos.alien_repo_path, urls, self.flags)
+            down.download()
+            print()
+
+        self.delete_bin_database_data(self.repos.alien_repo_name)
+        self.delete_last_updated(self.repos.alien_repo_name)
+        self.data.install_alien_data()
+        print()
 
     def multilib_repository(self) -> None:
-        if self.repos.multilib_repo:
-
-            if not self.repos.multilib_repo_mirror[0].startswith('file'):
-                print(f"Downloading the '{self.green}{self.repos.multilib_repo_name}{self.endc}' "
-                      f"repository, please wait...\n")
-                urls: list = []
-                self.make_dirs(self.repos.multilib_repo_name)
-
-                urls.append(f'{"".join(self.repos.multilib_repo_mirror)}{self.repos.multilib_repo_packages}')
-                urls.append(f'{self.repos.multilib_repo_mirror[0]}{self.repos.multilib_repo_changelog}')
-                urls.append(f'{self.repos.multilib_repo_mirror[0]}{self.repos.multilib_repo_checksums}')
-
-                self.utils.remove_file_if_exists(self.repos.multilib_repo_path, self.repos.multilib_repo_packages)
-                self.utils.remove_file_if_exists(self.repos.multilib_repo_path, self.repos.multilib_repo_changelog)
-                self.utils.remove_file_if_exists(self.repos.multilib_repo_path, self.repos.multilib_repo_checksums)
-
-                down = Downloader(self.repos.multilib_repo_path, urls, self.flags)
-                down.download()
-                print()
-
-            self.delete_bin_database_data(self.repos.multilib_repo_name)
-            self.delete_last_updated(self.repos.multilib_repo_name)
-            self.data.install_multilib_data()
-            print()
-        else:
-            self.not_enabled_message(self.repos.multilib_repo_name)
+        if not self.repos.multilib_repo_mirror[0].startswith('file'):
+            print(f"Downloading the '{self.green}{self.repos.multilib_repo_name}{self.endc}' "
+                  f"repository, please wait...\n")
+            urls: list = []
+            self.make_dirs(self.repos.multilib_repo_name)
+
+            urls.append(f'{"".join(self.repos.multilib_repo_mirror)}{self.repos.multilib_repo_packages}')
+            urls.append(f'{self.repos.multilib_repo_mirror[0]}{self.repos.multilib_repo_changelog}')
+            urls.append(f'{self.repos.multilib_repo_mirror[0]}{self.repos.multilib_repo_checksums}')
+
+            self.utils.remove_file_if_exists(self.repos.multilib_repo_path, self.repos.multilib_repo_packages)
+            self.utils.remove_file_if_exists(self.repos.multilib_repo_path, self.repos.multilib_repo_changelog)
+            self.utils.remove_file_if_exists(self.repos.multilib_repo_path, self.repos.multilib_repo_checksums)
+
+            down = Downloader(self.repos.multilib_repo_path, urls, self.flags)
+            down.download()
+            print()
+
+        self.delete_bin_database_data(self.repos.multilib_repo_name)
+        self.delete_last_updated(self.repos.multilib_repo_name)
+        self.data.install_multilib_data()
+        print()
 
     def restricted_repository(self) -> None:
-        if self.repos.restricted_repo:
-
-            if not self.repos.restricted_repo_mirror[0].startswith('file'):
-                print(f"Downloading the '{self.green}{self.repos.restricted_repo_name}{self.endc}' "
-                      f"repository, please wait...\n")
-                urls: list = []
-                self.make_dirs(self.repos.restricted_repo_name)
-
-                urls.append(f'{"".join(self.repos.restricted_repo_mirror)}{self.repos.restricted_repo_packages}')
-                urls.append(f'{self.repos.restricted_repo_mirror[0]}{self.repos.restricted_repo_changelog}')
-                urls.append(f'{"".join(self.repos.restricted_repo_mirror)}{self.repos.restricted_repo_checksums}')
-
-                self.utils.remove_file_if_exists(self.repos.restricted_repo_path, self.repos.restricted_repo_packages)
-                self.utils.remove_file_if_exists(self.repos.restricted_repo_path, self.repos.restricted_repo_changelog)
-                self.utils.remove_file_if_exists(self.repos.restricted_repo_path, self.repos.restricted_repo_checksums)
-
-                down = Downloader(self.repos.restricted_repo_path, urls, self.flags)
-                down.download()
-                print()
-
-            self.delete_bin_database_data(self.repos.restricted_repo_name)
-            self.delete_last_updated(self.repos.restricted_repo_name)
-            self.data.install_restricted_data()
-            print()
-        else:
-            self.not_enabled_message(self.repos.restricted_repo_name)
+        if not self.repos.restricted_repo_mirror[0].startswith('file'):
+            print(f"Downloading the '{self.green}{self.repos.restricted_repo_name}{self.endc}' "
+                  f"repository, please wait...\n")
+            urls: list = []
+            self.make_dirs(self.repos.restricted_repo_name)
+
+            urls.append(f'{"".join(self.repos.restricted_repo_mirror)}{self.repos.restricted_repo_packages}')
+            urls.append(f'{self.repos.restricted_repo_mirror[0]}{self.repos.restricted_repo_changelog}')
+            urls.append(f'{"".join(self.repos.restricted_repo_mirror)}{self.repos.restricted_repo_checksums}')
+
+            self.utils.remove_file_if_exists(self.repos.restricted_repo_path, self.repos.restricted_repo_packages)
+            self.utils.remove_file_if_exists(self.repos.restricted_repo_path, self.repos.restricted_repo_changelog)
+            self.utils.remove_file_if_exists(self.repos.restricted_repo_path, self.repos.restricted_repo_checksums)
+
+            down = Downloader(self.repos.restricted_repo_path, urls, self.flags)
+            down.download()
+            print()
+
+        self.delete_bin_database_data(self.repos.restricted_repo_name)
+        self.delete_last_updated(self.repos.restricted_repo_name)
+        self.data.install_restricted_data()
+        print()
 
     def gnome_repository(self) -> None:
-        if self.repos.gnome_repo:
-
-            if not self.repos.gnome_repo_mirror[0].startswith('file'):
-                print(f"Downloading the '{self.green}{self.repos.gnome_repo_name}{self.endc}' "
-                      f"repository, please wait...\n")
-                urls: list = []
-                self.make_dirs(self.repos.gnome_repo_name)
-
-                urls.append(f'{self.repos.gnome_repo_mirror[0]}{self.repos.gnome_repo_packages}')
-                urls.append(f'{self.repos.gnome_repo_mirror[0]}{self.repos.gnome_repo_changelog}')
-                urls.append(f'{self.repos.gnome_repo_mirror[0]}{self.repos.gnome_repo_checksums}')
-
-                self.utils.remove_file_if_exists(self.repos.gnome_repo_path, self.repos.gnome_repo_packages)
-                self.utils.remove_file_if_exists(self.repos.gnome_repo_path, self.repos.gnome_repo_changelog)
-                self.utils.remove_file_if_exists(self.repos.gnome_repo_path, self.repos.gnome_repo_checksums)
-
-                down = Downloader(self.repos.gnome_repo_path, urls, self.flags)
-                down.download()
-                print()
-
-            self.delete_bin_database_data(self.repos.gnome_repo_name)
-            self.delete_last_updated(self.repos.gnome_repo_name)
-            self.data.install_gnome_data()
-            print()
-        else:
-            self.not_enabled_message(self.repos.gnome_repo_name)
+        if not self.repos.gnome_repo_mirror[0].startswith('file'):
+            print(f"Downloading the '{self.green}{self.repos.gnome_repo_name}{self.endc}' "
+                  f"repository, please wait...\n")
+            urls: list = []
+            self.make_dirs(self.repos.gnome_repo_name)
+
+            urls.append(f'{self.repos.gnome_repo_mirror[0]}{self.repos.gnome_repo_packages}')
+            urls.append(f'{self.repos.gnome_repo_mirror[0]}{self.repos.gnome_repo_changelog}')
+            urls.append(f'{self.repos.gnome_repo_mirror[0]}{self.repos.gnome_repo_checksums}')
+
+            self.utils.remove_file_if_exists(self.repos.gnome_repo_path, self.repos.gnome_repo_packages)
+            self.utils.remove_file_if_exists(self.repos.gnome_repo_path, self.repos.gnome_repo_changelog)
+            self.utils.remove_file_if_exists(self.repos.gnome_repo_path, self.repos.gnome_repo_checksums)
+
+            down = Downloader(self.repos.gnome_repo_path, urls, self.flags)
+            down.download()
+            print()
+
+        self.delete_bin_database_data(self.repos.gnome_repo_name)
+        self.delete_last_updated(self.repos.gnome_repo_name)
+        self.data.install_gnome_data()
+        print()
 
     def msb_repository(self) -> None:
-        if self.repos.msb_repo:
-
-            if not self.repos.msb_repo_mirror[0].startswith('file'):
-                print(f"Downloading the '{self.green}{self.repos.msb_repo_name}{self.endc}' "
-                      f"repository, please wait...\n")
-                urls: list = []
-                self.make_dirs(self.repos.msb_repo_name)
-
-                urls.append(f'{"".join(self.repos.msb_repo_mirror)}{self.repos.msb_repo_packages}')
-                urls.append(f'{self.repos.msb_repo_mirror[0]}{self.repos.msb_repo_changelog}')
-                urls.append(f'{self.repos.msb_repo_mirror[0]}{self.repos.msb_repo_checksums}')
-
-                self.utils.remove_file_if_exists(self.repos.msb_repo_path,
-                                                 self.repos.msb_repo_packages)
-                self.utils.remove_file_if_exists(self.repos.msb_repo_path,
-                                                 self.repos.msb_repo_changelog)
-                self.utils.remove_file_if_exists(self.repos.msb_repo_path,
-                                                 self.repos.msb_repo_checksums)
-
-                down = Downloader(self.repos.msb_repo_path, urls, self.flags)
-                down.download()
-                print()
-
-            self.delete_bin_database_data(self.repos.msb_repo_name)
-            self.delete_last_updated(self.repos.msb_repo_name)
-            self.data.install_msb_data()
-            print()
-        else:
-            self.not_enabled_message(self.repos.msb_repo_name)
+        if not self.repos.msb_repo_mirror[0].startswith('file'):
+            print(f"Downloading the '{self.green}{self.repos.msb_repo_name}{self.endc}' "
+                  f"repository, please wait...\n")
+            urls: list = []
+            self.make_dirs(self.repos.msb_repo_name)
+
+            urls.append(f'{"".join(self.repos.msb_repo_mirror)}{self.repos.msb_repo_packages}')
+            urls.append(f'{self.repos.msb_repo_mirror[0]}{self.repos.msb_repo_changelog}')
+            urls.append(f'{self.repos.msb_repo_mirror[0]}{self.repos.msb_repo_checksums}')
+
+            self.utils.remove_file_if_exists(self.repos.msb_repo_path,
+                                             self.repos.msb_repo_packages)
+            self.utils.remove_file_if_exists(self.repos.msb_repo_path,
+                                             self.repos.msb_repo_changelog)
+            self.utils.remove_file_if_exists(self.repos.msb_repo_path,
+                                             self.repos.msb_repo_checksums)
+
+            down = Downloader(self.repos.msb_repo_path, urls, self.flags)
+            down.download()
+            print()
+
+        self.delete_bin_database_data(self.repos.msb_repo_name)
+        self.delete_last_updated(self.repos.msb_repo_name)
+        self.data.install_msb_data()
+        print()
 
     def csb_repository(self) -> None:
-        if self.repos.csb_repo:
-
-            if not self.repos.csb_repo_mirror[0].startswith('file'):
-                print(f"Downloading the '{self.green}{self.repos.csb_repo_name}{self.endc}' "
-                      f"repository, please wait...\n")
-                urls: list = []
-                self.make_dirs(self.repos.csb_repo_name)
-
-                urls.append(f'{"".join(self.repos.csb_repo_mirror)}{self.repos.csb_repo_packages}')
-                urls.append(f'{self.repos.csb_repo_mirror[0]}{self.repos.csb_repo_changelog}')
-                urls.append(f'{self.repos.csb_repo_mirror[0]}{self.repos.csb_repo_checksums}')
-
-                self.utils.remove_file_if_exists(self.repos.csb_repo_path,
-                                                 self.repos.csb_repo_packages)
-                self.utils.remove_file_if_exists(self.repos.csb_repo_path,
-                                                 self.repos.csb_repo_changelog)
-                self.utils.remove_file_if_exists(self.repos.csb_repo_path,
-                                                 self.repos.csb_repo_checksums)
-
-                down = Downloader(self.repos.csb_repo_path, urls, self.flags)
-                down.download()
-                print()
-
-            self.delete_bin_database_data(self.repos.csb_repo_name)
-            self.delete_last_updated(self.repos.csb_repo_name)
-            self.data.install_csb_data()
-            print()
-        else:
-            self.not_enabled_message(self.repos.csb_repo_name)
+        if not self.repos.csb_repo_mirror[0].startswith('file'):
+            print(f"Downloading the '{self.green}{self.repos.csb_repo_name}{self.endc}' "
+                  f"repository, please wait...\n")
+            urls: list = []
+            self.make_dirs(self.repos.csb_repo_name)
+
+            urls.append(f'{"".join(self.repos.csb_repo_mirror)}{self.repos.csb_repo_packages}')
+            urls.append(f'{self.repos.csb_repo_mirror[0]}{self.repos.csb_repo_changelog}')
+            urls.append(f'{self.repos.csb_repo_mirror[0]}{self.repos.csb_repo_checksums}')
+
+            self.utils.remove_file_if_exists(self.repos.csb_repo_path,
+                                             self.repos.csb_repo_packages)
+            self.utils.remove_file_if_exists(self.repos.csb_repo_path,
+                                             self.repos.csb_repo_changelog)
+            self.utils.remove_file_if_exists(self.repos.csb_repo_path,
+                                             self.repos.csb_repo_checksums)
+
+            down = Downloader(self.repos.csb_repo_path, urls, self.flags)
+            down.download()
+            print()
+
+        self.delete_bin_database_data(self.repos.csb_repo_name)
+        self.delete_last_updated(self.repos.csb_repo_name)
+        self.data.install_csb_data()
+        print()
 
     def conraid_repository(self) -> None:
-        if self.repos.conraid_repo:
-
-            if not self.repos.conraid_repo_mirror[0].startswith('file'):
-                print(f"Downloading the '{self.green}{self.repos.conraid_repo_name}{self.endc}' "
-                      f"repository, please wait...\n")
-                urls: list = []
-                self.make_dirs(self.repos.conraid_repo_name)
-
-                urls.append(f'{self.repos.conraid_repo_mirror[0]}{self.repos.conraid_repo_packages}')
-                urls.append(f'{self.repos.conraid_repo_mirror[0]}{self.repos.conraid_repo_changelog}')
-                urls.append(f'{self.repos.conraid_repo_mirror[0]}{self.repos.conraid_repo_checksums}')
-
-                self.utils.remove_file_if_exists(self.repos.conraid_repo_path, self.repos.conraid_repo_packages)
-                self.utils.remove_file_if_exists(self.repos.conraid_repo_path, self.repos.conraid_repo_changelog)
-                self.utils.remove_file_if_exists(self.repos.conraid_repo_path, self.repos.conraid_repo_checksums)
-
-                down = Downloader(self.repos.conraid_repo_path, urls, self.flags)
-                down.download()
-                print()
-
-            self.delete_bin_database_data(self.repos.conraid_repo_name)
-            self.delete_last_updated(self.repos.conraid_repo_name)
-            self.data.install_conraid_data()
-            print()
-        else:
-            self.not_enabled_message(self.repos.conraid_repo_name)
+        if not self.repos.conraid_repo_mirror[0].startswith('file'):
+            print(f"Downloading the '{self.green}{self.repos.conraid_repo_name}{self.endc}' "
+                  f"repository, please wait...\n")
+            urls: list = []
+            self.make_dirs(self.repos.conraid_repo_name)
+
+            urls.append(f'{self.repos.conraid_repo_mirror[0]}{self.repos.conraid_repo_packages}')
+            urls.append(f'{self.repos.conraid_repo_mirror[0]}{self.repos.conraid_repo_changelog}')
+            urls.append(f'{self.repos.conraid_repo_mirror[0]}{self.repos.conraid_repo_checksums}')
+
+            self.utils.remove_file_if_exists(self.repos.conraid_repo_path, self.repos.conraid_repo_packages)
+            self.utils.remove_file_if_exists(self.repos.conraid_repo_path, self.repos.conraid_repo_changelog)
+            self.utils.remove_file_if_exists(self.repos.conraid_repo_path, self.repos.conraid_repo_checksums)
+
+            down = Downloader(self.repos.conraid_repo_path, urls, self.flags)
+            down.download()
+            print()
+
+        self.delete_bin_database_data(self.repos.conraid_repo_name)
+        self.delete_last_updated(self.repos.conraid_repo_name)
+        self.data.install_conraid_data()
+        print()
 
     def slackonly_repository(self) -> None:
-        if self.repos.slackonly_repo:
-
-            if not self.repos.slackonly_repo_mirror[0].startswith('file'):
-                print(f"Downloading the '{self.green}{self.repos.slackonly_repo_name}{self.endc}' "
-                      f"repository, please wait...\n")
-                urls: list = []
-                self.make_dirs(self.repos.slackonly_repo_name)
-
-                urls.append(f'{self.repos.slackonly_repo_mirror[0]}{self.repos.slackonly_repo_packages}')
-                urls.append(f'{self.repos.slackonly_repo_mirror[0]}{self.repos.slackonly_repo_changelog}')
-                urls.append(f'{self.repos.slackonly_repo_mirror[0]}{self.repos.slackonly_repo_checksums}')
-
-                self.utils.remove_file_if_exists(self.repos.slackonly_repo_path, self.repos.slackonly_repo_packages)
-                self.utils.remove_file_if_exists(self.repos.slackonly_repo_path, self.repos.slackonly_repo_changelog)
-                self.utils.remove_file_if_exists(self.repos.slackonly_repo_path, self.repos.slackonly_repo_checksums)
-
-                down = Downloader(self.repos.slackonly_repo_path, urls, self.flags)
-                down.download()
-                print()
-
-            self.delete_bin_database_data(self.repos.slackonly_repo_name)
-            self.delete_last_updated(self.repos.slackonly_repo_name)
-            self.data.install_slackonly_data()
-            print()
-        else:
-            self.not_enabled_message(self.repos.slackonly_repo_name)
+        if not self.repos.slackonly_repo_mirror[0].startswith('file'):
+            print(f"Downloading the '{self.green}{self.repos.slackonly_repo_name}{self.endc}' "
+                  f"repository, please wait...\n")
+            urls: list = []
+            self.make_dirs(self.repos.slackonly_repo_name)
+
+            urls.append(f'{self.repos.slackonly_repo_mirror[0]}{self.repos.slackonly_repo_packages}')
+            urls.append(f'{self.repos.slackonly_repo_mirror[0]}{self.repos.slackonly_repo_changelog}')
+            urls.append(f'{self.repos.slackonly_repo_mirror[0]}{self.repos.slackonly_repo_checksums}')
+
+            self.utils.remove_file_if_exists(self.repos.slackonly_repo_path, self.repos.slackonly_repo_packages)
+            self.utils.remove_file_if_exists(self.repos.slackonly_repo_path, self.repos.slackonly_repo_changelog)
+            self.utils.remove_file_if_exists(self.repos.slackonly_repo_path, self.repos.slackonly_repo_checksums)
+
+            down = Downloader(self.repos.slackonly_repo_path, urls, self.flags)
+            down.download()
+            print()
+
+        self.delete_bin_database_data(self.repos.slackonly_repo_name)
+        self.delete_last_updated(self.repos.slackonly_repo_name)
+        self.data.install_slackonly_data()
+        print()
 
     def salixos_repository(self) -> None:
-        if self.repos.salixos_repo:
-
-            if not self.repos.salixos_repo_mirror[0].startswith('file'):
-                print(f"Downloading the '{self.green}{self.repos.salixos_repo_name}{self.endc}' "
-                      f"repository, please wait...\n")
-                urls: list = []
-                self.make_dirs(self.repos.salixos_repo_name)
-
-                urls.append(f'{self.repos.salixos_repo_mirror[0]}{self.repos.salixos_repo_packages}')
-                urls.append(f'{self.repos.salixos_repo_mirror[0]}{self.repos.salixos_repo_changelog}')
-                urls.append(f'{self.repos.salixos_repo_mirror[0]}{self.repos.salixos_repo_checksums}')
-
-                self.utils.remove_file_if_exists(self.repos.salixos_repo_path, self.repos.salixos_repo_packages)
-                self.utils.remove_file_if_exists(self.repos.salixos_repo_path, self.repos.salixos_repo_changelog)
-                self.utils.remove_file_if_exists(self.repos.salixos_repo_path, self.repos.salixos_repo_checksums)
-
-                down = Downloader(self.repos.salixos_repo_path, urls, self.flags)
-                down.download()
-                print()
-
-            self.delete_bin_database_data(self.repos.salixos_repo_name)
-            self.delete_last_updated(self.repos.salixos_repo_name)
-            self.data.install_salixos_data()
-            print()
-        else:
-            self.not_enabled_message(self.repos.salixos_repo_name)
+        if not self.repos.salixos_repo_mirror[0].startswith('file'):
+            print(f"Downloading the '{self.green}{self.repos.salixos_repo_name}{self.endc}' "
+                  f"repository, please wait...\n")
+            urls: list = []
+            self.make_dirs(self.repos.salixos_repo_name)
+
+            urls.append(f'{self.repos.salixos_repo_mirror[0]}{self.repos.salixos_repo_packages}')
+            urls.append(f'{self.repos.salixos_repo_mirror[0]}{self.repos.salixos_repo_changelog}')
+            urls.append(f'{self.repos.salixos_repo_mirror[0]}{self.repos.salixos_repo_checksums}')
+
+            self.utils.remove_file_if_exists(self.repos.salixos_repo_path, self.repos.salixos_repo_packages)
+            self.utils.remove_file_if_exists(self.repos.salixos_repo_path, self.repos.salixos_repo_changelog)
+            self.utils.remove_file_if_exists(self.repos.salixos_repo_path, self.repos.salixos_repo_checksums)
+
+            down = Downloader(self.repos.salixos_repo_path, urls, self.flags)
+            down.download()
+            print()
+
+        self.delete_bin_database_data(self.repos.salixos_repo_name)
+        self.delete_last_updated(self.repos.salixos_repo_name)
+        self.data.install_salixos_data()
+        print()
 
     def salixos_extra_repository(self) -> None:
-        if self.repos.salixos_extra_repo:
-
-            if not self.repos.salixos_extra_repo_mirror[0].startswith('file'):
-                print(f"Downloading the '{self.green}{self.repos.salixos_extra_repo_name}{self.endc}' "
-                      f"repository, please wait...\n")
-                urls: list = []
-                self.make_dirs(self.repos.salixos_extra_repo_name)
-
-                urls.append(f'{"".join(self.repos.salixos_extra_repo_mirror)}{self.repos.salixos_extra_repo_packages}')
-                urls.append(f'{self.repos.salixos_extra_repo_mirror[0]}{self.repos.salixos_extra_repo_changelog}')
-                urls.append(f'{self.repos.salixos_extra_repo_mirror[0]}{self.repos.salixos_extra_repo_checksums}')
-
-                self.utils.remove_file_if_exists(self.repos.salixos_extra_repo_path,
-                                                 self.repos.salixos_extra_repo_packages)
-                self.utils.remove_file_if_exists(self.repos.salixos_extra_repo_path,
-                                                 self.repos.salixos_extra_repo_changelog)
-                self.utils.remove_file_if_exists(self.repos.salixos_extra_repo_path,
-                                                 self.repos.salixos_extra_repo_checksums)
-
-                down = Downloader(self.repos.salixos_extra_repo_path, urls, self.flags)
-                down.download()
-                print()
-
-            self.delete_bin_database_data(self.repos.salixos_extra_repo_name)
-            self.delete_last_updated(self.repos.salixos_extra_repo_name)
-            self.data.install_salixos_extra_data()
-            print()
-        else:
-            self.not_enabled_message(self.repos.salixos_extra_repo_name)
+        if not self.repos.salixos_extra_repo_mirror[0].startswith('file'):
+            print(f"Downloading the '{self.green}{self.repos.salixos_extra_repo_name}{self.endc}' "
+                  f"repository, please wait...\n")
+            urls: list = []
+            self.make_dirs(self.repos.salixos_extra_repo_name)
+
+            urls.append(f'{"".join(self.repos.salixos_extra_repo_mirror)}{self.repos.salixos_extra_repo_packages}')
+            urls.append(f'{self.repos.salixos_extra_repo_mirror[0]}{self.repos.salixos_extra_repo_changelog}')
+            urls.append(f'{self.repos.salixos_extra_repo_mirror[0]}{self.repos.salixos_extra_repo_checksums}')
+
+            self.utils.remove_file_if_exists(self.repos.salixos_extra_repo_path,
+                                             self.repos.salixos_extra_repo_packages)
+            self.utils.remove_file_if_exists(self.repos.salixos_extra_repo_path,
+                                             self.repos.salixos_extra_repo_changelog)
+            self.utils.remove_file_if_exists(self.repos.salixos_extra_repo_path,
+                                             self.repos.salixos_extra_repo_checksums)
+
+            down = Downloader(self.repos.salixos_extra_repo_path, urls, self.flags)
+            down.download()
+            print()
+
+        self.delete_bin_database_data(self.repos.salixos_extra_repo_name)
+        self.delete_last_updated(self.repos.salixos_extra_repo_name)
+        self.data.install_salixos_extra_data()
+        print()
 
     def salixos_patches_repository(self) -> None:
-        if self.repos.salixos_patches_repo:
-
-            if not self.repos.salixos_patches_repo_mirror[0].startswith('file'):
-                print(f"Downloading the '{self.green}{self.repos.salixos_patches_repo_name}{self.endc}' "
-                      f"repository, please wait...\n")
-                urls: list = []
-                self.make_dirs(self.repos.salixos_patches_repo_name)
-
-                urls.append(f'{"".join(self.repos.salixos_patches_repo_mirror)}'
-                            f'{self.repos.salixos_patches_repo_packages}')
-                urls.append(f'{self.repos.salixos_patches_repo_mirror[0]}{self.repos.salixos_patches_repo_changelog}')
-                urls.append(f'{self.repos.salixos_patches_repo_mirror[0]}{self.repos.salixos_patches_repo_checksums}')
-
-                self.utils.remove_file_if_exists(self.repos.salixos_patches_repo_path,
-                                                 self.repos.salixos_patches_repo_packages)
-                self.utils.remove_file_if_exists(self.repos.salixos_patches_repo_path,
-                                                 self.repos.salixos_patches_repo_changelog)
-                self.utils.remove_file_if_exists(self.repos.salixos_patches_repo_path,
-                                                 self.repos.salixos_patches_repo_checksums)
-
-                down = Downloader(self.repos.salixos_patches_repo_path, urls, self.flags)
-                down.download()
-                print()
-
-            self.delete_bin_database_data(self.repos.salixos_patches_repo_name)
-            self.delete_last_updated(self.repos.salixos_patches_repo_name)
-            self.data.install_salixos_patches_data()
-            print()
-        else:
-            self.not_enabled_message(self.repos.salixos_patches_repo_name)
+        if not self.repos.salixos_patches_repo_mirror[0].startswith('file'):
+            print(f"Downloading the '{self.green}{self.repos.salixos_patches_repo_name}{self.endc}' "
+                  f"repository, please wait...\n")
+            urls: list = []
+            self.make_dirs(self.repos.salixos_patches_repo_name)
+
+            urls.append(f'{"".join(self.repos.salixos_patches_repo_mirror)}'
+                        f'{self.repos.salixos_patches_repo_packages}')
+            urls.append(f'{self.repos.salixos_patches_repo_mirror[0]}{self.repos.salixos_patches_repo_changelog}')
+            urls.append(f'{self.repos.salixos_patches_repo_mirror[0]}{self.repos.salixos_patches_repo_checksums}')
+
+            self.utils.remove_file_if_exists(self.repos.salixos_patches_repo_path,
+                                             self.repos.salixos_patches_repo_packages)
+            self.utils.remove_file_if_exists(self.repos.salixos_patches_repo_path,
+                                             self.repos.salixos_patches_repo_changelog)
+            self.utils.remove_file_if_exists(self.repos.salixos_patches_repo_path,
+                                             self.repos.salixos_patches_repo_checksums)
+
+            down = Downloader(self.repos.salixos_patches_repo_path, urls, self.flags)
+            down.download()
+            print()
+
+        self.delete_bin_database_data(self.repos.salixos_patches_repo_name)
+        self.delete_last_updated(self.repos.salixos_patches_repo_name)
+        self.data.install_salixos_patches_data()
+        print()
 
     def slackel_repository(self) -> None:
-        if self.repos.slackel_repo:
-
-            if not self.repos.slackel_repo_mirror[0].startswith('file'):
-                print(f"Downloading the '{self.green}{self.repos.slackel_repo_name}{self.endc}' "
-                      f"repository, please wait...\n")
-                urls: list = []
-                self.make_dirs(self.repos.slackel_repo_name)
-
-                urls.append(f'{self.repos.slackel_repo_mirror[0]}{self.repos.slackel_repo_packages}')
-                urls.append(f'{self.repos.slackel_repo_mirror[0]}{self.repos.slackel_repo_changelog}')
-                urls.append(f'{self.repos.slackel_repo_mirror[0]}{self.repos.slackel_repo_checksums}')
-
-                self.utils.remove_file_if_exists(self.repos.slackel_repo_path, self.repos.slackel_repo_packages)
-                self.utils.remove_file_if_exists(self.repos.slackel_repo_path, self.repos.slackel_repo_changelog)
-                self.utils.remove_file_if_exists(self.repos.slackel_repo_path, self.repos.slackel_repo_checksums)
-
-                down = Downloader(self.repos.slackel_repo_path, urls, self.flags)
-                down.download()
-                print()
-
-            self.delete_bin_database_data(self.repos.slackel_repo_name)
-            self.delete_last_updated(self.repos.slackel_repo_name)
-            self.data.install_slackel_data()
-            print()
-        else:
-            self.not_enabled_message(self.repos.slackel_repo_name)
+        if not self.repos.slackel_repo_mirror[0].startswith('file'):
+            print(f"Downloading the '{self.green}{self.repos.slackel_repo_name}{self.endc}' "
+                  f"repository, please wait...\n")
+            urls: list = []
+            self.make_dirs(self.repos.slackel_repo_name)
+
+            urls.append(f'{self.repos.slackel_repo_mirror[0]}{self.repos.slackel_repo_packages}')
+            urls.append(f'{self.repos.slackel_repo_mirror[0]}{self.repos.slackel_repo_changelog}')
+            urls.append(f'{self.repos.slackel_repo_mirror[0]}{self.repos.slackel_repo_checksums}')
+
+            self.utils.remove_file_if_exists(self.repos.slackel_repo_path, self.repos.slackel_repo_packages)
+            self.utils.remove_file_if_exists(self.repos.slackel_repo_path, self.repos.slackel_repo_changelog)
+            self.utils.remove_file_if_exists(self.repos.slackel_repo_path, self.repos.slackel_repo_checksums)
+
+            down = Downloader(self.repos.slackel_repo_path, urls, self.flags)
+            down.download()
+            print()
+
+        self.delete_bin_database_data(self.repos.slackel_repo_name)
+        self.delete_last_updated(self.repos.slackel_repo_name)
+        self.data.install_slackel_data()
+        print()
 
     def slint_repository(self) -> None:
-        if self.repos.slint_repo:
-
-            if not self.repos.slint_repo_mirror[0].startswith('file'):
-                print(f"Downloading the '{self.green}{self.repos.slint_repo_name}{self.endc}' "
-                      f"repository, please wait...\n")
-                urls: list = []
-                self.make_dirs(self.repos.slint_repo_name)
-
-                urls.append(f'{self.repos.slint_repo_mirror[0]}{self.repos.slint_repo_packages}')
-                urls.append(f'{self.repos.slint_repo_mirror[0]}{self.repos.slint_repo_changelog}')
-                urls.append(f'{self.repos.slint_repo_mirror[0]}{self.repos.slint_repo_checksums}')
-
-                self.utils.remove_file_if_exists(self.repos.slint_repo_path, self.repos.slint_repo_packages)
-                self.utils.remove_file_if_exists(self.repos.slint_repo_path, self.repos.slint_repo_changelog)
-                self.utils.remove_file_if_exists(self.repos.slint_repo_path, self.repos.slint_repo_checksums)
-
-                down = Downloader(self.repos.slint_repo_path, urls, self.flags)
-                down.download()
-                print()
-
-            self.delete_bin_database_data(self.repos.slint_repo_name)
-            self.delete_last_updated(self.repos.slint_repo_name)
-            self.data.install_slint_data()
-            print()
-        else:
-            self.not_enabled_message(self.repos.slint_repo_name)
+        if not self.repos.slint_repo_mirror[0].startswith('file'):
+            print(f"Downloading the '{self.green}{self.repos.slint_repo_name}{self.endc}' "
+                  f"repository, please wait...\n")
+            urls: list = []
+            self.make_dirs(self.repos.slint_repo_name)
+
+            urls.append(f'{self.repos.slint_repo_mirror[0]}{self.repos.slint_repo_packages}')
+            urls.append(f'{self.repos.slint_repo_mirror[0]}{self.repos.slint_repo_changelog}')
+            urls.append(f'{self.repos.slint_repo_mirror[0]}{self.repos.slint_repo_checksums}')
+
+            self.utils.remove_file_if_exists(self.repos.slint_repo_path, self.repos.slint_repo_packages)
+            self.utils.remove_file_if_exists(self.repos.slint_repo_path, self.repos.slint_repo_changelog)
+            self.utils.remove_file_if_exists(self.repos.slint_repo_path, self.repos.slint_repo_checksums)
+
+            down = Downloader(self.repos.slint_repo_path, urls, self.flags)
+            down.download()
+            print()
+
+        self.delete_bin_database_data(self.repos.slint_repo_name)
+        self.delete_last_updated(self.repos.slint_repo_name)
+        self.data.install_slint_data()
+        print()
 
     def slackbuild_repositories(self) -> None:
         """ Update the slackbuild repositories. """
         if self.repos.ponce_repo:
 
-            if (not self.utils.is_option(self.flag_generate, self.flags) or
-                    not self.repos.ponce_repo_mirror[0].startswith('file')):
+            if not self.option_for_generate or not self.repos.ponce_repo_mirror[0].startswith('file'):
                 print(f"Downloading the '{self.green}{self.repos.ponce_repo_name}"
                       f"{self.endc}' repository, please wait...\n")
                 self.make_dirs(self.repos.gnome_repo_name)
                 self.utils.remove_file_if_exists(self.repos.ponce_repo_path, self.repos.ponce_repo_slackbuilds)
                 lftp_command: str = (f'lftp {self.lftp_mirror_options} {self.repos.ponce_repo_mirror[0]} '
                                      f'{self.repos.ponce_repo_path}')
                 self.utils.process(lftp_command)
@@ -599,38 +527,33 @@
                 self.utils.process(lftp_command)
 
             self.delete_last_updated(self.repos.sbo_repo_name)
 
         self.delete_sbo_database_data()
         self.data.install_sbos_data()
 
-    def not_enabled_message(self, repo: str) -> None:
-        print(f"{self.prog_name}: Repository '{self.green}{repo}{self.endc}' is not enabled.")
-
     def make_dirs(self, repo) -> None:
         path = Path(self.repos.repositories_path, repo)
         if not os.path.isdir(path):
             os.makedirs(path)
 
     def check(self, queue) -> None:
-        compare = self.check_updates.check()
-        is_update: dict = {}
+        compare: dict = self.check_updates.check()
 
         print()
         for repo, comp in compare.items():
             if comp:
                 print(f"\n{self.endc}There are new updates available for the "
                       f"'{self.bgreen}{repo}{self.endc}' repository!")
-                is_update[repo] = comp
 
-        if True not in compare.values():
+        if not any(list(compare.values())):
             print(f'\n{self.endc}{self.yellow}No changes in ChangeLog.txt between your '
                   f'last update and now.{self.endc}')
 
-        return queue.put(is_update)
+        return queue.put(compare)
 
     def repositories(self) -> None:
         queue = Queue()
         message = f'Checking for news, please wait...'
 
         # Starting multiprocessing
         p1 = Process(target=self.check, args=(queue,))
@@ -648,15 +571,15 @@
 
         # Wait until process 2 finish
         p2.join()
 
         # Restore the terminal cursor
         print('\x1b[?25h', self.endc, end='')
 
-        self.repos_for_update = queue.get()
+        self.repos_for_update: dict = queue.get()
         self.update_the_repositories()
 
     def delete_sbo_database_data(self) -> None:
         """ Delete all the data from a table of the database. """
         if self.repos.ponce_repo:
             self.session.query(PonceTable).delete()
         else:
@@ -671,15 +594,16 @@
     def delete_last_updated(self, repo) -> None:
         """ Deletes the last updated date. """
         self.session.query(LastRepoUpdated).where(LastRepoUpdated.repo == repo).delete()
         self.session.commit()
 
     def drop_the_tables(self) -> None:
         """ Drop all the tables from the database. """
-        print(f'\n{self.prog_name}: {self.bred}WARNING{self.endc}: All the data from the database will be deleted!')
+        print(f'\n{self.prog_name}: {self.blink}{self.bold}{self.bred}WARNING!{self.endc}: '
+              f'All the data from the database will be deleted!')
         self.view.question()
 
         tables: list = [
             PonceTable.__table__,
             SBoTable.__table__,
             BinariesTable.__table__,
             LastRepoUpdated.__table__
@@ -698,8 +622,8 @@
 
             repo_path: Path = Path(self.repos.repositories_path, repo)
 
             if repo_path.exists():
                 shutil.rmtree(repo_path)
                 print(f"Deleted: '{repo_path}'")
 
-        print()  # new line at the end
+        print()
```

### Comparing `slpkg-4.8.0/slpkg/downloader.py` & `slpkg-4.8.1/slpkg/downloader.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 from typing import Union
 from pathlib import Path
 from urllib.parse import unquote
 from multiprocessing import Process
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
+from slpkg.error_messages import Errors
 
 
 class Downloader(Configs):
 
     def __init__(self, path: Union[str, Path], urls: list, flags: list):
         __slots__ = 'path', 'urls', 'flags'
         super(Configs, self).__init__()
-        self.path = path
+        self.path: Path = path
         self.urls: list = urls
         self.flags: list = flags
 
+        self.errors = Errors()
         self.utils = Utilities()
 
         self.option_for_parallel: bool = self.utils.is_option(
             ['-P', '--parallel'], self.flags)
 
     def download(self) -> None:
         """ Starting the processing for downloading. """
@@ -55,20 +57,20 @@
             elif self.downloader == 'curl':
                 command: str = f'{self.downloader} {self.curl_options} "{url}" --output {self.path}/{filename}'
 
             elif self.downloader == 'lftp':
                 command: str = f'{self.downloader} {self.lftp_get_options} {url} -o {self.path}'
 
             else:
-                self.utils.raise_error_message(f"Downloader '{self.downloader}' not supported")
+                self.errors.raise_error_message(f"Downloader '{self.downloader}' not supported")
 
         self.utils.process(command)
         self.check_if_downloaded(url)
 
     def check_if_downloaded(self, url: str) -> None:
         """ Checks if the file downloaded. """
         url: str = unquote(url)
         file: str = url.split('/')[-1]
-        path_file = Path(self.path, file)
+        path_file: Path = Path(self.path, file)
 
         if not path_file.exists():
-            self.utils.raise_error_message(f"Download the '{file}' file")
+            self.errors.raise_error_message(f"Download the '{file}' file")
```

### Comparing `slpkg-4.8.0/slpkg/models/models.py` & `slpkg-4.8.1/slpkg/models/models.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.0/slpkg/views/view_package.py` & `slpkg-4.8.1/slpkg/views/view_package.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,31 +19,22 @@
         super(Configs, self).__init__()
         self.flags: list = flags
 
         self.utils = Utilities()
         self.repos = Repositories()
         self.session = Session
         
-        self.color = self.colour()
-        self.green: str = self.color['green']
-        self.blue: str = self.color['blue']
-        self.yellow: str = self.color['yellow']
-        self.cyan: str = self.color['cyan']
-        self.red: str = self.color['red']
-        self.violet: str = self.color['violet']
-        self.endc: str = self.color['endc']
-
         # Switch between sbo and ponce repository.
         self.sbo_table = SBoTable
         self.repo_url: str = self.repos.sbo_repo_mirror[0]
         self.repo_path: Path = self.repos.sbo_repo_path
         self.repo_tar_suffix: str = self.repos.sbo_repo_tar_suffix
         if self.repos.ponce_repo:
             self.sbo_table = PonceTable
-            self.repo_url: str = self.repos.ponce_repo_mirror
+            self.repo_url: str = self.repos.ponce_repo_mirror[0]
             self.repo_path: Path = self.repos.ponce_repo_path
             self.repo_tar_suffix: str = ''
 
         self.option_for_pkg_version: bool = self.utils.is_option(
             ['-p', '--pkg-version'], self.flags)
 
     def slackbuild(self, data: dict, slackbuilds: list) -> None:
```

### Comparing `slpkg-4.8.0/slpkg/views/version.py` & `slpkg-4.8.1/slpkg/views/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 class Version:
     """ Print the version. """
 
     def __init__(self):
-        self.version_info: tuple = (4, 8, 0)
+        self.version_info: tuple = (4, 8, 1)
         self.version: str = '{0}.{1}.{2}'.format(*self.version_info)
         self.license: str = 'MIT License'
         self.author: str = 'Dimitris Zlatanidis (dslackw)'
         self.homepage: str = 'https://dslackw.gitlab.io/slpkg'
 
     def view(self) -> None:
         """ Prints the version. """
```

### Comparing `slpkg-4.8.0/slpkg/views/cli_menu.py` & `slpkg-4.8.1/slpkg/views/cli_menu.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,36 +5,29 @@
 from slpkg.configs import Configs
 
 
 class Usage(Configs):
 
     def __init__(self):
         super(Configs, self).__init__()
-        color = self.colour()
-
-        self.bold: str = color['bold']
-        self.red: str = color['red']
-        self.cyan: str = color['cyan']
-        self.yellow: str = color['yellow']
-        self.endc: str = color['endc']
 
     def help_minimal(self, message: str) -> NoReturn:
         """ Prints the minimal help menu. """
         print(message)
         args: str = (
             f'\nUsage: {self.prog_name} [{self.cyan}COMMAND{self.endc}] [{self.yellow}OPTIONS{self.endc}] '
             f'[FILELIST|PACKAGES...]\n'
             f"\nTry '{self.prog_name} --help' for more options.\n")
 
         print(args)
         raise SystemExit(1)
 
     def help_short(self, status: int) -> NoReturn:
         """ Prints the short menu. """
-        args = (
+        args: str = (
             f'Usage: {self.prog_name} [{self.cyan}COMMAND{self.endc}] [{self.yellow}OPTIONS{self.endc}] '
             f'[FILELIST|PACKAGES...]\n'
             f'\n  slpkg [{self.cyan}COMMAND{self.endc}] [-u, update, -U, upgrade, -c, check-updates, -I, repo-info]\n'
             f'  slpkg [{self.cyan}COMMAND{self.endc}] [-L, clean-logs, -T, clean-data, -D, clean-tmp, -g, configs]\n'
             f'  slpkg [{self.cyan}COMMAND{self.endc}] [-b, build, -i, install, -d, download [packages...]]\n'
             f'  slpkg [{self.cyan}COMMAND{self.endc}] [-R, remove, -f, find, -w, view [packages...]]\n'
             f'  slpkg [{self.cyan}COMMAND{self.endc}] [-s, search, -e, dependees, -t, tracking  [packages...]]\n'
```

### Comparing `slpkg-4.8.0/slpkg/views/ascii.py` & `slpkg-4.8.1/slpkg/views/ascii.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from slpkg.configs import Configs
 
 
 class Ascii(Configs):
     """ ascii characters. """
     def __init__(self):
         super(Configs, self).__init__()
-        self.color = self.colour()
         self.columns, self.rows = shutil.get_terminal_size()
 
         self.vertical_line: str = '|'
         self.horizontal_line: str = '='
         self.horizontal_vertical: str = '+'
         self.upper_right_corner: str = '+'
         self.lower_left_corner: str = '+'
@@ -34,25 +33,14 @@
             self.lower_right_corner: str = '┘'
             self.upper_left_corner: str = '┌'
             self.horizontal_and_up: str = '┴'
             self.horizontal_and_down: str = '┬'
             self.vertical_and_right: str = '├'
             self.vertical_and_left: str = '┤'
 
-        self.bold: str = self.color['bold']
-        self.blue: str = self.color['blue']
-        self.green: str = self.color['green']
-        self.cyan: str = self.color['cyan']
-        self.red: str = self.color['red']
-        self.yellow: str = self.color['yellow']
-        self.violet: str = self.color['violet']
-        self.endc: str = self.color['endc']
-        self.bgreen: str = f'{self.bold}{self.green}'
-        self.bred: str = f'{self.bold}{self.red}'
-
     def draw_package_title_box(self, message: str, title: str) -> None:
         """ Drawing package title box. """
         title = title.title()
         middle_title: int = int((self.columns / 2) - len(title) + 10)
 
         print(f'{self.bgreen}{self.upper_left_corner}' + f'{self.horizontal_line}' * (self.columns - 2) +
               f'{self.upper_right_corner}')
```

### Comparing `slpkg-4.8.0/slpkg/views/help_commands.py` & `slpkg-4.8.1/slpkg/views/help_commands.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,22 +8,14 @@
 
     def __init__(self, command: str, flags: list):
         __slots__ = 'command', 'flags'
         super(Configs, self).__init__()
         self.command: str = command
         self.flags: list = flags
 
-        color = self.colour()
-
-        self.bold: str = color['bold']
-        self.green: str = color['green']
-        self.cyan: str = color['cyan']
-        self.yellow: str = color['yellow']
-        self.endc: str = color['endc']
-
     def view(self) -> None:
         self.flags.reverse()  # Put first the short options.
 
         help_commands: dict = {
             'update': "Updates the package list and the database.",
             'upgrade': "Upgrade all the installed packages if the newer version exists in the repository.",
             'check-updates': "Check if there is any news on the repositories ChangeLog.txt file.",
```

### Comparing `slpkg-4.8.0/slpkg/views/views.py` & `slpkg-4.8.1/slpkg/views/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,24 +25,17 @@
         self.data: dict = data
 
         self.session = Session
         self.utils = Utilities()
         self.dialogbox = DialogBox()
         self.ascii = Ascii()
         self.upgrade = Upgrade(self.flags, self.data)
-        self.color = self.colour()
         self.repos = Repositories()
 
-        self.yellow: str = self.color['yellow']
-        self.cyan: str = self.color['cyan']
-        self.red: str = self.color['red']
-        self.grey: str = self.color['grey']
-        self.violet: str = self.color['violet']
-        self.endc: str = self.color['endc']
-        self.download_only = self.tmp_slpkg
+        self.download_only: Path = self.tmp_slpkg
         self.installed_packages: list = []
 
         self.option_for_resolve_off: bool = self.utils.is_option(
             ['-o', '--resolve-off'], self.flags)
 
         self.option_for_reinstall: bool = self.utils.is_option(
             ['-r', '--reinstall'], self.flags)
```

### Comparing `slpkg-4.8.0/slpkg/checks.py` & `slpkg-4.8.1/slpkg/checks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
+from slpkg.error_messages import Errors
 from slpkg.repositories import Repositories
 from slpkg.models.models import session as Session
 
 from slpkg.models.models import SBoTable, PonceTable, BinariesTable
 
 
 class Check(Configs):
@@ -16,14 +17,15 @@
 
     def __init__(self, flags: list, data: dict):
         __slots__ = 'flags', 'data'
         super(Configs, self).__init__()
         self.flags: list = flags
         self.data: dict = data
 
+        self.errors = Errors()
         self.utils = Utilities()
         self.repos = Repositories()
 
         self.session = Session
 
         self.option_for_binaries: bool = self.utils.is_option(
             ['-B', '--bin-repo='], self.flags)
@@ -45,40 +47,46 @@
                 if not self.data.get(pkg) and pkg != '*':
                     not_packages.append(pkg)
             else:
                 if not self.data.get(pkg) and pkg != '*':
                     not_packages.append(pkg)
 
         if not_packages:
-            self.utils.raise_error_message(f"Packages '{', '.join(not_packages)}' does not exists")
+            self.errors.raise_error_message(f"Packages '{', '.join(not_packages)}' does not exists")
 
     def is_package_unsupported(self, slackbuilds: list) -> None:
         """ Checking for unsupported slackbuilds. """
         for sbo in slackbuilds:
             if sbo != '*':
                 if self.os_arch == 'x86_64' and self.data[sbo][4]:
                     sources: list = self.data[sbo][4].split()
                 else:
                     sources: list = self.data[sbo][3].split()
 
                 if 'UNSUPPORTED' in sources:
-                    self.utils.raise_error_message(f"Package '{sbo}' unsupported by arch")
+                    self.errors.raise_error_message(f"Package '{sbo}' unsupported by arch")
 
     def is_installed(self, packages: list) -> None:
         """ Checking for installed packages. """
-        not_found = []
+        not_found: list = []
 
         for pkg in packages:
             package: str = self.utils.is_package_installed(pkg)
             if not package:
                 not_found.append(pkg)
 
         if not_found:
-            self.utils.raise_error_message(f'Not found \'{", ".join(not_found)}\' installed packages')
+            self.errors.raise_error_message(f'Not found \'{", ".join(not_found)}\' installed packages')
 
-    def is_empty_database(self) -> None:
+    def is_empty_database(self, repo: str) -> None:
         """ Checking for empty table and database file. """
         db = Path(self.db_path, self.database_name)
-        if not self.session.query(self.repo_table).first() or not db.is_file():
-            self.utils.raise_error_message("You need to update the package lists first, run:\n\n"
-                                           "              $ 'slpkg update'\n"
-                                           "              $ 'slpkg update --bin-repo='*' for binaries")
+
+        if self.option_for_binaries and repo != '*':
+            count: int = self.session.query(self.repo_table.id).where(self.repo_table.repo == repo).count()
+        else:
+            count: int = self.session.query(self.repo_table.id).count()
+
+        if not self.session.query(self.repo_table).first() or not db.is_file() or count == 0:
+            self.errors.raise_error_message("You need to update the package lists first, run:\n\n"
+                                            "              $ 'slpkg update'\n"
+                                            "              $ 'slpkg update --bin-repo='*' for binaries")
```

### Comparing `slpkg-4.8.0/slpkg/checksum.py` & `slpkg-4.8.1/slpkg/checksum.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,24 +4,26 @@
 import hashlib
 from pathlib import Path
 from typing import Union
 from urllib.parse import unquote
 
 from slpkg.views.ascii import Ascii
 from slpkg.utilities import Utilities
+from slpkg.error_messages import Errors
 from slpkg.views.views import ViewMessage
 
 
 class Md5sum:
     """ Checksum the sources. """
 
     def __init__(self, flags: list):
         __slots__ = 'flags'
         self.flags: list = flags
         self.ascii = Ascii()
+        self.errors = Errors()
         self.utils = Utilities()
 
     def check(self, path: Union[str, Path], source: str, checksum: str) -> None:
         """ Checksum the source. """
         source_file = unquote(source)
         filename = source_file.split('/')[-1]
         source_path = Path(path, filename)
@@ -39,8 +41,8 @@
 
     def read_file(self, filename: Union[str, Path]) -> bytes:
         """ Reads the text file. """
         try:
             with open(filename, 'rb') as f:
                 return f.read()
         except FileNotFoundError:
-            self.utils.raise_error_message(f"No such file or directory: '{filename}'")
+            self.errors.raise_error_message(f"No such file or directory: '{filename}'")
```

### Comparing `slpkg-4.8.0/slpkg/dialog_box.py` & `slpkg-4.8.1/slpkg/dialog_box.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.0/slpkg/clean_logs.py` & `slpkg-4.8.1/slpkg/clean_logs.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.0/slpkg/utilities.py` & `slpkg-4.8.1/slpkg/utilities.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,34 +8,26 @@
 import fnmatch
 import subprocess
 from pathlib import Path
 from typing import Generator, Union
 
 from slpkg.configs import Configs
 from slpkg.blacklist import Blacklist
+from slpkg.error_messages import Errors
 from slpkg.repositories import Repositories
 from slpkg.logging_config import LoggingConfig
 
 
-class Utilities:
+class Utilities(Configs):
 
     def __init__(self):
-        self.configs = Configs
-        self.colors = self.configs.colour
-        self.color = self.colors()
         self.black = Blacklist()
+        self.errors = Errors()
         self.repos = Repositories()
 
-        self.bold: str = self.color['bold']
-        self.yellow: str = self.color['yellow']
-        self.cyan: str = self.color['cyan']
-        self.red: str = self.color['red']
-        self.endc: str = self.color['endc']
-        self.bred: str = f'{self.bold}{self.red}'
-
         self.installed_packages: dict = dict(self.all_installed())
 
         logging.basicConfig(filename=LoggingConfig.log_file,
                             filemode='w',
                             encoding='utf-8',
                             level=logging.INFO)
 
@@ -44,18 +36,18 @@
         try:
             return self.installed_packages[name]
         except KeyError:
             return ''
 
     def all_installed(self) -> dict:
         """ Return all installed packages from /val/log/packages folder. """
-        var_log_packages: Path = Path(self.configs.log_packages)
+        var_log_packages: Path = Path(self.log_packages)
 
         try:
-            for file in var_log_packages.glob(self.configs.file_pattern):
+            for file in var_log_packages.glob(self.file_pattern):
                 name = self.split_binary_pkg(file.name)[0]
 
                 if not name.startswith('.') and not self.blacklist_pattern(name):
                     yield name, file.name
 
         except ValueError as err:
             logger = logging.getLogger(__name__)
@@ -93,15 +85,15 @@
         build: str = ''.join(re.findall(r'\d+', build_tag[:2]))
 
         return [name, version, arch, build]
 
     def finished_time(self, elapsed_time: float) -> None:
         """ Printing the elapsed time. """
         print(f'\n{self.yellow}Finished Successfully:{self.endc}',
-              time.strftime(f'[{self.cyan}%H:%M:%S{self.endc}]',
+              time.strftime(f'{self.cyan}%H:%M:%S{self.endc}',
                             time.gmtime(elapsed_time)))
 
     def read_sbo_build_tag(self, sbo: str, location: str) -> str:
         """ Returns build tag from .SlackBuild file. """
         build: str = ''
 
         sbo_script = Path(self.repos.sbo_repo_path, location, sbo, f'{sbo}.SlackBuild')
@@ -135,15 +127,15 @@
                 if package and not package.startswith('#'):
                     if '#' in package:
                         package = package.split('#')[0].strip()
 
                     yield package
 
         except FileNotFoundError:
-            self.raise_error_message(f"No such file or directory: '{file}'")
+            self.errors.raise_error_message(f"No such file or directory: '{file}'")
 
     @staticmethod
     def read_file(file: Union[str, Path]) -> list:
         """ Reads the text file. """
         with open(file, 'r', encoding='utf-8', errors='replace') as f:
             return f.readlines()
 
@@ -154,18 +146,14 @@
             output = subprocess.call(command, shell=True, stderr=stderr, stdout=stdout)
         except (KeyboardInterrupt, subprocess.CalledProcessError) as err:
             raise SystemExit(err)
 
         if output != 0:
             raise SystemExit(output)
 
-    def raise_error_message(self, message: str) -> None:
-        """ A general method to raise an error message and exit. """
-        raise SystemExit(f"\n{self.configs.prog_name}: {self.bred}Error{self.endc}: {message}.\n")
-
     def get_file_size(self, file: Path) -> str:
         """ Get the local file size and converted to units. """
         size = Path(file).stat().st_size
         return self.convert_file_sizes(size)
 
     @staticmethod
     def convert_file_sizes(size: int) -> str:
```

### Comparing `slpkg-4.8.0/slpkg/dependees.py` & `slpkg-4.8.1/slpkg/dependees.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,27 +16,19 @@
         super(Configs, self).__init__()
         self.data: dict = data
         self.packages: list = packages
         self.flags: list = flags
 
         self.ascii = Ascii()
         self.repos = Repositories()
-        self.color = self.colour()
         self.utils = Utilities()
 
         self.llc: str = self.ascii.lower_left_corner
         self.hl: str = self.ascii.horizontal_line
         self.var: str = self.ascii.vertical_and_right
-        self.bold: str = self.color['bold']
-        self.violet: str = self.color['violet']
-        self.cyan: str = self.color['cyan']
-        self.grey: str = self.color['grey']
-        self.yellow: str = self.color['yellow']
-        self.byellow: str = f'{self.bold}{self.yellow}'
-        self.endc: str = self.color['endc']
 
         self.option_for_full_reverse: bool = self.utils.is_option(
             ['-E', '--full-reverse'], self.flags)
 
         self.option_for_pkg_version: bool = self.utils.is_option(
             ['-p', '--pkg-version'], self.flags)
```

### Comparing `slpkg-4.8.0/slpkg/remove_packages.py` & `slpkg-4.8.1/slpkg/remove_packages.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,31 +19,23 @@
     def __init__(self, packages: list, flags: list):
         __slots__ = 'packages', 'flags'
         super(Configs, self).__init__()
         self.packages: list = packages
         self.flags: list = flags
 
         self.session = Session
-        self.color = self.colour()
         self.utils = Utilities()
         self.progress = ProgressBar()
         self.view = ViewMessage(self.flags)
 
-        self.output: int = 0
+        self.process_message: str = ''
         self.installed_packages: list = []
         self.dependencies: list = []
         self.stderr = None
         self.stdout = None
-        self.bold: str = self.color['bold']
-        self.cyan: str = self.color['cyan']
-        self.yellow: str = self.color['yellow']
-        self.red: str = self.color['red']
-        self.endc: str = self.color['endc']
-        self.byellow: str = f'{self.bold}{self.yellow}'
-        self.bred: str = f'{self.bold}{self.red}'
 
         self.option_resolve_off: bool = self.utils.is_option(
             ['-o', '--resolve-off'], self.flags)
 
         self.option_for_no_silent: bool = self.utils.is_option(
             ['-n', '--no-silent'], self.flags)
 
@@ -68,29 +60,30 @@
 
         self.utils.finished_time(elapsed_time)
 
     def remove_packages(self) -> None:
         """ Run Slackware command to remove the packages. """
         for package in self.installed_packages:
             name: str = self.utils.split_binary_pkg(package)[0]
+            self.process_message: str = f"package '{name}' to remove"
 
             if self.check_in_logs_for_dependencies_to_remove(name):
                 command: str = f'{self.removepkg} {package}'
                 self.multi_process(command, package)
 
     def check_in_logs_for_dependencies_to_remove(self, name: str) -> bool:
         dependencies: list = []
         logs: dict = self.query_dependencies()
 
         for package, requires in logs.items():
             if name in requires:
                 dependencies.append(package)
 
         if dependencies and not self.option_for_yes and self.ask_question:
-            print(f"\n[{self.bred}WARNING!{self.endc}] The package '{self.red}{name}{self.endc}' "
+            print(f"\n{self.bold}{self.violet}WARNING!{self.endc}: The package '{self.red}{name}{self.endc}' "
                   f"is a dependency for the packages:")
 
             for dep in dependencies:
                 print(f"{self.cyan:>16}-> {dep}{self.endc}")
 
             answer: str = input('\nDo you want to remove? [y/N] ')
 
@@ -128,34 +121,33 @@
         self.session.commit()
 
     def multi_process(self, command: str, package: str) -> None:
         """ Starting multiprocessing remove process. """
         if self.silent_mode and not self.option_for_no_silent:
 
             done: str = f' {self.byellow} Done{self.endc}'
-            message: str = f'{self.red}Remove{self.endc}'
+            message: str = f'{self.bold}{self.red}Remove{self.endc}'
             self.stderr = subprocess.DEVNULL
             self.stdout = subprocess.DEVNULL
 
             # Starting multiprocessing
             p1 = Process(target=self.utils.process, args=(command, self.stderr, self.stdout))
-            p2 = Process(target=self.progress.bar, args=(f'[{message}]', package))
+            p2 = Process(target=self.progress.bar, args=(f'{message}:', package))
 
             p1.start()
             p2.start()
 
             # Wait until process 1 finish
             p1.join()
 
             # Terminate process 2 if process 1 finished
             if not p1.is_alive():
 
                 if p1.exitcode != 0:
-                    done: str = f' {self.bred} Failed{self.endc}'
-                    self.output: int = p1.exitcode  # type: ignore
+                    done: str = f'{self.bred}Failed: {self.endc}{self.process_message}'
 
                 print(f'{self.endc}{done}', end='')
                 p2.terminate()
 
             # Wait until process 2 finish
             p2.join()
```

### Comparing `slpkg-4.8.0/slpkg/blacklist.py` & `slpkg-4.8.1/slpkg/blacklist.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,31 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 import tomli
 from pathlib import Path
 
 from slpkg.configs import Configs
+from slpkg.toml_error_message import TomlErrors
 from slpkg.models.models import session as Session
 
 
 class Blacklist(Configs):
     """ Reads and returns the blacklist. """
 
     def __init__(self):
         super(Configs, self).__init__()
         self.session = Session
 
-        self.color = self.colour()
-        self.bold: str = self.color['bold']
-        self.red: str = self.color['red']
-        self.cyan: str = self.color['cyan']
-        self.endc: str = self.color['endc']
-        self.bred: str = f'{self.bold}{self.red}'
+        self.errors = TomlErrors()
         self.blacklist_file_toml = Path(self.etc_path, 'blacklist.toml')
 
     def packages(self) -> list:
         """ Reads the blacklist file. """
         if self.blacklist_file_toml.is_file():
             try:
                 with open(self.blacklist_file_toml, 'rb') as black:
                     return tomli.load(black)['BLACKLIST']['PACKAGES']
             except (tomli.TOMLDecodeError, KeyError) as error:
-                raise SystemExit(f"\n{self.prog_name} {self.bred}Error{self.endc}: {error}: in the configuration file "
-                                 f"'{self.blacklist_file_toml}'.\n"
-                                 f"\nIf you have upgraded the '{self.prog_name}' probably you need to run:\n"
-                                 f"'mv {self.blacklist_file_toml}.new {self.blacklist_file_toml}'.\n"
-                                 f"or '{self.cyan}slpkg_new-configs{self.endc}' command.\n")
+                self.errors.raise_toml_error_message(error, self.blacklist_file_toml)
+
         return []
```

### Comparing `slpkg-4.8.0/slpkg/download_only.py` & `slpkg-4.8.1/slpkg/download_only.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.0/slpkg/tracking.py` & `slpkg-4.8.1/slpkg/tracking.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,24 +11,19 @@
 
     def __init__(self, flags: list):
         __slots__ = 'flags'
         super(Configs, self).__init__()
         self.flags: list = flags
 
         self.ascii = Ascii()
-        self.color = self.colour()
         self.utils = Utilities()
 
         self.llc: str = self.ascii.lower_left_corner
         self.hl: str = self.ascii.horizontal_line
         self.vl: str = self.ascii.vertical_line
-        self.cyan: str = self.color['cyan']
-        self.grey: str = self.color['grey']
-        self.yellow: str = self.color['yellow']
-        self.endc: str = self.color['endc']
 
         self.option_for_pkg_version: bool = self.utils.is_option(
             ['-p', '--pkg-version'], self.flags)
 
         self.option_for_binaries: bool = self.utils.is_option(
             ['-B', '--bin-repo='], self.flags)
```

### Comparing `slpkg-4.8.0/slpkg/main.py` & `slpkg-4.8.1/slpkg/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,26 +38,22 @@
 class Argparse(Configs):
 
     def __init__(self, args: list):
         __slots__ = 'args'
         super(Configs).__init__()
         self.args: list = args
         self.flags: list = []
+
         self.directory = self.tmp_slpkg
         self.dialogbox = DialogBox()
         self.utils = Utilities()
         self.usage = Usage()
         self.form_configs = FormConfigs()
-        self.color = self.colour()
         self.repos = Repositories()
 
-        self.bold: str = self.color['bold']
-        self.red: str = self.color['red']
-        self.endc: str = self.color['endc']
-        self.bred: str = f'{self.bold}{self.red}'
         self.binary_repo: str = ''
 
         if len(self.args) == 0 or '' in self.args:
             self.usage.help_short(1)
 
         self.data: dict = {}
         self.flag_yes: str = '--yes'
@@ -302,21 +298,22 @@
 
             except_options: list = [
                 '-s', 'search',
                 '-u', 'update',
                 '-c', 'check-updates',
             ]
 
-            if self.binary_repo in self.repos.bin_repos_names and self.binary_repo not in self.repos.bin_enabled_repos:
+            if (self.binary_repo in list(self.repos.repositories.keys())[2:]
+                    and not self.repos.repositories[self.binary_repo][0]):
                 self.usage.help_minimal(f"{self.prog_name}: repository '{self.binary_repo}' is disabled")
 
             elif self.binary_repo == '*' and not self.utils.is_option(except_options, self.args):
                 self.usage.help_minimal(f"{self.prog_name}: invalid binary repository '{self.binary_repo}'")
 
-            elif self.binary_repo not in self.repos.bin_repos_names and self.binary_repo != '*':
+            elif self.binary_repo not in list(self.repos.repositories.keys())[2:] and self.binary_repo != '*':
                 self.usage.help_minimal(f"{self.prog_name}: invalid binary repository '{self.binary_repo}'")
 
     def invalid_options(self) -> None:
         """ Checks for invalid options. """
         invalid, commands, repeat = [], [], []
 
         for arg in self.args:
@@ -520,15 +517,15 @@
             raise SystemExit()
         self.usage.help_short(1)
 
     def upgrade(self) -> None:
         command = Argparse.upgrade.__name__
 
         if len(self.args) == 1:
-            self.check.is_empty_database()
+            self.check.is_empty_database(self.binary_repo)
 
             upgrade = Upgrade(self.flags, self.data)
             packages: list = list(upgrade.packages())
 
             packages: list = self.choose_packages(packages, command)
 
             if not packages:
@@ -562,25 +559,25 @@
         if len(self.args) == 1:
             self.form_configs.edit()
             raise SystemExit()
         self.usage.help_short(1)
 
     def clean_logs(self) -> None:
         if len(self.args) == 1:
-            self.check.is_empty_database()
+            self.check.is_empty_database(self.binary_repo)
 
             logs = CleanLogsDependencies(self.flags)
             logs.clean()
             raise SystemExit()
         self.usage.help_short(1)
 
     def clean_tmp(self) -> None:
         if len(self.args) == 1:
 
-            print(f"\n{self.prog_name}: {self.bred}WARNING{self.endc}: All the files in the "
+            print(f"\n{self.prog_name}: {self.blink}{self.bold}{self.bred}WARNING!{self.endc}: All the files in the "
                   f"'{self.tmp_path}{self.prog_name}' "
                   f"folder will delete!")
 
             views = ViewMessage(self.flags)
             views.question()
 
             self.utils.remove_folder_if_exists(Path(self.tmp_path, self.prog_name))
@@ -598,15 +595,15 @@
         self.usage.help_short(1)
 
     def build(self) -> None:
         command = Argparse.build.__name__
 
         if len(self.args) >= 2:
 
-            self.check.is_empty_database()
+            self.check.is_empty_database(self.binary_repo)
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose_packages(packages, command)
 
             self.check.exists_in_the_database(packages)
             self.check.is_package_unsupported(packages)
@@ -617,15 +614,15 @@
         self.usage.help_short(1)
 
     def install(self) -> None:
         command = Argparse.install.__name__
 
         if len(self.args) >= 2:
 
-            self.check.is_empty_database()
+            self.check.is_empty_database(self.binary_repo)
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose_packages(packages, command)
 
             if self.utils.is_option(self.flag_binaries, self.flags):
                 self.check.exists_in_the_database(packages)
@@ -642,15 +639,15 @@
         self.usage.help_short(1)
 
     def download(self) -> None:
         command = Argparse.download.__name__
 
         if len(self.args) >= 2:
 
-            self.check.is_empty_database()
+            self.check.is_empty_database(self.binary_repo)
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose_packages(packages, command)
 
             self.check.exists_in_the_database(packages)
             download = Download(self.directory, self.flags)
@@ -676,15 +673,15 @@
         self.usage.help_short(1)
 
     def find(self) -> None:
         command = Argparse.find.__name__
 
         if len(self.args) >= 2:
 
-            self.check.is_empty_database()
+            self.check.is_empty_database(self.binary_repo)
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose_packages(packages, command)
 
             find = FindInstalled()
             find.find(packages)
@@ -692,15 +689,15 @@
         self.usage.help_short(1)
 
     def view(self) -> None:
         command = Argparse.view.__name__
 
         if len(self.args) >= 2:
 
-            self.check.is_empty_database()
+            self.check.is_empty_database(self.binary_repo)
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose_packages(packages, command)
 
             self.check.exists_in_the_database(packages)
 
@@ -714,15 +711,15 @@
         self.usage.help_short(1)
 
     def search(self) -> None:
         command = Argparse.search.__name__
 
         if len(self.args) >= 2:
 
-            self.check.is_empty_database()
+            self.check.is_empty_database(self.binary_repo)
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose_packages(packages, command)
 
             search = SearchPackage(self.flags)
             search.package(self.data, packages, self.binary_repo)
@@ -730,15 +727,15 @@
         self.usage.help_short(1)
 
     def dependees(self) -> None:
         command = Argparse.dependees.__name__
 
         if len(self.args) >= 2:
 
-            self.check.is_empty_database()
+            self.check.is_empty_database(self.binary_repo)
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose_packages(packages, command)
 
             self.check.exists_in_the_database(packages)
 
@@ -748,15 +745,15 @@
         self.usage.help_short(1)
 
     def tracking(self) -> None:
         command = Argparse.tracking.__name__
 
         if len(self.args) >= 2:
 
-            self.check.is_empty_database()
+            self.check.is_empty_database(self.binary_repo)
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose_packages(packages, command)
 
             self.check.exists_in_the_database(packages)
```

### Comparing `slpkg-4.8.0/slpkg/upgrade.py` & `slpkg-4.8.1/slpkg/upgrade.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.0/slpkg/search.py` & `slpkg-4.8.1/slpkg/search.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,24 +11,17 @@
     """ Search packages from the repositories. """
 
     def __init__(self, flags=None):
         __slots__ = 'flags'
         super(Configs, self).__init__()
         self.flags: list = flags
 
-        self.color = self.colour()
         self.utils = Utilities()
         self.repos = Repositories()
 
-        self.yellow: str = self.color['yellow']
-        self.cyan: str = self.color['cyan']
-        self.green: str = self.color['green']
-        self.grey: str = self.color['grey']
-        self.endc: str = self.color['endc']
-
         self.option_for_binaries: bool = self.utils.is_option(
             ['-B', '--bin-repo='], self.flags)
 
     def package(self, data: dict, packages: list, repo: str) -> None:
         """ Searching and print the matched packages. """
         print(f'The list below shows the repo '
               f'packages that contains \'{", ".join([p for p in packages])}\':\n')
```

### Comparing `slpkg-4.8.0/setup.cfg` & `slpkg-4.8.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = slpkg
-version = 4.8.0
+version = 4.8.1
 license_file = LICENSE
 author = Dimitris Zlatanidis
 author_email = d.zlatanidis@gmail.com
 description = Package manager utility for Slackware Linux.
 long_description = file:README.rst
 url = https://dslackw.gitlab.io/slpkg/
 project_urls =
```

### Comparing `slpkg-4.8.0/slpkg.egg-info/SOURCES.txt` & `slpkg-4.8.1/slpkg.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -10,23 +10,25 @@
 slpkg/clean_logs.py
 slpkg/configs.py
 slpkg/dependees.py
 slpkg/dialog_box.py
 slpkg/dialog_configs.py
 slpkg/download_only.py
 slpkg/downloader.py
+slpkg/error_messages.py
 slpkg/find_installed.py
 slpkg/install_data.py
 slpkg/logging_config.py
 slpkg/main.py
 slpkg/progress_bar.py
 slpkg/remove_packages.py
 slpkg/repo_info.py
 slpkg/repositories.py
 slpkg/search.py
+slpkg/toml_error_message.py
 slpkg/tracking.py
 slpkg/update_repository.py
 slpkg/upgrade.py
 slpkg/utilities.py
 slpkg.egg-info/PKG-INFO
 slpkg.egg-info/SOURCES.txt
 slpkg.egg-info/dependency_links.txt
```

### Comparing `slpkg-4.8.0/slpkg.egg-info/PKG-INFO` & `slpkg-4.8.1/slpkg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slpkg
-Version: 4.8.0
+Version: 4.8.1
 Summary: Package manager utility for Slackware Linux.
 Home-page: https://dslackw.gitlab.io/slpkg/
 Author: Dimitris Zlatanidis
 Author-email: d.zlatanidis@gmail.com
 License: UNKNOWN
 Project-URL: Source, https://dslackw.gitlab.io/slpkg/
 Project-URL: Documentation, https://dslackw.gitlab.io/slpkg/
```

### Comparing `slpkg-4.8.0/README.md` & `slpkg-4.8.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,43 +29,43 @@
 It also uses the Slackware Linux instructions for installing, upgrading or removing packages.
 
 ### Screenshots
 
 ```
 $ slpkg repo-info
 ```
-<img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_repo_info.png" width="700">
+<img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_repo_info.png" width="900">
 
 ```
 $ slpkg install audacity --bin-repo=alien
 ```
-<img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_install.png" width="700">
-<img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_install_done.png" width="700">
+<img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_install.png" width="900">
+<img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_install_done.png" width="900">
 
 ```
 $ slpkg remove audacity
 ```
-<img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_remove.png" width="700">
-<img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_remove_done.png" width="700">
+<img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_remove.png" width="900">
+<img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_remove_done.png" width="900">
 
 ```
 $ slpkg dependees --pkg-version --full-reverse greenlet
 ```
-<img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_dependees.png" width="700">
+<img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_dependees.png" width="900">
 
 ```
-$ slpkg tracking --pkg-version slpkg Flask awscli
+$ slpkg tracking --pkg-version Flask awscli pychess
 ```
-<img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_tracking.png" width="700">
+<img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_tracking.png" width="900">
 
 ### Installation
 
 ```
-$ tar xvf slpkg-4.8.0.tar.gz
-$ cd slpkg-4.8.0
+$ tar xvf slpkg-4.8.1.tar.gz
+$ cd slpkg-4.8.1
 $ ./install.sh
 ```
 
 ### Requirements
 
 ```
 SQLAlchemy >= 1.4.46
@@ -82,15 +82,15 @@
 
 The majority of trials have been made in Slackware x86_64 'stable' environment.
 
 
 ### Command Line Tool Usage
 
 ```
-USAGE: slpkg [OPTIONS] [COMMAND] [FILELIST|PACKAGES...]
+USAGE: slpkg [COMMAND] [OPTIONS] [FILELIST|PACKAGES...]
 
 DESCRIPTION: Package manager utility for Slackware.
 
 COMMANDS:
   -u, update                    Update the package lists.
   -U, upgrade                   Upgrade all the packages.
   -c, check-updates             Check for news on ChangeLog.txt.
@@ -102,28 +102,29 @@
   -b, build [packages...]       Build only the packages.
   -i, install [packages...]     Build and install the packages.
   -d, download [packages...]    Download only the scripts and sources.
   -R, remove [packages...]      Remove installed packages.
   -f, find [packages...]        Find installed packages.
   -w, view [packages...]        View packages from the repository.
   -s, search [packages...]      Search packages from the repository.
-  -e, dependees [packages...]   Show which packages depend.
+  -e, dependees [packages...]   Show which packages depend on.
   -t, tracking [packages...]    Tracking the packages dependencies.
 
 OPTIONS:
   -y, --yes                     Answer Yes to all questions.
   -j, --jobs                    Set it for multicore systems.
   -o, --resolve-off             Turns off dependency resolving.
   -r, --reinstall               Upgrade packages of the same version.
   -k, --skip-installed          Skip installed packages.
   -E, --full-reverse            Full reverse dependency.
   -S, --search                  Search packages from the repository.
   -n, --no-silent               Disable silent mode.
   -p, --pkg-version             Print the repository package version.
   -G, --generate-only           Generates only the SLACKBUILDS.TXT file.
+  -P, --parallel                Download files in parallel.
   -B, --bin-repo=[REPO]         Set a binary repository.
   -z, --directory=[PATH]        Download files to a specific path.
 
   -h, --help                    Show this message and exit.
   -v, --version                 Print version and exit.
 ```
```

### Comparing `slpkg-4.8.0/tools/gen_sbo_txt.sh` & `slpkg-4.8.1/tools/gen_sbo_txt.sh`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.0/bin/slpkg_new-configs` & `slpkg-4.8.1/bin/slpkg_new-configs`

 * *Files 7% similar despite different names*

```diff
@@ -7,60 +7,55 @@
 import subprocess
 from pathlib import Path
 
 
 class NewConfig:
 
     def __init__(self, flags: list):
+        __slots__ = 'flags'
         self.flags: list = flags
         self.etc_path: str = '/etc/slpkg'
-        self.slpkg_config = Path(self.etc_path, 'slpkg.toml')
-        self.repositories_config = Path(self.etc_path, 'repositories.toml')
-        self.blacklist_config = Path(self.etc_path, 'blacklist.toml')
-        self.slpkg_config_new = Path(self.etc_path, 'slpkg.toml.new')
-        self.repositories_config_new = Path(self.etc_path, 'repositories.toml.new')
-        self.blacklist_config_new = Path(self.etc_path, 'blacklist.toml.new')
-
-        self.color: dict = {}
-        self.colors()
-
-        self.bold: str = self.color['bold']
-        self.red: str = self.color['red']
-        self.green: str = self.color['green']
-        self.yellow: str = self.color['yellow']
-        self.bgreen: str = f'{self.color["bold"]}{self.color["green"]}'
-        self.byellow: str = f'{self.color["bold"]}{self.color["yellow"]}'
-        self.endc: str = self.color['endc']
+        self.slpkg_config: Path = Path(self.etc_path, 'slpkg.toml')
+        self.repositories_config: Path = Path(self.etc_path, 'repositories.toml')
+        self.blacklist_config: Path = Path(self.etc_path, 'blacklist.toml')
+        self.slpkg_config_new: Path = Path(self.etc_path, 'slpkg.toml.new')
+        self.repositories_config_new: Path = Path(self.etc_path, 'repositories.toml.new')
+        self.blacklist_config_new: Path = Path(self.etc_path, 'blacklist.toml.new')
+
+        self.bold: str = '\033[1m'
+        self.red: str = '\x1b[91m'
+        self.bred: str = f'{self.bold}{self.red}'
+        self.green: str = '\x1b[32m'
+        self.bgreen: str = f'{self.bold}{self.green}'
+        self.yellow: str = '\x1b[93m'
+        self.byellow: str = f'{self.bold}{self.yellow}'
+        self.cyan: str = '\x1b[96m'
+        self.blue: str = '\x1b[94m'
+        self.grey: str = '\x1b[38;5;247m'
+        self.violet: str = '\x1b[35m'
+        self.endc: str = '\x1b[0m'
+
+        self.set_no_colors()
+
         self.choice = None
 
-    def colors(self):
+    def set_no_colors(self):
         if '--no-colors' in self.flags:
-            self.color = {
-                'bold': '',
-                'red': '',
-                'green': '',
-                'yellow': '',
-                'cyan': '',
-                'blue': '',
-                'grey': '',
-                'violet': '',
-                'endc': ''
-            }
-        else:
-            self.color = {
-                'bold': '\033[1m',
-                'red': '\x1b[91m',
-                'green': '\x1b[32m',
-                'yellow': '\x1b[93m',
-                'cyan': '\x1b[96m',
-                'blue': '\x1b[94m',
-                'grey': '\x1b[38;5;247m',
-                'violet': '\x1b[35m',
-                'endc': '\x1b[0m'
-            }
+            self.bold: str = ''
+            self.red: str = ''
+            self.bred: str = ''
+            self.green: str = ''
+            self.bgreen: str = ''
+            self.yellow: str = ''
+            self.byellow: str = ''
+            self.cyan: str = ''
+            self.blue: str = ''
+            self.grey: str = ''
+            self.violet: str = ''
+            self.endc: str = ''
 
     def check(self):
         """ Checks for .new files. """
         print('Checking for NEW configuration files...')
         if (self.slpkg_config_new.is_file() or self.blacklist_config_new.is_file()
                 or self.repositories_config_new.is_file()):
             print('\nThere are NEW files:\n')
```

