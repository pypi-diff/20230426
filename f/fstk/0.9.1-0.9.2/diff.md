# Comparing `tmp/fstk-0.9.1-py3-none-any.whl.zip` & `tmp/fstk-0.9.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 652947 bytes, number of entries: 19
--rw-r-----  2.0 unx    28395 b- defN 23-Feb-28 23:25 fstk/Dialogs.py
--rw-r-----  2.0 unx    44769 b- defN 23-Feb-28 23:22 fstk/Fstk.py
+Zip file size: 653093 bytes, number of entries: 19
+-rw-r-----  2.0 unx    28588 b- defN 23-Apr-25 13:41 fstk/Dialogs.py
+-rw-r-----  2.0 unx    44667 b- defN 23-Apr-25 13:48 fstk/Fstk.py
 -rw-r-----  2.0 unx     2331 b- defN 22-Apr-20 21:28 fstk/Globals.py
 -rw-r-----  2.0 unx      196 b- defN 21-Mar-23 22:23 fstk/Palette.py
 -rw-r-----  2.0 unx     4561 b- defN 23-Feb-28 22:44 fstk/Redmine.py
--rw-r-----  2.0 unx     5879 b- defN 21-Mar-23 22:16 fstk/SaveFiles.py
+-rw-r-----  2.0 unx     5834 b- defN 23-Apr-21 12:28 fstk/SaveFiles.py
 -rw-r-----  2.0 unx     4279 b- defN 22-Apr-20 21:28 fstk/SavefilesMigrations.py
--rw-r-----  2.0 unx     1547 b- defN 21-Apr-17 22:06 fstk/Updater.py
+-rw-r-----  2.0 unx     1579 b- defN 23-Apr-21 10:26 fstk/Updater.py
 -rw-r-----  2.0 unx     1936 b- defN 22-Apr-20 21:50 fstk/Utils.py
--rw-r-----  2.0 unx       21 b- defN 23-Feb-28 23:25 fstk/__init__.py
+-rw-r-----  2.0 unx       21 b- defN 23-Mar-01 16:23 fstk/__init__.py
 -rw-r-----  2.0 unx     4293 b- defN 21-Apr-26 07:23 fstk/__main__.py
 -rw-rw----  2.0 unx  1380376 b- defN 21-Apr-17 21:06 fstk/assets/Font Awesome 5 Pro-Light-300.otf
 -rw-r-----  2.0 unx        0 b- defN 21-Mar-19 10:23 fstk/assets/__init__.py
 -rw-rw----  2.0 unx      158 b- defN 21-Mar-20 15:19 fstk/assets/fast-switch-time-keeper.desktop
 -rw-r--r--  2.0 unx    14412 b- defN 20-Oct-15 07:29 fstk/assets/icon.png
--rw-r-----  2.0 unx      910 b- defN 23-Feb-28 23:25 fstk-0.9.1.dist-info/METADATA
--rw-r-----  2.0 unx       92 b- defN 23-Feb-28 23:25 fstk-0.9.1.dist-info/WHEEL
--rw-r-----  2.0 unx        5 b- defN 23-Feb-28 23:25 fstk-0.9.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1444 b- defN 23-Feb-28 23:25 fstk-0.9.1.dist-info/RECORD
-19 files, 1495604 bytes uncompressed, 650637 bytes compressed:  56.5%
+-rw-r-----  2.0 unx      910 b- defN 23-Apr-25 13:48 fstk-0.9.2.dist-info/METADATA
+-rw-r-----  2.0 unx       92 b- defN 23-Apr-25 13:48 fstk-0.9.2.dist-info/WHEEL
+-rw-r-----  2.0 unx        5 b- defN 23-Apr-25 13:48 fstk-0.9.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1444 b- defN 23-Apr-25 13:48 fstk-0.9.2.dist-info/RECORD
+19 files, 1495682 bytes uncompressed, 650783 bytes compressed:  56.5%
```

## zipnote {}

```diff
@@ -39,20 +39,20 @@
 
 Filename: fstk/assets/fast-switch-time-keeper.desktop
 Comment: 
 
 Filename: fstk/assets/icon.png
 Comment: 
 
-Filename: fstk-0.9.1.dist-info/METADATA
+Filename: fstk-0.9.2.dist-info/METADATA
 Comment: 
 
-Filename: fstk-0.9.1.dist-info/WHEEL
+Filename: fstk-0.9.2.dist-info/WHEEL
 Comment: 
 
-Filename: fstk-0.9.1.dist-info/top_level.txt
+Filename: fstk-0.9.2.dist-info/top_level.txt
 Comment: 
 
-Filename: fstk-0.9.1.dist-info/RECORD
+Filename: fstk-0.9.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fstk/Dialogs.py

