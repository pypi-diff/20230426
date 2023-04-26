# Comparing `tmp/python-can-4.2.0.tar.gz` & `tmp/python-can-4.2.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-can-4.2.0.tar", last modified: Tue Apr 25 22:08:03 2023, max compression
+gzip compressed data, was "python-can-4.2.0rc0.tar", last modified: Sun Apr  9 18:21:46 2023, max compression
```

## Comparing `python-can-4.2.0.tar` & `python-can-4.2.0rc0.tar`

### file list

```diff
@@ -1,241 +1,241 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:08:03.306595 python-can-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-25 22:07:55.000000 python-can-4.2.0/CONTRIBUTORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-25 22:07:55.000000 python-can-4.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-25 22:07:55.000000 python-can-4.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-04-25 22:08:03.306595 python-can-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-04-25 22:07:55.000000 python-can-4.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:08:03.282594 python-can-4.2.0/can/
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-25 22:07:55.000000 python-can-4.2.0/can/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38043 2023-04-25 22:07:55.000000 python-can-4.2.0/can/bit_timing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11176 2023-04-25 22:07:55.000000 python-can-4.2.0/can/broadcastmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)    17109 2023-04-25 22:07:55.000000 python-can-4.2.0/can/bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-04-25 22:07:55.000000 python-can-4.2.0/can/ctypesutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-04-25 22:07:55.000000 python-can-4.2.0/can/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:08:03.286594 python-can-4.2.0/can/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/canalystii.py
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/cantact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:08:03.286594 python-can-4.2.0/can/interfaces/etas/
--rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/etas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20644 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/etas/boa.py
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/gs_usb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:08:03.286594 python-can-4.2.0/can/interfaces/ics_neovi/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/ics_neovi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17330 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/ics_neovi/neovi_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/iscan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:08:03.286594 python-can-4.2.0/can/interfaces/ixxat/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/ixxat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/ixxat/canlib.py
--rw-r--r--   0 runner    (1001) docker     (123)    34976 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/ixxat/canlib_vcinpl.py
--rw-r--r--   0 runner    (1001) docker     (123)    38458 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/ixxat/canlib_vcinpl2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/ixxat/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/ixxat/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/ixxat/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:08:03.286594 python-can-4.2.0/can/interfaces/kvaser/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/kvaser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24303 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/kvaser/canlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/kvaser/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/kvaser/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:08:03.286594 python-can-4.2.0/can/interfaces/neousys/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/neousys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/neousys/neousys.py
--rw-r--r--   0 runner    (1001) docker     (123)    11509 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/nican.py
--rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/nixnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:08:03.286594 python-can-4.2.0/can/interfaces/pcan/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/pcan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41828 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/pcan/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    26817 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/pcan/pcan.py
--rw-r--r--   0 runner    (1001) docker     (123)    15685 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/robotell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:08:03.286594 python-can-4.2.0/can/interfaces/seeedstudio/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/seeedstudio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/seeedstudio/seeedstudio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:08:03.286594 python-can-4.2.0/can/interfaces/serial/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/serial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/serial/serial_can.py
--rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/slcan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:08:03.290595 python-can-4.2.0/can/interfaces/socketcan/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/socketcan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/socketcan/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    32057 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/socketcan/socketcan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/socketcan/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:08:03.290595 python-can-4.2.0/can/interfaces/socketcand/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/socketcand/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/socketcand/socketcand.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:08:03.290595 python-can-4.2.0/can/interfaces/systec/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/systec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22700 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/systec/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/systec/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/systec/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)    46740 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/systec/ucan.py
--rw-r--r--   0 runner    (1001) docker     (123)    11213 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/systec/ucanbus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:08:03.290595 python-can-4.2.0/can/interfaces/udp_multicast/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/udp_multicast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16610 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/udp_multicast/bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/udp_multicast/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:08:03.290595 python-can-4.2.0/can/interfaces/usb2can/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/usb2can/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/usb2can/serial_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/usb2can/usb2canInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/usb2can/usb2canabstractionlayer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:08:03.290595 python-can-4.2.0/can/interfaces/vector/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43917 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/vector/canlib.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/vector/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/vector/xlclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/vector/xldefine.py
--rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/vector/xldriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-04-25 22:07:55.000000 python-can-4.2.0/can/interfaces/virtual.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:08:03.290595 python-can-4.2.0/can/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-25 22:07:55.000000 python-can-4.2.0/can/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17337 2023-04-25 22:07:55.000000 python-can-4.2.0/can/io/asc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21908 2023-04-25 22:07:55.000000 python-can-4.2.0/can/io/blf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-04-25 22:07:55.000000 python-can-4.2.0/can/io/canutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-04-25 22:07:55.000000 python-can-4.2.0/can/io/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-04-25 22:07:55.000000 python-can-4.2.0/can/io/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-04-25 22:07:55.000000 python-can-4.2.0/can/io/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    18222 2023-04-25 22:07:55.000000 python-can-4.2.0/can/io/mf4.py
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-04-25 22:07:55.000000 python-can-4.2.0/can/io/player.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-25 22:07:55.000000 python-can-4.2.0/can/io/printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-04-25 22:07:55.000000 python-can-4.2.0/can/io/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-04-25 22:07:55.000000 python-can-4.2.0/can/io/trc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-04-25 22:07:55.000000 python-can-4.2.0/can/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-25 22:07:55.000000 python-can-4.2.0/can/logconvert.py
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-04-25 22:07:55.000000 python-can-4.2.0/can/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    12004 2023-04-25 22:07:55.000000 python-can-4.2.0/can/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-04-25 22:07:55.000000 python-can-4.2.0/can/notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-25 22:07:55.000000 python-can-4.2.0/can/player.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 22:07:55.000000 python-can-4.2.0/can/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-25 22:07:55.000000 python-can-4.2.0/can/thread_safe_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-25 22:07:55.000000 python-can-4.2.0/can/typechecking.py
--rw-r--r--   0 runner    (1001) docker     (123)    15998 2023-04-25 22:07:55.000000 python-can-4.2.0/can/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    22278 2023-04-25 22:07:55.000000 python-can-4.2.0/can/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:08:03.294595 python-can-4.2.0/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/asyncio.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/bcm.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/bit_timing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/bus.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/errors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:08:03.294595 python-can-4.2.0/doc/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/interfaces/canalystii.rst
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/interfaces/cantact.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/interfaces/etas.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     2566 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/interfaces/gs_usb.rst
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/interfaces/iscan.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/interfaces/ixxat.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/interfaces/kvaser.rst
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/interfaces/neousys.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/interfaces/neovi.rst
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/interfaces/nican.rst
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/interfaces/nixnet.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/interfaces/pcan.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/interfaces/robotell.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/interfaces/seeedstudio.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/interfaces/serial.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1055 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/interfaces/slcan.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/interfaces/socketcan.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/interfaces/socketcand.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/interfaces/systec.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/interfaces/udp_multicast.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/interfaces/usb2can.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/interfaces/vector.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/interfaces/virtual.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/interfaces.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/internal-api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/listeners.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/message.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/other-tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/plugin-interface.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/scripts.rst
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8462 2023-04-25 22:07:55.000000 python-can-4.2.0/doc/virtual-interfaces.rst
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-25 22:07:55.000000 python-can-4.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:08:03.298595 python-can-4.2.0/python_can.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-04-25 22:08:03.000000 python-can-4.2.0/python_can.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-04-25 22:08:03.000000 python-can-4.2.0/python_can.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 22:08:03.000000 python-can-4.2.0/python_can.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-25 22:08:03.000000 python-can-4.2.0/python_can.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-25 22:08:03.000000 python-can-4.2.0/python_can.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-25 22:07:55.000000 python-can-4.2.0/requirements-lint.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:08:03.298595 python-can-4.2.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-25 22:07:55.000000 python-can-4.2.0/scripts/can_logconvert.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-25 22:07:55.000000 python-can-4.2.0/scripts/can_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-25 22:07:55.000000 python-can-4.2.0/scripts/can_player.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-25 22:07:55.000000 python-can-4.2.0/scripts/can_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-25 22:08:03.306595 python-can-4.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-04-25 22:07:55.000000 python-can-4.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:08:03.302595 python-can-4.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-25 22:07:55.000000 python-can-4.2.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15773 2023-04-25 22:07:55.000000 python-can-4.2.0/test/back2back_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-25 22:07:55.000000 python-can-4.2.0/test/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-25 22:07:55.000000 python-can-4.2.0/test/contextmanager_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:08:03.302595 python-can-4.2.0/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-25 22:07:55.000000 python-can-4.2.0/test/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-04-25 22:07:55.000000 python-can-4.2.0/test/data/example_data.py
--rw-r--r--   0 runner    (1001) docker     (123)   128078 2023-04-25 22:07:55.000000 python-can-4.2.0/test/data/issue_1256.asc
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-25 22:07:55.000000 python-can-4.2.0/test/data/issue_1299.asc
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-04-25 22:07:55.000000 python-can-4.2.0/test/data/logfile.asc
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-25 22:07:55.000000 python-can-4.2.0/test/data/logfile_errorframes.asc
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-25 22:07:55.000000 python-can-4.2.0/test/data/test_CanErrorFrameExt.blf
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-25 22:07:55.000000 python-can-4.2.0/test/data/test_CanErrorFrames.asc
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-25 22:07:55.000000 python-can-4.2.0/test/data/test_CanFdMessage.asc
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-25 22:07:55.000000 python-can-4.2.0/test/data/test_CanFdMessage.blf
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-25 22:07:55.000000 python-can-4.2.0/test/data/test_CanFdMessage64.asc
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-25 22:07:55.000000 python-can-4.2.0/test/data/test_CanFdMessage64.blf
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-25 22:07:55.000000 python-can-4.2.0/test/data/test_CanFdRemoteMessage.asc
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-25 22:07:55.000000 python-can-4.2.0/test/data/test_CanMessage.asc
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-25 22:07:55.000000 python-can-4.2.0/test/data/test_CanMessage.asc.gz
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-25 22:07:55.000000 python-can-4.2.0/test/data/test_CanMessage.blf
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-25 22:07:55.000000 python-can-4.2.0/test/data/test_CanMessage.trc
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-25 22:07:55.000000 python-can-4.2.0/test/data/test_CanMessage2.blf
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-25 22:07:55.000000 python-can-4.2.0/test/data/test_CanMessage_V1_0_BUS1.trc
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-25 22:07:55.000000 python-can-4.2.0/test/data/test_CanMessage_V1_1.trc
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-25 22:07:55.000000 python-can-4.2.0/test/data/test_CanMessage_V2_0_BUS1.trc
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-25 22:07:55.000000 python-can-4.2.0/test/data/test_CanMessage_V2_1.trc
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-25 22:07:55.000000 python-can-4.2.0/test/data/test_CanRemoteMessage.asc
--rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-04-25 22:07:55.000000 python-can-4.2.0/test/listener_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    33605 2023-04-25 22:07:55.000000 python-can-4.2.0/test/logformats_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-25 22:07:55.000000 python-can-4.2.0/test/message_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-04-25 22:07:55.000000 python-can-4.2.0/test/network_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-25 22:07:55.000000 python-can-4.2.0/test/notifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-04-25 22:07:55.000000 python-can-4.2.0/test/serial_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-04-25 22:07:55.000000 python-can-4.2.0/test/simplecyclic_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13580 2023-04-25 22:07:55.000000 python-can-4.2.0/test/test_bit_timing.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-25 22:07:55.000000 python-can-4.2.0/test/test_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-25 22:07:55.000000 python-can-4.2.0/test/test_cantact.py
--rw-r--r--   0 runner    (1001) docker     (123)    22230 2023-04-25 22:07:55.000000 python-can-4.2.0/test/test_cyclic_socketcan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-25 22:07:55.000000 python-can-4.2.0/test/test_detect_available_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-25 22:07:55.000000 python-can-4.2.0/test/test_interface.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3367 2023-04-25 22:07:55.000000 python-can-4.2.0/test/test_interface_canalystii.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-25 22:07:55.000000 python-can-4.2.0/test/test_interface_ixxat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-25 22:07:55.000000 python-can-4.2.0/test/test_interface_ixxat_fd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-25 22:07:55.000000 python-can-4.2.0/test/test_interface_virtual.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-04-25 22:07:55.000000 python-can-4.2.0/test/test_kvaser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-25 22:07:55.000000 python-can-4.2.0/test/test_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-04-25 22:07:55.000000 python-can-4.2.0/test/test_load_file_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-04-25 22:07:55.000000 python-can-4.2.0/test/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-04-25 22:07:55.000000 python-can-4.2.0/test/test_message_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-25 22:07:55.000000 python-can-4.2.0/test/test_message_filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-04-25 22:07:55.000000 python-can-4.2.0/test/test_message_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-04-25 22:07:55.000000 python-can-4.2.0/test/test_neousys.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-25 22:07:55.000000 python-can-4.2.0/test/test_neovi.py
--rw-r--r--   0 runner    (1001) docker     (123)    19093 2023-04-25 22:07:55.000000 python-can-4.2.0/test/test_pcan.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3930 2023-04-25 22:07:55.000000 python-can-4.2.0/test/test_player.py
--rw-r--r--   0 runner    (1001) docker     (123)    24830 2023-04-25 22:07:55.000000 python-can-4.2.0/test/test_robotell.py
--rw-r--r--   0 runner    (1001) docker     (123)     9343 2023-04-25 22:07:55.000000 python-can-4.2.0/test/test_rotating_loggers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-04-25 22:07:55.000000 python-can-4.2.0/test/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-04-25 22:07:55.000000 python-can-4.2.0/test/test_slcan.py
--rw-r--r--   0 runner    (1001) docker     (123)    13308 2023-04-25 22:07:55.000000 python-can-4.2.0/test/test_socketcan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-25 22:07:55.000000 python-can-4.2.0/test/test_socketcan_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-25 22:07:55.000000 python-can-4.2.0/test/test_socketcan_loopback.py
--rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-04-25 22:07:55.000000 python-can-4.2.0/test/test_systec.py
--rw-r--r--   0 runner    (1001) docker     (123)    11232 2023-04-25 22:07:55.000000 python-can-4.2.0/test/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    47118 2023-04-25 22:07:55.000000 python-can-4.2.0/test/test_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)    20951 2023-04-25 22:07:55.000000 python-can-4.2.0/test/test_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-25 22:07:55.000000 python-can-4.2.0/test/zero_dlc_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.875723 python-can-4.2.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/CONTRIBUTORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-04-09 18:21:46.875723 python-can-4.2.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.851723 python-can-4.2.0rc0/can/
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38043 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/bit_timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11176 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/broadcastmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17100 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/ctypesutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.851723 python-can-4.2.0rc0/can/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/canalystii.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/cantact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.855723 python-can-4.2.0rc0/can/interfaces/etas/
+-rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/etas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20644 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/etas/boa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/gs_usb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.855723 python-can-4.2.0rc0/can/interfaces/ics_neovi/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/ics_neovi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17330 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/ics_neovi/neovi_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/iscan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.855723 python-can-4.2.0rc0/can/interfaces/ixxat/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/ixxat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/ixxat/canlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34976 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/ixxat/canlib_vcinpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38458 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/ixxat/canlib_vcinpl2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/ixxat/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/ixxat/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/ixxat/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.855723 python-can-4.2.0rc0/can/interfaces/kvaser/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/kvaser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24303 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/kvaser/canlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/kvaser/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/kvaser/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.855723 python-can-4.2.0rc0/can/interfaces/neousys/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/neousys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/neousys/neousys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11509 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/nican.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/nixnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.855723 python-can-4.2.0rc0/can/interfaces/pcan/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/pcan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41828 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/pcan/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26817 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/pcan/pcan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15685 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/robotell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.855723 python-can-4.2.0rc0/can/interfaces/seeedstudio/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/seeedstudio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/seeedstudio/seeedstudio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.855723 python-can-4.2.0rc0/can/interfaces/serial/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/serial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/serial/serial_can.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/slcan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.855723 python-can-4.2.0rc0/can/interfaces/socketcan/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/socketcan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/socketcan/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32057 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/socketcan/socketcan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/socketcan/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.855723 python-can-4.2.0rc0/can/interfaces/socketcand/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/socketcand/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/socketcand/socketcand.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.859723 python-can-4.2.0rc0/can/interfaces/systec/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/systec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22700 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/systec/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/systec/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/systec/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46740 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/systec/ucan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11213 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/systec/ucanbus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.859723 python-can-4.2.0rc0/can/interfaces/udp_multicast/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/udp_multicast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16610 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/udp_multicast/bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/udp_multicast/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.859723 python-can-4.2.0rc0/can/interfaces/usb2can/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/usb2can/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/usb2can/serial_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/usb2can/usb2canInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/usb2can/usb2canabstractionlayer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.859723 python-can-4.2.0rc0/can/interfaces/vector/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43839 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/vector/canlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/vector/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/vector/xlclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/vector/xldefine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/vector/xldriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/virtual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.859723 python-can-4.2.0rc0/can/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17337 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/io/asc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21908 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/io/blf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/io/canutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/io/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/io/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/io/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18222 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/io/mf4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/io/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/io/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/io/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15104 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/io/trc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/logconvert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12004 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/thread_safe_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/typechecking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15998 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22278 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.863723 python-can-4.2.0rc0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/asyncio.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/bcm.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/bit_timing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/bus.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.867724 python-can-4.2.0rc0/doc/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/canalystii.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/cantact.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/etas.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2566 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/gs_usb.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/iscan.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/ixxat.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/kvaser.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/neousys.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/neovi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/nican.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/nixnet.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/pcan.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/robotell.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/seeedstudio.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/serial.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1055 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/slcan.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/socketcan.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/socketcand.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/systec.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/udp_multicast.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/usb2can.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/vector.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/virtual.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/internal-api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/listeners.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/message.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/other-tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/plugin-interface.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/scripts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8462 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/virtual-interfaces.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.867724 python-can-4.2.0rc0/python_can.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-04-09 18:21:46.000000 python-can-4.2.0rc0/python_can.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-04-09 18:21:46.000000 python-can-4.2.0rc0/python_can.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 18:21:46.000000 python-can-4.2.0rc0/python_can.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-09 18:21:46.000000 python-can-4.2.0rc0/python_can.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-09 18:21:46.000000 python-can-4.2.0rc0/python_can.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/requirements-lint.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.867724 python-can-4.2.0rc0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/scripts/can_logconvert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/scripts/can_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/scripts/can_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/scripts/can_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-09 18:21:46.875723 python-can-4.2.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.871724 python-can-4.2.0rc0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15773 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/back2back_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/contextmanager_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.875723 python-can-4.2.0rc0/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/example_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)   128078 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/issue_1256.asc
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/issue_1299.asc
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/logfile.asc
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/logfile_errorframes.asc
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/test_CanErrorFrameExt.blf
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/test_CanErrorFrames.asc
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/test_CanFdMessage.asc
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/test_CanFdMessage.blf
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/test_CanFdMessage64.asc
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/test_CanFdMessage64.blf
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/test_CanFdRemoteMessage.asc
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/test_CanMessage.asc
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/test_CanMessage.asc.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/test_CanMessage.blf
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/test_CanMessage.trc
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/test_CanMessage2.blf
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/test_CanMessage_V1_0_BUS1.trc
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/test_CanMessage_V1_1.trc
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/test_CanMessage_V2_0_BUS1.trc
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/test_CanMessage_V2_1.trc
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/test_CanRemoteMessage.asc
+-rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/listener_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33541 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/logformats_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/message_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/network_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/notifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/serial_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/simplecyclic_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13580 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_bit_timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_cantact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22230 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_cyclic_socketcan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_detect_available_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_interface.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3367 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_interface_canalystii.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_interface_ixxat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_interface_ixxat_fd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_interface_virtual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_kvaser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_load_file_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_message_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_message_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_message_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_neousys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_neovi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19093 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_pcan.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3930 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24830 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_robotell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9343 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_rotating_loggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_slcan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13308 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_socketcan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_socketcan_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_socketcan_loopback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_systec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11232 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47118 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20951 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/zero_dlc_test.py
```

### Comparing `python-can-4.2.0/CONTRIBUTORS.txt` & `python-can-4.2.0rc0/CONTRIBUTORS.txt`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/LICENSE.txt` & `python-can-4.2.0rc0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/PKG-INFO` & `python-can-4.2.0rc0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-can
-Version: 4.2.0
+Version: 4.2.0rc0
 Summary: Controller Area Network interface module for Python
 Home-page: https://github.com/hardbyte/python-can
 Author: python-can contributors
 License: LGPL v3
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -50,15 +50,15 @@
 License-File: LICENSE.txt
 
 python-can
 ==========
 
 |pypi| |conda| |python_implementation| |downloads| |downloads_monthly|
 
-|docs| |github-actions| |coverage| |mergify| |formatter|
+|docs| |github-actions| |build_travis| |coverage| |mergify| |formatter|
 
 .. |pypi| image:: https://img.shields.io/pypi/v/python-can.svg
    :target: https://pypi.python.org/pypi/python-can/
    :alt: Latest Version on PyPi
 
 .. |conda| image:: https://img.shields.io/conda/v/conda-forge/python-can
    :target: https://github.com/conda-forge/python-can-feedstock
@@ -84,14 +84,18 @@
    :target: https://python-can.readthedocs.io/en/stable/
    :alt: Documentation
 
 .. |github-actions| image:: https://github.com/hardbyte/python-can/actions/workflows/ci.yml/badge.svg
    :target: https://github.com/hardbyte/python-can/actions/workflows/ci.yml
    :alt: Github Actions workflow status
 
+.. |build_travis| image:: https://img.shields.io/travis/hardbyte/python-can/develop.svg?label=Travis%20CI
+   :target: https://app.travis-ci.com/github/hardbyte/python-can
+   :alt: Travis CI Server for develop branch
+
 .. |coverage| image:: https://coveralls.io/repos/github/hardbyte/python-can/badge.svg?branch=develop
    :target: https://coveralls.io/github/hardbyte/python-can?branch=develop
    :alt: Test coverage reports on Coveralls.io
 
 .. |mergify| image:: https://img.shields.io/endpoint.svg?url=https://api.mergify.com/v1/badges/hardbyte/python-can&style=flat
    :target: https://mergify.io
    :alt: Mergify Status
```

