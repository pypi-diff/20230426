# Comparing `tmp/srsgui-0.2.15.tar.gz` & `tmp/srsgui-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-p97ywxac\srsgui-0.2.15.tar", last modified: Tue Apr 25 23:11:40 2023, max compression
+gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-ps3u1u8m\srsgui-0.2.9.tar", last modified: Tue Apr 11 21:39:00 2023, max compression
```

## Comparing `srsgui-0.2.15.tar` & `srsgui-0.2.9.tar`

### file list

```diff
@@ -1,116 +1,115 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 23:11:40.909423 srsgui-0.2.15/
--rw-rw-rw-   0        0        0     1345 2022-08-02 00:19:43.000000 srsgui-0.2.15/.gitignore
--rw-rw-rw-   0        0        0     1107 2022-12-07 23:27:48.000000 srsgui-0.2.15/LICENSE.txt
--rw-rw-rw-   0        0        0     3331 2023-04-25 23:11:40.909423 srsgui-0.2.15/PKG-INFO
--rw-rw-rw-   0        0        0     2633 2023-02-13 17:17:13.000000 srsgui-0.2.15/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 23:11:40.829466 srsgui-0.2.15/docs/
--rw-rw-rw-   0        0        0      658 2023-01-30 16:55:49.000000 srsgui-0.2.15/docs/Makefile
--rwxrwxrwx   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.15/docs/autodoc.bat
--rwxrwxrwx   0        0        0      804 2023-01-30 16:55:49.000000 srsgui-0.2.15/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-04-25 23:11:40.839461 srsgui-0.2.15/docs/source/
-drwxrwxrwx   0        0        0        0 2023-04-25 23:11:40.849455 srsgui-0.2.15/docs/source/_static/
--rw-rw-rw-   0        0        0    31067 2023-01-30 16:55:49.000000 srsgui-0.2.15/docs/source/_static/cg-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    27242 2023-01-30 16:55:49.000000 srsgui-0.2.15/docs/source/_static/cg-terminal-screen-capture.png
--rw-rw-rw-   0        0        0     5762 2023-01-30 16:55:49.000000 srsgui-0.2.15/docs/source/_static/connect-dialog-box-capture.png
--rw-rw-rw-   0        0        0    71070 2023-01-30 16:55:49.000000 srsgui-0.2.15/docs/source/_static/example-screen-capture-1.png
--rw-rw-rw-   0        0        0    71011 2023-01-30 16:55:49.000000 srsgui-0.2.15/docs/source/_static/example-screen-capture-2.png
--rw-rw-rw-   0        0        0    56013 2023-01-30 16:55:49.000000 srsgui-0.2.15/docs/source/_static/initial-screen-capture.png
--rw-rw-rw-   0        0        0    29667 2023-01-30 16:55:49.000000 srsgui-0.2.15/docs/source/_static/osc-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    50740 2023-01-30 16:55:49.000000 srsgui-0.2.15/docs/source/_static/second-task-screen-capture.png
--rw-rw-rw-   0        0        0    39412 2023-01-30 16:55:49.000000 srsgui-0.2.15/docs/source/_static/terminal-with-example-2.png
--rw-rw-rw-   0        0        0    37573 2023-01-30 16:55:49.000000 srsgui-0.2.15/docs/source/_static/terminal-with-example.png
--rw-rw-rw-   0        0        0     1938 2023-01-30 16:55:49.000000 srsgui-0.2.15/docs/source/conf.py
--rw-rw-rw-   0        0        0     5998 2023-04-04 20:33:11.000000 srsgui-0.2.15/docs/source/create-project.rst
--rw-rw-rw-   0        0        0     6656 2023-04-04 20:33:11.000000 srsgui-0.2.15/docs/source/create-task.rst
--rw-rw-rw-   0        0        0     6110 2023-04-04 20:33:11.000000 srsgui-0.2.15/docs/source/define-instrument.rst
--rw-rw-rw-   0        0        0    15655 2023-04-04 20:33:11.000000 srsgui-0.2.15/docs/source/example.rst
--rw-rw-rw-   0        0        0     3684 2023-04-04 20:33:11.000000 srsgui-0.2.15/docs/source/index.rst
--rw-rw-rw-   0        0        0     4383 2023-04-04 20:33:11.000000 srsgui-0.2.15/docs/source/installation.rst
--rw-rw-rw-   0        0        0      936 2023-01-30 16:55:49.000000 srsgui-0.2.15/docs/source/srsgui.inst.communications.rst
--rw-rw-rw-   0        0        0      950 2023-01-30 16:55:49.000000 srsgui-0.2.15/docs/source/srsgui.inst.rst
--rw-rw-rw-   0        0        0      117 2023-01-30 16:55:49.000000 srsgui-0.2.15/docs/source/srsgui.rst
--rw-rw-rw-   0        0        0      989 2023-01-30 16:55:49.000000 srsgui-0.2.15/docs/source/srsgui.task.rst
--rw-rw-rw-   0        0        0      604 2023-01-30 16:55:49.000000 srsgui-0.2.15/docs/source/srsgui.ui.qt.rst
--rw-rw-rw-   0        0        0     1629 2023-01-30 16:55:49.000000 srsgui-0.2.15/docs/source/srsgui.ui.rst
--rw-rw-rw-   0        0        0     1197 2023-04-14 19:10:41.000000 srsgui-0.2.15/pyproject.toml
--rw-rw-rw-   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.15/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 23:11:40.909423 srsgui-0.2.15/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsgui-0.2.15/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-25 23:11:40.849455 srsgui-0.2.15/srsgui/
--rw-rw-rw-   0        0        0     1538 2023-04-25 22:53:58.000000 srsgui-0.2.15/srsgui/__init__.py
--rw-rw-rw-   0        0        0      314 2023-04-07 00:52:02.000000 srsgui-0.2.15/srsgui/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 23:11:40.809477 srsgui-0.2.15/srsgui/examples/
-drwxrwxrwx   0        0        0        0 2023-04-25 23:11:40.849455 srsgui-0.2.15/srsgui/examples/oscilloscope example/
-drwxrwxrwx   0        0        0        0 2023-04-25 23:11:40.859450 srsgui-0.2.15/srsgui/examples/oscilloscope example/instruments/
--rw-rw-rw-   0        0        0     1709 2023-01-30 16:55:49.000000 srsgui-0.2.15/srsgui/examples/oscilloscope example/instruments/cg635.py
--rw-rw-rw-   0        0        0     3025 2023-02-11 01:21:41.000000 srsgui-0.2.15/srsgui/examples/oscilloscope example/instruments/sds1202.py
--rw-rw-rw-   0        0        0     1977 2023-01-30 16:55:49.000000 srsgui-0.2.15/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
-drwxrwxrwx   0        0        0        0 2023-04-25 23:11:40.859450 srsgui-0.2.15/srsgui/examples/oscilloscope example/tasks/
--rw-rw-rw-   0        0        0     2401 2023-01-30 16:55:49.000000 srsgui-0.2.15/srsgui/examples/oscilloscope example/tasks/fifth.py
--rw-rw-rw-   0        0        0     1543 2023-01-30 16:55:49.000000 srsgui-0.2.15/srsgui/examples/oscilloscope example/tasks/first.py
--rw-rw-rw-   0        0        0     3978 2023-01-30 16:55:49.000000 srsgui-0.2.15/srsgui/examples/oscilloscope example/tasks/fourth.py
--rw-rw-rw-   0        0        0     2129 2023-01-30 16:55:49.000000 srsgui-0.2.15/srsgui/examples/oscilloscope example/tasks/second.py
--rw-rw-rw-   0        0        0     1893 2023-01-30 16:55:49.000000 srsgui-0.2.15/srsgui/examples/oscilloscope example/tasks/third.py
-drwxrwxrwx   0        0        0        0 2023-04-25 23:11:40.869444 srsgui-0.2.15/srsgui/inst/
--rw-rw-rw-   0        0        0     1074 2023-04-04 20:33:11.000000 srsgui-0.2.15/srsgui/inst/__init__.py
--rw-rw-rw-   0        0        0     9581 2023-04-25 22:43:06.000000 srsgui-0.2.15/srsgui/inst/commands.py
-drwxrwxrwx   0        0        0        0 2023-04-25 23:11:40.869444 srsgui-0.2.15/srsgui/inst/communications/
--rw-rw-rw-   0        0        0      126 2023-01-30 16:55:49.000000 srsgui-0.2.15/srsgui/inst/communications/__init__.py
--rw-rw-rw-   0        0        0     7903 2023-01-30 16:55:49.000000 srsgui-0.2.15/srsgui/inst/communications/interface.py
--rw-rw-rw-   0        0        0     1157 2023-01-30 16:55:49.000000 srsgui-0.2.15/srsgui/inst/communications/serial_ports.py
--rw-rw-rw-   0        0        0     8097 2023-01-30 16:55:49.000000 srsgui-0.2.15/srsgui/inst/communications/serialinterface.py
--rw-rw-rw-   0        0        0    10762 2023-01-30 16:55:49.000000 srsgui-0.2.15/srsgui/inst/communications/tcpipinterface.py
--rw-rw-rw-   0        0        0    14665 2023-04-11 20:13:55.000000 srsgui-0.2.15/srsgui/inst/component.py
--rw-rw-rw-   0        0        0      727 2023-01-30 16:55:49.000000 srsgui-0.2.15/srsgui/inst/exceptions.py
--rw-rw-rw-   0        0        0    10052 2023-04-13 19:22:26.000000 srsgui-0.2.15/srsgui/inst/indexcommands.py
--rw-rw-rw-   0        0        0     9647 2023-02-09 17:58:55.000000 srsgui-0.2.15/srsgui/inst/instrument.py
-drwxrwxrwx   0        0        0        0 2023-04-25 23:11:40.879439 srsgui-0.2.15/srsgui/task/
--rw-rw-rw-   0        0        0        2 2023-04-10 22:51:26.000000 srsgui-0.2.15/srsgui/task/__init__.py
--rw-rw-rw-   0        0        0      692 2023-01-30 16:55:49.000000 srsgui-0.2.15/srsgui/task/callbacks.py
--rw-rw-rw-   0        0        0     6485 2023-04-07 01:13:40.000000 srsgui-0.2.15/srsgui/task/config.py
--rw-rw-rw-   0        0        0     5203 2023-04-11 00:24:36.000000 srsgui-0.2.15/srsgui/task/inputs.py
--rw-rw-rw-   0        0        0     6865 2023-03-28 15:59:44.000000 srsgui-0.2.15/srsgui/task/sessionhandler.py
--rw-rw-rw-   0        0        0    22017 2023-04-24 19:12:17.000000 srsgui-0.2.15/srsgui/task/task.py
--rw-rw-rw-   0        0        0     4108 2023-01-30 16:55:49.000000 srsgui-0.2.15/srsgui/task/taskresult.py
-drwxrwxrwx   0        0        0        0 2023-04-25 23:11:40.889465 srsgui-0.2.15/srsgui/ui/
--rw-rw-rw-   0        0        0        0 2023-01-30 16:55:49.000000 srsgui-0.2.15/srsgui/ui/__init__.py
--rw-rw-rw-   0        0        0     3775 2023-04-04 20:33:12.000000 srsgui-0.2.15/srsgui/ui/commandhandler.py
--rw-rw-rw-   0        0        0     6019 2023-04-25 20:34:18.000000 srsgui-0.2.15/srsgui/ui/commandterminal.py
-drwxrwxrwx   0        0        0        0 2023-04-25 23:11:40.899428 srsgui-0.2.15/srsgui/ui/commandtree/
--rw-rw-rw-   0        0        0     2919 2023-04-07 19:57:55.000000 srsgui-0.2.15/srsgui/ui/commandtree/commandcapturewidget.py
--rw-rw-rw-   0        0        0     3362 2023-04-10 22:51:26.000000 srsgui-0.2.15/srsgui/ui/commandtree/commandcapturewidget.ui
--rw-rw-rw-   0        0        0     3633 2023-04-13 17:29:00.000000 srsgui-0.2.15/srsgui/ui/commandtree/commanddelegate.py
--rw-rw-rw-   0        0        0     1484 2023-04-25 22:09:06.000000 srsgui-0.2.15/srsgui/ui/commandtree/commandhandler.py
--rw-rw-rw-   0        0        0    11829 2023-04-25 22:14:10.000000 srsgui-0.2.15/srsgui/ui/commandtree/commanditem.py
--rw-rw-rw-   0        0        0     8234 2023-04-25 21:16:08.000000 srsgui-0.2.15/srsgui/ui/commandtree/commandmodel.py
--rw-rw-rw-   0        0        0     4860 2023-04-14 20:21:10.000000 srsgui-0.2.15/srsgui/ui/commandtree/commandspinbox.py
--rw-rw-rw-   0        0        0     3331 2023-04-12 19:07:11.000000 srsgui-0.2.15/srsgui/ui/commandtree/commandtreeview.py
--rw-rw-rw-   0        0        0     3989 2023-04-14 23:16:24.000000 srsgui-0.2.15/srsgui/ui/commandtree/commandtreewidget.py
--rw-rw-rw-   0        0        0     9296 2023-04-07 19:57:55.000000 srsgui-0.2.15/srsgui/ui/commandtree/jsonmodel.py
--rw-rw-rw-   0        0        0     4803 2023-04-10 22:51:26.000000 srsgui-0.2.15/srsgui/ui/commandtree/ui_commandcapturewidget.py
--rw-rw-rw-   0        0        0     4806 2023-04-11 17:35:42.000000 srsgui-0.2.15/srsgui/ui/commandtree/ui_commandtreewidget.py
--rw-rw-rw-   0        0        0     9679 2023-04-07 01:13:40.000000 srsgui-0.2.15/srsgui/ui/connectdlg.py
--rw-rw-rw-   0        0        0     3856 2023-04-04 20:33:12.000000 srsgui-0.2.15/srsgui/ui/deviceinfohandler.py
--rw-rw-rw-   0        0        0    15759 2023-04-25 19:32:12.000000 srsgui-0.2.15/srsgui/ui/dockhandler.py
--rw-rw-rw-   0        0        0    13671 2023-04-11 00:24:36.000000 srsgui-0.2.15/srsgui/ui/inputpanel.py
-drwxrwxrwx   0        0        0        0 2023-04-25 23:11:40.899428 srsgui-0.2.15/srsgui/ui/qt/
--rw-rw-rw-   0        0        0      678 2023-01-30 16:55:49.000000 srsgui-0.2.15/srsgui/ui/qt/QtCore.py
--rw-rw-rw-   0        0        0      556 2023-01-30 16:55:49.000000 srsgui-0.2.15/srsgui/ui/qt/QtGui.py
--rw-rw-rw-   0        0        0      656 2023-01-30 16:55:49.000000 srsgui-0.2.15/srsgui/ui/qt/QtWidgets.py
--rw-rw-rw-   0        0        0     1457 2023-03-08 01:32:20.000000 srsgui-0.2.15/srsgui/ui/qt/__init__.py
--rw-rw-rw-   0        0        0     1164 2023-01-30 16:55:49.000000 srsgui-0.2.15/srsgui/ui/qtloghandler.py
--rw-rw-rw-   0        0        0      268 2023-01-30 16:55:49.000000 srsgui-0.2.15/srsgui/ui/resource.qrc
--rw-rw-rw-   0        0        0    15358 2023-01-30 16:55:49.000000 srsgui-0.2.15/srsgui/ui/resource_rc.py
--rw-rw-rw-   0        0        0     2598 2023-01-30 16:55:49.000000 srsgui-0.2.15/srsgui/ui/signalhandler.py
--rw-rw-rw-   0        0        0    47891 2023-01-30 16:55:49.000000 srsgui-0.2.15/srsgui/ui/srslogo.jpg
--rw-rw-rw-   0        0        0      886 2023-01-30 16:55:49.000000 srsgui-0.2.15/srsgui/ui/stdout.py
--rw-rw-rw-   0        0        0    24562 2023-04-25 18:30:32.000000 srsgui-0.2.15/srsgui/ui/taskmain.py
--rw-rw-rw-   0        0        0    10403 2023-02-22 17:26:46.000000 srsgui-0.2.15/srsgui/ui/taskmain.ui
--rw-rw-rw-   0        0        0    11293 2023-02-22 17:26:46.000000 srsgui-0.2.15/srsgui/ui/ui_taskmain.py
-drwxrwxrwx   0        0        0        0 2023-04-25 23:11:40.849455 srsgui-0.2.15/srsgui.egg-info/
--rw-rw-rw-   0        0        0     3331 2023-04-25 23:11:40.000000 srsgui-0.2.15/srsgui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3202 2023-04-25 23:11:40.000000 srsgui-0.2.15/srsgui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 23:11:40.000000 srsgui-0.2.15/srsgui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-25 23:11:40.000000 srsgui-0.2.15/srsgui.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       53 2023-04-25 23:11:40.000000 srsgui-0.2.15/srsgui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-25 23:11:40.000000 srsgui-0.2.15/srsgui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.979862 srsgui-0.2.9/
+-rw-rw-rw-   0        0        0     1345 2022-08-02 00:19:43.000000 srsgui-0.2.9/.gitignore
+-rw-rw-rw-   0        0        0     1107 2022-12-07 23:27:48.000000 srsgui-0.2.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     3330 2023-04-11 21:39:00.979862 srsgui-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2633 2023-02-13 17:17:13.000000 srsgui-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.889910 srsgui-0.2.9/docs/
+-rw-rw-rw-   0        0        0      658 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/Makefile
+-rwxrwxrwx   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/autodoc.bat
+-rwxrwxrwx   0        0        0      804 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.899904 srsgui-0.2.9/docs/source/
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.919894 srsgui-0.2.9/docs/source/_static/
+-rw-rw-rw-   0        0        0    31067 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/cg-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    27242 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/cg-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0     5762 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/connect-dialog-box-capture.png
+-rw-rw-rw-   0        0        0    71070 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/example-screen-capture-1.png
+-rw-rw-rw-   0        0        0    71011 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/example-screen-capture-2.png
+-rw-rw-rw-   0        0        0    56013 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/initial-screen-capture.png
+-rw-rw-rw-   0        0        0    29667 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/osc-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    50740 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/second-task-screen-capture.png
+-rw-rw-rw-   0        0        0    39412 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/terminal-with-example-2.png
+-rw-rw-rw-   0        0        0    37573 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/terminal-with-example.png
+-rw-rw-rw-   0        0        0     1938 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/conf.py
+-rw-rw-rw-   0        0        0     5998 2023-04-04 20:33:11.000000 srsgui-0.2.9/docs/source/create-project.rst
+-rw-rw-rw-   0        0        0     6656 2023-04-04 20:33:11.000000 srsgui-0.2.9/docs/source/create-task.rst
+-rw-rw-rw-   0        0        0     6110 2023-04-04 20:33:11.000000 srsgui-0.2.9/docs/source/define-instrument.rst
+-rw-rw-rw-   0        0        0    15655 2023-04-04 20:33:11.000000 srsgui-0.2.9/docs/source/example.rst
+-rw-rw-rw-   0        0        0     3684 2023-04-04 20:33:11.000000 srsgui-0.2.9/docs/source/index.rst
+-rw-rw-rw-   0        0        0     4383 2023-04-04 20:33:11.000000 srsgui-0.2.9/docs/source/installation.rst
+-rw-rw-rw-   0        0        0      936 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/srsgui.inst.communications.rst
+-rw-rw-rw-   0        0        0      950 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/srsgui.inst.rst
+-rw-rw-rw-   0        0        0      117 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/srsgui.rst
+-rw-rw-rw-   0        0        0      989 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/srsgui.task.rst
+-rw-rw-rw-   0        0        0      604 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/srsgui.ui.qt.rst
+-rw-rw-rw-   0        0        0     1629 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/srsgui.ui.rst
+-rw-rw-rw-   0        0        0     1193 2023-04-07 01:13:40.000000 srsgui-0.2.9/pyproject.toml
+-rw-rw-rw-   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 21:39:00.979862 srsgui-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsgui-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.919894 srsgui-0.2.9/srsgui/
+-rw-rw-rw-   0        0        0     1537 2023-04-11 21:34:20.000000 srsgui-0.2.9/srsgui/__init__.py
+-rw-rw-rw-   0        0        0      314 2023-04-07 00:52:02.000000 srsgui-0.2.9/srsgui/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.879943 srsgui-0.2.9/srsgui/examples/
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.919894 srsgui-0.2.9/srsgui/examples/oscilloscope example/
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.919894 srsgui-0.2.9/srsgui/examples/oscilloscope example/instruments/
+-rw-rw-rw-   0        0        0     1709 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/instruments/cg635.py
+-rw-rw-rw-   0        0        0     3025 2023-02-11 01:21:41.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/instruments/sds1202.py
+-rw-rw-rw-   0        0        0     1977 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.929916 srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/
+-rw-rw-rw-   0        0        0     2401 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/fifth.py
+-rw-rw-rw-   0        0        0     1543 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/first.py
+-rw-rw-rw-   0        0        0     3978 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/fourth.py
+-rw-rw-rw-   0        0        0     2129 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/second.py
+-rw-rw-rw-   0        0        0     1893 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/third.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.939882 srsgui-0.2.9/srsgui/inst/
+-rw-rw-rw-   0        0        0     1074 2023-04-04 20:33:11.000000 srsgui-0.2.9/srsgui/inst/__init__.py
+-rw-rw-rw-   0        0        0     9578 2023-04-10 22:51:26.000000 srsgui-0.2.9/srsgui/inst/commands.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.939882 srsgui-0.2.9/srsgui/inst/communications/
+-rw-rw-rw-   0        0        0      126 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/inst/communications/__init__.py
+-rw-rw-rw-   0        0        0     7903 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/inst/communications/interface.py
+-rw-rw-rw-   0        0        0     1157 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/inst/communications/serial_ports.py
+-rw-rw-rw-   0        0        0     8097 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/inst/communications/serialinterface.py
+-rw-rw-rw-   0        0        0    10762 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/inst/communications/tcpipinterface.py
+-rw-rw-rw-   0        0        0    14665 2023-04-11 20:13:55.000000 srsgui-0.2.9/srsgui/inst/component.py
+-rw-rw-rw-   0        0        0      727 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/inst/exceptions.py
+-rw-rw-rw-   0        0        0    10049 2023-04-11 18:04:43.000000 srsgui-0.2.9/srsgui/inst/indexcommands.py
+-rw-rw-rw-   0        0        0     9647 2023-02-09 17:58:55.000000 srsgui-0.2.9/srsgui/inst/instrument.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.949878 srsgui-0.2.9/srsgui/task/
+-rw-rw-rw-   0        0        0        2 2023-04-10 22:51:26.000000 srsgui-0.2.9/srsgui/task/__init__.py
+-rw-rw-rw-   0        0        0      692 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/task/callbacks.py
+-rw-rw-rw-   0        0        0     6485 2023-04-07 01:13:40.000000 srsgui-0.2.9/srsgui/task/config.py
+-rw-rw-rw-   0        0        0     5203 2023-04-11 00:24:36.000000 srsgui-0.2.9/srsgui/task/inputs.py
+-rw-rw-rw-   0        0        0     6865 2023-03-28 15:59:44.000000 srsgui-0.2.9/srsgui/task/sessionhandler.py
+-rw-rw-rw-   0        0        0    22234 2023-04-10 22:51:26.000000 srsgui-0.2.9/srsgui/task/task.py
+-rw-rw-rw-   0        0        0     4108 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/task/taskresult.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.959872 srsgui-0.2.9/srsgui/ui/
+-rw-rw-rw-   0        0        0        0 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/__init__.py
+-rw-rw-rw-   0        0        0     3775 2023-04-04 20:33:12.000000 srsgui-0.2.9/srsgui/ui/commandhandler.py
+-rw-rw-rw-   0        0        0     5918 2023-04-04 20:33:12.000000 srsgui-0.2.9/srsgui/ui/commandterminal.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.969903 srsgui-0.2.9/srsgui/ui/commandtree/
+-rw-rw-rw-   0        0        0     2919 2023-04-07 19:57:55.000000 srsgui-0.2.9/srsgui/ui/commandtree/commandcapturewidget.py
+-rw-rw-rw-   0        0        0     3362 2023-04-10 22:51:26.000000 srsgui-0.2.9/srsgui/ui/commandtree/commandcapturewidget.ui
+-rw-rw-rw-   0        0        0     3489 2023-04-11 17:28:55.000000 srsgui-0.2.9/srsgui/ui/commandtree/commanddelegate.py
+-rw-rw-rw-   0        0        0    10180 2023-04-10 18:03:49.000000 srsgui-0.2.9/srsgui/ui/commandtree/commanditem.py
+-rw-rw-rw-   0        0        0     7833 2023-04-11 17:29:16.000000 srsgui-0.2.9/srsgui/ui/commandtree/commandmodel.py
+-rw-rw-rw-   0        0        0     4755 2023-04-11 17:22:27.000000 srsgui-0.2.9/srsgui/ui/commandtree/commandspinbox.py
+-rw-rw-rw-   0        0        0     3127 2023-04-11 21:33:12.000000 srsgui-0.2.9/srsgui/ui/commandtree/commandtreeview.py
+-rw-rw-rw-   0        0        0     3844 2023-04-11 17:33:14.000000 srsgui-0.2.9/srsgui/ui/commandtree/commandtreewidget.py
+-rw-rw-rw-   0        0        0     9296 2023-04-07 19:57:55.000000 srsgui-0.2.9/srsgui/ui/commandtree/jsonmodel.py
+-rw-rw-rw-   0        0        0     4803 2023-04-10 22:51:26.000000 srsgui-0.2.9/srsgui/ui/commandtree/ui_commandcapturewidget.py
+-rw-rw-rw-   0        0        0     4806 2023-04-11 17:35:42.000000 srsgui-0.2.9/srsgui/ui/commandtree/ui_commandtreewidget.py
+-rw-rw-rw-   0        0        0     9679 2023-04-07 01:13:40.000000 srsgui-0.2.9/srsgui/ui/connectdlg.py
+-rw-rw-rw-   0        0        0     3856 2023-04-04 20:33:12.000000 srsgui-0.2.9/srsgui/ui/deviceinfohandler.py
+-rw-rw-rw-   0        0        0    14127 2023-04-07 19:57:55.000000 srsgui-0.2.9/srsgui/ui/dockhandler.py
+-rw-rw-rw-   0        0        0    13671 2023-04-11 00:24:36.000000 srsgui-0.2.9/srsgui/ui/inputpanel.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.979862 srsgui-0.2.9/srsgui/ui/qt/
+-rw-rw-rw-   0        0        0      678 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/qt/QtCore.py
+-rw-rw-rw-   0        0        0      556 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/qt/QtGui.py
+-rw-rw-rw-   0        0        0      656 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/qt/QtWidgets.py
+-rw-rw-rw-   0        0        0     1457 2023-03-08 01:32:20.000000 srsgui-0.2.9/srsgui/ui/qt/__init__.py
+-rw-rw-rw-   0        0        0     1164 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/qtloghandler.py
+-rw-rw-rw-   0        0        0      268 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/resource.qrc
+-rw-rw-rw-   0        0        0    15358 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/resource_rc.py
+-rw-rw-rw-   0        0        0     2598 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/signalhandler.py
+-rw-rw-rw-   0        0        0    47891 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/srslogo.jpg
+-rw-rw-rw-   0        0        0      886 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/stdout.py
+-rw-rw-rw-   0        0        0    24758 2023-04-10 15:41:10.000000 srsgui-0.2.9/srsgui/ui/taskmain.py
+-rw-rw-rw-   0        0        0    10403 2023-02-22 17:26:46.000000 srsgui-0.2.9/srsgui/ui/taskmain.ui
+-rw-rw-rw-   0        0        0    11293 2023-02-22 17:26:46.000000 srsgui-0.2.9/srsgui/ui/ui_taskmain.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.919894 srsgui-0.2.9/srsgui.egg-info/
+-rw-rw-rw-   0        0        0     3330 2023-04-11 21:39:00.000000 srsgui-0.2.9/srsgui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3162 2023-04-11 21:39:00.000000 srsgui-0.2.9/srsgui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 21:39:00.000000 srsgui-0.2.9/srsgui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-11 21:39:00.000000 srsgui-0.2.9/srsgui.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       53 2023-04-11 21:39:00.000000 srsgui-0.2.9/srsgui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-11 21:39:00.000000 srsgui-0.2.9/srsgui.egg-info/top_level.txt
```

### Comparing `srsgui-0.2.15/.gitignore` & `srsgui-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/LICENSE.txt` & `srsgui-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/PKG-INFO` & `srsgui-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.2.15
+Version: 0.2.9
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Keywords: instrument control,data acquisition,data visualization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `srsgui-0.2.15/README.md` & `srsgui-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/docs/Makefile` & `srsgui-0.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/docs/make.bat` & `srsgui-0.2.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/docs/source/_static/cg-dir-terminal-screen-capture.png` & `srsgui-0.2.9/docs/source/_static/cg-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/docs/source/_static/cg-terminal-screen-capture.png` & `srsgui-0.2.9/docs/source/_static/cg-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/docs/source/_static/connect-dialog-box-capture.png` & `srsgui-0.2.9/docs/source/_static/connect-dialog-box-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/docs/source/_static/example-screen-capture-1.png` & `srsgui-0.2.9/docs/source/_static/example-screen-capture-1.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/docs/source/_static/example-screen-capture-2.png` & `srsgui-0.2.9/docs/source/_static/example-screen-capture-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/docs/source/_static/initial-screen-capture.png` & `srsgui-0.2.9/docs/source/_static/initial-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/docs/source/_static/osc-dir-terminal-screen-capture.png` & `srsgui-0.2.9/docs/source/_static/osc-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/docs/source/_static/second-task-screen-capture.png` & `srsgui-0.2.9/docs/source/_static/second-task-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/docs/source/_static/terminal-with-example-2.png` & `srsgui-0.2.9/docs/source/_static/terminal-with-example-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/docs/source/_static/terminal-with-example.png` & `srsgui-0.2.9/docs/source/_static/terminal-with-example.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/docs/source/conf.py` & `srsgui-0.2.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/docs/source/create-project.rst` & `srsgui-0.2.9/docs/source/create-project.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/docs/source/create-task.rst` & `srsgui-0.2.9/docs/source/create-task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/docs/source/define-instrument.rst` & `srsgui-0.2.9/docs/source/define-instrument.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/docs/source/example.rst` & `srsgui-0.2.9/docs/source/example.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/docs/source/index.rst` & `srsgui-0.2.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/docs/source/installation.rst` & `srsgui-0.2.9/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/docs/source/srsgui.inst.communications.rst` & `srsgui-0.2.9/docs/source/srsgui.inst.communications.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/docs/source/srsgui.inst.rst` & `srsgui-0.2.9/docs/source/srsgui.inst.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/docs/source/srsgui.task.rst` & `srsgui-0.2.9/docs/source/srsgui.task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/docs/source/srsgui.ui.qt.rst` & `srsgui-0.2.9/docs/source/srsgui.ui.qt.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/docs/source/srsgui.ui.rst` & `srsgui-0.2.9/docs/source/srsgui.ui.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/pyproject.toml` & `srsgui-0.2.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -19,22 +19,23 @@
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Topic :: Scientific/Engineering"
 ]
 dependencies = [
-    "pyserial >= 3",
+    "pyserial>=3",
 ]
 dynamic = ["version"]
 
 [tool.setuptools.dynamic]
 version = {attr = "srsgui.__version__"}
 
 [project.optional-dependencies]
-full = ['matplotlib >= 3.6.2', 'pyside6 != 6.5.0']
+full = ['matplotlib>=3.6.2', 'pyside6!=6.5.0']
+
 
 [project.scripts]
 srsgui = "srsgui.__main__:main"
 
 # ... other project metadata fields as specified in:
 #     https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
```

### Comparing `srsgui-0.2.15/srsgui/__init__.py` & `srsgui-0.2.9/srsgui/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
                         InstLoginFailureError, InstIdError, \
                         InstSetError, InstQueryError, InstIndexError
 
 from srsgui.inst import Interface, SerialInterface, TcpipInterface
 from srsgui.inst.instrument import Instrument
 from srsgui.inst.component import Component
 
-__version__ = "0.2.15"  # Global version number
+__version__ = "0.2.9"  # Global version number
```

### Comparing `srsgui-0.2.15/srsgui/examples/oscilloscope example/instruments/cg635.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/instruments/cg635.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/examples/oscilloscope example/instruments/sds1202.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/instruments/sds1202.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/examples/oscilloscope example/tasks/fifth.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/fifth.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/examples/oscilloscope example/tasks/first.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/first.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/examples/oscilloscope example/tasks/fourth.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/fourth.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/examples/oscilloscope example/tasks/second.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/second.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/examples/oscilloscope example/tasks/third.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/third.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/inst/__init__.py` & `srsgui-0.2.9/srsgui/inst/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/inst/commands.py` & `srsgui-0.2.9/srsgui/inst/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
     def __get__(self, instance, instance_type):
         if instance is None:
             return self
         query_string = self._get_command_format.format(self.remote_command)
         reply = None
         try:
-            reply = instance.comm.query_text(query_string).strip()
+            reply = instance.comm.query_text(query_string)
             if callable(self._get_convert_function):
                 self._value = self._get_convert_function(reply)
 
             else:
                 self._value = reply
         except InstCommunicationError:
             raise InstQueryError('Error during querying: CMD: {}'.format(query_string))