```diff
@@ -10,15 +10,15 @@
 from .Globals import default_window_style
 
 
 class AskForTextDialog(QDialog):
 
     def __init__(self, window_title, length, initial_text, validator=None):
         QDialog.__init__(self)
-        self.__validator = validator
+        self._validator = validator
 
         self.setWindowTitle(window_title)
         self.resize(length, 100)
         self.setStyleSheet(default_window_style + '''
             QDialog { background-color: #232931 }
             QLineEdit { background-color: #444f5d; }
             QPushButton { padding-top: 1; padding-bottom: 1; padding-left: 4; padding-right: 4; }
@@ -41,16 +41,16 @@
         self.box.addWidget(self.ok_button, 2, 0, alignment=Qt.AlignCenter)
 
         self.ok_button.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
 
         self.setLayout(self.box)
 
     def ok_handler(self):
-        if self.__validator is not None:
-            success, error_msg = self.__validator(self.line.text())
+        if self._validator is not None:
+            success, error_msg = self._validator(self.line.text())
             if not success:
                 self.line.setStyleSheet('background-color: #fa7161')
                 self.error_label.setText(error_msg)
                 return
 
         self.accept()
 
@@ -287,14 +287,19 @@
         ''')
 
         self.setWindowIcon(QtGui.QIcon(Utils.get_local_file_path('icon.png')))
 
         changelog_text = '''
             Current FSTK version: <b>{}</b><br>
             <br>
+            <b>Release 0.9.2</b>
+            <ul>
+                <li>Fix update code to report errors during self-update</li>
+                <li>Internal improvements</li>
+            </ul><br>
             <b>Release 0.9.1</b>
             <ul>
                 <li>Fix a small bug where a border was shown around ticket number placeholder of tasks without a ticket number set</li>
             </ul><br>
             <b>Release 0.9.0</b>
             <ul>
                 <li>A yellow border is now shown around ticket numbers which are duplicated between tasks</li>
```

## fstk/Fstk.py

