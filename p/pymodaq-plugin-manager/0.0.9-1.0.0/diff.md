# Comparing `tmp/pymodaq_plugin_manager-0.0.9.tar.gz` & `tmp/pymodaq_plugin_manager-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pymodaq_plugin_manager-0.0.9.tar", last modified: Mon Nov 16 09:48:48 2020, max compression
+gzip compressed data, was "pymodaq_plugin_manager-1.0.0.tar", last modified: Tue Apr 25 16:22:57 2023, max compression
```

## Comparing `pymodaq_plugin_manager-0.0.9.tar` & `pymodaq_plugin_manager-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2020-11-16 09:48:48.000000 pymodaq_plugin_manager-0.0.9/
--rw-rw-rw-   0        0        0      120 2020-11-10 15:38:05.000000 pymodaq_plugin_manager-0.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0     1106 2020-11-16 09:48:48.000000 pymodaq_plugin_manager-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0    26413 2020-11-16 09:48:47.000000 pymodaq_plugin_manager-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2020-11-16 09:48:48.000000 pymodaq_plugin_manager-0.0.9/pymodaq_plugin_manager/
--rw-rw-rw-   0        0        0        0 2020-11-09 12:51:09.000000 pymodaq_plugin_manager-0.0.9/pymodaq_plugin_manager/__init__.py
-drwxrwxrwx   0        0        0        0 2020-11-16 09:48:48.000000 pymodaq_plugin_manager-0.0.9/pymodaq_plugin_manager/doc/
--rw-rw-rw-   0        0        0    26227 2020-11-16 09:48:47.000000 pymodaq_plugin_manager-0.0.9/pymodaq_plugin_manager/doc/PluginList.md
--rw-rw-rw-   0        0        0    15280 2020-11-16 09:48:25.000000 pymodaq_plugin_manager-0.0.9/pymodaq_plugin_manager/manager.py
-drwxrwxrwx   0        0        0        0 2020-11-16 09:48:48.000000 pymodaq_plugin_manager-0.0.9/pymodaq_plugin_manager/src/
--rw-rw-rw-   0        0        0    12924 2020-11-16 09:48:25.000000 pymodaq_plugin_manager-0.0.9/pymodaq_plugin_manager/src/PluginList.json
--rw-rw-rw-   0        0        0     2050 2020-11-10 10:16:16.000000 pymodaq_plugin_manager-0.0.9/pymodaq_plugin_manager/src/plugin_list.schema
--rw-rw-rw-   0        0        0     8852 2020-11-16 09:41:22.000000 pymodaq_plugin_manager-0.0.9/pymodaq_plugin_manager/validate.py
--rw-rw-rw-   0        0        0     3245 2020-11-12 12:09:09.000000 pymodaq_plugin_manager-0.0.9/pymodaq_plugin_manager/version.py
-drwxrwxrwx   0        0        0        0 2020-11-16 09:48:48.000000 pymodaq_plugin_manager-0.0.9/pymodaq_plugin_manager.egg-info/
--rw-rw-rw-   0        0        0     1106 2020-11-16 09:48:47.000000 pymodaq_plugin_manager-0.0.9/pymodaq_plugin_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      576 2020-11-16 09:48:47.000000 pymodaq_plugin_manager-0.0.9/pymodaq_plugin_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-11-16 09:48:47.000000 pymodaq_plugin_manager-0.0.9/pymodaq_plugin_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2020-11-16 09:48:47.000000 pymodaq_plugin_manager-0.0.9/pymodaq_plugin_manager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       49 2020-11-16 09:48:47.000000 pymodaq_plugin_manager-0.0.9/pymodaq_plugin_manager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2020-11-16 09:48:47.000000 pymodaq_plugin_manager-0.0.9/pymodaq_plugin_manager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-11-16 09:48:48.000000 pymodaq_plugin_manager-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1870 2020-11-12 15:41:48.000000 pymodaq_plugin_manager-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:22:57.715698 pymodaq_plugin_manager-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-25 16:22:45.000000 pymodaq_plugin_manager-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-25 16:22:45.000000 pymodaq_plugin_manager-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-25 16:22:57.715698 pymodaq_plugin_manager-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    47137 2023-04-25 16:22:45.000000 pymodaq_plugin_manager-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    74359 2023-04-25 16:22:45.000000 pymodaq_plugin_manager-1.0.0/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 16:22:57.715698 pymodaq_plugin_manager-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-25 16:22:45.000000 pymodaq_plugin_manager-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:22:57.711697 pymodaq_plugin_manager-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:22:57.715698 pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-25 16:22:45.000000 pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:22:57.715698 pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    12424 2023-04-25 16:22:45.000000 pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager/data/PluginList.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-25 16:22:45.000000 pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager/data/plugin_list.schema
+-rw-r--r--   0 runner    (1001) docker     (123)    16410 2023-04-25 16:22:45.000000 pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-04-25 16:22:45.000000 pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14734 2023-04-25 16:22:45.000000 pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:22:57.715698 pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-25 16:22:57.000000 pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-25 16:22:57.000000 pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:22:57.000000 pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-25 16:22:57.000000 pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-25 16:22:57.000000 pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 16:22:57.000000 pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pymodaq_plugin_manager-0.0.9/pymodaq_plugin_manager/manager.py` & `pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager/manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,357 +1,387 @@
-import sys
-import subprocess
-from PyQt5 import QtWidgets, QtCore
-from PyQt5.QtCore import Qt, QVariant, pyqtSlot, pyqtSignal
-from pymodaq.daq_utils import gui_utils as gutils
-from pymodaq_plugin_manager.validate import validate_json_plugin_list, get_plugins, get_plugin, get_check_repo,\
-    find_dict_in_list_from_key_val
-import numpy as np
-from yawrap import Doc
-from pymodaq_plugin_manager.validate import get_pypi_pymodaq
-from packaging import version as version_mod
-from pymodaq_plugin_manager.version import get_version
-from pymodaq.daq_utils import daq_utils as utils
-logger = utils.set_logger(utils.get_module_name(__file__))
-config = utils.load_config()
-
-
-class TableModel(gutils.TableModel):
-
-    def __init__(self, *args, plugins=[], **kwargs):
-        super().__init__(*args, **kwargs)
-        self._selected = [False for ind in range(len(self._data))]
-        self.plugins = plugins
-
-    @property
-    def selected(self):
-        return self._selected
-
-    def flags(self, index):
-        f = super().flags(index)
-        if index.column() == 0:
-            f |= Qt.ItemIsUserCheckable
-        return f
-
-    def data(self, index, role=Qt.DisplayRole):
-        if index.isValid():
-            if role == Qt.DisplayRole or role == Qt.EditRole:
-                if index.column() == 0:
-                    dat = self._data[index.row()][0]
-                else:
-                    dat = self._data[index.row()][index.column()]
-                return dat
-            elif role == Qt.CheckStateRole:
-                if index.column() == 0:
-                    if self._selected[index.row()]:
-                        return Qt.Checked
-                    else:
-                        return Qt.Unchecked
-        return QVariant()
-
-    def setData(self, index, value, role):
-        if index.isValid():
-            if role == Qt.EditRole:
-                if self.validate_data(index.row(), index.column(), value):
-                    self._data[index.row()][index.column()] = value
-                    self.dataChanged.emit(index, index, [role])
-                    return True
-
-                else:
-                    return False
-            if role == Qt.CheckStateRole:
-                if index.column() == 0:
-                    self._selected[index.row()] = value == Qt.Checked
-                    self.dataChanged.emit(index, index, [role])
-                    return True
-        return False
-
-
-class FilterProxy(QtCore.QSortFilterProxyModel):
-
-    def __init__(self, parent=None):
-        super().__init__(parent)
-
-        self.textRegExp = QtCore.QRegExp()
-        self.textRegExp.setCaseSensitivity(QtCore.Qt.CaseInsensitive)
-        self.textRegExp.setPatternSyntax(QtCore.QRegExp.Wildcard)
-
-    def filterAcceptsRow(self, sourcerow, parent_index):
-        plugin_index = self.sourceModel().index(sourcerow, 0, parent_index)
-        try:
-            plugin = self.sourceModel().plugins[plugin_index.row()]
-            match = False
-            if not not plugin:
-                match = match or self.textRegExp.pattern().lower() in plugin['plugin-name'].lower()
-                match = match or self.textRegExp.pattern().lower() in plugin['display-name'].lower()
-                match = match or self.textRegExp.pattern().lower() in plugin['description'].lower()
-                for plug in plugin['instruments']:
-                    match = match | any(self.textRegExp.pattern().lower() in p.lower() for p in plugin['instruments'][plug])
-            return match
-        except Exception as e:
-            print(e)
-            return True
-
-    def setTextFilter(self, regexp):
-        self.textRegExp.setPattern(regexp)
-        self.invalidateFilter()
-
-
-
-
-class PluginManager(QtCore.QObject):
-
-    quit_signal = pyqtSignal()
-    restart_signal = pyqtSignal()
-
-    def __init__(self, parent, standalone=False):
-        super().__init__()
-        self.parent = parent
-        self.parent.setLayout(QtWidgets.QVBoxLayout())
-        self.standalone = standalone
-
-        #self.parent.setMinimumSize(1000, 500)
-
-        self.plugins_available, self.plugins_installed, self.plugins_update = get_plugins()
-
-        self.setup_UI()
-
-
-        if config['general']['check_version']:
-            self.check_version(show=False)
-
-    def check_version(self, show=True):
-        try:
-            current_version = version_mod.parse(get_version())
-            available_version = [version_mod.parse(ver['version']) for ver in get_pypi_pymodaq('pymodaq-plugin-manager')]
-            msgBox = QtWidgets.QMessageBox()
-            if max(available_version) > current_version:
-                msgBox.setText(f"A new version of PyMoDAQ Plugin Manager is available, {str(max(available_version))}!")
-                msgBox.setInformativeText("Do you want to install it?")
-                msgBox.setStandardButtons(msgBox.Ok | msgBox.Cancel)
-                msgBox.setDefaultButton(msgBox.Ok)
-
-                ret = msgBox.exec()
-
-                if ret == msgBox.Ok:
-                    command = [sys.executable, '-m', 'pip', 'install', f'pymodaq-plugin-manager=={str(max(available_version))}']
-                    subprocess.Popen(command)
-
-                self.restart()
-            else:
-                if show:
-                    msgBox.setText(f"Your version of PyMoDAQ Plugin Manager, {str(current_version)}, is up to date!")
-                    ret = msgBox.exec()
-        except Exception as e:
-            logger.exception("Error while checking the available PyMoDAQ version")
-
-    def quit(self):
-        self.parent.parent().close()
-        self.quit_signal.emit()
-
-    def restart(self):
-        self.parent.parent().close()
-        if self.standalone:
-            subprocess.call([sys.executable, __file__])
-        else:
-            self.restart_signal.emit()
-
-    def setup_UI(self):
-
-        settings_widget = QtWidgets.QWidget()
-        settings_widget.setLayout(QtWidgets.QHBoxLayout())
-        self.plugin_choice = QtWidgets.QComboBox()
-        self.plugin_choice.addItems(['Available', 'Update', 'Installed'])
-        self.plugin_choice.currentTextChanged.connect(self.update_model)
-
-        self.check_updates_pb = QtWidgets.QPushButton('Check Updates')
-        self.check_updates_pb.clicked.connect(lambda: self.check_version(True))
-
-        self.search_edit = QtWidgets.QLineEdit()
-        self.search_edit.setPlaceholderText("Plugin name")
-        settings_widget.layout().addWidget(self.plugin_choice)
-        settings_widget.layout().addStretch()
-        settings_widget.layout().addWidget(self.check_updates_pb)
-        settings_widget.layout().addStretch()
-        settings_widget.layout().addWidget(QtWidgets.QLabel('Search:'))
-        settings_widget.layout().addWidget(self.search_edit)
-        settings_widget.layout().addStretch()
-        self.action_button = QtWidgets.QPushButton('Install')
-        self.action_button.setEnabled(False)
-        self.action_button.clicked.connect(self.do_action)
-        settings_widget.layout().addWidget(self.action_button)
-
-
-        self.parent.layout().addWidget(settings_widget)
-
-        splitter = QtWidgets.QSplitter(Qt.Vertical)
-
-        self.table_view = gutils.TableView()
-
-        styledItemDelegate = QtWidgets.QStyledItemDelegate()
-        styledItemDelegate.setItemEditorFactory(gutils.SpinBoxDelegate())
-        self.table_view.setItemDelegate(styledItemDelegate)
-        self.table_view.horizontalHeader().show()
-        self.table_view.horizontalHeader().setSectionResizeMode(QtWidgets.QHeaderView.ResizeToContents)
-
-        self.model_available = TableModel([[plugin['display-name'],
-                                            plugin['version']] for plugin in self.plugins_available],
-                                          header=['Plugin', 'Version'],
-                                          editable=[False, False],
-                                          plugins=self.plugins_available)
-        self.model_update = TableModel([[plugin['display-name'],
-                                         plugin['version']] for plugin in self.plugins_update],
-                                       header=['Plugin', 'Version'],
-                                       editable=[False, False],
-                                          plugins=self.plugins_update)
-        self.model_installed = TableModel([[plugin['display-name'],
-                                            plugin['version']] for plugin in self.plugins_installed],
-                                          header=['Plugin', 'Version'],
-                                          editable=[False, False],
-                                          plugins=self.plugins_installed)
-
-        model_available_proxy = FilterProxy()
-        model_available_proxy.setSourceModel(self.model_available)
-        self.search_edit.textChanged.connect(model_available_proxy.setTextFilter)
-        self.table_view.setModel(model_available_proxy)
-        self.table_view.setSortingEnabled(True)
-        self.table_view.clicked.connect(self.item_clicked)
-
-        self.info_widget = QtWidgets.QTextEdit()
-        self.info_widget.setReadOnly(True)
-
-        splitter.addWidget(self.table_view)
-        splitter.addWidget(self.info_widget)
-
-        self.parent.layout().addWidget(splitter)
-
-    def do_action(self):
-        if self.plugin_choice.currentText() == 'Available':
-            action = 'install'
-            plugins = [plug[0] for ind, plug in enumerate(self.model_available.get_data_all())
-                       if self.model_available.selected[ind]]
-        elif self.plugin_choice.currentText() == 'Update':
-            action = 'update'
-            plugins = [plug[0] for ind, plug in enumerate(self.model_update.get_data_all())
-                       if self.model_update.selected[ind]]
-        elif self.plugin_choice.currentText() == 'Installed':
-            action = 'remove'
-            plugins = [plug[0] for ind, plug in enumerate(self.model_installed.get_data_all())
-                       if self.model_installed.selected[ind]]
-
-        msgBox = QtWidgets.QMessageBox()
-        msgBox.setText(f"You will {action} this list of plugins: {plugins}")
-        msgBox.setInformativeText("Do you want to proceed?")
-        msgBox.setStandardButtons(msgBox.Ok | msgBox.Cancel)
-        msgBox.setDefaultButton(msgBox.Ok)
-
-        ret = msgBox.exec()
-        self.info_widget.clear()
-        if ret == msgBox.Ok:
-            for plug in plugins:
-                plugin_dict = get_plugin(plug)
-                if self.plugin_choice.currentText() == 'Available' or self.plugin_choice.currentText() == 'Update':
-                    rep = get_check_repo(plugin_dict)
-                    if rep is None:
-                        command = [sys.executable, '-m', 'pip', 'install', plugin_dict['repository']]
-                        self.do_subprocess(command)
-                    else:
-                        self.info_widget.insertPlainText(rep)
-
-
-                elif self.plugin_choice.currentText() == 'Installed':
-                    command = [sys.executable, '-m', 'pip', 'uninstall', '--yes', plugin_dict['plugin-name']]
-                    self.do_subprocess(command)
-
-        msgBox = QtWidgets.QMessageBox()
-        msgBox.setText(f"All actions were performed!")
-        msgBox.setInformativeText(f"Do you want to quit and restart the application to take into account the modifications?")
-        msgBox.setStandardButtons(msgBox.Close | msgBox.Cancel)
-        restart_button = msgBox.addButton('Restart', msgBox.ApplyRole)
-        msgBox.setDefaultButton(msgBox.Close)
-        ret = msgBox.exec()
-        if ret == msgBox.Close:
-            self.quit()
-        elif msgBox.clickedButton() is restart_button:
-            self.restart()
-
-    def do_subprocess(self, command):
-        with subprocess.Popen(command, stdout=subprocess.PIPE, stdin=subprocess.PIPE, stderr=subprocess.PIPE,
-                              bufsize=1) as sp:
-            for line in sp.stdout:
-                self.info_widget.insertPlainText(line.decode())
-                QtWidgets.QApplication.processEvents()
-            for line in sp.stderr:
-                self.info_widget.insertPlainText(line.decode())
-                QtWidgets.QApplication.processEvents()
-
-    def update_model(self, plugin_choice):
-        self.search_edit.textChanged.disconnect()
-        model_proxy = FilterProxy()
-        if plugin_choice == 'Available':
-            model_proxy.setSourceModel(self.model_available)
-            self.action_button.setText('Install')
-        elif plugin_choice == 'Update':
-            model_proxy.setSourceModel(self.model_update)
-            self.action_button.setText('Update')
-        elif plugin_choice == 'Installed':
-            model_proxy.setSourceModel(self.model_installed)
-            self.action_button.setText('Remove')
-        self.search_edit.textChanged.connect(model_proxy.setTextFilter)
-        self.table_view.setModel(model_proxy)
-        self.item_clicked(model_proxy.index(0, 0))
-
-
-    def item_clicked(self, index):
-        if index.isValid():
-            self.display_info(index)
-            self.action_button.setEnabled(np.any(index.model().sourceModel().selected))
-
-
-
-    def display_info(self, index):
-        self.info_widget.clear()
-        if index.isValid():
-            if self.plugin_choice.currentText() == 'Available':
-                plugin = self.plugins_available[index.model().mapToSource(index).row()]
-            elif self.plugin_choice.currentText() == 'Update':
-                plugin = self.plugins_update[index.model().mapToSource(index).row()]
-            elif self.plugin_choice.currentText() == 'Installed':
-                plugin = self.plugins_installed[index.model().mapToSource(index).row()]
-            doc, tag, text = Doc().tagtext()
-
-            with tag('p'):
-                text(plugin['description'])
-
-            if not not plugin['authors']:
-                text('Authors:')
-                with tag('ul'):
-                    for inst in plugin['authors']:
-                        with tag('li'):
-                            text(inst)
-
-            if not not plugin['instruments']:
-                with tag('p'):
-                    text('This package include plugins for the instruments listed below:')
-                for inst in plugin['instruments']:
-                    with tag('p'):
-                        text(f'{inst}:')
-                    with tag('ul'):
-                        for instt in plugin['instruments'][inst]:
-                            with tag('li'):
-                                text(instt)
-            self.info_widget.insertHtml(doc.getvalue())
-
-
-def main():
-    app = QtWidgets.QApplication(sys.argv)
-    win = QtWidgets.QMainWindow()
-    win.setWindowTitle('PyMoDAQ Plugin Manager')
-    widget = QtWidgets.QWidget()
-    win.setCentralWidget(widget)
-    prog = PluginManager(widget, standalone=True)
-    win.show()
-    sys.exit(app.exec_())
-
-
-if __name__ == '__main__':
-    main()
+import logging
+from packaging import version as version_mod
+import sys
+import subprocess
+
+
+import numpy as np
+from qtpy import QtWidgets, QtCore
+from qtpy.QtCore import Qt, Slot, Signal
+from qtpy.QtGui import QTextCursor
+from readme_renderer.rst import render
+
+from pymodaq_plugin_manager.validate import validate_json_plugin_list, get_plugins, get_plugin, get_check_repo,\
+    find_dict_in_list_from_key_val
+from pymodaq_plugin_manager.validate import get_pypi_pymodaq
+from pymodaq_plugin_manager import __version__ as version
+from pymodaq_plugin_manager.utils import QVariant, TableModel, TableView, SpinBoxDelegate, get_pymodaq_version
+
+logger = logging.getLogger(__name__)
+# logger.addHandler(logging.NullHandler())
+
+
+class TableModel(TableModel):
+
+    def __init__(self, *args, plugins=[], **kwargs):
+        super().__init__(*args, **kwargs)
+        self._selected = [False for ind in range(len(self._data))]
+        self.plugins = plugins
+
+    @property
+    def selected(self):
+        return self._selected
+
+    def flags(self, index):
+        f = super().flags(index)
+        if index.column() == 0:
+            f |= Qt.ItemIsUserCheckable
+        return f
+
+    def data(self, index, role=Qt.DisplayRole):
+        if index.isValid():
+            if role == Qt.DisplayRole or role == Qt.EditRole:
+                if index.column() == 0:
+                    dat = self._data[index.row()][0]
+                else:
+                    dat = self._data[index.row()][index.column()]
+                return dat
+            elif role == Qt.CheckStateRole:
+                if index.column() == 0:
+                    if self._selected[index.row()]:
+                        return Qt.Checked
+                    else:
+                        return Qt.Unchecked
+        return QVariant()
+
+    def setData(self, index, value, role):
+        if index.isValid():
+            if role == Qt.EditRole:
+                if self.validate_data(index.row(), index.column(), value):
+                    self._data[index.row()][index.column()] = value
+                    self.dataChanged.emit(index, index, [role])
+                    return True
+
+                else:
+                    return False
+            if role == Qt.CheckStateRole:
+                if index.column() == 0:
+                    self._selected[index.row()] = value == Qt.Checked
+                    self.dataChanged.emit(index, index, [role])
+                    return True
+        return False
+
+
+class FilterProxy(QtCore.QSortFilterProxyModel):
+
+    def __init__(self, parent=None):
+        super().__init__(parent)
+
+        self.textRegExp = QtCore.QRegExp()
+        self.textRegExp.setCaseSensitivity(QtCore.Qt.CaseInsensitive)
+        self.textRegExp.setPatternSyntax(QtCore.QRegExp.Wildcard)
+
+    def filterAcceptsRow(self, sourcerow, parent_index):
+        plugin_index = self.sourceModel().index(sourcerow, 0, parent_index)
+        try:
+            plugin = self.sourceModel().plugins[plugin_index.row()]
+            match = False
+            if not not plugin:
+                match = match or self.textRegExp.pattern().lower() in plugin['plugin-name'].lower()
+                match = match or self.textRegExp.pattern().lower() in plugin['display-name'].lower()
+                match = match or self.textRegExp.pattern().lower() in plugin['description'].lower()
+                for plug in plugin['instruments']:
+                    match = match | any(self.textRegExp.pattern().lower() in p.lower() for p in plugin['instruments'][plug])
+            return match
+        except Exception as e:
+            print(e)
+            return True
+
+    def setTextFilter(self, regexp):
+        self.textRegExp.setPattern(regexp)
+        self.invalidateFilter()
+
+
+class PluginManager(QtCore.QObject):
+
+    quit_signal = Signal()
+    restart_signal = Signal()
+
+    def __init__(self, parent, standalone=False):
+        super().__init__()
+        self.parent = parent
+        self.parent.setLayout(QtWidgets.QVBoxLayout())
+        self.standalone = standalone
+
+        self.plugins_available, self.plugins_installed,\
+            self.plugins_update = get_plugins(False, pymodaq_version=get_pymodaq_version())
+
+        self.setup_UI()
+
+    def check_version(self, show=True):
+        try:
+            current_version = version_mod.parse(version)
+            available_version = [version_mod.parse(ver) for ver in
+                                 get_pypi_pymodaq('pymodaq-plugin-manager')['versions']]
+            msgBox = QtWidgets.QMessageBox()
+            if max(available_version) > current_version:
+                msgBox.setText(f"A new version of PyMoDAQ Plugin Manager is available, {str(max(available_version))}!")
+                msgBox.setInformativeText("Do you want to install it?")
+                msgBox.setStandardButtons(msgBox.Ok | msgBox.Cancel)
+                msgBox.setDefaultButton(msgBox.Ok)
+
+                ret = msgBox.exec()
+
+                if ret == msgBox.Ok:
+                    command = [sys.executable, '-m', 'pip', 'install', f'pymodaq-plugin-manager=={str(max(available_version))}']
+                    subprocess.Popen(command)
+
+                    self.restart()
+            else:
+                if show:
+                    msgBox.setText(f"Your version of PyMoDAQ Plugin Manager, {str(current_version)}, is up to date!")
+                    ret = msgBox.exec()
+        except Exception as e:
+            logger.exception("Error while checking the available PyMoDAQ version")
+
+    def quit(self):
+        self.parent.parent().close()
+        self.quit_signal.emit()
+
+    def restart(self):
+        self.parent.parent().close()
+        if self.standalone:
+            subprocess.call([sys.executable, __file__])
+        else:
+            self.restart_signal.emit()
+
+    def setup_UI(self):
+
+        settings_widget = QtWidgets.QWidget()
+        settings_widget.setLayout(QtWidgets.QHBoxLayout())
+        self.plugin_choice = QtWidgets.QComboBox()
+        self.plugin_choice.addItems(['Available', 'Update', 'Installed'])
+        self.plugin_choice.currentTextChanged.connect(self.update_model)
+
+        self.check_updates_pb = QtWidgets.QPushButton('Check Updates')
+        self.check_updates_pb.clicked.connect(lambda: self.check_version(True))
+
+        self.search_edit = QtWidgets.QLineEdit()
+        self.search_edit.setPlaceholderText("Plugin name")
+
+        settings_widget.layout().addWidget(self.plugin_choice)
+        settings_widget.layout().addStretch()
+        settings_widget.layout().addWidget(self.check_updates_pb)
+        settings_widget.layout().addStretch()
+        settings_widget.layout().addWidget(QtWidgets.QLabel('Search:'))
+        settings_widget.layout().addWidget(self.search_edit)
+        settings_widget.layout().addStretch()
+
+        pymodaq_version = QtWidgets.QLabel(f'PyMoDAQ Version: {get_pymodaq_version()}')
+        settings_widget.layout().addWidget(pymodaq_version)
+
+        settings_widget.layout().addStretch()
+        self.action_button = QtWidgets.QPushButton('Install')
+        self.action_button.setEnabled(False)
+        self.action_button.clicked.connect(self.do_action)
+        settings_widget.layout().addWidget(self.action_button)
+
+
+        self.parent.layout().addWidget(settings_widget)
+
+        splitter = QtWidgets.QSplitter(Qt.Vertical)
+
+        self.table_view = TableView()
+
+        styledItemDelegate = QtWidgets.QStyledItemDelegate()
+        styledItemDelegate.setItemEditorFactory(SpinBoxDelegate())
+        self.table_view.setItemDelegate(styledItemDelegate)
+        self.table_view.horizontalHeader().show()
+        self.table_view.horizontalHeader().setSectionResizeMode(QtWidgets.QHeaderView.ResizeToContents)
+
+        self.model_available = TableModel([[plugin['display-name'],
+                                            plugin['version']] for plugin in self.plugins_available],
+                                          header=['Plugin', 'Version'],
+                                          editable=[False, False],
+                                          plugins=self.plugins_available)
+        self.model_update = TableModel([[plugin['display-name'],
+                                         plugin['version']] for plugin in self.plugins_update],
+                                       header=['Plugin', 'Version'],
+                                       editable=[False, False],
+                                       plugins=self.plugins_update)
+        self.model_installed = TableModel([[plugin['display-name'],
+                                            plugin['version']] for plugin in self.plugins_installed],
+                                          header=['Plugin', 'Version'],
+                                          editable=[False, False],
+                                          plugins=self.plugins_installed)
+
+        model_available_proxy = FilterProxy()
+        model_available_proxy.setSourceModel(self.model_available)
+        self.search_edit.textChanged.connect(model_available_proxy.setTextFilter)
+        self.table_view.setModel(model_available_proxy)
+        self.table_view.setSortingEnabled(True)
+        self.table_view.clicked.connect(self.item_clicked)
+
+        self.info_widget = QtWidgets.QTextEdit()
+        self.info_widget.setReadOnly(True)
+
+        splitter.addWidget(self.table_view)
+        splitter.addWidget(self.info_widget)
+
+        self.parent.layout().addWidget(splitter)
+
+    def do_action(self):
+        indexes_plugin = []
+        plugins = []
+        if self.plugin_choice.currentText() == 'Available':
+            action = 'install'
+            for ind, plug in enumerate(self.model_available.get_data_all()):
+                if self.model_available.selected[ind]:
+                    plugins.append(plug[0])
+                    indexes_plugin.append(ind)
+        elif self.plugin_choice.currentText() == 'Update':
+            action = 'update'
+            for ind, plug in enumerate(self.model_update.get_data_all()):
+                if self.model_update.selected[ind]:
+                    plugins.append(plug[0])
+                    indexes_plugin.append(ind)
+        elif self.plugin_choice.currentText() == 'Installed':
+            action = 'remove'
+            for ind, plug in enumerate(self.model_installed.get_data_all()):
+                if self.model_installed.selected[ind]:
+                    plugins.append(plug[0])
+                    indexes_plugin.append(ind)
+
+        msgBox = QtWidgets.QMessageBox()
+        msgBox.setText(f"You will {action} this list of plugins: {plugins}")
+        msgBox.setInformativeText("Do you want to proceed?")
+        msgBox.setStandardButtons(msgBox.Ok | msgBox.Cancel)
+        msgBox.setDefaultButton(msgBox.Ok)
+
+        ret = msgBox.exec()
+        self.info_widget.clear()
+        if ret == msgBox.Ok:
+            for index in indexes_plugin:
+                # plugin_dict = get_plugin(plug)
+                if self.plugin_choice.currentText() == 'Available' or self.plugin_choice.currentText() == 'Update':
+                    if self.plugin_choice.currentText() == 'Available':
+                        plugin_dict = self.plugins_available[index]
+                    else:
+                        plugin_dict = self.plugins_update[index]
+                    if plugin_dict is not None:
+                        command = [sys.executable, '-m', 'pip', 'install',
+                                   f'{plugin_dict["plugin-name"]}=={plugin_dict["version"]}']
+                        self.do_subprocess(command)
+                    else:
+                        self.info_widget.insertPlainText(f'Plugin {plugin_dict["plugin-name"]} not found!')
+
+                elif self.plugin_choice.currentText() == 'Installed':
+                    plugin_dict = self.plugins_installed[index]
+                    command = [sys.executable, '-m', 'pip', 'uninstall', '--yes', plugin_dict['plugin-name']]
+                    self.do_subprocess(command)
+
+        msgBox = QtWidgets.QMessageBox()
+        msgBox.setText(f"All actions were performed!")
+        msgBox.setInformativeText(f"Do you want to quit and restart the application to take into account the modifications?")
+        msgBox.setStandardButtons(msgBox.Close | msgBox.Cancel)
+        restart_button = msgBox.addButton('Restart', msgBox.ApplyRole)
+        msgBox.setDefaultButton(msgBox.Close)
+        ret = msgBox.exec()
+        if ret == msgBox.Close:
+            self.quit()
+        elif msgBox.clickedButton() is restart_button:
+            self.restart()
+
+    def do_subprocess(self, command):
+        try:
+            self.info_widget.moveCursor(QTextCursor.End)
+            self.info_widget.insertPlainText(' '.join(command))
+            self.info_widget.moveCursor(QTextCursor.End)
+
+            with subprocess.Popen(command, stdout=subprocess.PIPE, universal_newlines=True, shell=True) as sp:
+                while True:
+                    self.info_widget.moveCursor(QTextCursor.End)
+                    self.info_widget.insertPlainText(sp.stdout.readline())
+                    self.info_widget.moveCursor(QTextCursor.End)
+                    QtWidgets.QApplication.processEvents()
+                    return_code = sp.poll()
+                    if return_code is not None:
+                        self.info_widget.insertPlainText(str(return_code))
+                        for output in sp.stdout.readlines():
+                            print(output.strip())
+                        break
+        except Exception as e:
+            logger.info(str(e))
+            subprocess.Popen(command)
+
+    def update_model(self, plugin_choice):
+        self.search_edit.textChanged.disconnect()
+        model_proxy = FilterProxy()
+        if plugin_choice == 'Available':
+            model_proxy.setSourceModel(self.model_available)
+            self.action_button.setText('Install')
+        elif plugin_choice == 'Update':
+            model_proxy.setSourceModel(self.model_update)
+            self.action_button.setText('Update')
+        elif plugin_choice == 'Installed':
+            model_proxy.setSourceModel(self.model_installed)
+            self.action_button.setText('Remove')
+        self.search_edit.textChanged.connect(model_proxy.setTextFilter)
+        self.table_view.setModel(model_proxy)
+        self.item_clicked(model_proxy.index(0, 0))
+
+
+    def item_clicked(self, index):
+        if index.isValid():
+            self.display_info(index)
+            self.action_button.setEnabled(bool(np.any(index.model().sourceModel().selected)))
+
+
+
+    def display_info(self, index):
+        self.info_widget.clear()
+        if index.isValid():
+            if self.plugin_choice.currentText() == 'Available':
+                plugin = self.plugins_available[index.model().mapToSource(index).row()]
+            elif self.plugin_choice.currentText() == 'Update':
+                plugin = self.plugins_update[index.model().mapToSource(index).row()]
+            elif self.plugin_choice.currentText() == 'Installed':
+                plugin = self.plugins_installed[index.model().mapToSource(index).row()]
+            # doc, tag, text = Doc().tagtext()
+            #
+            # with tag('p'):
+            #     text(plugin['description'])
+            #
+            # if not not plugin['authors']:
+            #     text('Authors:')
+            #     with tag('ul'):
+            #         for inst in plugin['authors']:
+            #             with tag('li'):
+            #                 text(inst)
+            #
+            # if not not plugin['instruments']:
+            #     with tag('p'):
+            #         text('This package include plugins for the instruments listed below:')
+            #     for inst in plugin['instruments']:
+            #         with tag('p'):
+            #             text(f'{inst}:')
+            #         with tag('ul'):
+            #             for instt in plugin['instruments'][inst]:
+            #                 with tag('li'):
+            #                     text(instt)
+            # self.info_widget.insertHtml(doc.getvalue())
+            self.info_widget.insertHtml(render(plugin['description']))
+
+
+def main():
+    app = QtWidgets.QApplication(sys.argv)
+    win = QtWidgets.QMainWindow()
+    win.setWindowTitle('PyMoDAQ Plugin Manager')
+    widget = QtWidgets.QWidget()
+    win.setCentralWidget(widget)
+    prog = PluginManager(widget, standalone=True)
+    win.show()
+    sys.exit(app.exec_())
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `pymodaq_plugin_manager-0.0.9/pymodaq_plugin_manager/src/PluginList.json` & `pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager/data/PluginList.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8151041666666666%*

 * *Differences: {"'pymodaq-plugins'": "{0: {'version': '3.0.2', 'id': "*

 * *                      "'52000a1191dbf8e9903708b77ac3fa82a3c41d91af328ad5d0362c4d449cdebe', "*

 * *                      "'repository': "*

 * *                      "'https://github.com/PyMoDAQ/pymodaq_plugins/archive/3.0.1.tar.gz', "*

 * *                      "'description': 'Plugins initially developed with PyMoDAQ\\r\\nIncludes Mock "*

 * *                      'plugins that are plugins of virtual instruments dedicated to code testing a '*

 * *                      "new fun […]*

```diff
@@ -2,18 +2,18 @@
     "name": "pymodaq-pluginList",
     "pymodaq-plugins": [
         {
             "authors": [
                 "Sebastien Weber"
             ],
             "contributors": [],
-            "description": "Plugins initially developed with PyMoDAQ\r\nIncludes Mock plugins that are plugins of virtual instruments dedicated to code testing a new functionalities development. The list of included plugins can be found on https://docs.google.com/spreadsheets/d/1wfMfvLwTitZd2R2m1O5i6wVEaX1lJBahP2HUbxVdidg",
+            "description": "Plugins initially developed with PyMoDAQ\r\nIncludes Mock plugins that are plugins of virtual instruments dedicated to code testing a new functionalities development.",
             "display-name": "Default",
-            "homepage": "https://github.com/CEMES-CNRS/pymodaq_plugins",
-            "id": "d1f66d6066e28d76335c40213ee6569ab5d52849e490a5475b39283e8e3d6a1f",
+            "homepage": "https://github.com/PyMoDAQ/pymodaq_plugins",
+            "id": "52000a1191dbf8e9903708b77ac3fa82a3c41d91af328ad5d0362c4d449cdebe",
             "instruments": {
                 "Actuator": [
                     "Mock actuator to test PyMoDAQ functionnalities",
                     "TCP server to communicate with other DAQ_Move or third party applications"
                 ],
                 "Viewer0D": [
                     "Mock detector to test PyMoDAQ functionnalities",
@@ -30,248 +30,248 @@
                     "TCP server to communicate with other DAQ_Viewer or third party applications"
                 ],
                 "ViewerND": [
                     "Mock actuator to test PyMoDAQ functionnalities"
                 ]
             },
             "plugin-name": "pymodaq_plugins",
-            "repository": "https://github.com/CEMES-CNRS/pymodaq_plugins/archive/3.0.0.tar.gz",
-            "version": "3.0.1"
+            "repository": "https://github.com/PyMoDAQ/pymodaq_plugins/archive/3.0.1.tar.gz",
+            "version": "3.0.2"
         },
         {
             "authors": [
                 "Sebastien Weber"
             ],
             "contributors": [
                 "Amelie Jarnac"
             ],
             "description": "Plugin devoted to the National Instrument signal acquisition and generation using the NiDAQmx library. Includes an actuator plugin for signal generation, a 1D viewer plugin for data acquisition as a function of time and a 0D viewer plugin for quick time averaging acquisition",
             "display-name": "National Instrument DAQmx",
-            "homepage": "https://github.com/CEMES-CNRS/pymodaq_plugins_daqmx",
+            "homepage": "https://github.com/PyMoDAQ/pymodaq_plugins_daqmx",
             "id": "3b4a50f1c0808343480cfbd400c6417cfa4267219d091d58441010d52eb502e3",
             "instruments": {
                 "Actuator": [
                     "Analog output DC, Sinus, Ramp..."
                 ],
                 "Viewer0D": [
                     "Analog acquisition",
                     "Counting"
                 ],
                 "Viewer1D": [
                     "Analog acquisition"
                 ]
             },
             "plugin-name": "pymodaq_plugins_daqmx",
-            "repository": "https://github.com/CEMES-CNRS/pymodaq_plugins_daqmx/archive/0.0.2.tar.gz",
+            "repository": "https://github.com/PyMoDAQ/pymodaq_plugins_daqmx/archive/0.0.2.tar.gz",
             "version": "0.0.2"
         },
         {
             "authors": [
                 "Sebastien Weber"
             ],
             "contributors": [],
             "description": "PyMoDAQ Orsay STEM and Camera plugin\r\nCan be used to control Ropers or Princeton Cameras\r\nCan be used to control STEM (Scanning Tunnel Electron Microscope) using the HOUDs 2 hardware module to drive coils within a STEM\n\nFrom Marcel Tence source code from LPS Laboratory at Orsay University, France ",
             "display-name": "OrsaySTEM and Cameras",
-            "homepage": "https://github.com/CEMES-CNRS/pymodaq_plugins_orsay",
+            "homepage": "https://github.com/PyMoDAQ/pymodaq_plugins_orsay",
             "id": "8587eca3ecdb07eab7dc6a2d2adb83bb2053f23a7d35458965566a0aa109f4b3",
             "instruments": {
                 "Actuator": [
                     "X and Y electron beam displacement in a STEM"
                 ],
                 "Viewer2D": [
                     "Cameras from Ropers and Princeton Instruments",
                     "STEM Imaging (even hyperspectral imaging)"
                 ]
             },
             "plugin-name": "pymodaq_plugins_orsay",
-            "repository": "https://github.com/CEMES-CNRS/pymodaq_plugins_orsay/archive/0.0.1.tar.gz",
+            "repository": "https://github.com/PyMoDAQ/pymodaq_plugins_orsay/archive/0.0.1.tar.gz",
             "version": "0.0.1"
         },
         {
             "authors": [
                 "Sebastien Weber"
             ],
             "contributors": [],
             "description": "Set of PyMoDAQ plugins for instruments from Newport (Conex, ESP100,...)",
             "display-name": "Newport Instruments",
-            "homepage": "https://github.com/CEMES-CNRS/pymodaq_plugins_newport",
+            "homepage": "https://github.com/PyMoDAQ/pymodaq_plugins_newport",
             "id": "11aaa70103138967053ae3db31af8977acf76f1f75b03bcc8e9624076d5e5dbd",
             "instruments": {
                 "Actuator": [
                     "Piezo actuators from the CONEX-AGAP series",
                     "ESP100 controllers"
                 ]
             },
             "plugin-name": "pymodaq_plugins_newport",
-            "repository": "https://github.com/CEMES-CNRS/pymodaq_plugins_newport/archive/0.0.2.tar.gz",
+            "repository": "https://github.com/PyMoDAQ/pymodaq_plugins_newport/archive/0.0.2.tar.gz",
             "version": "0.0.2"
         },
         {
             "authors": [
                 "Sebastien Weber"
             ],
             "contributors": [],
             "description": "Set of PyMoDAQ plugins for instruments from Thorlabs (Kinesis K10CR1 (stepper rotation actuator), Kinesis Flipper, Kinesis KSP100...)",
             "display-name": "Thorlabs Instruments",
-            "homepage": "https://github.com/CEMES-CNRS/pymodaq_plugins_thorlabs",
+            "homepage": "https://github.com/PyMoDAQ/pymodaq_plugins_thorlabs",
             "id": "562ef6ea46d9dc326db4448a8e314b815d363f1edcca4eeb6434d36ba8654d76",
             "instruments": {
                 "Actuator": [
                     "Kinesis serie (tested on K10CR1 and Flipper)"
                 ],
                 "Viewer0D": [
                     "Kinesis KPA101 Position Sensing Detector"
                 ]
             },
             "plugin-name": "pymodaq_plugins_thorlabs",
-            "repository": "https://github.com/CEMES-CNRS/pymodaq_plugins_thorlabs/archive/0.0.1.tar.gz",
+            "repository": "https://github.com/PyMoDAQ/pymodaq_plugins_thorlabs/archive/0.0.1.tar.gz",
             "version": "0.0.1"
         },
         {
             "authors": [
                 "Sebastien Weber"
             ],
             "contributors": [],
             "description": "Set of PyMoDAQ plugins for Actuators from Physik Instumente (All the ones compatible with the GCS2 commands as well as the old 32bits MMC controller...)",
             "display-name": "Physik Instrumente",
-            "homepage": "https://github.com/CEMES-CNRS/pymodaq_plugins_physik_instrumente",
+            "homepage": "https://github.com/PyMoDAQ/pymodaq_plugins_physik_instrumente",
             "id": "ae911130b4a6816f16707abd25db7bcd6d92801358d37a5541bdca0c92a6900f",
             "instruments": {
                 "Actuator": [
                     "All stages compatible with the GCS2 library",
                     "Old Stages using the 32 bits MMC dll"
                 ]
             },
             "plugin-name": "pymodaq_plugins_physik_instrumente",
-            "repository": "https://github.com/CEMES-CNRS/pymodaq_plugins_physik_instrumente/archive/0.0.1.tar.gz",
+            "repository": "https://github.com/PyMoDAQ/pymodaq_plugins_physik_instrumente/archive/0.0.1.tar.gz",
             "version": "0.0.1"
         },
         {
             "authors": [
                 "Sebastien Weber"
             ],
             "contributors": [],
             "description": "Set of PyMoDAQ plugins for Actuators from Piezoconcept (Tested on the Bio200 XY stage. Include a version of the controller firmware emulating functions from PhysikInstrumente)",
             "display-name": "PiezoConcept",
-            "homepage": "https://github.com/CEMES-CNRS/pymodaq_plugins_piezoconcept",
+            "homepage": "https://github.com/PyMoDAQ/pymodaq_plugins_piezoconcept",
             "id": "3ccdc960a25384f18a2a77d8b86e4100e2df6a2c8f020b479932dc3d7f2b3007",
             "instruments": {
                 "Actuator": [
                     "PiezoConcept stages (tested on BIO2.100) both using the usual serial commands and the ones derived from PI command set"
                 ]
             },
             "plugin-name": "pymodaq_plugins_piezoconcept",
-            "repository": "https://github.com/CEMES-CNRS/pymodaq_plugins_piezoconcept/archive/0.0.2.tar.gz",
+            "repository": "https://github.com/PyMoDAQ/pymodaq_plugins_piezoconcept/archive/0.0.2.tar.gz",
             "version": "0.0.2"
         },
         {
             "authors": [
                 "David Bresteau"
             ],
             "contributors": [],
             "description": "Set of PyMoDAQ plugins for Actuators from Smaract (MCS_controller, ...)",
             "display-name": "Smaract",
-            "homepage": "https://github.com/CEMES-CNRS/pymodaq_plugins_smaract",
+            "homepage": "https://github.com/PyMoDAQ/pymodaq_plugins_smaract",
             "id": "eb8c349bb16aa8c538b10617fb0af5bd8562c3f24e28a5c2a0f92e12fcdec18c",
             "instruments": {
                 "Actuator": [
                     "Actuators driven using the MCS controller and its library"
                 ]
             },
             "plugin-name": "pymodaq_plugins_smaract",
-            "repository": "https://github.com/CEMES-CNRS/pymodaq_plugins_smaract/archive/0.0.1.tar.gz",
+            "repository": "https://github.com/PyMoDAQ/pymodaq_plugins_smaract/archive/0.0.1.tar.gz",
             "version": "0.0.1"
         },
         {
             "authors": [
                 "Sebastien Weber"
             ],
             "contributors": [],
             "description": "Set of PyMoDAQ plugins for Andor Camera (CCD camera using SDK2, SCMOS cameras using SDK3...)",
             "display-name": "Andor",
-            "homepage": "https://github.com/CEMES-CNRS/pymodaq_plugins_andor",
+            "homepage": "https://github.com/PyMoDAQ/pymodaq_plugins_andor",
             "id": "9f2ce447a5a400e3c9457877d1cc9e138906e053344d2b4c3bb3aa20e7de033a",
             "instruments": {
                 "Viewer1D": [
                     "Shamrock series of spectrometer using the Andor CCD cameras"
                 ],
                 "Viewer2D": [
                     "Andor CCD camera using the SDK2"
                 ]
             },
             "plugin-name": "pymodaq_plugins_andor",
-            "repository": "https://github.com/CEMES-CNRS/pymodaq_plugins_andor/archive/0.0.1.tar.gz",
+            "repository": "https://github.com/PyMoDAQ/pymodaq_plugins_andor/archive/0.0.1.tar.gz",
             "version": "0.0.1"
         },
         {
             "authors": [
                 "Sebastien Weber"
             ],
             "contributors": [],
             "description": "Set of PyMoDAQ plugins for Picoquant instruments (TimeHarp260, ...)",
             "display-name": "Picoquant",
-            "homepage": "https://github.com/CEMES-CNRS/pymodaq_plugins_picoquant",
+            "homepage": "https://github.com/PyMoDAQ/pymodaq_plugins_picoquant",
             "id": "59c7d4bbede284fecf074bf1d32d7618c919107bd266710e492cf1db6f81308a",
             "instruments": {
                 "Viewer1D": [
                     "Timeharp TH260 for photon counting and time tagging"
                 ]
             },
             "plugin-name": "pymodaq_plugins_picoquant",
-            "repository": "https://github.com/CEMES-CNRS/pymodaq_plugins_picoquant/archive/0.0.1.tar.gz",
+            "repository": "https://github.com/PyMoDAQ/pymodaq_plugins_picoquant/archive/0.0.1.tar.gz",
             "version": "0.0.1"
         },
         {
             "authors": [
                 "Sebastien Weber"
             ],
             "contributors": [],
             "description": "Set of PyMoDAQ plugins for Horiba Instruments (Lapspec6TCP to communicate with labspec softaware using the AFM TCP/IP protocol)",
             "display-name": "Horiba",
-            "homepage": "https://github.com/CEMES-CNRS/pymodaq_plugins_horiba",
+            "homepage": "https://github.com/PyMoDAQ/pymodaq_plugins_horiba",
             "id": "01817fe5388ab383e025c48466a84e16fabb3672533736bb1cb29c072a7a7b03",
             "instruments": {
                 "Viewer1D": [
                     "Control of Labspec6 settings and acquisition using TCP/IP communication"
                 ]
             },
             "plugin-name": "pymodaq_plugins_horiba",
-            "repository": "https://github.com/CEMES-CNRS/pymodaq_plugins_horiba/archive/0.0.1.tar.gz",
+            "repository": "https://github.com/PyMoDAQ/pymodaq_plugins_horiba/archive/0.0.1.tar.gz",
             "version": "0.0.1"
         },
         {
             "authors": [
                 "Sebastien Weber"
             ],
             "contributors": [],
             "description": "Set of PyMoDAQ plugins for Fluorescence Lifetime Imaging Microscopy ",
             "display-name": "FLIM",
-            "homepage": "https://github.com/CEMES-CNRS/pymodaq_plugins_horiba",
+            "homepage": "https://github.com/PyMoDAQ/pymodaq_plugins_horiba",
             "id": "bf76f594875ef3b16cdc760499a3221e69eb0c5c0dc9b9105971f6d1325c257e",
             "instruments": {
                 "ViewerND": [
                     "FLIM using piezoconcept XY stage and picoquant timeharp TH260"
                 ]
             },
             "plugin-name": "pymodaq_plugins_flim",
-            "repository": "https://github.com/CEMES-CNRS/pymodaq_plugins_flim/archive/0.0.1.tar.gz",
+            "repository": "https://github.com/PyMoDAQ/pymodaq_plugins_flim/archive/0.0.1.tar.gz",
             "version": "0.0.1"
         },
         {
             "authors": [
                 "Sebastien Weber",
                 "Damien Lodie"
             ],
             "contributors": [
                 "David Bresteau",
                 "Nicolas Bruyant"
             ],
             "description": "Set of PyMoDAQ plugins for various physical measurements: multimeter, lockin, oscilloscope, indus cameras...",
             "display-name": "Physical Measurements Hardware",
-            "homepage": "https://github.com/CEMES-CNRS/pymodaq_plugins_horiba",
+            "homepage": "https://github.com/PyMoDAQ/pymodaq_plugins_horiba",
             "id": "4bd8c1f4ed210e5e3a84a314d5ea20f29f3485a41f56f7da58f1f786b3d28dd1",
             "instruments": {
                 "Viewer0D": [
                     "Pico-Amperemeter Keithley 648X Series, 6430 and 6514",
                     "Multimeter Keithley  2121",
                     "Lockin Amplifier Ametek 7270",
                     "LockIn Amplifier SR830"
@@ -284,67 +284,67 @@
                 "Viewer2D": [
                     "Webcams control using the opencv library",
                     "GeniCam compliant cameras",
                     "The Imaging Source TIS cameras"
                 ]
             },
             "plugin-name": "pymodaq_plugins_physical_measurements",
-            "repository": "https://github.com/CEMES-CNRS/pymodaq_plugins_physical_measurements/archive/0.0.3.tar.gz",
+            "repository": "https://github.com/PyMoDAQ/pymodaq_plugins_physical_measurements/archive/0.0.3.tar.gz",
             "version": "0.0.3"
         },
         {
             "authors": [
                 "Sebastien Weber"
             ],
             "contributors": [],
             "description": "Set of PyMoDAQ plugins for Holoeye Spatial Light Modulator (SLM)",
             "display-name": "Holoeye",
-            "homepage": "https://github.com/CEMES-CNRS/pymodaq_plugins_holoeye",
+            "homepage": "https://github.com/PyMoDAQ/pymodaq_plugins_holoeye",
             "id": "a3a63205dee749872a0ce3f5151a941d04b6780d57b57e771cf4bc5272141a1a",
             "instruments": {
                 "Actuator": [
                     "Let you apply various phase accross the SLM (tested with the LC2012)"
                 ]
             },
             "plugin-name": "pymodaq_plugins_holoeye",
-            "repository": "https://github.com/CEMES-CNRS/pymodaq_plugins_holoeye/archive/0.0.2.tar.gz",
+            "repository": "https://github.com/PyMoDAQ/pymodaq_plugins_holoeye/archive/0.0.2.tar.gz",
             "version": "0.0.2"
         },
         {
             "authors": [
                 "Sebastien Weber"
             ],
             "contributors": [],
             "description": "This repository contains a set of PyMoDAQ plugins for Amplitude Systems Lasers",
             "display-name": "Amplitude Lasers",
-            "homepage": "https://github.com/CEMES-CNRS/pymodaq_plugins_amplitude",
+            "homepage": "https://github.com/PyMoDAQ/pymodaq_plugins_amplitude",
             "id": "f8c262aedd985f3d3be90b28399caeda13a4855f99e68aa53ff640f7cab5e511",
             "instruments": {
                 "Viewer0D": [
                     "Let you control the laser settings and grab info on the laser status (tested on a Satsuma)"
                 ]
             },
             "plugin-name": "pymodaq_plugins_amplitude",
-            "repository": "https://github.com/CEMES-CNRS/pymodaq_plugins_amplitude/archive/0.0.1.tar.gz",
+            "repository": "https://github.com/PyMoDAQ/pymodaq_plugins_amplitude/archive/0.0.1.tar.gz",
             "version": "0.0.2"
         },
         {
             "authors": [
                 "Sebastien Weber"
             ],
             "contributors": [],
             "description": "Set of PyMoDAQ plugins for OceanInsight (OceanOptics) spectrometers",
             "display-name": "Ocean Insight (Optics)",
-            "homepage": "https://github.com/CEMES-CNRS/pymodaq_plugins_oceaninsight",
+            "homepage": "https://github.com/PyMoDAQ/pymodaq_plugins_oceaninsight",
             "id": "02c9776f0cfba56a6987300fb88040a22fbac1ba66573445d239ef685eb12007",
             "instruments": {
                 "Viewer1D": [
                     "Control of Spectrometer using the Omnidriver library (should be installed)"
                 ]
             },
             "plugin-name": "pymodaq_plugins_oceaninsight",
-            "repository": "https://github.com/CEMES-CNRS/pymodaq_plugins_oceaninsight/archive/0.0.1.tar.gz",
+            "repository": "https://github.com/PyMoDAQ/pymodaq_plugins_oceaninsight/archive/0.0.1.tar.gz",
             "version": "0.0.1"
         }
     ],
-    "version": "0.0.9"
+    "version": "0.0.17"
 }
