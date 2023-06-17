# Comparing `tmp/neophaser-0.1.4.tar.gz` & `tmp/neophaser-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neophaser-0.1.4.tar", last modified: Fri May 12 01:37:42 2023, max compression
+gzip compressed data, was "neophaser-0.2.0.tar", last modified: Sat Jun 17 04:58:58 2023, max compression
```

## Comparing `neophaser-0.1.4.tar` & `neophaser-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 01:37:42.780707 neophaser-0.1.4/
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-12 01:37:32.000000 neophaser-0.1.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      889 2023-05-12 01:37:42.780707 neophaser-0.1.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-05-12 01:37:32.000000 neophaser-0.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 01:37:42.776707 neophaser-0.1.4/neophaser/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-12 01:37:32.000000 neophaser-0.1.4/neophaser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      365 2023-05-12 01:37:32.000000 neophaser-0.1.4/neophaser/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 01:37:42.779707 neophaser-0.1.4/neophaser/assets/
--rw-rw-rw-   0 root         (0) root         (0)    67646 2023-05-12 01:37:32.000000 neophaser-0.1.4/neophaser/assets/icon.ico
--rw-rw-rw-   0 root         (0) root         (0)   208914 2023-05-12 01:37:32.000000 neophaser-0.1.4/neophaser/assets/icon.png
--rw-rw-rw-   0 root         (0) root         (0)     2127 2023-05-12 01:37:32.000000 neophaser-0.1.4/neophaser/board.py
--rw-rw-rw-   0 root         (0) root         (0)     3654 2023-05-12 01:37:32.000000 neophaser-0.1.4/neophaser/controllers.py
--rw-rw-rw-   0 root         (0) root         (0)    13886 2023-05-12 01:37:32.000000 neophaser-0.1.4/neophaser/gui.py
--rw-rw-rw-   0 root         (0) root         (0)      984 2023-05-12 01:37:32.000000 neophaser-0.1.4/neophaser/options.py
--rw-rw-rw-   0 root         (0) root         (0)     1187 2023-05-12 01:37:32.000000 neophaser-0.1.4/neophaser/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2683 2023-05-12 01:37:32.000000 neophaser-0.1.4/neophaser/visual.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 01:37:42.778707 neophaser-0.1.4/neophaser.egg-info/
--rw-r--r--   0 root         (0) root         (0)      889 2023-05-12 01:37:42.000000 neophaser-0.1.4/neophaser.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      417 2023-05-12 01:37:42.000000 neophaser-0.1.4/neophaser.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 01:37:42.000000 neophaser-0.1.4/neophaser.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-05-12 01:37:42.000000 neophaser-0.1.4/neophaser.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-12 01:37:42.000000 neophaser-0.1.4/neophaser.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      713 2023-05-12 01:37:32.000000 neophaser-0.1.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 01:37:42.780707 neophaser-0.1.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:58:58.681628 neophaser-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-06-17 04:58:50.000000 neophaser-0.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      889 2023-06-17 04:58:58.681628 neophaser-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-06-17 04:58:50.000000 neophaser-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:58:58.679628 neophaser-0.2.0/neophaser/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-17 04:58:50.000000 neophaser-0.2.0/neophaser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      365 2023-06-17 04:58:50.000000 neophaser-0.2.0/neophaser/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:58:58.680628 neophaser-0.2.0/neophaser/assets/
+-rw-rw-rw-   0 root         (0) root         (0)    67646 2023-06-17 04:58:50.000000 neophaser-0.2.0/neophaser/assets/icon.ico
+-rw-rw-rw-   0 root         (0) root         (0)   208914 2023-06-17 04:58:50.000000 neophaser-0.2.0/neophaser/assets/icon.png
+-rw-rw-rw-   0 root         (0) root         (0)     3071 2023-06-17 04:58:50.000000 neophaser-0.2.0/neophaser/board.py
+-rw-rw-rw-   0 root         (0) root         (0)     4132 2023-06-17 04:58:50.000000 neophaser-0.2.0/neophaser/controllers.py
+-rw-rw-rw-   0 root         (0) root         (0)    15208 2023-06-17 04:58:50.000000 neophaser-0.2.0/neophaser/gui.py
+-rw-rw-rw-   0 root         (0) root         (0)      984 2023-06-17 04:58:50.000000 neophaser-0.2.0/neophaser/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1187 2023-06-17 04:58:50.000000 neophaser-0.2.0/neophaser/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2683 2023-06-17 04:58:50.000000 neophaser-0.2.0/neophaser/visual.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:58:58.680628 neophaser-0.2.0/neophaser.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      889 2023-06-17 04:58:58.000000 neophaser-0.2.0/neophaser.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      417 2023-06-17 04:58:58.000000 neophaser-0.2.0/neophaser.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-17 04:58:58.000000 neophaser-0.2.0/neophaser.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-17 04:58:58.000000 neophaser-0.2.0/neophaser.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-17 04:58:58.000000 neophaser-0.2.0/neophaser.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      713 2023-06-17 04:58:50.000000 neophaser-0.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-17 04:58:58.681628 neophaser-0.2.0/setup.cfg
```

### Comparing `neophaser-0.1.4/PKG-INFO` & `neophaser-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neophaser
-Version: 0.1.4
+Version: 0.2.0
 Summary: NEOPHASER; or, audio effects as applied to the retina - an application for applying audio effects to image and video.
 Author-email: 8o-COLLECTIVE <ops@8oc.org>
 Project-URL: homepage, https://neophaser.library.8oc.org
 Project-URL: repository, https://gitlab.com/8o-collective/neophaser
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `neophaser-0.1.4/neophaser/assets/icon.ico` & `neophaser-0.2.0/neophaser/assets/icon.ico`

 * *Files identical despite different names*