```diff
@@ -1,15 +1,15 @@
 import json
 import logging
 import os
 import sys
 
 import requests
 import webbrowser
-from PySide2 import QtGui
+from PySide2 import QtGui, QtCore
 from PySide2.QtCore import Qt, Slot, QPoint, QEvent, QTimer, Signal, QThread
 from PySide2.QtGui import QFont, QDrag, QPixmap, QPainter, QCursor
 from PySide2.QtWidgets import (QAction, QApplication, QHBoxLayout, QLabel, QMainWindow, QPushButton, QWidget,
                                QListWidget, QListWidgetItem, QGridLayout,
                                QSizePolicy, QAbstractItemView, QListView, QMenu)
 
 from .Dialogs import (AskForTextDialog, ConfirmDialog, NewTaskDialog, HelpDialog, InformationDialog, ChangelogDialog,
@@ -57,35 +57,36 @@
         if self.timer.isActive():
             self.timer.stop()
             self.doubleClicked.emit()
 
         else:
             self.timer.start(250)
 
-class RowElement(QWidget):
-    __seconds = 0
-    __color_group = 'No color'
-
-    __saved = False
-    __main_widget = None
-    __list = None
-    __list_item = None
+class TaskElement(QWidget):
+    _seconds = 0
+    _color_group = 'No color'
+
+    _saved = False
+    _main_widget = None
+    _list = None
+    _list_item = None
 
-    __notes = ''
+    _notes = ''
 
+    type = 'task'
 
     def __init__(self, options, main_widget, list_, list_item):
         super().__init__()
-        self.__main_widget = main_widget
-        self.__list = list_
-        self.__list_item = list_item
+        self._main_widget = main_widget
+        self._list = list_
+        self._list_item = list_item
 
         # inizializzato in un metodo sotto
-        self.__notes_dialog = None
-        self.__notes = options.get('notes', '')
+        self._notes_dialog = None
+        self._notes = options.get('notes', '')
 
         fa5 = QFont('Font Awesome 5 Pro')
 
         self.box = QGridLayout()
 
         self.name = QLabelClickable(options['name'])
         self.name.setWordWrap(True)
@@ -146,15 +147,15 @@
         self.add_time.setMinimumHeight(self.get_button_size()[1])
 
         self.notes = QPushButtonHoverable('sticky-note')
         self.notes.setFont(fa5)
         self.notes.mouse_entered.connect(self.show_notes)
         self.notes.mouse_leaved.connect(self.hide_notes)
         self.notes.clicked.connect(self.edit_notes)
-        self.notes.setProperty('full', self.__notes != '')
+        self.notes.setProperty('full', self._notes != '')
         self.notes.setStyleSheet('''
             QPushButton { padding-top: 1; padding-bottom: 1; padding-left: 4; padding-right: 4; }
             QPushButton[full=true] { border: 1px solid #fae661;  }
         ''')
         self.notes.setMaximumWidth(self.get_button_size()[0])
         self.notes.setMinimumWidth(self.get_button_size()[0])
         self.notes.setMinimumHeight(self.get_button_size()[1])
@@ -199,41 +200,41 @@
 
         # aggiorna il label in modo da mostrare il tempo memorizzato
         self.set_time(options['elapsed_time'])
 
         # imposta flag per i visualizzare correttamente i gruppi colore
         self.setAutoFillBackground(True)
         self.setAttribute(Qt.WA_StyledBackground, True)
-        self.setStyleSheet('RowElement { border: solid ' + Palette.group_colors[options['color_group']] + '; border-width: 0px 0px 0px 5px; }')
-        self.__color_group = options['color_group']
+        self.setStyleSheet('TaskElement { border: solid ' + Palette.group_colors[options['color_group']] + '; border-width: 0px 0px 0px 5px; }')
+        self._color_group = options['color_group']
 
     def contextMenuEvent(self, event):
         contex_menu = QMenu(self)
 
         ris = {}
 
         for name, color in Palette.group_colors.items():
             ris[contex_menu.addAction(name)] = (name, color)
 
         action = contex_menu.exec_(self.mapToGlobal(event.pos()))
 
         if action is not None:
-            self.setStyleSheet('RowElement { border: solid ' + ris[action][1] + '; border-width: 0px 0px 0px 5px; }')
-            self.__color_group = ris[action][0]
+            self.setStyleSheet('TaskElement { border: solid ' + ris[action][1] + '; border-width: 0px 0px 0px 5px; }')
+            self._color_group = ris[action][0]
             Globals.config['stats']['task_color_set'] += 1
 
     def mousePressEvent(self, event):
         # ignora i click con il tasto destro per selezionare come attivo un widget
         if event.button() != Qt.RightButton:
             super().mousePressEvent(event)
 
             # se l'utente ha abilitato il reminder per switchare task lo resetto, poichè lui ha appena switchato tutto
             if Globals.config['options']['switch_reminder']['enabled']:
-                self.__main_widget.__main_window.task_switch_timer.stop()
-                self.__main_widget.__main_window.task_switch_timer.start(Globals.config['options']['switch_reminder']['interval'] * 60 * 1000)  # converto da minuti a millisecondi
+                self._main_widget._main_window.task_switch_timer.stop()
+                self._main_widget._main_window.task_switch_timer.start(Globals.config['options']['switch_reminder']['interval'] * 60 * 1000)  # converto da minuti a millisecondi
 
         else:
             event.accept()
 
     # Azioni eseguite dall'interfaccia grafica
 
     @Slot()
@@ -307,52 +308,52 @@
 
         self.ticket_number.setText('#' + n)
 
         if n == '':
             self.ticket_title.setText('')
         else:
             # aggiorno lo stato dei marker che indicano i task con numero ticket duplicato
-            self.__main_widget.update_duplicated_tickets_marker()
+            self._main_widget.update_duplicated_tickets_marker()
 
             if Globals.config['options']['redmine']['enabled']:
-                self.__main_widget.update_ticket_title(self.ticket_title, n)
+                self._main_widget.update_ticket_title(self.ticket_title, n)
 
         Globals.config['stats']['task_ticket_n_edited'] += 1
 
     @Slot()
     def edit_name(self):
         dialog = AskForTextDialog(window_title='Set task name',
                                   initial_text=self.name.text(), length=600,
                                   validator=Utils.not_empty_validator)
         if not dialog.exec():  # se l'utente non ha cliccato su ok non procediamo
             return
 
         t = dialog.line.text().strip()
 
         self.name.setText(t)
-        self.__list_item.setSizeHint(self.minimumSizeHint())
+        self._list_item.setSizeHint(self.minimumSizeHint())
         Globals.config['stats']['task_name_edited'] += 1
 
     @Slot()
     def del_task(self):
-        if self.__notes == '':
+        if self._notes == '':
             text = 'The task will be deleted, are you sure?'
         else:
             text = 'The task will be deleted, are you sure?\n--- THE TASK CONTAINS NOTES ---'
 
         dialog = ConfirmDialog(window_title='Confirm task deletion', text=text)
 
         if not dialog.exec():  # se l'utente non ha cliccato su ok non procediamo
             return
 
-        self.__list.takeItem(self.__list.row(self.__list_item))
+        self._list.takeItem(self._list.row(self._list_item))
 
-        self.__main_widget.update_total_time()
+        self._main_widget.update_total_time()
         # aggiorno lo stato dei marker che indicano i task con numero ticket duplicato
-        self.__main_widget.update_duplicated_tickets_marker()
+        self._main_widget.update_duplicated_tickets_marker()
 
         Globals.config['stats']['task_deleted'] += 1
 
     @Slot()
     def clear_time(self):
         dialog = ConfirmDialog(window_title='Confirm time deletion',
                                # text='The time has not been reported yet, are you sure?')
@@ -362,102 +363,103 @@
 
         self.set_time(0)
 
         Globals.config['stats']['task_time_cleared'] += 1
 
     @Slot()
     def show_notes(self, pos):
-        if self.__notes_dialog is None and self.__notes != '':
-            self.__notes_dialog = ShowNotesDialog(pos, self.__notes)
-            self.__notes_dialog.show()
+        if self._notes_dialog is None and self._notes != '':
+            self._notes_dialog = ShowNotesDialog(pos, self._notes)
+            self._notes_dialog.show()
 
             Globals.config['stats']['task_notes_viewed'] += 1
 
     @Slot()
     def hide_notes(self):
-        if self.__notes_dialog is not None:
-            self.__notes_dialog.accept()
-            self.__notes_dialog = None
+        if self._notes_dialog is not None:
+            self._notes_dialog.accept()
+            self._notes_dialog = None
 
     @Slot()
     def edit_notes(self):
-        dialog = EditNotesDialog(self.__notes)
+        dialog = EditNotesDialog(self._notes)
 
         if not dialog.exec():  # se l'utente non ha cliccato su ok non procediamo
             return
 
-        self.__notes = dialog.text.toPlainText().strip()
+        self._notes = dialog.text.toPlainText().strip()
         # marco come piene o vuote le note per mostrare il giusto stato nella UI
-        Utils.set_prop_and_refresh(self.notes, 'full', self.__notes != '')
+        Utils.set_prop_and_refresh(self.notes, 'full', self._notes != '')
 
         Globals.config['stats']['task_notes_edited'] += 1
 
     # Metodi chiamati esternamente
 
     def update_time(self, seconds):
         self.set_time(self.get_time()+seconds)
 
     def get_time(self):
-        return self.__seconds
+        return self._seconds
 
     def set_time(self, seconds):
-        old_seconds = self.__seconds
-        self.__seconds = seconds
+        old_seconds = self._seconds
+        self._seconds = seconds
 
-        if self.__seconds < 0:
-            self.__seconds = 0
+        if self._seconds < 0:
+            self._seconds = 0
 
-        self.spent_time.setText(Utils.format_time(self.__seconds))
+        self.spent_time.setText(Utils.format_time(self._seconds))
 
         elements = [self.spent_time, self.add_time, self.sub_time, self.del_record, self.clear_record_time, self.ticket_number, self.name, self.ticket_title, self.notes]
         # valuta se è possibile che sia avvenuta un condizione che provocherebbe il cambio di colore degli elementi
         # se non può essere avvenuta skippa il codice di set dello style
-        if (old_seconds == 0 and self.__seconds != 0) or (old_seconds != 0 and self.__seconds == 0) or (old_seconds == self.__seconds == 0):
+        if (old_seconds == 0 and self._seconds != 0) or (old_seconds != 0 and self._seconds == 0) or (old_seconds == self._seconds == 0):
             for x in elements:
-                Utils.set_prop_and_refresh(x, 'counting', self.__seconds != 0)
+                Utils.set_prop_and_refresh(x, 'counting', self._seconds != 0)
 
-        self.__main_widget.update_total_time()
+        self._main_widget.update_total_time()
 
     def to_dict(self):
         return {
             'name': self.name.text(),
             'ticket': self.ticket_number.text().strip('#'),
-            'elapsed_time': self.__seconds,
-            'color_group': self.__color_group,
+            'elapsed_time': self._seconds,
+            'color_group': self._color_group,
             'ticket_title': None if self.ticket_title.property('invalid') else self.ticket_title.text(),
-            'notes': self.__notes
+            'notes': self._notes
         }
 
     # funzione per la formattazione degli elementi grafici
     def get_button_size(self):
         metric = self.name.fontMetrics().boundingRect('+5')
         width = metric.width() + 14
         height = metric.height() + 4
 
         return width, height
 
 
 class ListWidget(QListWidget):
+    _pixmap = None
 
     def __init__(self):
         super().__init__()
 
     def startDrag(self, supported_actions):
         Globals.config['stats']['task_reordered'] += 1
 
         drag = QDrag(self)
         drag.setMimeData(self.model().mimeData(self.selectedIndexes()))
-        self.__pixmap = QPixmap(self.viewport().visibleRegion().boundingRect().size())
-        self.__pixmap.fill(Qt.transparent)
-        painter = QPainter(self.__pixmap)
+        self._pixmap = QPixmap(self.viewport().visibleRegion().boundingRect().size())
+        self._pixmap.fill(Qt.transparent)
+        painter = QPainter(self._pixmap)
 
         for i in self.selectedIndexes():
             painter.drawPixmap(self.visualRect(i), self.viewport().grab(self.visualRect(i)))
 
-        drag.setPixmap(self.__pixmap)
+        drag.setPixmap(self._pixmap)
         drag.setHotSpot(self.viewport().mapFromGlobal(QCursor.pos()))
         drag.exec_(supported_actions, Qt.MoveAction)
 
     def keyPressEvent(self, event):
         if event.key() == Qt.Key_Delete:
             for s in self.selectedItems():
                 self.itemWidget(s).del_task()
@@ -481,15 +483,15 @@
 
     def run(self):
            result = Redmine.are_creds_valid()
            self.finished.emit(result)
 
 class MainWidget(QWidget):
 
-    __main_window = None
+    _main_window = None
 
     def __init__(self):
         QWidget.__init__(self)
 
         # Create the list
         self.task_list = ListWidget()
         self.task_list.setSelectionMode(QAbstractItemView.SingleSelection)
@@ -564,15 +566,15 @@
 
 
     def insert_task_in_list(self, name, ticket_number='', elapsed_time=0, color_group='No color', ticket_title='', notes=''):
         # Add to list a new item (item is simply an entry in your list)
         item = QListWidgetItem()
 
         # Instanciate a custom widget
-        row = RowElement({
+        row = TaskElement({
             'name': name,
             'ticket_number': ticket_number,
             'elapsed_time': elapsed_time,
             'color_group': color_group,
             'ticket_title': ticket_title,
             'notes': notes
         }, self, self.task_list, item)
@@ -588,24 +590,23 @@
         if self.running:
             for s in self.task_list.selectedItems():
                 self.task_list.itemWidget(s).update_time(+1)
 
 
     def update_total_time(self):
         total = 0
-        for i in range(self.task_list.count()):
-            total += self.task_list.itemWidget(self.task_list.item(i)).get_time()
+        for t in widgets_of_type(list_=self.task_list, type_='task'):
+            total += t.get_time()
 
         self.total_time.setText('Total time: {}'.format(Utils.format_time(total)))
 
     def update_duplicated_tickets_marker(self):
         tickets = {}
 
-        for i in range(self.task_list.count()):
-            widget = self.task_list.itemWidget(self.task_list.item(i))
+        for widget in widgets_of_type(list_=self.task_list, type_='task'):
             ticket_number = widget.ticket_number.text().strip('#')
 
             if ticket_number != '':
                 if ticket_number not in tickets:
                     tickets[ticket_number] = []
 
                 tickets[ticket_number].append(widget)
@@ -647,28 +648,33 @@
             logging.info('Check for update failed: Invalid json response: {}'.format(e))
             self.finished.emit((False, 'Check for update failed: Invalid json response: {}'.format(e), None))
             return
 
         logging.info('Latest available version: {}'.format(resp['info']['version'].strip()))
         self.finished.emit((True, None, resp['info']['version'].strip()))
 
+def widgets_of_type(list_, type_):
+    for i in range(list_.count()):
+        w = list_.itemWidget(list_.item(i))
+        if w.type == type_:
+            yield w
 
 class MainWindow(QMainWindow):
     # dizionario che contiene le informaizoni riguardo ai tempi tracciati
     tasks = None
     # timer che gestisce l'autosave
     tasks_autosave_timer = None
     # thread che cerca aggiornamenti per il software in background
     update_thread = None
 
     def __init__(self, widget):
         QMainWindow.__init__(self)
 
         self.widget = widget
-        self.widget.__main_window = self
+        self.widget._main_window = self
 
         self.oldPos = self.pos()
 
         # carica il file di configurazione e applica alla finestra/applicazione le config salvate
         self.load_config()
         # carica gli elementi dell'interfaccia grafica
         self.load_ui()
@@ -823,17 +829,18 @@
         self.tasks_autosave_timer = QTimer()
         self.tasks_autosave_timer.timeout.connect(self.flush_tasks_to_savefile)
         self.tasks_autosave_timer.start(60 * 1000)
 
     def flush_tasks_to_savefile(self):
         logging.info("Autoflushing tasks to file...")
         self.tasks['current_tasks'].clear()
-        for i in range(self.widget.task_list.count()):
-            t = self.widget.task_list.itemWidget(self.widget.task_list.item(i))
+        i = 0
+        for t in widgets_of_type(list_=self.widget.task_list, type_='task'):
             self.tasks['current_tasks'][str(i)] = t.to_dict()
+            i += 1
         self.tasks.save()
 
     def search_for_updates(self, show_errors):
         def func(result):
             success_check, message_check, new_version = result
 
             if success_check:
@@ -843,29 +850,30 @@
                                                 'The update is completely automatic and takes 1 minute.<br>'
                                                 'Do you wish to update now?'.format(new_version, Globals.version),
                                            positive_button='Yes',
                                            negative_button='No',
                                            html=True)
 
                     if dialog.exec():  # se l'utente ha cliccato su aggiorna lanciamo l'aggiornamento
-                        success_install, message_install = Updater.install_package(Globals.package_name)
+                        success_install, message_install = Updater.install_package(Globals.package_name, new_version)
 
                         if success_install:
                             InformationDialog('Software update', 'Update completed! FSTK will now restart').exec()
                             # imposto la flag first run per mostrare il changelog al riavvio
                             Globals.config['first_run'] = True
                             # salvo lo stato dei contatori e delle configurazioni
                             self.closeEvent(None)
                             # riavvio il processo
                             Updater.restart()
                         else:
-                            InformationDialog('Software update', 'Update failed: {}'.format(message_install)).exec()
+                            message_install = message_install.replace("\n", "<br>")
+                            InformationDialog('Software update', f'Update failed: {message_install}').exec()
                 else:
                     if show_errors:
-                        InformationDialog('Software update', 'You are running the latest version (<b>v{}</b>)'.format(Globals.version.strip())).exec()
+                        InformationDialog('Software update', f'You are running the latest version (<b>v{Globals.version.strip()}</b>)').exec()
 
             else:
                 if show_errors:
                     InformationDialog('Software update', message_check).exec()
 
         # ----------------------------
 
@@ -951,25 +959,23 @@
             self.task_switch_timer.stop()
 
 
     def refresh_ticket_titles(self):
         Globals.config['stats']['ticket_titles_refreshed'] += 1
 
         tickets = []
-        for i in range(self.widget.task_list.count()):
-            t = self.widget.task_list.itemWidget(self.widget.task_list.item(i))
+        for t in widgets_of_type(list_=self.widget.task_list, type_='task'):
             # solo se il task ha un ticket number
             if t.ticket_number.text().strip('# ') != '':
                 tickets.append(t.ticket_number.text().strip('# '))
                 t.ticket_title.setText('...')
 
         def func(result):
             if result is not None:
-                for i in range(self.widget.task_list.count()):
-                    t = self.widget.task_list.itemWidget(self.widget.task_list.item(i))
+                for t in widgets_of_type(list_=self.widget.task_list, type_='task'):
                     # solo se il task ha un ticket number
                     if t.ticket_number.text().strip('# ') != '':
                         text = result.get(t.ticket_number.text().strip('# '))
                         if text is not None:
                             t.ticket_title.setText(text)
                             Utils.set_prop_and_refresh(t.ticket_title, 'invalid', False)
                         else:
@@ -978,24 +984,22 @@
             else:
                 logging.warning('Redmine api call returned empty dict searching for ticket title')
 
 
         Utils.launch_thread(UpdateTicketTitleWorker, [tickets], [('finished', func)])
 
     def clear_all_tasks_times(self):
-        for i in range(self.widget.task_list.count()):
-            w = self.widget.task_list.itemWidget(self.widget.task_list.item(i))
-            w.set_time(0)
+        for t in widgets_of_type(list_=self.widget.task_list, type_='task'):
+            t.set_time(0)
 
 
     def clear_ticket_titles(self):
-        for i in range(self.widget.task_list.count()):
-            w = self.widget.task_list.itemWidget(self.widget.task_list.item(i))
-            w.ticket_title.setText('')
-            w.ticket_title.setProperty('invalid', False)
+        for t in widgets_of_type(list_=self.widget.task_list, type_='task'):
+            t.ticket_title.setText('')
+            t.ticket_title.setProperty('invalid', False)
 
     def set_run_pause(self, state):
         self.widget.running = state
 
         if self.widget.running:
             self.run_pause_button.setStyleSheet('background-color: {}'.format('#630f31' if Globals.config['options']['boomer_compatibility']['invert_run_pause_button'] else '#42630f'))
             self.run_pause_button.setText('pause' if Globals.config['options']['boomer_compatibility']['invert_run_pause_button'] else 'play')
```

