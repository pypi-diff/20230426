# Comparing `tmp/prunerr-1.1.5.tar.gz` & `tmp/prunerr-1.1.5b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prunerr-1.1.5.tar", last modified: Wed Apr 26 01:44:14 2023, max compression
+gzip compressed data, was "prunerr-1.1.5b0.tar", last modified: Wed Apr 26 00:39:41 2023, max compression
```

## Comparing `prunerr-1.1.5.tar` & `prunerr-1.1.5b0.tar`

### file list

```diff
@@ -1,1374 +1,1374 @@
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.824174 prunerr-1.1.5/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      543 2023-04-25 04:48:04.000000 prunerr-1.1.5/.dir-locals.el.in
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1557 2023-04-25 04:48:04.000000 prunerr-1.1.5/.dockerignore
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1261 2023-04-25 04:48:04.000000 prunerr-1.1.5/.env.in
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.744173 prunerr-1.1.5/.github/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.784174 prunerr-1.1.5/.github/workflows/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3938 2023-04-25 04:48:04.000000 prunerr-1.1.5/.github/workflows/build-test.yml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1557 2023-04-25 04:48:04.000000 prunerr-1.1.5/.gitignore
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4341 2023-04-25 04:48:04.000000 prunerr-1.1.5/.gitlab-ci.yml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      777 2023-04-26 00:16:52.000000 prunerr-1.1.5/.pre-commit-config.yaml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2448 2023-04-25 04:48:04.000000 prunerr-1.1.5/.prospector.yaml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4109 2023-04-25 04:48:04.000000 prunerr-1.1.5/CONTRIBUTING.rst
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2429 2023-04-25 04:48:04.000000 prunerr-1.1.5/Dockerfile
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3224 2023-04-25 04:48:04.000000 prunerr-1.1.5/Dockerfile.devel
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1081 2023-04-25 04:48:04.000000 prunerr-1.1.5/LICENSE
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    58287 2023-04-26 00:16:52.000000 prunerr-1.1.5/Makefile
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       80 2023-04-26 00:48:12.000000 prunerr-1.1.5/NEWS-VERSION.rst
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5092 2023-04-26 00:48:12.000000 prunerr-1.1.5/NEWS.rst
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)    17773 2023-04-26 01:44:14.824174 prunerr-1.1.5/PKG-INFO
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    16788 2023-04-25 06:38:28.000000 prunerr-1.1.5/README.rst
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5038 2023-04-25 04:48:04.000000 prunerr-1.1.5/TODO.rst
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.784174 prunerr-1.1.5/bin/
--rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     2759 2023-04-25 04:48:04.000000 prunerr-1.1.5/bin/cz-check-bump
--rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)      918 2023-04-25 04:48:04.000000 prunerr-1.1.5/bin/entrypoint
--rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     1101 2023-04-25 04:48:04.000000 prunerr-1.1.5/bin/get-base-version
--rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)      321 2023-04-25 04:48:04.000000 prunerr-1.1.5/bin/hadolint
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.784174 prunerr-1.1.5/build-host/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1994 2023-04-25 04:48:04.000000 prunerr-1.1.5/build-host/Dockerfile
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1464 2023-04-25 04:48:04.000000 prunerr-1.1.5/build-host/Makefile
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      746 2023-04-25 04:48:04.000000 prunerr-1.1.5/build-host/README.rst
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.784174 prunerr-1.1.5/build-host/bin/
--rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     2041 2023-04-25 04:48:04.000000 prunerr-1.1.5/build-host/bin/entrypoint
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      730 2023-04-26 00:18:06.000000 prunerr-1.1.5/build-host/requirements-py310.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      673 2023-04-26 00:18:06.000000 prunerr-1.1.5/build-host/requirements-py311.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      947 2023-04-26 00:18:06.000000 prunerr-1.1.5/build-host/requirements-py37.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      728 2023-04-26 00:18:06.000000 prunerr-1.1.5/build-host/requirements-py38.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      728 2023-04-26 00:18:06.000000 prunerr-1.1.5/build-host/requirements-py39.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        4 2023-04-25 04:48:04.000000 prunerr-1.1.5/build-host/requirements.txt.in
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.784174 prunerr-1.1.5/dist/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      122 2023-04-25 04:48:04.000000 prunerr-1.1.5/dist/.gitignore
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1397 2023-04-25 04:48:04.000000 prunerr-1.1.5/docker-compose-servarr.yml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5132 2023-04-25 04:48:04.000000 prunerr-1.1.5/docker-compose.override.yml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4047 2023-04-25 04:48:04.000000 prunerr-1.1.5/docker-compose.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.784174 prunerr-1.1.5/gitlab-runner/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.784174 prunerr-1.1.5/gitlab-runner/config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1323 2023-04-25 04:48:04.000000 prunerr-1.1.5/gitlab-runner/config/config.toml.in
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      566 2023-04-25 04:48:04.000000 prunerr-1.1.5/gitlab-runner/docker-compose.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.784174 prunerr-1.1.5/home/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       64 2023-04-25 04:48:04.000000 prunerr-1.1.5/home/.gitignore
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      327 2023-04-25 04:48:04.000000 prunerr-1.1.5/home/.pypirc.in
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3005 2023-04-26 00:48:12.000000 prunerr-1.1.5/pyproject.toml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.784174 prunerr-1.1.5/requirements/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      668 2023-04-25 04:48:04.000000 prunerr-1.1.5/requirements/build.txt.in
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.784174 prunerr-1.1.5/requirements/py310/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2567 2023-04-26 00:16:52.000000 prunerr-1.1.5/requirements/py310/build.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5141 2023-04-26 01:28:06.000000 prunerr-1.1.5/requirements/py310/devel.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      859 2023-04-26 01:27:58.000000 prunerr-1.1.5/requirements/py310/user.txt
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.784174 prunerr-1.1.5/requirements/py311/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2529 2023-04-26 00:16:52.000000 prunerr-1.1.5/requirements/py311/build.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4915 2023-04-26 00:18:06.000000 prunerr-1.1.5/requirements/py311/devel.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      859 2023-04-26 00:18:06.000000 prunerr-1.1.5/requirements/py311/user.txt
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.784174 prunerr-1.1.5/requirements/py37/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2840 2023-04-26 00:16:52.000000 prunerr-1.1.5/requirements/py37/build.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5960 2023-04-26 00:18:06.000000 prunerr-1.1.5/requirements/py37/devel.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1398 2023-04-26 00:18:06.000000 prunerr-1.1.5/requirements/py37/user.txt
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.784174 prunerr-1.1.5/requirements/py38/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2668 2023-04-26 00:16:52.000000 prunerr-1.1.5/requirements/py38/build.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5459 2023-04-26 00:18:06.000000 prunerr-1.1.5/requirements/py38/devel.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1158 2023-04-26 00:18:06.000000 prunerr-1.1.5/requirements/py38/user.txt
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.784174 prunerr-1.1.5/requirements/py39/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2565 2023-04-26 00:16:52.000000 prunerr-1.1.5/requirements/py39/build.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5446 2023-04-26 00:18:06.000000 prunerr-1.1.5/requirements/py39/devel.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1158 2023-04-26 00:18:06.000000 prunerr-1.1.5/requirements/py39/user.txt
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.744173 prunerr-1.1.5/s6/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.744173 prunerr-1.1.5/s6/etc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.744173 prunerr-1.1.5/s6/etc/s6-overlay/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.744173 prunerr-1.1.5/s6/etc/s6-overlay/s6-rc.d/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.784174 prunerr-1.1.5/s6/etc/s6-overlay/s6-rc.d/svc-transmission/
--rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)      243 2023-04-25 04:48:04.000000 prunerr-1.1.5/s6/etc/s6-overlay/s6-rc.d/svc-transmission/finish
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1748 2023-04-26 01:44:14.824174 prunerr-1.1.5/setup.cfg
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.744173 prunerr-1.1.5/src/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.784174 prunerr-1.1.5/src/prunerr/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8429 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/__init__.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      201 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/__main__.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    15438 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/downloadclient.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11377 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/downloaditem.py
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.744173 prunerr-1.1.5/src/prunerr/home/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/home/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    10134 2023-04-25 21:32:47.000000 prunerr-1.1.5/src/prunerr/home/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/newsfragments/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       91 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/newsfragments/.gitignore
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     7937 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/operations.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    19064 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/runner.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11415 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/servarr.py
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/tests/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      911 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/Makefile
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    22019 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/__init__.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    67861 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/example-5s.mkv
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.744173 prunerr-1.1.5/src/prunerr/tests/home/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.744173 prunerr-1.1.5/src/prunerr/tests/home/daemon/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/tests/home/daemon/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3204 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/home/daemon/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.744173 prunerr-1.1.5/src/prunerr/tests/home/download-client-only/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/tests/home/download-client-only/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       90 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/home/download-client-only/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.744173 prunerr-1.1.5/src/prunerr/tests/home/download-clients/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/tests/home/download-clients/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2957 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/home/download-clients/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.744173 prunerr-1.1.5/src/prunerr/tests/home/download-items/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/tests/home/download-items/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       90 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/home/download-items/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.744173 prunerr-1.1.5/src/prunerr/tests/home/empty/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/tests/home/empty/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/home/empty/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.744173 prunerr-1.1.5/src/prunerr/tests/home/move-exec/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/tests/home/move-exec/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       88 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/home/move-exec/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.744173 prunerr-1.1.5/src/prunerr/tests/home/review-edge-cases/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/tests/home/review-edge-cases/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      820 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/home/review-edge-cases/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.780174 prunerr-1.1.5/src/prunerr/tests/responses/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.744173 prunerr-1.1.5/src/prunerr/tests/responses/daemon/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.744173 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.744173 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.744173 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.744173 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.744173 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.744173 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.744173 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.744173 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.744173 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.744173 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:42:39.000000 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1077 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5451 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/default/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/default/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     9537 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:42:39.000000 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1087 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5451 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2086 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/download-client-only/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/download-client-only/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.748173 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    13662 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.792174 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/https/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/download-items/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/download-items/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5081 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.752173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1467 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      126 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1484 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.796174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1467 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.756173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1495 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1498 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.800174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.760173 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.804174 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.764173 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1470 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-import/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1362 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      210 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1362 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.808174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.768173 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      210 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2102 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1470 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1086 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.772174 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.812174 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.816174 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.816174 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:42:39.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.816174 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.816174 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2044 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.816174 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.816174 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.816174 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.816174 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.816174 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    16163 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.816174 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.816174 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.816174 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      148 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.816174 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5383 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.816174 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      148 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.816174 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5495 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.816174 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.816174 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.816174 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.816174 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.816174 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.816174 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.816174 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.816174 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:42:39.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:42:39.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.816174 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2044 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    27061 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       61 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.780174 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.780174 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.776173 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1086 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.780174 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.780174 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.780174 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.780174 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.780174 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.780174 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.780174 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.780174 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.780174 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.780174 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.780174 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.780174 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    10807 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.780174 prunerr-1.1.5/src/prunerr/tests/responses/verify/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.780174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.780174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.780174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.780174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.780174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.780174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.780174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.780174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.780174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.780174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.780174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.780174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.780174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.780174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.780174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.780174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.780174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.780174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2086 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.820174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      123 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.824174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.824174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.824174 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      122 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4730 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/test_cli.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2906 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/test_daemon.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8822 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/test_downloadclient.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3745 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/test_downloaditem.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11350 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/test_free_space.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    17208 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/test_move.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8074 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/test_operations.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    13110 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/test_review.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1468 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/test_runner.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/test_servarr.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1204 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/tests/test_verify.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1374 2023-04-25 04:48:04.000000 prunerr-1.1.5/src/prunerr/utils.py
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)      160 2023-04-26 01:44:14.000000 prunerr-1.1.5/src/prunerr/version.py
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 01:44:14.788174 prunerr-1.1.5/src/prunerr.egg-info/
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)    17773 2023-04-26 01:44:14.000000 prunerr-1.1.5/src/prunerr.egg-info/PKG-INFO
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)    64656 2023-04-26 01:44:14.000000 prunerr-1.1.5/src/prunerr.egg-info/SOURCES.txt
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)        1 2023-04-26 01:44:14.000000 prunerr-1.1.5/src/prunerr.egg-info/dependency_links.txt
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)       41 2023-04-26 01:44:14.000000 prunerr-1.1.5/src/prunerr.egg-info/entry_points.txt
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)      312 2023-04-26 01:44:14.000000 prunerr-1.1.5/src/prunerr.egg-info/requires.txt
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)        8 2023-04-26 01:44:14.000000 prunerr-1.1.5/src/prunerr.egg-info/top_level.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3327 2023-04-25 04:48:04.000000 prunerr-1.1.5/tox.ini
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.268782 prunerr-1.1.5b0/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      543 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/.dir-locals.el.in
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1557 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/.dockerignore
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1261 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/.env.in
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.056779 prunerr-1.1.5b0/.github/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.168780 prunerr-1.1.5b0/.github/workflows/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3938 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/.github/workflows/build-test.yml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1557 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/.gitignore
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4341 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/.gitlab-ci.yml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      777 2023-04-26 00:16:52.000000 prunerr-1.1.5b0/.pre-commit-config.yaml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2448 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/.prospector.yaml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4109 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/CONTRIBUTING.rst
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2429 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/Dockerfile
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3224 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/Dockerfile.devel
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1081 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/LICENSE
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    58287 2023-04-26 00:16:52.000000 prunerr-1.1.5b0/Makefile
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)      168 2023-04-26 00:18:04.000000 prunerr-1.1.5b0/NEWS-VERSION.rst
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)     4939 2023-04-26 00:18:05.000000 prunerr-1.1.5b0/NEWS.rst
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)    17775 2023-04-26 00:39:41.272781 prunerr-1.1.5b0/PKG-INFO
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    16788 2023-04-25 06:38:28.000000 prunerr-1.1.5b0/README.rst
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5038 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/TODO.rst
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.168780 prunerr-1.1.5b0/bin/
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     2759 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/bin/cz-check-bump
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)      918 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/bin/entrypoint
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     1101 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/bin/get-base-version
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)      321 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/bin/hadolint
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.172781 prunerr-1.1.5b0/build-host/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1994 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/build-host/Dockerfile
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1464 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/build-host/Makefile
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      746 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/build-host/README.rst
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.172781 prunerr-1.1.5b0/build-host/bin/
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     2041 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/build-host/bin/entrypoint
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      730 2023-04-26 00:18:06.000000 prunerr-1.1.5b0/build-host/requirements-py310.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      673 2023-04-26 00:18:06.000000 prunerr-1.1.5b0/build-host/requirements-py311.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      947 2023-04-26 00:18:06.000000 prunerr-1.1.5b0/build-host/requirements-py37.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      728 2023-04-26 00:18:06.000000 prunerr-1.1.5b0/build-host/requirements-py38.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      728 2023-04-26 00:18:06.000000 prunerr-1.1.5b0/build-host/requirements-py39.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        4 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/build-host/requirements.txt.in
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.172781 prunerr-1.1.5b0/dist/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      122 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/dist/.gitignore
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1397 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/docker-compose-servarr.yml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5132 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/docker-compose.override.yml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4047 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/docker-compose.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.172781 prunerr-1.1.5b0/gitlab-runner/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.172781 prunerr-1.1.5b0/gitlab-runner/config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1323 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/gitlab-runner/config/config.toml.in
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      566 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/gitlab-runner/docker-compose.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.172781 prunerr-1.1.5b0/home/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       64 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/home/.gitignore
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      327 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/home/.pypirc.in
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)     3007 2023-04-26 00:18:06.000000 prunerr-1.1.5b0/pyproject.toml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.172781 prunerr-1.1.5b0/requirements/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      668 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/requirements/build.txt.in
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.172781 prunerr-1.1.5b0/requirements/py310/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2567 2023-04-26 00:16:52.000000 prunerr-1.1.5b0/requirements/py310/build.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5141 2023-04-26 00:18:06.000000 prunerr-1.1.5b0/requirements/py310/devel.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      859 2023-04-26 00:18:06.000000 prunerr-1.1.5b0/requirements/py310/user.txt
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.172781 prunerr-1.1.5b0/requirements/py311/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2529 2023-04-26 00:16:52.000000 prunerr-1.1.5b0/requirements/py311/build.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4915 2023-04-26 00:18:06.000000 prunerr-1.1.5b0/requirements/py311/devel.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      859 2023-04-26 00:18:06.000000 prunerr-1.1.5b0/requirements/py311/user.txt
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.172781 prunerr-1.1.5b0/requirements/py37/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2840 2023-04-26 00:16:52.000000 prunerr-1.1.5b0/requirements/py37/build.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5960 2023-04-26 00:18:06.000000 prunerr-1.1.5b0/requirements/py37/devel.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1398 2023-04-26 00:18:06.000000 prunerr-1.1.5b0/requirements/py37/user.txt
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.176781 prunerr-1.1.5b0/requirements/py38/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2668 2023-04-26 00:16:52.000000 prunerr-1.1.5b0/requirements/py38/build.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5459 2023-04-26 00:18:06.000000 prunerr-1.1.5b0/requirements/py38/devel.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1158 2023-04-26 00:18:06.000000 prunerr-1.1.5b0/requirements/py38/user.txt
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.176781 prunerr-1.1.5b0/requirements/py39/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2565 2023-04-26 00:16:52.000000 prunerr-1.1.5b0/requirements/py39/build.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5446 2023-04-26 00:18:06.000000 prunerr-1.1.5b0/requirements/py39/devel.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1158 2023-04-26 00:18:06.000000 prunerr-1.1.5b0/requirements/py39/user.txt
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.060779 prunerr-1.1.5b0/s6/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.060779 prunerr-1.1.5b0/s6/etc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.060779 prunerr-1.1.5b0/s6/etc/s6-overlay/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.060779 prunerr-1.1.5b0/s6/etc/s6-overlay/s6-rc.d/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.176781 prunerr-1.1.5b0/s6/etc/s6-overlay/s6-rc.d/svc-transmission/
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)      243 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/s6/etc/s6-overlay/s6-rc.d/svc-transmission/finish
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1748 2023-04-26 00:39:41.272781 prunerr-1.1.5b0/setup.cfg
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.060779 prunerr-1.1.5b0/src/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.176781 prunerr-1.1.5b0/src/prunerr/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8429 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/__init__.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      201 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/__main__.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    15438 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/downloadclient.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11377 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/downloaditem.py
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.060779 prunerr-1.1.5b0/src/prunerr/home/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.180781 prunerr-1.1.5b0/src/prunerr/home/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    10134 2023-04-25 21:32:47.000000 prunerr-1.1.5b0/src/prunerr/home/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.180781 prunerr-1.1.5b0/src/prunerr/newsfragments/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       91 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/newsfragments/.gitignore
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     7937 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/operations.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    19064 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/runner.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11415 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/servarr.py
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.180781 prunerr-1.1.5b0/src/prunerr/tests/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      911 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/Makefile
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    22019 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/__init__.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    67861 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/example-5s.mkv
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.060779 prunerr-1.1.5b0/src/prunerr/tests/home/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.060779 prunerr-1.1.5b0/src/prunerr/tests/home/daemon/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.180781 prunerr-1.1.5b0/src/prunerr/tests/home/daemon/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3204 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/home/daemon/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.060779 prunerr-1.1.5b0/src/prunerr/tests/home/download-client-only/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.180781 prunerr-1.1.5b0/src/prunerr/tests/home/download-client-only/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       90 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/home/download-client-only/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.060779 prunerr-1.1.5b0/src/prunerr/tests/home/download-clients/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.180781 prunerr-1.1.5b0/src/prunerr/tests/home/download-clients/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2957 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/home/download-clients/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.060779 prunerr-1.1.5b0/src/prunerr/tests/home/download-items/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.180781 prunerr-1.1.5b0/src/prunerr/tests/home/download-items/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       90 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/home/download-items/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.060779 prunerr-1.1.5b0/src/prunerr/tests/home/empty/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.184781 prunerr-1.1.5b0/src/prunerr/tests/home/empty/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/home/empty/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.060779 prunerr-1.1.5b0/src/prunerr/tests/home/move-exec/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.184781 prunerr-1.1.5b0/src/prunerr/tests/home/move-exec/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       88 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/home/move-exec/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.060779 prunerr-1.1.5b0/src/prunerr/tests/home/review-edge-cases/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.184781 prunerr-1.1.5b0/src/prunerr/tests/home/review-edge-cases/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      820 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/home/review-edge-cases/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.160781 prunerr-1.1.5b0/src/prunerr/tests/responses/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.064780 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.068780 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.064780 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.064780 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.064780 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.064780 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.184781 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.184781 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.184781 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.064780 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.184781 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.184781 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.184781 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.064780 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.064780 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.184781 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.184781 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.184781 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.064780 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.064780 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.068780 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.064780 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.184781 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.184781 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.184781 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.068780 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.068780 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.184781 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.184781 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:37:42.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.064780 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.184781 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.184781 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1077 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.184781 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.068780 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.068780 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.184781 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.188781 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.188781 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.188781 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.068780 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.068780 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.068780 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.188781 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.188781 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.188781 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5451 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.188781 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.188781 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.068780 prunerr-1.1.5b0/src/prunerr/tests/responses/default/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.072780 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.068780 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.068780 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.072780 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.068780 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.188781 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.188781 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     9537 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.068780 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.188781 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.188781 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.072780 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.072780 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.188781 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.188781 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.072780 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.072780 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.072780 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.072780 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.188781 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.188781 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.072780 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.072780 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.192781 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.192781 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:37:42.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.072780 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.188781 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.192781 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1087 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.072780 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.072780 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.192781 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.192781 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.072780 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.072780 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.072780 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.192781 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.192781 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.192781 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5451 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.192781 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.192781 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2086 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.076780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-client-only/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.076780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-client-only/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.076780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.076780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.076780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.192781 prunerr-1.1.5b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.192781 prunerr-1.1.5b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.192781 prunerr-1.1.5b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.080780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.080780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.076780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.076780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.076780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.192781 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.196781 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.196781 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.076780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.076780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.076780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.076780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.196781 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.196781 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.076780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.196781 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.196781 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.076780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.076780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.196781 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.196781 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.080780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.080780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.080780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.080780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.196781 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.196781 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    13662 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.080780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.196781 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.196781 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.080780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.080780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.196781 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.196781 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.080780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.080780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.080780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.196781 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.200781 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.200781 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.080780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.080780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.080780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.200781 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.200781 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.200781 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.084780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/https/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.080780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.080780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.200781 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.200781 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.200781 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.084780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.084780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.200781 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.200781 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.200781 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.084780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-items/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.084780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-items/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.084780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.084780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.084780 prunerr-1.1.5b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.200781 prunerr-1.1.5b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.200781 prunerr-1.1.5b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.204781 prunerr-1.1.5b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5081 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.084780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.088780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.084780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.084780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.084780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.084780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.204781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.204781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.084780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.204781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.204781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.084780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.084780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.204781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.204781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.084780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.088780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.088780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.088780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.204781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.204781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.088780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.204781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.204781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.088780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.088780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.204781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.204781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.088780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.088780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.088780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.204781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.204781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.204781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1467 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.204781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.208781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      126 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.088780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.092780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.088780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.088780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.092780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.088780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.208781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.208781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.088780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.208781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.208781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.092780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.092780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.208781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.208781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.092780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.092780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.092780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.092780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.208781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.208781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.092780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.208781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.208781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.092780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.092780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.208781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.208781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.092780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.092780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.092780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.208781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.208781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.208781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1484 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.092780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.096780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.092780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.092780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.096780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.092780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.208781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.208781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.092780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.208781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.212781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.096780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.096780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.212781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.212781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.096780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.096780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.096780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.096780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.212781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.212781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.096780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.212781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.212781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.096780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.096780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.212781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.212781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.096780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.096780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.096780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.212781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.212781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.212781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1467 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.212781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.212781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.096780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.100780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.096780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.096780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.100780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.096780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.212781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.212781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.100780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.212781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.216781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.100780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.100780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.216781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.216781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.100780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.100780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.100780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.100780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.216781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.216781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.100780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.216781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.216781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.100780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.100780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.216781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.216781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.100780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.100780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.100780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.216781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.216781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.216781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1495 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.100780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.104780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.100780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.100780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.104780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.100780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.216781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.216781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.104780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.216781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.216781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.104780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.104780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.216781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.220781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.104780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.104780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.104780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.104780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.220781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.220781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.104780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.220781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.220781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.104780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.104780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.220781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.220781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.104780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.104780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.104780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.220781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.220781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.220781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1498 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.220781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.220781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.220781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.104780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.108780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.108780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.108780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.108780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.108780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.220781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.220781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.108780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.220781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.224781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.108780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.108780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.224781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.224781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.108780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.108780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.108780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.108780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.224781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.224781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.108780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.224781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.224781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.108780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.108780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.224781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.224781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.108780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.108780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.108780 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.224781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.224781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.224781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.224781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.224781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.224781 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.112780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.112780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.112780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.112780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.112780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.112780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.228781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.228781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.112780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.228781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.228781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.112780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.112780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.228781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.228781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.112780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.112780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.112780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.112780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.228781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.228781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.112780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.228781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.228781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.112780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.112780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.228781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.228781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.116780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.116780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.116780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.228781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.228781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.228781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.116780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.120780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.116780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.116780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.116780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.116780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.228781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.228781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.116780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.232781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.232781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.116780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.116780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.232781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.232781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.116780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.116780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.116780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.116780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.232781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.232781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.116780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.232781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.232781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.116780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.116780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.232781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.232781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.120780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.120780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.120780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.232781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.232781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.232781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.120780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.124780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.120780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.120780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.120780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.120780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.232781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.232781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.120780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.232781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.232781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.120780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.120780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.232781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.232781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.120780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.120780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.120780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.120780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.232781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.236781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.120780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.236781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.236781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.120780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.120780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.236781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.236781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.124780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.124780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.124780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.236781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.236781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.236781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1470 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.124780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.128780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.124780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.124780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.124780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.124780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.236781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.236781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.124780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.236781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.236781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.124780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.124780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.236781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.236781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.124780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.124780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.128780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.124780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.236781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.236781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.124780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.236781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.240781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1362 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.128780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.240781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.240781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.128780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.128780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.240781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.240781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.128780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.128780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.128780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.240781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.240781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.240781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.240781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      210 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.132780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.136780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.132780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.132780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.132780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.132780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.244781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.244781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.132780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.244781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.244781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.132780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.132780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.244781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.244781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.136780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.136780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.136780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.136780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.244781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.244781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.136780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.244781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.244781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.136780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.136780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.248781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.248781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.136780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.136780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.136780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.248781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.248781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.248781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.128780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.132780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.128780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.128780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.128780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.128780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.240781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.240781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.128780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.240781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.240781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.128780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.128780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.240781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.240781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.128780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.128780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.132780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.132780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.240781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.240781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.132780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.240781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.240781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1362 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.132780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.244781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.244781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.132780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.132780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.244781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.244781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.132780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.132780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.132780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.244781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.244781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.244781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.244781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      210 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.136780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.140780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.136780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.136780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.140780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.136780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.248781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.248781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.136780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.248781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.248781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.140780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.140780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.248781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.248781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.140780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.140780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.140780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.140780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.248781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.248781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.140780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.248781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.248781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.140780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.140780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.248781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.248781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.140780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.140780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.140780 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.248781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.248781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2102 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.252781 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1470 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.144780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.148780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.144780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.144780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.144780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.144780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.252781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.252781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.144780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.252781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.252781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1086 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.144780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.144780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.252781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.252781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.144780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.144780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.144780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.144780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.252781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.252781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.144780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.144780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.252781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.252781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:37:42.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.144780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.252781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.252781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2044 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.144780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.144780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.252781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.252781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.148780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.148780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.148780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.252781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.252781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.252781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    16163 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.256781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.256781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.256781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      148 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.256781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5383 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.256781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      148 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.256781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5495 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.148780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.152780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.148780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.148780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.148780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.148780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.256781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.256781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.148780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.256781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.256781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.148780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.148780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.256781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.256781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.152780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.152780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.152780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.152780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.256781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.256781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.152780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.152780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.260781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.260781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:37:42.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.152780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.260781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.260781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:37:42.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.152780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.260781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.260781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2044 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.152780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.152780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.260781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.260781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.152780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.152780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.152780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.260781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.260781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.260781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    27061 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.260781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.260781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.260781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.264781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       61 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.156780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.160781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.156780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.156780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.156780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.156780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.264781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.264781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.156780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.264781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.264781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1086 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.156780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.156780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.264781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.264781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.156780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.156780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.156780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.156780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.264781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.264781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.156780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.264781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.264781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.156780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.156780 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.264781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.264781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.160781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.160781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.160781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.264781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.264781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.264781 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    10807 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.160781 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.164780 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.160781 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.160781 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.160781 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.160781 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.264781 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.264781 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.160781 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.264781 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.264781 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.160781 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.160781 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.268782 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.268782 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.160781 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.160781 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.160781 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.160781 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.268782 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.268782 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.160781 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.268782 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.268782 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.160781 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.160781 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.268782 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.268782 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.164780 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.164780 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.164780 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.268782 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.268782 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2086 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.268782 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.268782 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      123 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.268782 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.268782 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.268782 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      122 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4730 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/test_cli.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2906 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/test_daemon.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8822 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/test_downloadclient.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3745 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/test_downloaditem.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11350 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/test_free_space.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    17208 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/test_move.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8074 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/test_operations.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    13110 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/test_review.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1468 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/test_runner.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/test_servarr.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1204 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/tests/test_verify.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1374 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/src/prunerr/utils.py
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)      162 2023-04-26 00:39:40.000000 prunerr-1.1.5b0/src/prunerr/version.py
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-26 00:39:41.176781 prunerr-1.1.5b0/src/prunerr.egg-info/
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)    17775 2023-04-26 00:39:40.000000 prunerr-1.1.5b0/src/prunerr.egg-info/PKG-INFO
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)    64656 2023-04-26 00:39:41.000000 prunerr-1.1.5b0/src/prunerr.egg-info/SOURCES.txt
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)        1 2023-04-26 00:39:40.000000 prunerr-1.1.5b0/src/prunerr.egg-info/dependency_links.txt
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)       41 2023-04-26 00:39:40.000000 prunerr-1.1.5b0/src/prunerr.egg-info/entry_points.txt
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)      312 2023-04-26 00:39:40.000000 prunerr-1.1.5b0/src/prunerr.egg-info/requires.txt
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)        8 2023-04-26 00:39:40.000000 prunerr-1.1.5b0/src/prunerr.egg-info/top_level.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3327 2023-04-25 04:48:04.000000 prunerr-1.1.5b0/tox.ini
```

### Comparing `prunerr-1.1.5/.dir-locals.el.in` & `prunerr-1.1.5b0/.dir-locals.el.in`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/.dockerignore` & `prunerr-1.1.5b0/.dockerignore`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/.env.in` & `prunerr-1.1.5b0/.env.in`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/.github/workflows/build-test.yml` & `prunerr-1.1.5b0/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/.gitignore` & `prunerr-1.1.5b0/.gitignore`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/.gitlab-ci.yml` & `prunerr-1.1.5b0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/.pre-commit-config.yaml` & `prunerr-1.1.5b0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/.prospector.yaml` & `prunerr-1.1.5b0/.prospector.yaml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/CONTRIBUTING.rst` & `prunerr-1.1.5b0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/Dockerfile` & `prunerr-1.1.5b0/Dockerfile`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/Dockerfile.devel` & `prunerr-1.1.5b0/Dockerfile.devel`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/LICENSE` & `prunerr-1.1.5b0/LICENSE`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/Makefile` & `prunerr-1.1.5b0/Makefile`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/NEWS.rst` & `prunerr-1.1.5b0/NEWS.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,57 +1,51 @@
-prunerr 1.1.5 (2023-04-26)
-==========================
-
-No significant changes.
-
-
 prunerr 1.1.5b0 (2023-04-26)
 ============================
 
 Bugfixes
 --------
 
 - Upgrade all requirements to the latest versions as of Tue Apr 25 11:00:28 PM UTC 2023.
 
 
