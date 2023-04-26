# Comparing `tmp/feed-archiver-2.0.2.tar.gz` & `tmp/feed-archiver-2.0.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feed-archiver-2.0.2.tar", last modified: Wed Apr 26 02:25:45 2023, max compression
+gzip compressed data, was "feed-archiver-2.0.2b0.tar", last modified: Wed Apr 26 01:35:35 2023, max compression
```

## Comparing `feed-archiver-2.0.2.tar` & `feed-archiver-2.0.2b0.tar`

### file list

```diff
@@ -1,250 +1,250 @@
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.723037 feed-archiver-2.0.2/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      543 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/.dir-locals.el.in
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1733 2023-04-26 00:51:45.000000 feed-archiver-2.0.2/.dockerignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1150 2023-04-26 00:51:45.000000 feed-archiver-2.0.2/.env.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.711037 feed-archiver-2.0.2/.github/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/.github/workflows/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3944 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/.github/workflows/build-test.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1733 2023-04-26 00:51:45.000000 feed-archiver-2.0.2/.gitignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4347 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/.gitlab-ci.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      777 2023-04-26 00:51:45.000000 feed-archiver-2.0.2/.pre-commit-config.yaml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2442 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/.prospector.yaml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4121 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/CONTRIBUTING.rst
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2481 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/Dockerfile
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3218 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/Dockerfile.devel
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1081 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/LICENSE
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    60325 2023-04-26 00:51:45.000000 feed-archiver-2.0.2/Makefile
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)       92 2023-04-26 01:45:50.000000 feed-archiver-2.0.2/NEWS-VERSION.rst
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     4124 2023-04-26 01:45:50.000000 feed-archiver-2.0.2/NEWS.rst
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    25651 2023-04-26 02:25:45.723037 feed-archiver-2.0.2/PKG-INFO
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    24565 2023-04-26 00:51:45.000000 feed-archiver-2.0.2/README.rst
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3758 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/TODO.rst
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/bin/
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     2759 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/bin/cz-check-bump
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)      936 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/bin/entrypoint
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     1101 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/bin/get-base-version
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)      321 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/bin/hadolint
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/build-host/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2002 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/build-host/Dockerfile
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1476 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/build-host/Makefile
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      746 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/build-host/README.rst
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/build-host/bin/
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     2047 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/build-host/bin/entrypoint
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      730 2023-04-26 01:44:54.000000 feed-archiver-2.0.2/build-host/requirements-py310.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      673 2023-04-26 01:44:54.000000 feed-archiver-2.0.2/build-host/requirements-py311.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      947 2023-04-26 01:44:54.000000 feed-archiver-2.0.2/build-host/requirements-py37.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      728 2023-04-26 01:44:54.000000 feed-archiver-2.0.2/build-host/requirements-py38.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      728 2023-04-26 01:44:54.000000 feed-archiver-2.0.2/build-host/requirements-py39.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)        4 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/build-host/requirements.txt.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/dist/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      122 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/dist/.gitignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      954 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/docker-compose-servarr.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5769 2023-04-26 00:51:45.000000 feed-archiver-2.0.2/docker-compose.override.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      945 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/docker-compose.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/gitlab-runner/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/gitlab-runner/config/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1323 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/gitlab-runner/config/config.toml.in
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      566 2023-04-26 00:51:45.000000 feed-archiver-2.0.2/gitlab-runner/docker-compose.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/home/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       64 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/home/.gitignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      327 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/home/.pypirc.in
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      111 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/link-fallbacks.feature.rst
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.711037 feed-archiver-2.0.2/nginx/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/nginx/templates/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1086 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/nginx/templates/default.conf.template
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     2938 2023-04-26 01:45:50.000000 feed-archiver-2.0.2/pyproject.toml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/requirements/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      668 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/requirements/build.txt.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/requirements/py310/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2567 2023-04-26 00:51:45.000000 feed-archiver-2.0.2/requirements/py310/build.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6246 2023-04-26 01:44:54.000000 feed-archiver-2.0.2/requirements/py310/devel.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1140 2023-04-26 01:44:54.000000 feed-archiver-2.0.2/requirements/py310/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/requirements/py311/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2529 2023-04-26 00:51:45.000000 feed-archiver-2.0.2/requirements/py311/build.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6020 2023-04-26 01:44:54.000000 feed-archiver-2.0.2/requirements/py311/devel.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1140 2023-04-26 01:44:54.000000 feed-archiver-2.0.2/requirements/py311/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/requirements/py37/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2840 2023-04-26 00:51:45.000000 feed-archiver-2.0.2/requirements/py37/build.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6936 2023-04-26 01:44:54.000000 feed-archiver-2.0.2/requirements/py37/devel.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1487 2023-04-26 01:44:54.000000 feed-archiver-2.0.2/requirements/py37/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/requirements/py38/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2668 2023-04-26 00:51:45.000000 feed-archiver-2.0.2/requirements/py38/build.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6286 2023-04-26 01:44:54.000000 feed-archiver-2.0.2/requirements/py38/devel.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1138 2023-04-26 01:44:54.000000 feed-archiver-2.0.2/requirements/py38/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/requirements/py39/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2565 2023-04-26 00:51:45.000000 feed-archiver-2.0.2/requirements/py39/build.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6273 2023-04-26 01:44:54.000000 feed-archiver-2.0.2/requirements/py39/devel.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1138 2023-04-26 01:44:54.000000 feed-archiver-2.0.2/requirements/py39/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/server/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4397 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/server/docker-compose.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2152 2023-04-26 02:25:45.723037 feed-archiver-2.0.2/setup.cfg
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feed_archiver.egg-info/
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    25651 2023-04-26 02:25:45.000000 feed-archiver-2.0.2/src/feed_archiver.egg-info/PKG-INFO
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     7317 2023-04-26 02:25:45.000000 feed-archiver-2.0.2/src/feed_archiver.egg-info/SOURCES.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)        1 2023-04-26 02:25:45.000000 feed-archiver-2.0.2/src/feed_archiver.egg-info/dependency_links.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      277 2023-04-26 02:25:45.000000 feed-archiver-2.0.2/src/feed_archiver.egg-info/entry_points.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      345 2023-04-26 02:25:45.000000 feed-archiver-2.0.2/src/feed_archiver.egg-info/requires.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)       13 2023-04-26 02:25:45.000000 feed-archiver-2.0.2/src/feed_archiver.egg-info/top_level.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5287 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/__init__.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      201 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/__main__.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    11802 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/archive.py
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/enclosures/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3371 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/enclosures/__init__.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     8155 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/enclosures/servarr.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1968 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/enclosures/template.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    34925 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/feed.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7074 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/formats.py
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/newsfragments/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       91 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/newsfragments/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     9888 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/__init__.py
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/archives/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/archives/downloads/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1349 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/archives/downloads/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/archives/empty/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       32 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/archives/empty/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/archives/empty-feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       60 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/archives/empty-feeds/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/archives/empty-items/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      337 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/archives/empty-items/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/archives/end-to-end/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      962 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/archives/relink/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      936 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/archives/relink/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/archives/relink-wo-suffix/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      932 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/archives/relink-wo-suffix/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/archives/simple/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      228 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/archives/simple/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      243 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episode%3Fapikey=secret%26seriesId=7
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      224 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episodeFile%3Fapikey=secret%26seriesId=7
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       91 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/7%3Fapikey=secret
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      105 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series%3Fapikey=secret
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/download.mp3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/index.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3435 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/download.mp3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5617 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3435 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/empty-items/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/empty-items/orig/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/empty-items/orig/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/podcast/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      405 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/podcast/empty.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/added-item/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/added-item/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/added-item/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1186 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/empty/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/empty/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/empty/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       92 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/orig/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/orig/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/orig/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      831 1980-11-25 08:31:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/removed-item/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/removed-item/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/removed-item/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      841 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/reordered-item/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/reordered-item/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.719037 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/reordered-item/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.723037 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1550 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.715036 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 02:25:45.723037 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3286 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/test_archive.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4257 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/test_cli.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    10833 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/test_download.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    15051 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/test_feed.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7436 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/test_linking.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2165 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/tests/test_urls.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     8147 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/src/feedarchiver/utils.py
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      160 2023-04-26 02:25:45.000000 feed-archiver-2.0.2/src/feedarchiver/version.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3368 2023-04-24 06:43:00.000000 feed-archiver-2.0.2/tox.ini
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      543 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/.dir-locals.el.in
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1733 2023-04-26 00:51:45.000000 feed-archiver-2.0.2b0/.dockerignore
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1150 2023-04-26 00:51:45.000000 feed-archiver-2.0.2b0/.env.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.178572 feed-archiver-2.0.2b0/.github/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.186572 feed-archiver-2.0.2b0/.github/workflows/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3944 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/.github/workflows/build-test.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1733 2023-04-26 00:51:45.000000 feed-archiver-2.0.2b0/.gitignore
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4347 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/.gitlab-ci.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      777 2023-04-26 00:51:45.000000 feed-archiver-2.0.2b0/.pre-commit-config.yaml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2442 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/.prospector.yaml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4121 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/CONTRIBUTING.rst
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2481 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/Dockerfile
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3218 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/Dockerfile.devel
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1081 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/LICENSE
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    60325 2023-04-26 00:51:45.000000 feed-archiver-2.0.2b0/Makefile
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      180 2023-04-26 00:57:06.000000 feed-archiver-2.0.2b0/NEWS-VERSION.rst
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4031 2023-04-26 00:57:11.000000 feed-archiver-2.0.2b0/NEWS.rst
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    25653 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/PKG-INFO
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    24565 2023-04-26 00:51:45.000000 feed-archiver-2.0.2b0/README.rst
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3758 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/TODO.rst
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.186572 feed-archiver-2.0.2b0/bin/
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     2759 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/bin/cz-check-bump
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)      936 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/bin/entrypoint
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     1101 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/bin/get-base-version
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)      321 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/bin/hadolint
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.186572 feed-archiver-2.0.2b0/build-host/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2002 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/build-host/Dockerfile
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1476 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/build-host/Makefile
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      746 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/build-host/README.rst
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.186572 feed-archiver-2.0.2b0/build-host/bin/
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     2047 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/build-host/bin/entrypoint
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      730 2023-04-26 00:57:13.000000 feed-archiver-2.0.2b0/build-host/requirements-py310.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      673 2023-04-26 00:57:13.000000 feed-archiver-2.0.2b0/build-host/requirements-py311.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      947 2023-04-26 00:57:13.000000 feed-archiver-2.0.2b0/build-host/requirements-py37.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      728 2023-04-26 00:57:13.000000 feed-archiver-2.0.2b0/build-host/requirements-py38.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      728 2023-04-26 00:57:13.000000 feed-archiver-2.0.2b0/build-host/requirements-py39.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)        4 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/build-host/requirements.txt.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.186572 feed-archiver-2.0.2b0/dist/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      122 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/dist/.gitignore
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      954 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/docker-compose-servarr.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5769 2023-04-26 00:51:45.000000 feed-archiver-2.0.2b0/docker-compose.override.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      945 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/docker-compose.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.186572 feed-archiver-2.0.2b0/gitlab-runner/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.186572 feed-archiver-2.0.2b0/gitlab-runner/config/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1323 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/gitlab-runner/config/config.toml.in
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      566 2023-04-26 00:51:45.000000 feed-archiver-2.0.2b0/gitlab-runner/docker-compose.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.186572 feed-archiver-2.0.2b0/home/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       64 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/home/.gitignore
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      327 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/home/.pypirc.in
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      111 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/link-fallbacks.feature.rst
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.178572 feed-archiver-2.0.2b0/nginx/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.186572 feed-archiver-2.0.2b0/nginx/templates/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1086 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/nginx/templates/default.conf.template
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2940 2023-04-26 00:57:13.000000 feed-archiver-2.0.2b0/pyproject.toml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.186572 feed-archiver-2.0.2b0/requirements/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      668 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/requirements/build.txt.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.186572 feed-archiver-2.0.2b0/requirements/py310/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2567 2023-04-26 00:51:45.000000 feed-archiver-2.0.2b0/requirements/py310/build.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6246 2023-04-26 00:57:13.000000 feed-archiver-2.0.2b0/requirements/py310/devel.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1140 2023-04-26 00:57:13.000000 feed-archiver-2.0.2b0/requirements/py310/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.186572 feed-archiver-2.0.2b0/requirements/py311/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2529 2023-04-26 00:51:45.000000 feed-archiver-2.0.2b0/requirements/py311/build.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6020 2023-04-26 00:57:13.000000 feed-archiver-2.0.2b0/requirements/py311/devel.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1140 2023-04-26 00:57:13.000000 feed-archiver-2.0.2b0/requirements/py311/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.186572 feed-archiver-2.0.2b0/requirements/py37/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2840 2023-04-26 00:51:45.000000 feed-archiver-2.0.2b0/requirements/py37/build.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6936 2023-04-26 00:57:13.000000 feed-archiver-2.0.2b0/requirements/py37/devel.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1487 2023-04-26 00:57:13.000000 feed-archiver-2.0.2b0/requirements/py37/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.186572 feed-archiver-2.0.2b0/requirements/py38/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2668 2023-04-26 00:51:45.000000 feed-archiver-2.0.2b0/requirements/py38/build.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6286 2023-04-26 00:57:13.000000 feed-archiver-2.0.2b0/requirements/py38/devel.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1138 2023-04-26 00:57:13.000000 feed-archiver-2.0.2b0/requirements/py38/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/requirements/py39/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2565 2023-04-26 00:51:45.000000 feed-archiver-2.0.2b0/requirements/py39/build.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6273 2023-04-26 00:57:13.000000 feed-archiver-2.0.2b0/requirements/py39/devel.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1138 2023-04-26 00:57:13.000000 feed-archiver-2.0.2b0/requirements/py39/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/server/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4397 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/server/docker-compose.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2152 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/setup.cfg
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.178572 feed-archiver-2.0.2b0/src/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feed_archiver.egg-info/
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    25653 2023-04-26 01:35:35.000000 feed-archiver-2.0.2b0/src/feed_archiver.egg-info/PKG-INFO
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     7317 2023-04-26 01:35:35.000000 feed-archiver-2.0.2b0/src/feed_archiver.egg-info/SOURCES.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)        1 2023-04-26 01:35:35.000000 feed-archiver-2.0.2b0/src/feed_archiver.egg-info/dependency_links.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      277 2023-04-26 01:35:35.000000 feed-archiver-2.0.2b0/src/feed_archiver.egg-info/entry_points.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      345 2023-04-26 01:35:35.000000 feed-archiver-2.0.2b0/src/feed_archiver.egg-info/requires.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)       13 2023-04-26 01:35:35.000000 feed-archiver-2.0.2b0/src/feed_archiver.egg-info/top_level.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5287 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/__init__.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      201 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/__main__.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    11802 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/archive.py
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/enclosures/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3371 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/enclosures/__init__.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     8155 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/enclosures/servarr.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1968 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/enclosures/template.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    34925 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/feed.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7074 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/formats.py
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/newsfragments/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       91 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/newsfragments/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/tests/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     9888 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/__init__.py
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/downloads/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1349 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/downloads/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/empty/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       32 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/empty/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/empty-feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       60 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/empty-feeds/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/empty-items/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      337 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/empty-items/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/end-to-end/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      962 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/relink/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      936 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/relink/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/relink-wo-suffix/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      932 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/relink-wo-suffix/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/simple/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      228 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/simple/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      243 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episode%3Fapikey=secret%26seriesId=7
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      224 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episodeFile%3Fapikey=secret%26seriesId=7
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       91 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/7%3Fapikey=secret
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      105 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series%3Fapikey=secret
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/download.mp3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/index.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3435 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/download.mp3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5617 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3435 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/empty-items/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/empty-items/orig/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/empty-items/orig/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/podcast/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      405 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/podcast/empty.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1186 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       92 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      831 1980-11-25 08:31:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      841 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1550 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3286 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/test_archive.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4257 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/test_cli.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    10833 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/test_download.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    15051 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/test_feed.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7436 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/test_linking.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2165 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/test_urls.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     8147 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/utils.py
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      162 2023-04-26 01:35:35.000000 feed-archiver-2.0.2b0/src/feedarchiver/version.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3368 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/tox.ini
```

### Comparing `feed-archiver-2.0.2/.dir-locals.el.in` & `feed-archiver-2.0.2b0/.dir-locals.el.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/.dockerignore` & `feed-archiver-2.0.2b0/.dockerignore`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/.env.in` & `feed-archiver-2.0.2b0/.env.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/.github/workflows/build-test.yml` & `feed-archiver-2.0.2b0/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/.gitignore` & `feed-archiver-2.0.2b0/.gitignore`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/.gitlab-ci.yml` & `feed-archiver-2.0.2b0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/.pre-commit-config.yaml` & `feed-archiver-2.0.2b0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/.prospector.yaml` & `feed-archiver-2.0.2b0/.prospector.yaml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/CONTRIBUTING.rst` & `feed-archiver-2.0.2b0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/Dockerfile` & `feed-archiver-2.0.2b0/Dockerfile`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/Dockerfile.devel` & `feed-archiver-2.0.2b0/Dockerfile.devel`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/LICENSE` & `feed-archiver-2.0.2b0/LICENSE`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/Makefile` & `feed-archiver-2.0.2b0/Makefile`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/NEWS.rst` & `feed-archiver-2.0.2b0/NEWS.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-feed-archiver 2.0.2 (2023-04-26)
-================================
-
-No significant changes.
-
-
 feed-archiver 2.0.2b0 (2023-04-26)
 ==================================
 
 Bugfixes
 --------
 
 - Upgrade all requirements to the latest versions as of Tue Apr 25 11:00:28 PM UTC 2023.