## fstk/SaveFiles.py

```diff
@@ -2,35 +2,35 @@
 import logging
 
 from fstk import SavefilesMigrations, Globals
 
 
 class FlushFlagDict(dict):
 
-    __flushed = None
+    _flushed = None
 
     def __init__(self, flush_flag):
         super(FlushFlagDict, self).__init__(self)
 
-        self.__flushed = flush_flag
+        self._flushed = flush_flag
 
     def update(self, *args, **kwargs):
-        self.__flushed[0] = False
+        self._flushed[0] = False
         return super(FlushFlagDict, self).update(*args, **kwargs)
 
     def __setitem__(self, key, value):
         super(FlushFlagDict, self).__setitem__(key, (self.__transparent_obj_conversion(value)))
-        self.__flushed[0] = False
+        self._flushed[0] = False
 
     def __repr__(self):
-        return "<FlushFlagDict ({}) {}>".format('Flushed' if self.__flushed[0] else 'Not flushed', super(FlushFlagDict, self).__repr__())
+        return "<FlushFlagDict ({}) {}>".format('Flushed' if self._flushed[0] else 'Not flushed', super(FlushFlagDict, self).__repr__())
 
     def __transparent_obj_conversion(self, e):
         if isinstance(e, dict):
-            ffd = FlushFlagDict(flush_flag=self.__flushed)
+            ffd = FlushFlagDict(flush_flag=self._flushed)
             ffd.update(e)
             return ffd
         # elif isinstance(e, list):
         #     ffl = FlushFlagList(flush_flag=self.__flushed)
         #     ffl += e
         #     return ffl
         else:
@@ -88,84 +88,84 @@
         return self
 
     def __deepcopy__(self, memo):
         return self
 
 class SaveFile(object):
 
-    __data = None
-    __file = None
-    __flushed = None
+    _data = None
+    _file = None
+    _flushed = None
 
-    __filetypes_migrations = {
+    _filetypes_migrations = {
         'config': (SavefilesMigrations.ConfigMigrations, Globals.config_file_version),
         'tasks': (SavefilesMigrations.TasksMigrations, Globals.tasks_file_version)
     }
 
     def __init__(self, filename, filetype, default=None):
-        if filetype not in self.__filetypes_migrations:
+        if filetype not in self._filetypes_migrations:
             raise ValueError("The specified filetype does not exist ({})".format(filetype))
 
-        self.__file = open(filename, 'a+')
-        self.__file.seek(0)
+        self._file = open(filename, 'a+')
+        self._file.seek(0)
 
-        self.__flushed = UncopiableList([True])
+        self._flushed = UncopiableList([True])
 
         try:
-            self.__data = json.loads(self.__file.read(), object_hook=self.__object_hook)
+            self._data = json.loads(self._file.read(), object_hook=self._object_hook)
             # resetta la flag, che potrebbe essere stata modificata durante il caricamento in memoria dei dati
-            self.__flushed[0] = True
+            self._flushed[0] = True
             # applica le migrazioni al file, nel caso che una versione precedente del software stesse usando un versione precedente del file di salvataggio
-            mig = self.__filetypes_migrations[filetype]
-            self.__data = mig[0]().migrate(self.__data['version'], mig[1], self.__data)
+            mig = self._filetypes_migrations[filetype]
+            self._data = mig[0]().migrate(self._data['version'], mig[1], self._data)
         except json.decoder.JSONDecodeError as e:
-            logging.warning('Exception occurred loading config file ({}): {}. Using default.'.format(self.__file.name, e))
+            logging.warning('Exception occurred loading config file ({}): {}. Using default.'.format(self._file.name, e))
 
             if default is None:
-                self.__data = {}
+                self._data = {}
             else:
-                self.__data = self.__convert_default(default)
+                self._data = self._convert_default(default)
 
             # setto a false la flag, poichè il file non era valido, in modo che venga scritto al prossimo salvataggio
-            self.__flushed[0] = False
+            self._flushed[0] = False
 
     def save(self):
-        if not self.__flushed[0]:
-            self.__file.seek(0)
-            self.__file.truncate()
-            self.__file.write(json.dumps(self.__data, indent=4))
-            self.__file.flush()
-            self.__flushed[0] = True
-            logging.info("Flushing save file ({})...".format(self.__file.name))
+        if not self._flushed[0]:
+            self._file.seek(0)
+            self._file.truncate()
+            self._file.write(json.dumps(self._data, indent=4))
+            self._file.flush()
+            self._flushed[0] = True
+            logging.info("Flushing save file ({})...".format(self._file.name))
         else:
-            logging.info("Save file ({}) nothing to flush.".format(self.__file.name))
+            logging.info("Save file ({}) nothing to flush.".format(self._file.name))
 
-    def __object_hook(self, e):
+    def _object_hook(self, e):
         if isinstance(e, dict):
-            ffd = FlushFlagDict(flush_flag=self.__flushed)
+            ffd = FlushFlagDict(flush_flag=self._flushed)
             ffd.update(e)
             return ffd
         else:
             raise ValueError("L'oggetto passato ({}) non è di un tipo permesso ({}).".format(e, type(e)))
 
-    def __convert_default(self, o):
+    def _convert_default(self, o):
         if isinstance(o, dict):
-            ffd = FlushFlagDict(flush_flag=self.__flushed)
-            ffd.update({k: self.__convert_default(o[k]) for k in o})
+            ffd = FlushFlagDict(flush_flag=self._flushed)
+            ffd.update({k: self._convert_default(o[k]) for k in o})
             return ffd
 
         # elif isinstance(o, list):
         #     ffl = FlushFlagList(flush_flag=self.__flushed)
         #     ffl += [self.__convert_default(e) for e in o]
         #     return ffl
 
         return o
 
     def __getitem__(self, index):
-        return self.__data[index]
+        return self._data[index]
 
     def __setitem__(self, key, value):
-        self.__data[key] = value
-        self.__flushed[0] = False
+        self._data[key] = value
+        self._flushed[0] = False
 
     def __repr__(self):
-        return repr(self.__data)
+        return repr(self._data)
```