@@ -212,15 +212,15 @@
 
 class FloatCommand(Command):
     """
     Descriptor for a remote command to
     **set** and **query** a **float** value
     """
 
-    def __init__(self, remote_command_name, unit='', min=-1e6, max=1e6, step=1e-9,
+    def __init__(self, remote_command_name, unit='', min=-1000.0, max=1000.0, step=0.1,
                  significant_figures=4, default_value=None):
         super().__init__(remote_command_name, default_value)
         self._get_convert_function = float
 
         self.unit = unit
         self.maximum = max
         self.minimum = min
```

### Comparing `srsgui-0.2.15/srsgui/inst/communications/interface.py` & `srsgui-0.2.9/srsgui/inst/communications/interface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/inst/communications/serial_ports.py` & `srsgui-0.2.9/srsgui/inst/communications/serial_ports.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/inst/communications/serialinterface.py` & `srsgui-0.2.9/srsgui/inst/communications/serialinterface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/inst/communications/tcpipinterface.py` & `srsgui-0.2.9/srsgui/inst/communications/tcpipinterface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/inst/component.py` & `srsgui-0.2.9/srsgui/inst/component.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/inst/exceptions.py` & `srsgui-0.2.9/srsgui/inst/exceptions.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/inst/indexcommands.py` & `srsgui-0.2.9/srsgui/inst/indexcommands.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,28 +199,27 @@
 
 class IntIndexGetCommand(IntIndexCommand):
     """
     Command class for a remote command with index
     using only **query** returning an **integer**, without **set**.
     """
     _set_enable = False
-
     def __setitem__(self, instance, value):
         raise InstIndexError('No set allowed for index command {}'
                              .format(self.remote_command))
 
 
 class FloatIndexCommand(IndexCommand):
     """
     Command class for a remote command with index
     using **set** and **query** returning an **float**
     """
 
     def __init__(self, remote_command_name, index_max, index_min=0, index_dict=None,
-                 unit='', value_min=-1e6, value_max=1e6, step=1e-9, significant_figures=4, default_valaue=0.0 ):
+                 unit='', value_min=-1e6, value_max=1e6, step=0.1, significant_figures=4, default_valaue=0.0 ):
         super().__init__(remote_command_name, index_max, index_min, index_dict)
         self._get_convert_function = float
 
         self.unit = unit
         self.maximum = value_max
         self.minimum = value_min
         self.step = step
```

### Comparing `srsgui-0.2.15/srsgui/inst/instrument.py` & `srsgui-0.2.9/srsgui/inst/instrument.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/task/callbacks.py` & `srsgui-0.2.9/srsgui/task/callbacks.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/task/config.py` & `srsgui-0.2.9/srsgui/task/config.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/task/inputs.py` & `srsgui-0.2.9/srsgui/task/inputs.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/task/sessionhandler.py` & `srsgui-0.2.9/srsgui/task/sessionhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/task/task.py` & `srsgui-0.2.9/srsgui/task/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,15 +276,15 @@
             self._keep_running = False
 
     def delay(self, seconds):
         """
         Check if the task is stopped and wait for the given seconds.
         """
         if not self._keep_running:
-            raise Task.TaskException('Task is requested to stop')
+            raise KeyboardInterrupt('Task is stopped')
         else:
             time.sleep(seconds)
 
     def set_session_handler(self, session_handler):
         """
         Parent should set a session handler for Task to use file output.
         """
@@ -350,15 +350,15 @@
     def clear_figures(self):
         """
         Clear all the figures in figure_dict
         """
         for fig in self.figure_dict.values():
             if hasattr(fig, 'canvas'):
                 fig.clear()
-                self.request_figure_update(fig)
+                self.request_figure_update()
 
     def is_running(self):
         """
         Task should check is_running() is True.
         If it returns False, Task should stop ASAP.
         """
         return self._keep_running
@@ -512,18 +512,24 @@
             raise TypeError('{} is not  a Figure'.format(type(figure)))
         self.callbacks.figure_update_requested(figure)
 
     # It needs a matching update() as a slot to run from UI
     def notify_data_available(self, data={}):
         self.callbacks.data_available(data)
 
+    # These callbacks are used to update display for streaming data from another class or thread
+    # Signals are wrapped as a callback functions 
+
+    def data_available_callback(self, data={}, *args):
+        self.callbacks.data_available(data)
+
     def update(self, data: dict):
         """
-        when notify_data_available is called, this method handles data processing
-        and display update. By default, it does no data handling, but figure update request.
+        when data_available signal emits, this method handles display update.
+        By default, it does no data handling, but figure update request.
         GUI related data processing needs to be done here to be handled
         in proper order by the GUI event loop handler.
         """
         self.request_figure_update()
 
     def get_instrument(self, name):
         """Get an instrument from parent's inst_dict and check its validity"""
```

### Comparing `srsgui-0.2.15/srsgui/task/taskresult.py` & `srsgui-0.2.9/srsgui/task/taskresult.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/ui/commandhandler.py` & `srsgui-0.2.9/srsgui/ui/commandhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/ui/commandterminal.py` & `srsgui-0.2.9/srsgui/ui/commandterminal.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,10 @@
             self.command_requested.emit(cmd, '')
 
         except Exception as e:
             self.tbCommand.append('Error: {}'.format(str(e)))
 
     def handle_command(self, cmd, reply):
         try:
-            if reply:
-                self.tbCommand.append(f'{cmd}   ==>   {reply}')
-            else:
-                self.tbCommand.append(f'{cmd}')
-
+            self.tbCommand.append(f'{cmd}  :  {reply}')
         except Exception as e:
             self.tbCommand.append('Error from CommandTerminal: {}'.format(str(e)))
```

### Comparing `srsgui-0.2.15/srsgui/ui/commandtree/commandcapturewidget.py` & `srsgui-0.2.9/srsgui/ui/commandtree/commandcapturewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/ui/commandtree/commandcapturewidget.ui` & `srsgui-0.2.9/srsgui/ui/commandtree/commandcapturewidget.ui`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/ui/commandtree/commanddelegate.py` & `srsgui-0.2.9/srsgui/ui/commandtree/commanddelegate.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,30 +19,30 @@
         if item.comp_type == Index:
             comp = item.parent().comp
             comp_type = item.parent().comp_type
         else:
             comp = item.comp
             comp_type = item.comp_type
 
-        if issubclass(comp_type, FloatCommand) or issubclass(comp_type, FloatIndexCommand):
+        if comp_type in (FloatCommand, FloatIndexCommand):
             editor = FloatSpinBox(parent)
             editor.setDecimals(10)
             editor.setSingleStep(0.1)
             editor.setMinimum(comp.minimum)
             editor.setMaximum(comp.maximum)
-            editor.setSuffix(' ' + comp.unit)
+            editor.setSuffix(comp.unit)
             editor.set_significant_figures(comp.significant_figures)
             editor.set_minimum_step(comp.step)
             return editor
 
-        elif issubclass(comp_type, IntCommand) or issubclass(comp_type, IntIndexCommand):
+        elif comp_type in (IntCommand, IntIndexCommand):
             editor = IntegerSpinBox(parent)
             editor.setMinimum(comp.minimum)
             editor.setMaximum(comp.maximum)
-            editor.setSuffix(' ' + comp.unit)
+            editor.setSuffix(comp.unit)
             return editor
 
         elif comp_type in (DictCommand, DictIndexCommand):
             editor = QComboBox(parent)
             for key in comp.set_dict.keys():
                 editor.addItem(str(key))
             return editor
@@ -67,20 +67,20 @@
         if item.comp_type == Index:
             comp = item.parent().comp
             comp_type = item.parent().comp_type
         else:
             comp = item.comp
             comp_type = item.comp_type
 
-        if issubclass(comp_type, FloatCommand) or issubclass(comp_type, FloatIndexCommand):
+        if comp_type in (FloatCommand, FloatIndexCommand):
             value = editor.value()
             model.setData(index, value, Qt.EditRole)
             item.precision = editor.precision
             return True
-        elif issubclass(comp_type, IntCommand) or issubclass(comp_type, IntIndexCommand):
+        elif comp_type in (IntCommand, IntIndexCommand):
             value = editor.value()
             model.setData(index, value, Qt.EditRole)
             return True
         elif comp_type in (DictCommand, DictIndexCommand):
             val = editor.currentText()
             convert = type(list(comp.get_dict.keys())[0])
             value = convert(val)
```

