# Comparing `tmp/neophaser-0.1.2.tar.gz` & `tmp/neophaser-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neophaser-0.1.2.tar", last modified: Tue Apr 25 02:19:17 2023, max compression
+gzip compressed data, was "neophaser-0.1.3.tar", last modified: Wed Apr 26 03:16:11 2023, max compression
```

## Comparing `neophaser-0.1.2.tar` & `neophaser-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 02:19:17.539664 neophaser-0.1.2/
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-04-25 02:19:07.000000 neophaser-0.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      889 2023-04-25 02:19:17.538664 neophaser-0.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-04-25 02:19:07.000000 neophaser-0.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 02:19:17.535664 neophaser-0.1.2/neophaser/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 02:19:07.000000 neophaser-0.1.2/neophaser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      365 2023-04-25 02:19:07.000000 neophaser-0.1.2/neophaser/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 02:19:17.538664 neophaser-0.1.2/neophaser/assets/
--rw-rw-rw-   0 root         (0) root         (0)    67646 2023-04-25 02:19:07.000000 neophaser-0.1.2/neophaser/assets/icon.ico
--rw-rw-rw-   0 root         (0) root         (0)   208914 2023-04-25 02:19:07.000000 neophaser-0.1.2/neophaser/assets/icon.png
--rw-rw-rw-   0 root         (0) root         (0)     2140 2023-04-25 02:19:07.000000 neophaser-0.1.2/neophaser/board.py
--rw-rw-rw-   0 root         (0) root         (0)     3673 2023-04-25 02:19:07.000000 neophaser-0.1.2/neophaser/controllers.py
--rw-rw-rw-   0 root         (0) root         (0)    10107 2023-04-25 02:19:07.000000 neophaser-0.1.2/neophaser/gui.py
--rw-rw-rw-   0 root         (0) root         (0)      717 2023-04-25 02:19:07.000000 neophaser-0.1.2/neophaser/options.py
--rw-rw-rw-   0 root         (0) root         (0)     1187 2023-04-25 02:19:07.000000 neophaser-0.1.2/neophaser/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1304 2023-04-25 02:19:07.000000 neophaser-0.1.2/neophaser/visual.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 02:19:17.537664 neophaser-0.1.2/neophaser.egg-info/
--rw-r--r--   0 root         (0) root         (0)      889 2023-04-25 02:19:17.000000 neophaser-0.1.2/neophaser.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      417 2023-04-25 02:19:17.000000 neophaser-0.1.2/neophaser.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 02:19:17.000000 neophaser-0.1.2/neophaser.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-04-25 02:19:17.000000 neophaser-0.1.2/neophaser.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-25 02:19:17.000000 neophaser-0.1.2/neophaser.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      725 2023-04-25 02:19:07.000000 neophaser-0.1.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 02:19:17.539664 neophaser-0.1.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:16:11.072574 neophaser-0.1.3/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-04-26 03:16:00.000000 neophaser-0.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      889 2023-04-26 03:16:11.072574 neophaser-0.1.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-04-26 03:16:00.000000 neophaser-0.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:16:11.069574 neophaser-0.1.3/neophaser/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 03:16:00.000000 neophaser-0.1.3/neophaser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      365 2023-04-26 03:16:00.000000 neophaser-0.1.3/neophaser/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:16:11.071574 neophaser-0.1.3/neophaser/assets/
+-rw-rw-rw-   0 root         (0) root         (0)    67646 2023-04-26 03:16:00.000000 neophaser-0.1.3/neophaser/assets/icon.ico
+-rw-rw-rw-   0 root         (0) root         (0)   208914 2023-04-26 03:16:00.000000 neophaser-0.1.3/neophaser/assets/icon.png
+-rw-rw-rw-   0 root         (0) root         (0)     2127 2023-04-26 03:16:00.000000 neophaser-0.1.3/neophaser/board.py
+-rw-rw-rw-   0 root         (0) root         (0)     3654 2023-04-26 03:16:00.000000 neophaser-0.1.3/neophaser/controllers.py
+-rw-rw-rw-   0 root         (0) root         (0)    10896 2023-04-26 03:16:00.000000 neophaser-0.1.3/neophaser/gui.py
+-rw-rw-rw-   0 root         (0) root         (0)      984 2023-04-26 03:16:00.000000 neophaser-0.1.3/neophaser/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1187 2023-04-26 03:16:00.000000 neophaser-0.1.3/neophaser/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2634 2023-04-26 03:16:00.000000 neophaser-0.1.3/neophaser/visual.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:16:11.070574 neophaser-0.1.3/neophaser.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      889 2023-04-26 03:16:11.000000 neophaser-0.1.3/neophaser.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      417 2023-04-26 03:16:11.000000 neophaser-0.1.3/neophaser.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 03:16:11.000000 neophaser-0.1.3/neophaser.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-04-26 03:16:11.000000 neophaser-0.1.3/neophaser.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-26 03:16:11.000000 neophaser-0.1.3/neophaser.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      713 2023-04-26 03:16:00.000000 neophaser-0.1.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 03:16:11.072574 neophaser-0.1.3/setup.cfg
```

### Comparing `neophaser-0.1.2/PKG-INFO` & `neophaser-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neophaser
-Version: 0.1.2
+Version: 0.1.3
 Summary: NEOPHASER; or, audio effects as applied to the retina - an application for applying audio effects to image and video.
 Author-email: 8o-COLLECTIVE <ops@8oc.org>
 Project-URL: homepage, https://neophaser.library.8oc.org
 Project-URL: repository, https://gitlab.com/8o-collective/neophaser
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `neophaser-0.1.2/neophaser/assets/icon.ico` & `neophaser-0.1.3/neophaser/assets/icon.ico`

 * *Files identical despite different names*