### Comparing `neophaser-0.1.4/neophaser/assets/icon.png` & `neophaser-0.2.0/neophaser/assets/icon.png`

 * *Files identical despite different names*

### Comparing `neophaser-0.1.4/neophaser/board.py` & `neophaser-0.2.0/neophaser/board.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,36 +8,47 @@
 class ControllerBoard(list):
 	def __init__(self, visual):
 		super().__init__()
 
 		self.type = visual.type
 
 		# we remove color channels so images only have 2 dims, and videos only have 3 dims
-		self.dimensionality_options = EffectOption("Dimensionality", OptionType.DROPDOWN, options=["row", "column"] if self.type == DataType.IMAGE else ["row", "column", "temporal row", "temporal column"])
+		self.dimensionality_options = EffectOption("Dimensionality", OptionType.DROPDOWN, options=["row", "column"] if self.type == DataType.IMAGE else ["row", "column", "temporal row", "temporal column", "pseudo-temporal row(?)", "pseudo-temporal column(?)"])
 		self.sample_rate_options = EffectOption("Sample Rate", OptionType.RANGE_SLIDER, min=10000, max=40000, interval=5000)
 
 		self.options = {
 			"dimensionality": self.dimensionality_options,
 			"sample_rate": self.sample_rate_options,
 		}
 
 		self.board = Pedalboard()
 
 	def _preprocess(self, data):
-		self.dimensionality_lookup = [(0, 1, 2), (1, 0, 2)] if self.type == DataType.IMAGE else [(0, 1, 2, 3), (0, 2, 1, 3), (2, 0, 1, 3), (2, 1, 0, 3)]
+		self.dimensionality_lookup = [(0, 1, 2), (1, 0, 2)] if self.type == DataType.IMAGE else [(0, 1, 2, 3), (0, 2, 1, 3), (1, 2, 0, 3), (2, 1, 0, 3), (1, 0, 2, 3), (2, 0, 1, 3)]
 		self.dimensionality_transpose = self.dimensionality_lookup[self.dimensionality_options.options.index(self.dimensionality_options.value)]
 
+		self.original_shape = data.shape
 		transposed_data = np.transpose(data, self.dimensionality_transpose).copy()
 		self.process_shape = transposed_data.shape
 		return transposed_data.flatten()
 
 	def _postprocess(self, audio):
 		shaped_data = np.reshape(audio, self.process_shape)
