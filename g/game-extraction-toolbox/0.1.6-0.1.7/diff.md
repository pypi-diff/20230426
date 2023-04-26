# Comparing `tmp/game-extraction-toolbox-0.1.6.tar.gz` & `tmp/game-extraction-toolbox-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "game-extraction-toolbox-0.1.6.tar", last modified: Mon Mar 27 20:28:25 2023, max compression
+gzip compressed data, was "game-extraction-toolbox-0.1.7.tar", last modified: Wed Apr 26 07:01:16 2023, max compression
```

## Comparing `game-extraction-toolbox-0.1.6.tar` & `game-extraction-toolbox-0.1.7.tar`

### file list

```diff
@@ -1,196 +1,205 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.736860 game-extraction-toolbox-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-03-27 20:28:25.736860 game-extraction-toolbox-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11855 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-27 20:28:25.736860 game-extraction-toolbox-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.716860 game-extraction-toolbox-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.724860 game-extraction-toolbox-0.1.6/src/game_extraction_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-03-27 20:28:25.000000 game-extraction-toolbox-0.1.6/src/game_extraction_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-03-27 20:28:25.000000 game-extraction-toolbox-0.1.6/src/game_extraction_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 20:28:25.000000 game-extraction-toolbox-0.1.6/src/game_extraction_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-27 20:28:25.000000 game-extraction-toolbox-0.1.6/src/game_extraction_toolbox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-27 20:28:25.000000 game-extraction-toolbox-0.1.6/src/game_extraction_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-27 20:28:25.000000 game-extraction-toolbox-0.1.6/src/game_extraction_toolbox.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.724860 game-extraction-toolbox-0.1.6/src/gex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.724860 game-extraction-toolbox-0.1.6/src/gex/commands/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.724860 game-extraction-toolbox-0.1.6/src/gex/commands/archive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/commands/archive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.724860 game-extraction-toolbox-0.1.6/src/gex/commands/archive/arc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/commands/archive/arc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/commands/archive/arc/arc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/commands/archive/arc/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/commands/archive/archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.724860 game-extraction-toolbox-0.1.6/src/gex/commands/archive/kpka/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/commands/archive/kpka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/commands/archive/kpka/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/commands/archive/kpka/kpka.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.724860 game-extraction-toolbox-0.1.6/src/gex/commands/archive/zip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/commands/archive/zip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/commands/archive/zip/list.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/commands/archive/zip/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.724860 game-extraction-toolbox-0.1.6/src/gex/commands/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/commands/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/commands/file/deinterleave.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/commands/file/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/commands/file/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/commands/file/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/commands/file/identify.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/commands/file/slice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.724860 game-extraction-toolbox-0.1.6/src/gex/commands/finder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/commands/finder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/commands/finder/bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/commands/finder/finder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.724860 game-extraction-toolbox-0.1.6/src/gex/commands/postprocess/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/commands/postprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/commands/postprocess/postprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.724860 game-extraction-toolbox-0.1.6/src/gex/commands/postprocess/wii/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/commands/postprocess/wii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/commands/postprocess/wii/cleanrip.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/commands/postprocess/wii/wii.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.724860 game-extraction-toolbox-0.1.6/src/gex/commands/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/commands/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/commands/tasks/details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/commands/tasks/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/commands/tasks/list.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/commands/tasks/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/commands/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.720860 game-extraction-toolbox-0.1.6/src/gex/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.728860 game-extraction-toolbox-0.1.6/src/gex/lib/archive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/archive/arc.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/archive/bplist-mbundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/archive/kpka.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/archive/kvq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/archive/prs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/archive/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.728860 game-extraction-toolbox-0.1.6/src/gex/lib/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)    12938 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/contrib/bputil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.728860 game-extraction-toolbox-0.1.6/src/gex/lib/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/file/identify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.728860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/basetask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/copytask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.728860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.728860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/acac/
--rw-r--r--   0 runner    (1001) docker     (123)    35609 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/acac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25912 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/acac/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.728860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ags_digdug/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ags_digdug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ags_digdug/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.728860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ags_galaga/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ags_galaga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ags_galaga/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.728860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ags_mspacman/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ags_mspacman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ags_mspacman/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.728860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ags_pacman/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ags_pacman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ags_pacman/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.728860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/atarivault/
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/atarivault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/atarivault/arcade.py
--rw-r--r--   0 runner    (1001) docker     (123)   150649 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/atarivault/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.728860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/blizzarcade/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/blizzarcade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9799 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/blizzarcade/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.728860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/bubsy/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/bubsy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/bubsy/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.728860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/cas1/
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/cas1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.728860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/cas1_old/
--rw-r--r--   0 runner    (1001) docker     (123)    52289 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/cas1_old/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.728860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/cas2/
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/cas2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.728860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/cbeub/
--rw-r--r--   0 runner    (1001) docker     (123)    29929 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/cbeub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34368 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/cbeub/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.728860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/cfc/
--rw-r--r--   0 runner    (1001) docker     (123)    24350 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/cfc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32087 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/cfc/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.732860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ddragontrilogy/
--rw-r--r--   0 runner    (1001) docker     (123)    10041 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ddragontrilogy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ddragontrilogy/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.732860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/disneyac/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/disneyac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/disneyac/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.732860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/disneyalkb/
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/disneyalkb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/disneyalkb/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.732860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/genesis/
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/genesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54777 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/genesis/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.732860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/irem/
--rw-r--r--   0 runner    (1001) docker     (123)    35862 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/irem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42043 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/irem/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.732860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/mkak/
--rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/mkak/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.732860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/mmlc1/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/mmlc1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/mmlc1/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.732860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/mmxlc1/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/mmxlc1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/mmxlc1/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.732860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/neogeo_classics_humble/
--rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/neogeo_classics_humble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47979 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/neogeo_classics_humble/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.732860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/pacmanmplus/
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/pacmanmplus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19572 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/pacmanmplus/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.732860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/psikyo/
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/psikyo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.732860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/sadxgg/
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/sadxgg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11263 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/sadxgg/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.732860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/saga/
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/saga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/saga/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.732860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/sf30ac/
--rw-r--r--   0 runner    (1001) docker     (123)    49789 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/sf30ac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64915 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/sf30ac/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.736860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/snk40/
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/snk40/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/snk40/arcadedlc.py
--rw-r--r--   0 runner    (1001) docker     (123)    40772 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/snk40/arcademain.py
--rw-r--r--   0 runner    (1001) docker     (123)    20387 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/snk40/arcadepatch.py
--rw-r--r--   0 runner    (1001) docker     (123)   108367 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/snk40/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/snk40/nes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/snk40/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.736860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/spp_columnsiii/
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/spp_columnsiii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/spp_columnsiii/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.736860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/spp_drmbm/
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/spp_drmbm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/spp_drmbm/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.736860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ssp1/
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ssp1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ssp1/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.736860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ssp2/
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ssp2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ssp2/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.736860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/wonderboy3/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/wonderboy3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/wonderboy3/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.736860 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/zamn/
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/zamn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/zamn/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/splicetask.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/task_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/tasks/zipsplicetask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.736860 game-extraction-toolbox-0.1.6/src/gex/lib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.736860 game-extraction-toolbox-0.1.6/src/gex/lib/utils/blob/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/utils/blob/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/utils/blob/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/utils/gfx_rebuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/utils/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:25.736860 game-extraction-toolbox-0.1.6/src/gex/lib/utils/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/utils/vendor/capcom.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/utils/vendor/snk.py
--rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/lib/utils/verify.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-03-27 20:28:12.000000 game-extraction-toolbox-0.1.6/src/gex/toolbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.753595 game-extraction-toolbox-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-04-26 07:01:16.753595 game-extraction-toolbox-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12118 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-26 07:01:16.753595 game-extraction-toolbox-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.729595 game-extraction-toolbox-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.737595 game-extraction-toolbox-0.1.7/src/game_extraction_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-04-26 07:01:16.000000 game-extraction-toolbox-0.1.7/src/game_extraction_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-04-26 07:01:16.000000 game-extraction-toolbox-0.1.7/src/game_extraction_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 07:01:16.000000 game-extraction-toolbox-0.1.7/src/game_extraction_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-26 07:01:16.000000 game-extraction-toolbox-0.1.7/src/game_extraction_toolbox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-26 07:01:16.000000 game-extraction-toolbox-0.1.7/src/game_extraction_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-26 07:01:16.000000 game-extraction-toolbox-0.1.7/src/game_extraction_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.737595 game-extraction-toolbox-0.1.7/src/gex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.737595 game-extraction-toolbox-0.1.7/src/gex/commands/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.737595 game-extraction-toolbox-0.1.7/src/gex/commands/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/commands/archive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.737595 game-extraction-toolbox-0.1.7/src/gex/commands/archive/arc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/commands/archive/arc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/commands/archive/arc/arc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/commands/archive/arc/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/commands/archive/archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.737595 game-extraction-toolbox-0.1.7/src/gex/commands/archive/kpka/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/commands/archive/kpka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/commands/archive/kpka/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/commands/archive/kpka/kpka.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.737595 game-extraction-toolbox-0.1.7/src/gex/commands/archive/zip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/commands/archive/zip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/commands/archive/zip/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/commands/archive/zip/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.737595 game-extraction-toolbox-0.1.7/src/gex/commands/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/commands/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/commands/file/deinterleave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/commands/file/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/commands/file/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/commands/file/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/commands/file/identify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/commands/file/slice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.737595 game-extraction-toolbox-0.1.7/src/gex/commands/finder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/commands/finder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/commands/finder/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/commands/finder/finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.737595 game-extraction-toolbox-0.1.7/src/gex/commands/postprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/commands/postprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/commands/postprocess/postprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.737595 game-extraction-toolbox-0.1.7/src/gex/commands/postprocess/wii/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/commands/postprocess/wii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/commands/postprocess/wii/cleanrip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/commands/postprocess/wii/wii.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.741595 game-extraction-toolbox-0.1.7/src/gex/commands/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/commands/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/commands/tasks/details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/commands/tasks/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/commands/tasks/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/commands/tasks/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/commands/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.733595 game-extraction-toolbox-0.1.7/src/gex/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.741595 game-extraction-toolbox-0.1.7/src/gex/lib/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/archive/arc.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/archive/bplist-mbundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/archive/kpka.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/archive/kvq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/archive/prs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/archive/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.741595 game-extraction-toolbox-0.1.7/src/gex/lib/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)    12938 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/contrib/bputil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.741595 game-extraction-toolbox-0.1.7/src/gex/lib/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/file/identify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.741595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/basetask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/copytask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.741595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.741595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/acac/
+-rw-r--r--   0 runner    (1001) docker     (123)    37401 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/acac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31163 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/acac/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.741595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ags_digdug/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ags_digdug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ags_digdug/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.741595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ags_galaga/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ags_galaga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ags_galaga/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.741595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ags_mspacman/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ags_mspacman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ags_mspacman/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.741595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ags_pacman/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ags_pacman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ags_pacman/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.741595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/atarivault/
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/atarivault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/atarivault/arcade.py
+-rw-r--r--   0 runner    (1001) docker     (123)   150649 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/atarivault/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.741595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/blizzarcade/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/blizzarcade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9799 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/blizzarcade/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.741595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/breakers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/breakers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/breakers/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.745595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/bubsy/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/bubsy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/bubsy/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.745595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/cas1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/cas1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.745595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/cas1_old/
+-rw-r--r--   0 runner    (1001) docker     (123)    52289 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/cas1_old/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.745595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/cas2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/cas2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.745595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/cbeub/
+-rw-r--r--   0 runner    (1001) docker     (123)    29929 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/cbeub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34368 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/cbeub/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.745595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/cfc/
+-rw-r--r--   0 runner    (1001) docker     (123)    24350 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/cfc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32087 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/cfc/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.745595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ddragontrilogy/
+-rw-r--r--   0 runner    (1001) docker     (123)    10041 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ddragontrilogy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ddragontrilogy/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.745595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/disneyac/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/disneyac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/disneyac/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.745595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/disneyalkb/
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/disneyalkb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/disneyalkb/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.745595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/genesis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/genesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54777 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/genesis/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.745595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/irem/
+-rw-r--r--   0 runner    (1001) docker     (123)    36353 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/irem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42043 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/irem/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.745595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/mkak/
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/mkak/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.745595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/mmbnlc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/mmbnlc1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/mmbnlc1/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.745595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/mmbnlc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/mmbnlc2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7018 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/mmbnlc2/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.745595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/mmlc1/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/mmlc1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/mmlc1/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.745595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/mmxlc1/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/mmxlc1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/mmxlc1/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.745595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/neogeo_classics_humble/
+-rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/neogeo_classics_humble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47979 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/neogeo_classics_humble/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.745595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/pacmanmplus/
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/pacmanmplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19572 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/pacmanmplus/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.745595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/psikyo/
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/psikyo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.749595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/sadxgg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/sadxgg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11263 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/sadxgg/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.749595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/saga/
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/saga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/saga/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.749595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/sf30ac/
+-rw-r--r--   0 runner    (1001) docker     (123)    49789 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/sf30ac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64915 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/sf30ac/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.749595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/snk40/
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/snk40/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/snk40/arcadedlc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40772 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/snk40/arcademain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20387 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/snk40/arcadepatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)   108367 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/snk40/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/snk40/nes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/snk40/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.749595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/spp_columnsiii/
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/spp_columnsiii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/spp_columnsiii/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.749595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/spp_drmbm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/spp_drmbm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/spp_drmbm/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.749595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ssp1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ssp1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ssp1/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.749595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ssp2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ssp2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ssp2/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.749595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/wonderboy3/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/wonderboy3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/wonderboy3/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.749595 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/zamn/
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/zamn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/zamn/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/splicetask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/task_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/tasks/zipsplicetask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.749595 game-extraction-toolbox-0.1.7/src/gex/lib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.749595 game-extraction-toolbox-0.1.7/src/gex/lib/utils/blob/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/utils/blob/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/utils/blob/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/utils/gfx_rebuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/utils/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:01:16.753595 game-extraction-toolbox-0.1.7/src/gex/lib/utils/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/utils/vendor/capcom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/utils/vendor/snk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/lib/utils/verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-26 07:01:05.000000 game-extraction-toolbox-0.1.7/src/gex/toolbox.py
```

### Comparing `game-extraction-toolbox-0.1.6/LICENSE` & `game-extraction-toolbox-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/PKG-INFO` & `game-extraction-toolbox-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: game-extraction-toolbox
-Version: 0.1.6
+Version: 0.1.7
 Summary: CLI Tools for investigating game files and extracting known packages
 Author-email: Shawn McNaughton <shawngmc@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Shawn McNaughton
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,37 +23,37 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/shawngmc/game-extraction-toolbox
 Project-URL: Bug Tracker, https://github.com/shawngmc/game-extraction-toolbox/issues
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI version](https://badge.fury.io/py/game-extraction-toolbox.svg)](https://badge.fury.io/py/game-extraction-toolbox)
 
 # Game Extraction Toolbox
 
 CLI Tools for investigating game files and extracting known packages
 
 ## Requirements
-- Python 3.7 - 3.11
+- Python 3.9 - 3.11
   - This should be a final release, especially if on Windows / C++ build tools aren't installed
 - PIPx
 
 ## Installation
 ### Quick (if Python and Pipx are already installed)
 ```
 pipx install game-extraction-toolbox
 ```
 
 ### Full
-#### Python 3.7+
+#### Python 3.9+
 Should be on Linux and MacOSX by default; for Windows, I recommend [Digital Ocean's tutorial](https://www.digitalocean.com/community/tutorials/install-python-windows-10)
 
 #### PIPX
 
 ##### Windows
 ```
 py -m pip install --user pipx
@@ -146,24 +146,27 @@
 ### Playable
 
 **Collection**                                  | **Status**     | **Verification** | **Notes**           
 ------------------------------------------------|----------------|------------------|---------------------------------------------------  
  **Arcade Collection Anniversary Classics**     | 88%            | Y                | All games except scramble!
  **Atari Vault**                                | 90%            | Y                | Some arcade ROMs from this collection are incomplete.  
  **Blizzard Arcade Collection**                 | 100%           | Y                |   
+ **Breakers Collection**                        | 100%           | Y                |   
  **Bubsy Two-Fur**                              | 100%           | Y                |   
  **Capcom Arcade Stadium 1 (via Depot)**        | 95%            | N                | Requires Steam depot downloading, a couple shaky ROMs... 
  **Capcom Beat 'Em Up Bundle**                  | 95%            | Y                | 6/7 playable on some version of MAME, but wof/wofj missing audiocpu data  
  **Capcom Fighting Collection**                 | 90%            | Y                | CPS2 is semi-standard. No Enc keys present. CP3 game is a curveball!  
  **Collection of SaGa/Final Fantasy Legend**    | 100%           | Y                |  
  **Disney Afternoon Collection**                | 100%           | Y                |  
  **Disney Classics Aladdin & Lion King w/DLC**  | 100%           | Y                | Includes Jungle Book DLC
  **Double Dragon Trilogy**                      | 100%           | Y                |  
  **IREM Arcade Classics**                       | 100%           | Y                |  
  **Mega Man Legacy Collection 1**               | 100%           | Y                |  
+ **Mega Man Battle Network Legacy Collection 1**| 100%           | Y                | 
+ **Mega Man Battle Network Legacy Collection 2**| 100%           | Y                | 
  **Mega Man X Legacy Collection 1**             | 75%            | Y                | X4 doesn't appear to be ROM based  
  **Namco Arcade Game Series: Dig Dug**          | 100%           | Y                |   
  **Namco Arcade Game Series: Galaga**           | 100%           | Y                |   
  **Namco Arcade Game Series: Ms. Pac-Man**      | 100%           | Y                |   
  **Namco Arcade Game Series: Pacman**           | 100%           | Y                |   
  **NeoGeo Classics by SNK (Humble Store)**      | 95%            | Y                | Baseball Stars 2 is more complex 
  **Pac Man Museum Plus**                        | 40%            | Y                | Some progress, but there are a lot of non-extractable titles.
```

### Comparing `game-extraction-toolbox-0.1.6/README.md` & `game-extraction-toolbox-0.1.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [![PyPI version](https://badge.fury.io/py/game-extraction-toolbox.svg)](https://badge.fury.io/py/game-extraction-toolbox)
 
 # Game Extraction Toolbox
 
 CLI Tools for investigating game files and extracting known packages
 
 ## Requirements
-- Python 3.7 - 3.11
+- Python 3.9 - 3.11
   - This should be a final release, especially if on Windows / C++ build tools aren't installed
 - PIPx
 
 ## Installation
 ### Quick (if Python and Pipx are already installed)
 ```
 pipx install game-extraction-toolbox
 ```
 
 ### Full
-#### Python 3.7+
+#### Python 3.9+
 Should be on Linux and MacOSX by default; for Windows, I recommend [Digital Ocean's tutorial](https://www.digitalocean.com/community/tutorials/install-python-windows-10)
 
 #### PIPX
 
 ##### Windows
 ```
 py -m pip install --user pipx
@@ -113,24 +113,27 @@
 ### Playable
 
 **Collection**                                  | **Status**     | **Verification** | **Notes**           
 ------------------------------------------------|----------------|------------------|---------------------------------------------------  
  **Arcade Collection Anniversary Classics**     | 88%            | Y                | All games except scramble!
  **Atari Vault**                                | 90%            | Y                | Some arcade ROMs from this collection are incomplete.  
  **Blizzard Arcade Collection**                 | 100%           | Y                |   
+ **Breakers Collection**                        | 100%           | Y                |   
  **Bubsy Two-Fur**                              | 100%           | Y                |   
  **Capcom Arcade Stadium 1 (via Depot)**        | 95%            | N                | Requires Steam depot downloading, a couple shaky ROMs... 
  **Capcom Beat 'Em Up Bundle**                  | 95%            | Y                | 6/7 playable on some version of MAME, but wof/wofj missing audiocpu data  
  **Capcom Fighting Collection**                 | 90%            | Y                | CPS2 is semi-standard. No Enc keys present. CP3 game is a curveball!  
  **Collection of SaGa/Final Fantasy Legend**    | 100%           | Y                |  
  **Disney Afternoon Collection**                | 100%           | Y                |  
  **Disney Classics Aladdin & Lion King w/DLC**  | 100%           | Y                | Includes Jungle Book DLC
  **Double Dragon Trilogy**                      | 100%           | Y                |  
  **IREM Arcade Classics**                       | 100%           | Y                |  
  **Mega Man Legacy Collection 1**               | 100%           | Y                |  
+ **Mega Man Battle Network Legacy Collection 1**| 100%           | Y                | 
+ **Mega Man Battle Network Legacy Collection 2**| 100%           | Y                | 
  **Mega Man X Legacy Collection 1**             | 75%            | Y                | X4 doesn't appear to be ROM based  
  **Namco Arcade Game Series: Dig Dug**          | 100%           | Y                |   
  **Namco Arcade Game Series: Galaga**           | 100%           | Y                |   
  **Namco Arcade Game Series: Ms. Pac-Man**      | 100%           | Y                |   
  **Namco Arcade Game Series: Pacman**           | 100%           | Y                |   
  **NeoGeo Classics by SNK (Humble Store)**      | 95%            | Y                | Baseball Stars 2 is more complex 
  **Pac Man Museum Plus**                        | 40%            | Y                | Some progress, but there are a lot of non-extractable titles.
```

### Comparing `game-extraction-toolbox-0.1.6/pyproject.toml` & `game-extraction-toolbox-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "game-extraction-toolbox"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="Shawn McNaughton", email="shawngmc@gmail.com" },
 ]
 description = "CLI Tools for investigating game files and extracting known packages"
 readme = "README.md"
 license = { file="LICENSE" }
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 dependencies = [
   'bitarray >= 2.6.0',
   'click >= 8.1.3',
   'click-log >= 0.4.0',
   'psutil >= 5.9.1',
   'python-magic-bin >= 0.4.14; platform_system == "Windows"',
   'rich >= 12.5.1',
```

### Comparing `game-extraction-toolbox-0.1.6/src/game_extraction_toolbox.egg-info/PKG-INFO` & `game-extraction-toolbox-0.1.7/src/game_extraction_toolbox.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: game-extraction-toolbox
-Version: 0.1.6
+Version: 0.1.7
 Summary: CLI Tools for investigating game files and extracting known packages
 Author-email: Shawn McNaughton <shawngmc@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Shawn McNaughton
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,37 +23,37 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/shawngmc/game-extraction-toolbox
 Project-URL: Bug Tracker, https://github.com/shawngmc/game-extraction-toolbox/issues
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI version](https://badge.fury.io/py/game-extraction-toolbox.svg)](https://badge.fury.io/py/game-extraction-toolbox)
 
 # Game Extraction Toolbox
 
 CLI Tools for investigating game files and extracting known packages
 
 ## Requirements
-- Python 3.7 - 3.11
+- Python 3.9 - 3.11
   - This should be a final release, especially if on Windows / C++ build tools aren't installed
 - PIPx
 
 ## Installation
 ### Quick (if Python and Pipx are already installed)
 ```
 pipx install game-extraction-toolbox
 ```
 
 ### Full
-#### Python 3.7+
+#### Python 3.9+
 Should be on Linux and MacOSX by default; for Windows, I recommend [Digital Ocean's tutorial](https://www.digitalocean.com/community/tutorials/install-python-windows-10)
 
 #### PIPX
 
 ##### Windows
 ```
 py -m pip install --user pipx
@@ -146,24 +146,27 @@
 ### Playable
 
 **Collection**                                  | **Status**     | **Verification** | **Notes**           
 ------------------------------------------------|----------------|------------------|---------------------------------------------------  
  **Arcade Collection Anniversary Classics**     | 88%            | Y                | All games except scramble!
  **Atari Vault**                                | 90%            | Y                | Some arcade ROMs from this collection are incomplete.  
  **Blizzard Arcade Collection**                 | 100%           | Y                |   
+ **Breakers Collection**                        | 100%           | Y                |   
  **Bubsy Two-Fur**                              | 100%           | Y                |   
  **Capcom Arcade Stadium 1 (via Depot)**        | 95%            | N                | Requires Steam depot downloading, a couple shaky ROMs... 
  **Capcom Beat 'Em Up Bundle**                  | 95%            | Y                | 6/7 playable on some version of MAME, but wof/wofj missing audiocpu data  
  **Capcom Fighting Collection**                 | 90%            | Y                | CPS2 is semi-standard. No Enc keys present. CP3 game is a curveball!  
  **Collection of SaGa/Final Fantasy Legend**    | 100%           | Y                |  
  **Disney Afternoon Collection**                | 100%           | Y                |  
  **Disney Classics Aladdin & Lion King w/DLC**  | 100%           | Y                | Includes Jungle Book DLC
  **Double Dragon Trilogy**                      | 100%           | Y                |  
  **IREM Arcade Classics**                       | 100%           | Y                |  
  **Mega Man Legacy Collection 1**               | 100%           | Y                |  
+ **Mega Man Battle Network Legacy Collection 1**| 100%           | Y                | 
+ **Mega Man Battle Network Legacy Collection 2**| 100%           | Y                | 
  **Mega Man X Legacy Collection 1**             | 75%            | Y                | X4 doesn't appear to be ROM based  
  **Namco Arcade Game Series: Dig Dug**          | 100%           | Y                |   
  **Namco Arcade Game Series: Galaga**           | 100%           | Y                |   
  **Namco Arcade Game Series: Ms. Pac-Man**      | 100%           | Y                |   
  **Namco Arcade Game Series: Pacman**           | 100%           | Y                |   
  **NeoGeo Classics by SNK (Humble Store)**      | 95%            | Y                | Baseball Stars 2 is more complex 
  **Pac Man Museum Plus**                        | 40%            | Y                | Some progress, but there are a lot of non-extractable titles.
```

### Comparing `game-extraction-toolbox-0.1.6/src/game_extraction_toolbox.egg-info/SOURCES.txt` & `game-extraction-toolbox-0.1.7/src/game_extraction_toolbox.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -70,14 +70,16 @@
 src/gex/lib/tasks/impl/ags_pacman/__init__.py
 src/gex/lib/tasks/impl/ags_pacman/metadata.json
 src/gex/lib/tasks/impl/atarivault/__init__.py
 src/gex/lib/tasks/impl/atarivault/arcade.py
 src/gex/lib/tasks/impl/atarivault/metadata.json
 src/gex/lib/tasks/impl/blizzarcade/__init__.py
 src/gex/lib/tasks/impl/blizzarcade/metadata.json
+src/gex/lib/tasks/impl/breakers/__init__.py
+src/gex/lib/tasks/impl/breakers/metadata.json
 src/gex/lib/tasks/impl/bubsy/__init__.py
 src/gex/lib/tasks/impl/bubsy/metadata.json
 src/gex/lib/tasks/impl/cas1/__init__.py
 src/gex/lib/tasks/impl/cas1_old/__init__.py
 src/gex/lib/tasks/impl/cas2/__init__.py
 src/gex/lib/tasks/impl/cbeub/__init__.py
 src/gex/lib/tasks/impl/cbeub/metadata.json
@@ -90,14 +92,18 @@
 src/gex/lib/tasks/impl/disneyalkb/__init__.py
 src/gex/lib/tasks/impl/disneyalkb/metadata.json
 src/gex/lib/tasks/impl/genesis/__init__.py
 src/gex/lib/tasks/impl/genesis/metadata.json
 src/gex/lib/tasks/impl/irem/__init__.py
 src/gex/lib/tasks/impl/irem/metadata.json
 src/gex/lib/tasks/impl/mkak/__init__.py
+src/gex/lib/tasks/impl/mmbnlc1/__init__.py
+src/gex/lib/tasks/impl/mmbnlc1/metadata.json
+src/gex/lib/tasks/impl/mmbnlc2/__init__.py
+src/gex/lib/tasks/impl/mmbnlc2/metadata.json
 src/gex/lib/tasks/impl/mmlc1/__init__.py
 src/gex/lib/tasks/impl/mmlc1/metadata.json
 src/gex/lib/tasks/impl/mmxlc1/__init__.py
 src/gex/lib/tasks/impl/mmxlc1/metadata.json
 src/gex/lib/tasks/impl/neogeo_classics_humble/__init__.py
 src/gex/lib/tasks/impl/neogeo_classics_humble/metadata.json
 src/gex/lib/tasks/impl/pacmanmplus/__init__.py
```

### Comparing `game-extraction-toolbox-0.1.6/src/gex/commands/archive/arc/extract.py` & `game-extraction-toolbox-0.1.7/src/gex/commands/archive/arc/extract.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/commands/archive/kpka/extract.py` & `game-extraction-toolbox-0.1.7/src/gex/commands/archive/kpka/extract.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/commands/archive/zip/list.py` & `game-extraction-toolbox-0.1.7/src/gex/commands/archive/zip/list.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/commands/file/deinterleave.py` & `game-extraction-toolbox-0.1.7/src/gex/commands/file/deinterleave.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/commands/file/diff.py` & `game-extraction-toolbox-0.1.7/src/gex/commands/file/diff.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/commands/file/hash.py` & `game-extraction-toolbox-0.1.7/src/gex/commands/file/hash.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/commands/file/slice.py` & `game-extraction-toolbox-0.1.7/src/gex/commands/file/slice.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/commands/finder/bulk.py` & `game-extraction-toolbox-0.1.7/src/gex/commands/finder/bulk.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/commands/postprocess/wii/cleanrip.py` & `game-extraction-toolbox-0.1.7/src/gex/commands/postprocess/wii/cleanrip.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/commands/tasks/details.py` & `game-extraction-toolbox-0.1.7/src/gex/commands/tasks/details.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/commands/tasks/extract.py` & `game-extraction-toolbox-0.1.7/src/gex/commands/tasks/extract.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/archive/arc.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/archive/arc.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/archive/kpka.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/archive/kpka.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/archive/prs.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/archive/prs.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/archive/zip.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/archive/zip.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/contrib/bputil.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/contrib/bputil.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/file/identify.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/file/identify.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 '''
 Wrapper for python-magic that adds support for game extraction specific file types
 '''
 import magic
 
+# Internally tracking these in https://docs.google.com/spreadsheets/d/1eMI9EIzopg1J9UZsMFOx5lLSMPsf7EYxovLM5VFoUjU/edit#gid=0
+
 KPKA = "KPKA Archive, Capcom RE Engine"
 IBIS = "IBIS Archive, Capcom ROM Releases"
-ARC = "ARC Archive, Capcom MT Engine"
+ARC = "ARC Archive, Capcom MT Framework"
+M2 = "M2 Archive, M2 (Developer/Publisher)"
 
 def enhanced_magic_from_path(in_file):
     '''Use libmagic and enhanced_look to id a file's contents'''
     magic_id = None
     try:
         magic_id = magic.from_file(in_file)
     except Exception as error:
@@ -41,13 +44,15 @@
     '''Magic-like function that identifies uncommon relevant filetypes'''
     if content_peek[0:4] == b"KPKA":
         return KPKA
     if content_peek[0:4] == b"IBIS":
         return IBIS
     if content_peek[0:3] == b"ARC":
         return ARC
+    if content_peek[0:3] == b"mdf":
+        return M2
     return 'data'
 
 _PK_HEADER = "PK".encode('utf-8')
 def check_if_zip(contents):
     '''Simple ZIP file check that searches for a 'PK' ZIP header'''
     return contents[0:2] == _PK_HEADER
```

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/basetask.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/basetask.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/copytask.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/copytask.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/helpers.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 '''Convenience wrappers for task implementation'''
 import io
 import os
 import zipfile
 from gex.lib.utils.blob import transforms
+import gex.lib.archive.zip as ziphelper
 
 STEAM_APP_ROOT = r"C:\Program Files (x86)\Steam\steamapps\common"
 def gen_steam_app_default_folder(app_folder, library_root=STEAM_APP_ROOT):
     '''Convenience function to get a Steam App folder'''
     return os.path.join(library_root, app_folder)
 
 def build_rom(in_files, func_map):
@@ -118,7 +119,22 @@
         out_files = {}
 
         for src_name, dst_name in rename_map.items():
             out_files[dst_name] = common_file_map.get(src_name)
 
         return out_files
     return pick
+
+def pull_files_from_archive(archive_data, archive_type, file_map):
+    out_files = []
+
+    archive_contents = None
+    if archive_type == "zip":
+        archive_contents = ziphelper.extract(archive_data)
+
+    for destination_name, archive_name in file_map.items():
+        out_files.append({
+            'filename': destination_name,
+            'contents': archive_contents[archive_name]['contents']
+        })
+
+    return out_files
```

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/acac/__init__.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/acac/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,44 +28,55 @@
         '''Return a list of output files'''
         return {
             "files": self._metadata['out']['files'],
             "notes": self._metadata['out']['notes']
         }
 
     def execute(self, in_dir, out_dir):
-        src_file = os.path.join(in_dir, "AA_AC_ArcadeClassics.exe")
-        with open(src_file, 'rb') as src_file:
-            src_contents = src_file.read()
-            src_contents_decomp = self.lzma_multi_decomp(src_contents, out_dir)
+        src_file = self.read_all_datafiles(in_dir).get("source")
+        src_contents = src_file['contents']
+        file_ver = src_file['version']
 
-        with open(os.path.join(out_dir, 'merged_decomp_blob'), "wb") as out_file:
-            out_file.write(src_contents_decomp)
+        # src_contents_decomp = self.lzma_multi_decomp(src_contents, out_dir)
+
+        # with open(os.path.join(out_dir, 'merged_decomp_blob'), "wb") as out_file:
+        #     out_file.write(src_contents_decomp)
 
         out_files = []
-        out_files.extend(self._handle_nemesis(src_contents))
-        out_files.extend(self._handle_hcastle(src_contents))
-        out_files.extend(self._handle_ajax(src_contents))
-        out_files.extend(self._handle_vulcan(src_contents))
-        out_files.extend(self._handle_thunderx(src_contents))
-        out_files.extend(self._handle_salamand(src_contents))
-        out_files.extend(self._handle_twinbee(src_contents))
+        out_files.extend(self._handle_nemesis(src_contents, file_ver))
+        out_files.extend(self._handle_hcastle(src_contents, file_ver))
+        out_files.extend(self._handle_ajax(src_contents, file_ver))
+        out_files.extend(self._handle_vulcan(src_contents, file_ver))
+        out_files.extend(self._handle_thunderx(src_contents, file_ver))
+        out_files.extend(self._handle_salamand(src_contents, file_ver))
+        out_files.extend(self._handle_twinbee(src_contents, file_ver))
 
         if out_files:
             for out_file_entry in out_files:
                 filename = out_file_entry['filename']
                 _ = self.verify_out_file(filename, out_file_entry['contents'])
                 out_path = os.path.join(out_dir, filename)
                 with open(out_path, "wb") as out_file:
                     logger.info(f"Writing {out_file_entry['filename']}...")
                     out_file.write(out_file_entry['contents'])
 
         logger.info("Processing complete.")
 
-    def _handle_ajax(self, contents):
-        contents = transforms.cut(contents, 0x11B610, length=1124930)
+    def _get_extract_metadata(self, game_name):
+        for game in self._metadata['out']['files']:
+            if game['game'] == game_name:
+                return game['extract']
+
+        return None
+
+    def _handle_ajax(self, contents, version):
+        extract_metadata = self._get_extract_metadata('Typhoon')
+        contents = transforms.cut(contents, 
+            int(extract_metadata['versions'][version]['start'], 0),
+            length=extract_metadata['length'])
         lzd = lzma.LZMADecompressor()
         contents = lzd.decompress(contents)
         out_files = []
         
         # AJAX Common
         func_map = {}
         def k_roms(contents):
@@ -116,16 +127,19 @@
         func_map['maincpu'] = typhoon_maincpu
         func_map['k_roms'] = ajaxj_krom
         func_map['common'] = helpers.existing_files_helper(common_file_map)
         out_files.append({'filename': 'typhoon.zip', 'contents': helpers.build_rom(contents, func_map)})
         
         return out_files
 
-    def _handle_nemesis(self, contents):
-        contents = transforms.cut(contents, 0x2F2DE0, length=541168)
+    def _handle_nemesis(self, contents, version):
+        extract_metadata = self._get_extract_metadata('Nemesis')
+        contents = transforms.cut(contents, 
+            int(extract_metadata['versions'][version]['start'], 0),
+            length=extract_metadata['length'])
         lzd = lzma.LZMADecompressor()
         contents = lzd.decompress(contents)
         out_files = []
 
         # Nemesis Common
         func_map = {}
         def k_rom(contents):
@@ -188,16 +202,19 @@
         func_map['audiocpu'] = nemesisuk_audiocpu
         func_map['common'] = helpers.existing_files_helper(common_file_map)
         out_files.append({'filename': 'nemesisuk.zip', 'contents': helpers.build_rom(contents, func_map)})
 
         return out_files
 
 
-    def _handle_hcastle(self, contents):
-        contents = transforms.cut(contents, 0x22E110, length=798376)
+    def _handle_hcastle(self, contents, version):
+        extract_metadata = self._get_extract_metadata('Haunted Castle (Version M)')
+        contents = transforms.cut(contents, 
+            int(extract_metadata['versions'][version]['start'], 0),
+            length=extract_metadata['length'])
         lzd = lzma.LZMADecompressor()
         contents = lzd.decompress(contents)
 
         out_files = []
 
         # HCastle Common
         func_map = {}
@@ -268,16 +285,19 @@
             return out_chunks
         func_map['maincpu'] = akumajoun_maincpu
         func_map['common'] = helpers.existing_files_helper(common_file_map)
         out_files.append({'filename': 'akumajoun.zip', 'contents': helpers.build_rom(contents, func_map)})
 
         return out_files
 
-    def _handle_vulcan(self, contents):
-        contents = transforms.cut(contents, 0x37C280, length=3080192)
+    def _handle_vulcan(self, contents, version):
+        extract_metadata = self._get_extract_metadata('Vulcan Venture')
+        contents = transforms.cut(contents, 
+            int(extract_metadata['versions'][version]['start'], 0),
+            length=extract_metadata['length'])
         lzd = lzma.LZMADecompressor()
         contents = lzd.decompress(contents)
         out_files = []
 
         # 0x000000   0x040000     maincpu - gradius2
         # 0x040000   0x040000     maincpu - vulcan
         # 0x080000   0x040000     sub
@@ -378,15 +398,19 @@
         func_map['common'] = helpers.existing_files_helper(common_file_map)
         out_files.append({'filename': 'vulcan.zip', 'contents': helpers.build_rom(contents, func_map)})
 
         return out_files
 
 
 
-    def _handle_thunderx(self, contents):
+    def _handle_thunderx(self, contents, version):
+        extract_metadata = self._get_extract_metadata('Thunder Cross (Set 1)')
+        contents = transforms.cut(contents, 
+            int(extract_metadata['versions'][version]['start'], 0),
+            length=extract_metadata['length'])
         contents = transforms.cut(contents, 0x4D13D0, length=455549)
         lzd = lzma.LZMADecompressor()
         contents = lzd.decompress(contents)
         out_files = []
 
         # 0x000000 0x020000     maincpu - thunderxj
         # 0x020000 0x008000     audiocpu -thunderxj/xb/x
@@ -567,16 +591,19 @@
         func_map['audiocpu'] = thunderxa_audiocpu
         func_map['common'] = helpers.existing_files_helper(common_file_map)
         out_files.append({'filename': 'thunderxa.zip', 'contents': helpers.build_rom(contents, func_map)})
 
         return out_files
 
 
-    def _handle_salamand(self, contents):
-        contents = transforms.cut(contents, 0x4165D0, length=752816)
+    def _handle_salamand(self, contents, version):
+        extract_metadata = self._get_extract_metadata('Salamander')
+        contents = transforms.cut(contents, 
+            int(extract_metadata['versions'][version]['start'], 0),
+            length=extract_metadata['length'])
         lzd = lzma.LZMADecompressor()
         contents = lzd.decompress(contents)
         out_files = []
 
         #                                   salamand        salamandj       lifefrce        lifefrcej
         # 0x000000  0x20000     maincpu2                    X
         # 0x020000  0x40000     
@@ -718,19 +745,22 @@
             chunks = transforms.deinterleave(contents, 2, 1)
             return dict(zip(filenames, chunks))
         func_map['maincpu1'] = lifefrcej_maincpu1
         out_files.append({'filename': 'lifefrcej.zip', 'contents': helpers.build_rom(contents, func_map)})
 
         return out_files
 
-    def _handle_twinbee(self, full_contents):
+    def _handle_twinbee(self, full_contents, version):
         out_files = []
         
         # Get FSE files Nemesis
-        contents = transforms.cut(full_contents, 0x2F2DE0, length=541168)
+        extract_metadata = self._get_extract_metadata('Nemesis')
+        contents = transforms.cut(full_contents, 
+            int(extract_metadata['versions'][version]['start'], 0),
+            length=extract_metadata['length'])
         lzd = lzma.LZMADecompressor()
         contents = lzd.decompress(contents)
 
         func_map = {}
         def fse(contents):
             filenames = [
                 "400-a01.fse",
@@ -739,16 +769,19 @@
             chunks = []
             contents = transforms.cut(contents, 0x84000, length = 0x200)
             chunks = transforms.equal_split(contents, len(filenames))
             return dict(zip(filenames, chunks))
         func_map['fse'] = fse
         fse_file_map = helpers.process_rom_files(contents, func_map)
 
+        extract_metadata = self._get_extract_metadata('Twinbee')
         # Get the maincpu1
-        contents = transforms.cut(full_contents, 0x5407E0, length=67191)
+        contents = transforms.cut(full_contents, 
+            int(extract_metadata['versions'][version]['start_maincpu'], 0),
+            length=extract_metadata['length'])
         lzd = lzma.LZMADecompressor()
         contents = lzd.decompress(contents)
 
         func_map = {}
         def maincpu1(contents):
             filenames = [
                 "412-a07.12l",
@@ -756,15 +789,17 @@
             ]
             chunks = transforms.deinterleave(contents, 2, 1)
             return dict(zip(filenames, chunks))
         func_map['maincpu1'] = maincpu1
         maincpu1_file_map = helpers.process_rom_files(contents, func_map)
 
         # Get the k rom
-        contents = transforms.cut(full_contents, 0x2F1050, length=67191)
+        contents = transforms.cut(full_contents,
+            int(extract_metadata['versions'][version]['start_krom'], 0),
+            length=extract_metadata['length'])
         lzd = lzma.LZMADecompressor()
         contents = lzd.decompress(contents)
         func_map = {}
         def krom(contents):
             filenames = [
                 "400-a06.15l",
                 "400-a04.10l",
```

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ags_digdug/__init__.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ags_digdug/__init__.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ags_digdug/metadata.json` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ags_digdug/metadata.json`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ags_galaga/__init__.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ags_galaga/__init__.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ags_galaga/metadata.json` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ags_galaga/metadata.json`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ags_mspacman/__init__.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ags_mspacman/__init__.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ags_mspacman/metadata.json` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ags_mspacman/metadata.json`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ags_pacman/__init__.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ags_pacman/__init__.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ags_pacman/metadata.json` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ags_pacman/metadata.json`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/atarivault/__init__.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/atarivault/__init__.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/atarivault/arcade.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/atarivault/arcade.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/atarivault/metadata.json` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/atarivault/metadata.json`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/blizzarcade/__init__.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/blizzarcade/__init__.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/blizzarcade/metadata.json` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/blizzarcade/metadata.json`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/bubsy/metadata.json` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/bubsy/metadata.json`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/cas1/__init__.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/cas1/__init__.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/cas1_old/__init__.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/cas1_old/__init__.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/cas2/__init__.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/cas2/__init__.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/cbeub/__init__.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/cbeub/__init__.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/cbeub/metadata.json` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/cbeub/metadata.json`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/cfc/__init__.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/cfc/__init__.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/cfc/metadata.json` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/cfc/metadata.json`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ddragontrilogy/__init__.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ddragontrilogy/__init__.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ddragontrilogy/metadata.json` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ddragontrilogy/metadata.json`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/disneyac/__init__.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/disneyac/__init__.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/disneyac/metadata.json` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/disneyac/metadata.json`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/disneyalkb/__init__.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/disneyalkb/__init__.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/disneyalkb/metadata.json` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/disneyalkb/metadata.json`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/genesis/__init__.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/genesis/__init__.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/genesis/metadata.json` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/genesis/metadata.json`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/irem/__init__.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/irem/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from gex.lib.tasks import helpers
 from gex.lib.utils.blob import transforms
 from gex.lib.utils import gfx_rebuilder
 from gex.lib.tasks.basetask import BaseTask
 
 logger = logging.getLogger('gextoolbox')
 
+
 class IremTask(BaseTask):
     '''Implments irem: Irem Arcade Hits'''
     _task_name = "irem"
     _title = "Irem Arcade Hits"
     _details_markdown = '''
 Uses Windows version from https://www.gamefools.com/pc-games/irem-arcade-hits.html
 Based on dotemu2mame.js: https://gist.github.com/cxx/81b9f45eb5b3cb87b4f3783ccdf8894f
@@ -26,15 +27,16 @@
         return {
             "files": self._metadata['out']['files'],
             "notes": self._metadata['out']['notes']
         }
 
     def _read_irem_game(self, in_name, in_dir):
         '''Handle the zip-in-zip packaging format'''
-        outer_zip = self.read_datafile(in_dir, self._metadata['in']['files'][in_name])
+        outer_zip = self.read_datafile(
+            in_dir, self._metadata['in']['files'][in_name])
         outer_zip_bytes = outer_zip['contents']
         with ZipFile(BytesIO(outer_zip_bytes), 'r') as outer_zip:
             inner_zip_bytes = outer_zip.read(f"arcade_{in_name}.zip")
 
         out_files = {}
         with ZipFile(BytesIO(inner_zip_bytes), 'r') as inner_zip:
             for filename in inner_zip.namelist():
@@ -62,19 +64,21 @@
     def _handle_airduel(self, in_files):
         func_map = {}
 
         # maincpu
         maincpu_filenames = [
             'ad-c-l0.bin', 'ad-c-l3.bin', 'ad-c-h0.bin', 'ad-c-h3.bin'
         ]
+
         def maincpu(in_files):
             contents = in_files['CPU.BIN']
             contents = transforms.cut(contents, 0, length=0x80000)
             chunks = transforms.deinterleave(contents, num_ways=2, word_size=1)
-            chunks = transforms.transform_all(chunks, transforms.equal_split, 2)
+            chunks = transforms.transform_all(
+                chunks, transforms.equal_split, 2)
             return dict(zip(maincpu_filenames, chunks))
         func_map['maincpu'] = maincpu
 
         # GFX1 - Sprites
         func_map['gfx1'] = helpers.equal_split_helper(
             'GFX1.BIN',
             ['ad-00.bin', 'ad-10.bin', 'ad-20.bin', 'ad-30.bin']
@@ -104,19 +108,21 @@
         func_map = {}
 
         # maincpu
         maincpu_filenames = [
             'c-l0-b.rom', 'c-l1-b.rom', 'c-l3-b.rom',
             'c-h0-b.rom', 'c-h1-b.rom', 'c-h3-b.rom'
         ]
+
         def maincpu(in_files):
             contents = in_files['CPU.BIN']
             contents = transforms.cut(contents, 0, length=0x80000)
             chunks = transforms.deinterleave(contents, num_ways=2, word_size=1)
-            chunks = transforms.transform_all(chunks, transforms.equal_split, 4)
+            chunks = transforms.transform_all(
+                chunks, transforms.equal_split, 4)
             del chunks[6]
             del chunks[2]
             return dict(zip(maincpu_filenames, chunks))
         func_map['maincpu'] = maincpu
 
         # GFX1 - Sprites
         func_map['gfx1'] = helpers.equal_split_helper(
@@ -148,26 +154,29 @@
     def _handle_bmaster(self, in_files):
         func_map = {}
 
         # maincpu
         maincpu_filenames = [
             'bm_d-l0-b.5f', 'bm_d-l1-b.5j', 'bm_d-h0-b.5m', 'bm_d-h1-b.5l'
         ]
+
         def maincpu(in_files):
             contents = in_files['CPU1.BIN']
             contents = transforms.cut(contents, 0, length=0xa0000)
             chunks = transforms.deinterleave(contents, num_ways=2, word_size=1)
-            chunks = transforms.transform_all(chunks, transforms.custom_split, [0x40000, 0x10000])
+            chunks = transforms.transform_all(
+                chunks, transforms.custom_split, [0x40000, 0x10000])
             return dict(zip(maincpu_filenames, chunks))
         func_map['maincpu'] = maincpu
 
         # soundcpu
         soundcpu_filenames = [
             'bm_d-sl0.rom', 'bm_d-sh0.rom'
         ]
+
         def soundcpu(in_files):
             contents = in_files['CPU2.BIN']
             chunks = transforms.deinterleave(contents, num_ways=2, word_size=1)
             return dict(zip(soundcpu_filenames, chunks))
         func_map['soundcpu'] = soundcpu
 
         # GFX1 - Sprites
@@ -193,14 +202,15 @@
     def _handle_cosmccop(self, in_files):
         func_map = {}
 
         # maincpu
         maincpu_filenames = [
             'cc-d-l0b.bin', 'cc-d-h0b.bin'
         ]
+
         def maincpu(in_files):
             contents = in_files['CPU1.BIN']
             contents = transforms.cut(contents, 0, length=0x80000)
             chunks = transforms.deinterleave(contents, num_ways=2, word_size=1)
             return dict(zip(maincpu_filenames, chunks))
         func_map['maincpu'] = maincpu
 
@@ -233,19 +243,21 @@
     def _handle_dbreed72(self, in_files):
         func_map = {}
 
         # maincpu
         maincpu_filenames = [
             'db_c-l3.rom', 'db_c-l0.rom', 'db_c-h3.rom', 'db_c-h0.rom'
         ]
+
         def maincpu(in_files):
             contents = in_files['CPU.BIN']
             contents = transforms.cut(contents, 0, length=0x80000)
             chunks = transforms.deinterleave(contents, num_ways=2, word_size=1)
-            chunks = transforms.transform_all(chunks, transforms.custom_split, [0x20000, 0x10000, 0x10000])
+            chunks = transforms.transform_all(chunks, transforms.custom_split, [
+                                              0x20000, 0x10000, 0x10000])
             del chunks[4]
             del chunks[1]
             return dict(zip(maincpu_filenames, chunks))
         func_map['maincpu'] = maincpu
 
         # GFX1 - Sprites
         func_map['gfx1'] = helpers.equal_split_helper(
@@ -271,31 +283,34 @@
             'db_c-v0.rom'
         )
 
         return helpers.build_rom(in_files, func_map)
 
     def _handle_gunforce(self, in_files):
         func_map = {}
-        
+
         # maincpu
         maincpu_filenames = [
             'gf_l0-c.5f', 'gf_l1-c.5j', 'gf_h0-c.5m', 'gf_h1-c.5l'
         ]
+
         def maincpu(in_files):
             contents = in_files['CPU1.BIN']
             contents = transforms.cut(contents, 0, length=0x80000)
             chunks = transforms.deinterleave(contents, num_ways=2, word_size=1)
-            chunks = transforms.transform_all(chunks, transforms.equal_split, 2)
+            chunks = transforms.transform_all(
+                chunks, transforms.equal_split, 2)
             return dict(zip(maincpu_filenames, chunks))
         func_map['maincpu'] = maincpu
 
         # soundcpu
         soundcpu_filenames = [
             'gf_sl0.rom', 'gf_sh0.rom'
         ]
+
         def soundcpu(in_files):
             contents = in_files['CPU2.BIN']
             contents = transforms.cut(contents, 0, length=0x20000)
             chunks = transforms.deinterleave(contents, num_ways=2, word_size=1)
             return dict(zip(soundcpu_filenames, chunks))
         func_map['soundcpu'] = soundcpu
 
@@ -317,33 +332,36 @@
             'gf-da.rom'
         )
 
         return helpers.build_rom(in_files, func_map)
 
     def _handle_gunforc2(self, in_files):
         func_map = {}
-        
+
         # maincpu
         maincpu_filenames = [
             'a2-l0-a.8h', 'a2-l1-a.8f', 'a2-h0-a.6h', 'a2-h1-a.6f'
         ]
+
         def maincpu(in_files):
             contents = in_files['CPU1.BIN']
             chunks = transforms.deinterleave(contents, num_ways=2, word_size=1)
             contents = transforms.cut(contents, 0, length=0x80000)
-            chunks = transforms.transform_all(chunks, transforms.custom_split, [0x40000, 0x40000, 0x40000])
+            chunks = transforms.transform_all(chunks, transforms.custom_split, [
+                                              0x40000, 0x40000, 0x40000])
             del chunks[4]
             del chunks[1]
             return dict(zip(maincpu_filenames, chunks))
         func_map['maincpu'] = maincpu
 
         # soundcpu
         soundcpu_filenames = [
             'a2_sl0.5l', 'a2_sh0.3l'
         ]
+
         def soundcpu(in_files):
             contents = in_files['CPU2.BIN']
             contents = transforms.cut(contents, 0, length=0x20000)
             chunks = transforms.deinterleave(contents, num_ways=2, word_size=1)
             return dict(zip(soundcpu_filenames, chunks))
         func_map['soundcpu'] = soundcpu
 
@@ -370,19 +388,21 @@
     def _handle_hharry(self, in_files):
         func_map = {}
 
         # maincpu
         maincpu_filenames = [
             'a-l0-v.rom', 'a-l1-0.rom', 'a-h0-v.rom', 'a-h1-0.rom'
         ]
+
         def maincpu(in_files):
             contents = in_files['CPU1.BIN']
             contents = transforms.cut(contents, 0, length=0x80000)
             chunks = transforms.deinterleave(contents, num_ways=2, word_size=1)
-            chunks = transforms.transform_all(chunks, transforms.custom_split, [0x20000, 0x10000, 0x10000])
+            chunks = transforms.transform_all(chunks, transforms.custom_split, [
+                                              0x20000, 0x10000, 0x10000])
             del chunks[4]
             del chunks[1]
             return dict(zip(maincpu_filenames, chunks))
         func_map['maincpu'] = maincpu
 
         # Sound
         func_map['sound'] = helpers.name_file_helper(
@@ -403,29 +423,31 @@
         )
 
         # Samples
         func_map['samples'] = helpers.name_file_helper(
             'SAMPLES.BIN',
             'a-v0-0.rom'
         )
-        
+
         return helpers.build_rom(in_files, func_map)
 
     def _handle_imgfight(self, in_files):
         func_map = {}
 
         # maincpu
         maincpu_filenames = [
             'if-c-l0-a.bin', 'if-c-l3.bin', 'if-c-h0-a.bin', 'if-c-h3.bin'
         ]
+
         def maincpu(in_files):
             contents = in_files['CPU.BIN']
             contents = transforms.cut(contents, 0, length=0x80000)
             chunks = transforms.deinterleave(contents, num_ways=2, word_size=1)
-            chunks = transforms.transform_all(chunks, transforms.custom_split, [0x10000, 0x10000, 0x20000])
+            chunks = transforms.transform_all(chunks, transforms.custom_split, [
+                                              0x10000, 0x10000, 0x20000])
             del chunks[4]
             del chunks[1]
             return dict(zip(maincpu_filenames, chunks))
         func_map['maincpu'] = maincpu
 
         # GFX1 - Sprites
         func_map['gfx1'] = helpers.equal_split_helper(
@@ -456,32 +478,35 @@
     def _handle_inthunt(self, in_files):
         func_map = {}
 
         # maincpu
         maincpu_filenames = [
             'ith-l0-d.bin', 'ith-l1-b.bin', 'ith-h0-d.bin', 'ith-h1-b.bin'
         ]
+
         def maincpu(in_files):
             contents = in_files['CPU1.BIN']
             contents = transforms.cut(contents, 0, length=0xC0000)
             chunks = transforms.deinterleave(contents, num_ways=2, word_size=1)
-            chunks = transforms.transform_all(chunks, transforms.custom_split, [0x40000, 0x20000])
+            chunks = transforms.transform_all(
+                chunks, transforms.custom_split, [0x40000, 0x20000])
             return dict(zip(maincpu_filenames, chunks))
         func_map['maincpu'] = maincpu
 
         # soundcpu
         soundcpu_filenames = [
             'ith-sl0.rom', 'ith-sh0.rom'
         ]
+
         def soundcpu(in_files):
             contents = in_files['CPU2.BIN']
             chunks = transforms.deinterleave(contents, num_ways=2, word_size=1)
             return dict(zip(soundcpu_filenames, chunks))
         func_map['soundcpu'] = soundcpu
-        
+
         # GFX1 - Sprites
         func_map['gfx1'] = helpers.equal_split_helper(
             'GFX1.BIN',
             ['ith_ic26.rom', 'ith_ic25.rom', 'ith_ic24.rom', 'ith_ic23.rom']
         )
 
         # GFX2
@@ -508,21 +533,21 @@
         )
 
         # M6803
         func_map['m6803'] = helpers.equal_split_helper(
             'M6803.BIN',
             ['a-3e-.bin', 'a-3f-.bin', 'a-3h-.bin']
         )
-        
+
         # GFX1
         func_map['gfx1'] = helpers.equal_split_helper(
             'GFX1.BIN',
             ['g-4c-a.bin', 'g-4d-a.bin', 'g-4e-a.bin']
         )
-        
+
         # GFX2
         func_map['gfx2'] = helpers.equal_split_helper(
             'GFX2.BIN',
             ['b-4k-.bin', 'b-4f-.bin', 'b-4l-.bin', 'b-4h-.bin',
              'b-3n-.bin', 'b-4n-.bin', 'b-4m-.bin', 'b-3m-.bin',
              'b-4c-.bin', 'b-4e-.bin', 'b-4d-.bin', 'b-4a-.bin']
         )
@@ -544,24 +569,26 @@
         # Timing (Placeholder)
         func_map['timing'] = helpers.placeholder_helper({'b-6f-.bin': 0x100})
 
         return helpers.build_rom(in_files, func_map)
 
     def _handle_loht(self, in_files):
         func_map = {}
-        
+
         # maincpu
         maincpu_filenames = [
             'tom_c-l0.rom', 'tom_c-l3-', 'tom_c-h0.rom', 'tom_c-h3-'
         ]
+
         def maincpu(in_files):
             contents = in_files['CPU.BIN']
             contents = transforms.cut(contents, 0, length=0x80000)
             chunks = transforms.deinterleave(contents, num_ways=2, word_size=1)
-            chunks = transforms.transform_all(chunks, transforms.equal_split, 2)
+            chunks = transforms.transform_all(
+                chunks, transforms.equal_split, 2)
             return dict(zip(maincpu_filenames, chunks))
         func_map['maincpu'] = maincpu
 
         # GFX1 - Sprites
         func_map['gfx1'] = helpers.equal_split_helper(
             'GFX1.BIN',
             ['tom_m53.rom', 'tom_m51.rom', 'tom_m49.rom', 'tom_m47.rom']
@@ -591,19 +618,21 @@
         func_map = {}
 
         # maincpu
         maincpu_filenames = [
             'mh-c-l0.bin', 'mh-c-l1.bin', 'mh-c-l3.bin',
             'mh-c-h0.bin', 'mh-c-h1.bin', 'mh-c-h3.bin'
         ]
+
         def maincpu(in_files):
             contents = in_files['CPU.BIN']
             contents = transforms.cut(contents, 0, length=0x80000)
             chunks = transforms.deinterleave(contents, num_ways=2, word_size=1)
-            chunks = transforms.transform_all(chunks, transforms.equal_split, 4)
+            chunks = transforms.transform_all(
+                chunks, transforms.equal_split, 4)
             del chunks[6]
             del chunks[2]
             return dict(zip(maincpu_filenames, chunks))
         func_map['maincpu'] = maincpu
 
         # GFX1 - Sprites
         func_map['gfx1'] = helpers.equal_split_helper(
@@ -629,31 +658,34 @@
             'c-v0-b.rom'
         )
 
         return helpers.build_rom(in_files, func_map)
 
     def _handle_mysticri(self, in_files):
         func_map = {}
-        
+
         # maincpu
         maincpu_filenames = [
             'mr-l0-b.bin', 'mr-l1-b.bin', 'mr-h0-b.bin', 'mr-h1-b.bin'
         ]
+
         def maincpu(in_files):
             contents = in_files['CPU1.BIN']
             contents = transforms.cut(contents, 0, length=0xa0000)
             chunks = transforms.deinterleave(contents, num_ways=2, word_size=1)
-            chunks = transforms.transform_all(chunks, transforms.custom_split, [0x40000, 0x10000])
+            chunks = transforms.transform_all(
+                chunks, transforms.custom_split, [0x40000, 0x10000])
             return dict(zip(maincpu_filenames, chunks))
         func_map['maincpu'] = maincpu
 
         # soundcpu
         soundcpu_filenames = [
             'mr-sl0.bin', 'mr-sh0.bin'
         ]
+
         def soundcpu(in_files):
             contents = in_files['CPU2.BIN']
             contents = transforms.cut(contents, 0, length=0x20000)
             chunks = transforms.deinterleave(contents, num_ways=2, word_size=1)
             return dict(zip(soundcpu_filenames, chunks))
         func_map['soundcpu'] = soundcpu
 
@@ -663,14 +695,15 @@
             ['mr-c0.bin', 'mr-c1.bin', 'mr-c2.bin', 'mr-c3.bin']
         )
 
         # GFX2
         gfx2_filenames = [
             'mr-o00.bin', 'mr-o10.bin', 'mr-o20.bin', 'mr-o30.bin'
         ]
+
         def gfx2(in_files):
             contents = in_files['GFX2.BIN']
             chunks = transforms.equal_split(contents, 8)
             del chunks[7]
             del chunks[5]
             del chunks[3]
             del chunks[1]
@@ -683,25 +716,27 @@
             'mr-da.bin'
         )
 
         return helpers.build_rom(in_files, func_map)
 
     def _handle_nspirit(self, in_files):
         func_map = {}
-        
+
         # maincpu
         maincpu_filenames = [
             'nin_c-l0.6d', 'nin_c-l1.6c', 'nin_c-l2.6b', 'nin_c-l3.6a',
             'nin_c-h0.6h', 'nin_c-h1.6j', 'nin_c-h2.6l', 'nin_c-h3.6m'
         ]
+
         def maincpu(in_files):
             contents = in_files['CPU.BIN']
             contents = transforms.cut(contents, 0, length=0x80000)
             chunks = transforms.deinterleave(contents, num_ways=2, word_size=1)
-            chunks = transforms.transform_all(chunks, transforms.equal_split, 4)
+            chunks = transforms.transform_all(
+                chunks, transforms.equal_split, 4)
             return dict(zip(maincpu_filenames, chunks))
         func_map['maincpu'] = maincpu
 
         # GFX1 - Sprites
         func_map['gfx1'] = helpers.equal_split_helper(
             'GFX1.BIN',
             ['nin-r00.7m', 'nin-r10.7j', 'nin-r20.7f', 'nin-r30.7d']
@@ -734,31 +769,34 @@
             'm72_a-4d.4d': 0x100
         })
 
         return helpers.build_rom(in_files, func_map)
 
     def _handle_rtypeleo(self, in_files):
         func_map = {}
-        
+
         # maincpu
         maincpu_filenames = [
             'rtl-l0-c.bin', 'rtl-l1-d.bin', 'rtl-h0-c.bin', 'rtl-h1-d.bin'
         ]
+
         def maincpu(in_files):
             contents = in_files['CPU1.BIN']
             contents = transforms.cut(contents, 0, length=0xC0000)
             chunks = transforms.deinterleave(contents, num_ways=2, word_size=1)
-            chunks = transforms.transform_all(chunks, transforms.custom_split, [0x40000, 0x20000])
+            chunks = transforms.transform_all(
+                chunks, transforms.custom_split, [0x40000, 0x20000])
             return dict(zip(maincpu_filenames, chunks))
         func_map['maincpu'] = maincpu
-        
+
         # soundcpu
         soundcpu_filenames = [
             'rtl-sl0a.bin', 'rtl-sh0a.bin'
         ]
+
         def soundcpu(in_files):
             contents = in_files['CPU2.BIN']
             chunks = transforms.deinterleave(contents, num_ways=2, word_size=1)
             return dict(zip(soundcpu_filenames, chunks))
         func_map['soundcpu'] = soundcpu
 
         # GFX1
@@ -779,87 +817,96 @@
             'rtl-da.bin'
         )
 
         return helpers.build_rom(in_files, func_map)
 
     def _handle_ssoldier(self, in_files):
         func_map = {}
-        
+
         # maincpu
         maincpu_filenames = [
             'f3-l0-h.bin', 'f3-l1-a.bin', 'f3-h0-h.bin', 'f3-h1-a.bin'
         ]
+
         def maincpu(in_files):
             contents = in_files['CPU1.BIN']
             contents = transforms.cut(contents, 0, length=0xC0000)
             chunks = transforms.deinterleave(contents, num_ways=2, word_size=1)
-            chunks = transforms.transform_all(chunks, transforms.custom_split, [0x40000, 0x20000])
+            chunks = transforms.transform_all(
+                chunks, transforms.custom_split, [0x40000, 0x20000])
             return dict(zip(maincpu_filenames, chunks))
         func_map['maincpu'] = maincpu
-        
+
         # soundcpu
         soundcpu_filenames = [
             'f3_sl0.sl0', 'f3_sh0.sh0'
         ]
+
         def soundcpu(in_files):
             contents = in_files['CPU2.BIN']
             chunks = transforms.deinterleave(contents, num_ways=2, word_size=1)
             return dict(zip(soundcpu_filenames, chunks))
         func_map['soundcpu'] = soundcpu
 
         # GFX1
         gfx1_filenames = [
             'f3_w50.c0', 'f3_w51.c1', 'f3_w52.c2', 'f3_w53.c3'
         ]
+
         def gfx1(in_files):
             contents = in_files['GFX1.BIN']
             contents = transforms.cut(contents, 0, length=0x100000)
             chunks = transforms.equal_split(contents, 4)
             return dict(zip(gfx1_filenames, chunks))
         func_map['gfx1'] = gfx1
 
         # GFX2
         gfx2_filenames = [
             'f3_w38.001', 'f3_w40.011', 'f3_w42.021', 'f3_w44.031',
             'f3_w37.000', 'f3_w39.010', 'f3_w41.020', 'f3_w43.030'
         ]
+
         def gfx2(in_files):
             contents = in_files['GFX2.BIN']
             chunks = transforms.deinterleave(contents, num_ways=2, word_size=1)
-            chunks = transforms.transform_all(chunks, transforms.equal_split, 4)
+            chunks = transforms.transform_all(
+                chunks, transforms.equal_split, 4)
             return dict(zip(gfx2_filenames, chunks))
         func_map['gfx2'] = gfx2
 
         # Sound
         func_map['sound'] = helpers.name_file_helper(
             'SOUND.BIN',
             'f3_w95.da'
         )
 
         return helpers.build_rom(in_files, func_map)
 
     def _handle_uccops(self, in_files):
         func_map = {}
-        
+
         # maincpu
         maincpu_filenames = [
             'uc_l0.rom', 'uc_l1.rom', 'uc_h0.rom', 'uc_h1.rom'
         ]
+
         def maincpu(in_files):
             contents = in_files['CPU1.BIN']
             contents = transforms.cut(contents, 0, length=0xC0000)
             chunks = transforms.deinterleave(contents, num_ways=2, word_size=1)
-            chunks = transforms.transform_all(chunks, transforms.custom_split, [0x40000, 0x20000])
+            chunks = transforms.transform_all(
+                chunks, transforms.custom_split, [0x40000, 0x20000])
             return dict(zip(maincpu_filenames, chunks))
         func_map['maincpu'] = maincpu
-        
+
         # soundcpu
         soundcpu_filenames = [
             'uc_sl0.rom', 'uc_sh0.rom'
         ]
+
         def soundcpu(in_files):
             contents = in_files['CPU2.BIN']
             chunks = transforms.deinterleave(contents, num_ways=2, word_size=1)
             return dict(zip(soundcpu_filenames, chunks))
         func_map['soundcpu'] = soundcpu
 
         # GFX1
@@ -879,31 +926,34 @@
             'SOUND.BIN',
             'uc_w42.rom'
         )
         return helpers.build_rom(in_files, func_map)
 
     def _handle_uccopsj(self, in_files):
         func_map = {}
-        
+
         # maincpu
         maincpu_filenames = [
             'uc_l0_a.ic39', 'uc_l1_a.ic38', 'uc_h0_a.ic28', 'uc_h1_a.ic27'
         ]
+
         def maincpu(in_files):
             contents = in_files['CPU1.BIN']
             contents = transforms.cut(contents, 0, length=0xC0000)
             chunks = transforms.deinterleave(contents, num_ways=2, word_size=1)
-            chunks = transforms.transform_all(chunks, transforms.custom_split, [0x40000, 0x20000])
+            chunks = transforms.transform_all(
+                chunks, transforms.custom_split, [0x40000, 0x20000])
             return dict(zip(maincpu_filenames, chunks))
         func_map['maincpu'] = maincpu
-        
+
         # soundcpu
         soundcpu_filenames = [
             'uc_sl0.ic31', 'uc_sh0.ic30'
         ]
+
         def soundcpu(in_files):
             contents = in_files['CPU2.BIN']
             chunks = transforms.deinterleave(contents, num_ways=2, word_size=1)
             return dict(zip(soundcpu_filenames, chunks))
         func_map['soundcpu'] = soundcpu
 
         # GFX1
@@ -923,53 +973,59 @@
             'SOUND.BIN',
             'uc_da.bin'
         )
         return helpers.build_rom(in_files, func_map)
 
     def _handle_vigilant(self, in_files):
         func_map = {}
-        
+
         # maincpu
         maincpu_filenames = [
             'g07_c03.bin', 'j07_c04.bin'
         ]
+
         def maincpu(in_files):
             contents = in_files['CPU1.BIN']
             contents = transforms.cut(contents, 0, length=0x80000)
-            chunks = transforms.custom_split(contents, [0x8000, 0x8000, 0x10000])
+            chunks = transforms.custom_split(
+                contents, [0x8000, 0x8000, 0x10000])
             del chunks[1]
             return dict(zip(maincpu_filenames, chunks))
         func_map['maincpu'] = maincpu
-        
+
         # soundcpu
         func_map['soundcpu'] = helpers.name_file_helper(
             'CPU2.BIN',
             'g05_c02.bin'
         )
 
         # GFX1
         def gfx1(in_files):
             filenames = [
                 'f05_c08.bin', 'h05_c09.bin'
             ]
             contents = in_files['GFX1.BIN']
-            contents = gfx_rebuilder.reencode_gfx(contents, self._VIGILANT_TEXT_LAYOUT)
-            chunks = transforms.equal_split(contents, num_chunks=len(filenames))
+            contents = gfx_rebuilder.reencode_gfx(
+                contents, self._VIGILANT_TEXT_LAYOUT)
+            chunks = transforms.equal_split(
+                contents, num_chunks=len(filenames))
             return dict(zip(filenames, chunks))
         func_map['gfx1'] = gfx1
 
         # GFX2
         def gfx2(in_files):
             filenames = [
                 'n07_c12.bin', 'k07_c10.bin', 'o07_c13.bin', 'l07_c11.bin',
                 't07_c16.bin', 'p07_c14.bin', 'v07_c17.bin', 's07_c15.bin'
             ]
             contents = in_files['GFX2.BIN']
-            contents = gfx_rebuilder.reencode_gfx(contents, self._VIGILANT_SPRITE_LAYOUT)
-            chunks = transforms.equal_split(contents, num_chunks=len(filenames))
+            contents = gfx_rebuilder.reencode_gfx(
+                contents, self._VIGILANT_SPRITE_LAYOUT)
+            chunks = transforms.equal_split(
+                contents, num_chunks=len(filenames))
             return dict(zip(filenames, chunks))
         func_map['gfx2'] = gfx2
 
         # GFX3 - BAD
         def gfx3(in_files):
             def vigilant_reorder(src):
                 pages = 4
@@ -988,17 +1044,19 @@
                 return dst
 
             filenames = [
                 'd01_c05.bin', 'e01_c06.bin', 'f01_c07.bin'
             ]
             contents = in_files['GFX_BG.BIN']
             contents = vigilant_reorder(contents)
-            contents = gfx_rebuilder.reencode_gfx(contents, self._VIGILANT_BACK_LAYOUT)
+            contents = gfx_rebuilder.reencode_gfx(
+                contents, self._VIGILANT_BACK_LAYOUT)
             contents = transforms.cut(contents, 0, length=0x30000)
-            chunks = transforms.equal_split(contents, num_chunks=len(filenames))
+            chunks = transforms.equal_split(
+                contents, num_chunks=len(filenames))
             return dict(zip(filenames, chunks))
         func_map['gfx3'] = gfx3
 
         # Samples
         func_map['samples'] = helpers.name_file_helper(
             'SAMPLES.BIN',
             'd04_c01.bin'
@@ -1009,62 +1067,62 @@
             'pal16l8.8r': 0x104,
             'pal16l8.4m': 0x104,
             'pal16l8.1b': 0x104
         })
 
         return helpers.build_rom(in_files, func_map)
 
-
     def _dotemu_reencode_gfx_helper(self, in_file_name, filenames, layout):
         def encode(in_files):
             contents = in_files[in_file_name]
             contents = gfx_rebuilder.reencode_gfx(contents, layout)
-            chunks = transforms.equal_split(contents, num_chunks=len(filenames))
+            chunks = transforms.equal_split(
+                contents, num_chunks=len(filenames))
             return dict(zip(filenames, chunks))
         return encode
 
     _VIGILANT_TEXT_LAYOUT = {
         "width": 8,
         "height": 8,
-        "total": [1,2],
+        "total": [1, 2],
         "planes": 4,
-        "planeoffset": [[1,2], [1,2,4], 0, 4],
-        "xoffset": [0,1,2,3, 64+0,64+1,64+2,64+3],
+        "planeoffset": [[1, 2], [1, 2, 4], 0, 4],
+        "xoffset": [0, 1, 2, 3, 64+0, 64+1, 64+2, 64+3],
         "yoffset": [0*8, 1*8, 2*8, 3*8, 4*8, 5*8, 6*8, 7*8],
         "charincrement": 128
     }
 
     _VIGILANT_SPRITE_LAYOUT = {
         "width": 16,
         "height": 16,
-        "total": [1,2],
+        "total": [1, 2],
         "planes": 4,
-        "planeoffset": [[1,2], [1,2,4], 0, 4],
+        "planeoffset": [[1, 2], [1, 2, 4], 0, 4],
         "xoffset": [
-            0x00*8+0,0x00*8+1,0x00*8+2,0x00*8+3,
-            0x10*8+0,0x10*8+1,0x10*8+2,0x10*8+3,
-            0x20*8+0,0x20*8+1,0x20*8+2,0x20*8+3,
-            0x30*8+0,0x30*8+1,0x30*8+2,0x30*8+3
+            0x00*8+0, 0x00*8+1, 0x00*8+2, 0x00*8+3,
+            0x10*8+0, 0x10*8+1, 0x10*8+2, 0x10*8+3,
+            0x20*8+0, 0x20*8+1, 0x20*8+2, 0x20*8+3,
+            0x30*8+0, 0x30*8+1, 0x30*8+2, 0x30*8+3
         ],
         "yoffset": [
             0x00*8, 0x01*8, 0x02*8, 0x03*8,
             0x04*8, 0x05*8, 0x06*8, 0x07*8,
             0x08*8, 0x09*8, 0x0A*8, 0x0B*8,
             0x0C*8, 0x0D*8, 0x0E*8, 0x0F*8
         ],
         "charincrement": 0x40*8
     }
 
     _VIGILANT_BACK_LAYOUT = {
         "width": 32,
         "height": 1,
-        "total": [1,1],
+        "total": [1, 1],
         "planes": 4,
-        "planeoffset": [0,2,4,6],
+        "planeoffset": [0, 2, 4, 6],
         "xoffset": [
             0*8+1, 0*8,  1*8+1, 1*8, 2*8+1, 2*8, 3*8+1, 3*8, 4*8+1, 4*8, 5*8+1, 5*8,
-            6*8+1,6*8, 7*8+1,7*8, 8*8+1,8*8, 9*8+1,9*8, 10*8+1,10*8, 11*8+1,11*8,
+            6*8+1, 6*8, 7*8+1, 7*8, 8*8+1, 8*8, 9*8+1, 9*8, 10*8+1, 10*8, 11*8+1, 11*8,
             12*8+1, 12*8, 13*8+1, 13*8, 14*8+1, 14*8, 15*8+1, 15*8
         ],
         "yoffset": [0],
         "charincrement": 16*8
-    }
+    }
```

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/irem/metadata.json` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/irem/metadata.json`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/mkak/__init__.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/mkak/__init__.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/mmlc1/__init__.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/mmlc1/__init__.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/mmlc1/metadata.json` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/mmlc1/metadata.json`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/mmxlc1/__init__.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/mmxlc1/__init__.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/mmxlc1/metadata.json` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/mmxlc1/metadata.json`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/neogeo_classics_humble/__init__.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/neogeo_classics_humble/__init__.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/neogeo_classics_humble/metadata.json` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/neogeo_classics_humble/metadata.json`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/pacmanmplus/__init__.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/pacmanmplus/__init__.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/pacmanmplus/metadata.json` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/pacmanmplus/metadata.json`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/psikyo/__init__.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/psikyo/__init__.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/sadxgg/__init__.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/sadxgg/__init__.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/sadxgg/metadata.json` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/sadxgg/metadata.json`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/saga/__init__.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/saga/__init__.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/saga/metadata.json` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/saga/metadata.json`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/sf30ac/__init__.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/sf30ac/__init__.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/sf30ac/metadata.json` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/sf30ac/metadata.json`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/snk40/__init__.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/snk40/__init__.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/snk40/arcadedlc.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/snk40/arcadedlc.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/snk40/arcademain.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/snk40/arcademain.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/snk40/arcadepatch.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/snk40/arcadepatch.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/snk40/metadata.json` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/snk40/metadata.json`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/snk40/nes.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/snk40/nes.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/snk40/utils.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/snk40/utils.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/spp_columnsiii/__init__.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/spp_columnsiii/__init__.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/spp_columnsiii/metadata.json` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/spp_columnsiii/metadata.json`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/spp_drmbm/__init__.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/spp_drmbm/__init__.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/spp_drmbm/metadata.json` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/spp_drmbm/metadata.json`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ssp1/__init__.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ssp1/__init__.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ssp1/metadata.json` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ssp1/metadata.json`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ssp2/__init__.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ssp2/__init__.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/ssp2/metadata.json` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/ssp2/metadata.json`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/wonderboy3/__init__.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/wonderboy3/__init__.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/wonderboy3/metadata.json` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/wonderboy3/metadata.json`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/zamn/__init__.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/zamn/__init__.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/impl/zamn/metadata.json` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/impl/zamn/metadata.json`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/splicetask.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/splicetask.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/tasks/zipsplicetask.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/tasks/zipsplicetask.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/utils/blob/transforms.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/utils/blob/transforms.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/utils/gfx_rebuilder.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/utils/gfx_rebuilder.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/utils/helper.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/utils/helper.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/utils/vendor/capcom.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/utils/vendor/capcom.py`

 * *Files identical despite different names*

### Comparing `game-extraction-toolbox-0.1.6/src/gex/lib/utils/verify.py` & `game-extraction-toolbox-0.1.7/src/gex/lib/utils/verify.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,42 +54,42 @@
 
     # Compare each file size/CRC
     check_files = real_filenames.intersection(expected_filenames)
     for inner_filename in check_files:
         zip_meta = zip_metas.get(inner_filename)
         verify_entry = known_entries[inner_filename]
         if zip_meta['crc'] != verify_entry['crc']:
-            errors.append({VerifyErrors.CHECKSUM_MISMATCH, {zip_meta['crc'], verify_entry['crc'], "CRC", inner_filename}})
+            errors.append((VerifyErrors.CHECKSUM_MISMATCH, {zip_meta['crc'], verify_entry['crc'], "CRC", inner_filename}))
         if zip_meta['size'] != verify_entry['size']:
-            errors.append({VerifyErrors.SIZE_MISMATCH, {zip_meta['size'], verify_entry['size'], inner_filename}})
+            errors.append((VerifyErrors.SIZE_MISMATCH, {zip_meta['size'], verify_entry['size'], inner_filename}))
             
     return errors
 
 def verify_crc(contents, known_crc, known_size):
     size = len(contents)
     crc = hash_helper.get_crc(contents)
     known_crc = hex(int(known_crc, base=16))
     errors = []
     if known_size != size:
-        errors.append({VerifyErrors.SIZE_MISMATCH, {size, known_size}})
+        errors.append((VerifyErrors.SIZE_MISMATCH, {size, known_size}))
 
     if known_crc != crc:
-        errors.append({VerifyErrors.CHECKSUM_MISMATCH, {crc, known_crc, "CRC"}})
+        errors.append((VerifyErrors.CHECKSUM_MISMATCH, {crc, known_crc, "CRC"}))
 
     return errors
 
 def verify_sha(contents, known_sha, known_size):
     size = len(contents)
     sha = hash_helper.get_sha1(contents)
     errors = []
     if known_size != size:
-        errors.append({VerifyErrors.SIZE_MISMATCH, {size, known_size}})
+        errors.append((VerifyErrors.SIZE_MISMATCH, {size, known_size}))
 
     if known_sha != sha:
-        errors.append({VerifyErrors.CHECKSUM_MISMATCH, {sha, known_sha, "SHA-1"}})
+        errors.append((VerifyErrors.CHECKSUM_MISMATCH, {sha, known_sha, "SHA-1"}))
 
     return errors
 
 def print_errors(errors, ref):
     logger.info(f"Verification of {ref} failed!")
     for error in errors:
         message = ""
```

### Comparing `game-extraction-toolbox-0.1.6/src/gex/toolbox.py` & `game-extraction-toolbox-0.1.7/src/gex/toolbox.py`

 * *Files identical despite different names*