## fstk/Updater.py

```diff
@@ -1,34 +1,34 @@
 import logging
 import os
 import subprocess
 import sys
 
 
-def install_package(package_name):
+def install_package(package_name, version):
     logging.debug('Spawning pip to install update...')
-    proc_handle = subprocess.Popen([sys.executable, "-m", "pip", "install", "--upgrade", package_name], stdin=subprocess.DEVNULL, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+    proc_handle = subprocess.Popen([sys.executable, "-m", "pip", "install", f'{package_name}=={version}'], stdin=subprocess.DEVNULL, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
 
     # leggo lo standard output del processo, tenendo conto del timeout
     try:
         stdout, _ = proc_handle.communicate(timeout=10*60)
     except subprocess.TimeoutExpired:
         logging.warning('Pip killed during update beacuse of operation timeout expired')
         # se il timeout del processo scade, lo killo e leggo il suo stdout
         proc_handle.kill()
         # qui si può piantare solo nel caso che il processo stia eseguendo una system call piantata a causa di un fattore esterno.
         # un esempio è la lettura da un disco rimovibile rotto, o un modulo kernel buggato
         stdout, _ = proc_handle.communicate()
 
     if proc_handle.returncode == 0:
         logging.info('Pip update install completed successfully')
-        logging.debug('Pip update install output: "{}"'.format(stdout))
+        logging.debug(f'Pip update install output: "{stdout}"')
         return True, None
     else:
         logging.error('An error occurred trying to install package update: pip exited with code {} and output: "{}"'.format(proc_handle.returncode, stdout))
-        return False, 'Unknow error, see standard output'
+        return False, f'Unknow error occurred, pip returned: {stdout.decode("utf8")}'
 
 
 def restart():
     # riavvia il software dopo aver installato una nuova versione
     # execv magic
     os.execv(sys.executable, ['python3', '-m', 'fstk'])
```

