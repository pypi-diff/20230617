# Comparing `tmp/neophaser-0.1.3.tar.gz` & `tmp/neophaser-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neophaser-0.1.3.tar", last modified: Wed Apr 26 03:16:11 2023, max compression
+gzip compressed data, was "neophaser-0.1.4.tar", last modified: Fri May 12 01:37:42 2023, max compression
```

## Comparing `neophaser-0.1.3.tar` & `neophaser-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:16:11.072574 neophaser-0.1.3/
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-04-26 03:16:00.000000 neophaser-0.1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      889 2023-04-26 03:16:11.072574 neophaser-0.1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-04-26 03:16:00.000000 neophaser-0.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:16:11.069574 neophaser-0.1.3/neophaser/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 03:16:00.000000 neophaser-0.1.3/neophaser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      365 2023-04-26 03:16:00.000000 neophaser-0.1.3/neophaser/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:16:11.071574 neophaser-0.1.3/neophaser/assets/
--rw-rw-rw-   0 root         (0) root         (0)    67646 2023-04-26 03:16:00.000000 neophaser-0.1.3/neophaser/assets/icon.ico
--rw-rw-rw-   0 root         (0) root         (0)   208914 2023-04-26 03:16:00.000000 neophaser-0.1.3/neophaser/assets/icon.png
--rw-rw-rw-   0 root         (0) root         (0)     2127 2023-04-26 03:16:00.000000 neophaser-0.1.3/neophaser/board.py
--rw-rw-rw-   0 root         (0) root         (0)     3654 2023-04-26 03:16:00.000000 neophaser-0.1.3/neophaser/controllers.py
--rw-rw-rw-   0 root         (0) root         (0)    10896 2023-04-26 03:16:00.000000 neophaser-0.1.3/neophaser/gui.py
--rw-rw-rw-   0 root         (0) root         (0)      984 2023-04-26 03:16:00.000000 neophaser-0.1.3/neophaser/options.py
--rw-rw-rw-   0 root         (0) root         (0)     1187 2023-04-26 03:16:00.000000 neophaser-0.1.3/neophaser/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2634 2023-04-26 03:16:00.000000 neophaser-0.1.3/neophaser/visual.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:16:11.070574 neophaser-0.1.3/neophaser.egg-info/
--rw-r--r--   0 root         (0) root         (0)      889 2023-04-26 03:16:11.000000 neophaser-0.1.3/neophaser.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      417 2023-04-26 03:16:11.000000 neophaser-0.1.3/neophaser.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 03:16:11.000000 neophaser-0.1.3/neophaser.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-04-26 03:16:11.000000 neophaser-0.1.3/neophaser.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-26 03:16:11.000000 neophaser-0.1.3/neophaser.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      713 2023-04-26 03:16:00.000000 neophaser-0.1.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 03:16:11.072574 neophaser-0.1.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 01:37:42.780707 neophaser-0.1.4/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-12 01:37:32.000000 neophaser-0.1.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      889 2023-05-12 01:37:42.780707 neophaser-0.1.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-05-12 01:37:32.000000 neophaser-0.1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 01:37:42.776707 neophaser-0.1.4/neophaser/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-12 01:37:32.000000 neophaser-0.1.4/neophaser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      365 2023-05-12 01:37:32.000000 neophaser-0.1.4/neophaser/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 01:37:42.779707 neophaser-0.1.4/neophaser/assets/
+-rw-rw-rw-   0 root         (0) root         (0)    67646 2023-05-12 01:37:32.000000 neophaser-0.1.4/neophaser/assets/icon.ico
+-rw-rw-rw-   0 root         (0) root         (0)   208914 2023-05-12 01:37:32.000000 neophaser-0.1.4/neophaser/assets/icon.png
+-rw-rw-rw-   0 root         (0) root         (0)     2127 2023-05-12 01:37:32.000000 neophaser-0.1.4/neophaser/board.py
+-rw-rw-rw-   0 root         (0) root         (0)     3654 2023-05-12 01:37:32.000000 neophaser-0.1.4/neophaser/controllers.py
+-rw-rw-rw-   0 root         (0) root         (0)    13886 2023-05-12 01:37:32.000000 neophaser-0.1.4/neophaser/gui.py
+-rw-rw-rw-   0 root         (0) root         (0)      984 2023-05-12 01:37:32.000000 neophaser-0.1.4/neophaser/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1187 2023-05-12 01:37:32.000000 neophaser-0.1.4/neophaser/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2683 2023-05-12 01:37:32.000000 neophaser-0.1.4/neophaser/visual.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 01:37:42.778707 neophaser-0.1.4/neophaser.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      889 2023-05-12 01:37:42.000000 neophaser-0.1.4/neophaser.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      417 2023-05-12 01:37:42.000000 neophaser-0.1.4/neophaser.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 01:37:42.000000 neophaser-0.1.4/neophaser.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-05-12 01:37:42.000000 neophaser-0.1.4/neophaser.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-12 01:37:42.000000 neophaser-0.1.4/neophaser.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      713 2023-05-12 01:37:32.000000 neophaser-0.1.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 01:37:42.780707 neophaser-0.1.4/setup.cfg
```

### Comparing `neophaser-0.1.3/PKG-INFO` & `neophaser-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neophaser
-Version: 0.1.3
+Version: 0.1.4
 Summary: NEOPHASER; or, audio effects as applied to the retina - an application for applying audio effects to image and video.
 Author-email: 8o-COLLECTIVE <ops@8oc.org>
 Project-URL: homepage, https://neophaser.library.8oc.org
 Project-URL: repository, https://gitlab.com/8o-collective/neophaser
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `neophaser-0.1.3/neophaser/assets/icon.ico` & `neophaser-0.1.4/neophaser/assets/icon.ico`

 * *Files identical despite different names*