### Comparing `srsgui-0.2.15/srsgui/ui/commandtree/commanditem.py` & `srsgui-0.2.9/srsgui/ui/commandtree/commanditem.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,740 +1,637 @@
-00000000: 0d0a 696d 706f 7274 2074 696d 650d 0a69  ..import time..i
-00000010: 6d70 6f72 7420 6d61 7468 0d0a 0d0a 6672  mport math....fr
-00000020: 6f6d 2073 7273 6775 6920 696d 706f 7274  om srsgui import
-00000030: 2043 6f6d 706f 6e65 6e74 0d0a 6672 6f6d   Component..from
-00000040: 2073 7273 6775 692e 696e 7374 2069 6d70   srsgui.inst imp
-00000050: 6f72 7420 436f 6d6d 616e 642c 2049 6e64  ort Command, Ind
-00000060: 6578 436f 6d6d 616e 642c 205c 0d0a 2020  exCommand, \..  
-00000070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000080: 2020 2020 2020 466c 6f61 7443 6f6d 6d61        FloatComma
-00000090: 6e64 2c20 466c 6f61 7449 6e64 6578 436f  nd, FloatIndexCo
-000000a0: 6d6d 616e 640d 0a0d 0a0d 0a63 6c61 7373  mmand......class
-000000b0: 2049 6e64 6578 3a0d 0a20 2020 2070 6173   Index:..    pas
-000000c0: 730d 0a0d 0a0d 0a63 6c61 7373 2043 6f6d  s......class Com
-000000d0: 6d61 6e64 4974 656d 3a0d 0a20 2020 2022  mandItem:..    "
-000000e0: 2222 4120 436f 6d6d 616e 6420 6974 656d  ""A Command item
-000000f0: 2063 6f72 7265 7370 6f6e 6469 6e67 2074   corresponding t
-00000100: 6f20 6120 6c69 6e65 2069 6e20 5154 7265  o a line in QTre
-00000110: 6556 6965 7722 2222 0d0a 0d0a 2020 2020  eView"""....    
-00000120: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00000130: 662c 2070 6172 656e 743a 2022 436f 6d6d  f, parent: "Comm
-00000140: 616e 6449 7465 6d22 203d 204e 6f6e 6529  andItem" = None)
-00000150: 3a0d 0a20 2020 2020 2020 2073 656c 662e  :..        self.
-00000160: 5f70 6172 656e 7420 3d20 7061 7265 6e74  _parent = parent
-00000170: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-00000180: 6368 696c 6472 656e 203d 205b 5d0d 0a20  children = [].. 
-00000190: 2020 2020 2020 2073 656c 662e 5f76 616c         self._val
-000001a0: 7565 203d 204e 6f6e 650d 0a20 2020 2020  ue = None..     
-000001b0: 2020 200d 0a20 2020 2020 2020 2073 656c     ..        sel
-000001c0: 662e 6e61 6d65 203d 2022 220d 0a20 2020  f.name = ""..   
-000001d0: 2020 2020 2073 656c 662e 7661 6c75 655f       self.value_
-000001e0: 7479 7065 203d 204e 6f6e 6520 2023 2054  type = None  # T
-000001f0: 6865 7265 2061 7265 2033 2074 7970 6573  here are 3 types
-00000200: 206f 6620 7661 6c75 6573 3a20 7374 722c   of values: str,
-00000210: 2069 6e74 2c20 616e 6420 666c 6f61 740d   int, and float.
-00000220: 0a0d 0a20 2020 2020 2020 2073 656c 662e  ...        self.
-00000230: 636f 6d70 203d 204e 6f6e 650d 0a20 2020  comp = None..   
-00000240: 2020 2020 2073 656c 662e 636f 6d70 5f74       self.comp_t
-00000250: 7970 6520 3d20 4e6f 6e65 2020 2023 2054  ype = None   # T
-00000260: 6865 7265 2061 7265 2035 2074 7970 6573  here are 5 types
-00000270: 206f 6620 636f 6d70 6f6e 656e 7473 3a20   of components: 
-00000280: 436f 6d70 6f6e 656e 742c 2043 6f6d 6d61  Component, Comma
-00000290: 6e64 732c 2049 6e64 6578 436f 6d6d 616e  nds, IndexComman
-000002a0: 6473 2c20 6d65 7468 6f64 2061 6e64 2049  ds, method and I
-000002b0: 6e64 6578 0d0a 2020 2020 2020 2020 7365  ndex..        se
-000002c0: 6c66 2e73 6574 5f65 6e61 626c 6520 3d20  lf.set_enable = 
-000002d0: 4661 6c73 650d 0a20 2020 2020 2020 2073  False..        s
-000002e0: 656c 662e 6765 745f 656e 6162 6c65 203d  elf.get_enable =
-000002f0: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
-00000300: 7365 6c66 2e69 735f 6d65 7468 6f64 203d  self.is_method =
-00000310: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
-00000320: 7365 6c66 2e65 7863 6c75 6465 6420 3d20  self.excluded = 
-00000330: 4661 6c73 650d 0a20 2020 2020 2020 2073  False..        s
-00000340: 656c 662e 7261 775f 7265 6d6f 7465 5f63  elf.raw_remote_c
-00000350: 6f6d 6d61 6e64 203d 2022 220d 0a20 2020  ommand = ""..   
-00000360: 2020 2020 2073 656c 662e 7469 6d65 7374       self.timest
-00000370: 616d 7020 3d20 302e 300d 0a20 2020 2020  amp = 0.0..     
-00000380: 2020 2073 656c 662e 7175 6572 795f 7570     self.query_up
-00000390: 6461 7465 5f70 6572 696f 6420 3d20 302e  date_period = 0.
-000003a0: 330d 0a0d 0a20 2020 2064 6566 2061 7070  3....    def app
-000003b0: 656e 6443 6869 6c64 2873 656c 662c 2069  endChild(self, i
-000003c0: 7465 6d3a 2022 436f 6d6d 616e 6449 7465  tem: "CommandIte
-000003d0: 6d22 293a 0d0a 2020 2020 2020 2020 2222  m"):..        ""
-000003e0: 2241 6464 2069 7465 6d20 6173 2061 2063  "Add item as a c
-000003f0: 6869 6c64 2222 220d 0a20 2020 2020 2020  hild"""..       
-00000400: 2073 656c 662e 5f63 6869 6c64 7265 6e2e   self._children.
-00000410: 6170 7065 6e64 2869 7465 6d29 0d0a 0d0a  append(item)....
-00000420: 2020 2020 6465 6620 6368 696c 6428 7365      def child(se
-00000430: 6c66 2c20 726f 773a 2069 6e74 2920 2d3e  lf, row: int) ->
-00000440: 2022 436f 6d6d 616e 6449 7465 6d22 3a0d   "CommandItem":.
-00000450: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
-00000460: 726e 2074 6865 2063 6869 6c64 206f 6620  rn the child of 
-00000470: 7468 6520 6375 7272 656e 7420 6974 656d  the current item
-00000480: 2066 726f 6d20 7468 6520 6769 7665 6e20   from the given 
-00000490: 726f 7722 2222 0d0a 2020 2020 2020 2020  row"""..        
-000004a0: 7265 7475 726e 2073 656c 662e 5f63 6869  return self._chi
-000004b0: 6c64 7265 6e5b 726f 775d 0d0a 0d0a 2020  ldren[row]....  
-000004c0: 2020 6465 6620 7061 7265 6e74 2873 656c    def parent(sel
-000004d0: 6629 202d 3e20 2243 6f6d 6d61 6e64 4974  f) -> "CommandIt
-000004e0: 656d 223a 0d0a 2020 2020 2020 2020 2222  em":..        ""
-000004f0: 2252 6574 7572 6e20 7468 6520 7061 7265  "Return the pare
-00000500: 6e74 206f 6620 7468 6520 6375 7272 656e  nt of the curren
-00000510: 7420 6974 656d 2222 220d 0a20 2020 2020  t item"""..     
-00000520: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-00000530: 7061 7265 6e74 0d0a 0d0a 2020 2020 6465  parent....    de
-00000540: 6620 6368 696c 6443 6f75 6e74 2873 656c  f childCount(sel
-00000550: 6629 202d 3e20 696e 743a 0d0a 2020 2020  f) -> int:..    
-00000560: 2020 2020 2222 2252 6574 7572 6e20 7468      """Return th
-00000570: 6520 6e75 6d62 6572 206f 6620 6368 696c  e number of chil
-00000580: 6472 656e 206f 6620 7468 6520 6375 7272  dren of the curr
-00000590: 656e 7420 6974 656d 2222 220d 0a20 2020  ent item"""..   
-000005a0: 2020 2020 2072 6574 7572 6e20 6c65 6e28       return len(
-000005b0: 7365 6c66 2e5f 6368 696c 6472 656e 290d  self._children).
-000005c0: 0a0d 0a20 2020 2064 6566 2072 6f77 2873  ...    def row(s
-000005d0: 656c 6629 202d 3e20 696e 743a 0d0a 2020  elf) -> int:..  
-000005e0: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
-000005f0: 7468 6520 726f 7720 7768 6572 6520 7468  the row where th
-00000600: 6520 6375 7272 656e 7420 6974 656d 206f  e current item o
-00000610: 6363 7570 6965 7320 696e 2074 6865 2070  ccupies in the p
-00000620: 6172 656e 7422 2222 0d0a 2020 2020 2020  arent"""..      
-00000630: 2020 7265 7475 726e 2073 656c 662e 5f70    return self._p
-00000640: 6172 656e 742e 5f63 6869 6c64 7265 6e2e  arent._children.
-00000650: 696e 6465 7828 7365 6c66 2920 6966 2073  index(self) if s
-00000660: 656c 662e 5f70 6172 656e 7420 656c 7365  elf._parent else
-00000670: 2030 0d0a 0d0a 2020 2020 4070 726f 7065   0....    @prope
-00000680: 7274 790d 0a20 2020 2064 6566 2076 616c  rty..    def val
-00000690: 7565 2873 656c 6629 3a0d 0a20 2020 2020  ue(self):..     
-000006a0: 2020 2022 2222 5265 7475 726e 2074 6865     """Return the
-000006b0: 2076 616c 7565 206f 6620 7468 6520 6375   value of the cu
-000006c0: 7272 656e 7420 6974 656d 2222 220d 0a20  rrent item""".. 
-000006d0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-000006e0: 6c66 2e5f 7661 6c75 650d 0a0d 0a20 2020  lf._value....   
-000006f0: 2040 7661 6c75 652e 7365 7474 6572 0d0a   @value.setter..
-00000700: 2020 2020 6465 6620 7661 6c75 6528 7365      def value(se
-00000710: 6c66 2c20 7661 6c75 6529 3a0d 0a20 2020  lf, value):..   
-00000720: 2020 2020 2073 656c 662e 5f76 616c 7565       self._value
-00000730: 203d 2076 616c 7565 0d0a 0d0a 2020 2020   = value....    
-00000740: 6465 6620 7175 6572 795f 7661 6c75 6528  def query_value(
-00000750: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-00000760: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
-00000770: 2020 7473 203d 2074 696d 652e 7469 6d65    ts = time.time
-00000780: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00000790: 6966 2074 7320 2d20 7365 6c66 2e74 696d  if ts - self.tim
-000007a0: 6573 7461 6d70 203c 2073 656c 662e 7175  estamp < self.qu
-000007b0: 6572 795f 7570 6461 7465 5f70 6572 696f  ery_update_perio
-000007c0: 643a 2020 2320 446f 6e27 7420 7570 6461  d:  # Don't upda
-000007d0: 7465 2074 6f6f 206f 6674 656e 0d0a 2020  te too often..  
-000007e0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000007f0: 7475 726e 2073 656c 662e 5f76 616c 7565  turn self._value
-00000800: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00000810: 6966 2073 656c 662e 636f 6d70 5f74 7970  if self.comp_typ
-00000820: 6520 3d3d 2049 6e64 6578 2061 6e64 2073  e == Index and s
-00000830: 656c 662e 6765 745f 656e 6162 6c65 2061  elf.get_enable a
-00000840: 6e64 206e 6f74 2073 656c 662e 6578 636c  nd not self.excl
-00000850: 7564 6564 3a0d 0a20 2020 2020 2020 2020  uded:..         
-00000860: 2020 2020 2020 2073 656c 662e 5f76 616c         self._val
-00000870: 7565 203d 2073 656c 662e 5f70 6172 656e  ue = self._paren
-00000880: 742e 636f 6d70 2e5f 5f67 6574 6974 656d  t.comp.__getitem
-00000890: 5f5f 2873 656c 662e 636f 6d70 290d 0a20  __(self.comp).. 
-000008a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000008b0: 656c 662e 7661 6c75 655f 7479 7065 203d  elf.value_type =
-000008c0: 2074 7970 6528 7365 6c66 2e5f 7661 6c75   type(self._valu
-000008d0: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
-000008e0: 2020 2020 7365 6c66 2e74 696d 6573 7461      self.timesta
-000008f0: 6d70 203d 2074 730d 0a20 2020 2020 2020  mp = ts..       
-00000900: 2020 2020 2065 6c69 6620 6973 7375 6263       elif issubc
-00000910: 6c61 7373 2874 7970 6528 7365 6c66 2e63  lass(type(self.c
-00000920: 6f6d 7029 2c20 436f 6d6d 616e 6429 2061  omp), Command) a
-00000930: 6e64 2073 656c 662e 6765 745f 656e 6162  nd self.get_enab
-00000940: 6c65 2061 6e64 206e 6f74 2073 656c 662e  le and not self.
-00000950: 6578 636c 7564 6564 3a0d 0a20 2020 2020  excluded:..     
-00000960: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00000970: 5f76 616c 7565 203d 2073 656c 662e 636f  _value = self.co
-00000980: 6d70 2e5f 5f67 6574 5f5f 2873 656c 662e  mp.__get__(self.
-00000990: 5f70 6172 656e 742e 636f 6d70 2c20 7365  _parent.comp, se
-000009a0: 6c66 2e5f 7061 7265 6e74 2e63 6f6d 702e  lf._parent.comp.
-000009b0: 5f5f 636c 6173 735f 5f29 0d0a 2020 2020  __class__)..    
-000009c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000009d0: 2e76 616c 7565 5f74 7970 6520 3d20 7479  .value_type = ty
-000009e0: 7065 2873 656c 662e 5f76 616c 7565 290d  pe(self._value).
-000009f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000a00: 2073 656c 662e 7469 6d65 7374 616d 7020   self.timestamp 
-00000a10: 3d20 7473 0d0a 2020 2020 2020 2020 6578  = ts..        ex
-00000a20: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
-00000a30: 7320 653a 0d0a 2020 2020 2020 2020 2020  s e:..          
-00000a40: 2020 7072 696e 7428 2751 7565 7279 2065    print('Query e
-00000a50: 7272 6f72 3a20 7b7d 207b 7d27 2e66 6f72  rror: {} {}'.for
-00000a60: 6d61 7428 652c 2073 656c 662e 6e61 6d65  mat(e, self.name
-00000a70: 2929 0d0a 2020 2020 2020 2020 6669 6e61  ))..        fina
-00000a80: 6c6c 793a 0d0a 2020 2020 2020 2020 2020  lly:..          
-00000a90: 2020 7265 7475 726e 2073 656c 662e 5f76    return self._v
-00000aa0: 616c 7565 0d0a 0d0a 2020 2020 6465 6620  alue....    def 
-00000ab0: 7365 745f 7661 6c75 6528 7365 6c66 2c20  set_value(self, 
-00000ac0: 7661 6c75 6529 3a0d 0a20 2020 2020 2020  value):..       
-00000ad0: 2022 2222 5365 7420 7661 6c75 6520 746f   """Set value to
-00000ae0: 2074 6865 2069 6e73 7472 756d 656e 7420   the instrument 
-00000af0: 616e 6420 7570 6461 7465 2074 6865 2076  and update the v
-00000b00: 616c 7565 206f 6620 7468 6520 6974 656d  alue of the item
-00000b10: 2222 220d 0a20 2020 2020 2020 2074 7279  """..        try
-00000b20: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-00000b30: 6620 7365 6c66 2e63 6f6d 705f 7479 7065  f self.comp_type
-00000b40: 203d 3d20 496e 6465 783a 0d0a 2020 2020   == Index:..    
-00000b50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00000b60: 2e5f 7061 7265 6e74 2e63 6f6d 702e 5f5f  ._parent.comp.__
-00000b70: 7365 7469 7465 6d5f 5f28 7365 6c66 2e63  setitem__(self.c
-00000b80: 6f6d 702c 2076 616c 7565 290d 0a20 2020  omp, value)..   
-00000b90: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00000ba0: 662e 5f76 616c 7565 203d 2073 656c 662e  f._value = self.
-00000bb0: 5f70 6172 656e 742e 636f 6d70 2e5f 5f67  _parent.comp.__g
-00000bc0: 6574 6974 656d 5f5f 2873 656c 662e 636f  etitem__(self.co
-00000bd0: 6d70 290d 0a20 2020 2020 2020 2020 2020  mp)..           
-00000be0: 2020 2020 2073 656c 662e 7469 6d65 7374       self.timest
-00000bf0: 616d 7020 3d20 7469 6d65 2e74 696d 6528  amp = time.time(
-00000c00: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
-00000c10: 6c69 6620 6973 7375 6263 6c61 7373 2874  lif issubclass(t
-00000c20: 7970 6528 7365 6c66 2e63 6f6d 7029 2c20  ype(self.comp), 
-00000c30: 436f 6d6d 616e 6429 3a0d 0a20 2020 2020  Command):..     
-00000c40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00000c50: 636f 6d70 2e5f 5f73 6574 5f5f 2873 656c  comp.__set__(sel
-00000c60: 662e 5f70 6172 656e 742e 636f 6d70 2c20  f._parent.comp, 
-00000c70: 7661 6c75 6529 0d0a 2020 2020 2020 2020  value)..        
-00000c80: 2020 2020 2020 2020 7365 6c66 2e5f 7661          self._va
-00000c90: 6c75 6520 3d20 7365 6c66 2e63 6f6d 702e  lue = self.comp.
-00000ca0: 5f5f 6765 745f 5f28 7365 6c66 2e5f 7061  __get__(self._pa
-00000cb0: 7265 6e74 2e63 6f6d 702c 2073 656c 662e  rent.comp, self.
-00000cc0: 5f70 6172 656e 742e 636f 6d70 2e5f 5f63  _parent.comp.__c
-00000cd0: 6c61 7373 5f5f 290d 0a20 2020 2020 2020  lass__)..       
-00000ce0: 2020 2020 2020 2020 2073 656c 662e 7469           self.ti
-00000cf0: 6d65 7374 616d 7020 3d20 7469 6d65 2e74  mestamp = time.t
-00000d00: 696d 6528 290d 0a20 2020 2020 2020 2020  ime()..         
-00000d10: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00000d20: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00000d30: 7661 6c75 6520 3d20 7661 6c75 650d 0a20  value = value.. 
-00000d40: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
-00000d50: 6365 7074 696f 6e20 6173 2065 3a0d 0a20  ception as e:.. 
-00000d60: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00000d70: 2827 5365 7420 6572 726f 723a 207b 7d20  ('Set error: {} 
-00000d80: 7b7d 272e 666f 726d 6174 2865 2c20 7365  {}'.format(e, se
-00000d90: 6c66 2e6e 616d 6529 290d 0a0d 0a20 2020  lf.name))....   
-00000da0: 2064 6566 2069 735f 6564 6974 6162 6c65   def is_editable
-00000db0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-00000dc0: 2022 2222 5265 7475 726e 2054 7275 6520   """Return True 
-00000dd0: 6966 2074 6865 2069 7465 6d20 6973 2065  if the item is e
-00000de0: 6469 7461 626c 6522 2222 0d0a 2020 2020  ditable"""..    
-00000df0: 2020 2020 6966 2073 656c 662e 636f 6d70      if self.comp
-00000e00: 5f74 7970 6520 3d3d 2049 6e64 6578 2061  _type == Index a
-00000e10: 6e64 205c 0d0a 2020 2020 2020 2020 2020  nd \..          
-00000e20: 2020 2020 2020 7365 6c66 2e73 6574 5f65        self.set_e
-00000e30: 6e61 626c 6520 616e 6420 7365 6c66 2e67  nable and self.g
-00000e40: 6574 5f65 6e61 626c 6520 616e 6420 6e6f  et_enable and no
-00000e50: 7420 7365 6c66 2e65 7863 6c75 6465 643a  t self.excluded:
-00000e60: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00000e70: 7475 726e 2054 7275 650d 0a20 2020 2020  turn True..     
-00000e80: 2020 2065 6c69 6620 6973 7375 6263 6c61     elif issubcla
-00000e90: 7373 2874 7970 6528 7365 6c66 2e63 6f6d  ss(type(self.com
-00000ea0: 7029 2c20 436f 6d6d 616e 6429 2061 6e64  p), Command) and
-00000eb0: 205c 0d0a 2020 2020 2020 2020 2020 2020   \..            
-00000ec0: 2020 2020 7365 6c66 2e73 6574 5f65 6e61      self.set_ena
-00000ed0: 626c 6520 616e 6420 7365 6c66 2e67 6574  ble and self.get
-00000ee0: 5f65 6e61 626c 6520 616e 6420 6e6f 7420  _enable and not 
-00000ef0: 7365 6c66 2e65 7863 6c75 6465 643a 0d0a  self.excluded:..
-00000f00: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00000f10: 726e 2054 7275 650d 0a20 2020 2020 2020  rn True..       
-00000f20: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00000f30: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-00000f40: 0d0a 0d0a 2020 2020 6465 6620 6765 745f  ....    def get_
-00000f50: 666f 726d 6174 7465 645f 7661 6c75 6528  formatted_value(
-00000f60: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-00000f70: 2222 2252 6574 7572 6e20 666f 726d 6174  """Return format
-00000f80: 7465 6420 7661 6c75 6520 6f66 2061 2066  ted value of a f
-00000f90: 6c6f 6174 2222 220d 0a0d 0a20 2020 2020  loat"""....     
-00000fa0: 2020 2076 616c 7565 203d 2073 656c 662e     value = self.
-00000fb0: 7661 6c75 650d 0a20 2020 2020 2020 2069  value..        i
-00000fc0: 6620 7661 6c75 6520 6973 204e 6f6e 653a  f value is None:
-00000fd0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00000fe0: 7475 726e 204e 6f6e 650d 0a0d 0a20 2020  turn None....   
-00000ff0: 2020 2020 2063 6f6d 7020 3d20 4e6f 6e65       comp = None
-00001000: 0d0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
-00001010: 662e 636f 6d70 5f74 7970 6520 3d3d 2049  f.comp_type == I
-00001020: 6e64 6578 3a0d 0a20 2020 2020 2020 2020  ndex:..         
-00001030: 2020 2063 6f6d 7020 3d20 7365 6c66 2e70     comp = self.p
-00001040: 6172 656e 7428 292e 636f 6d70 0d0a 2020  arent().comp..  
-00001050: 2020 2020 2020 656c 6966 2069 7373 7562        elif issub
-00001060: 636c 6173 7328 7479 7065 2873 656c 662e  class(type(self.
-00001070: 636f 6d70 292c 2043 6f6d 6d61 6e64 2920  comp), Command) 
-00001080: 6f72 205c 0d0a 2020 2020 2020 2020 2020  or \..          
-00001090: 2020 2069 7373 7562 636c 6173 7328 7479     issubclass(ty
-000010a0: 7065 2873 656c 662e 636f 6d70 292c 2049  pe(self.comp), I
-000010b0: 6e64 6578 436f 6d6d 616e 6429 3a0d 0a20  ndexCommand):.. 
-000010c0: 2020 2020 2020 2020 2020 2063 6f6d 7020             comp 
-000010d0: 3d20 7365 6c66 2e63 6f6d 700d 0a0d 0a20  = self.comp.... 
-000010e0: 2020 2020 2020 2066 6d74 203d 2063 6f6d         fmt = com
-000010f0: 702e 666d 7420 6966 2063 6f6d 7020 616e  p.fmt if comp an
-00001100: 6420 6861 7361 7474 7228 636f 6d70 2c20  d hasattr(comp, 
-00001110: 2766 6d74 2729 2065 6c73 6520 2727 0d0a  'fmt') else ''..
-00001120: 2020 2020 2020 2020 756e 6974 203d 2063          unit = c
-00001130: 6f6d 702e 756e 6974 2069 6620 636f 6d70  omp.unit if comp
-00001140: 2061 6e64 2068 6173 6174 7472 2863 6f6d   and hasattr(com
-00001150: 702c 2027 756e 6974 2729 2065 6c73 6520  p, 'unit') else 
-00001160: 2727 0d0a 0d0a 2020 2020 2020 2020 6966  ''....        if
-00001170: 2063 6f6d 7020 616e 6420 2869 7373 7562   comp and (issub
-00001180: 636c 6173 7328 7479 7065 2863 6f6d 7029  class(type(comp)
-00001190: 2c20 466c 6f61 7449 6e64 6578 436f 6d6d  , FloatIndexComm
-000011a0: 616e 6429 206f 720d 0a20 2020 2020 2020  and) or..       
-000011b0: 2020 2020 2020 2020 2020 2020 2020 6973                is
-000011c0: 7375 6263 6c61 7373 2874 7970 6528 636f  subclass(type(co
-000011d0: 6d70 292c 2046 6c6f 6174 436f 6d6d 616e  mp), FloatComman
-000011e0: 6429 293a 0d0a 2020 2020 2020 2020 2020  d)):..          
-000011f0: 2020 6966 2076 616c 7565 203d 3d20 302e    if value == 0.
-00001200: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
-00001210: 2020 2020 7265 7475 726e 2027 3027 202b      return '0' +
-00001220: 2066 2720 7b75 6e69 747d 270d 0a20 2020   f' {unit}'..   
-00001230: 2020 2020 2020 2020 2073 7465 7020 3d20           step = 
-00001240: 636f 6d70 2e73 7465 700d 0a20 2020 2020  comp.step..     
-00001250: 2020 2020 2020 2073 6967 6e69 6669 6361         significa
-00001260: 6e74 5f66 6967 7572 6573 203d 2063 6f6d  nt_figures = com
-00001270: 702e 7369 676e 6966 6963 616e 745f 6669  p.significant_fi
-00001280: 6775 7265 730d 0a0d 0a20 2020 2020 2020  gures....       
-00001290: 2020 2020 2064 6563 696d 616c 7320 3d20       decimals = 
-000012a0: 6d61 7468 2e63 6569 6c28 2d6d 6174 682e  math.ceil(-math.
-000012b0: 6c6f 6731 3028 7374 6570 2929 0d0a 2020  log10(step))..  
-000012c0: 2020 2020 2020 2020 2020 6469 6769 7473            digits
-000012d0: 203d 206d 6174 682e 6365 696c 286d 6174   = math.ceil(mat
-000012e0: 682e 6c6f 6731 3028 6162 7328 7661 6c75  h.log10(abs(valu
-000012f0: 6529 2929 2069 6620 7661 6c75 6520 656c  e))) if value el
-00001300: 7365 2030 0d0a 2020 2020 2020 2020 2020  se 0..          
-00001310: 2020 7072 6563 6973 696f 6e20 3d20 6d69    precision = mi
-00001320: 6e28 6465 6369 6d61 6c73 2c20 7369 676e  n(decimals, sign
-00001330: 6966 6963 616e 745f 6669 6775 7265 7320  ificant_figures 
-00001340: 2d20 6469 6769 7473 290d 0a20 2020 2020  - digits)..     
-00001350: 2020 2020 2020 2070 7265 6369 7369 6f6e         precision
-00001360: 203d 206d 6178 2870 7265 6369 7369 6f6e   = max(precision
-00001370: 2c20 3029 0d0a 2020 2020 2020 2020 2020  , 0)..          
-00001380: 2020 6966 2061 6273 2876 616c 7565 2920    if abs(value) 
-00001390: 3e3d 2030 2e31 206f 7220 7072 6563 6973  >= 0.1 or precis
-000013a0: 696f 6e20 3c20 7369 676e 6966 6963 616e  ion < significan
-000013b0: 745f 6669 6775 7265 733a 0d0a 2020 2020  t_figures:..    
-000013c0: 2020 2020 2020 2020 2020 2020 2320 5265              # Re
-000013d0: 6d6f 7665 2074 7261 696c 696e 6720 7a65  move trailing ze
-000013e0: 726f 7320 616e 6420 7265 7475 726e 0d0a  ros and return..
-000013f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001400: 7320 3d20 6627 7b76 616c 7565 3a2e 7b70  s = f'{value:.{p
-00001410: 7265 6369 7369 6f6e 7d66 7d27 0d0a 2020  recision}f}'..  
-00001420: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00001430: 2027 2e27 2069 6e20 733a 0d0a 2020 2020   '.' in s:..    
-00001440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001450: 7265 7475 726e 2073 2e72 7374 7269 7028  return s.rstrip(
-00001460: 2730 2729 2e72 7374 7269 7028 272e 2729  '0').rstrip('.')
-00001470: 202b 2066 2720 7b75 6e69 747d 270d 0a20   + f' {unit}'.. 
-00001480: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00001490: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-000014a0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000014b0: 2073 202b 2066 2720 7b75 6e69 747d 270d   s + f' {unit}'.
-000014c0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-000014d0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000014e0: 2020 2020 7620 3d20 6627 7b76 616c 7565      v = f'{value
-000014f0: 3a2e 7b73 6967 6e69 6669 6361 6e74 5f66  :.{significant_f
-00001500: 6967 7572 6573 7d65 7d27 0d0a 2020 2020  igures}e}'..    
-00001510: 2020 2020 2020 2020 2020 2020 2320 5265              # Re
-00001520: 6d6f 7665 2074 7261 696c 696e 6720 7a65  move trailing ze
-00001530: 726f 7320 6265 666f 7265 2027 6527 2061  ros before 'e' a
-00001540: 6e64 2072 6574 7572 6e0d 0a20 2020 2020  nd return..     
-00001550: 2020 2020 2020 2020 2020 2074 203d 2076             t = v
-00001560: 2e73 706c 6974 2827 6527 290d 0a20 2020  .split('e')..   
-00001570: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00001580: 7572 6e20 6627 7b74 5b30 5d2e 7273 7472  urn f'{t[0].rstr
-00001590: 6970 2822 3022 292e 7273 7472 6970 2822  ip("0").rstrip("
-000015a0: 2e22 297d 657b 745b 315d 7d27 202b 2066  .")}e{t[1]}' + f
-000015b0: 2720 207b 756e 6974 7d27 0d0a 2020 2020  '  {unit}'..    
-000015c0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-000015d0: 2020 2020 2020 2072 6574 7572 6e20 6627         return f'
-000015e0: 7b76 616c 7565 3a7b 666d 747d 7d27 202b  {value:{fmt}}' +
-000015f0: 2066 2720 7b75 6e69 747d 270d 0a0d 0a20   f' {unit}'.... 
-00001600: 2020 2064 6566 2063 6f6e 7374 7275 6374     def construct
-00001610: 5f73 6574 5f63 6f6d 6d61 6e64 5f73 7472  _set_command_str
-00001620: 696e 6728 7365 6c66 2c20 7661 6c75 6529  ing(self, value)
-00001630: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
-00001640: 2020 2020 2020 2020 436f 6e73 7472 7563          Construc
-00001650: 7420 7079 7468 6f6e 2063 6f6d 6d61 6e64  t python command
-00001660: 2073 7472 696e 6720 636f 7272 6573 706f   string correspo
-00001670: 6e64 696e 6720 746f 2074 6865 2069 7465  nding to the ite
-00001680: 6d0d 0a20 2020 2020 2020 2022 2222 0d0a  m..        """..
-00001690: 2020 2020 2020 2020 7365 6c66 2e6e 616d          self.nam
-000016a0: 655f 6275 6666 6572 203d 205b 5d0d 0a20  e_buffer = [].. 
-000016b0: 2020 2020 2020 2073 656c 662e 6765 745f         self.get_
-000016c0: 6e61 6d65 5f73 7472 696e 6728 7365 6c66  name_string(self
-000016d0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-000016e0: 6e61 6d65 5f62 7566 6665 722e 7265 7665  name_buffer.reve
-000016f0: 7273 6528 290d 0a20 2020 2020 2020 2069  rse()..        i
-00001700: 6620 7479 7065 2876 616c 7565 2920 6973  f type(value) is
-00001710: 2073 7472 3a0d 0a20 2020 2020 2020 2020   str:..         
-00001720: 2020 2073 203d 2027 7b7d 203d 2022 7b7d     s = '{} = "{}
-00001730: 2227 2e66 6f72 6d61 7428 272e 272e 6a6f  "'.format('.'.jo
-00001740: 696e 2873 656c 662e 6e61 6d65 5f62 7566  in(self.name_buf
-00001750: 6665 7229 2c20 7661 6c75 6529 0d0a 2020  fer), value)..  
-00001760: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00001770: 2020 2020 2020 2020 2073 203d 2027 7b7d           s = '{}
-00001780: 203d 207b 7d27 2e66 6f72 6d61 7428 272e   = {}'.format('.
-00001790: 272e 6a6f 696e 2873 656c 662e 6e61 6d65  '.join(self.name
-000017a0: 5f62 7566 6665 7229 2c20 7661 6c75 6529  _buffer), value)
-000017b0: 0d0a 0d0a 2020 2020 2020 2020 7320 3d20  ....        s = 
-000017c0: 732e 7265 706c 6163 6528 272e 5b27 2c20  s.replace('.[', 
-000017d0: 275b 2729 0d0a 2020 2020 2020 2020 7265  '[')..        re
-000017e0: 7475 726e 2073 0d0a 0d0a 2020 2020 6465  turn s....    de
-000017f0: 6620 6765 745f 6e61 6d65 5f73 7472 696e  f get_name_strin
-00001800: 6728 7365 6c66 2c20 6974 656d 293a 0d0a  g(self, item):..
-00001810: 2020 2020 2020 2020 6966 2069 7465 6d2e          if item.
-00001820: 636f 6d70 5f74 7970 6520 3d3d 2049 6e64  comp_type == Ind
-00001830: 6578 3a0d 0a20 2020 2020 2020 2020 2020  ex:..           
-00001840: 2069 6620 7479 7065 2869 7465 6d2e 636f   if type(item.co
-00001850: 6d70 2920 6973 2073 7472 3a0d 0a20 2020  mp) is str:..   
-00001860: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00001870: 662e 6e61 6d65 5f62 7566 6665 722e 6170  f.name_buffer.ap
-00001880: 7065 6e64 2827 5b22 7b7d 225d 272e 666f  pend('["{}"]'.fo
-00001890: 726d 6174 2869 7465 6d2e 6e61 6d65 2929  rmat(item.name))
-000018a0: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-000018b0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-000018c0: 2020 2020 2073 656c 662e 6e61 6d65 5f62       self.name_b
-000018d0: 7566 6665 722e 6170 7065 6e64 2827 5b7b  uffer.append('[{
-000018e0: 7d5d 272e 666f 726d 6174 2869 7465 6d2e  }]'.format(item.
-000018f0: 6e61 6d65 2929 0d0a 2020 2020 2020 2020  name))..        
-00001900: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00001910: 2020 2073 656c 662e 6e61 6d65 5f62 7566     self.name_buf
-00001920: 6665 722e 6170 7065 6e64 2869 7465 6d2e  fer.append(item.
-00001930: 6e61 6d65 290d 0a20 2020 2020 2020 2069  name)..        i
-00001940: 6620 6974 656d 2e70 6172 656e 7428 293a  f item.parent():
-00001950: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00001960: 6c66 2e67 6574 5f6e 616d 655f 7374 7269  lf.get_name_stri
-00001970: 6e67 2869 7465 6d2e 7061 7265 6e74 2829  ng(item.parent()
-00001980: 290d 0a0d 0a20 2020 2040 636c 6173 736d  )....    @classm
-00001990: 6574 686f 640d 0a20 2020 2064 6566 206c  ethod..    def l
-000019a0: 6f61 6428 0d0a 2020 2020 2020 2020 636c  oad(..        cl
-000019b0: 732c 2063 6f6d 702c 2070 6172 656e 743a  s, comp, parent:
-000019c0: 2022 436f 6d6d 616e 6449 7465 6d22 203d   "CommandItem" =
-000019d0: 204e 6f6e 6529 202d 3e20 2243 6f6d 6d61   None) -> "Comma
-000019e0: 6e64 4974 656d 223a 0d0a 2020 2020 2020  ndItem":..      
-000019f0: 2020 2222 2243 7265 6174 6520 6120 2772    """Create a 'r
-00001a00: 6f6f 7427 2043 6f6d 6d61 6e64 4974 656d  oot' CommandItem
-00001a10: 2066 726f 6d20 6120 436f 6d70 6f6e 656e   from a Componen
-00001a20: 7420 616e 6420 0d0a 2020 2020 2020 2020  t and ..        
-00001a30: 706f 7075 6c61 7465 2069 7473 2073 7562  populate its sub
-00001a40: 636f 6d70 6f6e 656e 7420 616e 6420 636f  component and co
-00001a50: 6d6d 616e 6473 2072 6563 7572 7369 7665  mmands recursive
-00001a60: 6c79 2e0d 0a0d 0a20 2020 2020 2020 2052  ly.....        R
-00001a70: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
-00001a80: 2020 2020 2043 6f6d 6d61 6e64 4974 656d       CommandItem
-00001a90: 3a20 436f 6d6d 616e 6449 7465 6d0d 0a20  : CommandItem.. 
-00001aa0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00001ab0: 2020 2020 726f 6f74 5f69 7465 6d20 3d20      root_item = 
-00001ac0: 436f 6d6d 616e 6449 7465 6d28 7061 7265  CommandItem(pare
-00001ad0: 6e74 290d 0a20 2020 2020 2020 2072 6f6f  nt)..        roo
-00001ae0: 745f 6974 656d 2e6e 616d 6520 3d20 2272  t_item.name = "r
-00001af0: 6f6f 7422 0d0a 2020 2020 2020 2020 726f  oot"..        ro
-00001b00: 6f74 5f69 7465 6d2e 636f 6d70 203d 2063  ot_item.comp = c
-00001b10: 6f6d 700d 0a0d 0a20 2020 2020 2020 2069  omp....        i
-00001b20: 6620 6973 7375 6263 6c61 7373 2863 6f6d  f issubclass(com
-00001b30: 702e 5f5f 636c 6173 735f 5f2c 2043 6f6d  p.__class__, Com
-00001b40: 706f 6e65 6e74 293a 0d0a 2020 2020 2020  ponent):..      
-00001b50: 2020 2020 2020 726f 6f74 5f69 7465 6d2e        root_item.
-00001b60: 6e61 6d65 203d 2063 6f6d 702e 6765 745f  name = comp.get_
-00001b70: 6e61 6d65 2829 0d0a 2020 2020 2020 2020  name()..        
-00001b80: 2020 2020 666f 7220 6a20 696e 2063 6f6d      for j in com
-00001b90: 702e 5f5f 6469 6374 5f5f 3a0d 0a20 2020  p.__dict__:..   
-00001ba0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00001bb0: 6a20 3d3d 2027 5f70 6172 656e 7427 3a0d  j == '_parent':.
-00001bc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001bd0: 2020 2020 2063 6f6e 7469 6e75 650d 0a20       continue.. 
-00001be0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00001bf0: 6e73 7461 6e63 6520 3d20 636f 6d70 2e5f  nstance = comp._
-00001c00: 5f64 6963 745f 5f5b 6a5d 0d0a 2020 2020  _dict__[j]..    
-00001c10: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00001c20: 7373 7562 636c 6173 7328 696e 7374 616e  ssubclass(instan
-00001c30: 6365 2e5f 5f63 6c61 7373 5f5f 2c20 2043  ce.__class__,  C
-00001c40: 6f6d 706f 6e65 6e74 293a 2020 2020 2020  omponent):      
-00001c50: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00000000: 0d0a 696d 706f 7274 2074 696d 650d 0a66  ..import time..f
+00000010: 726f 6d20 7372 7367 7569 2069 6d70 6f72  rom srsgui impor
+00000020: 7420 436f 6d70 6f6e 656e 740d 0a66 726f  t Component..fro
+00000030: 6d20 7372 7367 7569 2e69 6e73 7420 696d  m srsgui.inst im
+00000040: 706f 7274 2043 6f6d 6d61 6e64 2c20 496e  port Command, In
+00000050: 6465 7843 6f6d 6d61 6e64 2c20 5c0d 0a20  dexCommand, \.. 
+00000060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000070: 2020 2020 2020 2046 6c6f 6174 436f 6d6d         FloatComm
+00000080: 616e 642c 2046 6c6f 6174 496e 6465 7843  and, FloatIndexC
+00000090: 6f6d 6d61 6e64 0d0a 0d0a 0d0a 636c 6173  ommand......clas
+000000a0: 7320 496e 6465 783a 0d0a 2020 2020 7061  s Index:..    pa
+000000b0: 7373 0d0a 0d0a 0d0a 636c 6173 7320 436f  ss......class Co
+000000c0: 6d6d 616e 6449 7465 6d3a 0d0a 2020 2020  mmandItem:..    
+000000d0: 2222 2241 2043 6f6d 6d61 6e64 2069 7465  """A Command ite
+000000e0: 6d20 636f 7272 6573 706f 6e64 696e 6720  m corresponding 
+000000f0: 746f 2061 206c 696e 6520 696e 2051 5472  to a line in QTr
+00000100: 6565 5669 6577 2222 220d 0a0d 0a20 2020  eeView"""....   
+00000110: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+00000120: 6c66 2c20 7061 7265 6e74 3a20 2243 6f6d  lf, parent: "Com
+00000130: 6d61 6e64 4974 656d 2220 3d20 4e6f 6e65  mandItem" = None
+00000140: 293a 0d0a 2020 2020 2020 2020 7365 6c66  ):..        self
+00000150: 2e5f 7061 7265 6e74 203d 2070 6172 656e  ._parent = paren
+00000160: 740d 0a20 2020 2020 2020 2073 656c 662e  t..        self.
+00000170: 5f63 6869 6c64 7265 6e20 3d20 5b5d 0d0a  _children = []..
+00000180: 2020 2020 2020 2020 7365 6c66 2e5f 7661          self._va
+00000190: 6c75 6520 3d20 4e6f 6e65 0d0a 2020 2020  lue = None..    
+000001a0: 2020 2020 0d0a 2020 2020 2020 2020 7365      ..        se
+000001b0: 6c66 2e6e 616d 6520 3d20 2222 0d0a 2020  lf.name = ""..  
+000001c0: 2020 2020 2020 7365 6c66 2e76 616c 7565        self.value
+000001d0: 5f74 7970 6520 3d20 4e6f 6e65 2020 2320  _type = None  # 
+000001e0: 5468 6572 6520 6172 6520 3320 7479 7065  There are 3 type
+000001f0: 7320 6f66 2076 616c 7565 733a 2073 7472  s of values: str
+00000200: 2c20 696e 742c 2061 6e64 2066 6c6f 6174  , int, and float
+00000210: 0d0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
+00000220: 7265 6369 7369 6f6e 203d 2034 0d0a 2020  recision = 4..  
+00000230: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00000240: 7365 6c66 2e63 6f6d 7020 3d20 4e6f 6e65  self.comp = None
+00000250: 0d0a 2020 2020 2020 2020 7365 6c66 2e63  ..        self.c
+00000260: 6f6d 705f 7479 7065 203d 204e 6f6e 6520  omp_type = None 
+00000270: 2020 2320 5468 6572 6520 6172 6520 3520    # There are 5 
+00000280: 7479 7065 7320 6f66 2063 6f6d 706f 6e65  types of compone
+00000290: 6e74 733a 2043 6f6d 706f 6e65 6e74 2c20  nts: Component, 
+000002a0: 436f 6d6d 616e 6473 2c20 496e 6465 7843  Commands, IndexC
+000002b0: 6f6d 6d61 6e64 732c 206d 6574 686f 6420  ommands, method 
+000002c0: 616e 6420 496e 6465 780d 0a20 2020 2020  and Index..     
+000002d0: 2020 2073 656c 662e 7365 745f 656e 6162     self.set_enab
+000002e0: 6c65 203d 2046 616c 7365 0d0a 2020 2020  le = False..    
+000002f0: 2020 2020 7365 6c66 2e67 6574 5f65 6e61      self.get_ena
+00000300: 626c 6520 3d20 4661 6c73 650d 0a20 2020  ble = False..   
+00000310: 2020 2020 2073 656c 662e 6973 5f6d 6574       self.is_met
+00000320: 686f 6420 3d20 4661 6c73 650d 0a20 2020  hod = False..   
+00000330: 2020 2020 2073 656c 662e 6578 636c 7564       self.exclud
+00000340: 6564 203d 2046 616c 7365 0d0a 2020 2020  ed = False..    
+00000350: 2020 2020 7365 6c66 2e72 6177 5f72 656d      self.raw_rem
+00000360: 6f74 655f 636f 6d6d 616e 6420 3d20 2222  ote_command = ""
+00000370: 0d0a 2020 2020 2020 2020 7365 6c66 2e74  ..        self.t
+00000380: 696d 6573 7461 6d70 203d 2030 2e30 0d0a  imestamp = 0.0..
+00000390: 0d0a 2020 2020 6465 6620 6170 7065 6e64  ..    def append
+000003a0: 4368 696c 6428 7365 6c66 2c20 6974 656d  Child(self, item
+000003b0: 3a20 2243 6f6d 6d61 6e64 4974 656d 2229  : "CommandItem")
+000003c0: 3a0d 0a20 2020 2020 2020 2022 2222 4164  :..        """Ad
+000003d0: 6420 6974 656d 2061 7320 6120 6368 696c  d item as a chil
+000003e0: 6422 2222 0d0a 2020 2020 2020 2020 7365  d"""..        se
+000003f0: 6c66 2e5f 6368 696c 6472 656e 2e61 7070  lf._children.app
+00000400: 656e 6428 6974 656d 290d 0a0d 0a20 2020  end(item)....   
+00000410: 2064 6566 2063 6869 6c64 2873 656c 662c   def child(self,
+00000420: 2072 6f77 3a20 696e 7429 202d 3e20 2243   row: int) -> "C
+00000430: 6f6d 6d61 6e64 4974 656d 223a 0d0a 2020  ommandItem":..  
+00000440: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
+00000450: 7468 6520 6368 696c 6420 6f66 2074 6865  the child of the
+00000460: 2063 7572 7265 6e74 2069 7465 6d20 6672   current item fr
+00000470: 6f6d 2074 6865 2067 6976 656e 2072 6f77  om the given row
+00000480: 2222 220d 0a20 2020 2020 2020 2072 6574  """..        ret
+00000490: 7572 6e20 7365 6c66 2e5f 6368 696c 6472  urn self._childr
+000004a0: 656e 5b72 6f77 5d0d 0a0d 0a20 2020 2064  en[row]....    d
+000004b0: 6566 2070 6172 656e 7428 7365 6c66 2920  ef parent(self) 
+000004c0: 2d3e 2022 436f 6d6d 616e 6449 7465 6d22  -> "CommandItem"
+000004d0: 3a0d 0a20 2020 2020 2020 2022 2222 5265  :..        """Re
+000004e0: 7475 726e 2074 6865 2070 6172 656e 7420  turn the parent 
+000004f0: 6f66 2074 6865 2063 7572 7265 6e74 2069  of the current i
+00000500: 7465 6d22 2222 0d0a 2020 2020 2020 2020  tem"""..        
+00000510: 7265 7475 726e 2073 656c 662e 5f70 6172  return self._par
+00000520: 656e 740d 0a0d 0a20 2020 2064 6566 2063  ent....    def c
+00000530: 6869 6c64 436f 756e 7428 7365 6c66 2920  hildCount(self) 
+00000540: 2d3e 2069 6e74 3a0d 0a20 2020 2020 2020  -> int:..       
+00000550: 2022 2222 5265 7475 726e 2074 6865 206e   """Return the n
+00000560: 756d 6265 7220 6f66 2063 6869 6c64 7265  umber of childre
+00000570: 6e20 6f66 2074 6865 2063 7572 7265 6e74  n of the current
+00000580: 2069 7465 6d22 2222 0d0a 2020 2020 2020   item"""..      
+00000590: 2020 7265 7475 726e 206c 656e 2873 656c    return len(sel
+000005a0: 662e 5f63 6869 6c64 7265 6e29 0d0a 0d0a  f._children)....
+000005b0: 2020 2020 6465 6620 726f 7728 7365 6c66      def row(self
+000005c0: 2920 2d3e 2069 6e74 3a0d 0a20 2020 2020  ) -> int:..     
+000005d0: 2020 2022 2222 5265 7475 726e 2074 6865     """Return the
+000005e0: 2072 6f77 2077 6865 7265 2074 6865 2063   row where the c
+000005f0: 7572 7265 6e74 2069 7465 6d20 6f63 6375  urrent item occu
+00000600: 7069 6573 2069 6e20 7468 6520 7061 7265  pies in the pare
+00000610: 6e74 2222 220d 0a20 2020 2020 2020 2072  nt"""..        r
+00000620: 6574 7572 6e20 7365 6c66 2e5f 7061 7265  eturn self._pare
+00000630: 6e74 2e5f 6368 696c 6472 656e 2e69 6e64  nt._children.ind
+00000640: 6578 2873 656c 6629 2069 6620 7365 6c66  ex(self) if self
+00000650: 2e5f 7061 7265 6e74 2065 6c73 6520 300d  ._parent else 0.
+00000660: 0a0d 0a20 2020 2040 7072 6f70 6572 7479  ...    @property
+00000670: 0d0a 2020 2020 6465 6620 7661 6c75 6528  ..    def value(
+00000680: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00000690: 2222 2252 6574 7572 6e20 7468 6520 7661  """Return the va
+000006a0: 6c75 6520 6f66 2074 6865 2063 7572 7265  lue of the curre
+000006b0: 6e74 2069 7465 6d22 2222 0d0a 2020 2020  nt item"""..    
+000006c0: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+000006d0: 2020 2020 2020 7473 203d 2074 696d 652e        ts = time.
+000006e0: 7469 6d65 2829 0d0a 2020 2020 2020 2020  time()..        
+000006f0: 2020 2020 6966 2074 7320 2d20 7365 6c66      if ts - self
+00000700: 2e74 696d 6573 7461 6d70 203c 2030 2e31  .timestamp < 0.1
+00000710: 3a20 2320 5570 6461 7465 2076 616c 7565  : # Update value
+00000720: 206c 6174 6572 2074 6861 6e20 302e 3120   later than 0.1 
+00000730: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
+00000740: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00000750: 7661 6c75 650d 0a0d 0a20 2020 2020 2020  value....       
+00000760: 2020 2020 2069 6620 7365 6c66 2e63 6f6d       if self.com
+00000770: 705f 7479 7065 203d 3d20 496e 6465 7820  p_type == Index 
+00000780: 616e 6420 7365 6c66 2e67 6574 5f65 6e61  and self.get_ena
+00000790: 626c 6520 616e 6420 6e6f 7420 7365 6c66  ble and not self
+000007a0: 2e65 7863 6c75 6465 643a 0d0a 2020 2020  .excluded:..    
+000007b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000007c0: 2e5f 7661 6c75 6520 3d20 7365 6c66 2e5f  ._value = self._
+000007d0: 7061 7265 6e74 2e63 6f6d 702e 5f5f 6765  parent.comp.__ge
+000007e0: 7469 7465 6d5f 5f28 7365 6c66 2e63 6f6d  titem__(self.com
+000007f0: 7029 0d0a 2020 2020 2020 2020 2020 2020  p)..            
+00000800: 2020 2020 7365 6c66 2e5f 7661 6c75 655f      self._value_
+00000810: 7479 7065 203d 2074 7970 6528 7365 6c66  type = type(self
+00000820: 2e5f 7661 6c75 6529 0d0a 2020 2020 2020  ._value)..      
+00000830: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+00000840: 696d 6573 7461 6d70 203d 2074 730d 0a20  imestamp = ts.. 
+00000850: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00000860: 6973 7375 6263 6c61 7373 2874 7970 6528  issubclass(type(
+00000870: 7365 6c66 2e63 6f6d 7029 2c20 436f 6d6d  self.comp), Comm
+00000880: 616e 6429 2061 6e64 2073 656c 662e 6765  and) and self.ge
+00000890: 745f 656e 6162 6c65 2061 6e64 206e 6f74  t_enable and not
+000008a0: 2073 656c 662e 6578 636c 7564 6564 3a0d   self.excluded:.
+000008b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000008c0: 2073 656c 662e 5f76 616c 7565 203d 2073   self._value = s
+000008d0: 656c 662e 636f 6d70 2e5f 5f67 6574 5f5f  elf.comp.__get__
+000008e0: 2873 656c 662e 5f70 6172 656e 742e 636f  (self._parent.co
+000008f0: 6d70 2c20 7365 6c66 2e5f 7061 7265 6e74  mp, self._parent
+00000900: 2e63 6f6d 702e 5f5f 636c 6173 735f 5f29  .comp.__class__)
+00000910: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000920: 2020 7365 6c66 2e5f 7661 6c75 655f 7479    self._value_ty
+00000930: 7065 203d 2074 7970 6528 7365 6c66 2e5f  pe = type(self._
+00000940: 7661 6c75 6529 0d0a 2020 2020 2020 2020  value)..        
+00000950: 2020 2020 2020 2020 7365 6c66 2e74 696d          self.tim
+00000960: 6573 7461 6d70 203d 2074 730d 0a20 2020  estamp = ts..   
+00000970: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+00000980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000990: 7365 6c66 2e5f 7661 6c75 655f 7479 7065  self._value_type
+000009a0: 203d 2074 7970 6528 7365 6c66 2e5f 7661   = type(self._va
+000009b0: 6c75 6529 0d0a 0d0a 2020 2020 2020 2020  lue)....        
+000009c0: 2020 2020 2320 526f 756e 6420 666c 6f61      # Round floa
+000009d0: 7420 746f 2069 7473 2070 7265 6369 7369  t to its precisi
+000009e0: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
+000009f0: 6966 2073 656c 662e 636f 6d70 5f74 7970  if self.comp_typ
+00000a00: 6520 3d3d 2046 6c6f 6174 436f 6d6d 616e  e == FloatComman
+00000a10: 643a 0d0a 2020 2020 2020 2020 2020 2020  d:..            
+00000a20: 2020 2020 7365 6c66 2e5f 7661 6c75 6520      self._value 
+00000a30: 3d20 726f 756e 6428 7365 6c66 2e5f 7661  = round(self._va
+00000a40: 6c75 652c 2073 656c 662e 7072 6563 6973  lue, self.precis
+00000a50: 696f 6e29 0d0a 2020 2020 2020 2020 2020  ion)..          
+00000a60: 2020 656c 6966 2073 656c 662e 636f 6d70    elif self.comp
+00000a70: 5f74 7970 6520 3d3d 2049 6e64 6578 2061  _type == Index a
+00000a80: 6e64 2073 656c 662e 5f70 6172 656e 742e  nd self._parent.
+00000a90: 636f 6d70 5f74 7970 6520 3d3d 2046 6c6f  comp_type == Flo
+00000aa0: 6174 496e 6465 7843 6f6d 6d61 6e64 3a0d  atIndexCommand:.
+00000ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000ac0: 2073 656c 662e 5f76 616c 7565 203d 2072   self._value = r
+00000ad0: 6f75 6e64 2873 656c 662e 5f76 616c 7565  ound(self._value
+00000ae0: 2c20 7365 6c66 2e70 7265 6369 7369 6f6e  , self.precision
+00000af0: 290d 0a20 2020 2020 2020 2065 7863 6570  )..        excep
+00000b00: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+00000b10: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
+00000b20: 7269 6e74 2865 2c20 7365 6c66 2e6e 616d  rint(e, self.nam
+00000b30: 6529 0d0a 2020 2020 2020 2020 7265 7475  e)..        retu
+00000b40: 726e 2073 656c 662e 5f76 616c 7565 0d0a  rn self._value..
+00000b50: 0d0a 2020 2020 4076 616c 7565 2e73 6574  ..    @value.set
+00000b60: 7465 720d 0a20 2020 2064 6566 2076 616c  ter..    def val
+00000b70: 7565 2873 656c 662c 2076 616c 7565 293a  ue(self, value):
+00000b80: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+00000b90: 7661 6c75 6520 3d20 7661 6c75 650d 0a0d  value = value...
+00000ba0: 0a20 2020 2064 6566 2073 6574 5f76 616c  .    def set_val
+00000bb0: 7565 2873 656c 662c 2076 616c 7565 293a  ue(self, value):
+00000bc0: 0d0a 2020 2020 2020 2020 2222 2253 6574  ..        """Set
+00000bd0: 2076 616c 7565 2074 6f20 7468 6520 696e   value to the in
+00000be0: 7374 7275 6d65 6e74 2061 6e64 2075 7064  strument and upd
+00000bf0: 6174 6520 7468 6520 7661 6c75 6520 6f66  ate the value of
+00000c00: 2074 6865 2069 7465 6d22 2222 0d0a 2020   the item"""..  
+00000c10: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
+00000c20: 6d70 5f74 7970 6520 3d3d 2049 6e64 6578  mp_type == Index
+00000c30: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00000c40: 656c 662e 5f70 6172 656e 742e 636f 6d70  elf._parent.comp
+00000c50: 2e5f 5f73 6574 6974 656d 5f5f 2873 656c  .__setitem__(sel
+00000c60: 662e 636f 6d70 2c20 7661 6c75 6529 0d0a  f.comp, value)..
+00000c70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00000c80: 2e5f 7661 6c75 6520 3d20 7365 6c66 2e5f  ._value = self._
+00000c90: 7061 7265 6e74 2e63 6f6d 702e 5f5f 6765  parent.comp.__ge
+00000ca0: 7469 7465 6d5f 5f28 7365 6c66 2e63 6f6d  titem__(self.com
+00000cb0: 7029 0d0a 2020 2020 2020 2020 2020 2020  p)..            
+00000cc0: 7365 6c66 2e74 696d 6573 7461 6d70 203d  self.timestamp =
+00000cd0: 2074 696d 652e 7469 6d65 2829 0d0a 2020   time.time()..  
+00000ce0: 2020 2020 2020 656c 6966 2069 7373 7562        elif issub
+00000cf0: 636c 6173 7328 7479 7065 2873 656c 662e  class(type(self.
+00000d00: 636f 6d70 292c 2043 6f6d 6d61 6e64 293a  comp), Command):
+00000d10: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00000d20: 6c66 2e63 6f6d 702e 5f5f 7365 745f 5f28  lf.comp.__set__(
+00000d30: 7365 6c66 2e5f 7061 7265 6e74 2e63 6f6d  self._parent.com
+00000d40: 702c 2076 616c 7565 290d 0a20 2020 2020  p, value)..     
+00000d50: 2020 2020 2020 2073 656c 662e 5f76 616c         self._val
+00000d60: 7565 203d 2073 656c 662e 636f 6d70 2e5f  ue = self.comp._
+00000d70: 5f67 6574 5f5f 2873 656c 662e 5f70 6172  _get__(self._par
+00000d80: 656e 742e 636f 6d70 2c20 7365 6c66 2e5f  ent.comp, self._
+00000d90: 7061 7265 6e74 2e63 6f6d 702e 5f5f 636c  parent.comp.__cl
+00000da0: 6173 735f 5f29 0d0a 2020 2020 2020 2020  ass__)..        
+00000db0: 2020 2020 7365 6c66 2e74 696d 6573 7461      self.timesta
+00000dc0: 6d70 203d 2074 696d 652e 7469 6d65 2829  mp = time.time()
+00000dd0: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
+00000de0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00000df0: 662e 5f76 616c 7565 203d 2076 616c 7565  f._value = value
+00000e00: 0d0a 0d0a 2020 2020 6465 6620 6973 5f65  ....    def is_e
+00000e10: 6469 7461 626c 6528 7365 6c66 293a 0d0a  ditable(self):..
+00000e20: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
+00000e30: 6e20 5472 7565 2069 6620 7468 6520 6974  n True if the it
+00000e40: 656d 2069 7320 6564 6974 6162 6c65 2222  em is editable""
+00000e50: 220d 0a20 2020 2020 2020 2069 6620 7365  "..        if se
+00000e60: 6c66 2e63 6f6d 705f 7479 7065 203d 3d20  lf.comp_type == 
+00000e70: 496e 6465 7820 616e 6420 5c0d 0a20 2020  Index and \..   
+00000e80: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00000e90: 662e 7365 745f 656e 6162 6c65 2061 6e64  f.set_enable and
+00000ea0: 2073 656c 662e 6765 745f 656e 6162 6c65   self.get_enable
+00000eb0: 2061 6e64 206e 6f74 2073 656c 662e 6578   and not self.ex
+00000ec0: 636c 7564 6564 3a0d 0a20 2020 2020 2020  cluded:..       
+00000ed0: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+00000ee0: 0d0a 2020 2020 2020 2020 656c 6966 2069  ..        elif i
+00000ef0: 7373 7562 636c 6173 7328 7479 7065 2873  ssubclass(type(s
+00000f00: 656c 662e 636f 6d70 292c 2043 6f6d 6d61  elf.comp), Comma
+00000f10: 6e64 2920 616e 6420 5c0d 0a20 2020 2020  nd) and \..     
+00000f20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00000f30: 7365 745f 656e 6162 6c65 2061 6e64 2073  set_enable and s
+00000f40: 656c 662e 6765 745f 656e 6162 6c65 2061  elf.get_enable a
+00000f50: 6e64 206e 6f74 2073 656c 662e 6578 636c  nd not self.excl
+00000f60: 7564 6564 3a0d 0a20 2020 2020 2020 2020  uded:..         
+00000f70: 2020 2072 6574 7572 6e20 5472 7565 0d0a     return True..
+00000f80: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00000f90: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00000fa0: 6e20 4661 6c73 650d 0a0d 0a20 2020 2064  n False....    d
+00000fb0: 6566 2067 6574 5f75 6e69 7428 7365 6c66  ef get_unit(self
+00000fc0: 293a 0d0a 2020 2020 2020 2020 2222 2252  ):..        """R
+00000fd0: 6574 7572 6e20 7468 6520 756e 6974 206f  eturn the unit o
+00000fe0: 6620 7468 6520 6974 656d 2222 220d 0a20  f the item""".. 
+00000ff0: 2020 2020 2020 2063 6f6d 7020 3d20 4e6f         comp = No
+00001000: 6e65 0d0a 2020 2020 2020 2020 6966 2073  ne..        if s
+00001010: 656c 662e 636f 6d70 5f74 7970 6520 3d3d  elf.comp_type ==
+00001020: 2049 6e64 6578 3a0d 0a20 2020 2020 2020   Index:..       
+00001030: 2020 2020 2063 6f6d 7020 3d20 7365 6c66       comp = self
+00001040: 2e70 6172 656e 7428 292e 636f 6d70 0d0a  .parent().comp..
+00001050: 2020 2020 2020 2020 656c 6966 2069 7373          elif iss
+00001060: 7562 636c 6173 7328 7479 7065 2873 656c  ubclass(type(sel
+00001070: 662e 636f 6d70 292c 2043 6f6d 6d61 6e64  f.comp), Command
+00001080: 2920 6f72 205c 0d0a 2020 2020 2020 2020  ) or \..        
+00001090: 2020 2020 2069 7373 7562 636c 6173 7328       issubclass(
+000010a0: 7479 7065 2873 656c 662e 636f 6d70 292c  type(self.comp),
+000010b0: 2049 6e64 6578 436f 6d6d 616e 6429 3a0d   IndexCommand):.
+000010c0: 0a20 2020 2020 2020 2020 2020 2063 6f6d  .            com
+000010d0: 7020 3d20 7365 6c66 2e63 6f6d 700d 0a0d  p = self.comp...
+000010e0: 0a20 2020 2020 2020 2069 6620 636f 6d70  .        if comp
+000010f0: 2061 6e64 2068 6173 6174 7472 2863 6f6d   and hasattr(com
+00001100: 702c 2027 756e 6974 2729 3a0d 0a20 2020  p, 'unit'):..   
+00001110: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00001120: 636f 6d70 2e75 6e69 740d 0a20 2020 2020  comp.unit..     
+00001130: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00001140: 2020 2020 2020 7265 7475 726e 2022 220d        return "".
+00001150: 0a0d 0a20 2020 2064 6566 2067 6574 5f66  ...    def get_f
+00001160: 6f72 6d61 7428 7365 6c66 293a 0d0a 2020  ormat(self):..  
+00001170: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
+00001180: 7468 6520 666f 726d 6174 206f 6620 7468  the format of th
+00001190: 6520 6974 656d 2222 220d 0a20 2020 2020  e item"""..     
+000011a0: 2020 2063 6f6d 7020 3d20 4e6f 6e65 0d0a     comp = None..
+000011b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000011c0: 636f 6d70 5f74 7970 6520 3d3d 2049 6e64  comp_type == Ind
+000011d0: 6578 3a0d 0a20 2020 2020 2020 2020 2020  ex:..           
+000011e0: 2063 6f6d 7020 3d20 7365 6c66 2e70 6172   comp = self.par
+000011f0: 656e 7428 292e 636f 6d70 0d0a 2020 2020  ent().comp..    
+00001200: 2020 2020 656c 6966 2069 7373 7562 636c      elif issubcl
+00001210: 6173 7328 7479 7065 2873 656c 662e 636f  ass(type(self.co
+00001220: 6d70 292c 2043 6f6d 6d61 6e64 2920 6f72  mp), Command) or
+00001230: 205c 0d0a 2020 2020 2020 2020 2020 2020   \..            
+00001240: 2069 7373 7562 636c 6173 7328 7479 7065   issubclass(type
+00001250: 2873 656c 662e 636f 6d70 292c 2049 6e64  (self.comp), Ind
+00001260: 6578 436f 6d6d 616e 6429 3a0d 0a20 2020  exCommand):..   
+00001270: 2020 2020 2020 2020 2063 6f6d 7020 3d20           comp = 
+00001280: 7365 6c66 2e63 6f6d 700d 0a0d 0a20 2020  self.comp....   
+00001290: 2020 2020 2069 6620 636f 6d70 2061 6e64       if comp and
+000012a0: 2068 6173 6174 7472 2863 6f6d 702c 2027   hasattr(comp, '
+000012b0: 666d 7427 293a 0d0a 2020 2020 2020 2020  fmt'):..        
+000012c0: 2020 2020 7265 7475 726e 2063 6f6d 702e      return comp.
+000012d0: 666d 740d 0a20 2020 2020 2020 2065 6c73  fmt..        els
+000012e0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+000012f0: 7265 7475 726e 2027 270d 0a0d 0a20 2020  return ''....   
+00001300: 2040 636c 6173 736d 6574 686f 640d 0a20   @classmethod.. 
+00001310: 2020 2064 6566 206c 6f61 6428 0d0a 2020     def load(..  
+00001320: 2020 2020 2020 636c 732c 2063 6f6d 702c        cls, comp,
+00001330: 2070 6172 656e 743a 2022 436f 6d6d 616e   parent: "Comman
+00001340: 6449 7465 6d22 203d 204e 6f6e 652c 2073  dItem" = None, s
+00001350: 6f72 743d 4661 6c73 650d 0a20 2020 2029  ort=False..    )
+00001360: 202d 3e20 2243 6f6d 6d61 6e64 4974 656d   -> "CommandItem
+00001370: 223a 0d0a 2020 2020 2020 2020 2222 2243  ":..        """C
+00001380: 7265 6174 6520 6120 2772 6f6f 7427 2043  reate a 'root' C
+00001390: 6f6d 6d61 6e64 4974 656d 2066 726f 6d20  ommandItem from 
+000013a0: 6120 436f 6d70 6f6e 656e 7420 616e 6420  a Component and 
+000013b0: 0d0a 2020 2020 2020 2020 706f 7075 6c61  ..        popula
+000013c0: 7465 2069 7473 2073 7562 636f 6d70 6f6e  te its subcompon
+000013d0: 656e 7420 616e 6420 636f 6d6d 616e 6473  ent and commands
+000013e0: 2072 6563 7572 7369 7665 6c79 2e0d 0a0d   recursively....
+000013f0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00001400: 3a0d 0a20 2020 2020 2020 2020 2020 2043  :..            C
+00001410: 6f6d 6d61 6e64 4974 656d 3a20 436f 6d6d  ommandItem: Comm
+00001420: 616e 6449 7465 6d0d 0a20 2020 2020 2020  andItem..       
+00001430: 2022 2222 0d0a 2020 2020 2020 2020 726f   """..        ro
+00001440: 6f74 5f69 7465 6d20 3d20 436f 6d6d 616e  ot_item = Comman
+00001450: 6449 7465 6d28 7061 7265 6e74 290d 0a20  dItem(parent).. 
+00001460: 2020 2020 2020 2072 6f6f 745f 6974 656d         root_item
+00001470: 2e6e 616d 6520 3d20 2272 6f6f 7422 0d0a  .name = "root"..
+00001480: 2020 2020 2020 2020 726f 6f74 5f69 7465          root_ite
+00001490: 6d2e 636f 6d70 203d 2063 6f6d 700d 0a0d  m.comp = comp...
+000014a0: 0a20 2020 2020 2020 2069 6620 6973 7375  .        if issu
+000014b0: 6263 6c61 7373 2863 6f6d 702e 5f5f 636c  bclass(comp.__cl
+000014c0: 6173 735f 5f2c 2043 6f6d 706f 6e65 6e74  ass__, Component
+000014d0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+000014e0: 666f 7220 6a20 696e 2063 6f6d 702e 5f5f  for j in comp.__
+000014f0: 6469 6374 5f5f 3a0d 0a20 2020 2020 2020  dict__:..       
+00001500: 2020 2020 2020 2020 2069 6620 6a20 3d3d           if j ==
+00001510: 2027 5f70 6172 656e 7427 3a0d 0a20 2020   '_parent':..   
+00001520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001530: 2063 6f6e 7469 6e75 650d 0a20 2020 2020   continue..     
+00001540: 2020 2020 2020 2020 2020 2069 6e73 7461             insta
+00001550: 6e63 6520 3d20 636f 6d70 2e5f 5f64 6963  nce = comp.__dic
+00001560: 745f 5f5b 6a5d 0d0a 2020 2020 2020 2020  t__[j]..        
+00001570: 2020 2020 2020 2020 6966 2069 7373 7562          if issub
+00001580: 636c 6173 7328 696e 7374 616e 6365 2e5f  class(instance._
+00001590: 5f63 6c61 7373 5f5f 2c20 2043 6f6d 706f  _class__,  Compo
+000015a0: 6e65 6e74 293a 2020 2020 2020 2020 2020  nent):          
+000015b0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000015c0: 2020 2020 2020 2020 2020 2020 6368 696c              chil
+000015d0: 6420 3d20 636c 732e 6c6f 6164 2869 6e73  d = cls.load(ins
+000015e0: 7461 6e63 652c 2072 6f6f 745f 6974 656d  tance, root_item
+000015f0: 2c20 736f 7274 290d 0a20 2020 2020 2020  , sort)..       
+00001600: 2020 2020 2020 2020 2020 2020 2063 6869               chi
+00001610: 6c64 2e6e 616d 6520 3d20 6a0d 0a20 2020  ld.name = j..   
+00001620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001630: 2063 6869 6c64 2e63 6f6d 7020 3d20 696e   child.comp = in
+00001640: 7374 616e 6365 0d0a 2020 2020 2020 2020  stance..        
+00001650: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00001660: 6e73 7461 6e63 6520 696e 2063 6f6d 702e  nstance in comp.
+00001670: 6578 636c 7564 655f 6361 7074 7572 653a  exclude_capture:
+00001680: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001690: 2020 2020 2020 2020 2020 6368 696c 642e            child.
+000016a0: 6578 636c 7564 6564 203d 2054 7275 650d  excluded = True.
+000016b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000016c0: 2020 2020 2063 6869 6c64 2e63 6f6d 705f       child.comp_
+000016d0: 7479 7065 203d 2074 7970 6528 696e 7374  type = type(inst
+000016e0: 616e 6365 290d 0a20 2020 2020 2020 2020  ance)..         
+000016f0: 2020 2020 2020 2020 2020 2072 6f6f 745f             root_
+00001700: 6974 656d 2e61 7070 656e 6443 6869 6c64  item.appendChild
+00001710: 2863 6869 6c64 290d 0a0d 0a20 2020 2020  (child)....     
+00001720: 2020 2020 2020 2063 7572 7265 6e74 5f61         current_a
+00001730: 7474 7269 6275 7465 7320 3d20 5b5d 0d0a  ttributes = []..
+00001740: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00001750: 6320 696e 2063 6f6d 702e 5f5f 636c 6173  c in comp.__clas
+00001760: 735f 5f2e 5f5f 6d72 6f5f 5f3a 2020 2320  s__.__mro__:  # 
+00001770: 6c6f 6f70 2074 6872 6f75 6768 2074 6865  loop through the
+00001780: 2063 6c61 7373 6573 2069 6e63 6c75 6469   classes includi
+00001790: 6e67 2073 7570 6572 2063 6c61 7373 6573  ng super classes
+000017a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000017b0: 2020 6966 206e 6f74 2069 7373 7562 636c    if not issubcl
+000017c0: 6173 7328 632c 2043 6f6d 706f 6e65 6e74  ass(c, Component
+000017d0: 293a 2020 2320 6974 2073 686f 756c 6420  ):  # it should 
+000017e0: 6265 2061 2073 7562 636c 6173 7320 6f66  be a subclass of
+000017f0: 2043 6f6d 706f 6e65 6e74 0d0a 2020 2020   Component..    
+00001800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001810: 6272 6561 6b0d 0a20 2020 2020 2020 2020  break..         
+00001820: 2020 2020 2020 2069 6620 6320 3d3d 2043         if c == C
+00001830: 6f6d 706f 6e65 6e74 3a20 2023 2042 7574  omponent:  # But
+00001840: 2069 7420 7368 6f75 6c64 206e 6f74 2062   it should not b
+00001850: 6520 436f 6d70 6f6e 656e 740d 0a20 2020  e Component..   
+00001860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001870: 2062 7265 616b 0d0a 0d0a 2020 2020 2020   break....      
+00001880: 2020 2020 2020 2020 2020 666f 7220 6b65            for ke
+00001890: 7920 696e 2063 2e5f 5f64 6963 745f 5f3a  y in c.__dict__:
+000018a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000018b0: 2020 2020 2020 636d 645f 696e 7374 616e        cmd_instan
+000018c0: 6365 203d 2063 2e5f 5f64 6963 745f 5f5b  ce = c.__dict__[
+000018d0: 6b65 795d 0d0a 2020 2020 2020 2020 2020  key]..          
+000018e0: 2020 2020 2020 2020 2020 6966 206b 6579            if key
+000018f0: 2069 6e20 6375 7272 656e 745f 6174 7472   in current_attr
+00001900: 6962 7574 6573 3a0d 0a20 2020 2020 2020  ibutes:..       
+00001910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001920: 2063 6f6e 7469 6e75 650d 0a20 2020 2020   continue..     
+00001930: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00001940: 7572 7265 6e74 5f61 7474 7269 6275 7465  urrent_attribute
+00001950: 732e 6170 7065 6e64 286b 6579 290d 0a0d  s.append(key)...
+00001960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001970: 2020 2020 2069 6620 6973 7375 6263 6c61       if issubcla
+00001980: 7373 2863 6d64 5f69 6e73 7461 6e63 652e  ss(cmd_instance.
+00001990: 5f5f 636c 6173 735f 5f2c 2043 6f6d 6d61  __class__, Comma
+000019a0: 6e64 293a 0d0a 2020 2020 2020 2020 2020  nd):..          
+000019b0: 2020 2020 2020 2020 2020 2020 2020 6368                ch
+000019c0: 696c 6420 3d20 636c 732e 6c6f 6164 2863  ild = cls.load(c
+000019d0: 6d64 5f69 6e73 7461 6e63 652c 2072 6f6f  md_instance, roo
+000019e0: 745f 6974 656d 2c20 736f 7274 290d 0a20  t_item, sort).. 
+000019f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a00: 2020 2020 2020 2063 6869 6c64 2e6e 616d         child.nam
+00001a10: 6520 3d20 6b65 790d 0a20 2020 2020 2020  e = key..       
+00001a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a30: 2063 6869 6c64 2e63 6f6d 7020 3d20 636d   child.comp = cm
+00001a40: 645f 696e 7374 616e 6365 0d0a 2020 2020  d_instance..    
+00001a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a60: 2020 2020 6368 696c 642e 636f 6d70 5f74      child.comp_t
+00001a70: 7970 6520 3d20 7479 7065 2863 6d64 5f69  ype = type(cmd_i
+00001a80: 6e73 7461 6e63 6529 0d0a 0d0a 2020 2020  nstance)....    
+00001a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001aa0: 2020 2020 726f 6f74 5f69 7465 6d2e 6170      root_item.ap
+00001ab0: 7065 6e64 4368 696c 6428 6368 696c 6429  pendChild(child)
+00001ac0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00001ad0: 2020 2020 2020 2020 656c 6966 2069 7373          elif iss
+00001ae0: 7562 636c 6173 7328 636d 645f 696e 7374  ubclass(cmd_inst
+00001af0: 616e 6365 2e5f 5f63 6c61 7373 5f5f 2c20  ance.__class__, 
+00001b00: 496e 6465 7843 6f6d 6d61 6e64 293a 0d0a  IndexCommand):..
+00001b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b20: 2020 2020 2020 2020 6368 696c 6420 3d20          child = 
+00001b30: 636c 732e 6c6f 6164 2863 6d64 5f69 6e73  cls.load(cmd_ins
+00001b40: 7461 6e63 652c 2072 6f6f 745f 6974 656d  tance, root_item
+00001b50: 2c20 736f 7274 290d 0a20 2020 2020 2020  , sort)..       
+00001b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b70: 2063 6869 6c64 2e6e 616d 6520 3d20 6b65   child.name = ke
+00001b80: 790d 0a20 2020 2020 2020 2020 2020 2020  y..             
+00001b90: 2020 2020 2020 2020 2020 2063 6869 6c64             child
+00001ba0: 2e63 6f6d 7020 3d20 636d 645f 696e 7374  .comp = cmd_inst
+00001bb0: 616e 6365 0d0a 2020 2020 2020 2020 2020  ance..          
+00001bc0: 2020 2020 2020 2020 2020 2020 2020 6368                ch
+00001bd0: 696c 642e 636f 6d70 5f74 7970 6520 3d20  ild.comp_type = 
+00001be0: 7479 7065 2863 6d64 5f69 6e73 7461 6e63  type(cmd_instanc
+00001bf0: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+00001c00: 2020 2020 2020 2020 2020 2020 726f 6f74              root
+00001c10: 5f69 7465 6d2e 6170 7065 6e64 4368 696c  _item.appendChil
+00001c20: 6428 6368 696c 6429 0d0a 0d0a 2020 2020  d(child)....    
+00001c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c40: 656c 6966 2063 616c 6c61 626c 6528 636d  elif callable(cm
+00001c50: 645f 696e 7374 616e 6365 293a 0d0a 2020  d_instance):..  
 00001c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c70: 6368 696c 6420 3d20 636c 732e 6c6f 6164  child = cls.load
-00001c80: 2869 6e73 7461 6e63 652c 2072 6f6f 745f  (instance, root_
-00001c90: 6974 656d 290d 0a20 2020 2020 2020 2020  item)..         
-00001ca0: 2020 2020 2020 2020 2020 2063 6869 6c64             child
-00001cb0: 2e6e 616d 6520 3d20 6a0d 0a20 2020 2020  .name = j..     
-00001cc0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00001cd0: 6869 6c64 2e63 6f6d 7020 3d20 696e 7374  hild.comp = inst
-00001ce0: 616e 6365 0d0a 2020 2020 2020 2020 2020  ance..          
-00001cf0: 2020 2020 2020 2020 2020 6966 2069 6e73            if ins
-00001d00: 7461 6e63 6520 696e 2063 6f6d 702e 6578  tance in comp.ex
-00001d10: 636c 7564 655f 6361 7074 7572 653a 0d0a  clude_capture:..
-00001d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d30: 2020 2020 2020 2020 6368 696c 642e 6578          child.ex
-00001d40: 636c 7564 6564 203d 2054 7275 650d 0a20  cluded = True.. 
-00001d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d60: 2020 2063 6869 6c64 2e63 6f6d 705f 7479     child.comp_ty
-00001d70: 7065 203d 2074 7970 6528 696e 7374 616e  pe = type(instan
-00001d80: 6365 290d 0a20 2020 2020 2020 2020 2020  ce)..           
-00001d90: 2020 2020 2020 2020 2072 6f6f 745f 6974           root_it
-00001da0: 656d 2e61 7070 656e 6443 6869 6c64 2863  em.appendChild(c
-00001db0: 6869 6c64 290d 0a0d 0a20 2020 2020 2020  hild)....       
-00001dc0: 2020 2020 2063 7572 7265 6e74 5f61 7474       current_att
-00001dd0: 7269 6275 7465 7320 3d20 5b5d 0d0a 2020  ributes = []..  
-00001de0: 2020 2020 2020 2020 2020 666f 7220 6320            for c 
-00001df0: 696e 2063 6f6d 702e 5f5f 636c 6173 735f  in comp.__class_
-00001e00: 5f2e 5f5f 6d72 6f5f 5f3a 2020 2320 6c6f  _.__mro__:  # lo
-00001e10: 6f70 2074 6872 6f75 6768 2074 6865 2063  op through the c
-00001e20: 6c61 7373 6573 2069 6e63 6c75 6469 6e67  lasses including
-00001e30: 2073 7570 6572 2063 6c61 7373 6573 0d0a   super classes..
-00001e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e50: 6966 206e 6f74 2069 7373 7562 636c 6173  if not issubclas
-00001e60: 7328 632c 2043 6f6d 706f 6e65 6e74 293a  s(c, Component):
-00001e70: 2020 2320 6974 2073 686f 756c 6420 6265    # it should be
-00001e80: 2061 2073 7562 636c 6173 7320 6f66 2043   a subclass of C
-00001e90: 6f6d 706f 6e65 6e74 0d0a 2020 2020 2020  omponent..      
-00001ea0: 2020 2020 2020 2020 2020 2020 2020 6272                br
-00001eb0: 6561 6b0d 0a20 2020 2020 2020 2020 2020  eak..           
-00001ec0: 2020 2020 2069 6620 6320 3d3d 2043 6f6d       if c == Com
-00001ed0: 706f 6e65 6e74 3a20 2023 2042 7574 2069  ponent:  # But i
-00001ee0: 7420 7368 6f75 6c64 206e 6f74 2062 6520  t should not be 
-00001ef0: 436f 6d70 6f6e 656e 740d 0a20 2020 2020  Component..     
-00001f00: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-00001f10: 7265 616b 0d0a 0d0a 2020 2020 2020 2020  reak....        
-00001f20: 2020 2020 2020 2020 666f 7220 6b65 7920          for key 
-00001f30: 696e 2063 2e5f 5f64 6963 745f 5f3a 0d0a  in c.__dict__:..
-00001f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f50: 2020 2020 636d 645f 696e 7374 616e 6365      cmd_instance
-00001f60: 203d 2063 2e5f 5f64 6963 745f 5f5b 6b65   = c.__dict__[ke
-00001f70: 795d 0d0a 2020 2020 2020 2020 2020 2020  y]..            
-00001f80: 2020 2020 2020 2020 6966 206b 6579 2069          if key i
-00001f90: 6e20 6375 7272 656e 745f 6174 7472 6962  n current_attrib
-00001fa0: 7574 6573 3a0d 0a20 2020 2020 2020 2020  utes:..         
-00001fb0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00001fc0: 6f6e 7469 6e75 650d 0a20 2020 2020 2020  ontinue..       
-00001fd0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00001fe0: 7265 6e74 5f61 7474 7269 6275 7465 732e  rent_attributes.
-00001ff0: 6170 7065 6e64 286b 6579 290d 0a0d 0a20  append(key).... 
-00002000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002010: 2020 2069 6620 6973 7375 6263 6c61 7373     if issubclass
-00002020: 2863 6d64 5f69 6e73 7461 6e63 652e 5f5f  (cmd_instance.__
-00002030: 636c 6173 735f 5f2c 2043 6f6d 6d61 6e64  class__, Command
-00002040: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00002050: 2020 2020 2020 2020 2020 2020 6368 696c              chil
-00002060: 6420 3d20 636c 732e 6c6f 6164 2863 6d64  d = cls.load(cmd
-00002070: 5f69 6e73 7461 6e63 652c 2072 6f6f 745f  _instance, root_
-00002080: 6974 656d 290d 0a20 2020 2020 2020 2020  item)..         
-00002090: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000020a0: 6869 6c64 2e6e 616d 6520 3d20 6b65 790d  hild.name = key.
-000020b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000020c0: 2020 2020 2020 2020 2063 6869 6c64 2e63           child.c
-000020d0: 6f6d 7020 3d20 636d 645f 696e 7374 616e  omp = cmd_instan
-000020e0: 6365 0d0a 2020 2020 2020 2020 2020 2020  ce..            
-000020f0: 2020 2020 2020 2020 2020 2020 6368 696c              chil
-00002100: 642e 636f 6d70 5f74 7970 6520 3d20 7479  d.comp_type = ty
-00002110: 7065 2863 6d64 5f69 6e73 7461 6e63 6529  pe(cmd_instance)
-00002120: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00002130: 2020 2020 2020 2020 2020 2020 726f 6f74              root
-00002140: 5f69 7465 6d2e 6170 7065 6e64 4368 696c  _item.appendChil
-00002150: 6428 6368 696c 6429 0d0a 0d0a 2020 2020  d(child)....    
-00002160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002170: 656c 6966 2069 7373 7562 636c 6173 7328  elif issubclass(
-00002180: 636d 645f 696e 7374 616e 6365 2e5f 5f63  cmd_instance.__c
-00002190: 6c61 7373 5f5f 2c20 496e 6465 7843 6f6d  lass__, IndexCom
-000021a0: 6d61 6e64 293a 0d0a 2020 2020 2020 2020  mand):..        
-000021b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021c0: 6368 696c 6420 3d20 636c 732e 6c6f 6164  child = cls.load
-000021d0: 2863 6d64 5f69 6e73 7461 6e63 652c 2072  (cmd_instance, r
-000021e0: 6f6f 745f 6974 656d 290d 0a20 2020 2020  oot_item)..     
-000021f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002200: 2020 2063 6869 6c64 2e6e 616d 6520 3d20     child.name = 
-00002210: 6b65 790d 0a20 2020 2020 2020 2020 2020  key..           
-00002220: 2020 2020 2020 2020 2020 2020 2063 6869               chi
-00002230: 6c64 2e63 6f6d 7020 3d20 636d 645f 696e  ld.comp = cmd_in
-00002240: 7374 616e 6365 0d0a 2020 2020 2020 2020  stance..        
-00002250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002260: 6368 696c 642e 636f 6d70 5f74 7970 6520  child.comp_type 
-00002270: 3d20 7479 7065 2863 6d64 5f69 6e73 7461  = type(cmd_insta
-00002280: 6e63 6529 0d0a 2020 2020 2020 2020 2020  nce)..          
-00002290: 2020 2020 2020 2020 2020 2020 2020 726f                ro
-000022a0: 6f74 5f69 7465 6d2e 6170 7065 6e64 4368  ot_item.appendCh
-000022b0: 696c 6428 6368 696c 6429 0d0a 0d0a 2020  ild(child)....  
+00001c70: 2020 2020 2020 6966 2069 7373 7562 636c        if issubcl
+00001c80: 6173 7328 636d 645f 696e 7374 616e 6365  ass(cmd_instance
+00001c90: 2e5f 5f63 6c61 7373 5f5f 2c20 7479 7065  .__class__, type
+00001ca0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00001cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001cc0: 636f 6e74 696e 7565 0d0a 2020 2020 2020  continue..      
+00001cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ce0: 2020 6966 206b 6579 2e73 7461 7274 7377    if key.startsw
+00001cf0: 6974 6828 275f 2729 3a0d 0a20 2020 2020  ith('_'):..     
+00001d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d10: 2020 2020 2020 2063 6f6e 7469 6e75 650d         continue.
+00001d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001d30: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00001d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d50: 2020 2063 6869 6c64 203d 2063 6c73 2e6c     child = cls.l
+00001d60: 6f61 6428 636d 645f 696e 7374 616e 6365  oad(cmd_instance
+00001d70: 2c20 726f 6f74 5f69 7465 6d2c 2073 6f72  , root_item, sor
+00001d80: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
+00001d90: 2020 2020 2020 2020 2020 2020 6368 696c              chil
+00001da0: 642e 6e61 6d65 203d 206b 6579 0d0a 2020  d.name = key..  
+00001db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001dc0: 2020 2020 2020 6368 696c 642e 636f 6d70        child.comp
+00001dd0: 203d 2063 6d64 5f69 6e73 7461 6e63 650d   = cmd_instance.
+00001de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001df0: 2020 2020 2020 2020 2063 6869 6c64 2e63           child.c
+00001e00: 6f6d 705f 7479 7065 203d 2074 7970 6528  omp_type = type(
+00001e10: 636d 645f 696e 7374 616e 6365 290d 0a20  cmd_instance).. 
+00001e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e30: 2020 2020 2020 2072 6f6f 745f 6974 656d         root_item
+00001e40: 2e61 7070 656e 6443 6869 6c64 2863 6869  .appendChild(chi
+00001e50: 6c64 290d 0a20 2020 2020 2020 2065 6c73  ld)..        els
+00001e60: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00001e70: 6966 2063 616c 6c61 626c 6528 636f 6d70  if callable(comp
+00001e80: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00001e90: 2020 2020 726f 6f74 5f69 7465 6d2e 636f      root_item.co
+00001ea0: 6d70 203d 2063 6f6d 700d 0a20 2020 2020  mp = comp..     
+00001eb0: 2020 2020 2020 2020 2020 2072 6f6f 745f             root_
+00001ec0: 6974 656d 2e63 6f6d 705f 7479 7065 203d  item.comp_type =
+00001ed0: 2074 7970 6528 636f 6d70 290d 0a20 2020   type(comp)..   
+00001ee0: 2020 2020 2020 2020 2020 2020 2072 6f6f               roo
+00001ef0: 745f 6974 656d 2e69 735f 6d65 7468 6f64  t_item.is_method
+00001f00: 203d 2054 7275 650d 0a0d 0a20 2020 2020   = True....     
+00001f10: 2020 2020 2020 2065 6c69 6620 6973 7375         elif issu
+00001f20: 6263 6c61 7373 2874 7970 6528 636f 6d70  bclass(type(comp
+00001f30: 292c 2043 6f6d 6d61 6e64 293a 0d0a 2020  ), Command):..  
+00001f40: 2020 2020 2020 2020 2020 2020 2020 726f                ro
+00001f50: 6f74 5f69 7465 6d2e 636f 6d70 203d 2063  ot_item.comp = c
+00001f60: 6f6d 700d 0a20 2020 2020 2020 2020 2020  omp..           
+00001f70: 2020 2020 2072 6f6f 745f 6974 656d 2e63       root_item.c
+00001f80: 6f6d 705f 7479 7065 203d 2074 7970 6528  omp_type = type(
+00001f90: 636f 6d70 290d 0a20 2020 2020 2020 2020  comp)..         
+00001fa0: 2020 2020 2020 2072 6f6f 745f 6974 656d         root_item
+00001fb0: 2e65 7863 6c75 6465 6420 3d20 636f 6d70  .excluded = comp
+00001fc0: 2069 6e20 726f 6f74 5f69 7465 6d2e 7061   in root_item.pa
+00001fd0: 7265 6e74 2829 2e63 6f6d 702e 6578 636c  rent().comp.excl
+00001fe0: 7564 655f 6361 7074 7572 650d 0a20 2020  ude_capture..   
+00001ff0: 2020 2020 2020 2020 2020 2020 2072 6f6f               roo
+00002000: 745f 6974 656d 2e72 6177 5f72 656d 6f74  t_item.raw_remot
+00002010: 655f 636f 6d6d 616e 6420 3d20 636f 6d70  e_command = comp
+00002020: 2e72 656d 6f74 655f 636f 6d6d 616e 640d  .remote_command.
+00002030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002040: 2072 6f6f 745f 6974 656d 2e73 6574 5f65   root_item.set_e
+00002050: 6e61 626c 6520 3d20 636f 6d70 2e5f 7365  nable = comp._se
+00002060: 745f 656e 6162 6c65 0d0a 2020 2020 2020  t_enable..      
+00002070: 2020 2020 2020 2020 2020 726f 6f74 5f69            root_i
+00002080: 7465 6d2e 6765 745f 656e 6162 6c65 203d  tem.get_enable =
+00002090: 2063 6f6d 702e 5f67 6574 5f65 6e61 626c   comp._get_enabl
+000020a0: 650d 0a0d 0a20 2020 2020 2020 2020 2020  e....           
+000020b0: 2065 6c69 6620 6973 7375 6263 6c61 7373   elif issubclass
+000020c0: 2874 7970 6528 636f 6d70 292c 2049 6e64  (type(comp), Ind
+000020d0: 6578 436f 6d6d 616e 6429 3a0d 0a20 2020  exCommand):..   
+000020e0: 2020 2020 2020 2020 2020 2020 2072 6f6f               roo
+000020f0: 745f 6974 656d 2e63 6f6d 7020 3d20 636f  t_item.comp = co
+00002100: 6d70 0d0a 2020 2020 2020 2020 2020 2020  mp..            
+00002110: 2020 2020 726f 6f74 5f69 7465 6d2e 636f      root_item.co
+00002120: 6d70 5f74 7970 6520 3d20 7479 7065 2863  mp_type = type(c
+00002130: 6f6d 7029 0d0a 2020 2020 2020 2020 2020  omp)..          
+00002140: 2020 2020 2020 726f 6f74 5f69 7465 6d2e        root_item.
+00002150: 6578 636c 7564 6564 203d 2063 6f6d 7020  excluded = comp 
+00002160: 696e 2072 6f6f 745f 6974 656d 2e70 6172  in root_item.par
+00002170: 656e 7428 292e 636f 6d70 2e65 7863 6c75  ent().comp.exclu
+00002180: 6465 5f63 6170 7475 7265 0d0a 2020 2020  de_capture..    
+00002190: 2020 2020 2020 2020 2020 2020 726f 6f74              root
+000021a0: 5f69 7465 6d2e 7261 775f 7265 6d6f 7465  _item.raw_remote
+000021b0: 5f63 6f6d 6d61 6e64 203d 2063 6f6d 702e  _command = comp.
+000021c0: 7265 6d6f 7465 5f63 6f6d 6d61 6e64 0d0a  remote_command..
+000021d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000021e0: 726f 6f74 5f69 7465 6d2e 7365 745f 656e  root_item.set_en
+000021f0: 6162 6c65 203d 2063 6f6d 702e 5f73 6574  able = comp._set
+00002200: 5f65 6e61 626c 650d 0a20 2020 2020 2020  _enable..       
+00002210: 2020 2020 2020 2020 2072 6f6f 745f 6974           root_it
+00002220: 656d 2e67 6574 5f65 6e61 626c 6520 3d20  em.get_enable = 
+00002230: 636f 6d70 2e5f 6765 745f 656e 6162 6c65  comp._get_enable
+00002240: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00002250: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+00002260: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00002270: 2063 6f6d 702e 696e 6465 785f 6469 6374   comp.index_dict
+00002280: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
+00002290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022a0: 2020 2069 6e64 6578 203d 2063 6f6d 702e     index = comp.
+000022b0: 696e 6465 785f 6d69 6e0d 0a20 2020 2020  index_min..     
 000022c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022d0: 2020 656c 6966 2063 616c 6c61 626c 6528    elif callable(
-000022e0: 636d 645f 696e 7374 616e 6365 293a 0d0a  cmd_instance):..
-000022f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002300: 2020 2020 2020 2020 6966 2069 7373 7562          if issub
-00002310: 636c 6173 7328 636d 645f 696e 7374 616e  class(cmd_instan
-00002320: 6365 2e5f 5f63 6c61 7373 5f5f 2c20 7479  ce.__class__, ty
-00002330: 7065 293a 0d0a 2020 2020 2020 2020 2020  pe):..          
+000022d0: 2020 2077 6869 6c65 2069 6e64 6578 203c     while index <
+000022e0: 3d20 636f 6d70 2e69 6e64 6578 5f6d 6178  = comp.index_max
+000022f0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00002300: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00002310: 6869 6c64 203d 2063 6c73 2e6c 6f61 6428  hild = cls.load(
+00002320: 696e 6465 782c 2072 6f6f 745f 6974 656d  index, root_item
+00002330: 2c20 736f 7274 290d 0a20 2020 2020 2020  , sort)..       
 00002340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002350: 2020 636f 6e74 696e 7565 0d0a 2020 2020    continue..    
-00002360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002370: 2020 2020 6966 206b 6579 2e73 7461 7274      if key.start
-00002380: 7377 6974 6828 275f 2729 3a0d 0a20 2020  swith('_'):..   
-00002390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023a0: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-000023b0: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
-000023c0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-000023d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023e0: 2020 2020 2063 6869 6c64 203d 2063 6c73       child = cls
-000023f0: 2e6c 6f61 6428 636d 645f 696e 7374 616e  .load(cmd_instan
-00002400: 6365 2c20 726f 6f74 5f69 7465 6d29 0d0a  ce, root_item)..
-00002410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002420: 2020 2020 2020 2020 6368 696c 642e 6e61          child.na
-00002430: 6d65 203d 206b 6579 0d0a 2020 2020 2020  me = key..      
-00002440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002450: 2020 6368 696c 642e 636f 6d70 203d 2063    child.comp = c
-00002460: 6d64 5f69 6e73 7461 6e63 650d 0a20 2020  md_instance..   
-00002470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002480: 2020 2020 2063 6869 6c64 2e63 6f6d 705f       child.comp_
-00002490: 7479 7065 203d 2074 7970 6528 636d 645f  type = type(cmd_
-000024a0: 696e 7374 616e 6365 290d 0a20 2020 2020  instance)..     
-000024b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024c0: 2020 2072 6f6f 745f 6974 656d 2e61 7070     root_item.app
-000024d0: 656e 6443 6869 6c64 2863 6869 6c64 290d  endChild(child).
-000024e0: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
-000024f0: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-00002500: 616c 6c61 626c 6528 636f 6d70 293a 0d0a  allable(comp):..
-00002510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002520: 726f 6f74 5f69 7465 6d2e 636f 6d70 203d  root_item.comp =
-00002530: 2063 6f6d 700d 0a20 2020 2020 2020 2020   comp..         
-00002540: 2020 2020 2020 2072 6f6f 745f 6974 656d         root_item
-00002550: 2e63 6f6d 705f 7479 7065 203d 2074 7970  .comp_type = typ
-00002560: 6528 636f 6d70 290d 0a20 2020 2020 2020  e(comp)..       
-00002570: 2020 2020 2020 2020 2072 6f6f 745f 6974           root_it
-00002580: 656d 2e69 735f 6d65 7468 6f64 203d 2054  em.is_method = T
-00002590: 7275 650d 0a0d 0a20 2020 2020 2020 2020  rue....         
-000025a0: 2020 2065 6c69 6620 6973 7375 6263 6c61     elif issubcla
-000025b0: 7373 2874 7970 6528 636f 6d70 292c 2043  ss(type(comp), C
-000025c0: 6f6d 6d61 6e64 293a 0d0a 2020 2020 2020  ommand):..      
-000025d0: 2020 2020 2020 2020 2020 726f 6f74 5f69            root_i
-000025e0: 7465 6d2e 636f 6d70 203d 2063 6f6d 700d  tem.comp = comp.
-000025f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002600: 2072 6f6f 745f 6974 656d 2e63 6f6d 705f   root_item.comp_
-00002610: 7479 7065 203d 2074 7970 6528 636f 6d70  type = type(comp
-00002620: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00002630: 2020 2072 6f6f 745f 6974 656d 2e65 7863     root_item.exc
-00002640: 6c75 6465 6420 3d20 636f 6d70 2069 6e20  luded = comp in 
-00002650: 726f 6f74 5f69 7465 6d2e 7061 7265 6e74  root_item.parent
-00002660: 2829 2e63 6f6d 702e 6578 636c 7564 655f  ().comp.exclude_
-00002670: 6361 7074 7572 650d 0a20 2020 2020 2020  capture..       
-00002680: 2020 2020 2020 2020 2072 6f6f 745f 6974           root_it
-00002690: 656d 2e72 6177 5f72 656d 6f74 655f 636f  em.raw_remote_co
-000026a0: 6d6d 616e 6420 3d20 636f 6d70 2e72 656d  mmand = comp.rem
-000026b0: 6f74 655f 636f 6d6d 616e 640d 0a20 2020  ote_command..   
-000026c0: 2020 2020 2020 2020 2020 2020 2072 6f6f               roo
-000026d0: 745f 6974 656d 2e73 6574 5f65 6e61 626c  t_item.set_enabl
-000026e0: 6520 3d20 636f 6d70 2e5f 7365 745f 656e  e = comp._set_en
-000026f0: 6162 6c65 0d0a 2020 2020 2020 2020 2020  able..          
-00002700: 2020 2020 2020 726f 6f74 5f69 7465 6d2e        root_item.
-00002710: 6765 745f 656e 6162 6c65 203d 2063 6f6d  get_enable = com
-00002720: 702e 5f67 6574 5f65 6e61 626c 650d 0a0d  p._get_enable...
-00002730: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-00002740: 6620 6973 7375 6263 6c61 7373 2874 7970  f issubclass(typ
-00002750: 6528 636f 6d70 292c 2049 6e64 6578 436f  e(comp), IndexCo
-00002760: 6d6d 616e 6429 3a0d 0a20 2020 2020 2020  mmand):..       
-00002770: 2020 2020 2020 2020 2072 6f6f 745f 6974           root_it
-00002780: 656d 2e63 6f6d 7020 3d20 636f 6d70 0d0a  em.comp = comp..
-00002790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027a0: 726f 6f74 5f69 7465 6d2e 636f 6d70 5f74  root_item.comp_t
-000027b0: 7970 6520 3d20 7479 7065 2863 6f6d 7029  ype = type(comp)
-000027c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000027d0: 2020 726f 6f74 5f69 7465 6d2e 6578 636c    root_item.excl
-000027e0: 7564 6564 203d 2063 6f6d 7020 696e 2072  uded = comp in r
-000027f0: 6f6f 745f 6974 656d 2e70 6172 656e 7428  oot_item.parent(
-00002800: 292e 636f 6d70 2e65 7863 6c75 6465 5f63  ).comp.exclude_c
-00002810: 6170 7475 7265 0d0a 2020 2020 2020 2020  apture..        
-00002820: 2020 2020 2020 2020 726f 6f74 5f69 7465          root_ite
-00002830: 6d2e 7261 775f 7265 6d6f 7465 5f63 6f6d  m.raw_remote_com
-00002840: 6d61 6e64 203d 2063 6f6d 702e 7265 6d6f  mand = comp.remo
-00002850: 7465 5f63 6f6d 6d61 6e64 0d0a 2020 2020  te_command..    
-00002860: 2020 2020 2020 2020 2020 2020 726f 6f74              root
-00002870: 5f69 7465 6d2e 7365 745f 656e 6162 6c65  _item.set_enable
-00002880: 203d 2063 6f6d 702e 5f73 6574 5f65 6e61   = comp._set_ena
-00002890: 626c 650d 0a20 2020 2020 2020 2020 2020  ble..           
-000028a0: 2020 2020 2072 6f6f 745f 6974 656d 2e67       root_item.g
-000028b0: 6574 5f65 6e61 626c 6520 3d20 636f 6d70  et_enable = comp
-000028c0: 2e5f 6765 745f 656e 6162 6c65 0d0a 0d0a  ._get_enable....
-000028d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028e0: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
-000028f0: 2020 2020 2020 2020 2020 6966 2063 6f6d            if com
-00002900: 702e 696e 6465 785f 6469 6374 2069 7320  p.index_dict is 
-00002910: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-00002920: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00002930: 6e64 6578 203d 2063 6f6d 702e 696e 6465  ndex = comp.inde
-00002940: 785f 6d69 6e0d 0a20 2020 2020 2020 2020  x_min..         
-00002950: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00002960: 6869 6c65 2069 6e64 6578 203c 3d20 636f  hile index <= co
-00002970: 6d70 2e69 6e64 6578 5f6d 6178 3a0d 0a20  mp.index_max:.. 
-00002980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002990: 2020 2020 2020 2020 2020 2063 6869 6c64             child
-000029a0: 203d 2063 6c73 2e6c 6f61 6428 696e 6465   = cls.load(inde
-000029b0: 782c 2072 6f6f 745f 6974 656d 290d 0a20  x, root_item).. 
-000029c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029d0: 2020 2020 2020 2020 2020 2063 6869 6c64             child
-000029e0: 2e6e 616d 6520 3d20 6627 7b69 6e64 6578  .name = f'{index
-000029f0: 7d27 0d0a 2020 2020 2020 2020 2020 2020  }'..            
-00002a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a10: 6368 696c 642e 636f 6d70 203d 2069 6e64  child.comp = ind
-00002a20: 6578 0d0a 2020 2020 2020 2020 2020 2020  ex..            
-00002a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a40: 6368 696c 642e 636f 6d70 5f74 7970 6520  child.comp_type 
-00002a50: 3d20 496e 6465 780d 0a20 2020 2020 2020  = Index..       
-00002a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a70: 2020 2020 2063 6869 6c64 2e65 7863 6c75       child.exclu
-00002a80: 6465 6420 3d20 726f 6f74 5f69 7465 6d2e  ded = root_item.
-00002a90: 6578 636c 7564 6564 0d0a 2020 2020 2020  excluded..      
-00002aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ab0: 2020 2020 2020 6368 696c 642e 7365 745f        child.set_
-00002ac0: 656e 6162 6c65 203d 2072 6f6f 745f 6974  enable = root_it
-00002ad0: 656d 2e73 6574 5f65 6e61 626c 650d 0a20  em.set_enable.. 
-00002ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002af0: 2020 2020 2020 2020 2020 2063 6869 6c64             child
-00002b00: 2e67 6574 5f65 6e61 626c 6520 3d20 726f  .get_enable = ro
-00002b10: 6f74 5f69 7465 6d2e 6765 745f 656e 6162  ot_item.get_enab
-00002b20: 6c65 0d0a 2020 2020 2020 2020 2020 2020  le..            
-00002b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b40: 726f 6f74 5f69 7465 6d2e 6170 7065 6e64  root_item.append
-00002b50: 4368 696c 6428 6368 696c 6429 0d0a 2020  Child(child)..  
-00002b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b70: 2020 2020 2020 2020 2020 696e 6465 7820            index 
-00002b80: 2b3d 2031 0d0a 2020 2020 2020 2020 2020  += 1..          
-00002b90: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
-00002ba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002bb0: 2020 2020 2020 2020 2066 6f72 206b 6579           for key
-00002bc0: 2069 6e20 636f 6d70 2e69 6e64 6578 5f64   in comp.index_d
-00002bd0: 6963 743a 0d0a 2020 2020 2020 2020 2020  ict:..          
-00002be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bf0: 2020 6368 696c 6420 3d20 636c 732e 6c6f    child = cls.lo
-00002c00: 6164 286b 6579 2c20 726f 6f74 5f69 7465  ad(key, root_ite
-00002c10: 6d29 0d0a 2020 2020 2020 2020 2020 2020  m)..            
-00002c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c30: 6368 696c 642e 6e61 6d65 203d 2066 277b  child.name = f'{
-00002c40: 6b65 797d 270d 0a20 2020 2020 2020 2020  key}'..         
-00002c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c60: 2020 2063 6869 6c64 2e63 6f6d 7020 3d20     child.comp = 
-00002c70: 6b65 790d 0a20 2020 2020 2020 2020 2020  key..           
-00002c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c90: 2063 6869 6c64 2e63 6f6d 705f 7479 7065   child.comp_type
-00002ca0: 203d 2049 6e64 6578 0d0a 2020 2020 2020   = Index..      
-00002cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002cc0: 2020 2020 2020 6368 696c 642e 6578 6c75        child.exlu
-00002cd0: 6465 6420 3d20 726f 6f74 5f69 7465 6d2e  ded = root_item.
-00002ce0: 6578 636c 7564 6564 0d0a 2020 2020 2020  excluded..      
-00002cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d00: 2020 2020 2020 6368 696c 642e 7365 745f        child.set_
-00002d10: 656e 6162 6c65 203d 2063 6f6d 702e 5f73  enable = comp._s
-00002d20: 6574 5f65 6e61 626c 650d 0a20 2020 2020  et_enable..     
-00002d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d40: 2020 2020 2020 2063 6869 6c64 2e67 6574         child.get
-00002d50: 5f65 6e61 626c 6520 3d20 636f 6d70 2e5f  _enable = comp._
-00002d60: 6765 745f 656e 6162 6c65 0d0a 2020 2020  get_enable..    
-00002d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d80: 2020 2020 2020 2020 726f 6f74 5f69 7465          root_ite
-00002d90: 6d2e 6170 7065 6e64 4368 696c 6428 6368  m.appendChild(ch
-00002da0: 696c 6429 0d0a 2020 2020 2020 2020 2020  ild)..          
-00002db0: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
-00002dc0: 6570 7469 6f6e 2061 7320 653a 0d0a 2020  eption as e:..  
-00002dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002de0: 2020 7072 696e 7428 6627 2020 7b74 7970    print(f'  {typ
-00002df0: 6528 6529 7d20 7b65 7d20 636f 6d6d 616e  e(e)} {e} comman
-00002e00: 643a 7b63 6f6d 702e 7265 6d6f 7465 5f63  d:{comp.remote_c
-00002e10: 6f6d 6d61 6e64 7d27 290d 0a20 2020 2020  ommand}')..     
-00002e20: 2020 2072 6574 7572 6e20 726f 6f74 5f69     return root_i
-00002e30: 7465 6d0d 0a                             tem..
+00002350: 2020 2020 2063 6869 6c64 2e6e 616d 6520       child.name 
+00002360: 3d20 6627 7b69 6e64 6578 7d27 0d0a 2020  = f'{index}'..  
+00002370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002380: 2020 2020 2020 2020 2020 6368 696c 642e            child.
+00002390: 636f 6d70 203d 2069 6e64 6578 0d0a 2020  comp = index..  
+000023a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023b0: 2020 2020 2020 2020 2020 6368 696c 642e            child.
+000023c0: 636f 6d70 5f74 7970 6520 3d20 496e 6465  comp_type = Inde
+000023d0: 780d 0a20 2020 2020 2020 2020 2020 2020  x..             
+000023e0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000023f0: 6869 6c64 2e65 7863 6c75 6465 6420 3d20  hild.excluded = 
+00002400: 726f 6f74 5f69 7465 6d2e 6578 636c 7564  root_item.exclud
+00002410: 6564 0d0a 2020 2020 2020 2020 2020 2020  ed..            
+00002420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002430: 6368 696c 642e 7365 745f 656e 6162 6c65  child.set_enable
+00002440: 203d 2072 6f6f 745f 6974 656d 2e73 6574   = root_item.set
+00002450: 5f65 6e61 626c 650d 0a20 2020 2020 2020  _enable..       
+00002460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002470: 2020 2020 2063 6869 6c64 2e67 6574 5f65       child.get_e
+00002480: 6e61 626c 6520 3d20 726f 6f74 5f69 7465  nable = root_ite
+00002490: 6d2e 6765 745f 656e 6162 6c65 0d0a 2020  m.get_enable..  
+000024a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024b0: 2020 2020 2020 2020 2020 726f 6f74 5f69            root_i
+000024c0: 7465 6d2e 6170 7065 6e64 4368 696c 6428  tem.appendChild(
+000024d0: 6368 696c 6429 0d0a 2020 2020 2020 2020  child)..        
+000024e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024f0: 2020 2020 696e 6465 7820 2b3d 2031 0d0a      index += 1..
+00002500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002510: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00002520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002530: 2020 2066 6f72 206b 6579 2069 6e20 636f     for key in co
+00002540: 6d70 2e69 6e64 6578 5f64 6963 743a 0d0a  mp.index_dict:..
+00002550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002560: 2020 2020 2020 2020 2020 2020 6368 696c              chil
+00002570: 6420 3d20 636c 732e 6c6f 6164 286b 6579  d = cls.load(key
+00002580: 2c20 726f 6f74 5f69 7465 6d2c 2073 6f72  , root_item, sor
+00002590: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
+000025a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025b0: 6368 696c 642e 6e61 6d65 203d 2066 277b  child.name = f'{
+000025c0: 6b65 797d 270d 0a20 2020 2020 2020 2020  key}'..         
+000025d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025e0: 2020 2063 6869 6c64 2e63 6f6d 7020 3d20     child.comp = 
+000025f0: 6b65 790d 0a20 2020 2020 2020 2020 2020  key..           
+00002600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002610: 2063 6869 6c64 2e63 6f6d 705f 7479 7065   child.comp_type
+00002620: 203d 2049 6e64 6578 0d0a 2020 2020 2020   = Index..      
+00002630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002640: 2020 2020 2020 6368 696c 642e 6578 6c75        child.exlu
+00002650: 6465 6420 3d20 726f 6f74 5f69 7465 6d2e  ded = root_item.
+00002660: 6578 636c 7564 6564 0d0a 2020 2020 2020  excluded..      
+00002670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002680: 2020 2020 2020 6368 696c 642e 7365 745f        child.set_
+00002690: 656e 6162 6c65 203d 2063 6f6d 702e 5f73  enable = comp._s
+000026a0: 6574 5f65 6e61 626c 650d 0a20 2020 2020  et_enable..     
+000026b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026c0: 2020 2020 2020 2063 6869 6c64 2e67 6574         child.get
+000026d0: 5f65 6e61 626c 6520 3d20 636f 6d70 2e5f  _enable = comp._
+000026e0: 6765 745f 656e 6162 6c65 0d0a 2020 2020  get_enable..    
+000026f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002700: 2020 2020 2020 2020 726f 6f74 5f69 7465          root_ite
+00002710: 6d2e 6170 7065 6e64 4368 696c 6428 6368  m.appendChild(ch
+00002720: 696c 6429 0d0a 2020 2020 2020 2020 2020  ild)..          
+00002730: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
+00002740: 6570 7469 6f6e 2061 7320 653a 0d0a 2020  eption as e:..  
+00002750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002760: 2020 7072 696e 7428 6627 2020 7b74 7970    print(f'  {typ
+00002770: 6528 6529 7d20 7b65 7d20 636f 6d6d 616e  e(e)} {e} comman
+00002780: 643a 7b63 6f6d 702e 7265 6d6f 7465 5f63  d:{comp.remote_c
+00002790: 6f6d 6d61 6e64 7d20 696e 6465 783a 207b  ommand} index: {
+000027a0: 696e 6465 787d 2729 0d0a 2020 2020 2020  index}')..      
+000027b0: 2020 7265 7475 726e 2072 6f6f 745f 6974    return root_it
+000027c0: 656d 0d0a                                em..
```

### Comparing `srsgui-0.2.15/srsgui/ui/commandtree/commandmodel.py` & `srsgui-0.2.9/srsgui/ui/commandtree/commandmodel.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,515 +1,490 @@
 00000000: 0d0a 696d 706f 7274 2074 696d 650d 0a69  ..import time..i
 00000010: 6d70 6f72 7420 6a73 6f6e 0d0a 696d 706f  mport json..impo
-00000020: 7274 2073 7973 0d0a 0d0a 6672 6f6d 2074  rt sys....from t
-00000030: 7970 696e 6720 696d 706f 7274 2041 6e79  yping import Any
-00000040: 2c20 4974 6572 6162 6c65 2c20 4c69 7374  , Iterable, List
-00000050: 2c20 4469 6374 2c20 556e 696f 6e0d 0a0d  , Dict, Union...
-00000060: 0a66 726f 6d20 7372 7367 7569 2e75 692e  .from srsgui.ui.
-00000070: 7174 2e51 7457 6964 6765 7473 2069 6d70  qt.QtWidgets imp
-00000080: 6f72 7420 5154 7265 6556 6965 772c 2051  ort QTreeView, Q
-00000090: 4170 706c 6963 6174 696f 6e2c 2051 4865  Application, QHe
-000000a0: 6164 6572 5669 6577 0d0a 6672 6f6d 2073  aderView..from s
-000000b0: 7273 6775 692e 7569 2e71 742e 5174 4775  rsgui.ui.qt.QtGu
-000000c0: 6920 696d 706f 7274 2051 4272 7573 682c  i import QBrush,
-000000d0: 2051 436f 6c6f 720d 0a66 726f 6d20 7372   QColor..from sr
-000000e0: 7367 7569 2e75 692e 7174 2e51 7443 6f72  sgui.ui.qt.QtCor
-000000f0: 6520 696d 706f 7274 2051 4162 7374 7261  e import QAbstra
-00000100: 6374 4974 656d 4d6f 6465 6c2c 2051 4d6f  ctItemModel, QMo
-00000110: 6465 6c49 6e64 6578 2c20 5c0d 0a20 2020  delIndex, \..   
-00000120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000130: 2020 2020 2020 2020 2020 2020 2051 4f62               QOb
-00000140: 6a65 6374 2c20 5174 2c20 5369 676e 616c  ject, Qt, Signal
-00000150: 0d0a 0d0a 6672 6f6d 2073 7273 6775 6920  ....from srsgui 
-00000160: 696d 706f 7274 2043 6f6d 706f 6e65 6e74  import Component
-00000170: 0d0a 0d0a 6672 6f6d 202e 636f 6d6d 616e  ....from .comman
-00000180: 6469 7465 6d20 696d 706f 7274 2043 6f6d  ditem import Com
-00000190: 6d61 6e64 4974 656d 2c20 496e 6465 780d  mandItem, Index.
-000001a0: 0a66 726f 6d20 2e63 6f6d 6d61 6e64 6465  .from .commandde
-000001b0: 6c65 6761 7465 2069 6d70 6f72 7420 436f  legate import Co
-000001c0: 6d6d 616e 6444 656c 6567 6174 650d 0a66  mmandDelegate..f
-000001d0: 726f 6d20 2e63 6f6d 6d61 6e64 6861 6e64  rom .commandhand
-000001e0: 6c65 7220 696d 706f 7274 2043 6f6d 6d61  ler import Comma
-000001f0: 6e64 4861 6e64 6c65 720d 0a0d 0a0d 0a63  ndHandler......c
-00000200: 6c61 7373 2043 6f6d 6d61 6e64 4d6f 6465  lass CommandMode
-00000210: 6c28 5141 6273 7472 6163 7449 7465 6d4d  l(QAbstractItemM
-00000220: 6f64 656c 293a 0d0a 2020 2020 2222 2220  odel):..    """ 
-00000230: 416e 2065 6469 7461 626c 6520 6d6f 6465  An editable mode
-00000240: 6c20 6f66 2043 6f6d 6d61 6e64 2061 6e64  l of Command and
-00000250: 2043 6f6d 706f 6e65 6e74 2022 2222 0d0a   Component """..
-00000260: 0d0a 2020 2020 2320 5369 676e 616c 2074  ..    # Signal t
-00000270: 6f20 7265 7175 6573 7420 746f 2070 726f  o request to pro
-00000280: 6365 7373 2061 2071 7565 7279 2074 6f20  cess a query to 
-00000290: 616e 206f 7574 7369 6465 2063 6f6d 6d61  an outside comma
-000002a0: 6e64 2070 726f 6365 7373 6f72 0d0a 2020  nd processor..  
-000002b0: 2020 7175 6572 795f 7265 7175 6573 7465    query_requeste
-000002c0: 6420 3d20 5369 676e 616c 2851 4d6f 6465  d = Signal(QMode
-000002d0: 6c49 6e64 6578 290d 0a0d 0a20 2020 2023  lIndex)....    #
-000002e0: 2053 6967 6e61 6c20 746f 2072 6571 7565   Signal to reque
-000002f0: 7374 2074 6f20 7072 6f63 6573 7320 6120  st to process a 
-00000300: 7365 7420 746f 2061 6e20 6f75 7473 6964  set to an outsid
-00000310: 6520 636f 6d6d 616e 6420 7072 6f63 6573  e command proces
-00000320: 736f 720d 0a20 2020 2073 6574 5f72 6571  sor..    set_req
-00000330: 7565 7374 6564 203d 2053 6967 6e61 6c28  uested = Signal(
-00000340: 7475 706c 6529 0d0a 0d0a 2020 2020 2320  tuple)....    # 
-00000350: 5369 676e 616c 2074 6f20 6469 7370 6c61  Signal to displa
-00000360: 7920 6675 6c6c 2050 7974 686f 6e20 636f  y full Python co
-00000370: 6d6d 616e 6420 746f 2043 6f6d 6d61 6e64  mmand to Command
-00000380: 5465 726d 696e 616c 0d0a 2020 2020 7365  Terminal..    se
-00000390: 745f 636f 6d6d 616e 645f 7365 6e74 203d  t_command_sent =
-000003a0: 2053 6967 6e61 6c28 7374 722c 2073 7472   Signal(str, str
-000003b0: 290d 0a0d 0a20 2020 2064 6566 205f 5f69  )....    def __i
-000003c0: 6e69 745f 5f28 7365 6c66 2c20 7061 7265  nit__(self, pare
-000003d0: 6e74 3a20 514f 626a 6563 7420 3d20 4e6f  nt: QObject = No
-000003e0: 6e65 293a 0d0a 2020 2020 2020 2020 7375  ne):..        su
-000003f0: 7065 7228 292e 5f5f 696e 6974 5f5f 2870  per().__init__(p
-00000400: 6172 656e 7429 0d0a 0d0a 2020 2020 2020  arent)....      
-00000410: 2020 7365 6c66 2e73 686f 775f 7261 775f    self.show_raw_
-00000420: 7265 6d6f 7465 5f63 6f6d 6d61 6e64 203d  remote_command =
-00000430: 2054 7275 650d 0a0d 0a20 2020 2020 2020   True....       
-00000440: 2073 656c 662e 5f72 6f6f 7449 7465 6d20   self._rootItem 
-00000450: 3d20 436f 6d6d 616e 6449 7465 6d28 290d  = CommandItem().
-00000460: 0a20 2020 2020 2020 2073 656c 662e 5f68  .        self._h
-00000470: 6561 6465 7273 203d 2028 2220 2063 6f6d  eaders = ("  com
-00000480: 6d61 6e64 2020 222c 2022 2020 7661 6c75  mand  ", "  valu
-00000490: 6520 2022 290d 0a0d 0a20 2020 2064 6566  e  ")....    def
-000004a0: 2068 616e 646c 655f 636f 6d6d 616e 6428   handle_command(
-000004b0: 7365 6c66 2c20 636d 645f 7475 706c 6529  self, cmd_tuple)
-000004c0: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
-000004d0: 2020 2020 2020 2020 4f75 7473 6964 6520          Outside 
-000004e0: 636f 6d6d 616e 6420 7072 6f63 6573 736f  command processo
-000004f0: 7220 6361 6c6c 7320 7468 6973 2073 6c6f  r calls this slo
-00000500: 7420 6f6e 6365 2061 2063 6f6d 6d61 6e64  t once a command
-00000510: 2069 7320 7072 6f63 6573 7365 640d 0a20   is processed.. 
-00000520: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00000530: 2020 2020 696e 6465 7820 3d20 636d 645f      index = cmd_
-00000540: 7475 706c 655b 305d 0d0a 2020 2020 2020  tuple[0]..      
-00000550: 2020 7661 6c75 6520 3d20 636d 645f 7475    value = cmd_tu
-00000560: 706c 655b 315d 0d0a 2020 2020 2020 2020  ple[1]..        
-00000570: 6368 616e 6765 6420 3d20 636d 645f 7475  changed = cmd_tu
-00000580: 706c 655b 325d 0d0a 2020 2020 2020 2020  ple[2]..        
-00000590: 6966 2063 6861 6e67 6564 3a0d 0a20 2020  if changed:..   
-000005a0: 2020 2020 2020 2020 2073 656c 662e 6461           self.da
-000005b0: 7461 4368 616e 6765 642e 656d 6974 2869  taChanged.emit(i
-000005c0: 6e64 6578 2c20 696e 6465 782c 205b 5174  ndex, index, [Qt
-000005d0: 2e49 7465 6d44 6174 6152 6f6c 652c 2051  .ItemDataRole, Q
-000005e0: 742e 4564 6974 526f 6c65 5d29 0d0a 0d0a  t.EditRole])....
-000005f0: 2020 2020 6465 6620 636c 6561 7228 7365      def clear(se
-00000600: 6c66 293a 0d0a 2020 2020 2020 2020 2222  lf):..        ""
-00000610: 2220 436c 6561 7220 6461 7461 2066 726f  " Clear data fro
-00000620: 6d20 7468 6520 6d6f 6465 6c20 2222 220d  m the model """.
-00000630: 0a20 2020 2020 2020 2073 656c 662e 6c6f  .        self.lo
-00000640: 6164 2843 6f6d 706f 6e65 6e74 2829 290d  ad(Component()).
-00000650: 0a0d 0a20 2020 2064 6566 206c 6f61 6428  ...    def load(
-00000660: 7365 6c66 2c20 646f 6375 6d65 6e74 3a20  self, document: 
-00000670: 436f 6d70 6f6e 656e 7429 3a0d 0a20 2020  Component):..   
-00000680: 2020 2020 2022 2222 4c6f 6164 206d 6f64       """Load mod
-00000690: 656c 2066 726f 6d20 6120 6e65 7374 6564  el from a nested
-000006a0: 2064 6963 7469 6f6e 6172 7920 7265 7475   dictionary retu
-000006b0: 726e 6564 2062 7920 6a73 6f6e 2e6c 6f61  rned by json.loa
-000006c0: 6473 2829 0d0a 0d0a 2020 2020 2020 2020  ds()....        
-000006d0: 4172 6775 6d65 6e74 733a 0d0a 2020 2020  Arguments:..    
-000006e0: 2020 2020 2020 2020 646f 6375 6d65 6e74          document
-000006f0: 2028 6469 6374 293a 204a 534f 4e2d 636f   (dict): JSON-co
-00000700: 6d70 6174 6962 6c65 2064 6963 7469 6f6e  mpatible diction
-00000710: 6172 790d 0a20 2020 2020 2020 2022 2222  ary..        """
-00000720: 0d0a 0d0a 2020 2020 2020 2020 6173 7365  ....        asse
-00000730: 7274 2069 7369 6e73 7461 6e63 6528 0d0a  rt isinstance(..
-00000740: 2020 2020 2020 2020 2020 2020 646f 6375              docu
-00000750: 6d65 6e74 2c20 436f 6d70 6f6e 656e 740d  ment, Component.
-00000760: 0a20 2020 2020 2020 2029 2c20 2260 646f  .        ), "`do
-00000770: 6375 6d65 6e74 6020 6d75 7374 2062 6520  cument` must be 
-00000780: 6120 436f 6d70 6f6e 656e 742c 2022 2066  a Component, " f
-00000790: 226e 6f74 207b 7479 7065 2864 6f63 756d  "not {type(docum
-000007a0: 656e 7429 7d22 0d0a 0d0a 2020 2020 2020  ent)}"....      
-000007b0: 2020 7365 6c66 2e62 6567 696e 5265 7365    self.beginRese
-000007c0: 744d 6f64 656c 2829 0d0a 0d0a 2020 2020  tModel()....    
-000007d0: 2020 2020 7365 6c66 2e5f 726f 6f74 4974      self._rootIt
-000007e0: 656d 203d 2043 6f6d 6d61 6e64 4974 656d  em = CommandItem
-000007f0: 2e6c 6f61 6428 646f 6375 6d65 6e74 290d  .load(document).
-00000800: 0a20 2020 2020 2020 2073 656c 662e 5f72  .        self._r
-00000810: 6f6f 7449 7465 6d2e 7661 6c75 655f 7479  ootItem.value_ty
-00000820: 7065 203d 2074 7970 6528 646f 6375 6d65  pe = type(docume
-00000830: 6e74 290d 0a0d 0a20 2020 2020 2020 2073  nt)....        s
-00000840: 656c 662e 656e 6452 6573 6574 4d6f 6465  elf.endResetMode
-00000850: 6c28 290d 0a20 2020 2020 2020 2072 6574  l()..        ret
-00000860: 7572 6e20 5472 7565 0d0a 0d0a 2020 2020  urn True....    
-00000870: 6465 6620 6461 7461 2873 656c 662c 2069  def data(self, i
-00000880: 6e64 6578 3a20 514d 6f64 656c 496e 6465  ndex: QModelInde
-00000890: 782c 2072 6f6c 653a 2051 742e 4974 656d  x, role: Qt.Item
-000008a0: 4461 7461 526f 6c65 2920 2d3e 2041 6e79  DataRole) -> Any
-000008b0: 3a0d 0a20 2020 2020 2020 2022 2222 4f76  :..        """Ov
-000008c0: 6572 7269 6465 2066 726f 6d20 5141 6273  erride from QAbs
-000008d0: 7472 6163 7449 7465 6d4d 6f64 656c 0d0a  tractItemModel..
-000008e0: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-000008f0: 2064 6174 6120 6672 6f6d 2061 6e20 6974   data from an it
-00000900: 656d 2061 6363 6f72 6469 6e67 2069 6e64  em according ind
-00000910: 6578 2061 6e64 2072 6f6c 650d 0a20 2020  ex and role..   
-00000920: 2020 2020 2022 2222 0d0a 0d0a 2020 2020       """....    
-00000930: 2020 2020 6966 206e 6f74 2069 6e64 6578      if not index
-00000940: 2e69 7356 616c 6964 2829 3a0d 0a20 2020  .isValid():..   
-00000950: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00000960: 4e6f 6e65 0d0a 0d0a 2020 2020 2020 2020  None....        
-00000970: 6966 2072 6f6c 6520 3d3d 2051 742e 4469  if role == Qt.Di
-00000980: 7370 6c61 7952 6f6c 653a 0d0a 2020 2020  splayRole:..    
-00000990: 2020 2020 2020 2020 6966 2069 6e64 6578          if index
-000009a0: 2e63 6f6c 756d 6e28 2920 3d3d 2030 3a0d  .column() == 0:.
-000009b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000009c0: 2069 7465 6d20 3d20 696e 6465 782e 696e   item = index.in
-000009d0: 7465 726e 616c 506f 696e 7465 7228 290d  ternalPointer().
-000009e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000009f0: 206e 616d 6520 3d20 6974 656d 2e6e 616d   name = item.nam
-00000a00: 650d 0a0d 0a20 2020 2020 2020 2020 2020  e....           
-00000a10: 2020 2020 2069 6620 7365 6c66 2e73 686f       if self.sho
-00000a20: 775f 7261 775f 7265 6d6f 7465 5f63 6f6d  w_raw_remote_com
-00000a30: 6d61 6e64 3a0d 0a20 2020 2020 2020 2020  mand:..         
-00000a40: 2020 2020 2020 2020 2020 206e 616d 6520             name 
-00000a50: 2b3d 2066 2720 3c7b 6974 656d 2e72 6177  += f' <{item.raw
-00000a60: 5f72 656d 6f74 655f 636f 6d6d 616e 647d  _remote_command}
-00000a70: 3e27 2069 6620 6974 656d 2e72 6177 5f72  >' if item.raw_r
-00000a80: 656d 6f74 655f 636f 6d6d 616e 6420 656c  emote_command el
-00000a90: 7365 2027 270d 0a0d 0a20 2020 2020 2020  se ''....       
-00000aa0: 2020 2020 2020 2020 206e 616d 6520 2b3d           name +=
-00000ab0: 2027 205b 4d5d 2720 6966 2069 7465 6d2e   ' [M]' if item.
-00000ac0: 6973 5f6d 6574 686f 6420 656c 7365 2027  is_method else '
-00000ad0: 270d 0a20 2020 2020 2020 2020 2020 2020  '..             
-00000ae0: 2020 206e 616d 6520 2b3d 2027 205b 4558     name += ' [EX
-00000af0: 5d27 2069 6620 6974 656d 2e65 7863 6c75  ]' if item.exclu
-00000b00: 6465 6420 656c 7365 2027 270d 0a20 2020  ded else ''..   
-00000b10: 2020 2020 2020 2020 2020 2020 206e 616d               nam
-00000b20: 6520 2b3d 2027 205b 534f 5d27 2069 6620  e += ' [SO]' if 
-00000b30: 6974 656d 2e73 6574 5f65 6e61 626c 6520  item.set_enable 
-00000b40: 616e 6420 6e6f 7420 6974 656d 2e67 6574  and not item.get
-00000b50: 5f65 6e61 626c 6520 656c 7365 2027 270d  _enable else ''.
-00000b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000b70: 206e 616d 6520 2b3d 2027 205b 514f 5d27   name += ' [QO]'
-00000b80: 2069 6620 6974 656d 2e67 6574 5f65 6e61   if item.get_ena
-00000b90: 626c 6520 616e 6420 6e6f 7420 6974 656d  ble and not item
-00000ba0: 2e73 6574 5f65 6e61 626c 6520 656c 7365  .set_enable else
-00000bb0: 2027 270d 0a20 2020 2020 2020 2020 2020   ''..           
-00000bc0: 2020 2020 2072 6574 7572 6e20 6e61 6d65       return name
-00000bd0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00000be0: 6966 2069 6e64 6578 2e63 6f6c 756d 6e28  if index.column(
-00000bf0: 2920 3d3d 2031 3a0d 0a20 2020 2020 2020  ) == 1:..       
-00000c00: 2020 2020 2020 2020 2069 7465 6d20 3d20           item = 
-00000c10: 696e 6465 782e 696e 7465 726e 616c 506f  index.internalPo
-00000c20: 696e 7465 7228 290d 0a20 2020 2020 2020  inter()..       
-00000c30: 2020 2020 2020 2020 2073 656c 662e 7175           self.qu
-00000c40: 6572 795f 7265 7175 6573 7465 642e 656d  ery_requested.em
-00000c50: 6974 2869 6e64 6578 290d 0a20 2020 2020  it(index)..     
-00000c60: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00000c70: 6e20 6974 656d 2e67 6574 5f66 6f72 6d61  n item.get_forma
-00000c80: 7474 6564 5f76 616c 7565 2829 0d0a 0d0a  tted_value()....
-00000c90: 2020 2020 2020 2020 656c 6966 2072 6f6c          elif rol
-00000ca0: 6520 3d3d 2051 742e 4564 6974 526f 6c65  e == Qt.EditRole
-00000cb0: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-00000cc0: 6620 696e 6465 782e 636f 6c75 6d6e 2829  f index.column()
-00000cd0: 203d 3d20 313a 0d0a 2020 2020 2020 2020   == 1:..        
-00000ce0: 2020 2020 2020 2020 6974 656d 203d 2069          item = i
-00000cf0: 6e64 6578 2e69 6e74 6572 6e61 6c50 6f69  ndex.internalPoi
-00000d00: 6e74 6572 2829 0d0a 2020 2020 2020 2020  nter()..        
-00000d10: 2020 2020 2020 2020 7365 6c66 2e71 7565          self.que
-00000d20: 7279 5f72 6571 7565 7374 6564 2e65 6d69  ry_requested.emi
-00000d30: 7428 696e 6465 7829 0d0a 2020 2020 2020  t(index)..      
-00000d40: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00000d50: 2069 7465 6d2e 7661 6c75 650d 0a0d 0a20   item.value.... 
-00000d60: 2020 2020 2020 2065 6c69 6620 726f 6c65         elif role
-00000d70: 203d 3d20 5174 2e42 6163 6b67 726f 756e   == Qt.Backgroun
-00000d80: 6452 6f6c 653a 0d0a 2020 2020 2020 2020  dRole:..        
-00000d90: 2020 2020 6974 656d 203d 2069 6e64 6578      item = index
-00000da0: 2e69 6e74 6572 6e61 6c50 6f69 6e74 6572  .internalPointer
-00000db0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00000dc0: 6966 2069 7465 6d2e 636f 6d70 5f74 7970  if item.comp_typ
-00000dd0: 6520 213d 2049 6e64 6578 2061 6e64 2069  e != Index and i
-00000de0: 7373 7562 636c 6173 7328 6974 656d 2e63  ssubclass(item.c
-00000df0: 6f6d 705f 7479 7065 2c20 436f 6d70 6f6e  omp_type, Compon
-00000e00: 656e 7429 3a0d 0a20 2020 2020 2020 2020  ent):..         
-00000e10: 2020 2020 2020 2072 6574 7572 6e20 5142         return QB
-00000e20: 7275 7368 2851 436f 6c6f 7228 3234 332c  rush(QColor(243,
-00000e30: 2032 3330 2c20 3232 3529 290d 0a20 2020   230, 225))..   
-00000e40: 2020 2020 2020 2020 2069 6620 6974 656d           if item
-00000e50: 2e72 6f77 2829 2025 2032 203d 3d20 303a  .row() % 2 == 0:
-00000e60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000e70: 2020 7265 7475 726e 2051 4272 7573 6828    return QBrush(
-00000e80: 5143 6f6c 6f72 2832 3430 2c20 3234 302c  QColor(240, 240,
-00000e90: 2032 3533 2929 0d0a 0d0a 2020 2020 2020   253))....      
-00000ea0: 2020 656c 6966 2072 6f6c 6520 3d3d 2051    elif role == Q
-00000eb0: 742e 546f 6f6c 5469 7052 6f6c 653a 0d0a  t.ToolTipRole:..
-00000ec0: 2020 2020 2020 2020 2020 2020 6974 656d              item
-00000ed0: 203d 2069 6e64 6578 2e69 6e74 6572 6e61   = index.interna
-00000ee0: 6c50 6f69 6e74 6572 2829 0d0a 2020 2020  lPointer()..    
-00000ef0: 2020 2020 2020 2020 6966 2069 7465 6d2e          if item.
-00000f00: 6973 5f6d 6574 686f 6420 6f72 2069 7373  is_method or iss
-00000f10: 7562 636c 6173 7328 6974 656d 2e63 6f6d  ubclass(item.com
-00000f20: 705f 7479 7065 2c20 436f 6d70 6f6e 656e  p_type, Componen
-00000f30: 7429 3a0d 0a20 2020 2020 2020 2020 2020  t):..           
-00000f40: 2020 2020 2069 6620 6861 7361 7474 7228       if hasattr(
-00000f50: 6974 656d 2e63 6f6d 702c 2027 5f5f 646f  item.comp, '__do
-00000f60: 635f 5f27 2920 616e 6420 696e 6465 782e  c__') and index.
-00000f70: 636f 6c75 6d6e 2829 203d 3d20 303a 0d0a  column() == 0:..
-00000f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f90: 2020 2020 7265 7475 726e 2069 7465 6d2e      return item.
-00000fa0: 636f 6d70 2e5f 5f64 6f63 5f5f 0d0a 0d0a  comp.__doc__....
-00000fb0: 2020 2020 6465 6620 7365 7444 6174 6128      def setData(
-00000fc0: 7365 6c66 2c20 696e 6465 783a 2051 4d6f  self, index: QMo
-00000fd0: 6465 6c49 6e64 6578 2c20 7661 6c75 653a  delIndex, value:
-00000fe0: 2041 6e79 2c20 726f 6c65 3a20 5174 2e49   Any, role: Qt.I
-00000ff0: 7465 6d44 6174 6152 6f6c 6529 3a0d 0a20  temDataRole):.. 
-00001000: 2020 2020 2020 2022 2222 4f76 6572 7269         """Overri
-00001010: 6465 2066 726f 6d20 5141 6273 7472 6163  de from QAbstrac
-00001020: 7449 7465 6d4d 6f64 656c 0d0a 0d0a 2020  tItemModel....  
-00001030: 2020 2020 2020 5365 7420 436f 6d6d 616e        Set Comman
-00001040: 6449 7465 6d20 6163 636f 7264 696e 6720  dItem according 
-00001050: 746f 2069 6e64 6578 2061 6e64 2072 6f6c  to index and rol
-00001060: 650d 0a0d 0a20 2020 2020 2020 2041 7267  e....        Arg
-00001070: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00001080: 696e 6465 7820 2851 4d6f 6465 6c49 6e64  index (QModelInd
-00001090: 6578 290d 0a20 2020 2020 2020 2020 2020  ex)..           
-000010a0: 2076 616c 7565 2028 416e 7929 0d0a 2020   value (Any)..  
-000010b0: 2020 2020 2020 2020 2020 726f 6c65 2028            role (
-000010c0: 5174 2e49 7465 6d44 6174 6152 6f6c 6529  Qt.ItemDataRole)
-000010d0: 0d0a 2020 2020 2020 2020 2222 220d 0a0d  ..        """...
-000010e0: 0a20 2020 2020 2020 2069 6620 726f 6c65  .        if role
-000010f0: 203d 3d20 5174 2e45 6469 7452 6f6c 653a   == Qt.EditRole:
-00001100: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00001110: 2069 6e64 6578 2e63 6f6c 756d 6e28 2920   index.column() 
-00001120: 3d3d 2031 3a0d 0a20 2020 2020 2020 2020  == 1:..         
-00001130: 2020 2020 2020 2069 7465 6d20 3d20 696e         item = in
-00001140: 6465 782e 696e 7465 726e 616c 506f 696e  dex.internalPoin
-00001150: 7465 7228 290d 0a20 2020 2020 2020 2020  ter()..         
-00001160: 2020 2020 2020 2073 656c 662e 7365 745f         self.set_
-00001170: 7265 7175 6573 7465 642e 656d 6974 2828  requested.emit((
-00001180: 696e 6465 782c 2076 616c 7565 2929 0d0a  index, value))..
-00001190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011a0: 7365 6e74 5f63 6f6d 6d61 6e64 203d 2069  sent_command = i
-000011b0: 7465 6d2e 636f 6e73 7472 7563 745f 7365  tem.construct_se
-000011c0: 745f 636f 6d6d 616e 645f 7374 7269 6e67  t_command_string
-000011d0: 2876 616c 7565 290d 0a20 2020 2020 2020  (value)..       
-000011e0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-000011f0: 745f 636f 6d6d 616e 645f 7365 6e74 2e65  t_command_sent.e
-00001200: 6d69 7428 7365 6e74 5f63 6f6d 6d61 6e64  mit(sent_command
-00001210: 2c20 4e6f 6e65 290d 0a20 2020 2020 2020  , None)..       
-00001220: 2020 2020 2020 2020 2023 2069 7465 6d2e           # item.
-00001230: 7365 745f 7661 6c75 6528 7661 6c75 6529  set_value(value)
-00001240: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001250: 2020 2373 656c 662e 6461 7461 4368 616e    #self.dataChan
-00001260: 6765 642e 656d 6974 2869 6e64 6578 2c20  ged.emit(index, 
-00001270: 696e 6465 782c 205b 5174 2e45 6469 7452  index, [Qt.EditR
-00001280: 6f6c 655d 290d 0a20 2020 2020 2020 2020  ole])..         
-00001290: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-000012a0: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
-000012b0: 7265 7475 726e 2046 616c 7365 0d0a 2020  return False..  
-000012c0: 2020 0d0a 2020 2020 6465 6620 6865 6164    ..    def head
-000012d0: 6572 4461 7461 2873 656c 662c 2073 6563  erData(self, sec
-000012e0: 7469 6f6e 3a20 696e 742c 206f 7269 656e  tion: int, orien
-000012f0: 7461 7469 6f6e 3a20 5174 2e4f 7269 656e  tation: Qt.Orien
-00001300: 7461 7469 6f6e 2c0d 0a20 2020 2020 2020  tation,..       
-00001310: 2020 2020 2020 2020 2020 2020 726f 6c65              role
-00001320: 3a20 5174 2e49 7465 6d44 6174 6152 6f6c  : Qt.ItemDataRol
-00001330: 6529 3a0d 0a20 2020 2020 2020 2022 2222  e):..        """
-00001340: 4f76 6572 7269 6465 2066 726f 6d20 5141  Override from QA
-00001350: 6273 7472 6163 7449 7465 6d4d 6f64 656c  bstractItemModel
-00001360: 0d0a 0d0a 2020 2020 2020 2020 6974 2072  ....        it r
-00001370: 6574 7572 6e73 206f 6e6c 7920 6461 7461  eturns only data
-00001380: 2066 6f72 2063 6f6c 756d 6e73 2028 6f72   for columns (or
-00001390: 6965 6e74 6174 696f 6e20 3d20 486f 7269  ientation = Hori
-000013a0: 7a6f 6e74 616c 290d 0a20 2020 2020 2020  zontal)..       
-000013b0: 2022 2222 0d0a 2020 2020 2020 2020 6966   """..        if
-000013c0: 2072 6f6c 6520 213d 2051 742e 4469 7370   role != Qt.Disp
-000013d0: 6c61 7952 6f6c 653a 0d0a 2020 2020 2020  layRole:..      
-000013e0: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-000013f0: 650d 0a0d 0a20 2020 2020 2020 2069 6620  e....        if 
-00001400: 6f72 6965 6e74 6174 696f 6e20 3d3d 2051  orientation == Q
-00001410: 742e 486f 7269 7a6f 6e74 616c 3a0d 0a20  t.Horizontal:.. 
-00001420: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00001430: 6e20 7365 6c66 2e5f 6865 6164 6572 735b  n self._headers[
-00001440: 7365 6374 696f 6e5d 0d0a 0d0a 2020 2020  section]....    
-00001450: 6465 6620 696e 6465 7828 7365 6c66 2c20  def index(self, 
-00001460: 726f 773a 2069 6e74 2c20 636f 6c75 6d6e  row: int, column
-00001470: 3a20 696e 742c 2070 6172 656e 743d 514d  : int, parent=QM
-00001480: 6f64 656c 496e 6465 7828 2929 202d 3e20  odelIndex()) -> 
-00001490: 514d 6f64 656c 496e 6465 783a 0d0a 2020  QModelIndex:..  
-000014a0: 2020 2020 2020 2222 224f 7665 7272 6964        """Overrid
-000014b0: 6520 6672 6f6d 2051 4162 7374 7261 6374  e from QAbstract
-000014c0: 4974 656d 4d6f 6465 6c0d 0a0d 0a20 2020  ItemModel....   
-000014d0: 2020 2020 2052 6574 7572 6e20 696e 6465       Return inde
-000014e0: 7820 6163 636f 7264 696e 6720 726f 772c  x according row,
-000014f0: 2063 6f6c 756d 6e20 616e 6420 7061 7265   column and pare
-00001500: 6e74 0d0a 2020 2020 2020 2020 2222 220d  nt..        """.
-00001510: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00001520: 7365 6c66 2e68 6173 496e 6465 7828 726f  self.hasIndex(ro
-00001530: 772c 2063 6f6c 756d 6e2c 2070 6172 656e  w, column, paren
-00001540: 7429 3a0d 0a20 2020 2020 2020 2020 2020  t):..           
-00001550: 2072 6574 7572 6e20 514d 6f64 656c 496e   return QModelIn
-00001560: 6465 7828 290d 0a0d 0a20 2020 2020 2020  dex()....       
-00001570: 2069 6620 6e6f 7420 7061 7265 6e74 2e69   if not parent.i
-00001580: 7356 616c 6964 2829 3a0d 0a20 2020 2020  sValid():..     
-00001590: 2020 2020 2020 2070 6172 656e 7449 7465         parentIte
-000015a0: 6d20 3d20 7365 6c66 2e5f 726f 6f74 4974  m = self._rootIt
-000015b0: 656d 0d0a 2020 2020 2020 2020 656c 7365  em..        else
-000015c0: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
-000015d0: 6172 656e 7449 7465 6d20 3d20 7061 7265  arentItem = pare
-000015e0: 6e74 2e69 6e74 6572 6e61 6c50 6f69 6e74  nt.internalPoint
-000015f0: 6572 2829 0d0a 0d0a 2020 2020 2020 2020  er()....        
-00001600: 6368 696c 6449 7465 6d20 3d20 7061 7265  childItem = pare
-00001610: 6e74 4974 656d 2e63 6869 6c64 2872 6f77  ntItem.child(row
-00001620: 290d 0a20 2020 2020 2020 2069 6620 6368  )..        if ch
-00001630: 696c 6449 7465 6d3a 0d0a 2020 2020 2020  ildItem:..      
-00001640: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00001650: 662e 6372 6561 7465 496e 6465 7828 726f  f.createIndex(ro
-00001660: 772c 2063 6f6c 756d 6e2c 2063 6869 6c64  w, column, child
-00001670: 4974 656d 290d 0a20 2020 2020 2020 2065  Item)..        e
-00001680: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00001690: 2020 7265 7475 726e 2051 4d6f 6465 6c49    return QModelI
-000016a0: 6e64 6578 2829 0d0a 0d0a 2020 2020 6465  ndex()....    de
-000016b0: 6620 7061 7265 6e74 2873 656c 662c 2069  f parent(self, i
-000016c0: 6e64 6578 3a20 514d 6f64 656c 496e 6465  ndex: QModelInde
-000016d0: 7829 202d 3e20 514d 6f64 656c 496e 6465  x) -> QModelInde
-000016e0: 783a 0d0a 2020 2020 2020 2020 2222 224f  x:..        """O
-000016f0: 7665 7272 6964 6520 6672 6f6d 2051 4162  verride from QAb
-00001700: 7374 7261 6374 4974 656d 4d6f 6465 6c0d  stractItemModel.
-00001710: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00001720: 6e20 7061 7265 6e74 2069 6e64 6578 206f  n parent index o
-00001730: 6620 696e 6465 780d 0a20 2020 2020 2020  f index..       
-00001740: 2022 2222 0d0a 0d0a 2020 2020 2020 2020   """....        
-00001750: 6966 206e 6f74 2069 6e64 6578 2e69 7356  if not index.isV
-00001760: 616c 6964 2829 3a0d 0a20 2020 2020 2020  alid():..       
-00001770: 2020 2020 2072 6574 7572 6e20 514d 6f64       return QMod
-00001780: 656c 496e 6465 7828 290d 0a0d 0a20 2020  elIndex()....   
-00001790: 2020 2020 2063 6869 6c64 4974 656d 203d       childItem =
-000017a0: 2069 6e64 6578 2e69 6e74 6572 6e61 6c50   index.internalP
-000017b0: 6f69 6e74 6572 2829 0d0a 2020 2020 2020  ointer()..      
-000017c0: 2020 7061 7265 6e74 4974 656d 203d 2063    parentItem = c
-000017d0: 6869 6c64 4974 656d 2e70 6172 656e 7428  hildItem.parent(
-000017e0: 290d 0a0d 0a20 2020 2020 2020 2069 6620  )....        if 
-000017f0: 7061 7265 6e74 4974 656d 203d 3d20 7365  parentItem == se
-00001800: 6c66 2e5f 726f 6f74 4974 656d 3a0d 0a20  lf._rootItem:.. 
-00001810: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00001820: 6e20 514d 6f64 656c 496e 6465 7828 290d  n QModelIndex().
-00001830: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
-00001840: 6e20 7365 6c66 2e63 7265 6174 6549 6e64  n self.createInd
-00001850: 6578 2870 6172 656e 7449 7465 6d2e 726f  ex(parentItem.ro
-00001860: 7728 292c 2030 2c20 7061 7265 6e74 4974  w(), 0, parentIt
-00001870: 656d 290d 0a0d 0a20 2020 2064 6566 2072  em)....    def r
-00001880: 6f77 436f 756e 7428 7365 6c66 2c20 7061  owCount(self, pa
-00001890: 7265 6e74 3d51 4d6f 6465 6c49 6e64 6578  rent=QModelIndex
-000018a0: 2829 293a 0d0a 2020 2020 2020 2020 2222  ()):..        ""
-000018b0: 224f 7665 7272 6964 6520 6672 6f6d 2051  "Override from Q
-000018c0: 4162 7374 7261 6374 4974 656d 4d6f 6465  AbstractItemMode
-000018d0: 6c0d 0a0d 0a20 2020 2020 2020 2052 6574  l....        Ret
-000018e0: 7572 6e20 726f 7720 636f 756e 7420 6672  urn row count fr
-000018f0: 6f6d 2070 6172 656e 7420 696e 6465 780d  om parent index.
-00001900: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00001910: 2020 2020 2020 6966 2070 6172 656e 742e        if parent.
-00001920: 636f 6c75 6d6e 2829 203e 2030 3a0d 0a20  column() > 0:.. 
-00001930: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00001940: 6e20 300d 0a0d 0a20 2020 2020 2020 2069  n 0....        i
-00001950: 6620 6e6f 7420 7061 7265 6e74 2e69 7356  f not parent.isV
-00001960: 616c 6964 2829 3a0d 0a20 2020 2020 2020  alid():..       
-00001970: 2020 2020 2070 6172 656e 7449 7465 6d20       parentItem 
-00001980: 3d20 7365 6c66 2e5f 726f 6f74 4974 656d  = self._rootItem
-00001990: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-000019a0: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
-000019b0: 656e 7449 7465 6d20 3d20 7061 7265 6e74  entItem = parent
-000019c0: 2e69 6e74 6572 6e61 6c50 6f69 6e74 6572  .internalPointer
-000019d0: 2829 0d0a 0d0a 2020 2020 2020 2020 7265  ()....        re
-000019e0: 7475 726e 2070 6172 656e 7449 7465 6d2e  turn parentItem.
-000019f0: 6368 696c 6443 6f75 6e74 2829 0d0a 0d0a  childCount()....
-00001a00: 2020 2020 6465 6620 636f 6c75 6d6e 436f      def columnCo
-00001a10: 756e 7428 7365 6c66 2c20 7061 7265 6e74  unt(self, parent
-00001a20: 3d51 4d6f 6465 6c49 6e64 6578 2829 293a  =QModelIndex()):
-00001a30: 0d0a 2020 2020 2020 2020 2222 224f 7665  ..        """Ove
-00001a40: 7272 6964 6520 6672 6f6d 2051 4162 7374  rride from QAbst
-00001a50: 7261 6374 4974 656d 4d6f 6465 6c0d 0a0d  ractItemModel...
-00001a60: 0a20 2020 2020 2020 2052 6574 7572 6e20  .        Return 
-00001a70: 636f 6c75 6d6e 206e 756d 6265 722e 2046  column number. F
-00001a80: 6f72 2074 6865 206d 6f64 656c 2c20 6974  or the model, it
-00001a90: 2061 6c77 6179 7320 7265 7475 726e 2032   always return 2
-00001aa0: 2063 6f6c 756d 6e73 0d0a 2020 2020 2020   columns..      
-00001ab0: 2020 2222 220d 0a20 2020 2020 2020 2072    """..        r
-00001ac0: 6574 7572 6e20 320d 0a0d 0a20 2020 2064  eturn 2....    d
-00001ad0: 6566 2066 6c61 6773 2873 656c 662c 2069  ef flags(self, i
-00001ae0: 6e64 6578 3a20 514d 6f64 656c 496e 6465  ndex: QModelInde
-00001af0: 7829 202d 3e20 5174 2e49 7465 6d46 6c61  x) -> Qt.ItemFla
-00001b00: 6773 3a0d 0a20 2020 2020 2020 2022 2222  gs:..        """
-00001b10: 4f76 6572 7269 6465 2066 726f 6d20 5141  Override from QA
-00001b20: 6273 7472 6163 7449 7465 6d4d 6f64 656c  bstractItemModel
-00001b30: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
-00001b40: 726e 2066 6c61 6773 206f 6620 696e 6465  rn flags of inde
-00001b50: 780d 0a20 2020 2020 2020 2022 2222 0d0a  x..        """..
-00001b60: 2020 2020 2020 2020 666c 6167 7320 3d20          flags = 
-00001b70: 7375 7065 7228 436f 6d6d 616e 644d 6f64  super(CommandMod
-00001b80: 656c 2c20 7365 6c66 292e 666c 6167 7328  el, self).flags(
-00001b90: 696e 6465 7829 0d0a 0d0a 2020 2020 2020  index)....      
-00001ba0: 2020 6966 2069 6e64 6578 2e63 6f6c 756d    if index.colum
-00001bb0: 6e28 2920 3d3d 2031 2061 6e64 2073 656c  n() == 1 and sel
-00001bc0: 662e 6973 5f69 7465 6d5f 6564 6974 6162  f.is_item_editab
-00001bd0: 6c65 2869 6e64 6578 293a 0d0a 2020 2020  le(index):..    
-00001be0: 2020 2020 2020 2020 7265 7475 726e 2051          return Q
-00001bf0: 742e 4974 656d 4973 4564 6974 6162 6c65  t.ItemIsEditable
-00001c00: 207c 2066 6c61 6773 0d0a 2020 2020 2020   | flags..      
-00001c10: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00001c20: 2020 2020 2072 6574 7572 6e20 666c 6167       return flag
-00001c30: 730d 0a0d 0a20 2020 2064 6566 2069 735f  s....    def is_
-00001c40: 6974 656d 5f65 6469 7461 626c 6528 7365  item_editable(se
-00001c50: 6c66 2c20 696e 6465 783a 2051 4d6f 6465  lf, index: QMode
-00001c60: 6c49 6e64 6578 2920 2d3e 2062 6f6f 6c3a  lIndex) -> bool:
-00001c70: 0d0a 2020 2020 2020 2020 2222 2252 6574  ..        """Ret
-00001c80: 7572 6e20 5472 7565 2069 6620 6974 656d  urn True if item
-00001c90: 2069 7320 6564 6974 6162 6c65 2c20 4661   is editable, Fa
-00001ca0: 6c73 6520 6f74 6865 7277 6973 6522 2222  lse otherwise"""
-00001cb0: 0d0a 2020 2020 2020 2020 6974 656d 203d  ..        item =
-00001cc0: 2069 6e64 6578 2e69 6e74 6572 6e61 6c50   index.internalP
-00001cd0: 6f69 6e74 6572 2829 0d0a 2020 2020 2020  ointer()..      
-00001ce0: 2020 6966 2074 7970 6528 6974 656d 2920    if type(item) 
-00001cf0: 3d3d 2043 6f6d 6d61 6e64 4974 656d 3a0d  == CommandItem:.
-00001d00: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00001d10: 7572 6e20 6974 656d 2e69 735f 6564 6974  urn item.is_edit
-00001d20: 6162 6c65 2829 0d0a 2020 2020 2020 2020  able()..        
-00001d30: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00001d40: 2020 2072 6574 7572 6e20 4661 6c73 650d     return False.
-00001d50: 0a0d 0a0d 0a69 6620 5f5f 6e61 6d65 5f5f  .....if __name__
-00001d60: 203d 3d20 225f 5f6d 6169 6e5f 5f22 3a0d   == "__main__":.
-00001d70: 0a20 2020 2066 726f 6d20 7372 7369 6e73  .    from srsins
-00001d80: 742e 7372 3836 3020 696d 706f 7274 2053  t.sr860 import S
-00001d90: 5238 3630 0d0a 0d0a 2020 2020 6170 7020  R860....    app 
-00001da0: 3d20 5141 7070 6c69 6361 7469 6f6e 2873  = QApplication(s
-00001db0: 7973 2e61 7267 7629 0d0a 2020 2020 7669  ys.argv)..    vi
-00001dc0: 6577 203d 2051 5472 6565 5669 6577 2829  ew = QTreeView()
-00001dd0: 0d0a 2020 2020 6465 6c65 6761 7465 203d  ..    delegate =
-00001de0: 2043 6f6d 6d61 6e64 4465 6c65 6761 7465   CommandDelegate
-00001df0: 2829 0d0a 2020 2020 6d6f 6465 6c20 3d20  ()..    model = 
-00001e00: 436f 6d6d 616e 644d 6f64 656c 2829 0d0a  CommandModel()..
-00001e10: 0d0a 2020 2020 7669 6577 2e73 6574 4d6f  ..    view.setMo
-00001e20: 6465 6c28 6d6f 6465 6c29 0d0a 2020 2020  del(model)..    
-00001e30: 7669 6577 2e73 6574 4974 656d 4465 6c65  view.setItemDele
-00001e40: 6761 7465 2864 656c 6567 6174 6529 0d0a  gate(delegate)..
-00001e50: 0d0a 2020 2020 696e 7374 203d 2053 5238  ..    inst = SR8
-00001e60: 3630 2827 7463 7069 7027 2c20 2731 3732  60('tcpip', '172
-00001e70: 2e32 352e 3730 2e31 3239 2729 0d0a 2020  .25.70.129')..  
-00001e80: 2020 696e 7374 2e71 7565 7279 5f74 6578    inst.query_tex
-00001e90: 7428 2720 2729 0d0a 0d0a 2020 2020 2320  t(' ')....    # 
-00001ea0: 696e 7374 203d 2052 4741 3130 3028 2774  inst = RGA100('t
-00001eb0: 6370 6970 272c 2731 3732 2e32 352e 3730  cpip','172.25.70
-00001ec0: 2e31 3227 2c27 6164 6d69 6e27 2c27 6164  .12','admin','ad
-00001ed0: 6d69 6e27 290d 0a20 2020 2023 2069 6e73  min')..    # ins
-00001ee0: 7420 3d20 5247 4131 3230 2827 7463 7069  t = RGA120('tcpi
-00001ef0: 7027 2c27 3137 322e 3235 2e37 302e 3132  p','172.25.70.12
-00001f00: 272c 2761 646d 696e 272c 2761 646d 696e  ','admin','admin
-00001f10: 2729 2020 2020 0d0a 2020 2020 0d0a 2020  ')    ..    ..  
-00001f20: 2020 2320 696e 7374 2e63 6f6d 6d2e 7365    # inst.comm.se
-00001f30: 745f 6361 6c6c 6261 636b 7328 7072 696e  t_callbacks(prin
-00001f40: 742c 2070 7269 6e74 290d 0a20 2020 2023  t, print)..    #
-00001f50: 2070 7269 6e74 2869 6e73 742e 6368 6563   print(inst.chec
-00001f60: 6b5f 6964 2829 290d 0a0d 0a20 2020 206d  k_id())....    m
-00001f70: 6f64 656c 2e6c 6f61 6428 696e 7374 290d  odel.load(inst).
-00001f80: 0a0d 0a20 2020 2076 6965 772e 7368 6f77  ...    view.show
-00001f90: 2829 0d0a 2020 2020 7669 6577 2e68 6561  ()..    view.hea
-00001fa0: 6465 7228 292e 7365 7453 6563 7469 6f6e  der().setSection
-00001fb0: 5265 7369 7a65 4d6f 6465 2830 2c20 5148  ResizeMode(0, QH
-00001fc0: 6561 6465 7256 6965 772e 5374 7265 7463  eaderView.Stretc
-00001fd0: 6829 0d0a 2020 2020 2320 7669 6577 2e73  h)..    # view.s
-00001fe0: 6574 416c 7465 726e 6174 696e 6752 6f77  etAlternatingRow
-00001ff0: 436f 6c6f 7273 2854 7275 6529 0d0a 2020  Colors(True)..  
-00002000: 2020 7669 6577 2e72 6573 697a 6528 3530    view.resize(50
-00002010: 302c 2033 3030 290d 0a20 2020 2061 7070  0, 300)..    app
-00002020: 2e65 7865 635f 2829 0d0a                 .exec_()..
+00000020: 7274 2073 7973 0d0a 6672 6f6d 2074 7970  rt sys..from typ
+00000030: 696e 6720 696d 706f 7274 2041 6e79 2c20  ing import Any, 
+00000040: 4974 6572 6162 6c65 2c20 4c69 7374 2c20  Iterable, List, 
+00000050: 4469 6374 2c20 556e 696f 6e0d 0a0d 0a66  Dict, Union....f
+00000060: 726f 6d20 7372 7367 7569 2e75 692e 7174  rom srsgui.ui.qt
+00000070: 2e51 7457 6964 6765 7473 2069 6d70 6f72  .QtWidgets impor
+00000080: 7420 5154 7265 6556 6965 772c 2051 4170  t QTreeView, QAp
+00000090: 706c 6963 6174 696f 6e2c 2051 4865 6164  plication, QHead
+000000a0: 6572 5669 6577 0d0a 6672 6f6d 2073 7273  erView..from srs
+000000b0: 6775 692e 7569 2e71 742e 5174 4775 6920  gui.ui.qt.QtGui 
+000000c0: 696d 706f 7274 2051 4272 7573 682c 2051  import QBrush, Q
+000000d0: 436f 6c6f 720d 0a66 726f 6d20 7372 7367  Color..from srsg
+000000e0: 7569 2e75 692e 7174 2e51 7443 6f72 6520  ui.ui.qt.QtCore 
+000000f0: 696d 706f 7274 2051 4162 7374 7261 6374  import QAbstract
+00000100: 4974 656d 4d6f 6465 6c2c 2051 4d6f 6465  ItemModel, QMode
+00000110: 6c49 6e64 6578 2c20 514f 626a 6563 742c  lIndex, QObject,
+00000120: 2051 742c 2051 4669 6c65 496e 666f 0d0a   Qt, QFileInfo..
+00000130: 0d0a 6672 6f6d 2073 7273 6775 6920 696d  ..from srsgui im
+00000140: 706f 7274 2043 6f6d 706f 6e65 6e74 0d0a  port Component..
+00000150: 0d0a 6672 6f6d 202e 636f 6d6d 616e 6469  ..from .commandi
+00000160: 7465 6d20 696d 706f 7274 2043 6f6d 6d61  tem import Comma
+00000170: 6e64 4974 656d 2c20 496e 6465 780d 0a66  ndItem, Index..f
+00000180: 726f 6d20 2e63 6f6d 6d61 6e64 6465 6c65  rom .commanddele
+00000190: 6761 7465 2069 6d70 6f72 7420 436f 6d6d  gate import Comm
+000001a0: 616e 6444 656c 6567 6174 650d 0a0d 0a0d  andDelegate.....
+000001b0: 0a63 6c61 7373 2043 6f6d 6d61 6e64 4d6f  .class CommandMo
+000001c0: 6465 6c28 5141 6273 7472 6163 7449 7465  del(QAbstractIte
+000001d0: 6d4d 6f64 656c 293a 0d0a 2020 2020 2222  mModel):..    ""
+000001e0: 2220 416e 2065 6469 7461 626c 6520 6d6f  " An editable mo
+000001f0: 6465 6c20 6f66 2043 6f6d 6d61 6e64 2061  del of Command a
+00000200: 6e64 2043 6f6d 706f 6e65 6e74 2022 2222  nd Component """
+00000210: 0d0a 0d0a 2020 2020 6465 6620 5f5f 696e  ....    def __in
+00000220: 6974 5f5f 2873 656c 662c 2070 6172 656e  it__(self, paren
+00000230: 743a 2051 4f62 6a65 6374 203d 204e 6f6e  t: QObject = Non
+00000240: 6529 3a0d 0a20 2020 2020 2020 2073 7570  e):..        sup
+00000250: 6572 2829 2e5f 5f69 6e69 745f 5f28 7061  er().__init__(pa
+00000260: 7265 6e74 290d 0a0d 0a20 2020 2020 2020  rent)....       
+00000270: 2073 656c 662e 7368 6f77 5f6d 6574 686f   self.show_metho
+00000280: 6473 203d 2054 7275 650d 0a20 2020 2020  ds = True..     
+00000290: 2020 2073 656c 662e 7368 6f77 5f65 7863     self.show_exc
+000002a0: 6c75 6465 6420 3d20 5472 7565 0d0a 2020  luded = True..  
+000002b0: 2020 2020 2020 7365 6c66 2e73 686f 775f        self.show_
+000002c0: 7365 745f 6f6e 6c79 203d 2054 7275 650d  set_only = True.
+000002d0: 0a20 2020 2020 2020 2073 656c 662e 7368  .        self.sh
+000002e0: 6f77 5f71 7565 7279 5f6f 6e6c 7920 3d20  ow_query_only = 
+000002f0: 5472 7565 0d0a 2020 2020 2020 2020 7365  True..        se
+00000300: 6c66 2e73 686f 775f 7261 775f 7265 6d6f  lf.show_raw_remo
+00000310: 7465 5f63 6f6d 6d61 6e64 203d 2054 7275  te_command = Tru
+00000320: 650d 0a0d 0a20 2020 2020 2020 2073 656c  e....        sel
+00000330: 662e 5f72 6f6f 7449 7465 6d20 3d20 436f  f._rootItem = Co
+00000340: 6d6d 616e 6449 7465 6d28 290d 0a20 2020  mmandItem()..   
+00000350: 2020 2020 2073 656c 662e 5f68 6561 6465       self._heade
+00000360: 7273 203d 2028 2220 2063 6f6d 6d61 6e64  rs = ("  command
+00000370: 2020 222c 2022 2020 7661 6c75 6520 2022    ", "  value  "
+00000380: 290d 0a0d 0a20 2020 2064 6566 2063 6c65  )....    def cle
+00000390: 6172 2873 656c 6629 3a0d 0a20 2020 2020  ar(self):..     
+000003a0: 2020 2022 2222 2043 6c65 6172 2064 6174     """ Clear dat
+000003b0: 6120 6672 6f6d 2074 6865 206d 6f64 656c  a from the model
+000003c0: 2022 2222 0d0a 2020 2020 2020 2020 7365   """..        se
+000003d0: 6c66 2e6c 6f61 6428 436f 6d70 6f6e 656e  lf.load(Componen
+000003e0: 7428 2929 0d0a 0d0a 2020 2020 6465 6620  t())....    def 
+000003f0: 6c6f 6164 2873 656c 662c 2064 6f63 756d  load(self, docum
+00000400: 656e 743a 2043 6f6d 706f 6e65 6e74 2c20  ent: Component, 
+00000410: 736f 7274 3d46 616c 7365 293a 0d0a 2020  sort=False):..  
+00000420: 2020 2020 2020 2222 224c 6f61 6420 6d6f        """Load mo
+00000430: 6465 6c20 6672 6f6d 2061 206e 6573 7465  del from a neste
+00000440: 6420 6469 6374 696f 6e61 7279 2072 6574  d dictionary ret
+00000450: 7572 6e65 6420 6279 206a 736f 6e2e 6c6f  urned by json.lo
+00000460: 6164 7328 290d 0a0d 0a20 2020 2020 2020  ads()....       
+00000470: 2041 7267 756d 656e 7473 3a0d 0a20 2020   Arguments:..   
+00000480: 2020 2020 2020 2020 2064 6f63 756d 656e           documen
+00000490: 7420 2864 6963 7429 3a20 4a53 4f4e 2d63  t (dict): JSON-c
+000004a0: 6f6d 7061 7469 626c 6520 6469 6374 696f  ompatible dictio
+000004b0: 6e61 7279 0d0a 2020 2020 2020 2020 2222  nary..        ""
+000004c0: 220d 0a0d 0a20 2020 2020 2020 2061 7373  "....        ass
+000004d0: 6572 7420 6973 696e 7374 616e 6365 280d  ert isinstance(.
+000004e0: 0a20 2020 2020 2020 2020 2020 2064 6f63  .            doc
+000004f0: 756d 656e 742c 2043 6f6d 706f 6e65 6e74  ument, Component
+00000500: 0d0a 2020 2020 2020 2020 292c 2022 6064  ..        ), "`d
+00000510: 6f63 756d 656e 7460 206d 7573 7420 6265  ocument` must be
+00000520: 206f 6620 6469 6374 2c20 6c69 7374 206f   of dict, list o
+00000530: 7220 7475 706c 652c 2022 2066 226e 6f74  r tuple, " f"not
+00000540: 207b 7479 7065 2864 6f63 756d 656e 7429   {type(document)
+00000550: 7d22 0d0a 0d0a 2020 2020 2020 2020 7365  }"....        se
+00000560: 6c66 2e62 6567 696e 5265 7365 744d 6f64  lf.beginResetMod
+00000570: 656c 2829 0d0a 0d0a 2020 2020 2020 2020  el()....        
+00000580: 7365 6c66 2e5f 726f 6f74 4974 656d 203d  self._rootItem =
+00000590: 2043 6f6d 6d61 6e64 4974 656d 2e6c 6f61   CommandItem.loa
+000005a0: 6428 646f 6375 6d65 6e74 2c20 736f 7274  d(document, sort
+000005b0: 3d73 6f72 7429 0d0a 2020 2020 2020 2020  =sort)..        
+000005c0: 7365 6c66 2e5f 726f 6f74 4974 656d 2e76  self._rootItem.v
+000005d0: 616c 7565 5f74 7970 6520 3d20 7479 7065  alue_type = type
+000005e0: 2864 6f63 756d 656e 7429 0d0a 0d0a 2020  (document)....  
+000005f0: 2020 2020 2020 7365 6c66 2e65 6e64 5265        self.endRe
+00000600: 7365 744d 6f64 656c 2829 0d0a 0d0a 2020  setModel()....  
+00000610: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+00000620: 650d 0a0d 0a20 2020 2064 6566 2064 6174  e....    def dat
+00000630: 6128 7365 6c66 2c20 696e 6465 783a 2051  a(self, index: Q
+00000640: 4d6f 6465 6c49 6e64 6578 2c20 726f 6c65  ModelIndex, role
+00000650: 3a20 5174 2e49 7465 6d44 6174 6152 6f6c  : Qt.ItemDataRol
+00000660: 6529 202d 3e20 416e 793a 0d0a 2020 2020  e) -> Any:..    
+00000670: 2020 2020 2222 224f 7665 7272 6964 6520      """Override 
+00000680: 6672 6f6d 2051 4162 7374 7261 6374 4974  from QAbstractIt
+00000690: 656d 4d6f 6465 6c0d 0a0d 0a20 2020 2020  emModel....     
+000006a0: 2020 2052 6574 7572 6e20 6461 7461 2066     Return data f
+000006b0: 726f 6d20 616e 2069 7465 6d20 6163 636f  rom an item acco
+000006c0: 7264 696e 6720 696e 6465 7820 616e 6420  rding index and 
+000006d0: 726f 6c65 0d0a 2020 2020 2020 2020 2222  role..        ""
+000006e0: 220d 0a0d 0a20 2020 2020 2020 2069 6620  "....        if 
+000006f0: 6e6f 7420 696e 6465 782e 6973 5661 6c69  not index.isVali
+00000700: 6428 293a 0d0a 2020 2020 2020 2020 2020  d():..          
+00000710: 2020 7265 7475 726e 204e 6f6e 650d 0a0d    return None...
+00000720: 0a20 2020 2020 2020 2069 6620 726f 6c65  .        if role
+00000730: 203d 3d20 5174 2e44 6973 706c 6179 526f   == Qt.DisplayRo
+00000740: 6c65 3a0d 0a20 2020 2020 2020 2020 2020  le:..           
+00000750: 2069 6620 696e 6465 782e 636f 6c75 6d6e   if index.column
+00000760: 2829 203d 3d20 303a 0d0a 2020 2020 2020  () == 0:..      
+00000770: 2020 2020 2020 2020 2020 6974 656d 203d            item =
+00000780: 2069 6e64 6578 2e69 6e74 6572 6e61 6c50   index.internalP
+00000790: 6f69 6e74 6572 2829 0d0a 2020 2020 2020  ointer()..      
+000007a0: 2020 2020 2020 2020 2020 6e61 6d65 203d            name =
+000007b0: 2069 7465 6d2e 6e61 6d65 0d0a 0d0a 2020   item.name....  
+000007c0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000007d0: 2073 656c 662e 7368 6f77 5f72 6177 5f72   self.show_raw_r
+000007e0: 656d 6f74 655f 636f 6d6d 616e 643a 0d0a  emote_command:..
+000007f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000800: 2020 2020 6e61 6d65 202b 3d20 6627 203c      name += f' <
+00000810: 7b69 7465 6d2e 7261 775f 7265 6d6f 7465  {item.raw_remote
+00000820: 5f63 6f6d 6d61 6e64 7d3e 2720 6966 2069  _command}>' if i
+00000830: 7465 6d2e 7261 775f 7265 6d6f 7465 5f63  tem.raw_remote_c
+00000840: 6f6d 6d61 6e64 2065 6c73 6520 2727 0d0a  ommand else ''..
+00000850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000860: 6966 2073 656c 662e 7368 6f77 5f6d 6574  if self.show_met
+00000870: 686f 6473 3a0d 0a20 2020 2020 2020 2020  hods:..         
+00000880: 2020 2020 2020 2020 2020 206e 616d 6520             name 
+00000890: 2b3d 2027 205b 4d5d 2720 6966 2069 7465  += ' [M]' if ite
+000008a0: 6d2e 6973 5f6d 6574 686f 6420 656c 7365  m.is_method else
+000008b0: 2027 270d 0a20 2020 2020 2020 2020 2020   ''..           
+000008c0: 2020 2020 2069 6620 7365 6c66 2e73 686f       if self.sho
+000008d0: 775f 6578 636c 7564 6564 3a0d 0a20 2020  w_excluded:..   
+000008e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008f0: 206e 616d 6520 2b3d 2027 205b 4558 5d27   name += ' [EX]'
+00000900: 2069 6620 6974 656d 2e65 7863 6c75 6465   if item.exclude
+00000910: 6420 656c 7365 2027 270d 0a20 2020 2020  d else ''..     
+00000920: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00000930: 6c66 2e73 686f 775f 7365 745f 6f6e 6c79  lf.show_set_only
+00000940: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00000950: 2020 2020 2020 206e 616d 6520 2b3d 2027         name += '
+00000960: 205b 534f 5d27 2069 6620 6974 656d 2e73   [SO]' if item.s
+00000970: 6574 5f65 6e61 626c 6520 616e 6420 6e6f  et_enable and no
+00000980: 7420 6974 656d 2e67 6574 5f65 6e61 626c  t item.get_enabl
+00000990: 6520 656c 7365 2027 270d 0a20 2020 2020  e else ''..     
+000009a0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+000009b0: 6c66 2e73 686f 775f 7175 6572 795f 6f6e  lf.show_query_on
+000009c0: 6c79 3a0d 0a20 2020 2020 2020 2020 2020  ly:..           
+000009d0: 2020 2020 2020 2020 206e 616d 6520 2b3d           name +=
+000009e0: 2027 205b 514f 5d27 2069 6620 6974 656d   ' [QO]' if item
+000009f0: 2e67 6574 5f65 6e61 626c 6520 616e 6420  .get_enable and 
+00000a00: 6e6f 7420 6974 656d 2e73 6574 5f65 6e61  not item.set_ena
+00000a10: 626c 6520 656c 7365 2027 270d 0a20 2020  ble else ''..   
+00000a20: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00000a30: 7572 6e20 6e61 6d65 0d0a 0d0a 2020 2020  urn name....    
+00000a40: 2020 2020 2020 2020 6966 2069 6e64 6578          if index
+00000a50: 2e63 6f6c 756d 6e28 2920 3d3d 2031 3a0d  .column() == 1:.
+00000a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000a70: 2069 7465 6d20 3d20 696e 6465 782e 696e   item = index.in
+00000a80: 7465 726e 616c 506f 696e 7465 7228 290d  ternalPointer().
+00000a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000aa0: 2076 203d 2069 7465 6d2e 7661 6c75 650d   v = item.value.
+00000ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000ac0: 2069 6620 7620 6973 204e 6f6e 653a 0d0a   if v is None:..
+00000ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ae0: 2020 2020 7265 7475 726e 0d0a 2020 2020      return..    
+00000af0: 2020 2020 2020 2020 2020 2020 756e 6974              unit
+00000b00: 203d 2069 7465 6d2e 6765 745f 756e 6974   = item.get_unit
+00000b10: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+00000b20: 2020 2020 666d 7420 3d20 6974 656d 2e67      fmt = item.g
+00000b30: 6574 5f66 6f72 6d61 7428 290d 0a20 2020  et_format()..   
+00000b40: 2020 2020 2020 2020 2020 2020 2074 7279               try
+00000b50: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00000b60: 2020 2020 2020 2069 6620 756e 6974 3a0d         if unit:.
+00000b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000b80: 2020 2020 2020 2020 2076 616c 203d 2066           val = f
+00000b90: 277b 763a 7b66 6d74 7d7d 2020 7b69 7465  '{v:{fmt}}  {ite
+00000ba0: 6d2e 6765 745f 756e 6974 2829 7d27 0d0a  m.get_unit()}'..
+00000bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000bc0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00000bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000be0: 2020 2076 616c 203d 2066 277b 763a 7b66     val = f'{v:{f
+00000bf0: 6d74 7d7d 270d 0a20 2020 2020 2020 2020  mt}}'..         
+00000c00: 2020 2020 2020 2065 7863 6570 7420 5661         except Va
+00000c10: 6c75 6545 7272 6f72 3a0d 0a20 2020 2020  lueError:..     
+00000c20: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00000c30: 7269 6e74 2866 2756 616c 7565 4572 726f  rint(f'ValueErro
+00000c40: 723a 207b 6974 656d 2e72 6177 5f72 656d  r: {item.raw_rem
+00000c50: 6f74 655f 636f 6d6d 616e 647d 207b 767d  ote_command} {v}
+00000c60: 207b 666d 747d 207b 756e 6974 7d27 290d   {fmt} {unit}').
+00000c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000c80: 2020 2020 2076 616c 203d 2066 277b 767d       val = f'{v}
+00000c90: 270d 0a20 2020 2020 2020 2020 2020 2020  '..             
+00000ca0: 2020 2072 6574 7572 6e20 7661 6c0d 0a0d     return val...
+00000cb0: 0a20 2020 2020 2020 2065 6c69 6620 726f  .        elif ro
+00000cc0: 6c65 203d 3d20 5174 2e45 6469 7452 6f6c  le == Qt.EditRol
+00000cd0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00000ce0: 6966 2069 6e64 6578 2e63 6f6c 756d 6e28  if index.column(
+00000cf0: 2920 3d3d 2031 3a0d 0a20 2020 2020 2020  ) == 1:..       
+00000d00: 2020 2020 2020 2020 2069 7465 6d20 3d20           item = 
+00000d10: 696e 6465 782e 696e 7465 726e 616c 506f  index.internalPo
+00000d20: 696e 7465 7228 290d 0a20 2020 2020 2020  inter()..       
+00000d30: 2020 2020 2020 2020 2076 616c 203d 2069           val = i
+00000d40: 7465 6d2e 7661 6c75 650d 0a20 2020 2020  tem.value..     
+00000d50: 2020 2020 2020 2020 2020 2023 2070 7269             # pri
+00000d60: 6e74 2827 6461 7461 272c 2069 7465 6d2e  nt('data', item.
+00000d70: 6e61 6d65 2c20 6974 656d 2e63 6f6d 702c  name, item.comp,
+00000d80: 2076 616c 290d 0a20 2020 2020 2020 2020   val)..         
+00000d90: 2020 2020 2020 2072 6574 7572 6e20 7661         return va
+00000da0: 6c0d 0a0d 0a20 2020 2020 2020 2065 6c69  l....        eli
+00000db0: 6620 726f 6c65 203d 3d20 5174 2e42 6163  f role == Qt.Bac
+00000dc0: 6b67 726f 756e 6452 6f6c 653a 0d0a 2020  kgroundRole:..  
+00000dd0: 2020 2020 2020 2020 2020 6974 656d 203d            item =
+00000de0: 2069 6e64 6578 2e69 6e74 6572 6e61 6c50   index.internalP
+00000df0: 6f69 6e74 6572 2829 0d0a 2020 2020 2020  ointer()..      
+00000e00: 2020 2020 2020 6966 2069 7465 6d2e 636f        if item.co
+00000e10: 6d70 5f74 7970 6520 213d 2049 6e64 6578  mp_type != Index
+00000e20: 2061 6e64 2069 7373 7562 636c 6173 7328   and issubclass(
+00000e30: 6974 656d 2e63 6f6d 705f 7479 7065 2c20  item.comp_type, 
+00000e40: 436f 6d70 6f6e 656e 7429 3a0d 0a20 2020  Component):..   
+00000e50: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00000e60: 7572 6e20 5142 7275 7368 2851 436f 6c6f  urn QBrush(QColo
+00000e70: 7228 3234 332c 2032 3330 2c20 3232 3529  r(243, 230, 225)
+00000e80: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
+00000e90: 6620 6974 656d 2e72 6f77 2829 2025 2032  f item.row() % 2
+00000ea0: 203d 3d20 303a 0d0a 2020 2020 2020 2020   == 0:..        
+00000eb0: 2020 2020 2020 2020 7265 7475 726e 2051          return Q
+00000ec0: 4272 7573 6828 5143 6f6c 6f72 2832 3430  Brush(QColor(240
+00000ed0: 2c20 3234 302c 2032 3533 2929 0d0a 0d0a  , 240, 253))....
+00000ee0: 2020 2020 6465 6620 7365 7444 6174 6128      def setData(
+00000ef0: 7365 6c66 2c20 696e 6465 783a 2051 4d6f  self, index: QMo
+00000f00: 6465 6c49 6e64 6578 2c20 7661 6c75 653a  delIndex, value:
+00000f10: 2041 6e79 2c20 726f 6c65 3a20 5174 2e49   Any, role: Qt.I
+00000f20: 7465 6d44 6174 6152 6f6c 6529 3a0d 0a20  temDataRole):.. 
+00000f30: 2020 2020 2020 2022 2222 4f76 6572 7269         """Overri
+00000f40: 6465 2066 726f 6d20 5141 6273 7472 6163  de from QAbstrac
+00000f50: 7449 7465 6d4d 6f64 656c 0d0a 0d0a 2020  tItemModel....  
+00000f60: 2020 2020 2020 5365 7420 436f 6d6d 616e        Set Comman
+00000f70: 6449 7465 6d20 6163 636f 7264 696e 6720  dItem according 
+00000f80: 746f 2069 6e64 6578 2061 6e64 2072 6f6c  to index and rol
+00000f90: 650d 0a0d 0a20 2020 2020 2020 2041 7267  e....        Arg
+00000fa0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00000fb0: 696e 6465 7820 2851 4d6f 6465 6c49 6e64  index (QModelInd
+00000fc0: 6578 290d 0a20 2020 2020 2020 2020 2020  ex)..           
+00000fd0: 2076 616c 7565 2028 416e 7929 0d0a 2020   value (Any)..  
+00000fe0: 2020 2020 2020 2020 2020 726f 6c65 2028            role (
+00000ff0: 5174 2e49 7465 6d44 6174 6152 6f6c 6529  Qt.ItemDataRole)
+00001000: 0d0a 2020 2020 2020 2020 2222 220d 0a0d  ..        """...
+00001010: 0a20 2020 2020 2020 2069 6620 726f 6c65  .        if role
+00001020: 203d 3d20 5174 2e45 6469 7452 6f6c 653a   == Qt.EditRole:
+00001030: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00001040: 2069 6e64 6578 2e63 6f6c 756d 6e28 2920   index.column() 
+00001050: 3d3d 2031 3a0d 0a20 2020 2020 2020 2020  == 1:..         
+00001060: 2020 2020 2020 2069 7465 6d20 3d20 696e         item = in
+00001070: 6465 782e 696e 7465 726e 616c 506f 696e  dex.internalPoin
+00001080: 7465 7228 290d 0a20 2020 2020 2020 2020  ter()..         
+00001090: 2020 2020 2020 2069 7465 6d2e 7365 745f         item.set_
+000010a0: 7661 6c75 6528 7661 6c75 6529 0d0a 2020  value(value)..  
+000010b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000010c0: 6c66 2e64 6174 6143 6861 6e67 6564 2e65  lf.dataChanged.e
+000010d0: 6d69 7428 696e 6465 782c 2069 6e64 6578  mit(index, index
+000010e0: 2c20 5b51 742e 4564 6974 526f 6c65 5d29  , [Qt.EditRole])
+000010f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001100: 2020 7265 7475 726e 2054 7275 650d 0a20    return True.. 
+00001110: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00001120: 6e20 4661 6c73 650d 0a20 2020 200d 0a20  n False..    .. 
+00001130: 2020 2064 6566 2068 6561 6465 7244 6174     def headerDat
+00001140: 6128 7365 6c66 2c20 7365 6374 696f 6e3a  a(self, section:
+00001150: 2069 6e74 2c20 6f72 6965 6e74 6174 696f   int, orientatio
+00001160: 6e3a 2051 742e 4f72 6965 6e74 6174 696f  n: Qt.Orientatio
+00001170: 6e2c 0d0a 2020 2020 2020 2020 2020 2020  n,..            
+00001180: 2020 2020 2020 2072 6f6c 653a 2051 742e         role: Qt.
+00001190: 4974 656d 4461 7461 526f 6c65 2020 2020  ItemDataRole    
+000011a0: 293a 0d0a 2020 2020 2020 2020 2222 224f  ):..        """O
+000011b0: 7665 7272 6964 6520 6672 6f6d 2051 4162  verride from QAb
+000011c0: 7374 7261 6374 4974 656d 4d6f 6465 6c0d  stractItemModel.
+000011d0: 0a0d 0a20 2020 2020 2020 2069 7420 7265  ...        it re
+000011e0: 7475 726e 7320 6f6e 6c79 2064 6174 6120  turns only data 
+000011f0: 666f 7220 636f 6c75 6d6e 7320 286f 7269  for columns (ori
+00001200: 656e 7461 7469 6f6e 203d 2048 6f72 697a  entation = Horiz
+00001210: 6f6e 7461 6c29 0d0a 2020 2020 2020 2020  ontal)..        
+00001220: 2222 220d 0a20 2020 2020 2020 2069 6620  """..        if 
+00001230: 726f 6c65 2021 3d20 5174 2e44 6973 706c  role != Qt.Displ
+00001240: 6179 526f 6c65 3a0d 0a20 2020 2020 2020  ayRole:..       
+00001250: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+00001260: 0d0a 0d0a 2020 2020 2020 2020 6966 206f  ....        if o
+00001270: 7269 656e 7461 7469 6f6e 203d 3d20 5174  rientation == Qt
+00001280: 2e48 6f72 697a 6f6e 7461 6c3a 0d0a 2020  .Horizontal:..  
+00001290: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000012a0: 2073 656c 662e 5f68 6561 6465 7273 5b73   self._headers[s
+000012b0: 6563 7469 6f6e 5d0d 0a0d 0a20 2020 2064  ection]....    d
+000012c0: 6566 2069 6e64 6578 2873 656c 662c 2072  ef index(self, r
+000012d0: 6f77 3a20 696e 742c 2063 6f6c 756d 6e3a  ow: int, column:
+000012e0: 2069 6e74 2c20 7061 7265 6e74 3d51 4d6f   int, parent=QMo
+000012f0: 6465 6c49 6e64 6578 2829 2920 2d3e 2051  delIndex()) -> Q
+00001300: 4d6f 6465 6c49 6e64 6578 3a0d 0a20 2020  ModelIndex:..   
+00001310: 2020 2020 2022 2222 4f76 6572 7269 6465       """Override
+00001320: 2066 726f 6d20 5141 6273 7472 6163 7449   from QAbstractI
+00001330: 7465 6d4d 6f64 656c 0d0a 0d0a 2020 2020  temModel....    
+00001340: 2020 2020 5265 7475 726e 2069 6e64 6578      Return index
+00001350: 2061 6363 6f72 6469 6e67 2072 6f77 2c20   according row, 
+00001360: 636f 6c75 6d6e 2061 6e64 2070 6172 656e  column and paren
+00001370: 740d 0a20 2020 2020 2020 2022 2222 0d0a  t..        """..
+00001380: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
+00001390: 656c 662e 6861 7349 6e64 6578 2872 6f77  elf.hasIndex(row
+000013a0: 2c20 636f 6c75 6d6e 2c20 7061 7265 6e74  , column, parent
+000013b0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+000013c0: 7265 7475 726e 2051 4d6f 6465 6c49 6e64  return QModelInd
+000013d0: 6578 2829 0d0a 0d0a 2020 2020 2020 2020  ex()....        
+000013e0: 6966 206e 6f74 2070 6172 656e 742e 6973  if not parent.is
+000013f0: 5661 6c69 6428 293a 0d0a 2020 2020 2020  Valid():..      
+00001400: 2020 2020 2020 7061 7265 6e74 4974 656d        parentItem
+00001410: 203d 2073 656c 662e 5f72 6f6f 7449 7465   = self._rootIte
+00001420: 6d0d 0a20 2020 2020 2020 2065 6c73 653a  m..        else:
+00001430: 0d0a 2020 2020 2020 2020 2020 2020 7061  ..            pa
+00001440: 7265 6e74 4974 656d 203d 2070 6172 656e  rentItem = paren
+00001450: 742e 696e 7465 726e 616c 506f 696e 7465  t.internalPointe
+00001460: 7228 290d 0a0d 0a20 2020 2020 2020 2063  r()....        c
+00001470: 6869 6c64 4974 656d 203d 2070 6172 656e  hildItem = paren
+00001480: 7449 7465 6d2e 6368 696c 6428 726f 7729  tItem.child(row)
+00001490: 0d0a 2020 2020 2020 2020 6966 2063 6869  ..        if chi
+000014a0: 6c64 4974 656d 3a0d 0a20 2020 2020 2020  ldItem:..       
+000014b0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+000014c0: 2e63 7265 6174 6549 6e64 6578 2872 6f77  .createIndex(row
+000014d0: 2c20 636f 6c75 6d6e 2c20 6368 696c 6449  , column, childI
+000014e0: 7465 6d29 0d0a 2020 2020 2020 2020 656c  tem)..        el
+000014f0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00001500: 2072 6574 7572 6e20 514d 6f64 656c 496e   return QModelIn
+00001510: 6465 7828 290d 0a0d 0a20 2020 2064 6566  dex()....    def
+00001520: 2070 6172 656e 7428 7365 6c66 2c20 696e   parent(self, in
+00001530: 6465 783a 2051 4d6f 6465 6c49 6e64 6578  dex: QModelIndex
+00001540: 2920 2d3e 2051 4d6f 6465 6c49 6e64 6578  ) -> QModelIndex
+00001550: 3a0d 0a20 2020 2020 2020 2022 2222 4f76  :..        """Ov
+00001560: 6572 7269 6465 2066 726f 6d20 5141 6273  erride from QAbs
+00001570: 7472 6163 7449 7465 6d4d 6f64 656c 0d0a  tractItemModel..
+00001580: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00001590: 2070 6172 656e 7420 696e 6465 7820 6f66   parent index of
+000015a0: 2069 6e64 6578 0d0a 2020 2020 2020 2020   index..        
+000015b0: 2222 220d 0a0d 0a20 2020 2020 2020 2069  """....        i
+000015c0: 6620 6e6f 7420 696e 6465 782e 6973 5661  f not index.isVa
+000015d0: 6c69 6428 293a 0d0a 2020 2020 2020 2020  lid():..        
+000015e0: 2020 2020 7265 7475 726e 2051 4d6f 6465      return QMode
+000015f0: 6c49 6e64 6578 2829 0d0a 0d0a 2020 2020  lIndex()....    
+00001600: 2020 2020 6368 696c 6449 7465 6d20 3d20      childItem = 
+00001610: 696e 6465 782e 696e 7465 726e 616c 506f  index.internalPo
+00001620: 696e 7465 7228 290d 0a20 2020 2020 2020  inter()..       
+00001630: 2070 6172 656e 7449 7465 6d20 3d20 6368   parentItem = ch
+00001640: 696c 6449 7465 6d2e 7061 7265 6e74 2829  ildItem.parent()
+00001650: 0d0a 0d0a 2020 2020 2020 2020 6966 2070  ....        if p
+00001660: 6172 656e 7449 7465 6d20 3d3d 2073 656c  arentItem == sel
+00001670: 662e 5f72 6f6f 7449 7465 6d3a 0d0a 2020  f._rootItem:..  
+00001680: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00001690: 2051 4d6f 6465 6c49 6e64 6578 2829 0d0a   QModelIndex()..
+000016a0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+000016b0: 2073 656c 662e 6372 6561 7465 496e 6465   self.createInde
+000016c0: 7828 7061 7265 6e74 4974 656d 2e72 6f77  x(parentItem.row
+000016d0: 2829 2c20 302c 2070 6172 656e 7449 7465  (), 0, parentIte
+000016e0: 6d29 0d0a 0d0a 2020 2020 6465 6620 726f  m)....    def ro
+000016f0: 7743 6f75 6e74 2873 656c 662c 2070 6172  wCount(self, par
+00001700: 656e 743d 514d 6f64 656c 496e 6465 7828  ent=QModelIndex(
+00001710: 2929 3a0d 0a20 2020 2020 2020 2022 2222  )):..        """
+00001720: 4f76 6572 7269 6465 2066 726f 6d20 5141  Override from QA
+00001730: 6273 7472 6163 7449 7465 6d4d 6f64 656c  bstractItemModel
+00001740: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
+00001750: 726e 2072 6f77 2063 6f75 6e74 2066 726f  rn row count fro
+00001760: 6d20 7061 7265 6e74 2069 6e64 6578 0d0a  m parent index..
+00001770: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00001780: 2020 2020 2069 6620 7061 7265 6e74 2e63       if parent.c
+00001790: 6f6c 756d 6e28 2920 3e20 303a 0d0a 2020  olumn() > 0:..  
+000017a0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000017b0: 2030 0d0a 0d0a 2020 2020 2020 2020 6966   0....        if
+000017c0: 206e 6f74 2070 6172 656e 742e 6973 5661   not parent.isVa
+000017d0: 6c69 6428 293a 0d0a 2020 2020 2020 2020  lid():..        
+000017e0: 2020 2020 7061 7265 6e74 4974 656d 203d      parentItem =
+000017f0: 2073 656c 662e 5f72 6f6f 7449 7465 6d0d   self._rootItem.
+00001800: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
+00001810: 2020 2020 2020 2020 2020 2020 7061 7265              pare
+00001820: 6e74 4974 656d 203d 2070 6172 656e 742e  ntItem = parent.
+00001830: 696e 7465 726e 616c 506f 696e 7465 7228  internalPointer(
+00001840: 290d 0a0d 0a20 2020 2020 2020 2072 6574  )....        ret
+00001850: 7572 6e20 7061 7265 6e74 4974 656d 2e63  urn parentItem.c
+00001860: 6869 6c64 436f 756e 7428 290d 0a0d 0a20  hildCount().... 
+00001870: 2020 2064 6566 2063 6f6c 756d 6e43 6f75     def columnCou
+00001880: 6e74 2873 656c 662c 2070 6172 656e 743d  nt(self, parent=
+00001890: 514d 6f64 656c 496e 6465 7828 2929 3a0d  QModelIndex()):.
+000018a0: 0a20 2020 2020 2020 2022 2222 4f76 6572  .        """Over
+000018b0: 7269 6465 2066 726f 6d20 5141 6273 7472  ride from QAbstr
+000018c0: 6163 7449 7465 6d4d 6f64 656c 0d0a 0d0a  actItemModel....
+000018d0: 2020 2020 2020 2020 5265 7475 726e 2063          Return c
+000018e0: 6f6c 756d 6e20 6e75 6d62 6572 2e20 466f  olumn number. Fo
+000018f0: 7220 7468 6520 6d6f 6465 6c2c 2069 7420  r the model, it 
+00001900: 616c 7761 7973 2072 6574 7572 6e20 3220  always return 2 
+00001910: 636f 6c75 6d6e 730d 0a20 2020 2020 2020  columns..       
+00001920: 2022 2222 0d0a 2020 2020 2020 2020 7265   """..        re
+00001930: 7475 726e 2032 0d0a 0d0a 2020 2020 6465  turn 2....    de
+00001940: 6620 666c 6167 7328 7365 6c66 2c20 696e  f flags(self, in
+00001950: 6465 783a 2051 4d6f 6465 6c49 6e64 6578  dex: QModelIndex
+00001960: 2920 2d3e 2051 742e 4974 656d 466c 6167  ) -> Qt.ItemFlag
+00001970: 733a 0d0a 2020 2020 2020 2020 2222 224f  s:..        """O
+00001980: 7665 7272 6964 6520 6672 6f6d 2051 4162  verride from QAb
+00001990: 7374 7261 6374 4974 656d 4d6f 6465 6c0d  stractItemModel.
+000019a0: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+000019b0: 6e20 666c 6167 7320 6f66 2069 6e64 6578  n flags of index
+000019c0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+000019d0: 2020 2020 2020 2066 6c61 6773 203d 2073         flags = s
+000019e0: 7570 6572 2843 6f6d 6d61 6e64 4d6f 6465  uper(CommandMode
+000019f0: 6c2c 2073 656c 6629 2e66 6c61 6773 2869  l, self).flags(i
+00001a00: 6e64 6578 290d 0a0d 0a20 2020 2020 2020  ndex)....       
+00001a10: 2069 6620 696e 6465 782e 636f 6c75 6d6e   if index.column
+00001a20: 2829 203d 3d20 3120 616e 6420 7365 6c66  () == 1 and self
+00001a30: 2e69 735f 6974 656d 5f65 6469 7461 626c  .is_item_editabl
+00001a40: 6528 696e 6465 7829 3a0d 0a20 2020 2020  e(index):..     
+00001a50: 2020 2020 2020 2072 6574 7572 6e20 5174         return Qt
+00001a60: 2e49 7465 6d49 7345 6469 7461 626c 6520  .ItemIsEditable 
+00001a70: 7c20 666c 6167 730d 0a20 2020 2020 2020  | flags..       
+00001a80: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00001a90: 2020 2020 7265 7475 726e 2066 6c61 6773      return flags
+00001aa0: 0d0a 0d0a 2020 2020 6465 6620 6973 5f69  ....    def is_i
+00001ab0: 7465 6d5f 6564 6974 6162 6c65 2873 656c  tem_editable(sel
+00001ac0: 662c 2069 6e64 6578 3a20 514d 6f64 656c  f, index: QModel
+00001ad0: 496e 6465 7829 202d 3e20 626f 6f6c 3a0d  Index) -> bool:.
+00001ae0: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
+00001af0: 726e 2054 7275 6520 6966 2069 7465 6d20  rn True if item 
+00001b00: 6973 2065 6469 7461 626c 652c 2046 616c  is editable, Fal
+00001b10: 7365 206f 7468 6572 7769 7365 2222 220d  se otherwise""".
+00001b20: 0a20 2020 2020 2020 2069 7465 6d20 3d20  .        item = 
+00001b30: 696e 6465 782e 696e 7465 726e 616c 506f  index.internalPo
+00001b40: 696e 7465 7228 290d 0a20 2020 2020 2020  inter()..       
+00001b50: 2069 6620 7479 7065 2869 7465 6d29 203d   if type(item) =
+00001b60: 3d20 436f 6d6d 616e 6449 7465 6d3a 0d0a  = CommandItem:..
+00001b70: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00001b80: 726e 2069 7465 6d2e 6973 5f65 6469 7461  rn item.is_edita
+00001b90: 626c 6528 290d 0a20 2020 2020 2020 2065  ble()..        e
+00001ba0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00001bb0: 2020 7265 7475 726e 2046 616c 7365 0d0a    return False..
+00001bc0: 0d0a 0d0a 6966 205f 5f6e 616d 655f 5f20  ....if __name__ 
+00001bd0: 3d3d 2022 5f5f 6d61 696e 5f5f 223a 0d0a  == "__main__":..
+00001be0: 2020 2020 6672 6f6d 2073 7273 696e 7374      from srsinst
+00001bf0: 2e73 7238 3630 2069 6d70 6f72 7420 5352  .sr860 import SR
+00001c00: 3836 300d 0a0d 0a20 2020 2061 7070 203d  860....    app =
+00001c10: 2051 4170 706c 6963 6174 696f 6e28 7379   QApplication(sy
+00001c20: 732e 6172 6776 290d 0a20 2020 2076 6965  s.argv)..    vie
+00001c30: 7720 3d20 5154 7265 6556 6965 7728 290d  w = QTreeView().
+00001c40: 0a20 2020 2064 656c 6567 6174 6520 3d20  .    delegate = 
+00001c50: 436f 6d6d 616e 6444 656c 6567 6174 6528  CommandDelegate(
+00001c60: 290d 0a20 2020 206d 6f64 656c 203d 2043  )..    model = C
+00001c70: 6f6d 6d61 6e64 4d6f 6465 6c28 290d 0a0d  ommandModel()...
+00001c80: 0a20 2020 2076 6965 772e 7365 744d 6f64  .    view.setMod
+00001c90: 656c 286d 6f64 656c 290d 0a20 2020 2076  el(model)..    v
+00001ca0: 6965 772e 7365 7449 7465 6d44 656c 6567  iew.setItemDeleg
+00001cb0: 6174 6528 6465 6c65 6761 7465 290d 0a0d  ate(delegate)...
+00001cc0: 0a20 2020 2069 6e73 7420 3d20 5352 3836  .    inst = SR86
+00001cd0: 3028 2774 6370 6970 272c 2027 3137 322e  0('tcpip', '172.
+00001ce0: 3235 2e37 302e 3132 3927 290d 0a20 2020  25.70.129')..   
+00001cf0: 2069 6e73 742e 7175 6572 795f 7465 7874   inst.query_text
+00001d00: 2827 2027 290d 0a0d 0a20 2020 2023 2069  (' ')....    # i
+00001d10: 6e73 7420 3d20 5247 4131 3030 2827 7463  nst = RGA100('tc
+00001d20: 7069 7027 2c27 3137 322e 3235 2e37 302e  pip','172.25.70.
+00001d30: 3132 272c 2761 646d 696e 272c 2761 646d  12','admin','adm
+00001d40: 696e 2729 0d0a 2020 2020 2320 696e 7374  in')..    # inst
+00001d50: 203d 2052 4741 3132 3028 2774 6370 6970   = RGA120('tcpip
+00001d60: 272c 2731 3732 2e32 352e 3730 2e31 3227  ','172.25.70.12'
+00001d70: 2c27 6164 6d69 6e27 2c27 6164 6d69 6e27  ,'admin','admin'
+00001d80: 2920 2020 200d 0a20 2020 200d 0a20 2020  )    ..    ..   
+00001d90: 2023 2069 6e73 742e 636f 6d6d 2e73 6574   # inst.comm.set
+00001da0: 5f63 616c 6c62 6163 6b73 2870 7269 6e74  _callbacks(print
+00001db0: 2c20 7072 696e 7429 0d0a 2020 2020 2320  , print)..    # 
+00001dc0: 7072 696e 7428 696e 7374 2e63 6865 636b  print(inst.check
+00001dd0: 5f69 6428 2929 0d0a 0d0a 2020 2020 6d6f  _id())....    mo
+00001de0: 6465 6c2e 6c6f 6164 2869 6e73 7429 0d0a  del.load(inst)..
+00001df0: 0d0a 2020 2020 7669 6577 2e73 686f 7728  ..    view.show(
+00001e00: 290d 0a20 2020 2076 6965 772e 6865 6164  )..    view.head
+00001e10: 6572 2829 2e73 6574 5365 6374 696f 6e52  er().setSectionR
+00001e20: 6573 697a 654d 6f64 6528 302c 2051 4865  esizeMode(0, QHe
+00001e30: 6164 6572 5669 6577 2e53 7472 6574 6368  aderView.Stretch
+00001e40: 290d 0a20 2020 2023 2076 6965 772e 7365  )..    # view.se
+00001e50: 7441 6c74 6572 6e61 7469 6e67 526f 7743  tAlternatingRowC
+00001e60: 6f6c 6f72 7328 5472 7565 290d 0a20 2020  olors(True)..   
+00001e70: 2076 6965 772e 7265 7369 7a65 2835 3030   view.resize(500
+00001e80: 2c20 3330 3029 0d0a 2020 2020 6170 702e  , 300)..    app.
+00001e90: 6578 6563 5f28 290d 0a                   exec_()..
```

### Comparing `srsgui-0.2.15/srsgui/ui/commandtree/commandspinbox.py` & `srsgui-0.2.9/srsgui/ui/commandtree/commandspinbox.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     def stepBy(self, steps):
         prefix_len = len(self.prefix())
         min_pos = prefix_len + 1 if self.value() < 0 else prefix_len
 
         text = self.lineEdit().text()
         cur_pos = self.lineEdit().cursorPosition()
-        sep_pos = len(text) - len(self.suffix())
+        sep_pos = len(text)
 
         if cur_pos < min_pos:
             return
 
         exponent = sep_pos - cur_pos
 
         single_step = 10 ** exponent
@@ -32,82 +32,78 @@
         super().stepBy(steps)
 
         self.lineEdit().deselect()
 
         min_pos = prefix_len + 1 if self.value() < 0 else prefix_len
 
         text = self.lineEdit().text()
-        new_sep_pos = len(text) - len(self.suffix())
+        new_sep_pos = len(text)
 
         new_cur_pos = cur_pos + new_sep_pos - sep_pos
         if new_cur_pos < min_pos:
             new_cur_pos = min_pos
         self.lineEdit().setCursorPosition(new_cur_pos)
 
 
 class FloatSpinBox(QDoubleSpinBox):
     """
-    Adjust step size depending on the cursor position
+    Adjust step size depending on the cursor postion
     """
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.minimum_step = 0.1
         self.significant_figures = 4
-        self.precision = 3
-        self.decis = 3
+        self.precision = 1
 
     def set_minimum_step(self, value):
         self.minimum_step = value
         step = self.minimum_step if self.minimum_step > 1e-12 else 1e-12
-        self.decis = math.ceil(-math.log10(step))
+        self.decimals = math.ceil(math.log10(1.0 / step))
 
     def set_significant_figures(self, value):
         self.significant_figures = value
 
     def valueFromText(self, text):
         try:
             if self.suffix():
                 unit_len = len(self.suffix())
                 value = float(text[:-unit_len])
-
             else:
                 value = float(text)
             if value < self.minimum():
                 value = self.minimum()
             elif value > self.maximum():
                 value = self.maximum()
-
         except ValueError:
             print('valueFromText ValueError', text, self.suffix())
             value = self.minimum()
         return value
 
     def textFromValue(self, value):
-        prec = self.decis
+        prec = self.decimals
         try:
             if value == 0:
                 return '0.0'
 
             digits = math.ceil(math.log10(abs(value)))
-            """
+            # digits = 0 if digits < 0 else digits
+
             if digits == self.significant_figures:
                 step = 1
             else:
                 step = 10 ** (digits - self.significant_figures)
             value = round(value / step) * step
-            """
             prec = self.significant_figures - digits
-            prec = self.decis if prec > self.decis else prec
-            prec = 0 if prec < 0 else prec
-            self.precision = prec
-            format_string = '{:.' + str(prec) + 'f}'
-            text = format_string.format(value)
+            if prec > self.decimals:
+                prec = self.decimals
         except Exception as e:
             print(e)
-            return ''
+        self.precision = prec
+        format_string = '{:.' + str(prec) + 'f}'
+        text = format_string.format(value)
         return text
 
     def stepBy(self, steps):
         prefix_len = len(self.prefix())
         min_pos = prefix_len + 1 if self.value() < 0 else prefix_len
 
         text = self.lineEdit().text()
```

### Comparing `srsgui-0.2.15/srsgui/ui/commandtree/commandtreeview.py` & `srsgui-0.2.9/srsgui/ui/commandtree/commandtreeview.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import inspect
 import logging
 
 from srsgui.ui.qt.QtCore import Qt, QModelIndex
-from srsgui.ui.qt.QtWidgets import QTreeView, QApplication, QHeaderView
+from srsgui.ui.qt.QtWidgets import QTreeView, QApplication, QHeaderView, QPushButton
 
 from .commandmodel import CommandModel
 from .commanddelegate import CommandDelegate
 from .commandspinbox import RunButton
 
 
 class CommandTreeView(QTreeView):
@@ -47,20 +47,15 @@
         for i in range(self.model().rowCount(parent)):
             index = self.model().index(i, 0, parent)
             self.connect_methods_to_buttons(index)
             try:
                 item = index.internalPointer()
                 if item.is_method:
                     widget_index = self.model().index(i, 1, parent)
-                    spec = inspect.getfullargspec(item.comp)
-                    if spec.defaults is None:
-                        flag = len(spec.args) == 1
-                    else:
-                        flag = len(spec.args) - len(spec.defaults) == 1
-                    if flag:
+                    if len(inspect.getfullargspec(item.comp).args) == 1:
                         parent_comp = item.parent().comp
                         meth = getattr(parent_comp, item.name)
                         if meth and meth.__func__ in parent_comp.allow_run_button:
                             button = RunButton()
                             button.pressed.connect(meth)
                             self.setIndexWidget(widget_index, button)
             except Exception as e:
```

### Comparing `srsgui-0.2.15/srsgui/ui/commandtree/commandtreewidget.py` & `srsgui-0.2.9/srsgui/ui/commandtree/commandtreewidget.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,21 +60,20 @@
     def on_method_changed(self, state):
         self.tree_view.method_included = state
         self.tree_view.update_item_display()
 
     def on_raw_command_changed(self, state):
         self.tree_view.show_raw_command = state
         self.model.show_raw_remote_command = self.tree_view.show_raw_command
-        self.model.dataChanged.emit(QModelIndex(), QModelIndex())
 
     def on_capture_clicked(self):
         if self.inst is not None and self.inst.is_connected():
             try:
                 self.model.show_raw_remote_command = self.show_raw_command
-                self.model.load(self.inst)
+                self.model.load(self.inst, False)
                 self.tree_view.expandToDepth(1)
                 self.tree_view.resizeColumnToContents(0)
                 # self.tree_view.collapseAll()
                 self.tree_view.update_item_display()
                 self.tree_view.connect_methods_to_buttons()
 
             except Exception as e:
@@ -84,16 +83,14 @@
 
     def on_expand_clicked(self):
         self.tree_view.expandAll()
 
     def on_collapse_clicked(self):
         self.tree_view.collapseAll()
 
-    def closeEvent(self, event) -> None:
-        self.model.command_handler.stop()
 
 if __name__ == '__main__':
     import sys
     from srsgui.ui.qt.QtWidgets import QApplication, QHeaderView
     from srsinst.sr860 import SR860
 
     app = QApplication(sys.argv)
```

### Comparing `srsgui-0.2.15/srsgui/ui/commandtree/jsonmodel.py` & `srsgui-0.2.9/srsgui/ui/commandtree/jsonmodel.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/ui/commandtree/ui_commandcapturewidget.py` & `srsgui-0.2.9/srsgui/ui/commandtree/ui_commandcapturewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/ui/commandtree/ui_commandtreewidget.py` & `srsgui-0.2.9/srsgui/ui/commandtree/ui_commandtreewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/ui/connectdlg.py` & `srsgui-0.2.9/srsgui/ui/connectdlg.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/ui/deviceinfohandler.py` & `srsgui-0.2.9/srsgui/ui/deviceinfohandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/ui/dockhandler.py` & `srsgui-0.2.9/srsgui/ui/dockhandler.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,19 +8,15 @@
 
 from matplotlib.figure import Figure
 import matplotlib.image as mpimg
 
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
 
-from .commandhandler import CommandHandler as TerminalCommandHandler
-from .commandtree.commandhandler import CommandHandler as CommandTreeCommandHandler
-
 from .commandterminal import CommandTerminal
-
 # from .commandtree.commandcapturewidget import CommandCaptureWidget
 from .commandtree.commandtreewidget import CommandTreeWidget
 
 logger = logging.getLogger(__name__)
 
 # define matplotlib level before importing to suppress debug messages
 logging.getLogger('matplotlib').setLevel(logging.WARNING)
@@ -60,20 +56,14 @@
             parent.menu_Docks.triggered.disconnect()
         except:
             pass
         actions = parent.menu_Docks.actions()
         for action in actions:
             parent.menu_Docks.removeAction(action)
 
-        # terminal_command_handler needs to access to self.parent.inst_dict
-        self.terminal_command_handler = TerminalCommandHandler(self.parent)
-
-        # CommandItemModel uses command_tree_command_handler to access Commands
-        self.command_tree_command_handler = CommandTreeCommandHandler()
-
         self.init_figure_dock(self.DefaultFigureName)
         self.init_terminal()
         self.init_console()
         self.init_inst_dock('instrument info')
         list(self.dock_dict.values())[-1].hide()
 
         fig = self.dock_dict.pop(self.DefaultFigureName)
@@ -149,19 +139,14 @@
             terminal_dock.setWindowTitle(name)
             terminal_dock.setMinimumSize(250, 150)
 
             self.terminal_widget = CommandTerminal(self.parent)
             terminal_dock.setWidget(self.terminal_widget)
             self.parent.addDockWidget(Qt.RightDockWidgetArea, terminal_dock)
             self.dock_dict[name] = terminal_dock
-
-            # Commands from terminal are processed by terminal_command_handler
-            self.terminal_widget.command_requested.connect(self.terminal_command_handler.process_command)
-            self.terminal_command_handler.command_processed.connect(self.terminal_widget.handle_command)
-
         except Exception as e:
             logger.error(e)
 
     def init_inst_dock(self, name):
         try:
             inst_dock = QDockWidget(self.parent)
             inst_dock.setObjectName(name)
@@ -170,21 +155,14 @@
             title = self.TitleFormat.format(name)
             inst_dock.setWindowTitle(title)
             inst_dock.setMinimumSize(200, 350)
 
             # inst_dock.command_capture_widget = CommandCaptureWidget(self.parent)
             inst_dock.command_capture_widget = CommandTreeWidget(self.parent)
 
-            # Connect the command handler in parent to signals and slots in CommandModel
-            inst_dock.command_capture_widget.model.set_command_sent.connect(self.terminal_widget.handle_command)
-            inst_dock.command_capture_widget.model.query_requested.connect(self.command_tree_command_handler.worker.handle_query)
-            inst_dock.command_capture_widget.model.set_requested.connect(self.command_tree_command_handler.worker.handle_set)
-            self.command_tree_command_handler.worker.query_processed.connect(inst_dock.command_capture_widget.model.handle_command)
-            self.command_tree_command_handler.worker.set_processed.connect(inst_dock.command_capture_widget.model.handle_command)
-
             inst_dock.setWidget(inst_dock.command_capture_widget)
             self.parent.addDockWidget(Qt.LeftDockWidgetArea, inst_dock)
             self.dock_dict[title] = inst_dock
             self.active_inst_dock_names.append(title)
             if len(self.active_inst_dock_names) > 1:
                 self.parent.tabifyDockWidget(
                     self.dock_dict[self.active_inst_dock_names[0]], inst_dock)
@@ -380,11 +358,7 @@
                     dock.toolbar.show()
         else:
             self.action_toolbar.setText('Show Toolbar')
             self.toolbar_visible = False
             for dock in self.dock_dict.values():
                 if hasattr(dock, 'toolbar'):
                     dock.toolbar.hide()
-
-    def stop_command_handlers(self):
-        self.terminal_command_handler.stop()
-        self.command_tree_command_handler.stop()
```

### Comparing `srsgui-0.2.15/srsgui/ui/inputpanel.py` & `srsgui-0.2.9/srsgui/ui/inputpanel.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/ui/qt/QtCore.py` & `srsgui-0.2.9/srsgui/ui/qt/QtCore.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/ui/qt/QtGui.py` & `srsgui-0.2.9/srsgui/ui/qt/QtGui.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/ui/qt/QtWidgets.py` & `srsgui-0.2.9/srsgui/ui/qt/QtWidgets.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/ui/qt/__init__.py` & `srsgui-0.2.9/srsgui/ui/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/ui/qtloghandler.py` & `srsgui-0.2.9/srsgui/ui/qtloghandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/ui/resource_rc.py` & `srsgui-0.2.9/srsgui/ui/resource_rc.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/ui/signalhandler.py` & `srsgui-0.2.9/srsgui/ui/signalhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/ui/srslogo.jpg` & `srsgui-0.2.9/srsgui/ui/srslogo.jpg`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/ui/stdout.py` & `srsgui-0.2.9/srsgui/ui/stdout.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/ui/taskmain.py` & `srsgui-0.2.9/srsgui/ui/taskmain.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 
 from .inputpanel import InputPanel
 from .signalhandler import SignalHandler
 
 from .stdout import StdOut
 from .qtloghandler import QtLogHandler
 from .deviceinfohandler import DeviceInfoHandler
-
 from .dockhandler import DockHandler
+from .commandhandler import CommandHandler
 
 from srsgui.task.config import Config
 from srsgui.task.sessionhandler import SessionHandler
 from srsgui.task.task import Task, Bold
 
 from srsgui import __version__
 
@@ -73,20 +73,22 @@
         self.data_dict = {}
 
         # self.inst_dict holds instances of subclass of Instrument
         self.inst_dict = {}
         self.inst_info_handler = DeviceInfoHandler(self)
 
         self.dock_handler = DockHandler(self)
-        self.command_handler = self.dock_handler.terminal_command_handler
         self.console = self.dock_handler.console
         self.terminal_widget = self.dock_handler.terminal_widget
         self.plotDockWidget = self.dock_handler.get_dock()
 
         # Make the terminal not blocking for log query
+        self.command_handler = CommandHandler(self)
+        self.terminal_widget.command_requested.connect(self.command_handler.process_command)
+        self.command_handler.command_processed.connect(self.terminal_widget.handle_command)
 
         self.geometry_dict = {}
         try:
             default_config_file = self.DefaultConfigFile
             self.config = Config()
             self.base_data_dir = self.config.base_data_dir
             self.base_log_file_name = self.config.base_log_file_name
@@ -218,43 +220,44 @@
             for name in self.task_dict:
                 m = self.menu_Tasks
 
                 # set up submenu structure
                 p = self.config.task_path_dict[name]
                 if p:
                     tokens = p.split('/')
+                    exists = False
                     for token in tokens:
-                        exists = False
-                        na = None
                         if type(m) == QAction:
                             ma = m.menu()
                             if ma:
                                 m = ma
                             else:
                                 continue
                         for action in m.actions():
                             if token == action.text():
                                 na = action
                                 exists = True
                                 break
                         if not exists:
                             na = m.addMenu(QMenu(token, m))
                         m = na
+                        exists = False
                     if type(m) == QAction:
                         ma = m.menu()
                         if ma:
                             m = ma
                         else:
                             continue
                 action_task = QAction(self)
                 action_task.setText(name)
                 m.addAction(action_task)
         except Exception as e:
             logger.error('Error adding to Task menu Task:{}  Error: {}'.format(name, e))
 
+
     def get_logo_file(self):
         return self.LogoFile
 
     def print_redirect(self, text):
         """
         Handles text output for stdout, stderr and various text output
         from :class:`srsgui.task.task.Task`
@@ -553,15 +556,15 @@
             logger.error('display_question error: {}'.format(e))
 
     def closeEvent(self, event):
         if self.okToContinue():
             # Save settings
             self.save_settings()
 
-            self.dock_handler.stop_command_handlers()
+            self.command_handler.stop()
 
             # Close instruments
             inst_dict = self.inst_dict
             for key in inst_dict:
                 if hasattr(inst_dict[key], "disconnect"):
                     inst_dict[key].disconnect()
         else:
```

### Comparing `srsgui-0.2.15/srsgui/ui/taskmain.ui` & `srsgui-0.2.9/srsgui/ui/taskmain.ui`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui/ui/ui_taskmain.py` & `srsgui-0.2.9/srsgui/ui/ui_taskmain.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.15/srsgui.egg-info/PKG-INFO` & `srsgui-0.2.9/srsgui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.2.15
+Version: 0.2.9
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Keywords: instrument control,data acquisition,data visualization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `srsgui-0.2.15/srsgui.egg-info/SOURCES.txt` & `srsgui-0.2.9/srsgui.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,14 @@
 srsgui/ui/stdout.py
 srsgui/ui/taskmain.py
 srsgui/ui/taskmain.ui
 srsgui/ui/ui_taskmain.py
 srsgui/ui/commandtree/commandcapturewidget.py
 srsgui/ui/commandtree/commandcapturewidget.ui
 srsgui/ui/commandtree/commanddelegate.py
-srsgui/ui/commandtree/commandhandler.py
 srsgui/ui/commandtree/commanditem.py
 srsgui/ui/commandtree/commandmodel.py
 srsgui/ui/commandtree/commandspinbox.py
 srsgui/ui/commandtree/commandtreeview.py
 srsgui/ui/commandtree/commandtreewidget.py
 srsgui/ui/commandtree/jsonmodel.py
 srsgui/ui/commandtree/ui_commandcapturewidget.py
```

