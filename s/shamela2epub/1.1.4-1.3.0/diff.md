# Comparing `tmp/shamela2epub-1.1.4.tar.gz` & `tmp/shamela2epub-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shamela2epub-1.1.4.tar", max compression
+gzip compressed data, was "shamela2epub-1.3.0.tar", max compression
```

## Comparing `shamela2epub-1.1.4.tar` & `shamela2epub-1.3.0.tar`

### file list

```diff
@@ -1,30 +1,29 @@
--rw-r--r--   0        0        0    35149 2022-07-09 23:30:01.570497 shamela2epub-1.1.4/LICENSE
--rw-r--r--   0        0        0     4177 2022-08-10 16:37:20.585434 shamela2epub-1.1.4/README.md
--rw-r--r--   0        0        0     1634 2022-12-06 11:46:44.155827 shamela2epub-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1419 2022-07-16 20:59:28.445135 shamela2epub-1.1.4/shamela2epub/__init__.py
--rw-r--r--   0        0        0      308 2022-07-19 12:23:43.292052 shamela2epub-1.1.4/shamela2epub/__main__.py
--rw-r--r--   0        0        0   132340 2022-07-12 09:01:57.456000 shamela2epub-1.1.4/shamela2epub/assets/NotoNaskhArabic-Regular.ttf
--rw-r--r--   0        0        0     2642 2022-07-11 21:45:18.273814 shamela2epub-1.1.4/shamela2epub/assets/books-duotone-128.png
--rw-r--r--   0        0        0    12405 2022-07-11 21:44:58.343656 shamela2epub-1.1.4/shamela2epub/assets/books-duotone-512.png
--rw-r--r--   0        0        0     9212 2022-07-16 12:17:14.319639 shamela2epub-1.1.4/shamela2epub/assets/books-duotone.ico
--rw-r--r--   0        0        0     1622 2022-07-11 21:40:01.487963 shamela2epub-1.1.4/shamela2epub/assets/books-duotone.svg
--rw-r--r--   0        0        0      715 2022-07-11 21:45:26.597214 shamela2epub-1.1.4/shamela2epub/assets/download-duotone-64.png
--rw-r--r--   0        0        0      752 2022-07-11 21:40:31.408201 shamela2epub-1.1.4/shamela2epub/assets/download-duotone.svg
--rw-r--r--   0        0        0      296 2022-08-09 16:51:53.801245 shamela2epub-1.1.4/shamela2epub/assets/styles.css
--rw-r--r--   0        0        0        0 2022-07-12 10:44:40.993865 shamela2epub-1.1.4/shamela2epub/cli/__init__.py
--rw-r--r--   0        0        0     1162 2022-07-16 20:59:28.445135 shamela2epub-1.1.4/shamela2epub/cli/app.py
--rw-r--r--   0        0        0        1 2022-07-12 11:06:24.986433 shamela2epub-1.1.4/shamela2epub/gui/__init__.py
--rw-r--r--   0        0        0     6081 2022-08-10 16:47:55.006270 shamela2epub-1.1.4/shamela2epub/gui/app.py
--rw-r--r--   0        0        0     3366 2022-07-15 20:49:22.620403 shamela2epub-1.1.4/shamela2epub/gui/ui.ui
--rw-r--r--   0        0        0     2326 2022-08-08 16:30:08.297495 shamela2epub-1.1.4/shamela2epub/main.py
--rw-r--r--   0        0        0        0 2022-07-09 23:30:06.020458 shamela2epub-1.1.4/shamela2epub/misc/__init__.py
--rw-r--r--   0        0        0       53 2022-07-15 20:49:22.700404 shamela2epub-1.1.4/shamela2epub/misc/constants.py
--rw-r--r--   0        0        0      949 2022-12-06 11:39:27.964539 shamela2epub-1.1.4/shamela2epub/misc/patterns.py
--rw-r--r--   0        0        0     1344 2022-08-08 16:30:12.344086 shamela2epub-1.1.4/shamela2epub/misc/utils.py
--rw-r--r--   0        0        0        0 2022-07-09 23:30:06.020458 shamela2epub-1.1.4/shamela2epub/models/__init__.py
--rw-r--r--   0        0        0      397 2022-12-06 11:43:25.916859 shamela2epub-1.1.4/shamela2epub/models/book_base_html_page.py
--rw-r--r--   0        0        0    10624 2022-12-06 11:45:47.729467 shamela2epub-1.1.4/shamela2epub/models/book_html_page.py
--rw-r--r--   0        0        0      890 2022-12-06 11:42:23.397153 shamela2epub-1.1.4/shamela2epub/models/book_info_html_page.py
--rw-r--r--   0        0        0     6710 2022-08-09 09:39:44.461040 shamela2epub-1.1.4/shamela2epub/models/epub_book.py
--rw-r--r--   0        0        0     5535 1970-01-01 00:00:00.000000 shamela2epub-1.1.4/setup.py
--rw-r--r--   0        0        0     5259 1970-01-01 00:00:00.000000 shamela2epub-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-07-09 23:30:01.570497 shamela2epub-1.3.0/LICENSE
+-rw-r--r--   0        0        0     4177 2022-08-10 16:37:20.585434 shamela2epub-1.3.0/README.md
+-rw-r--r--   0        0        0     2210 2023-06-17 11:40:51.296651 shamela2epub-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1421 2023-05-29 12:26:02.759708 shamela2epub-1.3.0/shamela2epub/__init__.py
+-rw-r--r--   0        0        0      360 2023-06-17 11:18:18.736301 shamela2epub-1.3.0/shamela2epub/__main__.py
+-rw-r--r--   0        0        0   132340 2022-07-12 09:01:57.456000 shamela2epub-1.3.0/shamela2epub/assets/NotoNaskhArabic-Regular.ttf
+-rw-r--r--   0        0        0     2642 2022-07-11 21:45:18.273814 shamela2epub-1.3.0/shamela2epub/assets/books-duotone-128.png
+-rw-r--r--   0        0        0    12405 2022-07-11 21:44:58.343656 shamela2epub-1.3.0/shamela2epub/assets/books-duotone-512.png
+-rw-r--r--   0        0        0     9212 2022-07-16 12:17:14.319639 shamela2epub-1.3.0/shamela2epub/assets/books-duotone.ico
+-rw-r--r--   0        0        0     1622 2022-07-11 21:40:01.487963 shamela2epub-1.3.0/shamela2epub/assets/books-duotone.svg
+-rw-r--r--   0        0        0      715 2022-07-11 21:45:26.597214 shamela2epub-1.3.0/shamela2epub/assets/download-duotone-64.png
+-rw-r--r--   0        0        0      752 2022-07-11 21:40:31.408201 shamela2epub-1.3.0/shamela2epub/assets/download-duotone.svg
+-rw-r--r--   0        0        0      296 2022-08-09 16:51:53.801245 shamela2epub-1.3.0/shamela2epub/assets/styles.css
+-rw-r--r--   0        0        0        0 2022-07-12 10:44:40.993865 shamela2epub-1.3.0/shamela2epub/cli/__init__.py
+-rw-r--r--   0        0        0     1138 2023-06-17 11:40:51.296651 shamela2epub-1.3.0/shamela2epub/cli/app.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:01:12.937795 shamela2epub-1.3.0/shamela2epub/gui/__init__.py
+-rw-r--r--   0        0        0     6724 2023-06-17 11:40:51.296651 shamela2epub-1.3.0/shamela2epub/gui/app.py
+-rw-r--r--   0        0        0     3366 2022-07-15 20:49:22.620403 shamela2epub-1.3.0/shamela2epub/gui/ui.ui
+-rw-r--r--   0        0        0     2948 2023-06-17 11:40:51.296651 shamela2epub-1.3.0/shamela2epub/main.py
+-rw-r--r--   0        0        0        0 2022-07-09 23:30:06.020458 shamela2epub-1.3.0/shamela2epub/misc/__init__.py
+-rw-r--r--   0        0        0       53 2022-07-15 20:49:22.700404 shamela2epub-1.3.0/shamela2epub/misc/constants.py
+-rw-r--r--   0        0        0     1146 2023-05-29 12:01:12.951128 shamela2epub-1.3.0/shamela2epub/misc/patterns.py
+-rw-r--r--   0        0        0     1374 2023-05-29 12:01:12.954462 shamela2epub-1.3.0/shamela2epub/misc/utils.py
+-rw-r--r--   0        0        0        0 2022-07-09 23:30:06.020458 shamela2epub-1.3.0/shamela2epub/models/__init__.py
+-rw-r--r--   0        0        0      450 2023-06-17 11:40:51.296651 shamela2epub-1.3.0/shamela2epub/models/book_base_html_page.py
+-rw-r--r--   0        0        0    10952 2023-06-17 11:40:51.296651 shamela2epub-1.3.0/shamela2epub/models/book_html_page.py
+-rw-r--r--   0        0        0     1019 2023-05-29 12:01:12.957795 shamela2epub-1.3.0/shamela2epub/models/book_info_html_page.py
+-rw-r--r--   0        0        0     6924 2023-06-17 11:40:51.299984 shamela2epub-1.3.0/shamela2epub/models/epub_book.py
+-rw-r--r--   0        0        0     5162 1970-01-01 00:00:00.000000 shamela2epub-1.3.0/PKG-INFO
```

### Comparing `shamela2epub-1.1.4/LICENSE` & `shamela2epub-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shamela2epub-1.1.4/README.md` & `shamela2epub-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `shamela2epub-1.1.4/pyproject.toml` & `shamela2epub-1.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 [tool.poetry]
 name = "shamela2epub"
-version = "1.1.4"
+version = "1.3.0"
 description = "A CLI and GUI tool to download a book on https://shamela.ws to an EPUB book."
 authors = ["yshalsager <ysh-alsager@hotmail.com>"]
 license = "GPL-3.0-only"
 repository = "https://github.com/yshalsager/shamela2epub/"
 keywords = ["epub3", "shamela", "book", "epub", "islamic"]
 packages = [
     { include = "shamela2epub" }
 ]
 include = [
     "README.md",
     "pyproject.toml"
 ]
 readme = "README.md"
 
-[tool.poetry.dependencies]
-python = ">=3.8,<3.11"
-httpx = "^0.23.0"
-beautifulsoup4 = "^4.11.1"
+[tool.poetry.group.main.dependencies]
+python = ">=3.11,<3.12"
+httpx = ">=0.23,<0.25"
 EbookLib = ">=0.17.1,<0.19.0"
+lxml = "^4.9.2"
 click = "^8.1.3"
-PyQt5 = {version = "^5.15.7", extras = ["gui"]}
-toml = "^0.10.2"
-typing-extensions = "^4.3.0"
-pyqtdarktheme = "^1.1.0"
-
-[tool.poetry.dev-dependencies]
-black = "^22.10.0"
-pre-commit = "^2.20.0"
-isort = "^5.10.1"
-mypy = "^0.991"
-flake8 = "^5.0.4"
+parsel = "^1.8.1"
+tomli = "^2.0.1"
+trogon = "^0.4.0"
+gevent = "^22.10.2"
+tqdm = "^4.65.0"
+
+[tool.poetry.group.gui.dependencies]
+PyQt5 = {version = "^5.15.7"}
+pyqtdarktheme = ">=1.1,<3.0"
+
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+pre-commit = "^3.3.2"
+ruff = "^0.0.272"
+mypy = "^1.3"
 types-toml = "^0.10.8"
 types-click = "^7.1.8"
-pyinstaller = "^5.6"
-pycln = "^2.1.2"
+pyinstaller = "^5.11"
 
 [tool.poetry.scripts]
 shamela2epub = "shamela2epub.__main__:main"
 shamela2epubgui = "shamela2epub.gui.app:gui"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
@@ -69,7 +72,17 @@
 show_error_codes = true
 warn_unused_ignores = true
 disallow_incomplete_defs = true
 disallow_untyped_decorators = true
 
 [tool.pycln]
 all = true
+
+[tool.ruff]  # https://github.com/charliermarsh/ruff
+fix = true
+ignore-init-module-imports = true
+line-length = 100
+select = ["A", "B", "BLE", "C4", "C90", "DTZ", "E", "ERA", "F", "G", "I", "INP", "ISC", "N", "NPY", "PGH", "PIE", "PLC", "PLE", "PLR", "PLW", "PT", "PTH", "PYI", "RET", "RSE", "RUF", "S", "SIM", "T10", "T20", "TID", "UP", "W", "YTT"]
+ignore = ["E501", "PGH001", "RET504", "S101", "D211", "D213", "ERA001", "G004"]
+unfixable = ["ERA001", "F401", "F841", "T201", "T203"]
+src = ["shamela2epub"]
+target-version = "py311"
```