```

### Comparing `pymodaq_plugin_manager-0.0.9/pymodaq_plugin_manager/src/plugin_list.schema` & `pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager/data/plugin_list.schema`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 27% similar despite different names*

```diff
@@ -1,129 +1,122 @@
-00000000: 7b0d 0a09 2274 7970 6522 3a20 226f 626a  {..."type": "obj
-00000010: 6563 7422 2c0d 0a09 2272 6571 7569 7265  ect",..."require
-00000020: 6422 3a20 5b0d 0a09 0922 6e61 6d65 222c  d": [...."name",
-00000030: 0d0a 0909 2276 6572 7369 6f6e 222c 0d0a  ...."version",..
-00000040: 0909 2270 796d 6f64 6171 2d70 6c75 6769  .."pymodaq-plugi
-00000050: 6e73 220d 0a09 5d2c 0d0a 0922 7072 6f70  ns"...],..."prop
-00000060: 6572 7469 6573 223a 207b 0d0a 0909 226e  erties": {...."n
-00000070: 616d 6522 3a20 7b20 2265 6e75 6d22 3a20  ame": { "enum": 
-00000080: 5b22 7079 6d6f 6461 712d 706c 7567 696e  ["pymodaq-plugin
-00000090: 4c69 7374 225d 207d 2c0d 0a09 0922 7665  List"] },...."ve
-000000a0: 7273 696f 6e22 3a20 7b0d 0a09 0909 2274  rsion": {....."t
-000000b0: 7970 6522 3a20 2273 7472 696e 6722 2c0d  ype": "string",.
-000000c0: 0a09 0909 2270 6174 7465 726e 223a 2022  ...."pattern": "
-000000d0: 5e5c 5c64 2b28 5c5c 2e5c 5c64 2b29 7b2c  ^\\d+(\\.\\d+){,
-000000e0: 337d 2422 0d0a 0909 7d2c 0d0a 0909 2270  3}$"....},...."p
-000000f0: 796d 6f64 6171 2d70 6c75 6769 6e73 223a  ymodaq-plugins":
-00000100: 207b 0d0a 0909 0922 7479 7065 223a 2022   {....."type": "
-00000110: 6172 7261 7922 2c0d 0a09 0909 2269 7465  array",....."ite
-00000120: 6d73 223a 207b 2022 2472 6566 223a 2022  ms": { "$ref": "
-00000130: 232f 6465 6669 6e69 7469 6f6e 732f 706c  #/definitions/pl
-00000140: 7567 696e 2220 7d0d 0a09 097d 0d0a 097d  ugin" }....}...}
-00000150: 2c0d 0a09 2264 6566 696e 6974 696f 6e73  ,..."definitions
-00000160: 223a 207b 0d0a 0909 2270 6c75 6769 6e22  ": {...."plugin"
-00000170: 3a20 7b0d 0a09 0909 2274 7970 6522 3a20  : {....."type": 
-00000180: 226f 626a 6563 7422 2c0d 0a09 0909 2272  "object",....."r
-00000190: 6571 7569 7265 6422 3a20 5b0d 0a09 0909  equired": [.....
-000001a0: 0922 706c 7567 696e 2d6e 616d 6522 2c0d  ."plugin-name",.
-000001b0: 0a09 0909 0922 6469 7370 6c61 792d 6e61  ....."display-na
-000001c0: 6d65 222c 0d0a 0909 0909 2276 6572 7369  me",......"versi
-000001d0: 6f6e 222c 0d0a 0909 0909 2269 6422 2c0d  on",......"id",.
-000001e0: 0a09 0909 0922 7265 706f 7369 746f 7279  ....."repository
-000001f0: 222c 0d0a 0909 0909 2264 6573 6372 6970  ",......"descrip
-00000200: 7469 6f6e 222c 0d0a 0909 0909 2269 6e73  tion",......"ins
-00000210: 7472 756d 656e 7473 222c 0d0a 0909 0909  truments",......
-00000220: 2261 7574 686f 7273 222c 0d0a 0909 0909  "authors",......
-00000230: 2263 6f6e 7472 6962 7574 6f72 7322 2c0d  "contributors",.
-00000240: 0a09 0909 0922 686f 6d65 7061 6765 220d  ....."homepage".
-00000250: 0a09 0909 5d2c 0d0a 0909 0922 7072 6f70  ....],....."prop
-00000260: 6572 7469 6573 223a 207b 0d0a 0909 0909  erties": {......
-00000270: 2270 6c75 6769 6e2d 6e61 6d65 223a 207b  "plugin-name": {
-00000280: 0d0a 0909 0909 0922 7479 7065 223a 2022  ......."type": "
-00000290: 7374 7269 6e67 222c 0d0a 0909 0909 0922  string",......."
-000002a0: 6d69 6e4c 656e 6774 6822 3a20 310d 0a09  minLength": 1...
-000002b0: 0909 097d 2c0d 0a09 0909 0922 6469 7370  ...},......"disp
-000002c0: 6c61 792d 6e61 6d65 223a 207b 0d0a 0909  lay-name": {....
-000002d0: 0909 0922 7479 7065 223a 2022 7374 7269  ..."type": "stri
-000002e0: 6e67 222c 0d0a 0909 0909 0922 6d69 6e4c  ng",......."minL
-000002f0: 656e 6774 6822 3a20 310d 0a09 0909 097d  ength": 1......}
-00000300: 2c0d 0a09 0909 0922 7665 7273 696f 6e22  ,......"version"
-00000310: 3a20 7b0d 0a09 0909 0909 2274 7970 6522  : {......."type"
-00000320: 3a20 2273 7472 696e 6722 2c0d 0a09 0909  : "string",.....
-00000330: 0909 2270 6174 7465 726e 223a 2022 5e5c  .."pattern": "^\
-00000340: 5c64 2b28 5c5c 2e5c 5c64 2b29 7b2c 337d  \d+(\\.\\d+){,3}
-00000350: 2422 0d0a 0909 0909 7d2c 0d0a 0909 0909  $"......},......
-00000360: 2269 6422 3a20 7b0d 0a09 0909 0909 2274  "id": {......."t
-00000370: 7970 6522 3a20 2273 7472 696e 6722 2c0d  ype": "string",.
-00000380: 0a09 0909 0909 2270 6174 7465 726e 223a  ......"pattern":
-00000390: 2022 5e28 3f69 295e 5b41 2d5a 302d 395d   "^(?i)^[A-Z0-9]
-000003a0: 7b36 347d 2422 0d0a 0909 0909 7d2c 0d0a  {64}$"......},..
-000003b0: 0909 0909 2272 6570 6f73 6974 6f72 7922  ...."repository"
-000003c0: 3a20 7b0d 0a09 0909 0909 2266 6f72 6d61  : {......."forma
-000003d0: 7422 3a20 2275 7269 220d 0a09 0909 097d  t": "uri"......}
-000003e0: 2c0d 0a09 0909 0922 6465 7363 7269 7074  ,......"descript
-000003f0: 696f 6e22 3a20 7b0d 0a09 0909 0909 2274  ion": {......."t
-00000400: 7970 6522 3a20 2273 7472 696e 6722 2c0d  ype": "string",.
-00000410: 0a09 0909 0909 226d 696e 4c65 6e67 7468  ......"minLength
-00000420: 223a 2031 0d0a 0909 0909 7d2c 0d0a 0909  ": 1......},....
-00000430: 0909 2269 6e73 7472 756d 656e 7473 223a  .."instruments":
-00000440: 207b 0d0a 0909 0909 0922 7479 7065 223a   {......."type":
-00000450: 2022 6f62 6a65 6374 222c 0d0a 0909 0909   "object",......
-00000460: 0922 7072 6f70 6572 7469 6573 223a 207b  ."properties": {
-00000470: 0d0a 0909 0909 0909 2241 6374 7561 746f  ........"Actuato
-00000480: 7222 3a20 7b0d 0a09 0909 0909 0909 2274  r": {........."t
-00000490: 7970 6522 3a20 2261 7272 6179 222c 0d0a  ype": "array",..
-000004a0: 0909 0909 0909 0922 6974 656d 7322 3a20  ......."items": 
-000004b0: 7b0d 0a09 0909 0909 0909 0922 7479 7065  {.........."type
-000004c0: 223a 2022 7374 7269 6e67 220d 0a09 0909  ": "string".....
-000004d0: 0909 0909 7d0d 0a09 0909 0909 097d 2c0d  ....}........},.
-000004e0: 0a09 0909 0909 0922 5669 6577 6572 3044  ......."Viewer0D
-000004f0: 223a 207b 0d0a 0909 0909 0909 0922 7479  ": {........."ty
-00000500: 7065 223a 2022 6172 7261 7922 2c0d 0a09  pe": "array",...
-00000510: 0909 0909 0909 2269 7465 6d73 223a 207b  ......"items": {
-00000520: 0d0a 0909 0909 0909 0909 2274 7970 6522  .........."type"
-00000530: 3a20 2273 7472 696e 6722 0d0a 0909 0909  : "string"......
-00000540: 0909 097d 0d0a 0909 0909 0909 7d2c 0d0a  ...}........},..
-00000550: 0909 0909 0909 2256 6965 7765 7231 4422  ......"Viewer1D"
-00000560: 3a20 7b0d 0a09 0909 0909 0909 2274 7970  : {........."typ
-00000570: 6522 3a20 2261 7272 6179 222c 0d0a 0909  e": "array",....
-00000580: 0909 0909 0922 6974 656d 7322 3a20 7b0d  ....."items": {.
-00000590: 0a09 0909 0909 0909 0922 7479 7065 223a  ........."type":
-000005a0: 2022 7374 7269 6e67 220d 0a09 0909 0909   "string".......
-000005b0: 0909 7d0d 0a09 0909 0909 097d 2c0d 0a09  ..}........},...
-000005c0: 0909 0909 0922 5669 6577 6572 3244 223a  ....."Viewer2D":
-000005d0: 207b 0d0a 0909 0909 0909 0922 7479 7065   {........."type
-000005e0: 223a 2022 6172 7261 7922 2c0d 0a09 0909  ": "array",.....
-000005f0: 0909 0909 2269 7465 6d73 223a 207b 0d0a  ...."items": {..
-00000600: 0909 0909 0909 0909 2274 7970 6522 3a20  ........"type": 
-00000610: 2273 7472 696e 6722 0d0a 0909 0909 0909  "string"........
-00000620: 097d 0d0a 0909 0909 0909 7d2c 0d0a 0909  .}........},....
-00000630: 0909 0909 2256 6965 7765 724e 4422 3a20  ...."ViewerND": 
-00000640: 7b0d 0a09 0909 0909 0909 2274 7970 6522  {........."type"
-00000650: 3a20 2261 7272 6179 222c 0d0a 0909 0909  : "array",......
-00000660: 0909 0922 6974 656d 7322 3a20 7b0d 0a09  ..."items": {...
-00000670: 0909 0909 0909 0922 7479 7065 223a 2022  ......."type": "
-00000680: 7374 7269 6e67 220d 0a09 0909 0909 0909  string".........
-00000690: 7d0d 0a09 0909 0909 097d 0d0a 0909 0909  }........}......
-000006a0: 097d 0d0a 0909 0909 7d2c 0d0a 0909 0909  .}......},......
-000006b0: 2261 7574 686f 7273 223a 207b 0d0a 0909  "authors": {....
-000006c0: 0909 0922 7479 7065 223a 2022 6172 7261  ..."type": "arra
-000006d0: 7922 2c0d 0a09 0909 0909 2269 7465 6d73  y",......."items
-000006e0: 223a 207b 0d0a 2020 2020 0909 0909 0922  ": {..    ....."
-000006f0: 7479 7065 223a 2022 7374 7269 6e67 220d  type": "string".
-00000700: 0a09 0909 0909 7d0d 0a09 0909 097d 2c0d  ......}......},.
-00000710: 0a09 0909 0922 636f 6e74 7269 6275 746f  ....."contributo
-00000720: 7273 223a 207b 0d0a 0909 0909 0922 7479  rs": {......."ty
-00000730: 7065 223a 2022 6172 7261 7922 2c0d 0a09  pe": "array",...
-00000740: 0909 0909 2269 7465 6d73 223a 207b 0d0a  ...."items": {..
-00000750: 2020 2020 0909 0909 0922 7479 7065 223a      ....."type":
-00000760: 2022 7374 7269 6e67 220d 0a09 0909 0909   "string".......
-00000770: 7d0d 0a09 0909 097d 2c0d 0a09 0909 0922  }......},......"
-00000780: 686f 6d65 7061 6765 223a 207b 0d0a 0909  homepage": {....
-00000790: 0909 0922 6f6e 654f 6622 3a20 5b0d 0a09  ..."oneOf": [...
-000007a0: 0909 0909 097b 2274 7970 6522 3a20 2273  .....{"type": "s
-000007b0: 7472 696e 6722 2c20 226d 6178 4c65 6e67  tring", "maxLeng
-000007c0: 7468 223a 2030 7d2c 0d0a 0909 0909 0909  th": 0},........
-000007d0: 7b22 666f 726d 6174 223a 2022 7572 6922  {"format": "uri"
-000007e0: 7d0d 0a09 0909 0909 5d0d 0a09 0909 097d  }.......]......}
-000007f0: 0d0a 0909 097d 0d0a 0909 7d0d 0a09 7d0d  .....}....}...}.
-00000800: 0a7d                                     .}
+00000000: 7b0a 0922 7479 7065 223a 2022 6f62 6a65  {.."type": "obje
+00000010: 6374 222c 0a09 2272 6571 7569 7265 6422  ct",.."required"
+00000020: 3a20 5b0a 0909 226e 616d 6522 2c0a 0909  : [..."name",...
+00000030: 2276 6572 7369 6f6e 222c 0a09 0922 7079  "version",..."py
+00000040: 6d6f 6461 712d 706c 7567 696e 7322 0a09  modaq-plugins"..
+00000050: 5d2c 0a09 2270 726f 7065 7274 6965 7322  ],.."properties"
+00000060: 3a20 7b0a 0909 226e 616d 6522 3a20 7b20  : {..."name": { 
+00000070: 2265 6e75 6d22 3a20 5b22 7079 6d6f 6461  "enum": ["pymoda
+00000080: 712d 706c 7567 696e 4c69 7374 225d 207d  q-pluginList"] }
+00000090: 2c0a 0909 2276 6572 7369 6f6e 223a 207b  ,..."version": {
+000000a0: 0a09 0909 2274 7970 6522 3a20 2273 7472  ...."type": "str
+000000b0: 696e 6722 2c0a 0909 0922 7061 7474 6572  ing",...."patter
+000000c0: 6e22 3a20 225e 5c5c 642b 285c 5c2e 5c5c  n": "^\\d+(\\.\\
+000000d0: 642b 297b 2c33 7d24 220a 0909 7d2c 0a09  d+){,3}$"...},..
+000000e0: 0922 7079 6d6f 6461 712d 706c 7567 696e  ."pymodaq-plugin
+000000f0: 7322 3a20 7b0a 0909 0922 7479 7065 223a  s": {...."type":
+00000100: 2022 6172 7261 7922 2c0a 0909 0922 6974   "array",...."it
+00000110: 656d 7322 3a20 7b20 2224 7265 6622 3a20  ems": { "$ref": 
+00000120: 2223 2f64 6566 696e 6974 696f 6e73 2f70  "#/definitions/p
+00000130: 6c75 6769 6e22 207d 0a09 097d 0a09 7d2c  lugin" }...}..},
+00000140: 0a09 2264 6566 696e 6974 696f 6e73 223a  .."definitions":
+00000150: 207b 0a09 0922 706c 7567 696e 223a 207b   {..."plugin": {
+00000160: 0a09 0909 2274 7970 6522 3a20 226f 626a  ...."type": "obj
+00000170: 6563 7422 2c0a 0909 0922 7265 7175 6972  ect",...."requir
+00000180: 6564 223a 205b 0a09 0909 0922 706c 7567  ed": [....."plug
+00000190: 696e 2d6e 616d 6522 2c0a 0909 0909 2264  in-name",....."d
+000001a0: 6973 706c 6179 2d6e 616d 6522 2c0a 0909  isplay-name",...
+000001b0: 0909 2276 6572 7369 6f6e 222c 0a09 0909  .."version",....
+000001c0: 0922 6964 222c 0a09 0909 0922 7265 706f  ."id",....."repo
+000001d0: 7369 746f 7279 222c 0a09 0909 0922 6465  sitory",....."de
+000001e0: 7363 7269 7074 696f 6e22 2c0a 0909 0909  scription",.....
+000001f0: 2269 6e73 7472 756d 656e 7473 222c 0a09  "instruments",..
+00000200: 0909 0922 6175 7468 6f72 7322 2c0a 0909  ..."authors",...
+00000210: 0909 2263 6f6e 7472 6962 7574 6f72 7322  .."contributors"
+00000220: 2c0a 0909 0909 2268 6f6d 6570 6167 6522  ,....."homepage"
+00000230: 0a09 0909 5d2c 0a09 0909 2270 726f 7065  ....],...."prope
+00000240: 7274 6965 7322 3a20 7b0a 0909 0909 2270  rties": {....."p
+00000250: 6c75 6769 6e2d 6e61 6d65 223a 207b 0a09  lugin-name": {..
+00000260: 0909 0909 2274 7970 6522 3a20 2273 7472  ...."type": "str
+00000270: 696e 6722 2c0a 0909 0909 0922 6d69 6e4c  ing",......"minL
+00000280: 656e 6774 6822 3a20 310a 0909 0909 7d2c  ength": 1.....},
+00000290: 0a09 0909 0922 6469 7370 6c61 792d 6e61  ....."display-na
+000002a0: 6d65 223a 207b 0a09 0909 0909 2274 7970  me": {......"typ
+000002b0: 6522 3a20 2273 7472 696e 6722 2c0a 0909  e": "string",...
+000002c0: 0909 0922 6d69 6e4c 656e 6774 6822 3a20  ..."minLength": 
+000002d0: 310a 0909 0909 7d2c 0a09 0909 0922 7665  1.....},....."ve
+000002e0: 7273 696f 6e22 3a20 7b0a 0909 0909 0922  rsion": {......"
+000002f0: 7479 7065 223a 2022 7374 7269 6e67 222c  type": "string",
+00000300: 0a09 0909 0909 2270 6174 7465 726e 223a  ......"pattern":
+00000310: 2022 5e5c 5c64 2b28 5c5c 2e5c 5c64 2b29   "^\\d+(\\.\\d+)
+00000320: 7b2c 337d 2422 0a09 0909 097d 2c0a 0909  {,3}$".....},...
+00000330: 0909 2269 6422 3a20 7b0a 0909 0909 0922  .."id": {......"
+00000340: 7479 7065 223a 2022 7374 7269 6e67 222c  type": "string",
+00000350: 0a09 0909 0909 2270 6174 7465 726e 223a  ......"pattern":
+00000360: 2022 5e28 3f69 295e 5b41 2d5a 302d 395d   "^(?i)^[A-Z0-9]
+00000370: 7b36 347d 2422 0a09 0909 097d 2c0a 0909  {64}$".....},...
+00000380: 0909 2272 6570 6f73 6974 6f72 7922 3a20  .."repository": 
+00000390: 7b0a 0909 0909 0922 666f 726d 6174 223a  {......"format":
+000003a0: 2022 7572 6922 0a09 0909 097d 2c0a 0909   "uri".....},...
+000003b0: 0909 2264 6573 6372 6970 7469 6f6e 223a  .."description":
+000003c0: 207b 0a09 0909 0909 2274 7970 6522 3a20   {......"type": 
+000003d0: 2273 7472 696e 6722 2c0a 0909 0909 0922  "string",......"
+000003e0: 6d69 6e4c 656e 6774 6822 3a20 310a 0909  minLength": 1...
+000003f0: 0909 7d2c 0a09 0909 0922 696e 7374 7275  ..},....."instru
+00000400: 6d65 6e74 7322 3a20 7b0a 0909 0909 0922  ments": {......"
+00000410: 7479 7065 223a 2022 6f62 6a65 6374 222c  type": "object",
+00000420: 0a09 0909 0909 2270 726f 7065 7274 6965  ......"propertie
+00000430: 7322 3a20 7b0a 0909 0909 0909 2241 6374  s": {......."Act
+00000440: 7561 746f 7222 3a20 7b0a 0909 0909 0909  uator": {.......
+00000450: 0922 7479 7065 223a 2022 6172 7261 7922  ."type": "array"
+00000460: 2c0a 0909 0909 0909 0922 6974 656d 7322  ,........"items"
+00000470: 3a20 7b0a 0909 0909 0909 0909 2274 7970  : {........."typ
+00000480: 6522 3a20 2273 7472 696e 6722 0a09 0909  e": "string"....
+00000490: 0909 0909 7d0a 0909 0909 0909 7d2c 0a09  ....}.......},..
+000004a0: 0909 0909 0922 5669 6577 6572 3044 223a  ....."Viewer0D":
+000004b0: 207b 0a09 0909 0909 0909 2274 7970 6522   {........"type"
+000004c0: 3a20 2261 7272 6179 222c 0a09 0909 0909  : "array",......
+000004d0: 0909 2269 7465 6d73 223a 207b 0a09 0909  .."items": {....
+000004e0: 0909 0909 0922 7479 7065 223a 2022 7374  ....."type": "st
+000004f0: 7269 6e67 220a 0909 0909 0909 097d 0a09  ring"........}..
+00000500: 0909 0909 097d 2c0a 0909 0909 0909 2256  .....},......."V
+00000510: 6965 7765 7231 4422 3a20 7b0a 0909 0909  iewer1D": {.....
+00000520: 0909 0922 7479 7065 223a 2022 6172 7261  ..."type": "arra
+00000530: 7922 2c0a 0909 0909 0909 0922 6974 656d  y",........"item
+00000540: 7322 3a20 7b0a 0909 0909 0909 0909 2274  s": {........."t
+00000550: 7970 6522 3a20 2273 7472 696e 6722 0a09  ype": "string"..
+00000560: 0909 0909 0909 7d0a 0909 0909 0909 7d2c  ......}.......},
+00000570: 0a09 0909 0909 0922 5669 6577 6572 3244  ......."Viewer2D
+00000580: 223a 207b 0a09 0909 0909 0909 2274 7970  ": {........"typ
+00000590: 6522 3a20 2261 7272 6179 222c 0a09 0909  e": "array",....
+000005a0: 0909 0909 2269 7465 6d73 223a 207b 0a09  ...."items": {..
+000005b0: 0909 0909 0909 0922 7479 7065 223a 2022  ......."type": "
+000005c0: 7374 7269 6e67 220a 0909 0909 0909 097d  string"........}
+000005d0: 0a09 0909 0909 097d 2c0a 0909 0909 0909  .......},.......
+000005e0: 2256 6965 7765 724e 4422 3a20 7b0a 0909  "ViewerND": {...
+000005f0: 0909 0909 0922 7479 7065 223a 2022 6172  ....."type": "ar
+00000600: 7261 7922 2c0a 0909 0909 0909 0922 6974  ray",........"it
+00000610: 656d 7322 3a20 7b0a 0909 0909 0909 0909  ems": {.........
+00000620: 2274 7970 6522 3a20 2273 7472 696e 6722  "type": "string"
+00000630: 0a09 0909 0909 0909 7d0a 0909 0909 0909  ........}.......
+00000640: 7d0a 0909 0909 097d 0a09 0909 097d 2c0a  }......}.....},.
+00000650: 0909 0909 2261 7574 686f 7273 223a 207b  ...."authors": {
+00000660: 0a09 0909 0909 2274 7970 6522 3a20 2261  ......"type": "a
+00000670: 7272 6179 222c 0a09 0909 0909 2269 7465  rray",......"ite
+00000680: 6d73 223a 207b 0a20 2020 2009 0909 0909  ms": {.    .....
+00000690: 2274 7970 6522 3a20 2273 7472 696e 6722  "type": "string"
+000006a0: 0a09 0909 0909 7d0a 0909 0909 7d2c 0a09  ......}.....},..
+000006b0: 0909 0922 636f 6e74 7269 6275 746f 7273  ..."contributors
+000006c0: 223a 207b 0a09 0909 0909 2274 7970 6522  ": {......"type"
+000006d0: 3a20 2261 7272 6179 222c 0a09 0909 0909  : "array",......
+000006e0: 2269 7465 6d73 223a 207b 0a20 2020 2009  "items": {.    .
+000006f0: 0909 0909 2274 7970 6522 3a20 2273 7472  ...."type": "str
+00000700: 696e 6722 0a09 0909 0909 7d0a 0909 0909  ing"......}.....
+00000710: 7d2c 0a09 0909 0922 686f 6d65 7061 6765  },....."homepage
+00000720: 223a 207b 0a09 0909 0909 226f 6e65 4f66  ": {......"oneOf
+00000730: 223a 205b 0a09 0909 0909 097b 2274 7970  ": [.......{"typ
+00000740: 6522 3a20 2273 7472 696e 6722 2c20 226d  e": "string", "m
+00000750: 6178 4c65 6e67 7468 223a 2030 7d2c 0a09  axLength": 0},..
+00000760: 0909 0909 097b 2266 6f72 6d61 7422 3a20  .....{"format": 
+00000770: 2275 7269 227d 0a09 0909 0909 5d0a 0909  "uri"}......]...
+00000780: 0909 7d0a 0909 097d 0a09 097d 0a09 7d0a  ..}....}...}..}.
+00000790: 7d                                       }
```