## fstk/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '0.9.1'
+__version__ = '0.9.2'
```

## Comparing `fstk-0.9.1.dist-info/METADATA` & `fstk-0.9.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fstk
-Version: 0.9.1
+Version: 0.9.2
 Summary: Fast Switch Time Keeper
 Author: Meow
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Requires-Dist: PySide2 (>=5.10)
```

## Comparing `fstk-0.9.1.dist-info/RECORD` & `fstk-0.9.2.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-fstk/Dialogs.py,sha256=e8ySUvZU8HVoTqY9l51B0oSFyPjXHak42ytOW71TqpA,28395
-fstk/Fstk.py,sha256=cp8ysQoiKVtsn4Wr2f7ozKe1X_XusC0r7GFEKdU2_dE,44769
+fstk/Dialogs.py,sha256=k6EMNyJecxn5eOiJgH7DXMvHQGneB4eEiWHVSd_SlnE,28588
+fstk/Fstk.py,sha256=1PfCvlm6s4YGbv_phkoCkrN9po_-h0f4kJacxfVzRTs,44667
 fstk/Globals.py,sha256=_kCb6SudubC50N1rMvqOfnCNjRubVT5rKUoHv5t49Pg,2331
 fstk/Palette.py,sha256=lPptRD-QnmRBZxENtXTja_-L9Exs_sdQkgNN0SBJeh8,196
 fstk/Redmine.py,sha256=klfDcygMHuXheZLmXMbSMnbkPckX2l6azEUnebDHhdk,4561