### Comparing `shamela2epub-1.1.4/shamela2epub/__init__.py` & `shamela2epub-1.3.0/shamela2epub/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """Module initialization"""
 import logging
 from importlib import metadata
 from logging.handlers import TimedRotatingFileHandler
 from pathlib import Path
 from sys import stderr, stdout
 
-import toml
+import tomli
 
 # Use __file__ so PyInstaller bundle can access files too
 PKG_DIR = Path(__file__).absolute().parent
 PARENT_DIR = PKG_DIR.parent
 
 # Set package version dynamically
 try:
     # In production use package metadata
     __version__ = metadata.version(__package__)
 except metadata.PackageNotFoundError:
     # otherwise, read version from pyproject
 
-    __version__ = toml.loads((PARENT_DIR / "pyproject.toml").read_text())["tool"][
+    __version__ = tomli.loads((PARENT_DIR / "pyproject.toml").read_text())["tool"][
         "poetry"
     ]["version"]
 
 
 OUT_DIR = PARENT_DIR / "out"
 OUT_DIR.mkdir(parents=True, exist_ok=True)
 # Logging
```

### Comparing `shamela2epub-1.1.4/shamela2epub/assets/NotoNaskhArabic-Regular.ttf` & `shamela2epub-1.3.0/shamela2epub/assets/NotoNaskhArabic-Regular.ttf`

 * *Files identical despite different names*

### Comparing `shamela2epub-1.1.4/shamela2epub/assets/books-duotone-128.png` & `shamela2epub-1.3.0/shamela2epub/assets/books-duotone-128.png`

 * *Files identical despite different names*

### Comparing `shamela2epub-1.1.4/shamela2epub/assets/books-duotone-512.png` & `shamela2epub-1.3.0/shamela2epub/assets/books-duotone-512.png`

 * *Files identical despite different names*

### Comparing `shamela2epub-1.1.4/shamela2epub/assets/books-duotone.ico` & `shamela2epub-1.3.0/shamela2epub/assets/books-duotone.ico`

 * *Files identical despite different names*

### Comparing `shamela2epub-1.1.4/shamela2epub/assets/books-duotone.svg` & `shamela2epub-1.3.0/shamela2epub/assets/books-duotone.svg`

 * *Files identical despite different names*

### Comparing `shamela2epub-1.1.4/shamela2epub/assets/download-duotone-64.png` & `shamela2epub-1.3.0/shamela2epub/assets/download-duotone-64.png`

 * *Files identical despite different names*

### Comparing `shamela2epub-1.1.4/shamela2epub/assets/download-duotone.svg` & `shamela2epub-1.3.0/shamela2epub/assets/download-duotone.svg`

 * *Files identical despite different names*

### Comparing `shamela2epub-1.1.4/shamela2epub/cli/app.py` & `shamela2epub-1.3.0/shamela2epub/cli/app.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 logger = logging.getLogger(__name__)
 
 
 @click.command()
 @click.argument("url", type=str)
 @click.option("-o", "--output", type=str, help="ePub output book custom name")
-def download(url: str, output: str) -> None:
+@click.option(
+    "-x", "--connections", type=int, default=10, help="Max number of connections"
+)
+def download(url: str, output: str, connections: int) -> None:
     """Download Shamela book form URL to ePub."""
-    downloader = BookDownloader(url)
+    downloader = BookDownloader(url, connections)
     if not downloader.valid:
-        print("The URL you entered is invalid! Exiting...")
+        logger.error("The URL you entered is invalid! Exiting...")
         return
     logger.info(f"Got valid URL: {url}")
     downloader.create_info_page()
     logger.info(
         f"Working on book {downloader.book_info_page.title} by {downloader.book_info_page.author}"
     )
-    first_page_url = downloader.create_first_page()
-    logger.info(f"Getting page {first_page_url}.")
-    for page in downloader.download():
-        logger.info(f"Getting page {page}.")
+    downloader.download()
     # Save new book
     logger.info("Saving the new book")
     output_book = downloader.save_book(output)
     logger.info(f"Done! You can find the book at: {output_book}")
 
 
 if __name__ == "__main__":
```

### Comparing `shamela2epub-1.1.4/shamela2epub/gui/app.py` & `shamela2epub-1.3.0/shamela2epub/gui/app.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,94 @@
 from functools import partial
 from pathlib import Path
-from typing import Optional
+from typing import cast
 
 import click
 import qdarktheme
+from gevent import Greenlet, joinall, spawn
 from PyQt5 import uic
-from PyQt5.QtCore import QObject, QThread, pyqtSignal
+from PyQt5.QtCore import QObject, QRunnable, QThreadPool, pyqtSignal
 from PyQt5.QtGui import QFontDatabase
 from PyQt5.QtWidgets import (
     QApplication,
     QDesktopWidget,
     QFileDialog,
     QLabel,
     QMainWindow,
     QMessageBox,
     QPushButton,
 )
 
 from shamela2epub import PKG_DIR
 from shamela2epub.main import BookDownloader
 from shamela2epub.misc.utils import browse_file_directory
+from shamela2epub.models.book_html_page import BookHTMLPage
 
 
-class Worker(QObject):
+class QBookDownloader(BookDownloader):
+    def __init__(self, url: str) -> None:
+        super().__init__(url, connections=10)
+        self.progress: pyqtSignal = pyqtSignal(str)
+
+    def download_page(self, page_number: int) -> BookHTMLPage:
+        with self._sem:
+            book_html_page = BookHTMLPage(f"{self.url}/{page_number}")
+            self.progress.emit(
+                f"تحميل الصفحة {page_number} من {self.epub_book.pages_count}"
+            )
+        return book_html_page
+
+    def download(self) -> None:
+        self.progress.emit(f"تحميل الصفحة 1 من {self.epub_book.pages_count}")
+        self.create_first_page()
+        jobs = [
+            spawn(self.download_page, page_number)
+            for page_number in range(2, self.epub_book.pages_count + 1)
+        ]
+        job: Greenlet
+        for job in joinall(jobs):
+            self.epub_book.add_page(job.value)
+
+
+class WorkerSignals(QObject):
     finished = pyqtSignal()
     progress = pyqtSignal(str)
     downloaded = pyqtSignal(Path)
 
-    def __init__(self, downloader: BookDownloader, output: str) -> None:
-        self.downloader: BookDownloader = downloader
-        self.output: str = output
+
+class Worker(QRunnable):
+    def __init__(self, downloader: QBookDownloader, output: str) -> None:
         super().__init__()
+        self.downloader: QBookDownloader = downloader
+        self.output: str = output
+        self.signals = WorkerSignals()
 
     def run(self) -> None:
         """Process the book."""
+        self.downloader.progress = self.signals.progress
         self.downloader.create_info_page()
-        self.progress.emit(
+        self.signals.progress.emit(
             f"بدء العمل على كتاب {self.downloader.book_info_page.title} لمؤلفه {self.downloader.book_info_page.author}"
         )
-        self.downloader.create_first_page()
-        self.progress.emit("إنشاء الصفحة الأولى")
-        for page in self.downloader.download():
-            self.progress.emit(f"إنشاء الصفحة {page}")
-        self.progress.emit("حفظ الكتاب")
+        self.downloader.download()
+        self.signals.progress.emit("حفظ الكتاب")
         output_book = self.downloader.save_book(self.output)
-        self.downloaded.emit(output_book)
-        self.finished.emit()
+        self.signals.downloaded.emit(output_book)
+        self.signals.finished.emit()
 
 
 class App(QMainWindow):
     download: QPushButton
     statusbar: QLabel
     url_form: QLabel
 
     def __init__(self) -> None:
         """GUI App constructor."""
         super().__init__()
-        self.thread: QThread = QThread()  # type:ignore
-        self.worker: Optional[Worker] = None
+        self.thread_pool: QThreadPool = QThreadPool()
 
         uic.loadUi(f"{PKG_DIR}/gui/ui.ui", self)
         # self.setWindowIcon(QIcon(f"{WORK_DIR}/assets/books-duotone-512.png"))
         self.center()
         self.download.clicked.connect(self.run)
         self.statusbar.setText("جاهز")
 
@@ -96,54 +123,51 @@
         """Opens select file Dialog."""
         output_directory = QFileDialog().getExistingDirectory(
             self, "اختر مكان حفظ الكتاب"
         )
         if not output_directory:
             self.show_error_message("لم تختر مكانا لحفظ الكتاب!")
             return ""
-        return output_directory
+        return cast(str, output_directory)
 
     def report_progress(self, progress: str) -> None:
         self.update_statusbar(progress)
 
+    def on_finish(self) -> None:
+        self.download.setEnabled(True)
+        self.url_form.setEnabled(True)
+        self.url_form.setText("")
+        self.update_statusbar("اكتمل التحميل!")
+
     def run(self) -> None:
         self.download.setDisabled(True)
         self.url_form.setDisabled(True)
         if not self.url_form.text():
             self.show_error_message("لم تدخل رابط الكتاب بعد!")
             self.download.setEnabled(True)
+            self.url_form.setDisabled(False)
             return
-        downloader = BookDownloader(self.url_form.text())
+        downloader = QBookDownloader(self.url_form.text())
         if not downloader.valid:
             self.show_error_message("رابط غير صحيح!")
             self.download.setEnabled(True)
             return
         output = self.choose_output_directory()
         if not output:
             self.download.setEnabled(True)
             return
         self.update_statusbar("تحليل معلومات الرابط")
-        # Create a worker object
-        self.worker = Worker(downloader, output)
-        # Move worker to the thread
-        self.worker.moveToThread(self.thread)
+        # Create a qrunner and start it in a thread
+        worker = Worker(downloader, output)
+        self.thread_pool.start(worker)
         # Connect signals and slots
-        self.thread.started.connect(self.worker.run)
-        self.worker.finished.connect(self.thread.quit)
-        self.worker.finished.connect(self.worker.deleteLater)
-        self.thread.finished.connect(self.thread.deleteLater)
-        self.worker.progress.connect(self.report_progress)
-        self.worker.downloaded.connect(self.on_process_complete)
-        # Start the thread
-        self.thread.start()
+        worker.signals.progress.connect(self.report_progress)
+        worker.signals.downloaded.connect(self.on_process_complete)
         # Final resets
-        self.thread.finished.connect(lambda: self.download.setEnabled(True))
-        self.thread.finished.connect(lambda: self.url_form.setEnabled(True))
-        self.thread.finished.connect(lambda: self.url_form.setText(""))
-        self.thread.finished.connect(lambda: self.update_statusbar("اكتمل التحميل!"))
+        worker.signals.finished.connect(self.on_finish)
 
     def center(self) -> None:
         """Dynamically center the window in screen."""
         # https://gist.github.com/saleph/163d73e0933044d0e2c4
         # geometry of the main window
         window = self.frameGeometry()
         # center point of screen
```

### Comparing `shamela2epub-1.1.4/shamela2epub/gui/ui.ui` & `shamela2epub-1.3.0/shamela2epub/gui/ui.ui`

 * *Files identical despite different names*

### Comparing `shamela2epub-1.1.4/shamela2epub/main.py` & `shamela2epub-1.3.0/shamela2epub/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,83 @@
 """shamela2epub main."""
 from pathlib import Path
-from typing import Iterator
+
+from gevent import Greenlet, joinall, spawn
+from gevent.lock import BoundedSemaphore
+from gevent.monkey import patch_all
+from tqdm import tqdm
 
 from shamela2epub import OUT_DIR
 from shamela2epub.misc.utils import (
     get_book_first_page_url,
     get_book_info_page_url,
     is_valid_url,
 )
 from shamela2epub.models.book_html_page import BookHTMLPage
 from shamela2epub.models.book_info_html_page import BookInfoHTMLPage
 from shamela2epub.models.epub_book import EPUBBook
 
+patch_all(thread=False)
+
 
 class BookDownloader:
     book_info_page: BookInfoHTMLPage
-    book_html_page: BookHTMLPage
 
-    def __init__(self, url: str) -> None:
+    def __init__(self, url: str, connections: int) -> None:
         """Book Downloader constructor."""
         self.url = url
         self.valid = is_valid_url(self.url)
         self.epub_book = EPUBBook()
+        self._sem = BoundedSemaphore(connections)
+        self._progress_bar: tqdm | None = None
 
     def create_info_page(self) -> None:
         # Info Page
         self.book_info_page = BookInfoHTMLPage(get_book_info_page_url(self.url))
         self.epub_book.init()
         self.epub_book.create_info_page(self.book_info_page)
 
-    def create_first_page(self) -> str:
-        # First Page
-        first_page_url = get_book_first_page_url(self.url)
-        self.book_html_page = BookHTMLPage(first_page_url)
-        self.epub_book.set_page_count(self.book_html_page.last_page)
-        self.epub_book.set_parts_map(self.book_html_page.parts_map)
-        self.epub_book.add_page(self.book_html_page)
-        return first_page_url
-
-    def download(self) -> Iterator[str]:
-        has_next = self.book_html_page.has_next_page
-        next_page_url = self.book_html_page.next_page_url
-        while has_next:
-            yield next_page_url
-            self.book_html_page = BookHTMLPage(next_page_url)
-            self.epub_book.add_page(self.book_html_page)
-            if not self.book_html_page.has_next_page:
-                has_next = False
-            next_page_url = self.book_html_page.next_page_url
+    def create_first_page(self) -> None:
+        book_html_page = BookHTMLPage(get_book_first_page_url(self.url))
+        self.epub_book.set_page_count(book_html_page.last_page)
+        self.epub_book.set_parts_map(book_html_page.parts_map)
+        self.epub_book.set_toc(book_html_page.toc)
+        self.epub_book.add_page(book_html_page)
+        if self._progress_bar is not None:
+            self._progress_bar.total = self.epub_book.pages_count
+            self._progress_bar.update(1)
+
+    def download_page(self, page_number: int) -> BookHTMLPage:
+        with self._sem:
+            book_html_page = BookHTMLPage(f"{self.url}/{page_number}")
+            if self._progress_bar is not None:
+                self._progress_bar.update(1)
+        return book_html_page
+
+    def download(self) -> None:
+        self._progress_bar = tqdm(
+            desc="Downloading", colour="white", unit=" page", dynamic_ncols=True
+        )
+        self.create_first_page()
+        jobs = [
+            spawn(self.download_page, page_number)
+            for page_number in range(2, self.epub_book.pages_count + 1)
+        ]
+        job: Greenlet
+        for job in joinall(jobs):
+            self.epub_book.add_page(job.value)
 
     def save_book(self, output: str) -> Path:
         # Generate TOC
-        self.epub_book.generate_toc(self.book_html_page.toc)
+        self.epub_book.generate_toc()
         # Save to disk
         book_name = f"{self.book_info_page.title} - {self.book_info_page.author}.epub"
         if output:
             output_book = (
                 output if output.endswith(".epub") else f"{output}/{book_name}"
             )
         else:
             output_book = f"{OUT_DIR}/{book_name}"
         self.epub_book.save_book(output_book)
+        if self._progress_bar is not None:
+            self._progress_bar.close()
         return Path(output_book)
```

### Comparing `shamela2epub-1.1.4/shamela2epub/misc/patterns.py` & `shamela2epub-1.3.0/shamela2epub/misc/patterns.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import re
-from typing import Pattern
+from re import Pattern
 
 from shamela2epub.misc.constants import SHAMELA_DOMAIN
 
 BOOK_URL_PATTERN: Pattern = re.compile(
     r"(?:https?://)?{}/book/(?P<bookID>\d+)/?(?P<page>\d+)?#?(?P<paragraph>p\d+)?".format(
         SHAMELA_DOMAIN
     )
@@ -26,7 +26,12 @@
 # POSSIBLE_HAMESH_NUMBER_HTML_PATTERN: Pattern = re.compile(
 #     r"(<span style=\"color:#008000\">(?P<other>.+?)?(?P<number>\([\u0660-\u0669]+\))</span>)"
 # )
 
 ARABIC_NUMBER_BETWEEN_CURLY_BRACES_PATTERN: Pattern = re.compile(
     r"{.+?(\([\u0660-\u0669]+\)).+?}"
 )
+
+
+# HTML_CLASS_PATTERN = re.compile(r' class="(.*?)"')  # r' class="[\w\d -]+"'
+HTML_STYLE_PATTERN = re.compile(r' style="(.*?)"')
+PARENT_DIV_CLASS_PATTERN = re.compile(r' class="nass margin-top-10"')
```

### Comparing `shamela2epub-1.1.4/shamela2epub/misc/utils.py` & `shamela2epub-1.3.0/shamela2epub/misc/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 from pathlib import Path
 from platform import system
 from re import Match
 from subprocess import Popen
-from typing import Dict, Optional
 
 from shamela2epub import PKG_DIR
 from shamela2epub.misc.constants import BOOK_RESOURCE, SHAMELA_DOMAIN
 from shamela2epub.misc.patterns import BOOK_URL_PATTERN
 
 
 def is_valid_url(url: str) -> bool:
     return bool(BOOK_URL_PATTERN.search(url))
 
 
-def get_info_from_url(url: str) -> Dict[str, str]:
-    match: Optional[Match[str]] = BOOK_URL_PATTERN.search(url)
+def get_info_from_url(url: str) -> dict[str, str]:
+    match: Match[str] | None = BOOK_URL_PATTERN.search(url)
     assert match is not None
     return match.groupdict()
 
 
 def get_book_first_page_url(url: str) -> str:
-    info: Dict[str, str] = get_info_from_url(url)
+    info: dict[str, str] = get_info_from_url(url)
     return f"https://{SHAMELA_DOMAIN}/{BOOK_RESOURCE}/{info['bookID']}/1"
 
 
 def get_book_info_page_url(url: str) -> str:
-    info: Dict[str, str] = get_info_from_url(url)
+    info: dict[str, str] = get_info_from_url(url)
     return f"https://{SHAMELA_DOMAIN}/{BOOK_RESOURCE}/{info['bookID']}/"
 
 
 def get_stylesheet() -> str:
     return Path(PKG_DIR / "assets/styles.css").read_text()
 
 
 def browse_file_directory(filepath: Path) -> None:
     """Browse a file parent directory in OS file explorer."""
     if system() == "Windows":
-        from os import startfile  # type: ignore
+        from os import startfile  # type: ignore[attr-defined]
 
-        startfile(filepath.parent)
+        startfile(filepath.parent)  # noqa: 606
     elif system() == "Darwin":
-        Popen(["open", filepath.parent])
+        Popen(["open", filepath.parent])  # noqa: S603, S607
     else:
-        Popen(["xdg-open", filepath.parent])
+        Popen(["xdg-open", filepath.parent])  # noqa: S603, S607
```

### Comparing `shamela2epub-1.1.4/shamela2epub/models/book_html_page.py` & `shamela2epub-1.3.0/shamela2epub/models/book_html_page.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,268 +1,275 @@
-from typing import Any, Dict, List
+from re import Match
+from typing import Any, cast
 
-from bs4 import BeautifulSoup, Tag
+from lxml.etree import Element, QName, XMLParser, tostring
+from parsel import Selector, SelectorList
 
 from shamela2epub.misc.constants import BOOK_RESOURCE
 from shamela2epub.misc.patterns import (
     ARABIC_NUMBER_BETWEEN_BRACKETS_PATTERN,
     ARABIC_NUMBER_BETWEEN_CURLY_BRACES_PATTERN,
     BOOK_URL_PATTERN,
     HAMESH_CONTINUATION_PATTERN,
     HAMESH_PATTERN,
+    HTML_STYLE_PATTERN,
+    PARENT_DIV_CLASS_PATTERN,
 )
 from shamela2epub.models.book_base_html_page import BookBaseHTMLPage
 
+xml_parser = XMLParser(resolve_entities=False)
+epub_type = QName("http://www.idpf.org/2007/ops", "type")
+
 
 class BookHTMLPage(BookBaseHTMLPage):
-    BOOK_TOC_SELECTOR = "div.s-nav-head + ul"
+    BOOK_TOC_SELECTOR = "div.s-nav-head + ul > li"
     COPY_BTN_SELECTOR = "a.btn_tag"
     PAGE_NUMBER_SELECTOR = "input#fld_goto_bottom"
     PAGE_PARTS_SELECTOR = "#fld_part_top ~ div"
     PAGE_PARTS_MENU_SELECTOR = f"{PAGE_PARTS_SELECTOR} ul[role='menu']"
-    PAGE_PART_SELECTOR = f"{PAGE_PARTS_SELECTOR} button"
+    PAGE_PART_SELECTOR = f"{PAGE_PARTS_SELECTOR} button::text"
     NEXT_PAGE_SELECTOR = f"{PAGE_NUMBER_SELECTOR} + a"
     LAST_PAGE_SELECTOR = f"{PAGE_NUMBER_SELECTOR} + a + a"
     CHAPTERS_SELECTOR = f"div.s-nav-head ~ ul a[href*='/{BOOK_RESOURCE}/']"
-    _previous_page_hamesh = ""
+    _previous_page_hamesh: str = ""
 
     def __init__(self, url: str):
         """Book HTML page model constructor."""
         super().__init__(url)
         self._remove_copy_btn_from_html()
         self.page_url = self.url.split("#")[0]
-        self._chapters_by_page: Dict[str, str] = {}
-        self._toc_chapters_levels: Dict[str, int] = {}
-        self.content: Tag = self.get_clean_page_content()
-        self.hamesh_items: Dict[str, Tag] = self.get_hamesh_items()
+        self._chapters_by_page: dict[str, str] = {}
+        self._toc_chapters_levels: dict[str, int] = {}
+        self.content: Selector | None = self.get_clean_page_content()
+        self.hamesh_items: dict[str, Element] = self.get_hamesh_items()
         self._update_hamesh()
 
     def _remove_copy_btn_from_html(self) -> None:
-        for btn in self._html.select(self.COPY_BTN_SELECTOR):
-            btn.decompose()
+        self._html.css(self.COPY_BTN_SELECTOR).drop()
 
     @property
     def current_page(self) -> Any:
-        return self._html.select_one(self.PAGE_NUMBER_SELECTOR).get("value", "")
+        return self._html.css(f"{self.PAGE_NUMBER_SELECTOR}::attr(value)").get("")
 
     @property
     def has_next_page(self) -> bool:
-        return bool(self._html.select_one(self.NEXT_PAGE_SELECTOR))
+        return bool(self._html.css(self.NEXT_PAGE_SELECTOR))
 
     @staticmethod
-    def _get_page_number(page_anchor: Tag) -> str:
-        match = BOOK_URL_PATTERN.search(page_anchor.get("href"))
+    def _get_page_number(page_anchor: SelectorList) -> str:
+        match: Match | None = BOOK_URL_PATTERN.search(
+            page_anchor.attrib.get("href", "")
+        )
         assert match is not None
         page = match.group("page")
         assert isinstance(page, str)
         return page
 
     @property
     def next_page(self) -> str:
-        next_page_element = self._html.select_one(self.NEXT_PAGE_SELECTOR)
-        if not next_page_element:
-            return ""
-        return self._get_page_number(next_page_element)
+        next_page_element: SelectorList = self._html.css(self.NEXT_PAGE_SELECTOR)
+        return self._get_page_number(next_page_element) if next_page_element else ""
 
     @property
-    def next_page_url(self) -> Any:
-        next_page_element = self._html.select_one(self.NEXT_PAGE_SELECTOR)
-        if not next_page_element:
-            return ""
-        return next_page_element.get("href", "")
+    def next_page_url(self) -> str:
+        next_page_element: SelectorList = self._html.css(self.NEXT_PAGE_SELECTOR)
+        return (
+            cast(str, next_page_element.attrib.get("href", ""))
+            if next_page_element
+            else ""
+        )
 
     @property
     def last_page(self) -> str:
-        last_page_element = self._html.select_one(self.LAST_PAGE_SELECTOR)
-        if not last_page_element:
-            return ""
-        return self._get_page_number(last_page_element)
-
-    def parse_toc(self, toc: Tag) -> List:
-        toc_list: List = []
-        item: Tag
-        for item in toc.children:
-            link = item.select_one("a")
-            ul_list = item.select_one("ul")
+        last_page_element: SelectorList = self._html.css(self.LAST_PAGE_SELECTOR)
+        return self._get_page_number(last_page_element) if last_page_element else ""
+
+    def parse_toc(self, toc: SelectorList) -> list:
+        toc_list: list = []
+        item: Selector
+        for item in toc:
+            link: str = item.css("a::text").get("")
+            ul_list: SelectorList = item.css("li ul")
             if ul_list:
-                toc_list.append([link.text, self.parse_toc(ul_list)])
+                toc_list.append([link, self.parse_toc(ul_list.css("ul li"))])
             else:
-                toc_list.append(link.text)
+                toc_list.append(link)
         return toc_list
 
     @property
-    def toc(self) -> List[Any]:
-        toc_ul: Tag = self._html.select_one(self.BOOK_TOC_SELECTOR)
-        for item in toc_ul.select('a[href="javascript:;"]'):
-            item.decompose()
+    def toc(self) -> list[Any]:
+        toc_ul: SelectorList = self._html.css(self.BOOK_TOC_SELECTOR)
+        toc_ul.css('a[href="javascript:;"]').drop()
         return self.parse_toc(toc_ul)
 
     @property
-    def chapters_by_page(self) -> Dict[str, Any]:
+    def chapters_by_page(self) -> dict[str, Any]:
         if self._chapters_by_page:
             return self.chapters_by_page
-        chapters_list = self._html.select(self.CHAPTERS_SELECTOR)
-        chapters: Dict = {}
+        chapters_list = self._html.css(self.CHAPTERS_SELECTOR)
+        chapters: dict = {}
         for chapter in chapters_list:
-            chapter_url = chapter.get("href")
+            chapter_url = chapter.attrib.get("href", "")
             if chapters.get(chapter_url):
-                chapters[chapter_url].append(chapter.text)
+                chapters[chapter_url].append(chapter.css("::text").get("").strip())
                 chapters.update({chapter_url: chapters[chapter_url]})
             else:
-                chapters.update({chapter_url: [chapter.text]})
+                chapters.update({chapter_url: [chapter.css("::text").get("").strip()]})
         self._chapters_by_page = chapters
         return self._chapters_by_page
 
     @property
-    def part(self) -> Any:
-        part_element: Tag = self._html.select_one(self.PAGE_PART_SELECTOR)
-        return part_element.text.strip() if part_element else ""
+    def part(self) -> str:
+        return cast(str, self._html.css(self.PAGE_PART_SELECTOR).get("").strip())
 
     @property
-    def parts_map(self) -> Dict[str, int]:
-        parts: Tag = self._html.select_one(self.PAGE_PARTS_MENU_SELECTOR)
+    def parts_map(self) -> dict[str, int]:
+        parts: SelectorList = self._html.css(self.PAGE_PARTS_MENU_SELECTOR)
         return (
-            {part.text: index for index, part in enumerate(parts.select("li a")[1:])}
+            {
+                part.get(""): index
+                for index, part in enumerate(parts.css("li a::text")[1:])
+            }
             if parts
             else {}
         )
 
-    def get_clean_page_content(self) -> Tag:
+    def get_clean_page_content(self) -> Selector | None:
         """Get cleaned-up page content."""
-        content = self.content
-        if not content:
-            return content
+        if not self.content:
+            return self.content
         # Delete parent div class
-        del content["class"]
+        self.content = Selector(
+            text=PARENT_DIV_CLASS_PATTERN.sub("", self.content.get())
+        )
         # Delete all elements classes
-        for element in filter(
-            lambda x: isinstance(x, Tag) and x.get("class", None),
-            content.recursiveChildGenerator(),
-        ):
-            if not any([c for c in element["class"] if c in ["text-center", "hamesh"]]):
-                del element["class"]
+        # for element in filter(
+        #     lambda x: isinstance(x, Tag) and x.get("class", None),
+        #     content.recursiveChildGenerator(),
+        # ):
+        #     if not any([c for c in element["class"] if c in ["text-center", "hamesh"]]):
+        #         del element["class"]
         # Delete empty spans
-        for element in content.select("span"):
-            if not element.text:
-                element.decompose()
+        for element in self.content.css("span"):
+            if not element.css("::text").get():
+                element.drop()
         # Delete paragraph style
-        for element in content.select('p[style="font-size: 15px"]'):
-            del element["style"]
-        return content
+        for _ in self.content.css('p[style="font-size: 15px"]'):
+            _ = Selector(text=HTML_STYLE_PATTERN.sub("", self.content.get()))
+        return self.content
 
-    def get_hamesh_items(self) -> Dict[str, Tag]:
-        hamesh_items: Dict[str, Tag] = {}
+    def get_hamesh_items(self) -> dict[str, Element]:
+        hamesh_items: dict[str, Element] = {}
         if not self.content:
             return hamesh_items
-        hamesh: Tag = self.content.select_one(".hamesh")
+        hamesh: SelectorList = self.content.css(".hamesh")
         if not hamesh:
             return hamesh_items
         hamesh_counter = 0
         current_hamesh = ""
         hamesh_continuation = HAMESH_CONTINUATION_PATTERN.search(str(hamesh))
         if hamesh_continuation:
             type(self)._previous_page_hamesh = (
                 hamesh_continuation.group("continuation")
                 if not type(self)._previous_page_hamesh
                 else f"{type(self)._previous_page_hamesh}\n{hamesh_continuation.group('continuation')}"
             )
-        else:
-            if not type(self)._previous_page_hamesh:
-                type(self)._previous_page_hamesh = ""
-        for match in HAMESH_PATTERN.finditer(str(hamesh)):
+        elif not type(self)._previous_page_hamesh:
+            type(self)._previous_page_hamesh = ""
+        for match in HAMESH_PATTERN.finditer(hamesh.get("")):
             hamesh_counter += 1
             current_hamesh = match.group("number").strip()
             hamesh_line = match.group("content").strip()
             #  <aside id="fn1" epub:type="footnote">
             #  <p><a href="#fnref1" title="footnote 1">[1]</a> Text in popup</p>
             #  </aside>
-            new_footnote = Tag(
-                builder=hamesh.builder,
-                name="aside",
-                attrs={"id": f"fn{hamesh_counter}", "epub:type": "footnote"},
+            new_footnote_aside = Element(
+                "aside",
+                {"id": f"fn{hamesh_counter}", epub_type: "footnote"},
             )
-            new_footnote_p = Tag(builder=hamesh.builder, name="p")
-            new_footnote_a = Tag(
-                builder=hamesh.builder,
-                name="a",
-                attrs={
+            new_footnote_span = Element("span")
+            new_footnote_a = Element(
+                "a",
+                {
                     "href": f"#fnref{hamesh_counter}",
                     # "title": f"هامش {hamesh_counter}",
                     "class": "nu",
                 },
             )
-            new_footnote_a.string = current_hamesh
-            new_footnote.append(new_footnote_p)
+            new_footnote_a.text = current_hamesh
             if type(self)._previous_page_hamesh:
-                new_footnote_p.append(
-                    BeautifulSoup(
-                        type(self)._previous_page_hamesh.replace("\n", "<br>"),
-                        "html.parser",
-                    )
+                new_footnote_span.text = type(self)._previous_page_hamesh.replace(
+                    "\n", "<br>"
                 )
-                new_footnote_p.append(Tag(name="br"))
-                new_footnote_p.append(new_footnote_a)
-                new_footnote_p.append(" ")
-                new_footnote_p.append(BeautifulSoup(hamesh_line.strip(), "html.parser"))
+                new_footnote_span.append(Element("br"))
+                new_footnote_span.text = " " + hamesh_line.strip()
                 type(self)._previous_page_hamesh = ""
             else:
-                new_footnote_p.append(new_footnote_a)
-                new_footnote_p.append(" ")
-                new_footnote_p.append(BeautifulSoup(hamesh_line.strip(), "html.parser"))
-            hamesh_items.update({current_hamesh: new_footnote})
+                new_footnote_span.text = " " + hamesh_line.strip()
+            new_footnote_aside.append(new_footnote_a)
+            new_footnote_aside.append(new_footnote_span)
+            hamesh_items.update({current_hamesh: new_footnote_aside})
         return hamesh_items
 
     def _update_hamesh(self) -> None:
         footnote_count = 1
         if not self.content:
             return
-        hamesh: Tag = self.content.select_one(".hamesh")
+        hamesh: SelectorList = self.content.css(".hamesh")
         if not hamesh:
             return
-        new_hamesh = Tag(builder=hamesh.builder, name="div", attrs={"class": "hamesh"})
-        parent = self.content.select_one("div")
-        p_elements = self.content.select("p:not(.hamesh)")
+        new_hamesh: Element = Element("div", {"class": "hamesh"})
+        parent: SelectorList = self.content.css("div")
+        p_elements: SelectorList = self.content.css("p:not(.hamesh)")
         for p in p_elements:
-            matches = ARABIC_NUMBER_BETWEEN_BRACKETS_PATTERN.finditer(str(p))
+            matches = ARABIC_NUMBER_BETWEEN_BRACKETS_PATTERN.finditer(p.get())
             for match in matches:
                 number = match.group("number")
                 if not self.hamesh_items.get(number, ""):
                     continue
-                aya_match = ARABIC_NUMBER_BETWEEN_CURLY_BRACES_PATTERN.search(str(p))
+                aya_match = ARABIC_NUMBER_BETWEEN_CURLY_BRACES_PATTERN.search(p.get())
                 if (
                     aya_match
                     and number in aya_match.group()
                     # number in inside aya
                     and match.start("number") > aya_match.start()
                 ):
                     continue
-                footnote_link: Tag = Tag(
-                    builder=p.builder,
-                    name="a",
-                    attrs={
+                footnote_link: Element = Element(
+                    "a",
+                    {
                         "href": f"#fn{footnote_count}",
-                        "epub:type": "noteref",
+                        epub_type: "noteref",
                         "role": "doc-noteref",
                         "id": f"fnref{footnote_count}",
                         # "title": f"هامش {footnote_count}",
                         "class": "fn nu",
                     },
                 )
-                footnote_link.string = number
+                footnote_link.text = number
                 # new_p_content = (
                 #     str(p)[len("<p>") : match.start()]
                 #     + str(footnote_link)
                 #     + str(p)[match.start() + len(match.group()) : 0 - len("</p>")]
                 # )
                 # TODO: Find a better way to replace number with its a element,
                 #  since replacing only the first occurrence might not be the best solution
-                new_p_content = str(p).replace(number, str(footnote_link), 1)
-                new_p = Tag(builder=p.builder, name="p", parent=parent)
-                new_p.append(BeautifulSoup(new_p_content, "html.parser"))
-                p.replace_with(new_p)
-                p = new_p
+                new_p_el = p.get().replace(
+                    number, self.element_as_text(footnote_link), 1
+                )
+                self.content = Selector(text=parent.get("").replace(p.get(), new_p_el))
                 footnote_count += 1
                 new_hamesh.append(self.hamesh_items[number])
-        hamesh.replace_with(new_hamesh)
+        self.content = Selector(
+            text=self.content.get().replace(
+                hamesh.get(""), self.element_as_text(new_hamesh)
+            )
+        )
+
+    @staticmethod
+    def element_as_text(element: Element) -> str:
+        element_text: str = tostring(element, encoding="utf-8").decode()
+        assert isinstance(element_text, str)
+        return element_text
 
     def __repr__(self) -> str:
         return f"<BookHTMLPage(url={self.url})>"
```

### Comparing `shamela2epub-1.1.4/shamela2epub/models/book_info_html_page.py` & `shamela2epub-1.3.0/shamela2epub/models/book_info_html_page.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+from shamela2epub.misc.patterns import PARENT_DIV_CLASS_PATTERN
 from shamela2epub.models.book_base_html_page import BookBaseHTMLPage
 
 
 class BookInfoHTMLPage(BookBaseHTMLPage):
     SEARCH_SELECTOR = f"{BookBaseHTMLPage.BOOK_PAGE_CONTENT_SELECTOR} div.text-left"
     INDEX_SELECTOR = f"{BookBaseHTMLPage.BOOK_PAGE_CONTENT_SELECTOR} div.betaka-index"
-    BOOK_AUTHOR_SELECTOR = "h1 + div a"
-    BOOK_TITLE_SELECTOR = "h1 a"
+    BOOK_AUTHOR_SELECTOR = "h1 + div a::text"
+    BOOK_TITLE_SELECTOR = "h1 a::text"
 
     def __init__(self, url: str):
         """Book Info Page model constructor."""
         self.url = url
         super().__init__(url)
+        self.text_content: str = ""
         self._sanitize_html()
-        self.title = self._html.select_one(self.BOOK_TITLE_SELECTOR).text.strip()
-        self.author = self._html.select_one(self.BOOK_AUTHOR_SELECTOR).text.strip()
+        self.title = self._html.css(self.BOOK_TITLE_SELECTOR).get("").strip()
+        self.author = self._html.css(self.BOOK_AUTHOR_SELECTOR).get("").strip()
 
     def _sanitize_html(self) -> None:
-        self._html.select_one(self.INDEX_SELECTOR).decompose()
-        self._html.select_one(self.SEARCH_SELECTOR).decompose()
-        del self.content["class"]
+        self._html.css(self.INDEX_SELECTOR).drop()
+        self._html.css(self.SEARCH_SELECTOR).drop()
+        self.text_content = PARENT_DIV_CLASS_PATTERN.sub("", self.content.get(""))
```

### Comparing `shamela2epub-1.1.4/shamela2epub/models/epub_book.py` & `shamela2epub-1.3.0/shamela2epub/models/epub_book.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,55 @@
 import re
-from typing import Dict, List, Optional
+from typing import Any, cast
 
-from bs4 import Tag
 from ebooklib.epub import (
     EpubBook,
     EpubHtml,
     EpubItem,
     EpubNav,
     EpubNcx,
     Link,
     write_epub,
 )
+from parsel import Selector
 
 from shamela2epub import __version__
 from shamela2epub.misc.constants import SHAMELA_DOMAIN
 from shamela2epub.misc.patterns import CSS_STYLE_COLOR_PATTERN
 from shamela2epub.misc.utils import get_stylesheet
 from shamela2epub.models.book_html_page import BookHTMLPage
 from shamela2epub.models.book_info_html_page import BookInfoHTMLPage
 
 
 class EPUBBook:
     def __init__(self) -> None:
         """EPUB Book model."""
-        self._pages_count: str = ""
+        self.pages_count: int = 0
         self._zfill_length = 0
         self._book: EpubBook = EpubBook()
-        self._pages: List[EpubHtml] = []
-        self._sections: List[Link] = []
-        self._sections_map: Dict[str, Link] = {}
-        self._parts_map: Dict[str, int] = {}
+        self._pages: list[EpubHtml] = []
+        self._sections: list[Link] = []
+        self._sections_map: dict[str, Link] = {}
+        self._parts_map: dict[str, int] = {}
+        self._toc: list[str] = []
         self._default_css: EpubItem = EpubItem()
-        self._color_styles_map: Dict[str, int] = {}
+        self._color_styles_map: dict[str, int] = {}
         self._last_color_id: int = 0
-        self._pages_map: Dict[int, int] = {}
+        self._pages_map: dict[int, int] = {}
 
     def set_page_count(self, count: str) -> None:
-        self._pages_count = count
+        self.pages_count = int(count) if count else 0
         self._zfill_length = len(count) + 1
 
-    def set_parts_map(self, parts_map: Dict[str, int]) -> None:
+    def set_parts_map(self, parts_map: dict[str, int]) -> None:
         self._parts_map = parts_map
 
+    def set_toc(self, toc_list: list[Any]) -> None:
+        self._toc = toc_list
+
     def init(self) -> None:
         self._book.set_language("ar")
         self._book.set_direction("rtl")
         self._book.add_metadata("DC", "publisher", f"https://{SHAMELA_DOMAIN}")
         self._book.add_metadata(
             None, "meta", "", {"name": "shamela2epub", "content": __version__}
         )
@@ -61,54 +65,55 @@
         self._book.set_title(book_info_html_page.title)
         self._book.add_author(book_info_html_page.author)
         self._book.add_metadata("DC", "source", book_info_html_page.url)
         info_page = EpubHtml(
             title="بطاقة الكتاب",
             file_name="info.xhtml",
             lang="ar",
-            content=f"<html><body>{book_info_html_page.content}</body></html>",
+            content=f"<html><body>{book_info_html_page.text_content}</body></html>",
         )
         info_page.add_item(self._default_css)
         self._book.add_item(info_page)
         self._pages.append(info_page)
 
     def add_chapter(
-        self, chapters_in_page: Dict, new_page: EpubHtml, page_filename: str
+        self, chapters_in_page: dict, new_page: EpubHtml, page_filename: str
     ) -> None:
         for i in chapters_in_page:
             link = Link(
                 page_filename,
                 i,
                 page_filename.replace(".xhtml", ""),
             )
             self._sections.append(link)
             self._sections_map.update({i: link})
 
-    def replace_color_styles_with_class(self, html: Tag) -> str:
-        html_str = str(html)
+    def replace_color_styles_with_class(self, html: Selector | None) -> str:
+        if not html:
+            return ""
+        html_str = html.get()
         matches = CSS_STYLE_COLOR_PATTERN.findall(html_str)
         if not matches:
-            return html_str
+            return cast(str, html_str)
         for style in list(set(CSS_STYLE_COLOR_PATTERN.findall(html_str))):
             color_class = self._color_styles_map.get(style, "")
             if not color_class:
                 color_class = f"color-{self._last_color_id + 1}"
                 self._color_styles_map.update({style: color_class})
                 self._last_color_id += 1
                 self._default_css.content += f"\n.{color_class} {{ {style}; }}\n\n"
             html_str = re.sub(f'style="{style}"', f'class="{color_class}"', html_str)
-        return html_str
+        return cast(str, html_str)
 
     def get_book_page_number(self, book_html_page: BookHTMLPage) -> str:
         """
         Get the correct page number, which will be in page file name
         """
         html_page_number: int = int(book_html_page.current_page)
-        book_page_count: Optional[int] = self._pages_map.get(html_page_number)
-        current_page = None
+        book_page_count: int | None = self._pages_map.get(html_page_number)
         if book_page_count:
             new_page_count = book_page_count + 1
             current_page = new_page_count
             self._pages_map[html_page_number] = new_page_count
             return f"{str(html_page_number).zfill(self._zfill_length)}_{current_page}"
         current_page = html_page_number
         self._pages_map[html_page_number] = 1
@@ -140,24 +145,25 @@
         new_page.add_item(self._default_css)
         self._book.add_item(new_page)
         self._pages.append(new_page)
         if chapters_in_page:
             self.add_chapter(chapters_in_page, new_page, page_filename)
         return new_page
 
-    def _update_toc_list(self, toc: List) -> None:
+    def _update_toc_list(self, toc: list) -> None:
         # Bug: Books that have a last nested section with level deeper than its next with the same page number
         # cannot be converted to KFX unless that last nested section is removed.
         for index, element in enumerate(toc):
             if isinstance(element, list):
                 self._update_toc_list(element)
             else:
                 toc[index] = self._sections_map.get(element, None)
 
-    def generate_toc(self, toc_list: List) -> None:
+    def generate_toc(self) -> None:
+        toc_list: list[Link | str] = self._toc
         self._update_toc_list(toc_list)
         toc_list.insert(0, Link("nav.xhtml", "فهرس الموضوعات", "nav"))
         toc_list.insert(0, Link("info.xhtml", "بطاقة الكتاب", "info"))
         self._book.toc = toc_list
         self._book.add_item(EpubNcx())
         nav = EpubNav()
         nav.add_item(self._default_css)
```

### Comparing `shamela2epub-1.1.4/setup.py` & `shamela2epub-1.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,135 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: shamela2epub
+Version: 1.3.0
+Summary: A CLI and GUI tool to download a book on https://shamela.ws to an EPUB book.
+Home-page: https://github.com/yshalsager/shamela2epub/
+License: GPL-3.0-only
+Keywords: epub3,shamela,book,epub,islamic
+Author: yshalsager
+Author-email: ysh-alsager@hotmail.com
+Requires-Python: >=3.11,<3.12
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: EbookLib (>=0.17.1,<0.19.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: gevent (>=22.10.2,<23.0.0)
+Requires-Dist: httpx (>=0.23,<0.25)
+Requires-Dist: lxml (>=4.9.2,<5.0.0)
+Requires-Dist: parsel (>=1.8.1,<2.0.0)
+Requires-Dist: tomli (>=2.0.1,<3.0.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Requires-Dist: trogon (>=0.4.0,<0.5.0)
+Project-URL: Repository, https://github.com/yshalsager/shamela2epub/
+Description-Content-Type: text/markdown
 
-packages = \
-['shamela2epub',
- 'shamela2epub.cli',
- 'shamela2epub.gui',
- 'shamela2epub.misc',
- 'shamela2epub.models']
-
-package_data = \
-{'': ['*'], 'shamela2epub': ['assets/*']}
-
-install_requires = \
-['EbookLib>=0.17.1,<0.19.0',
- 'PyQt5[gui]>=5.15.7,<6.0.0',
- 'beautifulsoup4>=4.11.1,<5.0.0',
- 'click>=8.1.3,<9.0.0',
- 'httpx>=0.23.0,<0.24.0',
- 'pyqtdarktheme>=1.1.0,<2.0.0',
- 'toml>=0.10.2,<0.11.0',
- 'typing-extensions>=4.3.0,<5.0.0']
-
-entry_points = \
-{'console_scripts': ['shamela2epub = shamela2epub.__main__:main',
-                     'shamela2epubgui = shamela2epub.gui.app:gui']}
-
-setup_kwargs = {
-    'name': 'shamela2epub',
-    'version': '1.1.4',
-    'description': 'A CLI and GUI tool to download a book on https://shamela.ws to an EPUB book.',
-    'long_description': '# shamela2epub\n\n> A CLI and GUI tool to download a book on [Shamela Library Website](https://shamela.ws) into an EPUB book.\n\n[![en](https://img.shields.io/badge/README-English-AB8B64.svg)](README.md)\n[![ara](https://img.shields.io/badge/README-Arabic-AB8B64.svg)](README.ar.md)\n\n![logo](shamela2epub/assets/books-duotone.svg)\n\n[![Codacy Badge](https://app.codacy.com/project/badge/Grade/901b1123964c4468a88b0cfcde9147fe)](https://www.codacy.com/gh/yshalsager/shamela2epub/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=yshalsager/shamela2epub&amp;utm_campaign=Badge_Grade)\n[![PyPI version](https://badge.fury.io/py/shamela2epub.svg)](https://pypi.org/project/shamela2epub/)\n[![PyPI Downloads](https://static.pepy.tech/personalized-badge/shamela2epub?period=total\\&units=international_system\\&left_color=grey\\&right_color=blue\\&left_text=Total%20Downloads%20\\(PyPI\\))](https://pepy.tech/project/shamela2epub)\n\n[![GitHub release](https://img.shields.io/github/release/yshalsager/shamela2epub.svg)](https://github.com/yshalsager/shamela2epub/releases/)\n[![GitHub Downloads](https://img.shields.io/github/downloads/yshalsager/shamela2epub/total.svg)](https://github.com/yshalsager/shamela2epub/releases/latest)\n\n[![made-with-python](https://img.shields.io/badge/Made%20with-Python%203-3776AB?style=flat\\&labelColor=3776AB\\&logo=python\\&logoColor=white\\&link=https://www.python.org/)](https://www.python.org/)\n[![Open Source Love](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://github.com/ellerbrock/open-source-badges/)\n\n[![PayPal](https://img.shields.io/badge/PayPal-Donate-00457C?style=flat\\&labelColor=00457C\\&logo=PayPal\\&logoColor=white\\&link=https://www.paypal.me/yshalsager)](https://www.paypal.me/yshalsager)\n[![LiberaPay](https://img.shields.io/badge/Liberapay-Support-F6C915?style=flat\\&labelColor=F6C915\\&logo=Liberapay\\&logoColor=white\\&link=https://liberapay.com/yshalsager)](https://liberapay.com/yshalsager)\n\n**Disclaimer:**\n\n*   This software is freeware and open source and is only intended for personal or educational use.\n\n## Installation\n\n### From PyPI\n\n```bash\npip install shamela2epub\n```\n\n### From the cloned repository\n\n```bash\n# Using poetry\npoetry install\n\n# or using pip 18+\npip install .\n```\n\n## Usage\n\n### Command-line Tool (CLI)\n\n```bash\npython3 -m shamela2epub download URL\n# python3 -m shamela2epub download "https://shamela.ws/book/823"\n\npython3 -m shamela2epub download --help\nUsage: python -m shamela2epub download [OPTIONS] URL\n\n  Download Shamela book form URL to ePub\n\nOptions:\n  -o, --output TEXT  ePub output book custom name\n  --help             Show this message and exit.\n```\n\n### Graphical User Interface (GUI)\n\n![gui](gui.png)\n\n*   If you installed the package from PyPI, you can use the following command:\n\n```bash\nshamela2epubgui\n```\n\n*   If you downloaded the latest gui exe file from releases you can open it normally and use it.\n*   Otherwise, use normal python command:\n\n```bash\npython3 -m shamela2epub gui\n```\n\n## Features\n\n*   CLI and GUI!\n*   Creates an [EPUB3](https://www.w3.org/publishing/epub3/epub-spec.html) RTL standard book.\n*   Automatically adds a page for book information.\n*   Automatically generated table of contents with support for nested chapters.\n*   Automatically adds book part and page number to each page\'s footer.\n*   Sanitizes the book HTML from unnecessary elements and classes.\n*   Converts inline CSS color styles to CSS classes.\n*   Inline footnotes for easier navigation, click any footnote, and it will appear in a popup instead of having all footnotes in page footer.\n\n## Known Issues\n\n*   Books that have a last nested section with level deeper (e.g. 3) than its next section (e.g. 2) and both have the same\n    page number (e.g. `page_017.xhtml`) cannot be converted to KFX unless that last nested section is removed.\n\n## TODO\n\n### Next\n\n*   You tell me :)\n\n### Maybe\n\n*   Fix TOC conversion problem when last nested section with level deeper than its next has the same page number by\n    removing it from the TOC.\n\n## Acknowledgments\n\n*   GUI icons are made by the amazing [Phosphor Icons](https://phosphoricons.com/) (books - duotone - `#AB8B64`).\n',
-    'author': 'yshalsager',
-    'author_email': 'ysh-alsager@hotmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/yshalsager/shamela2epub/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<3.11',
-}
+# shamela2epub
 
+> A CLI and GUI tool to download a book on [Shamela Library Website](https://shamela.ws) into an EPUB book.
+
+[![en](https://img.shields.io/badge/README-English-AB8B64.svg)](README.md)
+[![ara](https://img.shields.io/badge/README-Arabic-AB8B64.svg)](README.ar.md)
+
+![logo](shamela2epub/assets/books-duotone.svg)
+
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/901b1123964c4468a88b0cfcde9147fe)](https://www.codacy.com/gh/yshalsager/shamela2epub/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=yshalsager/shamela2epub&amp;utm_campaign=Badge_Grade)
+[![PyPI version](https://badge.fury.io/py/shamela2epub.svg)](https://pypi.org/project/shamela2epub/)
+[![PyPI Downloads](https://static.pepy.tech/personalized-badge/shamela2epub?period=total\&units=international_system\&left_color=grey\&right_color=blue\&left_text=Total%20Downloads%20\(PyPI\))](https://pepy.tech/project/shamela2epub)
+
+[![GitHub release](https://img.shields.io/github/release/yshalsager/shamela2epub.svg)](https://github.com/yshalsager/shamela2epub/releases/)
+[![GitHub Downloads](https://img.shields.io/github/downloads/yshalsager/shamela2epub/total.svg)](https://github.com/yshalsager/shamela2epub/releases/latest)
+
+[![made-with-python](https://img.shields.io/badge/Made%20with-Python%203-3776AB?style=flat\&labelColor=3776AB\&logo=python\&logoColor=white\&link=https://www.python.org/)](https://www.python.org/)
+[![Open Source Love](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://github.com/ellerbrock/open-source-badges/)
+
+[![PayPal](https://img.shields.io/badge/PayPal-Donate-00457C?style=flat\&labelColor=00457C\&logo=PayPal\&logoColor=white\&link=https://www.paypal.me/yshalsager)](https://www.paypal.me/yshalsager)
+[![LiberaPay](https://img.shields.io/badge/Liberapay-Support-F6C915?style=flat\&labelColor=F6C915\&logo=Liberapay\&logoColor=white\&link=https://liberapay.com/yshalsager)](https://liberapay.com/yshalsager)
+
+**Disclaimer:**
+
+*   This software is freeware and open source and is only intended for personal or educational use.
+
+## Installation
+
+### From PyPI
+
+```bash
+pip install shamela2epub
+```
+
+### From the cloned repository
+
+```bash
+# Using poetry
+poetry install
+
+# or using pip 18+
+pip install .
+```
+
+## Usage
+
+### Command-line Tool (CLI)
+
+```bash
+python3 -m shamela2epub download URL
+# python3 -m shamela2epub download "https://shamela.ws/book/823"
+
+python3 -m shamela2epub download --help
+Usage: python -m shamela2epub download [OPTIONS] URL
+
+  Download Shamela book form URL to ePub
+
+Options:
+  -o, --output TEXT  ePub output book custom name
+  --help             Show this message and exit.
+```
+
+### Graphical User Interface (GUI)
+
+![gui](gui.png)
+
+*   If you installed the package from PyPI, you can use the following command:
+
+```bash
+shamela2epubgui
+```
+
+*   If you downloaded the latest gui exe file from releases you can open it normally and use it.
+*   Otherwise, use normal python command:
+
+```bash
+python3 -m shamela2epub gui
+```
+
+## Features
+
+*   CLI and GUI!
+*   Creates an [EPUB3](https://www.w3.org/publishing/epub3/epub-spec.html) RTL standard book.
+*   Automatically adds a page for book information.
+*   Automatically generated table of contents with support for nested chapters.
+*   Automatically adds book part and page number to each page's footer.
+*   Sanitizes the book HTML from unnecessary elements and classes.
+*   Converts inline CSS color styles to CSS classes.
+*   Inline footnotes for easier navigation, click any footnote, and it will appear in a popup instead of having all footnotes in page footer.
+
+## Known Issues
+
+*   Books that have a last nested section with level deeper (e.g. 3) than its next section (e.g. 2) and both have the same
+    page number (e.g. `page_017.xhtml`) cannot be converted to KFX unless that last nested section is removed.
+
+## TODO
+
+### Next
+
+*   You tell me :)
+
+### Maybe
+
+*   Fix TOC conversion problem when last nested section with level deeper than its next has the same page number by
+    removing it from the TOC.
+
+## Acknowledgments
+
+*   GUI icons are made by the amazing [Phosphor Icons](https://phosphoricons.com/) (books - duotone - `#AB8B64`).
 
-setup(**setup_kwargs)
```