### Comparing `neophaser-0.1.3/neophaser/assets/icon.png` & `neophaser-0.1.4/neophaser/assets/icon.png`

 * *Files identical despite different names*

### Comparing `neophaser-0.1.3/neophaser/board.py` & `neophaser-0.1.4/neophaser/board.py`

 * *Files identical despite different names*

### Comparing `neophaser-0.1.3/neophaser/controllers.py` & `neophaser-0.1.4/neophaser/controllers.py`

 * *Files identical despite different names*

### Comparing `neophaser-0.1.3/neophaser/gui.py` & `neophaser-0.1.4/neophaser/gui.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os
+
 import cv2
 
 import numpy as np
 
 from PyQt6.QtCore import Qt, QMimeData, QByteArray, QDataStream, QIODevice, QUrl, QThread, QMutex, QMutexLocker, QSize, pyqtSignal
 from PyQt6.QtWidgets import QApplication, QMainWindow, QWidget, QPushButton, QLabel, QGridLayout, QListWidget, QListWidgetItem, QComboBox, QHBoxLayout, QVBoxLayout, QFormLayout, QCheckBox, QSlider, QGroupBox, QSplitter, QFileDialog, QMessageBox
 from PyQt6.QtMultimedia import QMediaPlayer
@@ -30,17 +32,60 @@
 			self.frame_ready.emit(self.visual.preview[self.frame])
 			QThread.msleep(30)
 	
 	def stop(self):
 		with QMutexLocker(self.mutex):
 			self._running = False
 
+class PaginatorWidget(QWidget):
+	# Define a custom signal that will emit the new page number
+	changed = pyqtSignal(int)
+
+	def __init__(self, parent=None):
+		super().__init__(parent)
+
+		# Initialize page counter to 1
+		self.page_number = 1
+		self.maximum = 0
+
+		# Create layout
+		self.layout = QHBoxLayout(self)
+
+		# Create and add widgets
+		self.left_button = QPushButton('<')
+		self.page_label = QLabel(f"{self.page_number}/{self.maximum}")
+		self.right_button = QPushButton('>')
+
+		self.layout.addWidget(self.left_button)
+		self.layout.addWidget(self.page_label)
+		self.layout.addWidget(self.right_button)
+
+		# Connect signals
+		self.left_button.clicked.connect(self.decrement_page)
+		self.right_button.clicked.connect(self.increment_page)
+	
+	def set_maximum(self, maximum):
+		self.maximum = maximum
+		self.page_label.setText(f"{self.page_number}/{self.maximum}")
+
+	def increment_page(self):
+		if self.page_number < self.maximum:
+			self.page_number += 1
+			self.page_label.setText(f"{self.page_number}/{self.maximum}")
+			self.changed.emit(self.page_number)
+
+	def decrement_page(self):
+		if self.page_number > 1:
+			self.page_number -= 1
+			self.page_label.setText(f"{self.page_number}/{self.maximum}")
+			self.changed.emit(self.page_number)
 
 class MediaLoader(QWidget):
 	loaded = pyqtSignal()
+	changed_visual = pyqtSignal(Visual)
 
 	def __init__(self, parent=None):
 		super().__init__(parent)
 		self.init_ui()
 
 	def init_ui(self):
 		layout = QVBoxLayout()