-prunerr 1.1.4 (2023-04-25)
-==========================
+prunerr  (2023-04-25)
+=====================
 
 No significant changes.
 
 
-prunerr 1.1.4b0 (2023-04-25)
-============================
+prunerr  (2023-04-25)
+=====================
 
 Improved Documentation
 ----------------------
 
 - Link important use cases to their corresponding example configuration.
 
 
-prunerr 1.1.3 (2023-04-24)
-==========================
+prunerr  (2023-04-24)
+=====================
 
 No significant changes.
 
 
-prunerr 1.1.3b0 (2023-04-24)
-============================
+prunerr  (2023-04-24)
+=====================
 
 No significant changes.
 
 
-prunerr 1.1.2 (2023-04-22)
-==========================
+prunerr  (2023-04-22)
+=====================
 
 No significant changes.
 
 
-prunerr 1.1.2b2 (2023-04-22)
-============================
+prunerr  (2023-04-22)
+=====================
 
 No significant changes.
 
 
 prunerr 1.1.2b1 (2023-04-20)
 ============================
```

### Comparing `prunerr-1.1.5/PKG-INFO` & `prunerr-1.1.5b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prunerr
-Version: 1.1.5
+Version: 1.1.5b0
 Summary: Perma-seed Servarr media libraries
 Home-page: https://gitlab.com/rpatterson/prunerr
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: servarr,sonarr,radarr,transmission,bittorent,torrent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `prunerr-1.1.5/README.rst` & `prunerr-1.1.5b0/README.rst`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/TODO.rst` & `prunerr-1.1.5b0/TODO.rst`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/bin/cz-check-bump` & `prunerr-1.1.5b0/bin/cz-check-bump`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/bin/entrypoint` & `prunerr-1.1.5b0/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/bin/get-base-version` & `prunerr-1.1.5b0/bin/get-base-version`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/build-host/Dockerfile` & `prunerr-1.1.5b0/build-host/Dockerfile`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/build-host/Makefile` & `prunerr-1.1.5b0/build-host/Makefile`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/build-host/README.rst` & `prunerr-1.1.5b0/build-host/README.rst`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/build-host/bin/entrypoint` & `prunerr-1.1.5b0/build-host/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/build-host/requirements-py310.txt` & `prunerr-1.1.5b0/build-host/requirements-py310.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/build-host/requirements-py311.txt` & `prunerr-1.1.5b0/build-host/requirements-py311.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/build-host/requirements-py37.txt` & `prunerr-1.1.5b0/build-host/requirements-py37.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/build-host/requirements-py38.txt` & `prunerr-1.1.5b0/build-host/requirements-py38.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/build-host/requirements-py39.txt` & `prunerr-1.1.5b0/build-host/requirements-py39.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/docker-compose-servarr.yml` & `prunerr-1.1.5b0/docker-compose-servarr.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/docker-compose.override.yml` & `prunerr-1.1.5b0/docker-compose.override.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/docker-compose.yml` & `prunerr-1.1.5b0/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/gitlab-runner/config/config.toml.in` & `prunerr-1.1.5b0/gitlab-runner/config/config.toml.in`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/gitlab-runner/docker-compose.yml` & `prunerr-1.1.5b0/gitlab-runner/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/pyproject.toml` & `prunerr-1.1.5b0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 [tool.commitizen]
 # Parse commit messages according to conventional commits to decide wether the next
 # versin tag should be a major, minor or patch bump and create the VCS tag.  Also
 # provides VCS hooks to enforce that commit messages comply with conventional commits:
 # https://commitizen-tools.github.io/commitizen/
 name = "cz_conventional_commits"
 changelog_start_rev = "v0.0.0"
-version = "1.1.5"
+version = "1.1.5b0"
 tag_format = "v$version"
 annotated_tag = true
 gpg_sign = true
 bump_message = """\
 build(release): Version $current_version → $new_version
 
 [actions skip]
```

