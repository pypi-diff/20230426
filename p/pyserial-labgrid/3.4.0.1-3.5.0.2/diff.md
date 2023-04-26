# Comparing `tmp/pyserial-labgrid-3.4.0.1.tar.gz` & `tmp/pyserial-labgrid-3.5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyserial-labgrid-3.4.0.1.tar", last modified: Thu Jan 13 05:16:05 2022, max compression
+gzip compressed data, was "pyserial-labgrid-3.5.0.2.tar", last modified: Wed Apr 26 09:56:50 2023, max compression
```

## Comparing `pyserial-labgrid-3.4.0.1.tar` & `pyserial-labgrid-3.5.0.2.tar`

### file list

```diff
@@ -1,91 +1,104 @@
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2022-01-13 05:16:05.000000 pyserial-labgrid-3.4.0.1/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)    24764 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/CHANGES.rst
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1885 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/LICENSE.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1074 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/MANIFEST.in
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1601 2022-01-13 05:16:05.000000 pyserial-labgrid-3.4.0.1/PKG-INFO
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1913 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/README.rst
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2022-01-13 05:16:05.000000 pyserial-labgrid-3.4.0.1/documentation/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     2997 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/documentation/Makefile
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     5597 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/documentation/appendix.rst
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     6526 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/documentation/conf.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)    10555 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/documentation/examples.rst
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      969 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/documentation/index.rst
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     7050 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/documentation/pyserial.png
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     4447 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/documentation/pyserial.rst
--rw-r--r--   0 nxa13855  (1001) atg       (1001)    40113 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/documentation/pyserial_api.rst
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     3550 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/documentation/shortintro.rst
--rw-r--r--   0 nxa13855  (1001) atg       (1001)    10375 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/documentation/tools.rst
--rw-r--r--   0 nxa13855  (1001) atg       (1001)    10805 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/documentation/url_handlers.rst
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2022-01-13 05:16:05.000000 pyserial-labgrid-3.4.0.1/examples/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     4936 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/examples/at_protocol.py
--rwxr-xr-x   0 nxa13855  (1001) atg       (1001)    20154 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/examples/port_publisher.py
--rwxr-xr-x   0 nxa13855  (1001) atg       (1001)     1054 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/examples/port_publisher.sh
--rwxr-xr-x   0 nxa13855  (1001) atg       (1001)     6148 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/examples/rfc2217_server.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      794 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/examples/setup-miniterm-py2exe.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      780 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/examples/setup-rfc2217_server-py2exe.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1027 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/examples/setup-wxTerminal-py2exe.py
--rwxr-xr-x   0 nxa13855  (1001) atg       (1001)     7096 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/examples/tcp_serial_redirect.py
--rwxr-xr-x   0 nxa13855  (1001) atg       (1001)    13223 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/examples/wxSerialConfigDialog.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)    13614 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/examples/wxSerialConfigDialog.wxg
--rwxr-xr-x   0 nxa13855  (1001) atg       (1001)    14710 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/examples/wxTerminal.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     6904 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/examples/wxTerminal.wxg
--rw-r--r--   0 nxa13855  (1001) atg       (1001)    12497 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/pylintrc
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2022-01-13 05:16:05.000000 pyserial-labgrid-3.4.0.1/pyserial_labgrid.egg-info/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1601 2022-01-13 05:16:05.000000 pyserial-labgrid-3.4.0.1/pyserial_labgrid.egg-info/PKG-INFO
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     2039 2022-01-13 05:16:05.000000 pyserial-labgrid-3.4.0.1/pyserial_labgrid.egg-info/SOURCES.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        1 2022-01-13 05:16:05.000000 pyserial-labgrid-3.4.0.1/pyserial_labgrid.egg-info/dependency_links.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        7 2022-01-13 05:16:05.000000 pyserial-labgrid-3.4.0.1/pyserial_labgrid.egg-info/top_level.txt
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2022-01-13 05:16:05.000000 pyserial-labgrid-3.4.0.1/serial/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     3216 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/serial/__init__.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)    60485 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/serial/rfc2217.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     3305 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/serial/rs485.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     9144 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/serial/serialcli.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     8454 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/serial/serialjava.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)    32977 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/serial/serialposix.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)    21724 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/serial/serialutil.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)    20126 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/serial/serialwin32.py
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2022-01-13 05:16:05.000000 pyserial-labgrid-3.4.0.1/serial/threaded/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     9312 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/serial/threaded/__init__.py
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2022-01-13 05:16:05.000000 pyserial-labgrid-3.4.0.1/serial/tools/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/serial/tools/__init__.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     3677 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/serial/tools/hexlify_codec.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     3389 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/serial/tools/list_ports.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     3736 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/serial/tools/list_ports_common.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     4513 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/serial/tools/list_ports_linux.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     9342 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/serial/tools/list_ports_osx.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     4535 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/serial/tools/list_ports_posix.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)    11401 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/serial/tools/list_ports_windows.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)    35440 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/serial/tools/miniterm.py
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2022-01-13 05:16:05.000000 pyserial-labgrid-3.4.0.1/serial/urlhandler/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/serial/urlhandler/__init__.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     2033 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/serial/urlhandler/protocol_alt.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     3159 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/serial/urlhandler/protocol_hwgrep.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)    10159 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/serial/urlhandler/protocol_loop.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      317 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/serial/urlhandler/protocol_rfc2217.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)    14170 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/serial/urlhandler/protocol_socket.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     9064 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/serial/urlhandler/protocol_spy.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)    10893 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/serial/win32.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      125 2022-01-13 05:16:05.000000 pyserial-labgrid-3.4.0.1/setup.cfg
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     3005 2022-01-13 05:15:51.000000 pyserial-labgrid-3.4.0.1/setup.py
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2022-01-13 05:16:05.000000 pyserial-labgrid-3.4.0.1/test/
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2022-01-13 05:16:05.000000 pyserial-labgrid-3.4.0.1/test/handlers/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/test/handlers/__init__.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     7099 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/test/handlers/protocol_test.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1689 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/test/run_all_tests.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     7942 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/test/test.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     6037 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/test/test_advanced.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     2518 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/test/test_asyncio.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     3508 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/test/test_cancel.py
--rwxr-xr-x   0 nxa13855  (1001) atg       (1001)     1238 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/test/test_context.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     2041 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/test/test_exclusive.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     2284 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/test/test_high_load.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1775 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/test/test_iolib.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1514 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/test/test_pty.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     3421 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/test/test_readline.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1358 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/test/test_rfc2217.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     2138 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/test/test_rs485.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     2678 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/test/test_settings_dict.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     2395 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/test/test_threaded.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     2009 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/test/test_timeout_class.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1557 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/test/test_url.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1148 2022-01-13 05:15:03.000000 pyserial-labgrid-3.4.0.1/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:56:50.890697 pyserial-labgrid-3.5.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:56:50.878697 pyserial-labgrid-3.5.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:56:50.882697 pyserial-labgrid-3.5.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/.github/workflows/build-and-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/.github/workflows/push-pr-unit-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/.github/workflows/reusable-unit-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/.github/workflows/scheduled-unit-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    28223 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-04-26 09:56:50.890697 pyserial-labgrid-3.5.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:56:50.882697 pyserial-labgrid-3.5.0.2/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/documentation/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/documentation/appendix.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/documentation/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10555 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/documentation/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/documentation/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/documentation/pyserial.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/documentation/pyserial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    40147 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/documentation/pyserial_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/documentation/shortintro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10453 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/documentation/tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/documentation/url_handlers.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:56:50.886697 pyserial-labgrid-3.5.0.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/examples/at_protocol.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20154 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/examples/port_publisher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1054 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/examples/port_publisher.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6148 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/examples/rfc2217_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/examples/setup-miniterm-py2exe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/examples/setup-rfc2217_server-py2exe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/examples/setup-wxTerminal-py2exe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7509 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/examples/tcp_serial_redirect.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13196 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/examples/wxSerialConfigDialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13614 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/examples/wxSerialConfigDialog.wxg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14524 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/examples/wxTerminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/examples/wxTerminal.wxg
+-rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:56:50.886697 pyserial-labgrid-3.5.0.2/pyserial_labgrid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-04-26 09:56:50.000000 pyserial-labgrid-3.5.0.2/pyserial_labgrid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-26 09:56:50.000000 pyserial-labgrid-3.5.0.2/pyserial_labgrid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 09:56:50.000000 pyserial-labgrid-3.5.0.2/pyserial_labgrid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-26 09:56:50.000000 pyserial-labgrid-3.5.0.2/pyserial_labgrid.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 09:56:50.000000 pyserial-labgrid-3.5.0.2/pyserial_labgrid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 09:56:50.000000 pyserial-labgrid-3.5.0.2/pyserial_labgrid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:56:50.886697 pyserial-labgrid-3.5.0.2/serial/
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/serial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/serial/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60508 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/serial/rfc2217.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/serial/rs485.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/serial/serialcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/serial/serialjava.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35127 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/serial/serialposix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21797 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/serial/serialutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20284 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/serial/serialwin32.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:56:50.886697 pyserial-labgrid-3.5.0.2/serial/threaded/
+-rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/serial/threaded/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:56:50.886697 pyserial-labgrid-3.5.0.2/serial/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/serial/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/serial/tools/hexlify_codec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/serial/tools/list_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/serial/tools/list_ports_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/serial/tools/list_ports_linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11178 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/serial/tools/list_ports_osx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/serial/tools/list_ports_posix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16021 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/serial/tools/list_ports_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37840 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/serial/tools/miniterm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:56:50.890697 pyserial-labgrid-3.5.0.2/serial/urlhandler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/serial/urlhandler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/serial/urlhandler/protocol_alt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/serial/urlhandler/protocol_cp2110.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/serial/urlhandler/protocol_hwgrep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10623 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/serial/urlhandler/protocol_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/serial/urlhandler/protocol_rfc2217.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14299 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/serial/urlhandler/protocol_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/serial/urlhandler/protocol_spy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11138 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/serial/win32.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-26 09:56:50.890697 pyserial-labgrid-3.5.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:56:50.890697 pyserial-labgrid-3.5.0.2/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:56:50.890697 pyserial-labgrid-3.5.0.2/test/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/test/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7125 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/test/handlers/protocol_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/test/run_all_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/test/test_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/test/test_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/test/test_cancel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1238 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/test/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/test/test_exclusive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/test/test_high_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/test/test_iolib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/test/test_pty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/test/test_readline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/test/test_rfc2217.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/test/test_rs485.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/test/test_settings_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/test/test_threaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/test/test_timeout_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/test/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-26 09:56:39.000000 pyserial-labgrid-3.5.0.2/test/test_util.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyserial-labgrid-3.4.0.1/CHANGES.rst` & `pyserial-labgrid-3.5.0.2/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -730,7 +730,96 @@
 Bugfixes (posix):
 
 - allow calling cancel functions w/o error if port is closed
 - [#220] protocol_socket: sync error handling with posix version
 - [#227] posix: ignore more blocking errors and EINTR, timeout only
   applies to blocking I/O
 - [#228] fix: port_publisher typo
+
+
+Version 3.5b0 2020-09-21
+------------------------
+New Features:
+
+- [#411] Add a backend for Silicon Labs CP2110/4 HID-to-UART bridge.
+  (depends on `hid` module)
+
+Improvements:
+
+- [#315] Use absolute import everywhere
+- [#351] win32: miniterm Working CMD.exe terminal using Windows 10 ANSI support
+- [#354] Make ListPortInfo hashable
+- [#372] threaded: "write" returns byte count
+- [#400] Add bytesize and stopbits argument parser to tcp_serial_redirect
+- [#408] loop: add out_waiting
+- [#495] list_ports_linux: Correct "interface" property on Linux hosts
+- [#500] Remove Python 3.2 and 3.3 from test
+- [#261, #285, #296, #320, #333, #342, #356, #358, #389, #397, #510] doc updates
+- miniterm: add :kbd:`CTRL+T Q` as alternative to exit
+- miniterm: suspend function key changed to :kbd:`CTRL-T Z`
+- add command line tool entries ``pyserial-miniterm`` (replaces ``miniterm.py``)
+  and ``pyserial-ports`` (runs ``serial.tools.list_ports``).
+- ``python -m serial`` opens miniterm (use w/o args and it will print port
+  list too) [experimental]
+
+Bugfixes:
+
+- [#371] Don't open port if self.port is not set while entering context manager
+- [#437, #502] refactor: raise new instances for PortNotOpenError and SerialTimeoutException
+- [#261, #263] list_ports: set default `name` attribute
+- [#286] fix: compare only of the same type in list_ports_common.ListPortInfo
+- rfc2217/close(): fix race-condition
+- [#305] return b'' when connection closes on rfc2217 connection
+- [#386] rfc2217/close(): fix race condition
+- Fixed flush_input_buffer() for situations where the remote end has closed the socket.
+- [#441] reset_input_buffer() can hang on sockets
+- examples: port_publisher python 3 fixes
+- [#324] miniterm: Fix miniterm constructor exit_character and menu_character
+- [#326] miniterm: use exclusive access for native serial ports by default
+- [#497] miniterm: fix double use of CTRL-T + s use z for suspend instead
+- [#443, #444] examples: refactor wx example, use Bind to avoid deprecated
+  warnings, IsChecked, unichr
+
+Bugfixes (posix):
+
+- [#265] posix: fix PosixPollSerial with timeout=None and add cancel support
+- [#290] option for low latency mode on linux
+- [#335] Add support to xr-usb-serial ports
+- [#494] posix: Don't catch the SerialException we just raised
+- [#519] posix: Fix custom baud rate to not temporarily set 38400 baud rates on linux
+- [#509 #518] list_ports: use hardcoded path to library on osx
+
+Bugfixes (win32):
+
+- [#481] win32: extend RS485 error messages
+- [#303] win32: do not check for links in serial.tools.list_ports
+- [#430] Add WaitCommEvent function to win32
+- [#314, #433] tools/list_ports_windows: Scan both 'Ports' and 'Modem' device classes
+- [#414] Serial number support for composite USB devices
+- Added recursive search for device USB serial number to support composite devices
+
+Bugfixes (MacOS):
+
+- [#364] MacOS: rework list_ports to support unicode product descriptors.
+- [#367] Mac and bsd fix _update_break_state
+
+
+Version 3.5 2020-11-23
+----------------------
+See above (3.5b0) for what's all new in this release
+
+Bugfixes:
+
+- spy: ensure bytes in write()
+
+Bugfixes (posix):
+
+- [#540] serialposix: Fix inconsistent state after exception in open()
+
+Bugfixes (win32):
+
+- [#530] win32: Fix exception for composite serial number search on Windows
+
+Bugfixes (MacOS):
+
+- [#542] list_ports_osx: kIOMasterPortDefault no longer exported on Big Sur
+- [#545, #545] list_ports_osx: getting USB info on BigSur/AppleSilicon
```

### Comparing `pyserial-labgrid-3.4.0.1/LICENSE.txt` & `pyserial-labgrid-3.5.0.2/LICENSE.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2001-2016 Chris Liechti <cliechti@gmx.net>
+Copyright (c) 2001-2020 Chris Liechti <cliechti@gmx.net>
 All Rights Reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are
 met:
 
   * Redistributions of source code must retain the above copyright
```

### Comparing `pyserial-labgrid-3.4.0.1/MANIFEST.in` & `pyserial-labgrid-3.5.0.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/README.rst` & `pyserial-labgrid-3.5.0.2/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,32 @@
-=================================
- pySerial  |build-status| |docs|
-=================================
+================================================
+ pySerial (labgrid fork)  |build-status| |docs|
+================================================
 
 Overview
 ========
 This module encapsulates the access for the serial port. It provides backends
 for Python_ running on Windows, OSX, Linux, BSD (possibly any POSIX compliant
 system) and IronPython. The module named "serial" automatically selects the
 appropriate backend.
 
-- Project Homepage: https://github.com/pyserial/pyserial
-- Download Page: https://pypi.python.org/pypi/pyserial
+This fork integrates RFC2217 relevant fixes which haven't been accepted
+upstream. We used to install from git, but newer pip enforces that all packages
+installed from pypi also have all dependencies on pypi. Therefore this is now a
+proper fork which:
 
-BSD license, (C) 2001-2017 Chris Liechti <cliechti@gmx.net>
+- converts to pyproject.toml
+- integrates rfc2217 fixes
+- will be available as pyserial-labgrid on pypi
+
+- Project Homepage: https://github.com/pyserial/pyserial-labgrid
+- Download Page: https://pypi.python.org/pypi/pyserial-labgrid
+
+BSD license, (C) 2001-2020 Chris Liechti <cliechti@gmx.net>
+BSD license, (C) 2023-2023 Rouven Czerwinski <entwicklung@pengutronix.de>
 
 
 Documentation
 =============
 For API documentation, usage and examples see files in the "documentation"
 directory.  The ".rst" files can be read in any text editor or being converted to
 HTML or PDF using Sphinx_. An HTML version is online at
```

### Comparing `pyserial-labgrid-3.4.0.1/documentation/Makefile` & `pyserial-labgrid-3.5.0.2/documentation/Makefile`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/documentation/appendix.rst` & `pyserial-labgrid-3.5.0.2/documentation/appendix.rst`

 * *Files 4% similar despite different names*

```diff
@@ -87,14 +87,20 @@
     On POSIX based systems, the user usually needs to be in a special group to
     have access to serial ports.
 
     On Debian based systems, serial ports are usually in the group ``dialout``,
     so running ``sudo adduser $USER dialout`` (and logging-out and -in) enables
     the user to access the port.
 
+Parity on Raspberry Pi
+    The Raspi has one full UART and a restricted one. On devices with built
+    in wireless (WIFI/BT) use the restricted one on the GPIO header pins.
+    If enhanced features are required, it is possible to swap UARTs, see
+    https://www.raspberrypi.org/documentation/configuration/uart.md
+
 Support for Python 2.6 or earlier
     Support for older Python releases than 2.7 will not return to pySerial 3.x.
     Python 2.7 is now many years old (released 2010). If you insist on using
     Python 2.6 or earlier, it is recommend to use pySerial `2.7`_
     (or any 2.x version).
 
 .. _`2.7`: https://pypi.python.org/pypi/pyserial/2.7
@@ -105,15 +111,15 @@
 
 com0com - http://com0com.sourceforge.net/
     Provides virtual serial ports for Windows.
 
 
 License
 =======
-Copyright (c) 2001-2017 Chris Liechti <cliechti@gmx.net>
+Copyright (c) 2001-2020 Chris Liechti <cliechti@gmx.net>
 All Rights Reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are
 met:
 
   * Redistributions of source code must retain the above copyright
```

### Comparing `pyserial-labgrid-3.4.0.1/documentation/conf.py` & `pyserial-labgrid-3.5.0.2/documentation/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 #source_encoding = 'utf-8'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = u'pySerial'
-copyright = u'2001-2017, Chris Liechti'
+copyright = u'2001-2020, Chris Liechti'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = '3.4'
```

### Comparing `pyserial-labgrid-3.4.0.1/documentation/examples.rst` & `pyserial-labgrid-3.5.0.2/documentation/examples.rst`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/documentation/index.rst` & `pyserial-labgrid-3.5.0.2/documentation/index.rst`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/documentation/pyserial.png` & `pyserial-labgrid-3.5.0.2/documentation/pyserial.png`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/documentation/pyserial.rst` & `pyserial-labgrid-3.5.0.2/documentation/pyserial.rst`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 for Python_ running on Windows, OSX, Linux, BSD (possibly any POSIX compliant
 system) and IronPython. The module named "serial" automatically selects the
 appropriate backend.
 
 It is released under a free software license, see LICENSE_ for more
 details.
 
-Copyright (C) 2001-2016 Chris Liechti <cliechti(at)gmx.net>
+Copyright (C) 2001-2020 Chris Liechti <cliechti(at)gmx.net>
 
 Other pages (online)
 
 - `project page on GitHub`_
 - `Download Page`_ with releases (PyPi)
 - This page, when viewed online is at https://pyserial.readthedocs.io/en/latest/ or
   http://pythonhosted.org/pyserial/ .
```

### Comparing `pyserial-labgrid-3.4.0.1/documentation/pyserial_api.rst` & `pyserial-labgrid-3.5.0.2/documentation/pyserial_api.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,27 +32,27 @@
 
         :param stopbits:
             Number of stop bits. Possible values:
             :const:`STOPBITS_ONE`, :const:`STOPBITS_ONE_POINT_FIVE`,
             :const:`STOPBITS_TWO`
 
         :param float timeout:
-            Set a read timeout value.
+            Set a read timeout value in seconds.
 
         :param bool xonxoff:
             Enable software flow control.
 
         :param bool rtscts:
             Enable hardware (RTS/CTS) flow control.
 
         :param bool dsrdtr:
             Enable hardware (DSR/DTR) flow control.
 
         :param float write_timeout:
-            Set a write timeout value.
+            Set a write timeout value in seconds.
 
         :param float inter_byte_timeout:
             Inter-character timeout, :const:`None` to disable (default).
 
         :param bool exclusive:
             Set exclusive access mode (POSIX only).  A port cannot be opened in 
             exclusive access mode if it is already open in exclusive access mode.
@@ -180,15 +180,15 @@
         :rtype: int
         :exception SerialTimeoutException:
             In case a write timeout is configured for the port and the time is
             exceeded.
 
         Write the bytes *data* to the port. This should be of type ``bytes``
         (or compatible such as ``bytearray`` or ``memoryview``). Unicode
-        strings must be encoded (e.g. ``'hello'.encode('utf-8'``).
+        strings must be encoded (e.g. ``'hello'.encode('utf-8')``.
 
     .. versionchanged:: 2.5
             Accepts instances of :class:`bytes` and :class:`bytearray` when
             available (Python 2.6 and newer) and :class:`str` otherwise.
 
         .. versionchanged:: 2.5
             Write returned ``None`` in previous versions.
@@ -233,15 +233,15 @@
         Note, for some USB serial adapters, this may only flush the buffer of
         the OS and not all the data that may be present in the USB part.
 
         .. versionchanged:: 3.0 renamed from ``flushOutput()``
 
     .. method:: send_break(duration=0.25)
 
-        :param float duration: Time to activate the BREAK condition.
+        :param float duration: Time in seconds, to activate the BREAK condition.
 
         Send break condition. Timed, returns to idle state after given
         duration.
 
 
     .. attribute:: break_condition
```

### Comparing `pyserial-labgrid-3.4.0.1/documentation/shortintro.rst` & `pyserial-labgrid-3.5.0.2/documentation/shortintro.rst`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/documentation/tools.rst` & `pyserial-labgrid-3.5.0.2/documentation/tools.rst`

 * *Files 1% similar despite different names*

```diff
@@ -270,21 +270,22 @@
     ---    7 8        set data bits
     ---    N E O S M  change parity (None, Even, Odd, Space, Mark)
     ---    1 2 3      set stop bits (1, 2, 1.5)
     ---    b          change baud rate
     ---    x X        disable/enable software flow control
     ---    r R        disable/enable hardware flow control
 
-:kbd:`Ctrl+T s` suspends the connection (port is opened) and reconnects when a
+:kbd:`Ctrl+T z` suspends the connection (port is opened) and reconnects when a
 key is pressed. This can be used to temporarily access the serial port with an
 other application, without exiting miniterm. If reconnecting fails it is
 also possible to exit (:kbd:`Ctrl+]`) or change the port (:kbd:`p`).
 
 .. versionchanged:: 2.5
     Added :kbd:`Ctrl+T` menu and added support for opening URLs.
 .. versionchanged:: 2.6
     File moved from the examples to :mod:`serial.tools.miniterm`.
 .. versionchanged:: 3.0
     Apply encoding on serial port, convert to Unicode for console.
     Added new filters, default to stripping terminal control sequences.
     Added ``--ask`` option.
-
+.. versionchanged:: 3.5
+    Enable escape code handling on Windows 10 console.
```

### Comparing `pyserial-labgrid-3.4.0.1/documentation/url_handlers.rst` & `pyserial-labgrid-3.5.0.2/documentation/url_handlers.rst`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 - ``rfc2217://<host>:<port>[?<option>[&<option>...]]``
 - ``socket://<host>:<port>[?logging={debug|info|warning|error}]``
 - ``loop://[?logging={debug|info|warning|error}]``
 - ``hwgrep://<regexp>[&skip_busy][&n=N]``
 - ``spy://port[?option[=value][&option[=value]]]``
 - ``alt://port?class=<classname>``
+- ``cp2110://<bus>:<dev>:<if>``
 
 .. versionchanged:: 3.0 Options are specified with ``?`` and ``&`` instead of ``/``
 
 Device names are also supported, e.g.:
 
 - ``/dev/ttyUSB0`` (Linux)
 - ``COM3`` (Windows)
@@ -44,15 +45,15 @@
   lines are read (CTS/DTR/RI/CD). Without this option it relies on the server
   sending the notifications automatically (that's what the RFC suggests and
   most servers do). Enable this option when :attr:`cts` does not work as
   expected, i.e. for servers that do not send notifications.
 
 - ``timeout=<value>``: Change network timeout (default 3 seconds). This is
   useful when the server takes a little more time to send its answers. The
-  timeout applies to the initial Telnet / :rfc:`2271` negotiation as well
+  timeout applies to the initial Telnet / :rfc:`2217` negotiation as well
   as changing port settings or control line change commands.
 
 - ``logging={debug|info|warning|error}``: Prints diagnostic messages (not
   useful for end users). It uses the logging module and a logger called
   ``pySerial.rfc2217`` so that the application can setup up logging
   handlers etc. It will call :meth:`logging.basicConfig` which initializes
   for output on ``sys.stderr`` (if no logging was set up already).
@@ -231,21 +232,36 @@
 Examples::
 
     alt:///dev/ttyUSB0?class=PosixPollSerial
     alt:///dev/ttyUSB0?class=VTIMESerial
 
 .. versionadded:: 3.0
 
+``cp2110://``
+=============
+
+This backend implements support for HID-to-UART devices manufactured by Silicon
+Labs and marketed as CP2110 and CP2114. The implementation is (mostly)
+OS-independent and in userland. It relies on `cython-hidapi`_.
+
+.. _cython-hidapi: https://github.com/trezor/cython-hidapi
+
+Examples::
+
+    cp2110://0001:004a:00
+    cp2110://0002:0077:00
+
+.. versionadded:: 3.5
 
 Examples
 ========
 
 - ``rfc2217://localhost:7000``
 - ``rfc2217://localhost:7000?poll_modem``
 - ``rfc2217://localhost:7000?ign_set_control&timeout=5.5``
 - ``socket://localhost:7777``
 - ``loop://?logging=debug``
 - ``hwgrep://0451:f432`` (USB VID:PID)
 - ``spy://COM54?file=log.txt``
 - ``alt:///dev/ttyUSB0?class=PosixPollSerial``
-
+- ``cp2110://0001:004a:00``
```

### Comparing `pyserial-labgrid-3.4.0.1/examples/at_protocol.py` & `pyserial-labgrid-3.5.0.2/examples/at_protocol.py`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/examples/port_publisher.py` & `pyserial-labgrid-3.5.0.2/examples/port_publisher.py`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/examples/port_publisher.sh` & `pyserial-labgrid-3.5.0.2/examples/port_publisher.sh`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/examples/rfc2217_server.py` & `pyserial-labgrid-3.5.0.2/examples/rfc2217_server.py`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/examples/setup-miniterm-py2exe.py` & `pyserial-labgrid-3.5.0.2/examples/setup-miniterm-py2exe.py`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/examples/setup-rfc2217_server-py2exe.py` & `pyserial-labgrid-3.5.0.2/examples/setup-rfc2217_server-py2exe.py`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/examples/setup-wxTerminal-py2exe.py` & `pyserial-labgrid-3.5.0.2/examples/setup-wxTerminal-py2exe.py`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/examples/tcp_serial_redirect.py` & `pyserial-labgrid-3.5.0.2/examples/tcp_serial_redirect.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 #
 # Redirect data from a TCP/IP connection to a serial port and vice versa.
 #
-# (C) 2002-2016 Chris Liechti <cliechti@gmx.net>
+# (C) 2002-2020 Chris Liechti <cliechti@gmx.net>
 #
 # SPDX-License-Identifier:    BSD-3-Clause
 
 import sys
 import socket
 import serial
 import serial.threaded
@@ -62,21 +62,35 @@
         action='store_true',
         help='Development mode, prints Python internals on errors',
         default=False)
 
     group = parser.add_argument_group('serial port')
 
     group.add_argument(
+        "--bytesize",
+        choices=[5, 6, 7, 8],
+        type=int,
+        help="set bytesize, one of {5 6 7 8}, default: 8",
+        default=8)
+
+    group.add_argument(
         "--parity",
         choices=['N', 'E', 'O', 'S', 'M'],
         type=lambda c: c.upper(),
         help="set parity, one of {N E O S M}, default: N",
         default='N')
 
     group.add_argument(
+        "--stopbits",
+        choices=[1, 1.5, 2],
+        type=float,
+        help="set stopbits, one of {1 1.5 2}, default: 1",
+        default=1)
+
+    group.add_argument(
         '--rtscts',
         action='store_true',
         help='enable RTS/CTS flow control (default off)',
         default=False)
 
     group.add_argument(
         '--xonxoff',
@@ -113,15 +127,17 @@
         default=False)
 
     args = parser.parse_args()
 
     # connect to serial port
     ser = serial.serial_for_url(args.SERIALPORT, do_not_open=True)
     ser.baudrate = args.BAUDRATE
+    ser.bytesize = args.bytesize
     ser.parity = args.parity
+    ser.stopbits = args.stopbits
     ser.rtscts = args.rtscts
     ser.xonxoff = args.xonxoff
 
     if args.rts is not None:
         ser.rts = args.rts
 
     if args.dtr is not None:
```

### Comparing `pyserial-labgrid-3.4.0.1/examples/wxSerialConfigDialog.py` & `pyserial-labgrid-3.5.0.2/examples/wxSerialConfigDialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,18 +198,18 @@
         sizer_2.Add(sizer_3, 0, wx.ALL | wx.ALIGN_RIGHT, 4)
         self.SetSizer(sizer_2)
         sizer_2.Fit(self)
         self.Layout()
         # end wxGlade
 
     def __attach_events(self):
-        wx.EVT_BUTTON(self, self.button_ok.GetId(), self.OnOK)
-        wx.EVT_BUTTON(self, self.button_cancel.GetId(), self.OnCancel)
+        self.button_ok.Bind(wx.EVT_BUTTON, self.OnOK)
+        self.button_cancel.Bind(wx.EVT_BUTTON, self.OnCancel)
         if self.show & SHOW_TIMEOUT:
-            wx.EVT_CHECKBOX(self, self.checkbox_timeout.GetId(), self.OnTimeout)
+            self.checkbox_timeout.Bind(wx.EVT_CHECKBOX, self.OnTimeout)
 
     def OnOK(self, events):
         success = True
         self.serial.port = self.ports[self.choice_port.GetSelection()]
         if self.show & SHOW_BAUDRATE:
             try:
                 b = int(self.combo_box_baudrate.GetValue())
```

### Comparing `pyserial-labgrid-3.4.0.1/examples/wxSerialConfigDialog.wxg` & `pyserial-labgrid-3.5.0.2/examples/wxSerialConfigDialog.wxg`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/examples/wxTerminal.py` & `pyserial-labgrid-3.5.0.2/examples/wxTerminal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,36 @@
 #!/usr/bin/env python
 #
 # A simple terminal application with wxPython.
 #
-# (C) 2001-2015 Chris Liechti <cliechti@gmx.net>
+# (C) 2001-2020 Chris Liechti <cliechti@gmx.net>
 #
 # SPDX-License-Identifier:    BSD-3-Clause
 
 import codecs
+from serial.tools.miniterm import unichr
 import serial
 import threading
 import wx
+import wx.lib.newevent
 import wxSerialConfigDialog
 
+try:
+    unichr
+except NameError:
+    unichr = chr
+
 # ----------------------------------------------------------------------
 # Create an own event type, so that GUI updates can be delegated
 # this is required as on some platforms only the main thread can
 # access the GUI without crashing. wxMutexGuiEnter/wxMutexGuiLeave
 # could be used too, but an event is more elegant.
 
+SerialRxEvent, EVT_SERIALRX = wx.lib.newevent.NewEvent()
 SERIALRX = wx.NewEventType()
-# bind to serial data receive events
-EVT_SERIALRX = wx.PyEventBinder(SERIALRX, 0)
-
-
-class SerialRxEvent(wx.PyCommandEvent):
-    eventType = SERIALRX
-
-    def __init__(self, windowID, data):
-        wx.PyCommandEvent.__init__(self, self.eventType, windowID)
-        self.data = data
-
-    def Clone(self):
-        self.__class__(self.GetId(), self.data)
 
 # ----------------------------------------------------------------------
 
 ID_CLEAR = wx.NewId()
 ID_SAVEAS = wx.NewId()
 ID_SETTINGS = wx.NewId()
 ID_TERM = wx.NewId()
@@ -211,14 +206,15 @@
         # register events at the controls
         self.Bind(wx.EVT_MENU, self.OnClear, id=ID_CLEAR)
         self.Bind(wx.EVT_MENU, self.OnSaveAs, id=ID_SAVEAS)
         self.Bind(wx.EVT_MENU, self.OnExit, id=ID_EXIT)
         self.Bind(wx.EVT_MENU, self.OnPortSettings, id=ID_SETTINGS)
         self.Bind(wx.EVT_MENU, self.OnTermSettings, id=ID_TERM)
         self.text_ctrl_output.Bind(wx.EVT_CHAR, self.OnKey)
+        self.Bind(wx.EVT_CHAR_HOOK, self.OnKey)
         self.Bind(EVT_SERIALRX, self.OnSerialRead)
         self.Bind(wx.EVT_CLOSE, self.OnClose)
 
     def OnExit(self, event):  # wxGlade: TerminalFrame.<event_handler>
         """Menu point Exit"""
         self.Close()
 
@@ -300,30 +296,31 @@
 
     def OnKey(self, event):
         """\
         Key event handler. If the key is in the ASCII range, write it to the
         serial port. Newline handling and local echo is also done here.
         """
         code = event.GetUnicodeKey()
-        if code < 256:   # XXX bug in some versions of wx returning only capital letters
-            code = event.GetKeyCode()
+        # if code < 256:   # XXX bug in some versions of wx returning only capital letters
+        #     code = event.GetKeyCode()
         if code == 13:                      # is it a newline? (check for CR which is the RETURN key)
             if self.settings.echo:          # do echo if needed
                 self.text_ctrl_output.AppendText('\n')
             if self.settings.newline == NEWLINE_CR:
                 self.serial.write(b'\r')     # send CR
             elif self.settings.newline == NEWLINE_LF:
                 self.serial.write(b'\n')     # send LF
             elif self.settings.newline == NEWLINE_CRLF:
                 self.serial.write(b'\r\n')   # send CR+LF
         else:
             char = unichr(code)
             if self.settings.echo:          # do echo if needed
                 self.WriteText(char)
             self.serial.write(char.encode('UTF-8', 'replace'))         # send the character
+        event.StopPropagation()
 
     def WriteText(self, text):
         if self.settings.unprintable:
             text = ''.join([c if (c >= ' ' and c != '\x7f') else unichr(0x2400 + ord(c)) for c in text])
         self.text_ctrl_output.AppendText(text)
 
     def OnSerialRead(self, event):
@@ -341,29 +338,27 @@
                 # newline transformation
                 if self.settings.newline == NEWLINE_CR:
                     b = b.replace(b'\r', b'\n')
                 elif self.settings.newline == NEWLINE_LF:
                     pass
                 elif self.settings.newline == NEWLINE_CRLF:
                     b = b.replace(b'\r\n', b'\n')
-                event = SerialRxEvent(self.GetId(), b)
-                self.GetEventHandler().AddPendingEvent(event)
+                wx.PostEvent(self, SerialRxEvent(data=b))
 
     def OnRTS(self, event):  # wxGlade: TerminalFrame.<event_handler>
         self.serial.rts = event.IsChecked()
 
     def OnDTR(self, event):  # wxGlade: TerminalFrame.<event_handler>
-        self.serial.dtr = event.Checked()
+        self.serial.dtr = event.IsChecked()
 
 # end of class TerminalFrame
 
 
 class MyApp(wx.App):
     def OnInit(self):
-        wx.InitAllImageHandlers()
         frame_terminal = TerminalFrame(None, -1, "")
         self.SetTopWindow(frame_terminal)
         frame_terminal.Show(True)
         return 1
 
 # end of class MyApp
```

### Comparing `pyserial-labgrid-3.4.0.1/examples/wxTerminal.wxg` & `pyserial-labgrid-3.5.0.2/examples/wxTerminal.wxg`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/pylintrc` & `pyserial-labgrid-3.5.0.2/pylintrc`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/pyserial_labgrid.egg-info/SOURCES.txt` & `pyserial-labgrid-3.5.0.2/pyserial_labgrid.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,21 @@
+.gitignore
+.travis.yml
 CHANGES.rst
 LICENSE.txt
 MANIFEST.in
 README.rst
 pylintrc
+pyproject.toml
+requirements.txt
 setup.cfg
-setup.py
+.github/workflows/build-and-release.yml
+.github/workflows/push-pr-unit-tests.yml
+.github/workflows/reusable-unit-tests.yml
+.github/workflows/scheduled-unit-tests.yml
 documentation/Makefile
 documentation/appendix.rst
 documentation/conf.py
 documentation/examples.rst
 documentation/index.rst
 documentation/pyserial.png
 documentation/pyserial.rst
@@ -27,16 +34,19 @@
 examples/wxSerialConfigDialog.py
 examples/wxSerialConfigDialog.wxg
 examples/wxTerminal.py
 examples/wxTerminal.wxg
 pyserial_labgrid.egg-info/PKG-INFO
 pyserial_labgrid.egg-info/SOURCES.txt
 pyserial_labgrid.egg-info/dependency_links.txt
+pyserial_labgrid.egg-info/entry_points.txt
+pyserial_labgrid.egg-info/requires.txt
 pyserial_labgrid.egg-info/top_level.txt
 serial/__init__.py
+serial/__main__.py
 serial/rfc2217.py
 serial/rs485.py
 serial/serialcli.py
 serial/serialjava.py
 serial/serialposix.py
 serial/serialutil.py
 serial/serialwin32.py
@@ -49,14 +59,15 @@
 serial/tools/list_ports_linux.py
 serial/tools/list_ports_osx.py
 serial/tools/list_ports_posix.py
 serial/tools/list_ports_windows.py
 serial/tools/miniterm.py
 serial/urlhandler/__init__.py
 serial/urlhandler/protocol_alt.py
+serial/urlhandler/protocol_cp2110.py
 serial/urlhandler/protocol_hwgrep.py
 serial/urlhandler/protocol_loop.py
 serial/urlhandler/protocol_rfc2217.py
 serial/urlhandler/protocol_socket.py
 serial/urlhandler/protocol_spy.py
 test/run_all_tests.py
 test/test.py
```

### Comparing `pyserial-labgrid-3.4.0.1/serial/__init__.py` & `pyserial-labgrid-3.5.0.2/serial/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/env python
 #
 # This is a wrapper module for different platform implementations
 #
 # This file is part of pySerial. https://github.com/pyserial/pyserial
-# (C) 2001-2017 Chris Liechti <cliechti@gmx.net>
+# (C) 2001-2020 Chris Liechti <cliechti@gmx.net>
 #
 # SPDX-License-Identifier:    BSD-3-Clause
 
 from __future__ import absolute_import
 
 import sys
 import importlib
 
 from serial.serialutil import *
 #~ SerialBase, SerialException, to_bytes, iterbytes
 
-__version__ = '3.4.0.1'
+__version__ = '3.5.0.2'
 
 VERSION = __version__
 
 # pylint: disable=wrong-import-position
 if sys.platform == 'cli':
     from serial.serialcli import Serial
 else:
```

### Comparing `pyserial-labgrid-3.4.0.1/serial/rfc2217.py` & `pyserial-labgrid-3.5.0.2/serial/rfc2217.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 try:
     import Queue
 except ImportError:
     import queue as Queue
 
 import serial
 from serial.serialutil import SerialBase, SerialException, to_bytes, \
-    iterbytes, portNotOpenError, Timeout
+    iterbytes, PortNotOpenError, Timeout
 
 # port string is expected to be something like this:
 # rfc2217://host:port
 # host may be an IP or including domain, whatever.
 # port is 0...65535
 
 # map log level names to constants. used in from_url()
@@ -483,15 +483,15 @@
                     break
             else:
                 raise SerialException(
                     "Remote does not seem to support RFC2217 or BINARY mode {!r}".format(mandadory_options))
             if self.logger:
                 self.logger.info("Negotiated options: {}".format(self._telnet_options))
 
-            # fine, go on, set RFC 2271 specific things
+            # fine, go on, set RFC 2217 specific things
             self._reconfigure_port()
             # all things set up get, now a clean start
             if not self._dsrdtr:
                 self._update_dtr_state()
             if not self._rtscts:
                 self._update_rts_state()
             self.reset_input_buffer()
@@ -598,30 +598,30 @@
 
     #  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -
 
     @property
     def in_waiting(self):
         """Return the number of bytes currently in the input buffer."""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         return self._read_buffer.qsize()
 
     def read(self, size=1):
         """\
         Read size bytes from the serial port. If a timeout is set it may
         return less characters as requested. With no timeout it will block
         until the requested number of bytes is read.
         """
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         data = bytearray()
         try:
             timeout = Timeout(self._timeout)
             while len(data) < size:
-                if self._thread is None:
+                if self._thread is None or not self._thread.is_alive():
                     raise SerialException('connection failed (reader thread died)')
                 buf = self._read_buffer.get(True, timeout.time_left())
                 if buf is None:
                     return bytes(data)
                 data += buf
                 if timeout.expired():
                     break
@@ -632,102 +632,102 @@
     def write(self, data):
         """\
         Output the given byte string over the serial port. Can block if the
         connection is blocked. May raise SerialException if the connection is
         closed.
         """
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         with self._write_lock:
             try:
                 self._socket.sendall(to_bytes(data).replace(IAC, IAC_DOUBLED))
             except socket.error as e:
                 raise SerialException("connection failed (socket error): {}".format(e))
         return len(data)
 
     def reset_input_buffer(self):
         """Clear input buffer, discarding all that is in the buffer."""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         self.rfc2217_send_purge(PURGE_RECEIVE_BUFFER)
         # empty read buffer
         while self._read_buffer.qsize():
             self._read_buffer.get(False)
 
     def reset_output_buffer(self):
         """\
         Clear output buffer, aborting the current output and
         discarding all that is in the buffer.
         """
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         self.rfc2217_send_purge(PURGE_TRANSMIT_BUFFER)
 
     def _update_break_state(self):
         """\
         Set break: Controls TXD. When active, to transmitting is
         possible.
         """
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         if self.logger:
             self.logger.info('set BREAK to {}'.format('active' if self._break_state else 'inactive'))
         if self._break_state:
             self.rfc2217_set_control(SET_CONTROL_BREAK_ON)
         else:
             self.rfc2217_set_control(SET_CONTROL_BREAK_OFF)
 
     def _update_rts_state(self):
         """Set terminal status line: Request To Send."""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         if self.logger:
             self.logger.info('set RTS to {}'.format('active' if self._rts_state else 'inactive'))
         if self._rts_state:
             self.rfc2217_set_control(SET_CONTROL_RTS_ON)
         else:
             self.rfc2217_set_control(SET_CONTROL_RTS_OFF)
 
     def _update_dtr_state(self):
         """Set terminal status line: Data Terminal Ready."""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         if self.logger:
             self.logger.info('set DTR to {}'.format('active' if self._dtr_state else 'inactive'))
         if self._dtr_state:
             self.rfc2217_set_control(SET_CONTROL_DTR_ON)
         else:
             self.rfc2217_set_control(SET_CONTROL_DTR_OFF)
 
     @property
     def cts(self):
         """Read terminal status line: Clear To Send."""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         return bool(self.get_modem_state() & MODEMSTATE_MASK_CTS)
 
     @property
     def dsr(self):
         """Read terminal status line: Data Set Ready."""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         return bool(self.get_modem_state() & MODEMSTATE_MASK_DSR)
 
     @property
     def ri(self):
         """Read terminal status line: Ring Indicator."""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         return bool(self.get_modem_state() & MODEMSTATE_MASK_RI)
 
     @property
     def cd(self):
         """Read terminal status line: Carrier Detect."""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         return bool(self.get_modem_state() & MODEMSTATE_MASK_CD)
 
     @property
     def timeout(self):
         """Get the current timeout setting."""
         return self._timeout
 
@@ -807,15 +807,14 @@
                             # other telnet commands
                             self._telnet_process_command(byte)
                             mode = M_NORMAL
                     elif mode == M_NEGOTIATE:  # DO, DONT, WILL, WONT was received, option now following
                         self._telnet_negotiate_option(telnet_command, byte)
                         mode = M_NORMAL
         finally:
-            self._thread = None
             if self.logger:
                 self.logger.debug("read thread terminated")
 
     # - incoming telnet commands and options
 
     def _telnet_process_command(self, command):
         """Process commands other than DO, DONT, WILL, WONT."""
```

### Comparing `pyserial-labgrid-3.4.0.1/serial/rs485.py` & `pyserial-labgrid-3.5.0.2/serial/rs485.py`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/serial/serialcli.py` & `pyserial-labgrid-3.5.0.2/serial/serialcli.py`

 * *Files 5% similar despite different names*

```diff
@@ -144,25 +144,25 @@
 
     #  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -
 
     @property
     def in_waiting(self):
         """Return the number of characters currently in the input buffer."""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         return self._port_handle.BytesToRead
 
     def read(self, size=1):
         """\
         Read size bytes from the serial port. If a timeout is set it may
         return less characters as requested. With no timeout it will block
         until the requested number of bytes is read.
         """
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         # must use single byte reads as this is the only way to read
         # without applying encodings
         data = bytearray()
         while size:
             try:
                 data.append(self._port_handle.ReadByte())
             except System.TimeoutException:
@@ -170,84 +170,84 @@
             else:
                 size -= 1
         return bytes(data)
 
     def write(self, data):
         """Output the given string over the serial port."""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         #~ if not isinstance(data, (bytes, bytearray)):
             #~ raise TypeError('expected %s or bytearray, got %s' % (bytes, type(data)))
         try:
             # must call overloaded method with byte array argument
             # as this is the only one not applying encodings
             self._port_handle.Write(as_byte_array(data), 0, len(data))
         except System.TimeoutException:
-            raise writeTimeoutError
+            raise SerialTimeoutException('Write timeout')
         return len(data)
 
     def reset_input_buffer(self):
         """Clear input buffer, discarding all that is in the buffer."""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         self._port_handle.DiscardInBuffer()
 
     def reset_output_buffer(self):
         """\
         Clear output buffer, aborting the current output and
         discarding all that is in the buffer.
         """
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         self._port_handle.DiscardOutBuffer()
 
     def _update_break_state(self):
         """
         Set break: Controls TXD. When active, to transmitting is possible.
         """
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         self._port_handle.BreakState = bool(self._break_state)
 
     def _update_rts_state(self):
         """Set terminal status line: Request To Send"""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         self._port_handle.RtsEnable = bool(self._rts_state)
 
     def _update_dtr_state(self):
         """Set terminal status line: Data Terminal Ready"""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         self._port_handle.DtrEnable = bool(self._dtr_state)
 
     @property
     def cts(self):
         """Read terminal status line: Clear To Send"""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         return self._port_handle.CtsHolding
 
     @property
     def dsr(self):
         """Read terminal status line: Data Set Ready"""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         return self._port_handle.DsrHolding
 
     @property
     def ri(self):
         """Read terminal status line: Ring Indicator"""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         #~ return self._port_handle.XXX
         return False  # XXX an error would be better
 
     @property
     def cd(self):
         """Read terminal status line: Carrier Detect"""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         return self._port_handle.CDHolding
 
     # - - platform specific - - - -
     # none
```

### Comparing `pyserial-labgrid-3.4.0.1/serial/serialjava.py` & `pyserial-labgrid-3.5.0.2/serial/serialjava.py`

 * *Files 6% similar despite different names*

```diff
@@ -148,104 +148,104 @@
 
     #  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -
 
     @property
     def in_waiting(self):
         """Return the number of characters currently in the input buffer."""
         if not self.sPort:
-            raise portNotOpenError
+            raise PortNotOpenError()
         return self._instream.available()
 
     def read(self, size=1):
         """\
         Read size bytes from the serial port. If a timeout is set it may
         return less characters as requested. With no timeout it will block
         until the requested number of bytes is read.
         """
         if not self.sPort:
-            raise portNotOpenError
+            raise PortNotOpenError()
         read = bytearray()
         if size > 0:
             while len(read) < size:
                 x = self._instream.read()
                 if x == -1:
                     if self.timeout >= 0:
                         break
                 else:
                     read.append(x)
         return bytes(read)
 
     def write(self, data):
         """Output the given string over the serial port."""
         if not self.sPort:
-            raise portNotOpenError
+            raise PortNotOpenError()
         if not isinstance(data, (bytes, bytearray)):
             raise TypeError('expected %s or bytearray, got %s' % (bytes, type(data)))
         self._outstream.write(data)
         return len(data)
 
     def reset_input_buffer(self):
         """Clear input buffer, discarding all that is in the buffer."""
         if not self.sPort:
-            raise portNotOpenError
+            raise PortNotOpenError()
         self._instream.skip(self._instream.available())
 
     def reset_output_buffer(self):
         """\
         Clear output buffer, aborting the current output and
         discarding all that is in the buffer.
         """
         if not self.sPort:
-            raise portNotOpenError
+            raise PortNotOpenError()
         self._outstream.flush()
 
     def send_break(self, duration=0.25):
         """Send break condition. Timed, returns to idle state after given duration."""
         if not self.sPort:
-            raise portNotOpenError
+            raise PortNotOpenError()
         self.sPort.sendBreak(duration*1000.0)
 
     def _update_break_state(self):
         """Set break: Controls TXD. When active, to transmitting is possible."""
         if self.fd is None:
-            raise portNotOpenError
+            raise PortNotOpenError()
         raise SerialException("The _update_break_state function is not implemented in java.")
 
     def _update_rts_state(self):
         """Set terminal status line: Request To Send"""
         if not self.sPort:
-            raise portNotOpenError
+            raise PortNotOpenError()
         self.sPort.setRTS(self._rts_state)
 
     def _update_dtr_state(self):
         """Set terminal status line: Data Terminal Ready"""
         if not self.sPort:
-            raise portNotOpenError
+            raise PortNotOpenError()
         self.sPort.setDTR(self._dtr_state)
 
     @property
     def cts(self):
         """Read terminal status line: Clear To Send"""
         if not self.sPort:
-            raise portNotOpenError
+            raise PortNotOpenError()
         self.sPort.isCTS()
 
     @property
     def dsr(self):
         """Read terminal status line: Data Set Ready"""
         if not self.sPort:
-            raise portNotOpenError
+            raise PortNotOpenError()
         self.sPort.isDSR()
 
     @property
     def ri(self):
         """Read terminal status line: Ring Indicator"""
         if not self.sPort:
-            raise portNotOpenError
+            raise PortNotOpenError()
         self.sPort.isRI()
 
     @property
     def cd(self):
         """Read terminal status line: Carrier Detect"""
         if not self.sPort:
-            raise portNotOpenError
+            raise PortNotOpenError()
         self.sPort.isCD()
```

### Comparing `pyserial-labgrid-3.4.0.1/serial/serialposix.py` & `pyserial-labgrid-3.5.0.2/serial/serialposix.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 #
 # backend for serial IO for POSIX compatible systems, like Linux, OSX
 #
 # This file is part of pySerial. https://github.com/pyserial/pyserial
-# (C) 2001-2016 Chris Liechti <cliechti@gmx.net>
+# (C) 2001-2020 Chris Liechti <cliechti@gmx.net>
 #
 # SPDX-License-Identifier:    BSD-3-Clause
 #
 # parts based on code from Grant B. Edwards  <grante@visi.com>:
 #  ftp://ftp.visi.com/users/grante/python/PosixSerial.py
 #
 # references: http://www.easysw.com/~mike/serial/serial.html
@@ -35,29 +35,38 @@
 import select
 import struct
 import sys
 import termios
 
 import serial
 from serial.serialutil import SerialBase, SerialException, to_bytes, \
-    portNotOpenError, writeTimeoutError, Timeout
+    PortNotOpenError, SerialTimeoutException, Timeout
 
 
 class PlatformSpecificBase(object):
     BAUDRATE_CONSTANTS = {}
 
     def _set_special_baudrate(self, baudrate):
         raise NotImplementedError('non-standard baudrates are not supported on this platform')
 
     def _set_rs485_mode(self, rs485_settings):
         raise NotImplementedError('RS485 not supported on this platform')
 
     def set_low_latency_mode(self, low_latency_settings):
         raise NotImplementedError('Low latency not supported on this platform')
 
+    def _update_break_state(self):
+        """\
+        Set break: Controls TXD. When active, no transmitting is possible.
+        """
+        if self._break_state:
+            fcntl.ioctl(self.fd, TIOCSBRK)
+        else:
+            fcntl.ioctl(self.fd, TIOCCBRK)
+    
 
 # some systems support an extra flag to enable the two in POSIX unsupported
 # paritiy settings for MARK and SPACE
 CMSPAR = 0  # default, for unsupported platforms, override below
 
 # try to detect the OS so that a device can be selected...
 # this code block should supply a device() and set_special_baudrate() function
@@ -201,21 +210,33 @@
 
 elif plat[:6] == 'darwin':   # OS X
     import array
     IOSSIOSPEED = 0x80045402  # _IOW('T', 2, speed_t)
 
     class PlatformSpecific(PlatformSpecificBase):
         osx_version = os.uname()[2].split('.')
+        TIOCSBRK = 0x2000747B # _IO('t', 123)
+        TIOCCBRK = 0x2000747A # _IO('t', 122)
+
         # Tiger or above can support arbitrary serial speeds
         if int(osx_version[0]) >= 8:
             def _set_special_baudrate(self, baudrate):
                 # use IOKit-specific call to set up high speeds
                 buf = array.array('i', [baudrate])
                 fcntl.ioctl(self.fd, IOSSIOSPEED, buf, 1)
 
+        def _update_break_state(self):
+            """\
+            Set break: Controls TXD. When active, no transmitting is possible.
+            """
+            if self._break_state:
+                fcntl.ioctl(self.fd, PlatformSpecific.TIOCSBRK)
+            else:
+                fcntl.ioctl(self.fd, PlatformSpecific.TIOCCBRK)
+
 elif plat[:3] == 'bsd' or \
      plat[:7] == 'freebsd' or \
      plat[:6] == 'netbsd' or \
      plat[:7] == 'openbsd':
 
     class ReturnBaudrate(object):
         def __getitem__(self, key):
@@ -223,14 +244,27 @@
 
     class PlatformSpecific(PlatformSpecificBase):
         # Only tested on FreeBSD:
         # The baud rate may be passed in as
         # a literal value.
         BAUDRATE_CONSTANTS = ReturnBaudrate()
 
+        TIOCSBRK = 0x2000747B # _IO('t', 123)
+        TIOCCBRK = 0x2000747A # _IO('t', 122)
+
+        
+        def _update_break_state(self):
+            """\
+            Set break: Controls TXD. When active, no transmitting is possible.
+            """
+            if self._break_state:
+                fcntl.ioctl(self.fd, PlatformSpecific.TIOCSBRK)
+            else:
+                fcntl.ioctl(self.fd, PlatformSpecific.TIOCCBRK)
+
 else:
     class PlatformSpecific(PlatformSpecificBase):
         pass
 
 
 # load some constants for later use.
 # try to use values from termios, use defaults from linux otherwise
@@ -287,43 +321,61 @@
         try:
             self.fd = os.open(self.portstr, os.O_RDWR | os.O_NOCTTY | os.O_NONBLOCK)
         except OSError as msg:
             self.fd = None
             raise SerialException(msg.errno, "could not open port {}: {}".format(self._port, msg))
         #~ fcntl.fcntl(self.fd, fcntl.F_SETFL, 0)  # set blocking
 
+        self.pipe_abort_read_r, self.pipe_abort_read_w = None, None
+        self.pipe_abort_write_r, self.pipe_abort_write_w = None, None
+
         try:
             self._reconfigure_port(force_update=True)
-        except:
+
+            try:
+                if not self._dsrdtr:
+                    self._update_dtr_state()
+                if not self._rtscts:
+                    self._update_rts_state()
+            except IOError as e:
+                # ignore Invalid argument and Inappropriate ioctl
+                if e.errno not in (errno.EINVAL, errno.ENOTTY):
+                    raise
+
+            self._reset_input_buffer()
+
+            self.pipe_abort_read_r, self.pipe_abort_read_w = os.pipe()
+            self.pipe_abort_write_r, self.pipe_abort_write_w = os.pipe()
+            fcntl.fcntl(self.pipe_abort_read_r, fcntl.F_SETFL, os.O_NONBLOCK)
+            fcntl.fcntl(self.pipe_abort_write_r, fcntl.F_SETFL, os.O_NONBLOCK)
+        except BaseException:
             try:
                 os.close(self.fd)
-            except:
+            except Exception:
                 # ignore any exception when closing the port
                 # also to keep original exception that happened when setting up
                 pass
             self.fd = None
+
+            if self.pipe_abort_read_w is not None:
+                os.close(self.pipe_abort_read_w)
+                self.pipe_abort_read_w = None
+            if self.pipe_abort_read_r is not None:
+                os.close(self.pipe_abort_read_r)
+                self.pipe_abort_read_r = None
+            if self.pipe_abort_write_w is not None:
+                os.close(self.pipe_abort_write_w)
+                self.pipe_abort_write_w = None
+            if self.pipe_abort_write_r is not None:
+                os.close(self.pipe_abort_write_r)
+                self.pipe_abort_write_r = None
+
             raise
-        else:
-            self.is_open = True
-        try:
-            if not self._dsrdtr:
-                self._update_dtr_state()
-            if not self._rtscts:
-                self._update_rts_state()
-        except IOError as e:
-            if e.errno in (errno.EINVAL, errno.ENOTTY):
-                # ignore Invalid argument and Inappropriate ioctl
-                pass
-            else:
-                raise
-        self.reset_input_buffer()
-        self.pipe_abort_read_r, self.pipe_abort_read_w = os.pipe()
-        self.pipe_abort_write_r, self.pipe_abort_write_w = os.pipe()
-        fcntl.fcntl(self.pipe_abort_read_r, fcntl.F_SETFL, os.O_NONBLOCK)
-        fcntl.fcntl(self.pipe_abort_write_r, fcntl.F_SETFL, os.O_NONBLOCK)
+
+        self.is_open = True
 
     def _reconfigure_port(self, force_update=False):
         """Set communication parameters on opened port."""
         if self.fd is None:
             raise SerialException("Can only operate on a valid file descriptor")
 
         # if exclusive lock is requested, create it before we modify anything else
@@ -367,16 +419,23 @@
         try:
             ispeed = ospeed = getattr(termios, 'B{}'.format(self._baudrate))
         except AttributeError:
             try:
                 ispeed = ospeed = self.BAUDRATE_CONSTANTS[self._baudrate]
             except KeyError:
                 #~ raise ValueError('Invalid baud rate: %r' % self._baudrate)
-                # may need custom baud rate, it isn't in our list.
-                ispeed = ospeed = getattr(termios, 'B38400')
+
+                # See if BOTHER is defined for this platform; if it is, use
+                # this for a speed not defined in the baudrate constants list.
+                try:
+                    ispeed = ospeed = BOTHER
+                except NameError:
+                    # may need custom baud rate, it isn't in our list.
+                    ispeed = ospeed = getattr(termios, 'B38400')
+
                 try:
                     custom_baud = int(self._baudrate)  # store for later
                 except ValueError:
                     raise ValueError('Invalid baud rate: {!r}'.format(self._baudrate))
                 else:
                     if custom_baud < 0:
                         raise ValueError('Invalid baud rate: {!r}'.format(self._baudrate))
@@ -494,15 +553,15 @@
     def read(self, size=1):
         """\
         Read size bytes from the serial port. If a timeout is set it may
         return less characters as requested. With no timeout it will block
         until the requested number of bytes is read.
         """
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         read = bytearray()
         timeout = Timeout(self._timeout)
         while len(read) < size:
             try:
                 ready, _, _ = select.select([self.fd, self.pipe_abort_read_r], [], [], timeout.time_left())
                 if self.pipe_abort_read_r in ready:
                     os.read(self.pipe_abort_read_r, 1000)
@@ -510,36 +569,38 @@
                 # If select was used with a timeout, and the timeout occurs, it
                 # returns with empty lists -> thus abort read operation.
                 # For timeout == 0 (non-blocking operation) also abort when
                 # there is nothing to read.
                 if not ready:
                     break   # timeout
                 buf = os.read(self.fd, size - len(read))
-                # read should always return some data as select reported it was
-                # ready to read when we get to this point.
-                if not buf:
-                    # Disconnected devices, at least on Linux, show the
-                    # behavior that they are always ready to read immediately
-                    # but reading returns nothing.
-                    raise SerialException(
-                        'device reports readiness to read but returned no data '
-                        '(device disconnected or multiple access on port?)')
-                read.extend(buf)
             except OSError as e:
                 # this is for Python 3.x where select.error is a subclass of
                 # OSError ignore BlockingIOErrors and EINTR. other errors are shown
                 # https://www.python.org/dev/peps/pep-0475.
                 if e.errno not in (errno.EAGAIN, errno.EALREADY, errno.EWOULDBLOCK, errno.EINPROGRESS, errno.EINTR):
                     raise SerialException('read failed: {}'.format(e))
             except select.error as e:
                 # this is for Python 2.x
                 # ignore BlockingIOErrors and EINTR. all errors are shown
                 # see also http://www.python.org/dev/peps/pep-3151/#select
                 if e[0] not in (errno.EAGAIN, errno.EALREADY, errno.EWOULDBLOCK, errno.EINPROGRESS, errno.EINTR):
                     raise SerialException('read failed: {}'.format(e))
+            else:
+                # read should always return some data as select reported it was
+                # ready to read when we get to this point.
+                if not buf:
+                    # Disconnected devices, at least on Linux, show the
+                    # behavior that they are always ready to read immediately
+                    # but reading returns nothing.
+                    raise SerialException(
+                        'device reports readiness to read but returned no data '
+                        '(device disconnected or multiple access on port?)')
+                read.extend(buf)
+
             if timeout.expired():
                 break
         return bytes(read)
 
     def cancel_read(self):
         if self.is_open:
             os.write(self.pipe_abort_read_w, b"x")
@@ -547,36 +608,36 @@
     def cancel_write(self):
         if self.is_open:
             os.write(self.pipe_abort_write_w, b"x")
 
     def write(self, data):
         """Output the given byte string over the serial port."""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         d = to_bytes(data)
         tx_len = length = len(d)
         timeout = Timeout(self._write_timeout)
         while tx_len > 0:
             try:
                 n = os.write(self.fd, d)
                 if timeout.is_non_blocking:
                     # Zero timeout indicates non-blocking - simply return the
                     # number of bytes of data actually written
                     return n
                 elif not timeout.is_infinite:
                     # when timeout is set, use select to wait for being ready
                     # with the time left as timeout
                     if timeout.expired():
-                        raise writeTimeoutError
+                        raise SerialTimeoutException('Write timeout')
                     abort, ready, _ = select.select([self.pipe_abort_write_r], [self.fd], [], timeout.time_left())
                     if abort:
                         os.read(self.pipe_abort_write_r, 1000)
                         break
                     if not ready:
-                        raise writeTimeoutError
+                        raise SerialTimeoutException('Write timeout')
                 else:
                     assert timeout.time_left() is None
                     # wait for write operation
                     abort, ready, _ = select.select([self.pipe_abort_write_r], [self.fd], [], None)
                     if abort:
                         os.read(self.pipe_abort_write_r, 1)
                         break
@@ -595,59 +656,54 @@
             except select.error as e:
                 # this is for Python 2.x
                 # ignore BlockingIOErrors and EINTR. all errors are shown
                 # see also http://www.python.org/dev/peps/pep-3151/#select
                 if e[0] not in (errno.EAGAIN, errno.EALREADY, errno.EWOULDBLOCK, errno.EINPROGRESS, errno.EINTR):
                     raise SerialException('write failed: {}'.format(e))
             if not timeout.is_non_blocking and timeout.expired():
-                raise writeTimeoutError
+                raise SerialTimeoutException('Write timeout')
         return length - len(d)
 
     def flush(self):
         """\
         Flush of file like objects. In this case, wait until all data
         is written.
         """
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         termios.tcdrain(self.fd)
 
+    def _reset_input_buffer(self):
+        """Clear input buffer, discarding all that is in the buffer."""
+        termios.tcflush(self.fd, termios.TCIFLUSH)
+
     def reset_input_buffer(self):
         """Clear input buffer, discarding all that is in the buffer."""
         if not self.is_open:
-            raise portNotOpenError
-        termios.tcflush(self.fd, termios.TCIFLUSH)
+            raise PortNotOpenError()
+        self._reset_input_buffer()
 
     def reset_output_buffer(self):
         """\
         Clear output buffer, aborting the current output and discarding all
         that is in the buffer.
         """
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         termios.tcflush(self.fd, termios.TCOFLUSH)
 
     def send_break(self, duration=0.25):
         """\
         Send break condition. Timed, returns to idle state after given
         duration.
         """
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         termios.tcsendbreak(self.fd, int(duration / 0.25))
 
-    def _update_break_state(self):
-        """\
-        Set break: Controls TXD. When active, no transmitting is possible.
-        """
-        if self._break_state:
-            fcntl.ioctl(self.fd, TIOCSBRK)
-        else:
-            fcntl.ioctl(self.fd, TIOCCBRK)
-
     def _update_rts_state(self):
         """Set terminal status line: Request To Send"""
         if self._rts_state:
             fcntl.ioctl(self.fd, TIOCMBIS, TIOCM_RTS_str)
         else:
             fcntl.ioctl(self.fd, TIOCMBIC, TIOCM_RTS_str)
 
@@ -658,39 +714,39 @@
         else:
             fcntl.ioctl(self.fd, TIOCMBIC, TIOCM_DTR_str)
 
     @property
     def cts(self):
         """Read terminal status line: Clear To Send"""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         s = fcntl.ioctl(self.fd, TIOCMGET, TIOCM_zero_str)
         return struct.unpack('I', s)[0] & TIOCM_CTS != 0
 
     @property
     def dsr(self):
         """Read terminal status line: Data Set Ready"""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         s = fcntl.ioctl(self.fd, TIOCMGET, TIOCM_zero_str)
         return struct.unpack('I', s)[0] & TIOCM_DSR != 0
 
     @property
     def ri(self):
         """Read terminal status line: Ring Indicator"""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         s = fcntl.ioctl(self.fd, TIOCMGET, TIOCM_zero_str)
         return struct.unpack('I', s)[0] & TIOCM_RI != 0
 
     @property
     def cd(self):
         """Read terminal status line: Carrier Detect"""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         s = fcntl.ioctl(self.fd, TIOCMGET, TIOCM_zero_str)
         return struct.unpack('I', s)[0] & TIOCM_CD != 0
 
     # - - platform specific - - - -
 
     @property
     def out_waiting(self):
@@ -701,38 +757,38 @@
 
     def fileno(self):
         """\
         For easier use of the serial port instance with select.
         WARNING: this function is not portable to different platforms!
         """
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         return self.fd
 
     def set_input_flow_control(self, enable=True):
         """\
         Manually control flow - when software flow control is enabled.
         This will send XON (true) or XOFF (false) to the other device.
         WARNING: this function is not portable to different platforms!
         """
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         if enable:
             termios.tcflow(self.fd, termios.TCION)
         else:
             termios.tcflow(self.fd, termios.TCIOFF)
 
     def set_output_flow_control(self, enable=True):
         """\
         Manually control flow of outgoing data - when hardware or software flow
         control is enabled.
         WARNING: this function is not portable to different platforms!
         """
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         if enable:
             termios.tcflow(self.fd, termios.TCOON)
         else:
             termios.tcflow(self.fd, termios.TCOOFF)
 
     def nonblocking(self):
         """DEPRECATED - has no use"""
@@ -750,15 +806,15 @@
     def read(self, size=1):
         """\
         Read size bytes from the serial port. If a timeout is set it may
         return less characters as requested. With no timeout it will block
         until the requested number of bytes is read.
         """
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         read = bytearray()
         timeout = Timeout(self._timeout)
         poll = select.poll()
         poll.register(self.fd, select.POLLIN | select.POLLERR | select.POLLHUP | select.POLLNVAL)
         poll.register(self.pipe_abort_read_r, select.POLLIN | select.POLLERR | select.POLLHUP | select.POLLNVAL)
         if size > 0:
             while len(read) < size:
@@ -827,15 +883,15 @@
     def read(self, size=1):
         """\
         Read size bytes from the serial port. If a timeout is set it may
         return less characters as requested. With no timeout it will block
         until the requested number of bytes is read.
         """
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         read = bytearray()
         while len(read) < size:
             buf = os.read(self.fd, size - len(read))
             if not buf:
                 break
             read.extend(buf)
         return bytes(read)
```

### Comparing `pyserial-labgrid-3.4.0.1/serial/serialutil.py` & `pyserial-labgrid-3.5.0.2/serial/serialutil.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #! python
 #
 # Base class and support functions used by various backends.
 #
 # This file is part of pySerial. https://github.com/pyserial/pyserial
-# (C) 2001-2016 Chris Liechti <cliechti@gmx.net>
+# (C) 2001-2020 Chris Liechti <cliechti@gmx.net>
 #
 # SPDX-License-Identifier:    BSD-3-Clause
 
 from __future__ import absolute_import
 
 import io
 import time
@@ -93,16 +93,18 @@
     """Base class for serial port related exceptions."""
 
 
 class SerialTimeoutException(SerialException):
     """Write timeouts give an exception"""
 
 
-writeTimeoutError = SerialTimeoutException('Write timeout')
-portNotOpenError = SerialException('Attempting to use a port that is not open')
+class PortNotOpenError(SerialException):
+    """Port is not open"""
+    def __init__(self):
+        super(PortNotOpenError, self).__init__('Attempting to use a port that is not open')
 
 
 class Timeout(object):
     """\
     Abstraction for timeout operations. Using time.monotonic() if available
     or time.time() in all other cases.
 
@@ -555,30 +557,30 @@
             b[:n] = array.array('b', data)
         return n
 
     #  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -
     # context manager
 
     def __enter__(self):
-        if not self.is_open:
+        if self._port is not None and not self.is_open:
             self.open()
         return self
 
     def __exit__(self, *args, **kwargs):
         self.close()
 
     #  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -
 
     def send_break(self, duration=0.25):
         """\
         Send break condition. Timed, returns to idle state after given
         duration.
         """
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         self.break_condition = True
         time.sleep(duration)
         self.break_condition = False
 
     #  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -
     # backwards compatibility / deprecated functions
```

### Comparing `pyserial-labgrid-3.4.0.1/serial/serialwin32.py` & `pyserial-labgrid-3.5.0.2/serial/serialwin32.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #! python
 #
 # backend for Windows ("win32" incl. 32/64 bit support)
 #
-# (C) 2001-2015 Chris Liechti <cliechti@gmx.net>
+# (C) 2001-2020 Chris Liechti <cliechti@gmx.net>
 #
 # This file is part of pySerial. https://github.com/pyserial/pyserial
 # SPDX-License-Identifier:    BSD-3-Clause
 #
 # Initial patch to use ctypes by Giovanni Bajo <rasky@develer.com>
 
 from __future__ import absolute_import
 
 # pylint: disable=invalid-name,too-few-public-methods
 import ctypes
 import time
 from serial import win32
 
 import serial
-from serial.serialutil import SerialBase, SerialException, to_bytes, portNotOpenError, writeTimeoutError
+from serial.serialutil import SerialBase, SerialException, to_bytes, PortNotOpenError, SerialTimeoutException
 
 
 class Serial(SerialBase):
     """Serial port implementation for Win32 based on ctypes."""
 
     BAUDRATES = (50, 75, 110, 134, 150, 200, 300, 600, 1200, 1800, 2400, 4800,
                  9600, 19200, 38400, 57600, 115200)
@@ -180,31 +180,31 @@
                 comDCB.fRtsControl = win32.RTS_CONTROL_ENABLE if self._rts_state else win32.RTS_CONTROL_DISABLE
             comDCB.fOutxCtsFlow = self._rtscts
         else:
             # checks for unsupported settings
             # XXX verify if platform really does not have a setting for those
             if not self._rs485_mode.rts_level_for_tx:
                 raise ValueError(
-                    'Unsupported value for RS485Settings.rts_level_for_tx: {!r}'.format(
+                    'Unsupported value for RS485Settings.rts_level_for_tx: {!r} (only True is allowed)'.format(
                         self._rs485_mode.rts_level_for_tx,))
             if self._rs485_mode.rts_level_for_rx:
                 raise ValueError(
-                    'Unsupported value for RS485Settings.rts_level_for_rx: {!r}'.format(
+                    'Unsupported value for RS485Settings.rts_level_for_rx: {!r} (only False is allowed)'.format(
                         self._rs485_mode.rts_level_for_rx,))
             if self._rs485_mode.delay_before_tx is not None:
                 raise ValueError(
-                    'Unsupported value for RS485Settings.delay_before_tx: {!r}'.format(
+                    'Unsupported value for RS485Settings.delay_before_tx: {!r} (only None is allowed)'.format(
                         self._rs485_mode.delay_before_tx,))
             if self._rs485_mode.delay_before_rx is not None:
                 raise ValueError(
-                    'Unsupported value for RS485Settings.delay_before_rx: {!r}'.format(
+                    'Unsupported value for RS485Settings.delay_before_rx: {!r} (only None is allowed)'.format(
                         self._rs485_mode.delay_before_rx,))
             if self._rs485_mode.loopback:
                 raise ValueError(
-                    'Unsupported value for RS485Settings.loopback: {!r}'.format(
+                    'Unsupported value for RS485Settings.loopback: {!r} (only False is allowed)'.format(
                         self._rs485_mode.loopback,))
             comDCB.fRtsControl = win32.RTS_CONTROL_TOGGLE
             comDCB.fOutxCtsFlow = 0
 
         if self._dsrdtr:
             comDCB.fDtrControl = win32.DTR_CONTROL_HANDSHAKE
         else:
@@ -262,15 +262,15 @@
     def read(self, size=1):
         """\
         Read size bytes from the serial port. If a timeout is set it may
         return less characters as requested. With no timeout it will block
         until the requested number of bytes is read.
         """
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         if size > 0:
             win32.ResetEvent(self._overlapped_read.hEvent)
             flags = win32.DWORD()
             comstat = win32.COMSTAT()
             if not win32.ClearCommError(self._port_handle, ctypes.byref(flags), ctypes.byref(comstat)):
                 raise SerialException("ClearCommError failed ({!r})".format(ctypes.WinError()))
             n = min(comstat.cbInQue, size) if self.timeout == 0 else size
@@ -299,15 +299,15 @@
         else:
             read = bytes()
         return bytes(read)
 
     def write(self, data):
         """Output the given byte string over the serial port."""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         #~ if not isinstance(data, (bytes, bytearray)):
             #~ raise TypeError('expected %s or bytearray, got %s' % (bytes, type(data)))
         # convert data (needed in case of memoryview instance: Py 3.1 io lib), ctypes doesn't like memoryview
         data = to_bytes(data)
         if data:
             #~ win32event.ResetEvent(self._overlapped_write.hEvent)
             n = win32.DWORD()
@@ -318,15 +318,15 @@
 
                 # Wait for the write to complete.
                 #~ win32.WaitForSingleObject(self._overlapped_write.hEvent, win32.INFINITE)
                 win32.GetOverlappedResult(self._port_handle, self._overlapped_write, ctypes.byref(n), True)
                 if win32.GetLastError() == win32.ERROR_OPERATION_ABORTED:
                     return n.value  # canceled IO is no error
                 if n.value != len(data):
-                    raise writeTimeoutError
+                    raise SerialTimeoutException('Write timeout')
                 return n.value
             else:
                 errorcode = win32.ERROR_SUCCESS if success else win32.GetLastError()
                 if errorcode in (win32.ERROR_INVALID_USER_BUFFER, win32.ERROR_NOT_ENOUGH_MEMORY,
                                  win32.ERROR_OPERATION_ABORTED):
                     return 0
                 elif errorcode in (win32.ERROR_SUCCESS, win32.ERROR_IO_PENDING):
@@ -347,30 +347,30 @@
         # XXX could also use WaitCommEvent with mask EV_TXEMPTY, but it would
         # require overlapped IO and it's also only possible to set a single mask
         # on the port---
 
     def reset_input_buffer(self):
         """Clear input buffer, discarding all that is in the buffer."""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         win32.PurgeComm(self._port_handle, win32.PURGE_RXCLEAR | win32.PURGE_RXABORT)
 
     def reset_output_buffer(self):
         """\
         Clear output buffer, aborting the current output and discarding all
         that is in the buffer.
         """
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         win32.PurgeComm(self._port_handle, win32.PURGE_TXCLEAR | win32.PURGE_TXABORT)
 
     def _update_break_state(self):
         """Set break: Controls TXD. When active, to transmitting is possible."""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         if self._break_state:
             win32.SetCommBreak(self._port_handle)
         else:
             win32.ClearCommBreak(self._port_handle)
 
     def _update_rts_state(self):
         """Set terminal status line: Request To Send"""
@@ -384,15 +384,15 @@
         if self._dtr_state:
             win32.EscapeCommFunction(self._port_handle, win32.SETDTR)
         else:
             win32.EscapeCommFunction(self._port_handle, win32.CLRDTR)
 
     def _GetCommModemStatus(self):
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         stat = win32.DWORD()
         win32.GetCommModemStatus(self._port_handle, ctypes.byref(stat))
         return stat.value
 
     @property
     def cts(self):
         """Read terminal status line: Clear To Send"""
@@ -428,15 +428,15 @@
         """\
         Manually control flow - when software flow control is enabled.
         This will do the same as if XON (true) or XOFF (false) are received
         from the other device and control the transmission accordingly.
         WARNING: this function is not portable to different platforms!
         """
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         if enable:
             win32.EscapeCommFunction(self._port_handle, win32.SETXON)
         else:
             win32.EscapeCommFunction(self._port_handle, win32.SETXOFF)
 
     @property
     def out_waiting(self):
```

### Comparing `pyserial-labgrid-3.4.0.1/serial/threaded/__init__.py` & `pyserial-labgrid-3.5.0.2/serial/threaded/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,28 +199,28 @@
             except serial.SerialException as e:
                 # probably some I/O problem such as disconnected USB serial
                 # adapters -> exit
                 error = e
                 break
             else:
                 if data:
-                    # make a separated try-except for called used code
+                    # make a separated try-except for called user code
                     try:
                         self.protocol.data_received(data)
                     except Exception as e:
                         error = e
                         break
         self.alive = False
         self.protocol.connection_lost(error)
         self.protocol = None
 
     def write(self, data):
         """Thread safe writing (uses lock)"""
         with self._lock:
-            self.serial.write(data)
+            return self.serial.write(data)
 
     def close(self):
         """Close the serial port and exit reader thread (uses lock)"""
         # use the lock to let other threads finish writing
         with self._lock:
             # first stop reading, so that closing can be done on idle port
             self.stop()
```

### Comparing `pyserial-labgrid-3.4.0.1/serial/tools/hexlify_codec.py` & `pyserial-labgrid-3.5.0.2/serial/tools/hexlify_codec.py`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/serial/tools/list_ports.py` & `pyserial-labgrid-3.5.0.2/serial/tools/list_ports.py`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/serial/tools/list_ports_common.py` & `pyserial-labgrid-3.5.0.2/serial/tools/list_ports_common.py`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/serial/tools/list_ports_linux.py` & `pyserial-labgrid-3.5.0.2/serial/tools/list_ports_linux.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             if num_if > 1:  # multi interface devices like FT4232
                 self.location = os.path.basename(self.usb_interface_path)
             else:
                 self.location = os.path.basename(self.usb_device_path)
 
             self.manufacturer = self.read_line(self.usb_device_path, 'manufacturer')
             self.product = self.read_line(self.usb_device_path, 'product')
-            self.interface = self.read_line(self.device_path, 'interface')
+            self.interface = self.read_line(self.usb_interface_path, 'interface')
 
         if self.subsystem in ('usb', 'usb-serial'):
             self.apply_usb_info()
         #~ elif self.subsystem in ('pnp', 'amba'):  # PCI based devices, raspi
         elif self.subsystem == 'pnp':  # PCI based devices
             self.description = self.name
             self.hwid = self.read_line(self.device_path, 'id')
@@ -101,9 +101,9 @@
     return [info
             for info in [SysFS(d) for d in devices]
             if info.subsystem != "platform"]    # hide non-present internal serial ports
 
 # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 # test
 if __name__ == '__main__':
-    for port, desc, hwid in sorted(comports()):
-        print("{}: {} [{}]".format(port, desc, hwid))
+    for info in sorted(comports()):
+        print("{0}: {0.subsystem}".format(info))
```

### Comparing `pyserial-labgrid-3.4.0.1/serial/tools/list_ports_osx.py` & `pyserial-labgrid-3.5.0.2/serial/tools/list_ports_osx.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This is a module that gathers a list of serial ports including details on OSX
 #
 # code originally from https://github.com/makerbot/pyserial/tree/master/serial/tools
 # with contributions from cibomahto, dgs3, FarMcKon, tedbrandston
 # and modifications by cliechti, hoihu, hardkrash
 #
 # This file is part of pySerial. https://github.com/pyserial/pyserial
-# (C) 2013-2015
+# (C) 2013-2020
 #
 # SPDX-License-Identifier:    BSD-3-Clause
 
 
 # List all of the callout devices in OS/X by querying IOKit.
 
 # See the following for a reference of how to do this:
@@ -20,54 +20,72 @@
 # More help from darwin_hid.py
 
 # Also see the 'IORegistryExplorer' for an idea of what we are actually searching
 
 from __future__ import absolute_import
 
 import ctypes
-import ctypes.util
 
 from serial.tools import list_ports_common
 
-iokit = ctypes.cdll.LoadLibrary(ctypes.util.find_library('IOKit'))
-cf = ctypes.cdll.LoadLibrary(ctypes.util.find_library('CoreFoundation'))
+iokit = ctypes.cdll.LoadLibrary('/System/Library/Frameworks/IOKit.framework/IOKit')
+cf = ctypes.cdll.LoadLibrary('/System/Library/Frameworks/CoreFoundation.framework/CoreFoundation')
 
-kIOMasterPortDefault = ctypes.c_void_p.in_dll(iokit, "kIOMasterPortDefault")
+# kIOMasterPortDefault is no longer exported in BigSur but no biggie, using NULL works just the same
+kIOMasterPortDefault = 0 # WAS: ctypes.c_void_p.in_dll(iokit, "kIOMasterPortDefault")
 kCFAllocatorDefault = ctypes.c_void_p.in_dll(cf, "kCFAllocatorDefault")
 
 kCFStringEncodingMacRoman = 0
+kCFStringEncodingUTF8 = 0x08000100
+
+# defined in `IOKit/usb/USBSpec.h`
+kUSBVendorString = 'USB Vendor Name'
+kUSBSerialNumberString = 'USB Serial Number'
+
+# `io_name_t` defined as `typedef char io_name_t[128];`
+# in `device/device_types.h`
+io_name_size = 128
+
+# defined in `mach/kern_return.h`
+KERN_SUCCESS = 0
+# kern_return_t defined as `typedef int kern_return_t;` in `mach/i386/kern_return.h`
+kern_return_t = ctypes.c_int
 
 iokit.IOServiceMatching.restype = ctypes.c_void_p
 
 iokit.IOServiceGetMatchingServices.argtypes = [ctypes.c_void_p, ctypes.c_void_p, ctypes.c_void_p]
-iokit.IOServiceGetMatchingServices.restype = ctypes.c_void_p
+iokit.IOServiceGetMatchingServices.restype = kern_return_t
 
 iokit.IORegistryEntryGetParentEntry.argtypes = [ctypes.c_void_p, ctypes.c_void_p, ctypes.c_void_p]
+iokit.IOServiceGetMatchingServices.restype = kern_return_t
 
 iokit.IORegistryEntryCreateCFProperty.argtypes = [ctypes.c_void_p, ctypes.c_void_p, ctypes.c_void_p, ctypes.c_uint32]
 iokit.IORegistryEntryCreateCFProperty.restype = ctypes.c_void_p
 
 iokit.IORegistryEntryGetPath.argtypes = [ctypes.c_void_p, ctypes.c_void_p, ctypes.c_void_p]
-iokit.IORegistryEntryGetPath.restype = ctypes.c_void_p
+iokit.IORegistryEntryGetPath.restype = kern_return_t
 
 iokit.IORegistryEntryGetName.argtypes = [ctypes.c_void_p, ctypes.c_void_p]
-iokit.IORegistryEntryGetName.restype = ctypes.c_void_p
+iokit.IORegistryEntryGetName.restype = kern_return_t
 
 iokit.IOObjectGetClass.argtypes = [ctypes.c_void_p, ctypes.c_void_p]
-iokit.IOObjectGetClass.restype = ctypes.c_void_p
+iokit.IOObjectGetClass.restype = kern_return_t
 
 iokit.IOObjectRelease.argtypes = [ctypes.c_void_p]
 
 
 cf.CFStringCreateWithCString.argtypes = [ctypes.c_void_p, ctypes.c_char_p, ctypes.c_int32]
 cf.CFStringCreateWithCString.restype = ctypes.c_void_p
 
 cf.CFStringGetCStringPtr.argtypes = [ctypes.c_void_p, ctypes.c_uint32]
 cf.CFStringGetCStringPtr.restype = ctypes.c_char_p
 
+cf.CFStringGetCString.argtypes = [ctypes.c_void_p, ctypes.c_void_p, ctypes.c_long, ctypes.c_uint32]
+cf.CFStringGetCString.restype = ctypes.c_bool
+
 cf.CFNumberGetValue.argtypes = [ctypes.c_void_p, ctypes.c_uint32, ctypes.c_void_p]
 cf.CFNumberGetValue.restype = ctypes.c_void_p
 
 # void CFRelease ( CFTypeRef cf );
 cf.CFRelease.argtypes = [ctypes.c_void_p]
 cf.CFRelease.restype = None
 
@@ -84,28 +102,33 @@
 
     @param device_type Type of Device
     @param property String to search for
     @return Python string containing the value, or None if not found.
     """
     key = cf.CFStringCreateWithCString(
             kCFAllocatorDefault,
-            property.encode("mac_roman"),
-            kCFStringEncodingMacRoman)
+            property.encode("utf-8"),
+            kCFStringEncodingUTF8)
 
     CFContainer = iokit.IORegistryEntryCreateCFProperty(
             device_type,
             key,
             kCFAllocatorDefault,
             0)
     output = None
 
     if CFContainer:
         output = cf.CFStringGetCStringPtr(CFContainer, 0)
         if output is not None:
-            output = output.decode('mac_roman')
+            output = output.decode('utf-8')
+        else:
+            buffer = ctypes.create_string_buffer(io_name_size);
+            success = cf.CFStringGetCString(CFContainer, ctypes.byref(buffer), io_name_size, kCFStringEncodingUTF8)
+            if success:
+                output = buffer.value.decode('utf-8')
         cf.CFRelease(CFContainer)
     return output
 
 
 def get_int_property(device_type, property, cf_number_type):
     """
     Search the given device for the specified string property
@@ -114,16 +137,16 @@
     @param property String to search for
     @param cf_number_type CFType number
 
     @return Python string containing the value, or None if not found.
     """
     key = cf.CFStringCreateWithCString(
             kCFAllocatorDefault,
-            property.encode("mac_roman"),
-            kCFStringEncodingMacRoman)
+            property.encode("utf-8"),
+            kCFStringEncodingUTF8)
 
     CFContainer = iokit.IORegistryEntryCreateCFProperty(
             device_type,
             key,
             kCFAllocatorDefault,
             0)
 
@@ -133,50 +156,57 @@
         elif (cf_number_type == kCFNumberSInt16Type):
             number = ctypes.c_uint16()
         cf.CFNumberGetValue(CFContainer, cf_number_type, ctypes.byref(number))
         cf.CFRelease(CFContainer)
         return number.value
     return None
 
-
 def IORegistryEntryGetName(device):
-    pathname = ctypes.create_string_buffer(100)  # TODO: Is this ok?
-    iokit.IOObjectGetClass(device, ctypes.byref(pathname))
-    return pathname.value
-
+    devicename = ctypes.create_string_buffer(io_name_size);
+    res = iokit.IORegistryEntryGetName(device, ctypes.byref(devicename))
+    if res != KERN_SUCCESS:
+        return None
+    # this works in python2 but may not be valid. Also I don't know if
+    # this encoding is guaranteed. It may be dependent on system locale.
+    return devicename.value.decode('utf-8')
+
+def IOObjectGetClass(device):
+    classname = ctypes.create_string_buffer(io_name_size)
+    iokit.IOObjectGetClass(device, ctypes.byref(classname))
+    return classname.value
 
 def GetParentDeviceByType(device, parent_type):
     """ Find the first parent of a device that implements the parent_type
         @param IOService Service to inspect
         @return Pointer to the parent type, or None if it was not found.
     """
     # First, try to walk up the IOService tree to find a parent of this device that is a IOUSBDevice.
-    parent_type = parent_type.encode('mac_roman')
-    while IORegistryEntryGetName(device) != parent_type:
+    parent_type = parent_type.encode('utf-8')
+    while IOObjectGetClass(device) != parent_type:
         parent = ctypes.c_void_p()
         response = iokit.IORegistryEntryGetParentEntry(
                 device,
-                "IOService".encode("mac_roman"),
+                "IOService".encode("utf-8"),
                 ctypes.byref(parent))
         # If we weren't able to find a parent for the device, we're done.
-        if response != 0:
+        if response != KERN_SUCCESS:
             return None
         device = parent
     return device
 
 
 def GetIOServicesByType(service_type):
     """
     returns iterator over specified service_type
     """
     serial_port_iterator = ctypes.c_void_p()
 
     iokit.IOServiceGetMatchingServices(
             kIOMasterPortDefault,
-            iokit.IOServiceMatching(service_type.encode('mac_roman')),
+            iokit.IOServiceMatching(service_type.encode('utf-8')),
             ctypes.byref(serial_port_iterator))
 
     services = []
     while iokit.IOIteratorIsValid(serial_port_iterator):
         service = iokit.IOIteratorNext(serial_port_iterator)
         if not service:
             break
@@ -237,22 +267,29 @@
     serial_interfaces = scan_interfaces()
     for service in services:
         # First, add the callout device file.
         device = get_string_property(service, "IOCalloutDevice")
         if device:
             info = list_ports_common.ListPortInfo(device)
             # If the serial port is implemented by IOUSBDevice
-            usb_device = GetParentDeviceByType(service, "IOUSBDevice")
+            # NOTE IOUSBDevice was deprecated as of 10.11 and finally on Apple Silicon
+            # devices has been completely removed.  Thanks to @oskay for this patch.
+            usb_device = GetParentDeviceByType(service, "IOUSBHostDevice")
+            if not usb_device:
+                usb_device = GetParentDeviceByType(service, "IOUSBDevice")
             if usb_device:
                 # fetch some useful informations from properties
                 info.vid = get_int_property(usb_device, "idVendor", kCFNumberSInt16Type)
                 info.pid = get_int_property(usb_device, "idProduct", kCFNumberSInt16Type)
-                info.serial_number = get_string_property(usb_device, "USB Serial Number")
-                info.product = get_string_property(usb_device, "USB Product Name") or 'n/a'
-                info.manufacturer = get_string_property(usb_device, "USB Vendor Name")
+                info.serial_number = get_string_property(usb_device, kUSBSerialNumberString)
+                # We know this is a usb device, so the
+                # IORegistryEntryName should always be aliased to the
+                # usb product name string descriptor.
+                info.product = IORegistryEntryGetName(usb_device) or 'n/a'
+                info.manufacturer = get_string_property(usb_device, kUSBVendorString)
                 locationID = get_int_property(usb_device, "locationID", kCFNumberSInt32Type)
                 info.location = location_to_string(locationID)
                 info.interface = search_for_locationID_in_interfaces(serial_interfaces, locationID)
                 info.apply_usb_info()
             ports.append(info)
     return ports
```

### Comparing `pyserial-labgrid-3.4.0.1/serial/tools/list_ports_posix.py` & `pyserial-labgrid-3.5.0.2/serial/tools/list_ports_posix.py`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/serial/tools/list_ports_windows.py` & `pyserial-labgrid-3.5.0.2/serial/tools/list_ports_windows.py`

 * *Files 24% similar despite different names*

```diff
@@ -114,41 +114,155 @@
 RegCloseKey.argtypes = [HKEY]
 RegCloseKey.restype = LONG
 
 RegQueryValueEx = advapi32.RegQueryValueExW
 RegQueryValueEx.argtypes = [HKEY, LPCTSTR, LPDWORD, LPDWORD, LPBYTE, LPDWORD]
 RegQueryValueEx.restype = LONG
 
+cfgmgr32 = ctypes.windll.LoadLibrary("Cfgmgr32")
+CM_Get_Parent = cfgmgr32.CM_Get_Parent
+CM_Get_Parent.argtypes = [PDWORD, DWORD, ULONG]
+CM_Get_Parent.restype = LONG
+
+CM_Get_Device_IDW = cfgmgr32.CM_Get_Device_IDW
+CM_Get_Device_IDW.argtypes = [DWORD, PTSTR, ULONG, ULONG]
+CM_Get_Device_IDW.restype = LONG
+
+CM_MapCrToWin32Err = cfgmgr32.CM_MapCrToWin32Err
+CM_MapCrToWin32Err.argtypes = [DWORD, DWORD]
+CM_MapCrToWin32Err.restype = DWORD
+
 
 DIGCF_PRESENT = 2
 DIGCF_DEVICEINTERFACE = 16
 INVALID_HANDLE_VALUE = 0
 ERROR_INSUFFICIENT_BUFFER = 122
+ERROR_NOT_FOUND = 1168
 SPDRP_HARDWAREID = 1
 SPDRP_FRIENDLYNAME = 12
 SPDRP_LOCATION_PATHS = 35
 SPDRP_MFG = 11
 DICS_FLAG_GLOBAL = 1
 DIREG_DEV = 0x00000001
 KEY_READ = 0x20019
 
 
+MAX_USB_DEVICE_TREE_TRAVERSAL_DEPTH = 5
+
+
+def get_parent_serial_number(child_devinst, child_vid, child_pid, depth=0, last_serial_number=None):
+    """ Get the serial number of the parent of a device.
+
+    Args:
+        child_devinst: The device instance handle to get the parent serial number of.
+        child_vid: The vendor ID of the child device.
+        child_pid: The product ID of the child device.
+        depth: The current iteration depth of the USB device tree.
+    """
+
+    # If the traversal depth is beyond the max, abandon attempting to find the serial number.
+    if depth > MAX_USB_DEVICE_TREE_TRAVERSAL_DEPTH:
+        return '' if not last_serial_number else last_serial_number
+
+    # Get the parent device instance.
+    devinst = DWORD()
+    ret = CM_Get_Parent(ctypes.byref(devinst), child_devinst, 0)
+
+    if ret:
+        win_error = CM_MapCrToWin32Err(DWORD(ret), DWORD(0))
+
+        # If there is no parent available, the child was the root device. We cannot traverse
+        # further.
+        if win_error == ERROR_NOT_FOUND:
+            return '' if not last_serial_number else last_serial_number
+
+        raise ctypes.WinError(win_error)
+
+    # Get the ID of the parent device and parse it for vendor ID, product ID, and serial number.
+    parentHardwareID = ctypes.create_unicode_buffer(250)
+
+    ret = CM_Get_Device_IDW(
+        devinst,
+        parentHardwareID,
+        ctypes.sizeof(parentHardwareID) - 1,
+        0)
+
+    if ret:
+        raise ctypes.WinError(CM_MapCrToWin32Err(DWORD(ret), DWORD(0)))
+
+    parentHardwareID_str = parentHardwareID.value
+    m = re.search(r'VID_([0-9a-f]{4})(&PID_([0-9a-f]{4}))?(&MI_(\d{2}))?(\\(.*))?',
+                  parentHardwareID_str,
+                  re.I)
+
+    # return early if we have no matches (likely malformed serial, traversed too far)
+    if not m:
+        return '' if not last_serial_number else last_serial_number
+
+    vid = None
+    pid = None
+    serial_number = None
+    if m.group(1):
+        vid = int(m.group(1), 16)
+    if m.group(3):
+        pid = int(m.group(3), 16)
+    if m.group(7):
+        serial_number = m.group(7)
+
+    # store what we found as a fallback for malformed serial values up the chain
+    found_serial_number = serial_number
+
+    # Check that the USB serial number only contains alpha-numeric characters. It may be a windows
+    # device ID (ephemeral ID).
+    if serial_number and not re.match(r'^\w+$', serial_number):
+        serial_number = None
+
+    if not vid or not pid:
+        # If pid and vid are not available at this device level, continue to the parent.
+        return get_parent_serial_number(devinst, child_vid, child_pid, depth + 1, found_serial_number)
+
+    if pid != child_pid or vid != child_vid:
+        # If the VID or PID has changed, we are no longer looking at the same physical device. The
+        # serial number is unknown.
+        return '' if not last_serial_number else last_serial_number
+
+    # In this case, the vid and pid of the parent device are identical to the child. However, if
+    # there still isn't a serial number available, continue to the next parent.
+    if not serial_number:
+        return get_parent_serial_number(devinst, child_vid, child_pid, depth + 1, found_serial_number)
+
+    # Finally, the VID and PID are identical to the child and a serial number is present, so return
+    # it.
+    return serial_number
+
+
 def iterate_comports():
     """Return a generator that yields descriptions for serial ports"""
-    GUIDs = (GUID * 8)()  # so far only seen one used, so hope 8 are enough...
-    guids_size = DWORD()
+    PortsGUIDs = (GUID * 8)()  # so far only seen one used, so hope 8 are enough...
+    ports_guids_size = DWORD()
     if not SetupDiClassGuidsFromName(
             "Ports",
-            GUIDs,
-            ctypes.sizeof(GUIDs),
-            ctypes.byref(guids_size)):
+            PortsGUIDs,
+            ctypes.sizeof(PortsGUIDs),
+            ctypes.byref(ports_guids_size)):
         raise ctypes.WinError()
 
+    ModemsGUIDs = (GUID * 8)()  # so far only seen one used, so hope 8 are enough...
+    modems_guids_size = DWORD()
+    if not SetupDiClassGuidsFromName(
+            "Modem",
+            ModemsGUIDs,
+            ctypes.sizeof(ModemsGUIDs),
+            ctypes.byref(modems_guids_size)):
+        raise ctypes.WinError()
+
+    GUIDs = PortsGUIDs[:ports_guids_size.value] + ModemsGUIDs[:modems_guids_size.value]
+
     # repeat for all possible GUIDs
-    for index in range(guids_size.value):
+    for index in range(len(GUIDs)):
         bInterfaceNumber = None
         g_hdi = SetupDiGetClassDevs(
             ctypes.byref(GUIDs[index]),
             None,
             NULL,
             DIGCF_PRESENT)  # was DIGCF_PRESENT|DIGCF_DEVICEINTERFACE which misses CDC ports
 
@@ -209,23 +323,29 @@
             szHardwareID_str = szHardwareID.value
 
             info = list_ports_common.ListPortInfo(port_name_buffer.value, skip_link_detection=True)
 
             # in case of USB, make a more readable string, similar to that form
             # that we also generate on other platforms
             if szHardwareID_str.startswith('USB'):
-                m = re.search(r'VID_([0-9a-f]{4})(&PID_([0-9a-f]{4}))?(&MI_(\d{2}))?(\\(\w+))?', szHardwareID_str, re.I)
+                m = re.search(r'VID_([0-9a-f]{4})(&PID_([0-9a-f]{4}))?(&MI_(\d{2}))?(\\(.*))?', szHardwareID_str, re.I)
                 if m:
                     info.vid = int(m.group(1), 16)
                     if m.group(3):
                         info.pid = int(m.group(3), 16)
                     if m.group(5):
                         bInterfaceNumber = int(m.group(5))
-                    if m.group(7):
+
+                    # Check that the USB serial number only contains alpha-numeric characters. It
+                    # may be a windows device ID (ephemeral ID) for composite devices.
+                    if m.group(7) and re.match(r'^\w+$', m.group(7)):
                         info.serial_number = m.group(7)
+                    else:
+                        info.serial_number = get_parent_serial_number(devinfo.DevInst, info.vid, info.pid)
+
                 # calculate a location string
                 loc_path_str = ctypes.create_unicode_buffer(250)
                 if SetupDiGetDeviceRegistryProperty(
                         g_hdi,
                         ctypes.byref(devinfo),
                         SPDRP_LOCATION_PATHS,
                         None,
```

### Comparing `pyserial-labgrid-3.4.0.1/serial/tools/miniterm.py` & `pyserial-labgrid-3.5.0.2/serial/tools/miniterm.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 #
 # Very simple serial terminal
 #
 # This file is part of pySerial. https://github.com/pyserial/pyserial
-# (C)2002-2017 Chris Liechti <cliechti@gmx.net>
+# (C)2002-2020 Chris Liechti <cliechti@gmx.net>
 #
 # SPDX-License-Identifier:    BSD-3-Clause
 
 from __future__ import absolute_import
 
 import codecs
 import os
@@ -84,51 +84,103 @@
     def __exit__(self, *args, **kwargs):
         self.setup()
 
 
 if os.name == 'nt':  # noqa
     import msvcrt
     import ctypes
+    import platform
 
     class Out(object):
         """file-like wrapper that uses os.write"""
 
         def __init__(self, fd):
             self.fd = fd
 
         def flush(self):
             pass
 
         def write(self, s):
             os.write(self.fd, s)
 
     class Console(ConsoleBase):
+        fncodes = {
+            ';': '\1bOP',  # F1
+            '<': '\1bOQ',  # F2
+            '=': '\1bOR',  # F3
+            '>': '\1bOS',  # F4
+            '?': '\1b[15~',  # F5
+            '@': '\1b[17~',  # F6
+            'A': '\1b[18~',  # F7
+            'B': '\1b[19~',  # F8
+            'C': '\1b[20~',  # F9
+            'D': '\1b[21~',  # F10
+        }
+        navcodes = {
+            'H': '\x1b[A',  # UP
+            'P': '\x1b[B',  # DOWN
+            'K': '\x1b[D',  # LEFT
+            'M': '\x1b[C',  # RIGHT
+            'G': '\x1b[H',  # HOME
+            'O': '\x1b[F',  # END
+            'R': '\x1b[2~',  # INSERT
+            'S': '\x1b[3~',  # DELETE
+            'I': '\x1b[5~',  # PGUP
+            'Q': '\x1b[6~',  # PGDN        
+        }
+        
         def __init__(self):
             super(Console, self).__init__()
             self._saved_ocp = ctypes.windll.kernel32.GetConsoleOutputCP()
             self._saved_icp = ctypes.windll.kernel32.GetConsoleCP()
             ctypes.windll.kernel32.SetConsoleOutputCP(65001)
             ctypes.windll.kernel32.SetConsoleCP(65001)
+            # ANSI handling available through SetConsoleMode since Windows 10 v1511 
+            # https://en.wikipedia.org/wiki/ANSI_escape_code#cite_note-win10th2-1
+            if platform.release() == '10' and int(platform.version().split('.')[2]) > 10586:
+                ENABLE_VIRTUAL_TERMINAL_PROCESSING = 0x0004
+                import ctypes.wintypes as wintypes
+                if not hasattr(wintypes, 'LPDWORD'): # PY2
+                    wintypes.LPDWORD = ctypes.POINTER(wintypes.DWORD)
+                SetConsoleMode = ctypes.windll.kernel32.SetConsoleMode
+                GetConsoleMode = ctypes.windll.kernel32.GetConsoleMode
+                GetStdHandle = ctypes.windll.kernel32.GetStdHandle
+                mode = wintypes.DWORD()
+                GetConsoleMode(GetStdHandle(-11), ctypes.byref(mode))
+                if (mode.value & ENABLE_VIRTUAL_TERMINAL_PROCESSING) == 0:
+                    SetConsoleMode(GetStdHandle(-11), mode.value | ENABLE_VIRTUAL_TERMINAL_PROCESSING)
+                    self._saved_cm = mode
             self.output = codecs.getwriter('UTF-8')(Out(sys.stdout.fileno()), 'replace')
             # the change of the code page is not propagated to Python, manually fix it
             sys.stderr = codecs.getwriter('UTF-8')(Out(sys.stderr.fileno()), 'replace')
             sys.stdout = self.output
             self.output.encoding = 'UTF-8'  # needed for input
 
         def __del__(self):
             ctypes.windll.kernel32.SetConsoleOutputCP(self._saved_ocp)
             ctypes.windll.kernel32.SetConsoleCP(self._saved_icp)
+            try:
+                ctypes.windll.kernel32.SetConsoleMode(ctypes.windll.kernel32.GetStdHandle(-11), self._saved_cm)
+            except AttributeError: # in case no _saved_cm
+                pass
 
         def getkey(self):
             while True:
                 z = msvcrt.getwch()
                 if z == unichr(13):
                     return unichr(10)
-                elif z in (unichr(0), unichr(0x0e)):    # functions keys, ignore
-                    msvcrt.getwch()
+                elif z is unichr(0) or z is unichr(0xe0):
+                    try:
+                        code = msvcrt.getwch()
+                        if z is unichr(0):
+                            return self.fncodes[code]
+                        else:
+                            return self.navcodes[code]
+                    except KeyError:
+                        pass
                 else:
                     return z
 
         def cancel(self):
             # CancelIo, CancelSynchronousIo do not seem to work when using
             # getwch, so instead, send a key to the window with the console
             hwnd = ctypes.windll.kernel32.GetConsoleWindow()
@@ -533,15 +585,15 @@
             self.change_encoding()
         elif c == '\x09':                       # CTRL+I -> info
             self.dump_port_settings()
         #~ elif c == '\x01':                       # CTRL+A -> cycle escape mode
         #~ elif c == '\x0c':                       # CTRL+L -> cycle linefeed mode
         elif c in 'pP':                         # P -> change port
             self.change_port()
-        elif c in 'sS':                         # S -> suspend / open port temporarily
+        elif c in 'zZ':                         # S -> suspend / open port temporarily
             self.suspend_port()
         elif c in 'bB':                         # B -> change baudrate
             self.change_baudrate()
         elif c == '8':                          # 8 -> change to 8 bits
             self.serial.bytesize = serial.EIGHTBITS
             self.dump_port_settings()
         elif c == '7':                          # 7 -> change to 8 bits
@@ -573,14 +625,16 @@
             self.dump_port_settings()
         elif c in 'xX':                         # X -> change software flow control
             self.serial.xonxoff = (c == 'X')
             self.dump_port_settings()
         elif c in 'rR':                         # R -> change hardware flow control
             self.serial.rtscts = (c == 'R')
             self.dump_port_settings()
+        elif c in 'qQ':
+            self.stop()                         # Q -> exit app
         else:
             sys.stderr.write('--- unknown menu character {} --\n'.format(key_description(c)))
 
     def upload_file(self):
         """Ask user for filenname and send its contents"""
         sys.stderr.write('\n--- File to upload: ')
         sys.stderr.flush()
@@ -714,15 +768,15 @@
 
     def get_help_text(self):
         """return the help text"""
         # help text, starts with blank line!
         return """
 --- pySerial ({version}) - miniterm - help
 ---
---- {exit:8} Exit program
+--- {exit:8} Exit program (alias {menu} Q)
 --- {menu:8} Menu escape key, followed by:
 --- Menu keys:
 ---    {menu:7} Send the menu character itself to remote
 ---    {exit:7} Send the exit character itself to remote
 ---    {info:7} Show info
 ---    {upload:7} Upload file (prompt will be shown)
 ---    {repr:7} encoding
```

### Comparing `pyserial-labgrid-3.4.0.1/serial/urlhandler/protocol_alt.py` & `pyserial-labgrid-3.5.0.2/serial/urlhandler/protocol_alt.py`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/serial/urlhandler/protocol_hwgrep.py` & `pyserial-labgrid-3.5.0.2/serial/urlhandler/protocol_hwgrep.py`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/serial/urlhandler/protocol_loop.py` & `pyserial-labgrid-3.5.0.2/serial/urlhandler/protocol_loop.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # This module implements a loop back connection receiving itself what it sent.
 #
 # The purpose of this module is.. well... You can run the unit tests with it.
 # and it was so easy to implement ;-)
 #
 # This file is part of pySerial. https://github.com/pyserial/pyserial
-# (C) 2001-2015 Chris Liechti <cliechti@gmx.net>
+# (C) 2001-2020 Chris Liechti <cliechti@gmx.net>
 #
 # SPDX-License-Identifier:    BSD-3-Clause
 #
 # URL format:    loop://[option[/option...]]
 # options:
 # - "debug" print diagnostic messages
 from __future__ import absolute_import
@@ -23,15 +23,15 @@
 except ImportError:
     import urllib.parse as urlparse
 try:
     import queue
 except ImportError:
     import Queue as queue
 
-from serial.serialutil import SerialBase, SerialException, to_bytes, iterbytes, writeTimeoutError, portNotOpenError
+from serial.serialutil import SerialBase, SerialException, to_bytes, iterbytes, SerialTimeoutException, PortNotOpenError
 
 # map log level names to constants. used in from_url()
 LOGGER_LEVELS = {
     'debug': logging.DEBUG,
     'info': logging.INFO,
     'warning': logging.WARNING,
     'error': logging.ERROR,
@@ -123,29 +123,29 @@
 
     #  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -
 
     @property
     def in_waiting(self):
         """Return the number of bytes currently in the input buffer."""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         if self.logger:
             # attention the logged value can differ from return value in
             # threaded environments...
             self.logger.debug('in_waiting -> {:d}'.format(self.queue.qsize()))
         return self.queue.qsize()
 
     def read(self, size=1):
         """\
         Read size bytes from the serial port. If a timeout is set it may
         return less characters as requested. With no timeout it will block
         until the requested number of bytes is read.
         """
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         if self._timeout is not None and self._timeout != 0:
             timeout = time.time() + self._timeout
         else:
             timeout = None
         data = bytearray()
         while size > 0 and self.is_open:
             try:
@@ -177,60 +177,71 @@
         """\
         Output the given byte string over the serial port. Can block if the
         connection is blocked. May raise SerialException if the connection is
         closed.
         """
         self._cancel_write = False
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         data = to_bytes(data)
         # calculate aprox time that would be used to send the data
         time_used_to_send = 10.0 * len(data) / self._baudrate
         # when a write timeout is configured check if we would be successful
         # (not sending anything, not even the part that would have time)
         if self._write_timeout is not None and time_used_to_send > self._write_timeout:
             # must wait so that unit test succeeds
             time_left = self._write_timeout
             while time_left > 0 and not self._cancel_write:
                 time.sleep(min(time_left, 0.5))
                 time_left -= 0.5
             if self._cancel_write:
                 return 0  # XXX
-            raise writeTimeoutError
+            raise SerialTimeoutException('Write timeout')
         for byte in iterbytes(data):
             self.queue.put(byte, timeout=self._write_timeout)
         return len(data)
 
     def reset_input_buffer(self):
         """Clear input buffer, discarding all that is in the buffer."""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         if self.logger:
             self.logger.info('reset_input_buffer()')
         try:
             while self.queue.qsize():
                 self.queue.get_nowait()
         except queue.Empty:
             pass
 
     def reset_output_buffer(self):
         """\
         Clear output buffer, aborting the current output and
         discarding all that is in the buffer.
         """
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         if self.logger:
             self.logger.info('reset_output_buffer()')
         try:
             while self.queue.qsize():
                 self.queue.get_nowait()
         except queue.Empty:
             pass
 
+    @property
+    def out_waiting(self):
+        """Return how many bytes the in the outgoing buffer"""
+        if not self.is_open:
+            raise PortNotOpenError()
+        if self.logger:
+            # attention the logged value can differ from return value in
+            # threaded environments...
+            self.logger.debug('out_waiting -> {:d}'.format(self.queue.qsize()))
+        return self.queue.qsize()
+
     def _update_break_state(self):
         """\
         Set break: Controls TXD. When active, to transmitting is
         possible.
         """
         if self.logger:
             self.logger.info('_update_break_state({!r})'.format(self._break_state))
@@ -245,15 +256,15 @@
         if self.logger:
             self.logger.info('_update_dtr_state({!r}) -> state of DSR'.format(self._dtr_state))
 
     @property
     def cts(self):
         """Read terminal status line: Clear To Send"""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         if self.logger:
             self.logger.info('CTS -> state of RTS ({!r})'.format(self._rts_state))
         return self._rts_state
 
     @property
     def dsr(self):
         """Read terminal status line: Data Set Ready"""
@@ -261,24 +272,24 @@
             self.logger.info('DSR -> state of DTR ({!r})'.format(self._dtr_state))
         return self._dtr_state
 
     @property
     def ri(self):
         """Read terminal status line: Ring Indicator"""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         if self.logger:
             self.logger.info('returning dummy for RI')
         return False
 
     @property
     def cd(self):
         """Read terminal status line: Carrier Detect"""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         if self.logger:
             self.logger.info('returning dummy for CD')
         return True
 
     # - - - platform specific - - -
     # None so far
```

### Comparing `pyserial-labgrid-3.4.0.1/serial/urlhandler/protocol_socket.py` & `pyserial-labgrid-3.5.0.2/serial/urlhandler/protocol_socket.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import time
 try:
     import urlparse
 except ImportError:
     import urllib.parse as urlparse
 
 from serial.serialutil import SerialBase, SerialException, to_bytes, \
-    portNotOpenError, writeTimeoutError, Timeout
+    PortNotOpenError, SerialTimeoutException, Timeout
 
 # map log level names to constants. used in from_url()
 LOGGER_LEVELS = {
     'debug': logging.DEBUG,
     'info': logging.INFO,
     'warning': logging.WARNING,
     'error': logging.ERROR,
@@ -132,15 +132,15 @@
 
     #  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -
 
     @property
     def in_waiting(self):
         """Return the number of bytes currently in the input buffer."""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         # Poll the socket to see if it is ready for reading.
         # If ready, at least one byte will be to read.
         lr, lw, lx = select.select([self._socket], [], [], 0)
         return len(lr)
 
     # select based implementation, similar to posix, but only using socket API
     # to be portable, additionally handle socket timeout which is used to
@@ -148,15 +148,15 @@
     def read(self, size=1):
         """\
         Read size bytes from the serial port. If a timeout is set it may
         return less characters as requested. With no timeout it will block
         until the requested number of bytes is read.
         """
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         read = bytearray()
         timeout = Timeout(self._timeout)
         while len(read) < size:
             try:
                 ready, _, _ = select.select([self._socket], [], [], timeout.time_left())
                 # If select was used with a timeout, and the timeout occurs, it
                 # returns with empty lists -> thus abort read operation.
@@ -189,15 +189,15 @@
     def write(self, data):
         """\
         Output the given byte string over the serial port. Can block if the
         connection is blocked. May raise SerialException if the connection is
         closed.
         """
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
 
         d = to_bytes(data)
         tx_len = length = len(d)
         timeout = Timeout(self._write_timeout)
         while tx_len > 0:
             try:
                 n = self._socket.send(d)
@@ -205,18 +205,18 @@
                     # Zero timeout indicates non-blocking - simply return the
                     # number of bytes of data actually written
                     return n
                 elif not timeout.is_infinite:
                     # when timeout is set, use select to wait for being ready
                     # with the time left as timeout
                     if timeout.expired():
-                        raise writeTimeoutError
+                        raise SerialTimeoutException('Write timeout')
                     _, ready, _ = select.select([], [self._socket], [], timeout.time_left())
                     if not ready:
-                        raise writeTimeoutError
+                        raise SerialTimeoutException('Write timeout')
                 else:
                     assert timeout.time_left() is None
                     # wait for write operation
                     _, ready, _ = select.select([], [self._socket], [], None)
                     if not ready:
                         raise SerialException('write failed (select)')
                 d = d[n:]
@@ -232,28 +232,29 @@
             except select.error as e:
                 # this is for Python 2.x
                 # ignore BlockingIOErrors and EINTR. all errors are shown
                 # see also http://www.python.org/dev/peps/pep-3151/#select
                 if e[0] not in (errno.EAGAIN, errno.EALREADY, errno.EWOULDBLOCK, errno.EINPROGRESS, errno.EINTR):
                     raise SerialException('write failed: {}'.format(e))
             if not timeout.is_non_blocking and timeout.expired():
-                raise writeTimeoutError
+                raise SerialTimeoutException('Write timeout')
         return length - len(d)
 
     def reset_input_buffer(self):
         """Clear input buffer, discarding all that is in the buffer."""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
 
         # just use recv to remove input, while there is some
         ready = True
         while ready:
             ready, _, _ = select.select([self._socket], [], [], 0)
             try:
-                self._socket.recv(4096)
+                if ready:
+                    ready = self._socket.recv(4096)
             except OSError as e:
                 # this is for Python 3.x where select.error is a subclass of
                 # OSError ignore BlockingIOErrors and EINTR. other errors are shown
                 # https://www.python.org/dev/peps/pep-0475.
                 if e.errno not in (errno.EAGAIN, errno.EALREADY, errno.EWOULDBLOCK, errno.EINPROGRESS, errno.EINTR):
                     raise SerialException('read failed: {}'.format(e))
             except (select.error, socket.error) as e:
@@ -265,25 +266,25 @@
 
     def reset_output_buffer(self):
         """\
         Clear output buffer, aborting the current output and
         discarding all that is in the buffer.
         """
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         if self.logger:
             self.logger.info('ignored reset_output_buffer')
 
     def send_break(self, duration=0.25):
         """\
         Send break condition. Timed, returns to idle state after given
         duration.
         """
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         if self.logger:
             self.logger.info('ignored send_break({!r})'.format(duration))
 
     def _update_break_state(self):
         """Set break: Controls TXD. When active, to transmitting is
         possible."""
         if self.logger:
@@ -299,42 +300,42 @@
         if self.logger:
             self.logger.info('ignored _update_dtr_state({!r})'.format(self._dtr_state))
 
     @property
     def cts(self):
         """Read terminal status line: Clear To Send"""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         if self.logger:
             self.logger.info('returning dummy for cts')
         return True
 
     @property
     def dsr(self):
         """Read terminal status line: Data Set Ready"""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         if self.logger:
             self.logger.info('returning dummy for dsr')
         return True
 
     @property
     def ri(self):
         """Read terminal status line: Ring Indicator"""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         if self.logger:
             self.logger.info('returning dummy for ri')
         return False
 
     @property
     def cd(self):
         """Read terminal status line: Carrier Detect"""
         if not self.is_open:
-            raise portNotOpenError
+            raise PortNotOpenError()
         if self.logger:
             self.logger.info('returning dummy for cd)')
         return True
 
     # - - - platform specific - - -
 
     # works on Linux and probably all the other POSIX systems
```

### Comparing `pyserial-labgrid-3.4.0.1/serial/urlhandler/protocol_spy.py` & `pyserial-labgrid-3.5.0.2/serial/urlhandler/protocol_spy.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 from __future__ import absolute_import
 
 import sys
 import time
 
 import serial
+from serial.serialutil import  to_bytes
 
 try:
     import urlparse
 except ImportError:
     import urllib.parse as urlparse
 
 
@@ -196,14 +197,15 @@
             raise serial.SerialException(
                 'expected a string in the form '
                 '"spy://port[?option[=value][&option[=value]]]": {}'.format(e))
         self.formatter = formatter(output, color)
         return ''.join([parts.netloc, parts.path])
 
     def write(self, tx):
+        tx = to_bytes(tx)
         self.formatter.tx(tx)
         return super(Serial, self).write(tx)
 
     def read(self, size=1):
         rx = super(Serial, self).read(size)
         if rx or self.show_all:
             self.formatter.rx(rx)
```

### Comparing `pyserial-labgrid-3.4.0.1/serial/win32.py` & `pyserial-labgrid-3.5.0.2/serial/win32.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,14 +177,18 @@
 SetCommTimeouts.restype = BOOL
 SetCommTimeouts.argtypes = [HANDLE, LPCOMMTIMEOUTS]
 
 WaitForSingleObject = _stdcall_libraries['kernel32'].WaitForSingleObject
 WaitForSingleObject.restype = DWORD
 WaitForSingleObject.argtypes = [HANDLE, DWORD]
 
+WaitCommEvent = _stdcall_libraries['kernel32'].WaitCommEvent
+WaitCommEvent.restype = BOOL
+WaitCommEvent.argtypes = [HANDLE, LPDWORD, LPOVERLAPPED]
+
 CancelIoEx = _stdcall_libraries['kernel32'].CancelIoEx
 CancelIoEx.restype = BOOL
 CancelIoEx.argtypes = [HANDLE, LPOVERLAPPED]
 
 ONESTOPBIT = 0  # Variable c_int
 TWOSTOPBITS = 2  # Variable c_int
 ONE5STOPBITS = 1
@@ -243,14 +247,20 @@
 GENERIC_READ = 2147483648  # Variable c_ulong
 EV_EVENT2 = 4096  # Variable c_int
 EV_CTS = 8  # Variable c_int
 EV_BREAK = 64  # Variable c_int
 PURGE_RXCLEAR = 8  # Variable c_int
 INFINITE = 0xFFFFFFFF
 
+CE_RXOVER = 0x0001
+CE_OVERRUN = 0x0002
+CE_RXPARITY = 0x0004
+CE_FRAME = 0x0008
+CE_BREAK = 0x0010
+
 
 class N11_OVERLAPPED4DOLLAR_48E(Union):
     pass
 
 
 class N11_OVERLAPPED4DOLLAR_484DOLLAR_49E(Structure):
     pass
```

### Comparing `pyserial-labgrid-3.4.0.1/test/handlers/protocol_test.py` & `pyserial-labgrid-3.5.0.2/test/handlers/protocol_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,99 +76,99 @@
             raise SerialException('expected a string in the form "[test://][option[/option...]]": {}'.format(e))
         return (host, port)
 
     #  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -
 
     def inWaiting(self):
         """Return the number of characters currently in the input buffer."""
-        if not self._isOpen: raise portNotOpenError
+        if not self._isOpen: raise PortNotOpenError()
         if self.logger:
             # set this one to debug as the function could be called often...
             self.logger.debug('WARNING: inWaiting returns dummy value')
         return 0 # hmmm, see comment in read()
 
     def read(self, size=1):
         """Read size bytes from the serial port. If a timeout is set it may
         return less characters as requested. With no timeout it will block
         until the requested number of bytes is read."""
-        if not self._isOpen: raise portNotOpenError
+        if not self._isOpen: raise PortNotOpenError()
         data = '123' # dummy data
         return bytes(data)
 
     def write(self, data):
         """Output the given string over the serial port. Can block if the
         connection is blocked. May raise SerialException if the connection is
         closed."""
-        if not self._isOpen: raise portNotOpenError
+        if not self._isOpen: raise PortNotOpenError()
         # nothing done
         return len(data)
 
     def flushInput(self):
         """Clear input buffer, discarding all that is in the buffer."""
-        if not self._isOpen: raise portNotOpenError
+        if not self._isOpen: raise PortNotOpenError()
         if self.logger:
             self.logger.info('ignored flushInput')
 
     def flushOutput(self):
         """Clear output buffer, aborting the current output and
         discarding all that is in the buffer."""
-        if not self._isOpen: raise portNotOpenError
+        if not self._isOpen: raise PortNotOpenError()
         if self.logger:
             self.logger.info('ignored flushOutput')
 
     def sendBreak(self, duration=0.25):
         """Send break condition. Timed, returns to idle state after given
         duration."""
-        if not self._isOpen: raise portNotOpenError
+        if not self._isOpen: raise PortNotOpenError()
         if self.logger:
             self.logger.info('ignored sendBreak({!r})'.format(duration))
 
     def setBreak(self, level=True):
         """Set break: Controls TXD. When active, to transmitting is
         possible."""
-        if not self._isOpen: raise portNotOpenError
+        if not self._isOpen: raise PortNotOpenError()
         if self.logger:
             self.logger.info('ignored setBreak({!r})'.format(level))
 
     def setRTS(self, level=True):
         """Set terminal status line: Request To Send"""
-        if not self._isOpen: raise portNotOpenError
+        if not self._isOpen: raise PortNotOpenError()
         if self.logger:
             self.logger.info('ignored setRTS({!r})'.format(level))
 
     def setDTR(self, level=True):
         """Set terminal status line: Data Terminal Ready"""
-        if not self._isOpen: raise portNotOpenError
+        if not self._isOpen: raise PortNotOpenError()
         if self.logger:
             self.logger.info('ignored setDTR({!r})'.format(level))
 
     def getCTS(self):
         """Read terminal status line: Clear To Send"""
-        if not self._isOpen: raise portNotOpenError
+        if not self._isOpen: raise PortNotOpenError()
         if self.logger:
             self.logger.info('returning dummy for getCTS()')
         return True
 
     def getDSR(self):
         """Read terminal status line: Data Set Ready"""
-        if not self._isOpen: raise portNotOpenError
+        if not self._isOpen: raise PortNotOpenError()
         if self.logger:
             self.logger.info('returning dummy for getDSR()')
         return True
 
     def getRI(self):
         """Read terminal status line: Ring Indicator"""
-        if not self._isOpen: raise portNotOpenError
+        if not self._isOpen: raise PortNotOpenError()
         if self.logger:
             self.logger.info('returning dummy for getRI()')
         return False
 
     def getCD(self):
         """Read terminal status line: Carrier Detect"""
-        if not self._isOpen: raise portNotOpenError
+        if not self._isOpen: raise PortNotOpenError()
         if self.logger:
             self.logger.info('returning dummy for getCD()')
         return True
 
     # - - - platform specific - - -
     # None so far
```

### Comparing `pyserial-labgrid-3.4.0.1/test/run_all_tests.py` & `pyserial-labgrid-3.5.0.2/test/run_all_tests.py`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/test/test.py` & `pyserial-labgrid-3.5.0.2/test/test.py`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/test/test_advanced.py` & `pyserial-labgrid-3.5.0.2/test/test_advanced.py`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/test/test_asyncio.py` & `pyserial-labgrid-3.5.0.2/test/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/test/test_cancel.py` & `pyserial-labgrid-3.5.0.2/test/test_cancel.py`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/test/test_context.py` & `pyserial-labgrid-3.5.0.2/test/test_context.py`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/test/test_exclusive.py` & `pyserial-labgrid-3.5.0.2/test/test_exclusive.py`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/test/test_high_load.py` & `pyserial-labgrid-3.5.0.2/test/test_high_load.py`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/test/test_iolib.py` & `pyserial-labgrid-3.5.0.2/test/test_iolib.py`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/test/test_pty.py` & `pyserial-labgrid-3.5.0.2/test/test_pty.py`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/test/test_readline.py` & `pyserial-labgrid-3.5.0.2/test/test_readline.py`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/test/test_rfc2217.py` & `pyserial-labgrid-3.5.0.2/test/test_rfc2217.py`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/test/test_rs485.py` & `pyserial-labgrid-3.5.0.2/test/test_rs485.py`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/test/test_settings_dict.py` & `pyserial-labgrid-3.5.0.2/test/test_settings_dict.py`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/test/test_threaded.py` & `pyserial-labgrid-3.5.0.2/test/test_threaded.py`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/test/test_timeout_class.py` & `pyserial-labgrid-3.5.0.2/test/test_timeout_class.py`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/test/test_url.py` & `pyserial-labgrid-3.5.0.2/test/test_url.py`

 * *Files identical despite different names*

### Comparing `pyserial-labgrid-3.4.0.1/test/test_util.py` & `pyserial-labgrid-3.5.0.2/test/test_util.py`

 * *Files identical despite different names*