### Comparing `python-can-4.2.0/README.rst` & `python-can-4.2.0rc0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 python-can
 ==========
 
 |pypi| |conda| |python_implementation| |downloads| |downloads_monthly|
 
-|docs| |github-actions| |coverage| |mergify| |formatter|
+|docs| |github-actions| |build_travis| |coverage| |mergify| |formatter|
 
 .. |pypi| image:: https://img.shields.io/pypi/v/python-can.svg
    :target: https://pypi.python.org/pypi/python-can/
    :alt: Latest Version on PyPi
 
 .. |conda| image:: https://img.shields.io/conda/v/conda-forge/python-can
    :target: https://github.com/conda-forge/python-can-feedstock
@@ -33,14 +33,18 @@
    :target: https://python-can.readthedocs.io/en/stable/
    :alt: Documentation
 
 .. |github-actions| image:: https://github.com/hardbyte/python-can/actions/workflows/ci.yml/badge.svg
    :target: https://github.com/hardbyte/python-can/actions/workflows/ci.yml
    :alt: Github Actions workflow status
 
+.. |build_travis| image:: https://img.shields.io/travis/hardbyte/python-can/develop.svg?label=Travis%20CI
+   :target: https://app.travis-ci.com/github/hardbyte/python-can
+   :alt: Travis CI Server for develop branch
+
 .. |coverage| image:: https://coveralls.io/repos/github/hardbyte/python-can/badge.svg?branch=develop
    :target: https://coveralls.io/github/hardbyte/python-can?branch=develop
    :alt: Test coverage reports on Coveralls.io
 
 .. |mergify| image:: https://img.shields.io/endpoint.svg?url=https://api.mergify.com/v1/badges/hardbyte/python-can&style=flat
    :target: https://mergify.io
    :alt: Mergify Status