-		transposed_data = np.transpose(shaped_data, self.dimensionality_transpose).copy()
-		return transposed_data.astype(np.uint8)
+		involuted_data = np.transpose(shaped_data, self.dimensionality_transpose).copy()
+
+		# wanna see the worst hack of all time?
+
+		# basically if our "transposition" (really a permutation of axes on a tensor) permutes more than 2 axes it's not an involution
+		# it has to be called as many times as the axes were changed to get back to the original shape (god damned group theory)
+		# in our case we're only in 4 dimensions, 3 because we don't care about the color channel
+		# so we can just transpose twice to get back to the original shape because we'll never permute more than 2 axes
+		if involuted_data.shape != self.original_shape:
+			involuted_data = np.transpose(involuted_data, self.dimensionality_transpose).copy()
+			
+		return involuted_data.astype(np.uint8)
 	
 	def append(self, item):
 		super().append(item)
 		self.board.append(item.effect)
 	
 	def remove(self, item):
 		super().remove(item)
@@ -51,9 +62,11 @@
 		d = self._preprocess(data)
 		self._apply_options()
 		out = self.board(d.astype(np.float32), self.sample_rate*sample_rate_multiplier).astype(np.uint8)
 		return self._postprocess(out)
 
 	def _apply_options(self):
 		self.sample_rate = self.sample_rate_options.value
-		for item in self:
+		for index, item in enumerate(self):
+			if self.board[index] != item.effect: # update any effects that have been changed
+				self.board[index] = item.effect # only really used for external plugin effects
 			item._apply_options()
```

### Comparing `neophaser-0.1.4/neophaser/controllers.py` & `neophaser-0.2.0/neophaser/controllers.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 	Chorus,
 	Delay,
 	HighShelfFilter,
 	LowShelfFilter,
 	Phaser,
 	Reverb,
 	Resample,
+
+	AudioUnitPlugin,
+	Plugin,
+	VST3Plugin,
 )
 
 from neophaser.options import EffectController, EffectOption, OptionType
 
 class ChorusController(EffectController):
 	def __init__(self):
 		self.effect = Chorus()
@@ -80,16 +84,39 @@
 	def __init__(self):
 		self.effect = Resample()
 
 		self.options = {
 			"target_sample_rate": EffectOption("Target Sample Rate", OptionType.RANGE_SLIDER, min=1, max=20000, interval=1000),
 		}
 
+class PluginController():
+	def __init__(self):
+		self.effect = None # noop until we load the file
+
+		self.options = None
+		self.loaded = False
+	
+	def _apply_options(self):
+		pass
+
+	def load_plugin(self, path):
+		if path.endswith(".component"):
+			self.effect = AudioUnitPlugin(path)
+		else:
+			self.effect = VST3Plugin(path)
+		
+		self.loaded = True
+	
+	def open_plugin_ui(self):
+		self.effect.show_editor()
+
 controllers = {
 	"Chorus": ChorusController,
 	"Delay": DelayController,
 	"HighShelf": HighShelfFilterController,
 	"LowShelf": LowShelfFilterController,
 	"Phaser": PhaserController,
 	"Reverb": ReverbController,
 	"Resample": ResampleController,
+
+	"Plugin": PluginController,
 }
```

### Comparing `neophaser-0.1.4/neophaser/gui.py` & `neophaser-0.2.0/neophaser/gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import mimetypes
 import os
+import platform
 
 import cv2
 
 import numpy as np
 
 from PyQt6.QtCore import Qt, QMimeData, QByteArray, QDataStream, QIODevice, QUrl, QThread, QMutex, QMutexLocker, QSize, pyqtSignal
 from PyQt6.QtWidgets import QApplication, QMainWindow, QWidget, QPushButton, QLabel, QGridLayout, QListWidget, QListWidgetItem, QComboBox, QHBoxLayout, QVBoxLayout, QFormLayout, QCheckBox, QSlider, QGroupBox, QSplitter, QFileDialog, QMessageBox
@@ -128,26 +130,26 @@
 	def dropEvent(self, event):
 		for url in event.mimeData().urls():
 			file_path = url.toLocalFile()
 			self.load_media(file_path)
 			break  # Only load the first file
 
 	def open_file(self):
-		file_paths, _ = QFileDialog.getOpenFileNames(self, "Open Media File", "", "Images (*.png *.jpg *.jpeg);;Videos (*.gif *.mp4 *.avi)")
+		file_paths, _ = QFileDialog.getOpenFileNames(self, "Open Media File", "", f"Images and Videos ({' *'.join([ext for ext, mime in mimetypes.types_map.items() if mime.startswith('image/') or mime.startswith('video/')])});;All Files (*)")
 
 		if file_paths:
 			self.load_media(file_paths)
 
 	def load_media(self, file_paths):
 		for file_path in file_paths:
 			if not Visual.check_valid_file(file_path):
 				return QMessageBox.critical(
 					self,
 					"Invalid File",
-					f"{file_path} is not a valid image or video format.",
+					f"{file_path} is not a valid if self.visual.type == DataType.IMAGEor video format.",
 					buttons=QMessageBox.StandardButton.Ok,
 					defaultButton=QMessageBox.StandardButton.Ok,
 				)
 		
 		if len(file_paths) == 1:
 			file_path = file_paths[0]
 