-fstk/SaveFiles.py,sha256=du77EUuO2NoLdDTCEAnyzT4NcLqiuS4R2-AI6cjs3Vg,5879
+fstk/SaveFiles.py,sha256=Pg_RZ1ZxflOf12EUeFwPRKritX0JayivmctrFotOZbM,5834
 fstk/SavefilesMigrations.py,sha256=rhEqQ7eu_GOy66ZpT0jCGaAdm0pnn2EobGBgn8lByII,4279
-fstk/Updater.py,sha256=gERXyiLpDaEJ_Zh8TFMN0Kk3aV_sdpxd5g-sGkP--SE,1547
+fstk/Updater.py,sha256=KDajPD9kMp0uXlH9Msx7nDd7ryou-9Koad9Lc4YtKJc,1579
 fstk/Utils.py,sha256=eMYQFhuOqe0eAuSKmqn1JfY6TLhPEGX2VOwRBfAMHMA,1936
-fstk/__init__.py,sha256=jBymv0cPbifiMUhwR5u0_pyJLbt6IG_MQ2fiM6cwcJE,21
+fstk/__init__.py,sha256=aqzh3Ecm7h661-XD1jLUE6A0k9OzjnKQADweETHcPqs,21
 fstk/__main__.py,sha256=vSycTiXe8OSkUQE_Br18HVZ9F9ex61bVU1dBCIQrqMA,4293
 fstk/assets/Font Awesome 5 Pro-Light-300.otf,sha256=g_fxrf65UtqcxjfbHRG0Q-pV9Uph4avG_XlS3HTItDc,1380376
 fstk/assets/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fstk/assets/fast-switch-time-keeper.desktop,sha256=F-6bXBvp8fjF0R6aJhrzGQIrn2rY5vQTzrKJsKKrrjo,158
 fstk/assets/icon.png,sha256=fmWIYnG-JeyBNPaM9RDO8M2-a55JCoEZoBwsnaZ3fL0,14412
-fstk-0.9.1.dist-info/METADATA,sha256=3UFvi_wEctUYKNUpirdGyyR12Qk9aMKk02m5T7UQhBc,910
-fstk-0.9.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-fstk-0.9.1.dist-info/top_level.txt,sha256=jCGTGXOm3ec6CwE6xHLcuocg-VwLzz8HEeXkE9Ziisk,5
-fstk-0.9.1.dist-info/RECORD,,
+fstk-0.9.2.dist-info/METADATA,sha256=Zm3vgJRVCVdWBfMNpTF8L9sMiP81acRVM_6n_ENq12A,910
+fstk-0.9.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+fstk-0.9.2.dist-info/top_level.txt,sha256=jCGTGXOm3ec6CwE6xHLcuocg-VwLzz8HEeXkE9Ziisk,5
+fstk-0.9.2.dist-info/RECORD,,
```