@@ -49,14 +94,19 @@
 		controls_layout = QHBoxLayout()
 		layout.addLayout(controls_layout)
 
 		open_file_button = QPushButton("Open")
 		open_file_button.clicked.connect(self.open_file)
 		controls_layout.addWidget(open_file_button)
 
+		self.pagination_widget = PaginatorWidget()
+		self.pagination_widget.changed.connect(self.set_active_visual)
+		controls_layout.addWidget(self.pagination_widget)
+		self.pagination_widget.hide()
+
 		self.save_file_button = QPushButton("Save")
 		controls_layout.addWidget(self.save_file_button)
 		self.save_file_button.hide()
 
 		self.media_display = QLabel(self)
 		layout.addWidget(self.media_display)
 
@@ -78,40 +128,58 @@
 	def dropEvent(self, event):
 		for url in event.mimeData().urls():
 			file_path = url.toLocalFile()
 			self.load_media(file_path)
 			break  # Only load the first file
 
 	def open_file(self):
-		file_path, _ = QFileDialog.getOpenFileName(self, "Open Media File", "", "Images (*.png *.jpg *.jpeg);;Videos (*.gif *.mp4 *.avi)")
+		file_paths, _ = QFileDialog.getOpenFileNames(self, "Open Media File", "", "Images (*.png *.jpg *.jpeg);;Videos (*.gif *.mp4 *.avi)")
 
-		if file_path:
-			self.load_media(file_path)
+		if file_paths:
+			self.load_media(file_paths)
 
-	def load_media(self, file_path):
-		if not Visual.check_valid_file(file_path):
-			return QMessageBox.critical(
-				self,
-				"Invalid File",
-				"The file is not a valid image or video format.",
-				buttons=QMessageBox.StandardButton.Ok,
-				defaultButton=QMessageBox.StandardButton.Ok,
-			)
+	def load_media(self, file_paths):
+		for file_path in file_paths:
+			if not Visual.check_valid_file(file_path):
+				return QMessageBox.critical(
+					self,
+					"Invalid File",
+					f"{file_path} is not a valid image or video format.",
+					buttons=QMessageBox.StandardButton.Ok,
+					defaultButton=QMessageBox.StandardButton.Ok,
+				)
+		
+		if len(file_paths) == 1:
+			file_path = file_paths[0]
 
-		self.media_player.setSource(QUrl.fromLocalFile(file_path))
+			self.media_player.setSource(QUrl.fromLocalFile(file_path))
 
-		self.visual = Visual(file_path)
-		self.data = self.visual.preview
+			self.visual = Visual(file_path)
+			self.data = self.visual.preview
+		else:
+			self.visuals = [Visual(file_path) for file_path in file_paths]
+			self.file_paths = file_paths
+			self.active_visual = 0
+			self.visual = self.visuals[0]
+			self.data = self.visual.preview
+			self.pagination_widget.set_maximum(len(self.visuals))
+			self.pagination_widget.show()
 
 		self.loaded.emit()
 
 		self.save_file_button.show()
 
 		self.set_data(self.visual)
 	
+	def set_active_visual(self, page_number):
+		self.active_visual = page_number - 1
+		self.visual = self.visuals[self.active_visual]
+		self.set_data(self.visual)
+		self.changed_visual.emit(self.visual)
+	
 	def set_data(self, visual):
 		self.visual = visual
 		self.data = self.visual.preview
 
 		if visual.type == DataType.IMAGE:
 			self.update_frame(self.data)
 		elif self.visual.type == DataType.VIDEO:
@@ -316,51 +384,74 @@
 	def __init__(self):
 		super().__init__()
 
 		self.setWindowTitle("neophaser")
 
 		self.layout = QGridLayout()
 
-		# button = QPushButton("Quit")
-		# button.pressed.connect(self.close)
-		# layout.addWidget(button, 0, 0)
-
 		self.media_player = MediaLoader()
 		self.media_player.loaded.connect(self.load_board)
+		self.media_player.changed_visual.connect(self.change_visual)
 		self.media_player.save_file_button.clicked.connect(self.render_and_save)
 		self.layout.addWidget(self.media_player, 0, 0)
 
 		widget = QWidget()
 		widget.setLayout(self.layout)
 		self.setCentralWidget(widget)
 		self.show()
 	
+	def change_visual(self, visual):
+		self.visual = self.media_player.visual
+		self.data = self.visual.original_preview.copy()
+
+		self.process_visual()
+	
 	def load_board(self):
 		self.visual = self.media_player.visual