```

### Comparing `python-can-4.2.0/can/__init__.py` & `python-can-4.2.0rc0/can/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 different hardware devices, and a suite of utilities for sending and receiving
 messages on a can bus.
 """
 
 import logging
 from typing import Any, Dict
 
-__version__ = "4.2.0"
+__version__ = "4.2.0rc0"
 __all__ = [
     "ASCReader",
     "ASCWriter",
     "AsyncBufferedReader",
     "BitTiming",
     "BitTimingFd",
     "BLFReader",
```

### Comparing `python-can-4.2.0/can/bit_timing.py` & `python-can-4.2.0rc0/can/bit_timing.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/broadcastmanager.py` & `python-can-4.2.0rc0/can/broadcastmanager.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/bus.py` & `python-can-4.2.0rc0/can/bus.py`

 * *Files 0% similar despite different names*

```diff
@@ -435,15 +435,15 @@
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.shutdown()
 
     def __del__(self) -> None:
         if not self._is_shutdown:
-            LOG.warning("%s was not properly shut down", self.__class__.__name__)
+            LOG.warning("%s was not properly shut down", self.__class__)
             # We do some best-effort cleanup if the user
             # forgot to properly close the bus instance
             with contextlib.suppress(AttributeError):
                 self.shutdown()
 
     @property
     def state(self) -> BusState:
```

### Comparing `python-can-4.2.0/can/ctypesutil.py` & `python-can-4.2.0rc0/can/ctypesutil.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/exceptions.py` & `python-can-4.2.0rc0/can/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interface.py` & `python-can-4.2.0rc0/can/interface.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/__init__.py` & `python-can-4.2.0rc0/can/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/canalystii.py` & `python-can-4.2.0rc0/can/interfaces/canalystii.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/cantact.py` & `python-can-4.2.0rc0/can/interfaces/cantact.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/etas/__init__.py` & `python-can-4.2.0rc0/can/interfaces/etas/__init__.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/etas/boa.py` & `python-can-4.2.0rc0/can/interfaces/etas/boa.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/gs_usb.py` & `python-can-4.2.0rc0/can/interfaces/gs_usb.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/ics_neovi/neovi_bus.py` & `python-can-4.2.0rc0/can/interfaces/ics_neovi/neovi_bus.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/iscan.py` & `python-can-4.2.0rc0/can/interfaces/iscan.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/ixxat/canlib.py` & `python-can-4.2.0rc0/can/interfaces/ixxat/canlib.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/ixxat/canlib_vcinpl.py` & `python-can-4.2.0rc0/can/interfaces/ixxat/canlib_vcinpl.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/ixxat/canlib_vcinpl2.py` & `python-can-4.2.0rc0/can/interfaces/ixxat/canlib_vcinpl2.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/ixxat/constants.py` & `python-can-4.2.0rc0/can/interfaces/ixxat/constants.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/ixxat/exceptions.py` & `python-can-4.2.0rc0/can/interfaces/ixxat/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/ixxat/structures.py` & `python-can-4.2.0rc0/can/interfaces/ixxat/structures.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/kvaser/canlib.py` & `python-can-4.2.0rc0/can/interfaces/kvaser/canlib.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/kvaser/constants.py` & `python-can-4.2.0rc0/can/interfaces/kvaser/constants.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/kvaser/structures.py` & `python-can-4.2.0rc0/can/interfaces/kvaser/structures.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/neousys/neousys.py` & `python-can-4.2.0rc0/can/interfaces/neousys/neousys.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/nican.py` & `python-can-4.2.0rc0/can/interfaces/nican.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/nixnet.py` & `python-can-4.2.0rc0/can/interfaces/nixnet.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/pcan/basic.py` & `python-can-4.2.0rc0/can/interfaces/pcan/basic.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/pcan/pcan.py` & `python-can-4.2.0rc0/can/interfaces/pcan/pcan.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/robotell.py` & `python-can-4.2.0rc0/can/interfaces/robotell.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/seeedstudio/seeedstudio.py` & `python-can-4.2.0rc0/can/interfaces/seeedstudio/seeedstudio.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/serial/serial_can.py` & `python-can-4.2.0rc0/can/interfaces/serial/serial_can.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/slcan.py` & `python-can-4.2.0rc0/can/interfaces/slcan.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/socketcan/constants.py` & `python-can-4.2.0rc0/can/interfaces/socketcan/constants.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/socketcan/socketcan.py` & `python-can-4.2.0rc0/can/interfaces/socketcan/socketcan.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/socketcan/utils.py` & `python-can-4.2.0rc0/can/interfaces/socketcan/utils.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/socketcand/socketcand.py` & `python-can-4.2.0rc0/can/interfaces/socketcand/socketcand.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/systec/constants.py` & `python-can-4.2.0rc0/can/interfaces/systec/constants.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/systec/exceptions.py` & `python-can-4.2.0rc0/can/interfaces/systec/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/systec/structures.py` & `python-can-4.2.0rc0/can/interfaces/systec/structures.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/systec/ucan.py` & `python-can-4.2.0rc0/can/interfaces/systec/ucan.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/systec/ucanbus.py` & `python-can-4.2.0rc0/can/interfaces/systec/ucanbus.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/udp_multicast/bus.py` & `python-can-4.2.0rc0/can/interfaces/udp_multicast/bus.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/udp_multicast/utils.py` & `python-can-4.2.0rc0/can/interfaces/udp_multicast/utils.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/usb2can/serial_selector.py` & `python-can-4.2.0rc0/can/interfaces/usb2can/serial_selector.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/usb2can/usb2canInterface.py` & `python-can-4.2.0rc0/can/interfaces/usb2can/usb2canInterface.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/usb2can/usb2canabstractionlayer.py` & `python-can-4.2.0rc0/can/interfaces/usb2can/usb2canabstractionlayer.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/vector/canlib.py` & `python-can-4.2.0rc0/can/interfaces/vector/canlib.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 Ctypes wrapper module for Vector CAN Interface on win32/win64 systems.
 
 Authors: Julien Grave <grave.jul@gmail.com>, Christian Sandberg
 """
 
 # Import Standard Python Modules
 # ==============================