@@ -221,47 +223,74 @@
 		self.layout().removeWidget(self.options_stack)
 
 		self.options_stack = QGroupBox()
 		self.options_stack.setMinimumWidth(450)
 		self.options_layout = QFormLayout()
 		self.options_stack.setLayout(self.options_layout)
 
-		for option in effect.options.values():
-			option.callback = lambda v, opt=option: (
-				opt.set_value(v),
-				self.render.emit(),
-			)
-
-			if option.type == OptionType.CHECKBOX:
-				checkbox = QCheckBox()
-				checkbox.setChecked(True if option.value == option.on else False)
-				checkbox.stateChanged.connect(option.callback)
-				self.options_layout.addRow(option.name, checkbox)
-			elif option.type == OptionType.DROPDOWN:
-				dropdown = QComboBox()
-				for drop in option.options:
-					dropdown.addItem(drop)
-				dropdown.setCurrentText(option.value)
-				dropdown.currentTextChanged.connect(option.callback)
-				self.options_layout.addRow(option.name, dropdown)
-			elif option.type == OptionType.RANGE_SLIDER:
-				if option.interval < 1:
-					slider = DecimalSlider()
-					slider.setRange(option.min, option.max)
-					slider.setValue(option.value)
-					slider.decimalValueChanged.connect(option.callback)
-				else:
-					slider = QSlider(orientation=Qt.Orientation.Horizontal)
-					slider.setRange(option.min, option.max)
-					slider.setValue(int(option.value))
-					slider.valueChanged.connect(option.callback)
-				slider.setMinimumWidth(250)
-				slider.setTickPosition(QSlider.TickPosition.TicksBelow)
-				slider.setTickInterval(option.interval)
-				self.options_layout.addRow(option.name, slider)
+		if effect.options == None: # this is an AU/VST3
+			if effect.loaded:
+				# stuff
+				open_plugin_ui_button = QPushButton("Open plugin UI")
+				open_plugin_ui_button.clicked.connect(effect.open_plugin_ui)
+				render_button = QPushButton("Render")
+				render_button.clicked.connect(self.render.emit)
+
+				self.options_layout.addRow(open_plugin_ui_button)
+				self.options_layout.addRow(render_button)
+			else:
+				plugin_path = "/Library/Audio/Plug-Ins/VST3/"
+				if platform.system() == "Windows":
+					plugin_path = "C:/Program Files/Common Files/VST3/"
+				elif platform.system() == "Linux":
+					plugin_path = "/usr/lib/vst3/"
+
+				load_plugin_from_path = lambda: (
+					effect.load_plugin(QFileDialog.getOpenFileName(self, "Open Plugin", plugin_path, "Audio Plugin (*.dll *.vst3 *.component *.so)")[0]),
+					self.set_options(effect),
+					self.render.emit(),
+				)
+
+				load_plugin_button = QPushButton("Load plugin")
+				load_plugin_button.clicked.connect(load_plugin_from_path)
+				self.options_layout.addRow(load_plugin_button)
+		else:
+			for option in effect.options.values():
+				option.callback = lambda v, opt=option: (
+					opt.set_value(v),
+					self.render.emit(),
+				)
+
+				if option.type == OptionType.CHECKBOX:
+					checkbox = QCheckBox()
+					checkbox.setChecked(True if option.value == option.on else False)
+					checkbox.stateChanged.connect(option.callback)
+					self.options_layout.addRow(option.name, checkbox)
+				elif option.type == OptionType.DROPDOWN:
+					dropdown = QComboBox()
+					for drop in option.options:
+						dropdown.addItem(drop)
+					dropdown.setCurrentText(option.value)
+					dropdown.currentTextChanged.connect(option.callback)
+					self.options_layout.addRow(option.name, dropdown)
+				elif option.type == OptionType.RANGE_SLIDER:
+					if option.interval < 1:
+						slider = DecimalSlider()
+						slider.setRange(option.min, option.max)
+						slider.setValue(option.value)
+						slider.decimalValueChanged.connect(option.callback)
+					else:
+						slider = QSlider(orientation=Qt.Orientation.Horizontal)
+						slider.setRange(option.min, option.max)
+						slider.setValue(int(option.value))
+						slider.valueChanged.connect(option.callback)
+					slider.setMinimumWidth(250)
+					slider.setTickPosition(QSlider.TickPosition.TicksBelow)
+					slider.setTickInterval(option.interval)
+					self.options_layout.addRow(option.name, slider)
 
 		self.options_stack.setLayout(self.options_layout)
 		self.layout().addWidget(self.options_stack)
 		
 class DraggableListWidget(QListWidget):
 	render = pyqtSignal()
 