### Comparing `neophaser-0.1.2/neophaser/assets/icon.png` & `neophaser-0.1.3/neophaser/assets/icon.png`

 * *Files identical despite different names*

### Comparing `neophaser-0.1.2/neophaser/board.py` & `neophaser-0.1.3/neophaser/board.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,17 +5,14 @@
 from neophaser.options import OptionType, EffectOption
 from neophaser.visual import DataType
 
 class ControllerBoard(list):
 	def __init__(self, visual):
 		super().__init__()
 
-		self.data = visual.data
-
-		self.data_shape = self.data.shape
 		self.type = visual.type
 
 		# we remove color channels so images only have 2 dims, and videos only have 3 dims
 		self.dimensionality_options = EffectOption("Dimensionality", OptionType.DROPDOWN, options=["row", "column"] if self.type == DataType.IMAGE else ["row", "column", "temporal row", "temporal column"])
 		self.sample_rate_options = EffectOption("Sample Rate", OptionType.RANGE_SLIDER, min=10000, max=40000, interval=5000)
 
 		self.options = {
@@ -46,17 +43,17 @@
 		super().remove(item)
 		self.board.remove(item.effect)
 	
 	def insert(self, index, item):
 		super().insert(index, item)
 		self.board.insert(index, item.effect)
 	
-	def process(self):
-		d = self._preprocess(self.data)
+	def process(self, data, sample_rate_multiplier=1):
+		d = self._preprocess(data)
 		self._apply_options()
-		out = self.board(d.astype(np.float32), self.sample_rate).astype(np.uint8)
+		out = self.board(d.astype(np.float32), self.sample_rate*sample_rate_multiplier).astype(np.uint8)
 		return self._postprocess(out)
 
 	def _apply_options(self):
 		self.sample_rate = self.sample_rate_options.value
 		for item in self:
 			item._apply_options()
```

### Comparing `neophaser-0.1.2/neophaser/controllers.py` & `neophaser-0.1.3/neophaser/controllers.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,23 +69,23 @@
 
 		self.options = {
 			"room_size": EffectOption("Room Size", OptionType.RANGE_SLIDER, min=0, max=1, interval=0.1),
 			"damping": EffectOption("Damping", OptionType.RANGE_SLIDER, min=0, max=1, interval=0.1),
 			"wet_level": EffectOption("Wet Level", OptionType.RANGE_SLIDER, min=0, max=1, interval=0.1),
 			"dry_level": EffectOption("Dry Level", OptionType.RANGE_SLIDER, min=0, max=1, interval=0.1),
 			"width": EffectOption("Width", OptionType.RANGE_SLIDER, min=0, max=1, interval=0.1),
-			"freeze_mode": EffectOption("Freeze Mode", OptionType.RANGE_SLIDER, min=0, max=1, interval=0.1),
+			"freeze_mode": EffectOption("Freeze Mode", OptionType.CHECKBOX, on=1, off=0),
 		}
 
 class ResampleController(EffectController):
 	def __init__(self):
 		self.effect = Resample()
 
 		self.options = {
-			"target_sample_rate": EffectOption("Target Sample Rate", OptionType.RANGE_SLIDER, min=0, max=20000, interval=1000),
+			"target_sample_rate": EffectOption("Target Sample Rate", OptionType.RANGE_SLIDER, min=1, max=20000, interval=1000),
 		}
 
 controllers = {
 	"Chorus": ChorusController,
 	"Delay": DelayController,
 	"HighShelf": HighShelfFilterController,
 	"LowShelf": LowShelfFilterController,
```

### Comparing `neophaser-0.1.2/neophaser/gui.py` & `neophaser-0.1.3/neophaser/gui.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import cv2
-import imageio
 
 import numpy as np
 
-from PyQt6.QtCore import Qt, QMimeData, QByteArray, QDataStream, QIODevice, QUrl, QThread, QMutex, QMutexLocker, pyqtSignal
-from PyQt6.QtWidgets import QMainWindow, QWidget, QPushButton, QLabel, QGridLayout, QListWidget, QListWidgetItem, QComboBox, QHBoxLayout, QVBoxLayout, QFormLayout, QCheckBox, QSlider, QGroupBox, QSplitter, QFileDialog
+from PyQt6.QtCore import Qt, QMimeData, QByteArray, QDataStream, QIODevice, QUrl, QThread, QMutex, QMutexLocker, QSize, pyqtSignal
+from PyQt6.QtWidgets import QApplication, QMainWindow, QWidget, QPushButton, QLabel, QGridLayout, QListWidget, QListWidgetItem, QComboBox, QHBoxLayout, QVBoxLayout, QFormLayout, QCheckBox, QSlider, QGroupBox, QSplitter, QFileDialog, QMessageBox
 from PyQt6.QtMultimedia import QMediaPlayer
 from PyQt6.QtGui import QPixmap, QImage
 
 from neophaser.board import ControllerBoard
 from neophaser.controllers import controllers
 from neophaser.options import OptionType
 from neophaser.utils import DecimalSlider
@@ -17,22 +16,22 @@
 class VideoThread(QThread):
 	frame_ready = pyqtSignal(np.ndarray)
 	frame = 0
 
 	def __init__(self, visual, parent=None):
 		super().__init__(parent)
 		self.visual = visual
-		self.frames = visual.data.shape[0]
+		self.frames = visual.preview.shape[0]
 		self._running = True
 		self.mutex = QMutex()
 
 	def run(self):
 		while self._running:
 			self.frame = (self.frame + 1) % self.frames
-			self.frame_ready.emit(self.visual.data[self.frame])
+			self.frame_ready.emit(self.visual.preview[self.frame])
 			QThread.msleep(30)
 	
 	def stop(self):
 		with QMutexLocker(self.mutex):
 			self._running = False
 
 
@@ -51,75 +50,85 @@
 		layout.addLayout(controls_layout)
 
 		open_file_button = QPushButton("Open")
 		open_file_button.clicked.connect(self.open_file)
 		controls_layout.addWidget(open_file_button)
 
 		self.save_file_button = QPushButton("Save")
-		self.save_file_button.clicked.connect(self.save_file)
 		controls_layout.addWidget(self.save_file_button)
 		self.save_file_button.hide()
 
-		# Image and video display
 		self.media_display = QLabel(self)
-		# self.media_display.setScaledContents(True)
-		# self.media_display.setMinimumSize(480, 270)
 		layout.addWidget(self.media_display)
 
 		self.setLayout(layout)
 
 		# Media player
 		self.media_player = QMediaPlayer(self)
-		# self.video_widget = QVideoWidget(self)
-		# self.media_player.setVideoOutput(self.video_widget)
 		self.media_player.mediaStatusChanged.connect(self.media_status_changed)
 
 		self.video_thread = None
 
+		# Enable drag and drop
+		self.setAcceptDrops(True)
+
+	def dragEnterEvent(self, event):
+		if event.mimeData().hasUrls():
+			event.acceptProposedAction()
+
+	def dropEvent(self, event):
+		for url in event.mimeData().urls():
+			file_path = url.toLocalFile()
+			self.load_media(file_path)
+			break  # Only load the first file
+
 	def open_file(self):
 		file_path, _ = QFileDialog.getOpenFileName(self, "Open Media File", "", "Images (*.png *.jpg *.jpeg);;Videos (*.gif *.mp4 *.avi)")
 
 		if file_path:
-			self.media_player.setSource(QUrl.fromLocalFile(file_path))
+			self.load_media(file_path)
+
+	def load_media(self, file_path):
+		if not Visual.check_valid_file(file_path):
+			return QMessageBox.critical(
+				self,
+				"Invalid File",
+				"The file is not a valid image or video format.",
+				buttons=QMessageBox.StandardButton.Ok,
+				defaultButton=QMessageBox.StandardButton.Ok,
+			)
+
+		self.media_player.setSource(QUrl.fromLocalFile(file_path))
 
-			self.visual = Visual(file_path)
-			self.data = self.visual.data
+		self.visual = Visual(file_path)
+		self.data = self.visual.preview
 
-			self.loaded.emit()
+		self.loaded.emit()
 
-			self.save_file_button.show()
+		self.save_file_button.show()
 
-			self.set_data(self.visual)
+		self.set_data(self.visual)
 	
 	def set_data(self, visual):
 		self.visual = visual
-		self.data = self.visual.data
+		self.data = self.visual.preview
 
 		if visual.type == DataType.IMAGE:
 			self.update_frame(self.data)
 		elif self.visual.type == DataType.VIDEO:
 			if self.video_thread:
 				self.video_thread.stop()
 				self.video_thread.wait()
 			self.video_thread = VideoThread(self.visual)
 			self.video_thread.frame_ready.connect(self.update_frame)
 			self.video_thread.start()
 	
 	def update_frame(self, frame):
-		self.media_display.setPixmap(QPixmap.fromImage(QImage(frame, frame.shape[1], frame.shape[0], frame.strides[0], QImage.Format.Format_RGB888).rgbSwapped()))
-	
-	def save_file(self):
-		file_path, _ = QFileDialog.getSaveFileName(parent=self, caption='Save File', directory='', filter="Images (*.png *.jpg *.jpeg);;Animated (*.gif);;All files (*)")
-		
-
-		if file_path:
-			if self.visual.type == DataType.IMAGE:
-				cv2.imwrite(file_path, self.visual.data)
-			elif self.visual.type == DataType.VIDEO:
-				imageio.mimwrite(file_path, self.visual.data, fps=30)
+		pixmap = QPixmap.fromImage(QImage(frame, frame.shape[1], frame.shape[0], frame.strides[0], QImage.Format.Format_RGB888).rgbSwapped())
+		self.media_display.setPixmap(pixmap)
 
 	def media_status_changed(self, status):
 		if status == QMediaPlayer.MediaStatus.EndOfMedia:
 			self.video_widget.setHidden(True)
 			self.media_display.setHidden(False)
 			self.layout().removeWidget(self.video_widget)
 
@@ -146,41 +155,42 @@
 		self.options_stack = QGroupBox()
 		self.options_stack.setMinimumWidth(450)
 		self.options_layout = QFormLayout()
 		self.options_stack.setLayout(self.options_layout)
 
 		for option in effect.options.values():
 			option.callback = lambda v, opt=option: (
-				setattr(opt, "value", v),
+				opt.set_value(v),
 				self.render.emit(),
 			)
 
 			if option.type == OptionType.CHECKBOX:
 				checkbox = QCheckBox()
-				checkbox.setValue(option.value)
+				checkbox.setChecked(True if option.value == option.on else False)
 				checkbox.stateChanged.connect(option.callback)
 				self.options_layout.addRow(option.name, checkbox)
 			elif option.type == OptionType.DROPDOWN:
 				dropdown = QComboBox()
 				for drop in option.options:
 					dropdown.addItem(drop)
 				dropdown.setCurrentText(option.value)
 				dropdown.currentTextChanged.connect(option.callback)
 				self.options_layout.addRow(option.name, dropdown)
 			elif option.type == OptionType.RANGE_SLIDER:
 				if option.interval < 1:
 					slider = DecimalSlider()
-					# slider.setValue(option.value)
+					slider.setRange(option.min, option.max)
+					slider.setValue(option.value)
 					slider.decimalValueChanged.connect(option.callback)
 				else:
 					slider = QSlider(orientation=Qt.Orientation.Horizontal)
-					# slider.setValue(int(option.value))
+					slider.setRange(option.min, option.max)
+					slider.setValue(int(option.value))
 					slider.valueChanged.connect(option.callback)
 				slider.setMinimumWidth(250)
-				slider.setRange(option.min, option.max)
 				slider.setTickPosition(QSlider.TickPosition.TicksBelow)
 				slider.setTickInterval(option.interval)
 				self.options_layout.addRow(option.name, slider)
 
 		self.options_stack.setLayout(self.options_layout)
 		self.layout().addWidget(self.options_stack)
 		
@@ -294,15 +304,15 @@
 		
 		self.render.emit()
 
 	def show_effect_options(self, current, previous):
 		if current is not None:
 			item_index = self.list_widget.row(current)
 			effect_item = self.board[item_index]
-			self.effect_options_widget.set_options(effect_item)  # Just an example to change options based on index
+			self.effect_options_widget.set_options(effect_item)
 		else:
 			self.effect_options_widget.set_options(self.board)
 
 class MainWindow(QMainWindow):
 	def __init__(self):
 		super().__init__()
 
@@ -312,28 +322,45 @@
 
 		# button = QPushButton("Quit")
 		# button.pressed.connect(self.close)
 		# layout.addWidget(button, 0, 0)
 
 		self.media_player = MediaLoader()
 		self.media_player.loaded.connect(self.load_board)
+		self.media_player.save_file_button.clicked.connect(self.render_and_save)
 		self.layout.addWidget(self.media_player, 0, 0)
 
 		widget = QWidget()
 		widget.setLayout(self.layout)
 		self.setCentralWidget(widget)
 		self.show()
 	
 	def load_board(self):
 		self.visual = self.media_player.visual
-		self.data = self.visual.data
+		self.data = self.visual.preview
 
 		self.board = ControllerBoard(self.visual)
 		board_manager = BoardWidget(self.board)
 
 		board_manager.render.connect(self.process_visual)
 
 		self.layout.addWidget(board_manager, 0, 1)
 	
 	def process_visual(self):
-		self.visual.data = self.board.process()
-		self.media_player.set_data(self.visual)
+		self.visual.preview = self.board.process(self.data, sample_rate_multiplier=self.visual.sample_rate_multiplier)
+		self.media_player.set_data(self.visual)
+	
+	def render_and_save(self):
+		file_path, _ = QFileDialog.getSaveFileName(parent=self, caption='Save File', directory='', filter="Images (*.png *.jpg *.jpeg);;Animated (*.gif);;All files (*)")
+
+		rendered = self.board.process(self.visual.original)
+
+		if file_path:
+			if self.visual.type == DataType.IMAGE:
+				cv2.imwrite(file_path, rendered)
+			elif self.visual.type == DataType.VIDEO:
+				fps = 30
+				_, height, width, _ = rendered.shape
+				out = cv2.VideoWriter(file_path, cv2.VideoWriter_fourcc('M','J','P','G'), fps, (width, height))
+				for frame in rendered:
+					out.write(frame)
+				out.release()
```

### Comparing `neophaser-0.1.2/neophaser/options.py` & `neophaser-0.1.3/neophaser/options.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,20 +10,30 @@
 class EffectOption:
 	def __init__(self, name, t, **kwargs):
 		self.name = name
 		self.type = t
 
 		self.value = None
 
-		if self.type == OptionType.DROPDOWN:
+		if self.type == OptionType.CHECKBOX:
+			self.on = kwargs["on"]
+			self.off = kwargs["off"]
+			self.value = self.off
+		elif self.type == OptionType.DROPDOWN:
 			self.options = kwargs["options"]
 			self.value = self.options[0]
 		elif self.type == OptionType.RANGE_SLIDER:
 			self.min = kwargs["min"]
 			self.max = kwargs["max"]
 			self.interval = kwargs["interval"]
 			self.value = self.min + ((self.max - self.min) / 2)
+	
+	def set_value(self, value):
+		if self.type == OptionType.CHECKBOX:
+			self.value = self.on if value else self.off
+		else:
+			self.value = value
 
 class EffectController():
 	def _apply_options(self):
 		for (name, option) in self.options.items():
 			setattr(self.effect, name, option.value)
```

### Comparing `neophaser-0.1.2/neophaser/utils.py` & `neophaser-0.1.3/neophaser/utils.py`

 * *Files identical despite different names*

### Comparing `neophaser-0.1.2/neophaser/visual.py` & `neophaser-0.1.3/neophaser/visual.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,35 +6,67 @@
 
 # image and video file types enum
 class DataType(enum.Enum):
 	IMAGE = enum.auto()
 	VIDEO = enum.auto()
 
 class Visual:
-	def __init__(self, path):
+	def __init__(self, path, max_width=500, max_height=500):
 		self.path = path
+		
+		self.preview_dimensions = (max_width, max_height)
 
-		mime_type, _ = mimetypes.guess_type(self.path)
+		self.type = self.check_valid_file(path)
 
-		if mime_type.startswith("video") or mime_type == "image/gif":
-			self.type = DataType.VIDEO
-			self.data = self._read_video()
-		elif mime_type.startswith("image"):
-			self.type = DataType.IMAGE
-			self.data = self._read_image()
+		if self.type == DataType.VIDEO:
+			self.original = self._read_video()
+			self.preview = self._resize_video(self.original.copy())
+		elif self.type == DataType.IMAGE:
+			self.original = self._read_image()
+			self.preview = self._resize_image(self.original.copy())
 		else:
 			raise ValueError("The file is neither an image nor a video.")
 
-		self.original = self.data
+		self.sample_rate_multiplier = self.preview.size / self.original.size
 
 		self.effects = []
+	
+	@staticmethod
+	def check_valid_file(path):
+		mime_type, _ = mimetypes.guess_type(path)
+
+		if mime_type is None:
+			return False
+
+		if mime_type.startswith("video") or mime_type == "image/gif":
+			return DataType.VIDEO
+		elif mime_type.startswith("image"):
+			return DataType.IMAGE
+		else:
+			return False
 
 	def _read_image(self):
 		return cv2.imread(self.path)
 
+	def _resize_image(self, image):		
+		# Get the dimensions of the image
+		height, width, _ = image.shape
+
+		aspect_ratio = width / height
+
+		if width > height:
+			width = min(self.preview_dimensions[0], width)
+			height = int(width / aspect_ratio)
+		else: 
+			height = min(self.preview_dimensions[1], height)
+			width = int(height * aspect_ratio)
+
+		# Resize the image
+		return cv2.resize(image, (width, height))
+
 	def _read_video(self):
 		cap = cv2.VideoCapture(self.path)
 
 		num_frames = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
 
 		height = int(cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
 		width = int(cap.get(cv2.CAP_PROP_FRAME_WIDTH))
@@ -52,7 +84,23 @@
 			video_array[frame_index] = frame
 			frame_index += 1
 
 		# Release the video capture object
 		cap.release()
 
 		return video_array
+
+	def _resize_video(self, video):
+		# Get the dimensions of the video
+		num_frames, height, width, _ = video.shape
+
+		aspect_ratio = width / height
+
+		if width > height:
+			width = min(self.preview_dimensions[0], width)
+			height = int(width / aspect_ratio)
+		else: 
+			height = min(self.preview_dimensions[1], height)
+			width = int(height * aspect_ratio)
+
+		# Resize the video
+		return np.array([cv2.resize(frame, (width, height)) for frame in video])
```

### Comparing `neophaser-0.1.2/neophaser.egg-info/PKG-INFO` & `neophaser-0.1.3/neophaser.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neophaser
-Version: 0.1.2
+Version: 0.1.3
 Summary: NEOPHASER; or, audio effects as applied to the retina - an application for applying audio effects to image and video.
 Author-email: 8o-COLLECTIVE <ops@8oc.org>
 Project-URL: homepage, https://neophaser.library.8oc.org
 Project-URL: repository, https://gitlab.com/8o-collective/neophaser
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `neophaser-0.1.2/pyproject.toml` & `neophaser-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "neophaser"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="8o-COLLECTIVE", email="ops@8oc.org" },
 ]
 description = "NEOPHASER; or, audio effects as applied to the retina - an application for applying audio effects to image and video."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
@@ -14,15 +14,14 @@
     "Operating System :: OS Independent",
 ]
 dependencies = [
 	"numpy",
 	"opencv-python",
 	"pyqt6",
 	"pedalboard",
-	"imageio",
 ]
 
 [project.urls]
 homepage = "https://neophaser.library.8oc.org"
 repository = "https://gitlab.com/8o-collective/neophaser"
 
 [build-system]
```