-import contextlib
 import ctypes
 import logging
 import os
 import time
 from types import ModuleType
 from typing import (
     Any,
@@ -866,19 +865,17 @@
         return xl_can_tx_event
 
     def flush_tx_buffer(self) -> None:
         self.xldriver.xlCanFlushTransmitQueue(self.port_handle, self.mask)
 
     def shutdown(self) -> None:
         super().shutdown()
-
-        with contextlib.suppress(VectorError):
-            self.xldriver.xlDeactivateChannel(self.port_handle, self.mask)
-            self.xldriver.xlClosePort(self.port_handle)
-            self.xldriver.xlCloseDriver()
+        self.xldriver.xlDeactivateChannel(self.port_handle, self.mask)
+        self.xldriver.xlClosePort(self.port_handle)
+        self.xldriver.xlCloseDriver()
 
     def reset(self) -> None:
         self.xldriver.xlDeactivateChannel(self.port_handle, self.mask)
         self.xldriver.xlActivateChannel(
             self.port_handle, self.mask, xldefine.XL_BusTypes.XL_BUS_TYPE_CAN, 0
         )
```

### Comparing `python-can-4.2.0/can/interfaces/vector/exceptions.py` & `python-can-4.2.0rc0/can/interfaces/vector/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/vector/xlclass.py` & `python-can-4.2.0rc0/can/interfaces/vector/xlclass.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/vector/xldefine.py` & `python-can-4.2.0rc0/can/interfaces/vector/xldefine.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/vector/xldriver.py` & `python-can-4.2.0rc0/can/interfaces/vector/xldriver.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/interfaces/virtual.py` & `python-can-4.2.0rc0/can/interfaces/virtual.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/io/__init__.py` & `python-can-4.2.0rc0/can/io/__init__.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/io/asc.py` & `python-can-4.2.0rc0/can/io/asc.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/io/blf.py` & `python-can-4.2.0rc0/can/io/blf.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/io/canutils.py` & `python-can-4.2.0rc0/can/io/canutils.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/io/csv.py` & `python-can-4.2.0rc0/can/io/csv.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/io/generic.py` & `python-can-4.2.0rc0/can/io/generic.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/io/logger.py` & `python-can-4.2.0rc0/can/io/logger.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/io/mf4.py` & `python-can-4.2.0rc0/can/io/mf4.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/io/player.py` & `python-can-4.2.0rc0/can/io/player.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/io/printer.py` & `python-can-4.2.0rc0/can/io/printer.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/io/sqlite.py` & `python-can-4.2.0rc0/can/io/sqlite.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/io/trc.py` & `python-can-4.2.0rc0/can/io/trc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 Reader and writer for can logging files in peak trc format
 
 See https://www.peak-system.com/produktcd/Pdf/English/PEAK_CAN_TRC_File_Format.pdf
 for file format description
 
 Version 1.1 will be implemented as it is most commonly used
-"""
+"""  # noqa
 
+import io
 import logging
 import os
 from datetime import datetime, timedelta, timezone
 from enum import Enum
 from typing import Callable, Dict, Generator, List, Optional, TextIO, Union
 
 from ..message import Message
@@ -269,15 +270,15 @@
                      write mode, not binary write mode.
         :param channel: a default channel to use when the message does not
                         have a channel set
         """
         super().__init__(file, mode="w")
         self.channel = channel
 
-        if hasattr(self.file, "reconfigure"):
+        if isinstance(self.file, io.TextIOWrapper):
             self.file.reconfigure(newline="\r\n")
         else:
             raise TypeError("File must be opened in text mode.")
 
         self.filepath = os.path.abspath(self.file.name)
         self.header_written = False
         self.msgnr = 0
```

### Comparing `python-can-4.2.0/can/listener.py` & `python-can-4.2.0rc0/can/listener.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/logconvert.py` & `python-can-4.2.0rc0/can/logconvert.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/logger.py` & `python-can-4.2.0rc0/can/logger.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/message.py` & `python-can-4.2.0rc0/can/message.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/notifier.py` & `python-can-4.2.0rc0/can/notifier.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/player.py` & `python-can-4.2.0rc0/can/player.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/thread_safe_bus.py` & `python-can-4.2.0rc0/can/thread_safe_bus.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/typechecking.py` & `python-can-4.2.0rc0/can/typechecking.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/util.py` & `python-can-4.2.0rc0/can/util.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/can/viewer.py` & `python-can-4.2.0rc0/can/viewer.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/asyncio.rst` & `python-can-4.2.0rc0/doc/asyncio.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/bcm.rst` & `python-can-4.2.0rc0/doc/bcm.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/bit_timing.rst` & `python-can-4.2.0rc0/doc/bit_timing.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/bus.rst` & `python-can-4.2.0rc0/doc/bus.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/configuration.rst` & `python-can-4.2.0rc0/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/development.rst` & `python-can-4.2.0rc0/doc/development.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/history.rst` & `python-can-4.2.0rc0/doc/history.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/index.rst` & `python-can-4.2.0rc0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/installation.rst` & `python-can-4.2.0rc0/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/interfaces/canalystii.rst` & `python-can-4.2.0rc0/doc/interfaces/canalystii.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/interfaces/etas.rst` & `python-can-4.2.0rc0/doc/interfaces/etas.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/interfaces/gs_usb.rst` & `python-can-4.2.0rc0/doc/interfaces/gs_usb.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/interfaces/ixxat.rst` & `python-can-4.2.0rc0/doc/interfaces/ixxat.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/interfaces/kvaser.rst` & `python-can-4.2.0rc0/doc/interfaces/kvaser.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/interfaces/neousys.rst` & `python-can-4.2.0rc0/doc/interfaces/neousys.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/interfaces/neovi.rst` & `python-can-4.2.0rc0/doc/interfaces/neovi.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/interfaces/nican.rst` & `python-can-4.2.0rc0/doc/interfaces/nican.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/interfaces/pcan.rst` & `python-can-4.2.0rc0/doc/interfaces/pcan.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/interfaces/robotell.rst` & `python-can-4.2.0rc0/doc/interfaces/robotell.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/interfaces/seeedstudio.rst` & `python-can-4.2.0rc0/doc/interfaces/seeedstudio.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/interfaces/serial.rst` & `python-can-4.2.0rc0/doc/interfaces/serial.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/interfaces/slcan.rst` & `python-can-4.2.0rc0/doc/interfaces/slcan.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/interfaces/socketcan.rst` & `python-can-4.2.0rc0/doc/interfaces/socketcan.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/interfaces/socketcand.rst` & `python-can-4.2.0rc0/doc/interfaces/socketcand.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/interfaces/systec.rst` & `python-can-4.2.0rc0/doc/interfaces/systec.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/interfaces/udp_multicast.rst` & `python-can-4.2.0rc0/doc/interfaces/udp_multicast.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/interfaces/usb2can.rst` & `python-can-4.2.0rc0/doc/interfaces/usb2can.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/interfaces/vector.rst` & `python-can-4.2.0rc0/doc/interfaces/vector.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/interfaces/virtual.rst` & `python-can-4.2.0rc0/doc/interfaces/virtual.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/interfaces.rst` & `python-can-4.2.0rc0/doc/interfaces.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/internal-api.rst` & `python-can-4.2.0rc0/doc/internal-api.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/listeners.rst` & `python-can-4.2.0rc0/doc/listeners.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/message.rst` & `python-can-4.2.0rc0/doc/message.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/other-tools.rst` & `python-can-4.2.0rc0/doc/other-tools.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/plugin-interface.rst` & `python-can-4.2.0rc0/doc/plugin-interface.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/scripts.rst` & `python-can-4.2.0rc0/doc/scripts.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/doc/virtual-interfaces.rst` & `python-can-4.2.0rc0/doc/virtual-interfaces.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/python_can.egg-info/PKG-INFO` & `python-can-4.2.0rc0/python_can.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-can
-Version: 4.2.0
+Version: 4.2.0rc0
 Summary: Controller Area Network interface module for Python
 Home-page: https://github.com/hardbyte/python-can
 Author: python-can contributors
 License: LGPL v3
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -50,15 +50,15 @@
 License-File: LICENSE.txt
 
 python-can
 ==========
 
 |pypi| |conda| |python_implementation| |downloads| |downloads_monthly|
 
-|docs| |github-actions| |coverage| |mergify| |formatter|
+|docs| |github-actions| |build_travis| |coverage| |mergify| |formatter|
 
 .. |pypi| image:: https://img.shields.io/pypi/v/python-can.svg
    :target: https://pypi.python.org/pypi/python-can/
    :alt: Latest Version on PyPi
 
 .. |conda| image:: https://img.shields.io/conda/v/conda-forge/python-can
    :target: https://github.com/conda-forge/python-can-feedstock
@@ -84,14 +84,18 @@
    :target: https://python-can.readthedocs.io/en/stable/
    :alt: Documentation
 
 .. |github-actions| image:: https://github.com/hardbyte/python-can/actions/workflows/ci.yml/badge.svg
    :target: https://github.com/hardbyte/python-can/actions/workflows/ci.yml
    :alt: Github Actions workflow status
 
+.. |build_travis| image:: https://img.shields.io/travis/hardbyte/python-can/develop.svg?label=Travis%20CI
+   :target: https://app.travis-ci.com/github/hardbyte/python-can
+   :alt: Travis CI Server for develop branch
+
 .. |coverage| image:: https://coveralls.io/repos/github/hardbyte/python-can/badge.svg?branch=develop
    :target: https://coveralls.io/github/hardbyte/python-can?branch=develop
    :alt: Test coverage reports on Coveralls.io
 
 .. |mergify| image:: https://img.shields.io/endpoint.svg?url=https://api.mergify.com/v1/badges/hardbyte/python-can&style=flat
    :target: https://mergify.io
    :alt: Mergify Status
```

### Comparing `python-can-4.2.0/python_can.egg-info/SOURCES.txt` & `python-can-4.2.0rc0/python_can.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/python_can.egg-info/requires.txt` & `python-can-4.2.0rc0/python_can.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/setup.cfg` & `python-can-4.2.0rc0/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/setup.py` & `python-can-4.2.0rc0/setup.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/back2back_test.py` & `python-can-4.2.0rc0/test/back2back_test.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/config.py` & `python-can-4.2.0rc0/test/config.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/contextmanager_test.py` & `python-can-4.2.0rc0/test/contextmanager_test.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/data/example_data.py` & `python-can-4.2.0rc0/test/data/example_data.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/data/issue_1256.asc` & `python-can-4.2.0rc0/test/data/issue_1256.asc`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/data/issue_1299.asc` & `python-can-4.2.0rc0/test/data/issue_1299.asc`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/data/logfile.asc` & `python-can-4.2.0rc0/test/data/logfile.asc`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/data/logfile_errorframes.asc` & `python-can-4.2.0rc0/test/data/logfile_errorframes.asc`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/data/test_CanErrorFrames.asc` & `python-can-4.2.0rc0/test/data/test_CanErrorFrames.asc`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/data/test_CanFdMessage.asc` & `python-can-4.2.0rc0/test/data/test_CanFdMessage.asc`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/data/test_CanFdMessage.blf` & `python-can-4.2.0rc0/test/data/test_CanFdMessage.blf`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/data/test_CanFdMessage64.asc` & `python-can-4.2.0rc0/test/data/test_CanFdMessage64.asc`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/data/test_CanFdMessage64.blf` & `python-can-4.2.0rc0/test/data/test_CanFdMessage64.blf`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/data/test_CanMessage.trc` & `python-can-4.2.0rc0/test/data/test_CanMessage.trc`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/data/test_CanMessage_V1_0_BUS1.trc` & `python-can-4.2.0rc0/test/data/test_CanMessage_V1_0_BUS1.trc`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/data/test_CanMessage_V1_1.trc` & `python-can-4.2.0rc0/test/data/test_CanMessage_V1_1.trc`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/data/test_CanMessage_V2_0_BUS1.trc` & `python-can-4.2.0rc0/test/data/test_CanMessage_V2_0_BUS1.trc`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/data/test_CanMessage_V2_1.trc` & `python-can-4.2.0rc0/test/data/test_CanMessage_V2_1.trc`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/listener_test.py` & `python-can-4.2.0rc0/test/listener_test.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/logformats_test.py` & `python-can-4.2.0rc0/test/logformats_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -930,19 +930,18 @@
                 msg_ext(20.9560),
                 msg_ext(21.0971),
             ]
             actual = self._read_log_file(filename)
             self.assertMessagesEqual(actual, expected_messages)
 
     def test_not_supported_version(self):
-        with tempfile.NamedTemporaryFile(mode="w") as f:
-            with self.assertRaises(NotImplementedError):
-                writer = can.TRCWriter(f)
-                writer.file_version = can.TRCFileVersion.UNKNOWN
-                writer.on_message_received(can.Message())
+        with self.assertRaises(NotImplementedError):
+            writer = can.TRCWriter("test.trc")
+            writer.file_version = can.TRCFileVersion.UNKNOWN
+            writer.on_message_received(can.Message())
 
 
 class TestTrcFileFormatV1_0(TestTrcFileFormatBase):
     """Tests can.TRCWriter and can.TRCReader with file version 1.0"""
 
     @staticmethod
     def Writer(filename):
```

### Comparing `python-can-4.2.0/test/message_helper.py` & `python-can-4.2.0rc0/test/message_helper.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/network_test.py` & `python-can-4.2.0rc0/test/network_test.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/notifier_test.py` & `python-can-4.2.0rc0/test/notifier_test.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/serial_test.py` & `python-can-4.2.0rc0/test/serial_test.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/simplecyclic_test.py` & `python-can-4.2.0rc0/test/simplecyclic_test.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/test_bit_timing.py` & `python-can-4.2.0rc0/test/test_bit_timing.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/test_bus.py` & `python-can-4.2.0rc0/test/test_bus.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/test_cantact.py` & `python-can-4.2.0rc0/test/test_cantact.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/test_cyclic_socketcan.py` & `python-can-4.2.0rc0/test/test_cyclic_socketcan.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/test_detect_available_configs.py` & `python-can-4.2.0rc0/test/test_detect_available_configs.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/test_interface.py` & `python-can-4.2.0rc0/test/test_interface.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/test_interface_canalystii.py` & `python-can-4.2.0rc0/test/test_interface_canalystii.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/test_interface_ixxat.py` & `python-can-4.2.0rc0/test/test_interface_ixxat.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/test_interface_ixxat_fd.py` & `python-can-4.2.0rc0/test/test_interface_ixxat_fd.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/test_interface_virtual.py` & `python-can-4.2.0rc0/test/test_interface_virtual.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/test_kvaser.py` & `python-can-4.2.0rc0/test/test_kvaser.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/test_load_config.py` & `python-can-4.2.0rc0/test/test_load_config.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/test_load_file_config.py` & `python-can-4.2.0rc0/test/test_load_file_config.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/test_logger.py` & `python-can-4.2.0rc0/test/test_logger.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/test_message_class.py` & `python-can-4.2.0rc0/test/test_message_class.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/test_message_filtering.py` & `python-can-4.2.0rc0/test/test_message_filtering.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/test_message_sync.py` & `python-can-4.2.0rc0/test/test_message_sync.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/test_neousys.py` & `python-can-4.2.0rc0/test/test_neousys.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/test_neovi.py` & `python-can-4.2.0rc0/test/test_neovi.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/test_pcan.py` & `python-can-4.2.0rc0/test/test_pcan.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/test_player.py` & `python-can-4.2.0rc0/test/test_player.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/test_robotell.py` & `python-can-4.2.0rc0/test/test_robotell.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/test_rotating_loggers.py` & `python-can-4.2.0rc0/test/test_rotating_loggers.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/test_scripts.py` & `python-can-4.2.0rc0/test/test_scripts.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/test_slcan.py` & `python-can-4.2.0rc0/test/test_slcan.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/test_socketcan.py` & `python-can-4.2.0rc0/test/test_socketcan.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/test_socketcan_helpers.py` & `python-can-4.2.0rc0/test/test_socketcan_helpers.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/test_socketcan_loopback.py` & `python-can-4.2.0rc0/test/test_socketcan_loopback.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/test_systec.py` & `python-can-4.2.0rc0/test/test_systec.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/test_util.py` & `python-can-4.2.0rc0/test/test_util.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/test_vector.py` & `python-can-4.2.0rc0/test/test_vector.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/test_viewer.py` & `python-can-4.2.0rc0/test/test_viewer.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.0/test/zero_dlc_test.py` & `python-can-4.2.0rc0/test/zero_dlc_test.py`

 * *Files identical despite different names*