@@ -425,33 +454,37 @@
 			directory_path = QFileDialog.getExistingDirectory(parent=self, caption='Save Files', directory='')
 
 			if directory_path:
 				for visual, file_path in zip(self.media_player.visuals, self.media_player.file_paths):
 					rendered = self.board.process(visual.original)
 
 					filename = os.path.basename(file_path)
+
+					if visual.type == DataType.VIDEO:
+						filename = os.path.splitext(filename)[0] + '.webm'
+
 					save_path = os.path.join(directory_path, filename)
 
 					if visual.type == DataType.IMAGE:
 						cv2.imwrite(save_path, rendered)
 					elif visual.type == DataType.VIDEO:
 						fps = 30
 						_, height, width, _ = rendered.shape
-						out = cv2.VideoWriter(save_path, cv2.VideoWriter_fourcc('M','J','P','G'), fps, (width, height))
+						out = cv2.VideoWriter(save_path, cv2.VideoWriter_fourcc(*'VP90'), fps, (width, height))
 						for frame in rendered:
 							out.write(frame)
 						out.release()
 		else:
-			file_path, _ = QFileDialog.getSaveFileName(parent=self, caption='Save File', directory='', filter="Images (*.png *.jpg *.jpeg);;Animated (*.gif);;All files (*)")
+			file_path, _ = QFileDialog.getSaveFileName(parent=self, caption='Save File', directory='output' + ('.png' if self.visual.type == DataType.IMAGE else '.webm'))
 
 			rendered = self.board.process(self.visual.original)
 
 			if file_path:
 				if self.visual.type == DataType.IMAGE:
 					cv2.imwrite(file_path, rendered)
 				elif self.visual.type == DataType.VIDEO:
 					fps = 30
 					_, height, width, _ = rendered.shape
-					out = cv2.VideoWriter(file_path, cv2.VideoWriter_fourcc('M','J','P','G'), fps, (width, height))
+					out = cv2.VideoWriter(file_path, cv2.VideoWriter_fourcc(*'VP90'), fps, (width, height))
 					for frame in rendered:
 						out.write(frame)
 					out.release()
```

### Comparing `neophaser-0.1.4/neophaser/options.py` & `neophaser-0.2.0/neophaser/options.py`

 * *Files identical despite different names*

### Comparing `neophaser-0.1.4/neophaser/utils.py` & `neophaser-0.2.0/neophaser/utils.py`

 * *Files identical despite different names*

### Comparing `neophaser-0.1.4/neophaser/visual.py` & `neophaser-0.2.0/neophaser/visual.py`

 * *Files identical despite different names*

### Comparing `neophaser-0.1.4/neophaser.egg-info/PKG-INFO` & `neophaser-0.2.0/neophaser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neophaser
-Version: 0.1.4
+Version: 0.2.0
 Summary: NEOPHASER; or, audio effects as applied to the retina - an application for applying audio effects to image and video.
 Author-email: 8o-COLLECTIVE <ops@8oc.org>
 Project-URL: homepage, https://neophaser.library.8oc.org
 Project-URL: repository, https://gitlab.com/8o-collective/neophaser
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `neophaser-0.1.4/pyproject.toml` & `neophaser-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "neophaser"
-version = "0.1.4"
+version = "0.2.0"
 authors = [
   { name="8o-COLLECTIVE", email="ops@8oc.org" },
 ]
 description = "NEOPHASER; or, audio effects as applied to the retina - an application for applying audio effects to image and video."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

