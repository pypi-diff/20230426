# Comparing `tmp/pymodaq_plugins_mock-4.0.1.tar.gz` & `tmp/pymodaq_plugins_mock-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodaq_plugins_mock-4.0.1.tar", last modified: Tue Apr 18 13:34:02 2023, max compression
+gzip compressed data, was "pymodaq_plugins_mock-4.0.2.tar", last modified: Tue Apr 25 16:45:13 2023, max compression
```

## Comparing `pymodaq_plugins_mock-4.0.1.tar` & `pymodaq_plugins_mock-4.0.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:34:02.625826 pymodaq_plugins_mock-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-18 13:34:02.625826 pymodaq_plugins_mock-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 13:34:02.625826 pymodaq_plugins_mock-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:34:02.621826 pymodaq_plugins_mock-4.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:34:02.621826 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:34:02.625826 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_move_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_move_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_Mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockCamera.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockTau.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_TCPServer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:34:02.625826 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:34:02.625826 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_MockAdaptive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TCPServer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:34:02.625826 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Mock_spectro.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_TCPServer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:34:02.625826 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_MockCamera.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_TCPServer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:34:02.625826 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_ND/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_ND/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10461 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_ND/daq_NDviewer_Mock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:34:02.625826 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/hardware/
--rw-r--r--   0 runner    (1001) docker     (123)    26323 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/hardware/CNRS_degrade.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/hardware/camera_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/hardware/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:34:02.625826 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/models/PIDModelBeamSteering.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:34:02.625826 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-18 13:34:02.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-18 13:34:02.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 13:34:02.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-18 13:34:02.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-18 13:34:02.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-18 13:34:02.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:13.492589 pymodaq_plugins_mock-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-25 16:45:13.492589 pymodaq_plugins_mock-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 16:45:13.492589 pymodaq_plugins_mock-4.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:13.488589 pymodaq_plugins_mock-4.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:13.488589 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:13.488589 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_move_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_move_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_Mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockCamera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockTau.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_TCPServer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:13.488589 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:13.488589 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_MockAdaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TCPServer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:13.492589 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Mock_spectro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_TCPServer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:13.492589 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_MockCamera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_TCPServer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:13.492589 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_ND/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_ND/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10461 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_ND/daq_NDviewer_Mock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:13.492589 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/hardware/
+-rw-r--r--   0 runner    (1001) docker     (123)    26323 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/hardware/CNRS_degrade.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/hardware/camera_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/hardware/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:13.492589 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/models/PIDModelBeamSteering.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:13.488589 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-25 16:45:13.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-25 16:45:13.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:45:13.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-25 16:45:13.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-25 16:45:13.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-25 16:45:13.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock.egg-info/top_level.txt
```

### Comparing `pymodaq_plugins_mock-4.0.1/LICENSE` & `pymodaq_plugins_mock-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.0.1/PKG-INFO` & `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pymodaq_plugins_mock
-Version: 4.0.1
+Name: pymodaq-plugins-mock
+Version: 4.0.2
 Summary: Set of base PyMoDAQ plugins including Mock ones for development
 Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_mock
 Author: Sébastien Weber
 Author-email: sebastien.weber@cemes.fr
 License: CECILL B
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymodaq_plugins_mock-4.0.1/README.rst` & `pymodaq_plugins_mock-4.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.0.1/setup.py` & `pymodaq_plugins_mock-4.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_Mock.py` & `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_Mock.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockCamera.py` & `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockCamera.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockTau.py` & `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockTau.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Mock.py` & `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Mock.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_MockAdaptive.py` & `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_MockAdaptive.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TCPServer.py` & `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TCPServer.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Mock.py` & `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Mock.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Mock_spectro.py` & `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Mock_spectro.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_TCPServer.py` & `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_TCPServer.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Mock.py` & `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Mock.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_MockCamera.py` & `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_MockCamera.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,19 +10,24 @@
 
 
 from pymodaq_plugins_mock.hardware.camera_wrapper import Camera
 
 
 class DAQ_2DViewer_MockCamera(DAQ_Viewer_base):
 