```

### Comparing `feed-archiver-2.0.2/PKG-INFO` & `feed-archiver-2.0.2b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feed-archiver
-Version: 2.0.2
+Version: 2.0.2b0
 Summary: Archive the full contents of RSS/Atom syndication feeds including enclosures and assets.
 Home-page: https://gitlab.com/rpatterson/feed-archiver
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: feeds,syndication,rss,atom,podcasts,enclosures
 Classifier: Development Status :: 4 - Beta
```

### Comparing `feed-archiver-2.0.2/README.rst` & `feed-archiver-2.0.2b0/README.rst`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/TODO.rst` & `feed-archiver-2.0.2b0/TODO.rst`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/bin/cz-check-bump` & `feed-archiver-2.0.2b0/bin/cz-check-bump`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/bin/entrypoint` & `feed-archiver-2.0.2b0/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/bin/get-base-version` & `feed-archiver-2.0.2b0/bin/get-base-version`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/build-host/Dockerfile` & `feed-archiver-2.0.2b0/build-host/Dockerfile`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/build-host/Makefile` & `feed-archiver-2.0.2b0/build-host/Makefile`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/build-host/README.rst` & `feed-archiver-2.0.2b0/build-host/README.rst`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/build-host/bin/entrypoint` & `feed-archiver-2.0.2b0/build-host/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/build-host/requirements-py310.txt` & `feed-archiver-2.0.2b0/build-host/requirements-py310.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/build-host/requirements-py311.txt` & `feed-archiver-2.0.2b0/build-host/requirements-py311.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/build-host/requirements-py37.txt` & `feed-archiver-2.0.2b0/build-host/requirements-py37.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/build-host/requirements-py38.txt` & `feed-archiver-2.0.2b0/build-host/requirements-py38.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/build-host/requirements-py39.txt` & `feed-archiver-2.0.2b0/build-host/requirements-py39.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/docker-compose-servarr.yml` & `feed-archiver-2.0.2b0/docker-compose-servarr.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/docker-compose.override.yml` & `feed-archiver-2.0.2b0/docker-compose.override.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/docker-compose.yml` & `feed-archiver-2.0.2b0/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/gitlab-runner/config/config.toml.in` & `feed-archiver-2.0.2b0/gitlab-runner/config/config.toml.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/gitlab-runner/docker-compose.yml` & `feed-archiver-2.0.2b0/gitlab-runner/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/nginx/templates/default.conf.template` & `feed-archiver-2.0.2b0/nginx/templates/default.conf.template`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/pyproject.toml` & `feed-archiver-2.0.2b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 [tool.commitizen]
 # Parse commit messages according to conventional commits to decide wether the next
 # versin tag should be a major, minor or patch bump and create the VCS tag.  Also
 # provides VCS hooks to enforce that commit messages comply with conventional commits:
 # https://commitizen-tools.github.io/commitizen/
 name = "cz_conventional_commits"
 changelog_start_rev = "v0.0.0"