-		self.data = self.visual.preview
+		self.data = self.visual.preview.copy()
 
 		self.board = ControllerBoard(self.visual)
 		board_manager = BoardWidget(self.board)
 
 		board_manager.render.connect(self.process_visual)
 
 		self.layout.addWidget(board_manager, 0, 1)
 	
 	def process_visual(self):
 		self.visual.preview = self.board.process(self.data, sample_rate_multiplier=self.visual.sample_rate_multiplier)
 		self.media_player.set_data(self.visual)
 	
 	def render_and_save(self):
-		file_path, _ = QFileDialog.getSaveFileName(parent=self, caption='Save File', directory='', filter="Images (*.png *.jpg *.jpeg);;Animated (*.gif);;All files (*)")
+		if hasattr(self.media_player, "visuals"):
+			directory_path = QFileDialog.getExistingDirectory(parent=self, caption='Save Files', directory='')
+
+			if directory_path:
+				for visual, file_path in zip(self.media_player.visuals, self.media_player.file_paths):
+					rendered = self.board.process(visual.original)
+
+					filename = os.path.basename(file_path)
+					save_path = os.path.join(directory_path, filename)
+
+					if visual.type == DataType.IMAGE:
+						cv2.imwrite(save_path, rendered)
+					elif visual.type == DataType.VIDEO:
+						fps = 30
+						_, height, width, _ = rendered.shape
+						out = cv2.VideoWriter(save_path, cv2.VideoWriter_fourcc('M','J','P','G'), fps, (width, height))
+						for frame in rendered:
+							out.write(frame)
+						out.release()
+		else:
+			file_path, _ = QFileDialog.getSaveFileName(parent=self, caption='Save File', directory='', filter="Images (*.png *.jpg *.jpeg);;Animated (*.gif);;All files (*)")
 
-		rendered = self.board.process(self.visual.original)
+			rendered = self.board.process(self.visual.original)
 
-		if file_path:
-			if self.visual.type == DataType.IMAGE:
-				cv2.imwrite(file_path, rendered)
-			elif self.visual.type == DataType.VIDEO:
-				fps = 30
-				_, height, width, _ = rendered.shape
-				out = cv2.VideoWriter(file_path, cv2.VideoWriter_fourcc('M','J','P','G'), fps, (width, height))
-				for frame in rendered:
-					out.write(frame)
-				out.release()
+			if file_path:
+				if self.visual.type == DataType.IMAGE:
+					cv2.imwrite(file_path, rendered)
+				elif self.visual.type == DataType.VIDEO:
+					fps = 30
+					_, height, width, _ = rendered.shape
+					out = cv2.VideoWriter(file_path, cv2.VideoWriter_fourcc('M','J','P','G'), fps, (width, height))
+					for frame in rendered:
+						out.write(frame)
+					out.release()
```

### Comparing `neophaser-0.1.3/neophaser/options.py` & `neophaser-0.1.4/neophaser/options.py`

 * *Files identical despite different names*

### Comparing `neophaser-0.1.3/neophaser/utils.py` & `neophaser-0.1.4/neophaser/utils.py`

 * *Files identical despite different names*

### Comparing `neophaser-0.1.3/neophaser/visual.py` & `neophaser-0.1.4/neophaser/visual.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 			self.original = self._read_video()
 			self.preview = self._resize_video(self.original.copy())
 		elif self.type == DataType.IMAGE:
 			self.original = self._read_image()
 			self.preview = self._resize_image(self.original.copy())
 		else:
 			raise ValueError("The file is neither an image nor a video.")
+		
+		self.original_preview = self.preview.copy()
 
 		self.sample_rate_multiplier = self.preview.size / self.original.size
 
 		self.effects = []
 	
 	@staticmethod
 	def check_valid_file(path):
```

### Comparing `neophaser-0.1.3/neophaser.egg-info/PKG-INFO` & `neophaser-0.1.4/neophaser.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neophaser
-Version: 0.1.3
+Version: 0.1.4
 Summary: NEOPHASER; or, audio effects as applied to the retina - an application for applying audio effects to image and video.
 Author-email: 8o-COLLECTIVE <ops@8oc.org>
 Project-URL: homepage, https://neophaser.library.8oc.org
 Project-URL: repository, https://gitlab.com/8o-collective/neophaser
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `neophaser-0.1.3/pyproject.toml` & `neophaser-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "neophaser"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="8o-COLLECTIVE", email="ops@8oc.org" },
 ]
 description = "NEOPHASER; or, audio effects as applied to the retina - an application for applying audio effects to image and video."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