### Comparing `prunerr-1.1.5/requirements/build.txt.in` & `prunerr-1.1.5b0/requirements/build.txt.in`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/requirements/py310/build.txt` & `prunerr-1.1.5b0/requirements/py310/build.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/requirements/py310/devel.txt` & `prunerr-1.1.5b0/requirements/py310/devel.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/requirements/py310/user.txt` & `prunerr-1.1.5b0/requirements/py310/user.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/requirements/py311/build.txt` & `prunerr-1.1.5b0/requirements/py311/build.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/requirements/py311/devel.txt` & `prunerr-1.1.5b0/requirements/py311/devel.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/requirements/py311/user.txt` & `prunerr-1.1.5b0/requirements/py311/user.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/requirements/py37/build.txt` & `prunerr-1.1.5b0/requirements/py37/build.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/requirements/py37/devel.txt` & `prunerr-1.1.5b0/requirements/py37/devel.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/requirements/py37/user.txt` & `prunerr-1.1.5b0/requirements/py37/user.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/requirements/py38/build.txt` & `prunerr-1.1.5b0/requirements/py38/build.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/requirements/py38/devel.txt` & `prunerr-1.1.5b0/requirements/py38/devel.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/requirements/py38/user.txt` & `prunerr-1.1.5b0/requirements/py38/user.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/requirements/py39/build.txt` & `prunerr-1.1.5b0/requirements/py39/build.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/requirements/py39/devel.txt` & `prunerr-1.1.5b0/requirements/py39/devel.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/requirements/py39/user.txt` & `prunerr-1.1.5b0/requirements/py39/user.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/setup.cfg` & `prunerr-1.1.5b0/setup.cfg`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/__init__.py` & `prunerr-1.1.5b0/src/prunerr/__init__.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/downloadclient.py` & `prunerr-1.1.5b0/src/prunerr/downloadclient.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/downloaditem.py` & `prunerr-1.1.5b0/src/prunerr/downloaditem.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/home/.config/prunerr.yml` & `prunerr-1.1.5b0/src/prunerr/home/.config/prunerr.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/operations.py` & `prunerr-1.1.5b0/src/prunerr/operations.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/runner.py` & `prunerr-1.1.5b0/src/prunerr/runner.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/servarr.py` & `prunerr-1.1.5b0/src/prunerr/servarr.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/Makefile` & `prunerr-1.1.5b0/src/prunerr/tests/Makefile`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/__init__.py` & `prunerr-1.1.5b0/src/prunerr/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/example-5s.mkv` & `prunerr-1.1.5b0/src/prunerr/tests/example-5s.mkv`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/home/daemon/.config/prunerr.yml` & `prunerr-1.1.5b0/src/prunerr/tests/home/daemon/.config/prunerr.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/home/download-clients/.config/prunerr.yml` & `prunerr-1.1.5b0/src/prunerr/tests/home/download-clients/.config/prunerr.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/home/review-edge-cases/.config/prunerr.yml` & `prunerr-1.1.5b0/src/prunerr/tests/home/review-edge-cases/.config/prunerr.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/request.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/request.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/request.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/response.json` & `prunerr-1.1.5b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/test_cli.py` & `prunerr-1.1.5b0/src/prunerr/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/test_daemon.py` & `prunerr-1.1.5b0/src/prunerr/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/test_downloadclient.py` & `prunerr-1.1.5b0/src/prunerr/tests/test_downloadclient.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/test_downloaditem.py` & `prunerr-1.1.5b0/src/prunerr/tests/test_downloaditem.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/test_free_space.py` & `prunerr-1.1.5b0/src/prunerr/tests/test_free_space.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/test_move.py` & `prunerr-1.1.5b0/src/prunerr/tests/test_move.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/test_operations.py` & `prunerr-1.1.5b0/src/prunerr/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/test_review.py` & `prunerr-1.1.5b0/src/prunerr/tests/test_review.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/test_runner.py` & `prunerr-1.1.5b0/src/prunerr/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/test_servarr.py` & `prunerr-1.1.5b0/src/prunerr/tests/test_servarr.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/tests/test_verify.py` & `prunerr-1.1.5b0/src/prunerr/tests/test_verify.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr/utils.py` & `prunerr-1.1.5b0/src/prunerr/utils.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/src/prunerr.egg-info/PKG-INFO` & `prunerr-1.1.5b0/src/prunerr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prunerr
-Version: 1.1.5
+Version: 1.1.5b0
 Summary: Perma-seed Servarr media libraries
 Home-page: https://gitlab.com/rpatterson/prunerr
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: servarr,sonarr,radarr,transmission,bittorent,torrent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `prunerr-1.1.5/src/prunerr.egg-info/SOURCES.txt` & `prunerr-1.1.5b0/src/prunerr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.5/tox.ini` & `prunerr-1.1.5b0/tox.ini`

 * *Files identical despite different names*