-version = "2.0.2"
+version = "2.0.2b0"
 tag_format = "v$version"
 annotated_tag = true
 gpg_sign = true
 bump_message = """\
 build(release): Version $current_version → $new_version
 
 [actions skip]
```

### Comparing `feed-archiver-2.0.2/requirements/build.txt.in` & `feed-archiver-2.0.2b0/requirements/build.txt.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/requirements/py310/build.txt` & `feed-archiver-2.0.2b0/requirements/py310/build.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/requirements/py310/devel.txt` & `feed-archiver-2.0.2b0/requirements/py310/devel.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/requirements/py310/user.txt` & `feed-archiver-2.0.2b0/requirements/py310/user.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/requirements/py311/build.txt` & `feed-archiver-2.0.2b0/requirements/py311/build.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/requirements/py311/devel.txt` & `feed-archiver-2.0.2b0/requirements/py311/devel.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/requirements/py311/user.txt` & `feed-archiver-2.0.2b0/requirements/py311/user.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/requirements/py37/build.txt` & `feed-archiver-2.0.2b0/requirements/py37/build.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/requirements/py37/devel.txt` & `feed-archiver-2.0.2b0/requirements/py37/devel.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/requirements/py37/user.txt` & `feed-archiver-2.0.2b0/requirements/py37/user.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/requirements/py38/build.txt` & `feed-archiver-2.0.2b0/requirements/py38/build.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/requirements/py38/devel.txt` & `feed-archiver-2.0.2b0/requirements/py38/devel.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/requirements/py38/user.txt` & `feed-archiver-2.0.2b0/requirements/py38/user.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/requirements/py39/build.txt` & `feed-archiver-2.0.2b0/requirements/py39/build.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/requirements/py39/devel.txt` & `feed-archiver-2.0.2b0/requirements/py39/devel.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/requirements/py39/user.txt` & `feed-archiver-2.0.2b0/requirements/py39/user.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/server/docker-compose.yml` & `feed-archiver-2.0.2b0/server/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/setup.cfg` & `feed-archiver-2.0.2b0/setup.cfg`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feed_archiver.egg-info/PKG-INFO` & `feed-archiver-2.0.2b0/src/feed_archiver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feed-archiver
-Version: 2.0.2
+Version: 2.0.2b0
 Summary: Archive the full contents of RSS/Atom syndication feeds including enclosures and assets.
 Home-page: https://gitlab.com/rpatterson/feed-archiver
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: feeds,syndication,rss,atom,podcasts,enclosures
 Classifier: Development Status :: 4 - Beta
```

### Comparing `feed-archiver-2.0.2/src/feed_archiver.egg-info/SOURCES.txt` & `feed-archiver-2.0.2b0/src/feed_archiver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/__init__.py` & `feed-archiver-2.0.2b0/src/feedarchiver/__init__.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/archive.py` & `feed-archiver-2.0.2b0/src/feedarchiver/archive.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/enclosures/__init__.py` & `feed-archiver-2.0.2b0/src/feedarchiver/enclosures/__init__.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/enclosures/servarr.py` & `feed-archiver-2.0.2b0/src/feedarchiver/enclosures/servarr.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/enclosures/template.py` & `feed-archiver-2.0.2b0/src/feedarchiver/enclosures/template.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/feed.py` & `feed-archiver-2.0.2b0/src/feedarchiver/feed.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/formats.py` & `feed-archiver-2.0.2b0/src/feedarchiver/formats.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/__init__.py` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/archives/downloads/.feed-archiver.yml` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/downloads/.feed-archiver.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/archives/relink/.feed-archiver.yml` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/relink/.feed-archiver.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/archives/relink-wo-suffix/.feed-archiver.yml` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/relink-wo-suffix/.feed-archiver.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/download.mp3` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/download.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/index.html` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/index.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/download.mp3` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/download.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/test_archive.py` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/test_cli.py` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/test_download.py` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/test_feed.py` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/test_feed.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/test_linking.py` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/test_linking.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/tests/test_urls.py` & `feed-archiver-2.0.2b0/src/feedarchiver/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/src/feedarchiver/utils.py` & `feed-archiver-2.0.2b0/src/feedarchiver/utils.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2/tox.ini` & `feed-archiver-2.0.2b0/tox.ini`

 * *Files identical despite different names*