+    live_mode_available = True
+
     params = comon_parameters + [
         {'title': 'Wait time (ms)', 'name': 'wait_time', 'type': 'int', 'value': 100, 'default': 100, 'min': 0},
         {'title': 'Nimages colors:', 'name': 'Nimagescolor', 'type': 'int', 'value': 1, 'default': 1, 'min': 0,
          'max': 3},
         {'title': 'Nimages pannels:', 'name': 'Nimagespannel', 'type': 'int', 'value': 1, 'default': 0, 'min': 0},
+
+        {'title': 'Read only prop:', 'name': 'read_only', 'type': 'bool', 'value': False},
+
         {'title': 'Use ROISelect', 'name': 'use_roi_select', 'type': 'bool', 'value': False},
         {'title': 'Threshold', 'name': 'threshold', 'type': 'int', 'value': 1, 'min': 0},
 
         {'title': 'Values', 'name': 'current_values', 'type': 'group', 'children': [
             {'title': 'X', 'name': 'X', 'type': 'float', 'value': 0.},
             {'title': 'Y', 'name': 'Y', 'type': 'float', 'value': 0.},
             {'title': 'Theta', 'name': 'Theta', 'type': 'float', 'value': 0.},
@@ -60,14 +65,18 @@
         if param.name() in iter_children(self.settings.child('cam_settings'), []):
             if hasattr(self.controller, param.name()):
                 setattr(self.controller, param.name(), param.value())
             self.controller.base_Mock_data()
             self.x_axis = Axis(data=self.controller.x_axis, label='pixel', index=1)
             self.y_axis = Axis(data=self.controller.y_axis, label='pixel', index=0)
 
+        if param.name() == 'read_only':
+            for child in self.settings.child('cam_settings').children():
+                child.setOpts(readonly=param.value())
+
     def ini_detector(self, controller=None):
         self.ini_detector_init(controller, Camera())
         self.emit_status(ThreadCommand('update_main_settings',
                                        [['wait_time'], self.settings['wait_time'], 'value']))
 
         self.controller.base_Mock_data()
         self.x_axis = Axis(data=self.controller.x_axis, label='pixel', index=1)
@@ -115,39 +124,33 @@
             See Also
             --------
             set_Mock_data
         """
         return self.controller.y_axis
 
     def grab_data(self, Naverage=1, **kwargs):
-        """
-            | For each integer step of naverage range set mock data.
-            | Construct the data matrix and send the data_grabed_signal once done.
+        """Start a grab from the detector
 
-            =============== ======== ===============================================
-            **Parameters**  **Type**  **Description**
-            *Naverage*      int       The number of images to average.
-                                      specify the threshold of the mean calculation
-            =============== ======== ===============================================
-
-            See Also
-            --------
-            set_Mock_data
+        Parameters
+        ----------
+        Naverage: int
+            Number of hardware averaging (if hardware averaging is possible, self.hardware_averaging should be set to
+            True in class preamble and you should code this implementation)
+        kwargs: dict
+            others optionals arguments
         """
-
-        "live is an attempt to export data as fast as possible"
         if 'live' in kwargs:
             if kwargs['live']:
                 self.live = True
-                self.live = False  # don't want to use that for the moment
+                # self.live = False  # don't want to use that for the moment
 
         if self.live:
             while self.live:
                 data = self.average_data(Naverage)
-                QThread.msleep(100)
+                QThread.msleep(kwargs.get('wait_time', 100))
                 self.data_grabed_signal.emit(data)
                 QtWidgets.QApplication.processEvents()
         else:
             data = self.average_data(Naverage)
             QThread.msleep(000)
             self.data_grabed_signal.emit(data)
```

### Comparing `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_TCPServer.py` & `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_TCPServer.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_ND/daq_NDviewer_Mock.py` & `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_ND/daq_NDviewer_Mock.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/hardware/CNRS_degrade.png` & `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/hardware/CNRS_degrade.png`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/hardware/camera_wrapper.py` & `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/hardware/camera_wrapper.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/hardware/wrapper.py` & `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/hardware/wrapper.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/models/PIDModelBeamSteering.py` & `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/models/PIDModelBeamSteering.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock.egg-info/PKG-INFO` & `pymodaq_plugins_mock-4.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pymodaq-plugins-mock
-Version: 4.0.1
+Name: pymodaq_plugins_mock
+Version: 4.0.2
 Summary: Set of base PyMoDAQ plugins including Mock ones for development
 Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_mock
 Author: Sébastien Weber
 Author-email: sebastien.weber@cemes.fr
 License: CECILL B
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock.egg-info/SOURCES.txt` & `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

