# Comparing `tmp/CustomTkinterTitlebar-1.0.7.8.tar.gz` & `tmp/CustomTkinterTitlebar-1.0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CustomTkinterTitlebar-1.0.7.8.tar", last modified: Mon May  1 12:48:50 2023, max compression
+gzip compressed data, was "CustomTkinterTitlebar-1.0.7.9.tar", last modified: Sat Jun 17 05:49:58 2023, max compression
```

## Comparing `CustomTkinterTitlebar-1.0.7.8.tar` & `CustomTkinterTitlebar-1.0.7.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 12:48:50.412053 CustomTkinterTitlebar-1.0.7.8/
-drwxrwxrwx   0        0        0        0 2023-05-01 12:48:50.213828 CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar/
--rw-rw-rw-   0        0        0       24 2023-04-30 10:02:33.000000 CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 12:48:50.237764 CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar/asset/
-drwxrwxrwx   0        0        0        0 2023-05-01 12:48:50.329304 CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar/asset/dark/
--rw-rw-rw-   0        0        0      297 2023-04-30 10:02:34.000000 CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar/asset/dark/close_100.png
--rw-rw-rw-   0        0        0      346 2023-04-30 10:02:34.000000 CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar/asset/dark/close_50.png
--rw-rw-rw-   0        0        0      142 2023-04-30 10:02:34.000000 CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar/asset/dark/fullwin_100.png
--rw-rw-rw-   0        0        0      146 2023-04-30 10:02:34.000000 CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar/asset/dark/fullwin_50.png
--rw-rw-rw-   0        0        0      120 2023-04-30 10:02:34.000000 CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar/asset/dark/minisize_100.png
--rw-rw-rw-   0        0        0      123 2023-04-30 10:02:34.000000 CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar/asset/dark/minisize_50.png
--rw-rw-rw-   0        0        0      163 2023-04-30 10:02:34.000000 CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar/asset/dark/togglefull_100.png
--rw-rw-rw-   0        0        0      167 2023-04-30 10:02:34.000000 CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar/asset/dark/togglefull_50.png
-drwxrwxrwx   0        0        0        0 2023-05-01 12:48:50.409088 CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar/asset/light/
--rw-rw-rw-   0        0        0      145 2023-04-30 10:02:34.000000 CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar/asset/light/close_100.png
--rw-rw-rw-   0        0        0      346 2023-04-30 10:02:34.000000 CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar/asset/light/close_50.png
--rw-rw-rw-   0        0        0      103 2023-04-30 10:02:34.000000 CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar/asset/light/fullwin_100.png
--rw-rw-rw-   0        0        0      105 2023-04-30 10:02:34.000000 CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar/asset/light/fullwin_50.png
--rw-rw-rw-   0        0        0       94 2023-04-30 10:02:34.000000 CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar/asset/light/minisize_100.png
--rw-rw-rw-   0        0        0      106 2023-04-30 10:02:34.000000 CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar/asset/light/minisize_50.png
--rw-rw-rw-   0        0        0      114 2023-04-30 10:02:34.000000 CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar/asset/light/togglefull_100.png
--rw-rw-rw-   0        0        0      115 2023-04-30 10:02:34.000000 CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar/asset/light/togglefull_50.png
--rw-rw-rw-   0        0        0    57022 2023-04-30 10:02:34.000000 CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar/asset/tk.ico
--rw-rw-rw-   0        0        0    80896 2023-04-30 10:14:18.000000 CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar/plugin32.dll
--rw-rw-rw-   0        0        0   104960 2023-04-30 10:11:34.000000 CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar/plugin64.dll
--rw-rw-rw-   0        0        0    12693 2023-04-30 10:41:55.000000 CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar/titlebar.py
-drwxrwxrwx   0        0        0        0 2023-05-01 12:48:50.222805 CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar.egg-info/
--rw-rw-rw-   0        0        0     4649 2023-05-01 12:48:50.000000 CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1227 2023-05-01 12:48:50.000000 CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 12:48:50.000000 CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-01 12:48:50.000000 CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-05-01 12:48:50.000000 CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1073 2023-04-30 10:02:33.000000 CustomTkinterTitlebar-1.0.7.8/LICENSE
--rw-rw-rw-   0        0        0       12 2023-05-01 12:44:02.000000 CustomTkinterTitlebar-1.0.7.8/MANIFEST.in
--rw-rw-rw-   0        0        0     4649 2023-05-01 12:48:50.411055 CustomTkinterTitlebar-1.0.7.8/PKG-INFO
--rw-rw-rw-   0        0        0     3584 2023-04-30 10:02:33.000000 CustomTkinterTitlebar-1.0.7.8/README.md
--rw-rw-rw-   0        0        0       42 2023-05-01 12:48:50.412053 CustomTkinterTitlebar-1.0.7.8/setup.cfg
--rw-rw-rw-   0        0        0     1287 2023-05-01 12:46:58.000000 CustomTkinterTitlebar-1.0.7.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 05:49:58.201945 CustomTkinterTitlebar-1.0.7.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 05:49:58.201945 CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-17 05:49:41.000000 CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 05:49:58.201945 CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar/asset/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 05:49:58.201945 CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar/asset/dark/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-17 05:49:41.000000 CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar/asset/dark/close_100.png
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-17 05:49:41.000000 CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar/asset/dark/close_50.png
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-17 05:49:41.000000 CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar/asset/dark/fullwin_100.png
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-17 05:49:41.000000 CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar/asset/dark/fullwin_50.png
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-17 05:49:41.000000 CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar/asset/dark/minisize_100.png
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-17 05:49:41.000000 CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar/asset/dark/minisize_50.png
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-17 05:49:41.000000 CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar/asset/dark/togglefull_100.png
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-17 05:49:41.000000 CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar/asset/dark/togglefull_50.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 05:49:58.201945 CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar/asset/light/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-17 05:49:41.000000 CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar/asset/light/close_100.png
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-17 05:49:41.000000 CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar/asset/light/close_50.png
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-17 05:49:41.000000 CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar/asset/light/fullwin_100.png
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 05:49:41.000000 CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar/asset/light/fullwin_50.png
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-17 05:49:41.000000 CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar/asset/light/minisize_100.png
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-17 05:49:41.000000 CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar/asset/light/minisize_50.png
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-17 05:49:41.000000 CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar/asset/light/togglefull_100.png
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-17 05:49:41.000000 CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar/asset/light/togglefull_50.png
+-rw-r--r--   0 runner    (1001) docker     (123)    57022 2023-06-17 05:49:41.000000 CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar/asset/tk.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    80896 2023-06-17 05:49:41.000000 CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar/plugin32.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   104960 2023-06-17 05:49:41.000000 CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar/plugin64.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    12668 2023-06-17 05:49:41.000000 CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar/titlebar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 05:49:58.201945 CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-06-17 05:49:58.000000 CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-17 05:49:58.000000 CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 05:49:58.000000 CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-17 05:49:58.000000 CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-17 05:49:58.000000 CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-17 05:49:41.000000 CustomTkinterTitlebar-1.0.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-17 05:49:41.000000 CustomTkinterTitlebar-1.0.7.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-06-17 05:49:58.201945 CustomTkinterTitlebar-1.0.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-06-17 05:49:41.000000 CustomTkinterTitlebar-1.0.7.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 05:49:58.201945 CustomTkinterTitlebar-1.0.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-17 05:49:41.000000 CustomTkinterTitlebar-1.0.7.9/setup.py
```

### Comparing `CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar/asset/tk.ico` & `CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar/asset/tk.ico`

 * *Files identical despite different names*

### Comparing `CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar/plugin32.dll` & `CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar/plugin32.dll`

 * *Files identical despite different names*

### Comparing `CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar/plugin64.dll` & `CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar/plugin64.dll`

 * *Files identical despite different names*

### Comparing `CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar/titlebar.py` & `CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar/titlebar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from tkinter import Tk, Button, Menu, Frame, Label, X, Y, TOP, RIGHT, LEFT, FLAT
-from BlurWindow.blurWindow import blur
 from ctypes import windll, c_char_p, c_int, byref, sizeof
 from PIL import Image, ImageTk
 from darkdetect import isDark
 from os import getcwd, system
 from pathlib import Path
 
+try:
+	from BlurWindow.blurWindow import blur
+except: # ignore it
+	pass
+
 env = Path(__file__).parent
 try:
 	plugin = windll.LoadLibrary(str(env / "plugin64.dll"))
-except OSError:
+except OSError: # 32 bit
 	plugin = windll.LoadLibrary(str(env / "plugin32.dll"))
 except FileNotFoundError:
 	system("pip install CustomTkinterTitlebar --force-reinstall")
 
 class CTT(Tk):
 	""" A class for custom titlebar """
 	def __init__(self, theme : str = "followsystem", unlimit: bool = False):
@@ -33,33 +37,36 @@
 				self.settheme("dark")
 			else:
 				path /= "light"
 				self.settheme("light")
 		else:
 			path /= theme
 			self.settheme(theme)
+
 		self.close_load = Image.open(path / "close_50.png")
 		self.close_hov_load = Image.open(path / "close_100.png")
-		self.close_img = ImageTk.PhotoImage(self.close_load)
-		self.close_hov_img = ImageTk.PhotoImage(self.close_hov_load)
 		self.min_load= Image.open(path / "minisize_50.png")
 		self.min_hov_load = Image.open(path / "minisize_100.png")
-		self.min_img = ImageTk.PhotoImage(self.min_load)
-		self.min_hov_img = ImageTk.PhotoImage(self.min_hov_load)
 		self.full_load = Image.open(path / "fullwin_50.png")
 		self.full_hov_load = Image.open(path / "fullwin_100.png")
-		self.full_img = ImageTk.PhotoImage(self.full_load)
-		self.full_hov_img = ImageTk.PhotoImage(self.full_hov_load)
 		self.max_load = Image.open(path / "togglefull_50.png")
 		self.max_hov_load = Image.open(path / "togglefull_100.png")
+		
+		self.close_img = ImageTk.PhotoImage(self.close_load)
+		self.close_hov_img = ImageTk.PhotoImage(self.close_hov_load)
+		self.min_img = ImageTk.PhotoImage(self.min_load)
+		self.min_hov_img = ImageTk.PhotoImage(self.min_hov_load)
+		self.full_img = ImageTk.PhotoImage(self.full_load)
+		self.full_hov_img = ImageTk.PhotoImage(self.full_hov_load)
 		self.max_img = ImageTk.PhotoImage(self.max_load)
 		self.max_hov_img = ImageTk.PhotoImage(self.max_hov_load)
 		
 		self.width, self.height = 265, 320
 		self.o_m = self.o_f = False
+		self.unlimit = unlimit
 		
 		self.popup = Menu(self, tearoff = 0)
 		self.popup.add_command(label = "Restore", command = self.resize)
 		self.popup.add_command(label = "Minsize", command = self.minsize)
 		self.popup.add_command(label = "Maxsize", command = self.maxsize)
 		self.popup.add_separator()
 		self.popup.add_command(label = "Close (Alt+F4)", command = self.destroy)
@@ -118,33 +125,37 @@
 		self._titletext.pack(fill = Y, side = LEFT, pady = 5)
 		self._titleexit.pack(fill = Y, side = RIGHT)
 		self._titlemax.pack(fill = Y, side = RIGHT)
 		self._titlemin.pack(fill = Y, side = RIGHT)
 		self.titlebar.pack(fill = X, side = TOP)
 		self.titlebar.pack_propagate(0)
 		self.setup()
-		
+
 	# Titlebar
 	def titlebarconfig(self, color = {"color": None, "color_nf": None}, height = 30):
 		""" Config for titlebar """
 		if color["color"] and color["color_nf"]: # Require two colors : focuson & focusout
 			self.bg = color["color"]
 			self.nf = color["color_nf"]
 			self["background"] = color["color"]
 		
-		if unlimit:
+		if self.unlimit:
 			self.titlebar["height"] = height
 		else:
-			if height > 30 and height <= 50: # Limit for titlebar height
+			if height > 30 and height <= 50:
 				self.titlebar["height"] = height
 
+		self.focusout()
+		self.focusin()
+		self.update()
+
 	# Titlename
 	def title(self, text):
 		""" Rebuild tkinter's title """
-		# TODO: find a good way to show ... if text is too long
+		# TODO: show "..." if title is too long
 		self._titletext["text"] = text
 		self.wm_title(text)
 
 	def title_grey(self):
 		""" ... """
 		self._titletext["foreground"] = "grey"
 
@@ -153,25 +164,24 @@
 		self._titletext["foreground"] = "white"
 
 	def usetitle(self, flag = True):
 		""" Show / forget titlename """
 		if not flag:
 			self._titletext.pack_forget()
 
-	def titlenameconfig(self, pack = "left", font = None):
-		""" Config the titlename """
+	def titleconfig(self, pack = "left", font = None):
+		""" Config the title """
 		self.usetitle(False)
 		if pack == "left":
 			self._titletext.pack(side = LEFT)
 		elif pack == "right":
 			self._titletext.pack(side = RIGHT)
 		else:
 			self._titletext.config(justify = "center")
 			self._titletext.pack(expand = True)
-			
 		if font:
 			self._titletext.config(font = font)
 
 	# Titleicon
 	def useicon(self, flag = True):
 		""" Show / forget icon """
 		if not flag:
@@ -258,45 +268,44 @@
 
 	def disabledo(self):
 		""" ... """
 		pass
 
 	def usemaxmin(self, minsize = True, maxsize = True, minshow = True, maxshow = True):
 		""" Show / Disable min / max button """
-		if not minshow: # packforget min button
+		if not minshow:
 			self._titlemin.pack_forget()
-		elif not minsize: # disable min button
+		elif not minsize:
 			self.min_grey(None)
 			self._titlemin["command"] = self.disabledo
 			self._titlemin.unbind("<Leave>")
 			self._titlemin.unbind("<Enter>")
 
-		if not maxshow: # packforget max button
+		if not maxshow:
 			self._titlemax.pack_forget()
-		elif not maxsize: # disable max button
+		elif not maxsize:
 			self.max_grey(None)
 			self._titlemax["command"] = self.disabledo
 			self._titlemax.unbind("<Leave>")
 			self._titlemax.unbind("<Enter>")
 
-	# Window
+	# Window functions
 	def setup(self):
 		""" Window Setup """
 		
 		self.title("CTT")
 		self.geometry("%sx%s" % (self.width, self.height))
 		self.iconbitmap(env / "asset" / "tk.ico")
 		
+		
 		self.hwnd = windll.user32.FindWindowW(c_char_p(None), "CTT")
 		plugin.setwindow(self.hwnd)
+		#self.overrideredirect(1)
 		
-		self.withdraw()
-		self.deiconify()
 		self.update()
-		
 		self.focus_force()
 
 	def moving(self, event):
 		""" Window moving """
 		global x, y
 		if not self.o_m:
 			plugin.move(self.hwnd, self.winfo_x(), self.winfo_y(), event.x - x, event.y - y) # Use C for speed
@@ -320,15 +329,15 @@
 			self.popup.entryconfig("Restore", state = "active")
 			self.popup.entryconfig("Maxsize", state = "disabled")
 			self.w_x, self.w_y = self.winfo_x(), self.winfo_y()
 			self.o_m = True
 			self._titlemax["image"] = self.max_hov_img
 			self._titlemax["command"] = self.resize
 			w, h = self.wm_maxsize()
-			self.geometry("%dx%d+0+0" % (w, h - 40))
+			self.geometry("%dx%d-1+0" % (w - 14, h - 40))
 
 	def resize(self):
 		""" Resize window """
 		self.popup.entryconfig("Restore", state = "disabled")
 		self.popup.entryconfig("Maxsize", state = "active")
 		self.wm_geometry("%dx%d+%d+%d" % (int(self.width), int(self.height), int(self.w_x), int(self.w_y)))
 		self._titlemax["command"] = self.maxsize
@@ -366,19 +375,19 @@
 		self.titlebar["bg"] = color
 		self._titletext["bg"] = color
 		self._titleicon["bg"] = color
 		self._titlemin["bg"] = color
 		self._titlemax["bg"] = color
 		self._titleexit["bg"] = color
 	
-	def focusout(self, event):
+	def focusout(self, event = None):
 		""" When focusout """
 		self.setcolor("out", self.nf)
 
-	def focusin(self, event):
+	def focusin(self, event = None):
 		""" When focusin """
 		self.setcolor("in", self.bg)
 		
 	def useblur(self, acrylic = True, dark = isDark()):
 		""" Add blur / acrylic effect to window """
 		if dark and self.theme != "light":
 			blur(hwnd = self.hwnd, hexColor = '#19191800', Dark = dark, Acrylic = acrylic)
@@ -414,11 +423,7 @@
 			self.update()
 		else:
 			self.theme = "light"
 			self.bg = self.colors["light"]
 			self.nf = self.colors["light_nf"]
 			self.fg = "dark"
 			self.update()
-
-
-a = CTT()
-a.mainloop()
```

### Comparing `CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar.egg-info/PKG-INFO` & `CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,291 +1,302 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310d 0a4e 616d 653a 2043 7573  : 2.1..Name: Cus
-00000020: 746f 6d54 6b69 6e74 6572 5469 746c 6562  tomTkinterTitleb
-00000030: 6172 0d0a 5665 7273 696f 6e3a 2031 2e30  ar..Version: 1.0
-00000040: 2e37 2e38 0d0a 5375 6d6d 6172 793a 2054  .7.8..Summary: T
-00000050: 6869 7320 6973 2061 2070 726f 6a65 6374  his is a project
-00000060: 2063 616e 2068 656c 7020 796f 7520 746f   can help you to
-00000070: 2068 6176 6520 6120 6375 7374 6f6d 2074   have a custom t
-00000080: 6974 6c65 6261 7221 0d0a 486f 6d65 2d70  itlebar!..Home-p
-00000090: 6167 653a 2068 7474 703a 2f2f 6769 7468  age: http://gith
-000000a0: 7562 2e63 6f6d 2f6c 6974 746c 6577 6869  ub.com/littlewhi
-000000b0: 7465 636c 6f75 642f 4375 7374 6f6d 546b  tecloud/CustomTk
-000000c0: 696e 7465 7254 6974 6c65 6261 720d 0a41  interTitlebar..A
-000000d0: 7574 686f 723a 206c 6974 746c 6577 6869  uthor: littlewhi
-000000e0: 7465 636c 6f75 640d 0a41 7574 686f 722d  tecloud..Author-
-000000f0: 656d 6169 6c3a 2071 3131 3431 3932 3636  email: q11419266
-00000100: 3437 4031 3633 2e63 6f6d 0d0a 4b65 7977  47@163.com..Keyw
-00000110: 6f72 6473 3a20 7079 7468 6f6e 2063 2077  ords: python c w
-00000120: 696e 646f 7773 2063 706c 7573 706c 7573  indows cplusplus
-00000130: 2064 6c6c 2063 7070 2063 7573 746f 6d20   dll cpp custom 
-00000140: 7069 6c6c 6f77 2062 6c75 7220 6374 7970  pillow blur ctyp
-00000150: 6573 2074 6b20 7469 746c 6562 6172 2074  es tk titlebar t
-00000160: 6b69 6e74 6572 2077 696e 646f 7720 7769  kinter window wi
-00000170: 6e64 6f77 7331 3020 646f 6320 6d73 7663  ndows10 doc msvc
-00000180: 2064 6574 6169 6c73 2075 7365 7233 3220   details user32 
-00000190: 6461 726b 6465 7465 6374 0d0a 436c 6173  darkdetect..Clas
-000001a0: 7369 6669 6572 3a20 4465 7665 6c6f 706d  sifier: Developm
-000001b0: 656e 7420 5374 6174 7573 203a 3a20 3520  ent Status :: 5 
-000001c0: 2d20 5072 6f64 7563 7469 6f6e 2f53 7461  - Production/Sta
-000001d0: 626c 650d 0a43 6c61 7373 6966 6965 723a  ble..Classifier:
-000001e0: 2049 6e74 656e 6465 6420 4175 6469 656e   Intended Audien
-000001f0: 6365 203a 3a20 4465 7665 6c6f 7065 7273  ce :: Developers
-00000200: 0d0a 436c 6173 7369 6669 6572 3a20 546f  ..Classifier: To
-00000210: 7069 6320 3a3a 2053 6f66 7477 6172 6520  pic :: Software 
-00000220: 4465 7665 6c6f 706d 656e 7420 3a3a 204c  Development :: L
-00000230: 6962 7261 7269 6573 203a 3a20 5079 7468  ibraries :: Pyth
-00000240: 6f6e 204d 6f64 756c 6573 0d0a 436c 6173  on Modules..Clas
-00000250: 7369 6669 6572 3a20 4c69 6365 6e73 6520  sifier: License 
-00000260: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
-00000270: 3a3a 204d 4954 204c 6963 656e 7365 0d0a  :: MIT License..
-00000280: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-00000290: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-000002a0: 203a 3a20 5079 7468 6f6e 203a 3a20 330d   :: Python :: 3.
-000002b0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-000002c0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000002d0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000002e0: 2e38 0d0a 436c 6173 7369 6669 6572 3a20  .8..Classifier: 
-000002f0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000300: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000310: 3a20 332e 390d 0a43 6c61 7373 6966 6965  : 3.9..Classifie
-00000320: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000330: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000340: 6e20 3a3a 2033 2e31 300d 0a43 6c61 7373  n :: 3.10..Class
-00000350: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00000360: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000370: 7974 686f 6e20 3a3a 2033 2e31 310d 0a52  ython :: 3.11..R
-00000380: 6571 7569 7265 732d 5079 7468 6f6e 3a20  equires-Python: 
-00000390: 3e3d 332e 380d 0a44 6573 6372 6970 7469  >=3.8..Descripti
-000003a0: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
-000003b0: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
-000003c0: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
-000003d0: 4345 4e53 450d 0a0d 0a3c 7020 616c 6967  CENSE....<p alig
-000003e0: 6e3d 2263 656e 7465 7222 3e0d 0a20 20f0  n="center">..  .
-000003f0: 9f8c 8f0d 0a20 203c 6120 6872 6566 3d22  .....  <a href="
-00000400: 5245 4144 4d45 5f43 482e 6d64 223e e7ae  README_CH.md">..
-00000410: 80e4 bd93 e4b8 ade6 9687 3c2f 613e 0d0a  ..........</a>..
-00000420: 3c2f 703e 0d0a 0d0a 2320 f09f 939c 205f  </p>....# .... _
-00000430: 4375 7374 6f6d 546b 696e 7465 7254 6974  CustomTkinterTit
-00000440: 6c65 6261 725f 0d0a 0d0a 215b 696d 6167  lebar_....![imag
-00000450: 655d 2868 7474 7073 3a2f 2f75 7365 722d  e](https://user-
-00000460: 696d 6167 6573 2e67 6974 6875 6275 7365  images.githubuse
-00000470: 7263 6f6e 7465 6e74 2e63 6f6d 2f37 3131  rcontent.com/711
-00000480: 3539 3634 312f 3230 3832 3331 3839 392d  59641/208231899-
-00000490: 6332 3566 6139 3530 2d35 3766 372d 3461  c25fa950-57f7-4a
-000004a0: 3930 2d38 3039 352d 6363 6561 6462 6636  90-8095-cceadbf6
-000004b0: 6433 3731 2e70 6e67 290d 0a23 2323 20f0  d371.png)..### .
-000004c0: 9f93 8320 2a54 6869 7320 6973 2061 2070  ... *This is a p
-000004d0: 726f 6a65 6374 2063 616e 2068 656c 7020  roject can help 
-000004e0: 796f 7520 746f 2068 6176 6520 6120 6375  you to have a cu
-000004f0: 7374 6f6d 2074 6974 6c65 6261 7221 2057  stom titlebar! W
-00000500: 6964 6765 7473 2063 616e 2061 6464 2069  idgets can add i
-00000510: 6e74 6f20 7469 746c 6562 6172 212a 0d0a  nto titlebar!*..
-00000520: 2323 2323 20e2 9d94 204d 6f72 6520 6162  #### ... More ab
-00000530: 6f75 7420 7468 6973 2070 726f 6a65 6374  out this project
-00000540: 2c20 4920 7772 6f74 6520 616e 2061 7274  , I wrote an art
-00000550: 6963 6c65 206f 6e20 4269 6c69 6269 6c69  icle on Bilibili
-00000560: 2c20 7768 6963 6820 7461 6c6b 7320 6162  , which talks ab
-00000570: 6f75 7420 7468 6973 2070 726f 6a65 6374  out this project
-00000580: 2069 6e20 6d6f 7265 2064 6574 6169 6c3a   in more detail:
-00000590: 205f 2068 7474 7073 3a2f 2f77 7777 2e62   _ https://www.b
-000005a0: 696c 6962 696c 692e 636f 6d2f 7265 6164  ilibili.com/read
-000005b0: 2f63 7632 3035 3538 3437 330d 0a23 2323  /cv20558473..###
-000005c0: 2320 2a48 6f70 6520 676f 7420 736f 6d65  # *Hope got some
-000005d0: 2073 7461 7273 7e2a 0d0a 0d0a 2323 2320   stars~*....### 
-000005e0: f09f 8eb0 2044 656d 6f3a 0d0a 6874 7470  .... Demo:..http
-000005f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6c  s://github.com/l
-00000600: 6974 746c 6577 6869 7465 636c 6f75 642f  ittlewhitecloud/
-00000610: 4375 7374 6f6d 546b 696e 7465 7254 6974  CustomTkinterTit
-00000620: 6c65 6261 722d 4578 616d 706c 6573 0d0a  lebar-Examples..
-00000630: 0d0a 2323 2320 f09f 939a 205f 2a57 696b  ..### .... _*Wik
-00000640: 692a 5f3a 0d0a 2323 2323 2049 6620 796f  i*_:..#### If yo
-00000650: 7527 6420 6c69 6b65 2074 6f20 6b6e 6f77  u'd like to know
-00000660: 2068 6f77 2074 6f20 7573 6520 7468 6520   how to use the 
-00000670: 6675 6e63 7469 6f6e 7320 796f 7520 6361  functions you ca
-00000680: 6e20 6361 6c6c 2c20 7669 7369 7420 7468  n call, visit th
-00000690: 6520 5363 7269 7074 2073 6563 7469 6f6e  e Script section
-000006a0: 206f 6620 7468 6520 4375 7374 6f6d 546b   of the CustomTk
-000006b0: 696e 7465 7254 6974 6c65 6261 7220 7769  interTitlebar wi
-000006c0: 6b69 3a0d 0a68 7474 7073 3a2f 2f67 6974  ki:..https://git
-000006d0: 6875 622e 636f 6d2f 6c69 7474 6c65 7768  hub.com/littlewh
-000006e0: 6974 6563 6c6f 7564 2f43 7573 746f 6d54  itecloud/CustomT
-000006f0: 6b69 6e74 6572 5469 746c 6562 6172 2f77  kinterTitlebar/w
-00000700: 696b 692f 5363 7269 7074 0d0a 0d0a 2323  iki/Script....##
-00000710: 2320 f09f 93a5 2044 6f77 6e6c 6f61 643a  # .... Download:
-00000720: 0d0a 596f 7520 6361 6e20 7573 6520 7069  ..You can use pi
-00000730: 7020 746f 2069 6e73 7461 6c6c 0d0a 6060  p to install..``
-00000740: 6062 6174 6368 0d0a 7069 7020 696e 7374  `batch..pip inst
-00000750: 616c 6c20 4375 7374 6f6d 546b 696e 7465  all CustomTkinte
-00000760: 7254 6974 6c65 6261 723e 3d31 2e30 2e37  rTitlebar>=1.0.7
-00000770: 2e33 0d0a 6060 600d 0a59 6f75 2063 616e  .3..```..You can
-00000780: 2061 6c73 6f20 646f 776e 6c6f 6164 2074   also download t
-00000790: 6865 2063 6f64 6520 6672 6f6d 2067 6974  he code from git
-000007a0: 6875 6220 6f72 2063 6865 636b 2074 6865  hub or check the
-000007b0: 2072 6561 6c61 7365 0d0a 0d0a 2323 2320   realase....### 
-000007c0: 5669 6577 3a20 0d0a 6874 7470 733a 2f2f  View: ..https://
-000007d0: 7573 6572 2d69 6d61 6765 732e 6769 7468  user-images.gith
-000007e0: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
-000007f0: 6d2f 3731 3135 3936 3431 2f32 3332 3138  m/71159641/23218
-00000800: 3132 3638 2d63 6632 3064 3232 372d 6430  1268-cf20d227-d0
-00000810: 6264 2d34 3834 302d 3962 3331 2d66 6133  bd-4840-9b31-fa3
-00000820: 6166 3135 3065 3463 382e 6d70 340d 0a23  af150e4c8.mp4..#
-00000830: 2323 2320 696e 7365 7274 2063 6f6d 706f  ### insert compo
-00000840: 6e65 6e74 2074 6f20 7469 746c 6562 6172  nent to titlebar
-00000850: 3a0d 0a21 5b69 6d61 6765 5d28 6874 7470  :..![image](http
-00000860: 733a 2f2f 7573 6572 2d69 6d61 6765 732e  s://user-images.
-00000870: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
-00000880: 742e 636f 6d2f 3731 3135 3936 3431 2f32  t.com/71159641/2
-00000890: 3038 3233 3138 3939 2d63 3235 6661 3935  08231899-c25fa95
-000008a0: 302d 3537 6637 2d34 6139 302d 3830 3935  0-57f7-4a90-8095
-000008b0: 2d63 6365 6164 6266 3664 3337 312e 706e  -cceadbf6d371.pn
-000008c0: 6729 0d0a 2323 2323 2042 6c75 723a 0d0a  g)..#### Blur:..
-000008d0: 215b 696d 6167 655d 2868 7474 7073 3a2f  ![image](https:/
-000008e0: 2f75 7365 722d 696d 6167 6573 2e67 6974  /user-images.git
-000008f0: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00000900: 6f6d 2f37 3131 3539 3634 312f 3231 3533  om/71159641/2153
-00000910: 3138 3932 332d 3532 3163 3565 6664 2d38  18923-521c5efd-8
-00000920: 3536 622d 3432 6562 2d61 6162 382d 3032  56b-42eb-aab8-02
-00000930: 6263 3561 6434 3732 3765 2e70 6e67 290d  bc5ad4727e.png).
-00000940: 0a23 2323 2320 466c 7565 6e74 203a 0d0a  .#### Fluent :..
-00000950: 215b 696d 6167 655d 2868 7474 7073 3a2f  ![image](https:/
-00000960: 2f75 7365 722d 696d 6167 6573 2e67 6974  /user-images.git
-00000970: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00000980: 6f6d 2f37 3131 3539 3634 312f 3231 3533  om/71159641/2153
-00000990: 3138 3932 302d 6135 6263 6531 3139 2d63  18920-a5bce119-c
-000009a0: 3334 332d 3430 6664 2d62 3036 382d 3965  343-40fd-b068-9e
-000009b0: 6362 6534 3434 6136 3066 2e70 6e67 290d  cbe444a60f.png).
-000009c0: 0a23 2323 2069 636f 6e20 2620 7769 6e64  .### icon & wind
-000009d0: 6f77 7465 7874 3a0d 0a21 5b69 6d61 6765  owtext:..![image
-000009e0: 5d28 6874 7470 733a 2f2f 7573 6572 2d69  ](https://user-i
-000009f0: 6d61 6765 732e 6769 7468 7562 7573 6572  mages.githubuser
-00000a00: 636f 6e74 656e 742e 636f 6d2f 3731 3135  content.com/7115
-00000a10: 3936 3431 2f32 3039 3630 3539 3335 2d65  9641/209605935-e
-00000a20: 3832 3437 3063 652d 6530 6432 2d34 3234  82470ce-e0d2-424
-00000a30: 342d 3932 3939 2d64 6263 6636 3636 6337  4-9299-dbcf666c7
-00000a40: 6536 622e 706e 6729 0d0a 215b 696d 6167  e6b.png)..![imag
-00000a50: 655d 2868 7474 7073 3a2f 2f75 7365 722d  e](https://user-
-00000a60: 696d 6167 6573 2e67 6974 6875 6275 7365  images.githubuse
-00000a70: 7263 6f6e 7465 6e74 2e63 6f6d 2f37 3131  rcontent.com/711
-00000a80: 3539 3634 312f 3230 3936 3035 3934 302d  59641/209605940-
-00000a90: 6339 6335 3863 6439 2d36 6666 332d 3434  c9c58cd9-6ff3-44
-00000aa0: 3535 2d39 6637 662d 3232 3936 3131 6136  55-9f7f-229611a6
-00000ab0: 3763 6461 2e70 6e67 290d 0a21 5b69 6d61  7cda.png)..![ima
-00000ac0: 6765 5d28 6874 7470 733a 2f2f 7573 6572  ge](https://user
-00000ad0: 2d69 6d61 6765 732e 6769 7468 7562 7573  -images.githubus
-00000ae0: 6572 636f 6e74 656e 742e 636f 6d2f 3731  ercontent.com/71
-00000af0: 3135 3936 3431 2f32 3039 3630 3539 3431  159641/209605941
-00000b00: 2d64 3338 3733 3264 642d 3139 3137 2d34  -d38732dd-1917-4
-00000b10: 3265 302d 3938 3561 2d65 6261 3938 6532  2e0-985a-eba98e2
-00000b20: 3134 3934 622e 706e 6729 0d0a 2323 2323  1494b.png)..####
-00000b30: 2043 7573 746f 6d20 6d69 6e73 697a 6520   Custom minsize 
-00000b40: 2620 6d61 7873 697a 653a 0d0a 215b 696d  & maxsize:..![im
-00000b50: 6167 655d 2868 7474 7073 3a2f 2f75 7365  age](https://use
-00000b60: 722d 696d 6167 6573 2e67 6974 6875 6275  r-images.githubu
-00000b70: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f37  sercontent.com/7
-00000b80: 3131 3539 3634 312f 3230 3934 3534 3938  1159641/20945498
-00000b90: 332d 6261 3062 6161 3331 2d39 6330 372d  3-ba0baa31-9c07-
-00000ba0: 3435 6265 2d38 6466 662d 3437 6461 3736  45be-8dff-47da76
-00000bb0: 6266 3164 6266 2e70 6e67 290d 0a21 5b69  bf1dbf.png)..![i
-00000bc0: 6d61 6765 5d28 6874 7470 733a 2f2f 7573  mage](https://us
-00000bd0: 6572 2d69 6d61 6765 732e 6769 7468 7562  er-images.github
-00000be0: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00000bf0: 3731 3135 3936 3431 2f32 3039 3435 3439  71159641/2094549
-00000c00: 3834 2d65 3336 3938 6638 392d 3964 3064  84-e3698f89-9d0d
-00000c10: 2d34 6265 312d 3861 6633 2d31 6361 3738  -4be1-8af3-1ca78
-00000c20: 6331 3036 3864 632e 706e 6729 0d0a 215b  c1068dc.png)..![
-00000c30: 696d 6167 655d 2868 7474 7073 3a2f 2f75  image](https://u
-00000c40: 7365 722d 696d 6167 6573 2e67 6974 6875  ser-images.githu
-00000c50: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00000c60: 2f37 3131 3539 3634 312f 3230 3934 3534  /71159641/209454
-00000c70: 3938 352d 3764 3732 3530 3833 2d64 6263  985-7d725083-dbc
-00000c80: 622d 3438 3536 2d38 3865 342d 3230 3061  b-4856-88e4-200a
-00000c90: 3334 3131 3139 3338 2e70 6e67 290d 0a21  34111938.png)..!
-00000ca0: 5b69 6d61 6765 5d28 6874 7470 733a 2f2f  [image](https://
-00000cb0: 7573 6572 2d69 6d61 6765 732e 6769 7468  user-images.gith
-00000cc0: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
-00000cd0: 6d2f 3731 3135 3936 3431 2f32 3039 3435  m/71159641/20945
-00000ce0: 3530 3031 2d66 3438 6330 3736 612d 6361  5001-f48c076a-ca
-00000cf0: 6330 2d34 3331 302d 3937 3565 2d30 6662  c0-4310-975e-0fb
-00000d00: 3634 3835 3566 3463 642e 706e 6729 0d0a  64855f4cd.png)..
-00000d10: 2323 2323 204c 6967 6874 2054 6865 6d65  #### Light Theme
-00000d20: 3a0d 0a21 5b69 6d61 6765 5d28 6874 7470  :..![image](http
-00000d30: 733a 2f2f 7573 6572 2d69 6d61 6765 732e  s://user-images.
-00000d40: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
-00000d50: 742e 636f 6d2f 3731 3135 3936 3431 2f32  t.com/71159641/2
-00000d60: 3130 3238 3338 3633 2d35 3366 3436 3339  10283863-53f4639
-00000d70: 322d 6665 3734 2d34 6434 662d 3839 3339  2-fe74-4d4f-8939
-00000d80: 2d34 6234 3266 3665 3936 6330 622e 706e  -4b42f6e96c0b.pn
-00000d90: 6729 0d0a 215b 696d 6167 655d 2868 7474  g)..![image](htt
-00000da0: 7073 3a2f 2f75 7365 722d 696d 6167 6573  ps://user-images
-00000db0: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-00000dc0: 6e74 2e63 6f6d 2f37 3131 3539 3634 312f  nt.com/71159641/
-00000dd0: 3231 3032 3834 3135 372d 6130 3131 3137  210284157-a01117
-00000de0: 6235 2d32 6161 652d 3434 6366 2d38 3963  b5-2aae-44cf-89c
-00000df0: 652d 6265 3365 6430 3237 3630 3766 2e70  e-be3ed027607f.p
-00000e00: 6e67 290d 0a23 2323 2320 466f 6375 7320  ng)..#### Focus 
-00000e10: 6f6e 3a0d 0a21 5b69 6d61 6765 5d28 6874  on:..![image](ht
-00000e20: 7470 733a 2f2f 7573 6572 2d69 6d61 6765  tps://user-image
-00000e30: 732e 6769 7468 7562 7573 6572 636f 6e74  s.githubusercont
-00000e40: 656e 742e 636f 6d2f 3731 3135 3936 3431  ent.com/71159641
-00000e50: 2f32 3135 3331 3930 3032 2d31 6236 6432  /215319002-1b6d2
-00000e60: 6166 392d 3238 3935 2d34 6665 322d 3830  af9-2895-4fe2-80
-00000e70: 3065 2d36 3337 3736 3166 3038 6666 352e  0e-637761f08ff5.
-00000e80: 706e 6729 0d0a 2323 2323 2046 6f63 7573  png)..#### Focus
-00000e90: 206f 7574 3a0d 0a21 5b69 6d61 6765 5d28   out:..![image](
-00000ea0: 6874 7470 733a 2f2f 7573 6572 2d69 6d61  https://user-ima
-00000eb0: 6765 732e 6769 7468 7562 7573 6572 636f  ges.githubuserco
-00000ec0: 6e74 656e 742e 636f 6d2f 3731 3135 3936  ntent.com/711596
-00000ed0: 3431 2f32 3135 3331 3930 3030 2d33 3163  41/215319000-31c
-00000ee0: 3630 3831 642d 3361 6235 2d34 6361 382d  6081d-3ab5-4ca8-
-00000ef0: 3934 3333 2d61 3830 3333 6131 3532 6161  9433-a8033a152aa
-00000f00: 652e 706e 6729 0d0a 0d0a 2323 2320 f09f  e.png)....### ..
-00000f10: 93a6 2052 6571 7569 7265 3a0d 0a3e 202d  .. Require:..> -
-00000f20: 205f 5769 6e64 6f77 7320 3130 5f0d 0a3e   _Windows 10_..>
-00000f30: 202d 205f 5079 7468 6f6e 203e 3d20 332e   - _Python >= 3.
-00000f40: 382e 305f 0d0a 3e20 2d20 5f54 636c 2f54  8.0_..> - _Tcl/T
-00000f50: 6b20 3e3d 2038 2e36 2e30 5f0d 0a3e 202d  k >= 8.6.0_..> -
-00000f60: 205f 5069 6c6c 6f77 203e 3d20 392e 302e   _Pillow >= 9.0.
-00000f70: 305f 0d0a 3e20 2d20 5f64 6172 6b64 6574  0_..> - _darkdet
-00000f80: 6563 7420 3e3d 2030 2e38 2e30 5f0d 0a3e  ect >= 0.8.0_..>
-00000f90: 202d 205f 426c 7572 5769 6e64 6f77 203e   - _BlurWindow >
-00000fa0: 3d20 312e 322e 315f 2049 6620 796f 7520  = 1.2.1_ If you 
-00000fb0: 646f 6e27 7420 7573 6520 626c 7572 2c20  don't use blur, 
-00000fc0: 796f 7520 6361 6e20 6967 6e6f 7265 2069  you can ignore i
-00000fd0: 740d 0a60 6060 6261 7463 680d 0a70 7974  t..```batch..pyt
-00000fe0: 686f 6e20 2d6d 2070 6970 2069 6e73 7461  hon -m pip insta
-00000ff0: 6c6c 202d 2d75 7067 7261 6465 2070 6970  ll --upgrade pip
-00001000: 0d0a 7069 7020 696e 7374 616c 6c20 7069  ..pip install pi
-00001010: 6c6c 6f77 202d 2d75 7365 720d 0a70 6970  llow --user..pip
-00001020: 2069 6e73 7461 6c6c 2064 6172 6b64 6574   install darkdet
-00001030: 6563 7420 2d2d 7573 6572 0d0a 7069 7020  ect --user..pip 
-00001040: 696e 7374 616c 6c20 426c 7572 5769 6e64  install BlurWind
-00001050: 6f77 202d 2d75 7365 7220 0d0a 6060 600d  ow --user ..```.
-00001060: 0a0d 0a23 2323 20f0 9f93 9620 5573 6167  ...### .... Usag
-00001070: 653a 0d0a 6060 6070 7974 686f 6e0d 0a66  e:..```python..f
-00001080: 726f 6d20 6375 7374 6f6d 746b 696e 7465  rom customtkinte
-00001090: 7274 6974 6c65 6261 7220 696d 706f 7274  rtitlebar import
-000010a0: 2054 6b0d 0a66 726f 6d20 746b 696e 7465   Tk..from tkinte
-000010b0: 7220 696d 706f 7274 2074 746b 0d0a 6578  r import ttk..ex
-000010c0: 616d 706c 6520 3d20 546b 2829 0d0a 6578  ample = Tk()..ex
-000010d0: 616d 706c 652e 7469 746c 6528 2254 6974  ample.title("Tit
-000010e0: 6c65 4261 7222 290d 0a65 7861 6d70 6c65  leBar")..example
-000010f0: 2e67 656f 6d65 7472 7928 2231 3033 3078  .geometry("1030x
-00001100: 3537 3022 290d 0a65 6e20 3d20 7474 6b2e  570")..en = ttk.
-00001110: 456e 7472 7928 6578 616d 706c 652e 7469  Entry(example.ti
-00001120: 746c 6562 6172 290d 0a65 6e2e 7061 636b  tlebar)..en.pack
-00001130: 2866 696c 6c20 3d20 592c 2065 7870 616e  (fill = Y, expan
-00001140: 6420 3d20 5472 7565 2c20 6970 6164 7820  d = True, ipadx 
-00001150: 3d20 3330 2c20 7061 6479 203d 2035 290d  = 30, pady = 5).
-00001160: 0a65 7861 6d70 6c65 2e6d 6169 6e6c 6f6f  .example.mainloo
-00001170: 7028 290d 0a60 6060 0d0a 0d0a 2323 2320  p()..```....### 
-00001180: f09f 92be 2053 7570 706f 7274 3a0d 0a23  .... Support:..#
-00001190: 2323 2320 4974 2073 7570 706f 7274 2057  ### It support W
-000011a0: 696e 646f 7773 2031 3020 3332 202f 2036  indows 10 32 / 6
-000011b0: 3420 6269 7420 6e6f 772e 0d0a 3e20 2a2a  4 bit now...> **
-000011c0: 4d61 7962 6520 6974 2061 6c73 6f20 7375  Maybe it also su
-000011d0: 7070 6f72 7420 5769 6e64 6f77 7320 3131  pport Windows 11
-000011e0: 2c20 4920 616d 2075 7369 6e67 2057 696e  , I am using Win
-000011f0: 646f 7773 2031 302c 2049 2064 6964 6e27  dows 10, I didn'
-00001200: 7420 7465 7374 2074 6869 7320 7072 6f6a  t test this proj
-00001210: 6563 7420 6f6e 2057 696e 646f 7773 2031  ect on Windows 1
-00001220: 3120 7965 742a 2a0d 0a                   1 yet**..
+00000010: 3a20 322e 310a 4e61 6d65 3a20 4375 7374  : 2.1.Name: Cust
+00000020: 6f6d 546b 696e 7465 7254 6974 6c65 6261  omTkinterTitleba
+00000030: 720a 5665 7273 696f 6e3a 2031 2e30 2e37  r.Version: 1.0.7
+00000040: 2e39 0a53 756d 6d61 7279 3a20 5468 6973  .9.Summary: This
+00000050: 2069 7320 6120 f09f 939a 7072 6f6a 6563   is a ....projec
+00000060: 7420 6361 6e20 6865 6c70 2079 6f75 2074  t can help you t
+00000070: 6f20 6861 7665 2061 2063 7573 746f 6d20  o have a custom 
+00000080: 7469 746c 6562 6172 2120 e8bf 99e6 98af  titlebar! ......
+00000090: e4b8 80e4 b8aa e58f afe4 bba5 e588 9be5  ................
+000000a0: bbba e887 aae5 ae9a e4b9 89e6 a087 e9a2  ................
+000000b0: 98e6 a08f e79a 84f0 9f93 9ae9 a1b9 e79b  ................
+000000c0: ae0a 486f 6d65 2d70 6167 653a 2068 7474  ..Home-page: htt
+000000d0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000000e0: 6c69 7474 6c65 7768 6974 6563 6c6f 7564  littlewhitecloud
+000000f0: 2f43 7573 746f 6d54 6b69 6e74 6572 5469  /CustomTkinterTi
+00000100: 746c 6562 6172 0a41 7574 686f 723a 206c  tlebar.Author: l
+00000110: 6974 746c 6577 6869 7465 636c 6f75 640a  ittlewhitecloud.
+00000120: 4175 7468 6f72 2d65 6d61 696c 3a20 7131  Author-email: q1
+00000130: 3134 3139 3236 3634 3740 3136 332e 636f  141926647@163.co
+00000140: 6d0a 436c 6173 7369 6669 6572 3a20 4465  m.Classifier: De
+00000150: 7665 6c6f 706d 656e 7420 5374 6174 7573  velopment Status
+00000160: 203a 3a20 3520 2d20 5072 6f64 7563 7469   :: 5 - Producti
+00000170: 6f6e 2f53 7461 626c 650a 436c 6173 7369  on/Stable.Classi
+00000180: 6669 6572 3a20 496e 7465 6e64 6564 2041  fier: Intended A
+00000190: 7564 6965 6e63 6520 3a3a 2044 6576 656c  udience :: Devel
+000001a0: 6f70 6572 730a 436c 6173 7369 6669 6572  opers.Classifier
+000001b0: 3a20 4c69 6365 6e73 6520 3a3a 204f 5349  : License :: OSI
+000001c0: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
+000001d0: 204c 6963 656e 7365 0a43 6c61 7373 6966   License.Classif
+000001e0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+000001f0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000200: 686f 6e20 3a3a 2033 2e38 0a43 6c61 7373  hon :: 3.8.Class
+00000210: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00000220: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000230: 7974 686f 6e20 3a3a 2033 2e39 0a43 6c61  ython :: 3.9.Cla
+00000240: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+00000250: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000260: 2050 7974 686f 6e20 3a3a 2033 2e31 300a   Python :: 3.10.
+00000270: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000280: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000290: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+000002a0: 3131 0a44 6573 6372 6970 7469 6f6e 2d43  11.Description-C
+000002b0: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
+000002c0: 742f 6d61 726b 646f 776e 0a4c 6963 656e  t/markdown.Licen
+000002d0: 7365 2d46 696c 653a 204c 4943 454e 5345  se-File: LICENSE
+000002e0: 0a0a 2320 5fe8 87aa e5ae 9ae4 b989 e6a0  ..# _...........
+000002f0: 87e9 a298 e6a0 8f5f 205f 4375 7374 6f6d  ......._ _Custom
+00000300: 546b 696e 7465 7254 6974 6c65 6261 725f  TkinterTitlebar_
+00000310: 0a21 5b69 6d61 6765 5d28 6874 7470 733a  .![image](https:
+00000320: 2f2f 6769 7468 7562 2e63 6f6d 2f6c 6974  //github.com/lit
+00000330: 746c 6577 6869 7465 636c 6f75 642f 4375  tlewhitecloud/Cu
+00000340: 7374 6f6d 546b 696e 7465 7254 6974 6c65  stomTkinterTitle
+00000350: 6261 722f 6173 7365 7473 2f37 3131 3539  bar/assets/71159
+00000360: 3634 312f 3330 6637 6337 3835 2d64 3138  641/30f7c785-d18
+00000370: 392d 3438 3635 2d38 3039 352d 3338 3432  9-4865-8095-3842
+00000380: 3539 6539 6234 3139 290a 0a21 5b69 6d61  59e9b419)..![ima
+00000390: 6765 5d28 6874 7470 733a 2f2f 7573 6572  ge](https://user
+000003a0: 2d69 6d61 6765 732e 6769 7468 7562 7573  -images.githubus
+000003b0: 6572 636f 6e74 656e 742e 636f 6d2f 3731  ercontent.com/71
+000003c0: 3135 3936 3431 2f32 3039 3738 3333 3734  159641/209783374
+000003d0: 2d66 3565 6133 3631 332d 6562 3635 2d34  -f5ea3613-eb65-4
+000003e0: 6563 332d 3934 3632 2d30 6562 3738 3833  ec3-9462-0eb7883
+000003f0: 6433 6266 392e 706e 6729 0a21 5b69 6d61  d3bf9.png).![ima
+00000400: 6765 5d28 6874 7470 733a 2f2f 7573 6572  ge](https://user
+00000410: 2d69 6d61 6765 732e 6769 7468 7562 7573  -images.githubus
+00000420: 6572 636f 6e74 656e 742e 636f 6d2f 3731  ercontent.com/71
+00000430: 3135 3936 3431 2f32 3039 3132 3836 3733  159641/209128673
+00000440: 2d39 3361 3666 3164 622d 3636 6136 2d34  -93a6f1db-66a6-4
+00000450: 3636 372d 3962 6437 2d61 3363 3262 6130  667-9bd7-a3c2ba0
+00000460: 3936 6635 632e 706e 6729 0a0a 2323 2320  96f5c.png)..### 
+00000470: f09f 9383 202a e8bf 99e6 98af e4b8 80e4  .... *..........
+00000480: b8aa e9a1 b9e7 9bae e58f afe4 bba5 e5b8  ................
+00000490: aee5 8aa9 e4bd a0e6 8ba5 e69c 89e4 b880  ................
+000004a0: e4b8 aae8 87aa e5ae 9ae4 b989 e79a 84e6  ................
+000004b0: a087 e9a2 98e6 a08f efbc 81e5 b08f e7bb  ................
+000004c0: 84e4 bbb6 e58f afe4 bba5 e8a2 abe6 94be  ................
+000004d0: e588 b0e8 bf99 e4b8 aae6 a087 e9a2 98e6  ................
+000004e0: a08f e987 8ce9 9da2 2a20 2a54 6869 7320  ........* *This 
+000004f0: 6973 2061 2070 726f 6a65 6374 2063 616e  is a project can
+00000500: 2068 656c 7020 796f 7520 746f 2068 6176   help you to hav
+00000510: 6520 6120 6375 7374 6f6d 2074 6974 6c65  e a custom title
+00000520: 6261 7221 2057 6964 6765 7473 2063 616e  bar! Widgets can
+00000530: 2061 6464 2069 6e74 6f20 7469 746c 6562   add into titleb
+00000540: 6172 212a 0a23 2323 2320 5fe5 85b3 e4ba  ar!*.#### _.....
+00000550: 8ee6 9bb4 e5a4 9ae8 bf99 e4b8 aae9 a1b9  ................
+00000560: e79b aeef bc8c e688 91e5 8699 e4ba 86e4  ................
+00000570: b880 e7af 87e6 9687 e7ab a0e5 9ca8 4269  ..............Bi
+00000580: 6c69 6269 6c69 e4b8 8aef bc8c e5ae 83e5  libili..........
+00000590: be88 e8af a6e7 bb86 e79a 84e8 afb4 e4ba  ................
+000005a0: 86e8 bf99 e4b8 aae9 a1b9 e79b ae5f 205f  ............._ _
+000005b0: 4d6f 7265 2061 626f 7574 2074 6869 7320  More about this 
+000005c0: 7072 6f6a 6563 742c 2049 2077 726f 7465  project, I wrote
+000005d0: 2061 6e20 6172 7469 636c 6520 6f6e 2042   an article on B
+000005e0: 696c 6962 696c 692c 2077 6869 6368 2074  ilibili, which t
+000005f0: 616c 6b73 2061 626f 7574 2074 6869 7320  alks about this 
+00000600: 7072 6f6a 6563 7420 696e 206d 6f72 6520  project in more 
+00000610: 6465 7461 696c 3a5f 2068 7474 7073 3a2f  detail:_ https:/
+00000620: 2f77 7777 2e62 696c 6962 696c 692e 636f  /www.bilibili.co
+00000630: 6d2f 7265 6164 2f63 7632 3035 3538 3437  m/read/cv2055847
+00000640: 330a 2323 2323 20e5 a682 e69e 9ce4 bda0  3.#### .........
+00000650: e596 9ce6 aca2 e5ae 83ef bc8c e8af b7e7  ................
+00000660: bb99 e9a2 97e6 989f efbc 8120 6c65 6176  ........... leav
+00000670: 6520 6120 7374 6172 2069 6620 796f 7520  e a star if you 
+00000680: 6c69 6b65 2069 7421 0a0a 2323 2320 e9a2  like it!..### ..
+00000690: 84e8 a788 2056 6965 773a 200a 6874 7470  .... View: .http
+000006a0: 733a 2f2f 7573 6572 2d69 6d61 6765 732e  s://user-images.
+000006b0: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+000006c0: 742e 636f 6d2f 3731 3135 3936 3431 2f32  t.com/71159641/2
+000006d0: 3332 3138 3132 3638 2d63 6632 3064 3232  32181268-cf20d22
+000006e0: 372d 6430 6264 2d34 3834 302d 3962 3331  7-d0bd-4840-9b31
+000006f0: 2d66 6133 6166 3135 3065 3463 382e 6d70  -fa3af150e4c8.mp
+00000700: 340a 2323 2323 20e6 8f92 e585 a5e7 bb84  4.#### .........
+00000710: e4bb b620 496e 7365 7274 2063 6f6d 706f  ... Insert compo
+00000720: 6e65 6e74 2074 6f20 7469 746c 6562 6172  nent to titlebar
+00000730: 3a0a 215b 696d 6167 655d 2868 7474 7073  :.![image](https
+00000740: 3a2f 2f75 7365 722d 696d 6167 6573 2e67  ://user-images.g
+00000750: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00000760: 2e63 6f6d 2f37 3131 3539 3634 312f 3230  .com/71159641/20
+00000770: 3832 3331 3839 392d 6332 3566 6139 3530  8231899-c25fa950
+00000780: 2d35 3766 372d 3461 3930 2d38 3039 352d  -57f7-4a90-8095-
+00000790: 6363 6561 6462 6636 6433 3731 2e70 6e67  cceadbf6d371.png
+000007a0: 290a 2323 2323 20e8 87aa e5ae 9ae4 b989  ).#### .........
+000007b0: e69c 80e5 a4a7 e58c 96e6 9c80 e5b0 8fe5  ................
+000007c0: 8c96 2043 7573 746f 6d20 6d69 6e73 697a  .. Custom minsiz
+000007d0: 6520 2620 6d61 7873 697a 653a 0a21 5b69  e & maxsize:.![i
+000007e0: 6d61 6765 5d28 6874 7470 733a 2f2f 7573  mage](https://us
+000007f0: 6572 2d69 6d61 6765 732e 6769 7468 7562  er-images.github
+00000800: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00000810: 3731 3135 3936 3431 2f32 3039 3435 3439  71159641/2094549
+00000820: 3833 2d62 6130 6261 6133 312d 3963 3037  83-ba0baa31-9c07
+00000830: 2d34 3562 652d 3864 6666 2d34 3764 6137  -45be-8dff-47da7
+00000840: 3662 6631 6462 662e 706e 6729 0a21 5b69  6bf1dbf.png).![i
+00000850: 6d61 6765 5d28 6874 7470 733a 2f2f 7573  mage](https://us
+00000860: 6572 2d69 6d61 6765 732e 6769 7468 7562  er-images.github
+00000870: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00000880: 3731 3135 3936 3431 2f32 3039 3435 3439  71159641/2094549
+00000890: 3834 2d65 3336 3938 6638 392d 3964 3064  84-e3698f89-9d0d
+000008a0: 2d34 6265 312d 3861 6633 2d31 6361 3738  -4be1-8af3-1ca78
+000008b0: 6331 3036 3864 632e 706e 6729 0a21 5b69  c1068dc.png).![i
+000008c0: 6d61 6765 5d28 6874 7470 733a 2f2f 7573  mage](https://us
+000008d0: 6572 2d69 6d61 6765 732e 6769 7468 7562  er-images.github
+000008e0: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+000008f0: 3731 3135 3936 3431 2f32 3039 3435 3439  71159641/2094549
+00000900: 3835 2d37 6437 3235 3038 332d 6462 6362  85-7d725083-dbcb
+00000910: 2d34 3835 362d 3838 6534 2d32 3030 6133  -4856-88e4-200a3
+00000920: 3431 3131 3933 382e 706e 6729 0a21 5b69  4111938.png).![i
+00000930: 6d61 6765 5d28 6874 7470 733a 2f2f 7573  mage](https://us
+00000940: 6572 2d69 6d61 6765 732e 6769 7468 7562  er-images.github
+00000950: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00000960: 3731 3135 3936 3431 2f32 3039 3435 3530  71159641/2094550
+00000970: 3031 2d66 3438 6330 3736 612d 6361 6330  01-f48c076a-cac0
+00000980: 2d34 3331 302d 3937 3565 2d30 6662 3634  -4310-975e-0fb64
+00000990: 3835 3566 3463 642e 706e 6729 0a23 2323  855f4cd.png).###
+000009a0: 2320 e4ba aee4 b8bb e9a2 9820 4c69 6768  # ......... Ligh
+000009b0: 7420 5468 656d 653a 0a21 5b69 6d61 6765  t Theme:.![image
+000009c0: 5d28 6874 7470 733a 2f2f 7573 6572 2d69  ](https://user-i
+000009d0: 6d61 6765 732e 6769 7468 7562 7573 6572  mages.githubuser
+000009e0: 636f 6e74 656e 742e 636f 6d2f 3731 3135  content.com/7115
+000009f0: 3936 3431 2f32 3130 3238 3338 3633 2d35  9641/210283863-5
+00000a00: 3366 3436 3339 322d 6665 3734 2d34 6434  3f46392-fe74-4d4
+00000a10: 662d 3839 3339 2d34 6234 3266 3665 3936  f-8939-4b42f6e96
+00000a20: 6330 622e 706e 6729 0a21 5b69 6d61 6765  c0b.png).![image
+00000a30: 5d28 6874 7470 733a 2f2f 7573 6572 2d69  ](https://user-i
+00000a40: 6d61 6765 732e 6769 7468 7562 7573 6572  mages.githubuser
+00000a50: 636f 6e74 656e 742e 636f 6d2f 3731 3135  content.com/7115
+00000a60: 3936 3431 2f32 3130 3238 3431 3537 2d61  9641/210284157-a
+00000a70: 3031 3131 3762 352d 3261 6165 2d34 3463  01117b5-2aae-44c
+00000a80: 662d 3839 6365 2d62 6533 6564 3032 3736  f-89ce-be3ed0276
+00000a90: 3037 662e 706e 6729 0a23 2323 2320 e881  07f.png).#### ..
+00000aa0: 9ae7 84a6 e592 8ce6 9caa e881 9ae7 84a6  ................
+00000ab0: 2046 6f63 7573 2069 6e20 2620 6f75 743a   Focus in & out:
+00000ac0: 0a21 5b69 6d61 6765 5d28 6874 7470 733a  .![image](https:
+00000ad0: 2f2f 7573 6572 2d69 6d61 6765 732e 6769  //user-images.gi
+00000ae0: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+00000af0: 636f 6d2f 3731 3135 3936 3431 2f32 3335  com/71159641/235
+00000b00: 3334 3838 3837 2d62 6661 3231 3033 352d  348887-bfa21035-
+00000b10: 3534 6230 2d34 3032 312d 3863 3933 2d34  54b0-4021-8c93-4
+00000b20: 6362 3764 3431 6261 3131 612e 706e 6729  cb7d41ba11a.png)
+00000b30: 0a21 5b69 6d61 6765 5d28 6874 7470 733a  .![image](https:
+00000b40: 2f2f 7573 6572 2d69 6d61 6765 732e 6769  //user-images.gi
+00000b50: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+00000b60: 636f 6d2f 3731 3135 3936 3431 2f32 3335  com/71159641/235
+00000b70: 3334 3838 3838 2d38 6665 3264 6535 612d  348888-8fe2de5a-
+00000b80: 6435 6265 2d34 3265 632d 6261 3433 2d66  d5be-42ec-ba43-f
+00000b90: 3938 3364 6439 3363 3833 372e 706e 6729  983dd93c837.png)
+00000ba0: 0a23 2323 2320 e4ba 91e6 af8d 204d 6963  .#### ...... Mic
+00000bb0: 613a 0a21 5b69 6d61 6765 5d28 6874 7470  a:.![image](http
+00000bc0: 733a 2f2f 7573 6572 2d69 6d61 6765 732e  s://user-images.
+00000bd0: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00000be0: 742e 636f 6d2f 3836 3336 3234 3233 2f32  t.com/86362423/2
+00000bf0: 3335 3432 3831 3232 2d33 3334 6430 3563  35428122-334d05c
+00000c00: 322d 3839 3237 2d34 6234 342d 6263 3033  2-8927-4b44-bc03
+00000c10: 2d61 6230 6163 3066 3136 3837 662e 706e  -ab0ac0f1687f.pn
+00000c20: 6729 0a21 5b69 6d61 6765 5d28 6874 7470  g).![image](http
+00000c30: 733a 2f2f 7573 6572 2d69 6d61 6765 732e  s://user-images.
+00000c40: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00000c50: 742e 636f 6d2f 3836 3336 3234 3233 2f32  t.com/86362423/2
+00000c60: 3335 3432 3839 3934 2d36 3863 3334 6339  35428994-68c34c9
+00000c70: 642d 3162 3330 2d34 6339 662d 3861 3634  d-1b30-4c9f-8a64
+00000c80: 2d61 3661 3736 3036 3030 3732 362e 706e  -a6a760600726.pn
+00000c90: 6729 0a23 2323 2320 e6a8 a1e7 b38a 2042  g).#### ...... B
+00000ca0: 6c75 723a 0a21 5b69 6d61 6765 5d28 6874  lur:.![image](ht
+00000cb0: 7470 733a 2f2f 7573 6572 2d69 6d61 6765  tps://user-image
+00000cc0: 732e 6769 7468 7562 7573 6572 636f 6e74  s.githubusercont
+00000cd0: 656e 742e 636f 6d2f 3731 3135 3936 3431  ent.com/71159641
+00000ce0: 2f32 3135 3331 3839 3233 2d35 3231 6335  /215318923-521c5
+00000cf0: 6566 642d 3835 3662 2d34 3265 622d 6161  efd-856b-42eb-aa
+00000d00: 6238 2d30 3262 6335 6164 3437 3237 652e  b8-02bc5ad4727e.
+00000d10: 706e 6729 0a23 2323 2320 e4ba 9ae5 858b  png).#### ......
+00000d20: e58a 9b20 466c 7565 6e74 203a 0a21 5b69  ... Fluent :.![i
+00000d30: 6d61 6765 5d28 6874 7470 733a 2f2f 7573  mage](https://us
+00000d40: 6572 2d69 6d61 6765 732e 6769 7468 7562  er-images.github
+00000d50: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00000d60: 3731 3135 3936 3431 2f32 3135 3331 3839  71159641/2153189
+00000d70: 3230 2d61 3562 6365 3131 392d 6333 3433  20-a5bce119-c343
+00000d80: 2d34 3066 642d 6230 3638 2d39 6563 6265  -40fd-b068-9ecbe
+00000d90: 3434 3461 3630 662e 706e 6729 0a0a 2323  444a60f.png)..##
+00000da0: 2320 f09f 8eb0 20e6 a0b7 e4be 8b20 4578  # .... ...... Ex
+00000db0: 616d 706c 653a 0a68 7474 7073 3a2f 2f67  ample:.https://g
+00000dc0: 6974 6875 622e 636f 6d2f 6c69 7474 6c65  ithub.com/little
+00000dd0: 7768 6974 6563 6c6f 7564 2f43 7573 746f  whitecloud/Custo
+00000de0: 6d54 6b69 6e74 6572 5469 746c 6562 6172  mTkinterTitlebar
+00000df0: 2d45 7861 6d70 6c65 730a 0a23 2323 20f0  -Examples..### .
+00000e00: 9f93 9a20 5f2a e7bb b4e5 9fba 2a5f 205f  ... _*......*_ _
+00000e10: 2a57 696b 692a 5f3a 0a23 2323 2320 6874  *Wiki*_:.#### ht
+00000e20: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000e30: 2f6c 6974 746c 6577 6869 7465 636c 6f75  /littlewhiteclou
+00000e40: 642f 4375 7374 6f6d 546b 696e 7465 7254  d/CustomTkinterT
+00000e50: 6974 6c65 6261 722f 7769 6b69 2f53 6372  itlebar/wiki/Scr
+00000e60: 6970 740a 0a23 2323 20f0 9f93 a520 e4b8  ipt..### .... ..
+00000e70: 8be8 bdbd 2044 6f77 6e6c 6f61 643a 0ae4  .... Download:..
+00000e80: bda0 e58f afe4 bba5 e4bd bfe7 94a8 5069  ..............Pi
+00000e90: 70e6 9da5 e5ae 89e8 a385 2059 6f75 2063  p......... You c
+00000ea0: 616e 2075 7365 2070 6970 2074 6f20 696e  an use pip to in
+00000eb0: 7374 616c 6c0a 6060 6062 6174 6368 0a70  stall.```batch.p
+00000ec0: 6970 2069 6e73 7461 6c6c 2043 7573 746f  ip install Custo
+00000ed0: 6d54 6b69 6e74 6572 5469 746c 6562 6172  mTkinterTitlebar
+00000ee0: 3e3d 312e 302e 372e 330a 6060 600a e4bd  >=1.0.7.3.```...
+00000ef0: a0e4 b99f e58f afe4 bba5 e79b b4e6 8ea5  ................
+00000f00: e4bb 8e67 6974 6875 62e4 b88a e4b8 8be8  ...github.......
+00000f10: bdbd e58e 9fe7 a081 e688 96e6 9fa5 e79c  ................
+00000f20: 8be5 8f91 e5b8 8320 596f 7520 6361 6e20  ....... You can 
+00000f30: 616c 736f 2064 6f77 6e6c 6f61 6420 7468  also download th
+00000f40: 6520 636f 6465 2066 726f 6d20 6769 7468  e code from gith
+00000f50: 7562 206f 7220 6368 6563 6b20 7468 6520  ub or check the 
+00000f60: 7265 616c 6173 650a 2323 2320 f09f 93a6  realase.### ....
+00000f70: 20e4 be9d e8b5 9620 5265 7175 6972 653a   ...... Require:
+00000f80: 0a3e 202d 205f 5769 6e64 6f77 7320 3130  .> - _Windows 10
+00000f90: 5f0a 3e20 2d20 5f50 7974 686f 6e20 3e3d  _.> - _Python >=
+00000fa0: 2033 2e38 2e30 5f0a 3e20 2d20 5f54 636c   3.8.0_.> - _Tcl
+00000fb0: 2f54 6b20 3e3d 2038 2e36 2e30 5f0a 3e20  /Tk >= 8.6.0_.> 
+00000fc0: 2d20 5f50 696c 6c6f 7720 3e3d 2039 2e30  - _Pillow >= 9.0
+00000fd0: 2e30 5f0a 3e20 2d20 5f64 6172 6b64 6574  .0_.> - _darkdet
+00000fe0: 6563 7420 3e3d 2030 2e38 2e30 5f0a 3e20  ect >= 0.8.0_.> 
+00000ff0: 2d20 5f42 6c75 7257 696e 646f 7720 3e3d  - _BlurWindow >=
+00001000: 2031 2e32 2e31 5f0a 6060 6062 6174 6368   1.2.1_.```batch
+00001010: 0a70 7974 686f 6e20 2d6d 2070 6970 2069  .python -m pip i
+00001020: 6e73 7461 6c6c 202d 2d75 7067 7261 6465  nstall --upgrade
+00001030: 2070 6970 0a70 6970 2069 6e73 7461 6c6c   pip.pip install
+00001040: 2070 696c 6c6f 7720 2d2d 7573 6572 0a70   pillow --user.p
+00001050: 6970 2069 6e73 7461 6c6c 2064 6172 6b64  ip install darkd
+00001060: 6574 6563 7420 2d2d 7573 6572 0a70 6970  etect --user.pip
+00001070: 2069 6e73 7461 6c6c 2042 6c75 7257 696e   install BlurWin
+00001080: 646f 7720 2d2d 7573 6572 200a 6060 600a  dow --user .```.
+00001090: e688 96e8 8085 e58f aae8 bf90 e8a1 8c20  ............... 
+000010a0: 4f72 206a 7573 7420 7275 6e0a 6060 6062  Or just run.```b
+000010b0: 6174 6368 0a70 6970 2069 6e73 7461 6c6c  atch.pip install
+000010c0: 2043 7573 746f 6d54 6b69 6e74 6572 5469   CustomTkinterTi
+000010d0: 746c 6562 6172 202d 2d75 7365 720a 6060  tlebar --user.``
+000010e0: 600a 0a23 2323 20f0 9f93 9620 e794 a8e6  `..### .... ....
+000010f0: b395 2055 7361 6765 3a0a 6060 6070 7974  .. Usage:.```pyt
+00001100: 686f 6e0a 6672 6f6d 2063 7573 746f 6d74  hon.from customt
+00001110: 6b69 6e74 6572 7469 746c 6562 6172 2069  kintertitlebar i
+00001120: 6d70 6f72 7420 546b 0a66 726f 6d20 746b  mport Tk.from tk
+00001130: 696e 7465 7220 696d 706f 7274 2074 746b  inter import ttk
+00001140: 0a65 7861 6d70 6c65 203d 2054 6b28 290a  .example = Tk().
+00001150: 6578 616d 706c 652e 7469 746c 6528 2254  example.title("T
+00001160: 6974 6c65 4261 7222 290a 6578 616d 706c  itleBar").exampl
+00001170: 652e 6765 6f6d 6574 7279 2822 3130 3330  e.geometry("1030
+00001180: 7835 3730 2229 0a65 6e20 3d20 7474 6b2e  x570").en = ttk.
+00001190: 456e 7472 7928 6578 616d 706c 652e 7469  Entry(example.ti
+000011a0: 746c 6562 6172 290a 656e 2e70 6163 6b28  tlebar).en.pack(
+000011b0: 6669 6c6c 203d 2059 2c20 6578 7061 6e64  fill = Y, expand
+000011c0: 203d 2054 7275 652c 2069 7061 6478 203d   = True, ipadx =
+000011d0: 2033 302c 2070 6164 7920 3d20 3529 0a65   30, pady = 5).e
+000011e0: 7861 6d70 6c65 2e6d 6169 6e6c 6f6f 7028  xample.mainloop(
+000011f0: 290a 6060 600a 0a23 2323 20f0 9f92 be20  ).```..### .... 
+00001200: e694 afe6 8c81 2053 7570 706f 7274 3a0a  ...... Support:.
+00001210: 2323 2323 20e5 ae83 e78e b0e5 9ca8 e694  #### ...........
+00001220: afe6 8c81 2057 696e 646f 7773 2031 302f  .... Windows 10/
+00001230: 3131 2033 322f 3634 20e4 bd8d 2049 7420  11 32/64 ... It 
+00001240: 7375 7070 6f72 7420 5769 6e64 6f77 7320  support Windows 
+00001250: 3130 2f31 3120 3332 2f36 3420 6269 7473  10/11 32/64 bits
+00001260: 206e 6f77 2e0a 0ae6 849f e8b0 a220 4048   now......... @H
+00001270: 7579 4875 6e67 3134 3038 e88a b1e6 97b6  uyHung1408......
+00001280: e997 b4e6 9da5 e59c a857 696e 646f 7773  .........Windows
+00001290: 3131 e4b8 8ae6 b58b e8af 95e5 ae83 210a  11............!.
+000012a0: 5468 616e 6b73 2040 4875 7948 756e 6731  Thanks @HuyHung1
+000012b0: 3430 3820 666f 7220 7465 7374 696e 6720  408 for testing 
+000012c0: 6974 206f 6e20 7769 6e64 6f77 7320 3131  it on windows 11
+000012d0: 210a                                     !.
```

### Comparing `CustomTkinterTitlebar-1.0.7.8/CustomTkinterTitlebar.egg-info/SOURCES.txt` & `CustomTkinterTitlebar-1.0.7.9/CustomTkinterTitlebar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CustomTkinterTitlebar-1.0.7.8/LICENSE` & `CustomTkinterTitlebar-1.0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `CustomTkinterTitlebar-1.0.7.8/PKG-INFO` & `CustomTkinterTitlebar-1.0.7.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,291 +1,302 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310d 0a4e 616d 653a 2043 7573  : 2.1..Name: Cus
-00000020: 746f 6d54 6b69 6e74 6572 5469 746c 6562  tomTkinterTitleb
-00000030: 6172 0d0a 5665 7273 696f 6e3a 2031 2e30  ar..Version: 1.0
-00000040: 2e37 2e38 0d0a 5375 6d6d 6172 793a 2054  .7.8..Summary: T
-00000050: 6869 7320 6973 2061 2070 726f 6a65 6374  his is a project
-00000060: 2063 616e 2068 656c 7020 796f 7520 746f   can help you to
-00000070: 2068 6176 6520 6120 6375 7374 6f6d 2074   have a custom t
-00000080: 6974 6c65 6261 7221 0d0a 486f 6d65 2d70  itlebar!..Home-p
-00000090: 6167 653a 2068 7474 703a 2f2f 6769 7468  age: http://gith
-000000a0: 7562 2e63 6f6d 2f6c 6974 746c 6577 6869  ub.com/littlewhi
-000000b0: 7465 636c 6f75 642f 4375 7374 6f6d 546b  tecloud/CustomTk
-000000c0: 696e 7465 7254 6974 6c65 6261 720d 0a41  interTitlebar..A
-000000d0: 7574 686f 723a 206c 6974 746c 6577 6869  uthor: littlewhi
-000000e0: 7465 636c 6f75 640d 0a41 7574 686f 722d  tecloud..Author-
-000000f0: 656d 6169 6c3a 2071 3131 3431 3932 3636  email: q11419266
-00000100: 3437 4031 3633 2e63 6f6d 0d0a 4b65 7977  47@163.com..Keyw
-00000110: 6f72 6473 3a20 7079 7468 6f6e 2063 2077  ords: python c w
-00000120: 696e 646f 7773 2063 706c 7573 706c 7573  indows cplusplus
-00000130: 2064 6c6c 2063 7070 2063 7573 746f 6d20   dll cpp custom 
-00000140: 7069 6c6c 6f77 2062 6c75 7220 6374 7970  pillow blur ctyp
-00000150: 6573 2074 6b20 7469 746c 6562 6172 2074  es tk titlebar t
-00000160: 6b69 6e74 6572 2077 696e 646f 7720 7769  kinter window wi
-00000170: 6e64 6f77 7331 3020 646f 6320 6d73 7663  ndows10 doc msvc
-00000180: 2064 6574 6169 6c73 2075 7365 7233 3220   details user32 
-00000190: 6461 726b 6465 7465 6374 0d0a 436c 6173  darkdetect..Clas
-000001a0: 7369 6669 6572 3a20 4465 7665 6c6f 706d  sifier: Developm
-000001b0: 656e 7420 5374 6174 7573 203a 3a20 3520  ent Status :: 5 
-000001c0: 2d20 5072 6f64 7563 7469 6f6e 2f53 7461  - Production/Sta
-000001d0: 626c 650d 0a43 6c61 7373 6966 6965 723a  ble..Classifier:
-000001e0: 2049 6e74 656e 6465 6420 4175 6469 656e   Intended Audien
-000001f0: 6365 203a 3a20 4465 7665 6c6f 7065 7273  ce :: Developers
-00000200: 0d0a 436c 6173 7369 6669 6572 3a20 546f  ..Classifier: To
-00000210: 7069 6320 3a3a 2053 6f66 7477 6172 6520  pic :: Software 
-00000220: 4465 7665 6c6f 706d 656e 7420 3a3a 204c  Development :: L
-00000230: 6962 7261 7269 6573 203a 3a20 5079 7468  ibraries :: Pyth
-00000240: 6f6e 204d 6f64 756c 6573 0d0a 436c 6173  on Modules..Clas
-00000250: 7369 6669 6572 3a20 4c69 6365 6e73 6520  sifier: License 
-00000260: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
-00000270: 3a3a 204d 4954 204c 6963 656e 7365 0d0a  :: MIT License..
-00000280: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-00000290: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-000002a0: 203a 3a20 5079 7468 6f6e 203a 3a20 330d   :: Python :: 3.
-000002b0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-000002c0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000002d0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000002e0: 2e38 0d0a 436c 6173 7369 6669 6572 3a20  .8..Classifier: 
-000002f0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000300: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000310: 3a20 332e 390d 0a43 6c61 7373 6966 6965  : 3.9..Classifie
-00000320: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000330: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000340: 6e20 3a3a 2033 2e31 300d 0a43 6c61 7373  n :: 3.10..Class
-00000350: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00000360: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000370: 7974 686f 6e20 3a3a 2033 2e31 310d 0a52  ython :: 3.11..R
-00000380: 6571 7569 7265 732d 5079 7468 6f6e 3a20  equires-Python: 
-00000390: 3e3d 332e 380d 0a44 6573 6372 6970 7469  >=3.8..Descripti
-000003a0: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
-000003b0: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
-000003c0: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
-000003d0: 4345 4e53 450d 0a0d 0a3c 7020 616c 6967  CENSE....<p alig
-000003e0: 6e3d 2263 656e 7465 7222 3e0d 0a20 20f0  n="center">..  .
-000003f0: 9f8c 8f0d 0a20 203c 6120 6872 6566 3d22  .....  <a href="
-00000400: 5245 4144 4d45 5f43 482e 6d64 223e e7ae  README_CH.md">..
-00000410: 80e4 bd93 e4b8 ade6 9687 3c2f 613e 0d0a  ..........</a>..
-00000420: 3c2f 703e 0d0a 0d0a 2320 f09f 939c 205f  </p>....# .... _
-00000430: 4375 7374 6f6d 546b 696e 7465 7254 6974  CustomTkinterTit
-00000440: 6c65 6261 725f 0d0a 0d0a 215b 696d 6167  lebar_....![imag
-00000450: 655d 2868 7474 7073 3a2f 2f75 7365 722d  e](https://user-
-00000460: 696d 6167 6573 2e67 6974 6875 6275 7365  images.githubuse
-00000470: 7263 6f6e 7465 6e74 2e63 6f6d 2f37 3131  rcontent.com/711
-00000480: 3539 3634 312f 3230 3832 3331 3839 392d  59641/208231899-
-00000490: 6332 3566 6139 3530 2d35 3766 372d 3461  c25fa950-57f7-4a
-000004a0: 3930 2d38 3039 352d 6363 6561 6462 6636  90-8095-cceadbf6
-000004b0: 6433 3731 2e70 6e67 290d 0a23 2323 20f0  d371.png)..### .
-000004c0: 9f93 8320 2a54 6869 7320 6973 2061 2070  ... *This is a p
-000004d0: 726f 6a65 6374 2063 616e 2068 656c 7020  roject can help 
-000004e0: 796f 7520 746f 2068 6176 6520 6120 6375  you to have a cu
-000004f0: 7374 6f6d 2074 6974 6c65 6261 7221 2057  stom titlebar! W
-00000500: 6964 6765 7473 2063 616e 2061 6464 2069  idgets can add i
-00000510: 6e74 6f20 7469 746c 6562 6172 212a 0d0a  nto titlebar!*..
-00000520: 2323 2323 20e2 9d94 204d 6f72 6520 6162  #### ... More ab
-00000530: 6f75 7420 7468 6973 2070 726f 6a65 6374  out this project
-00000540: 2c20 4920 7772 6f74 6520 616e 2061 7274  , I wrote an art
-00000550: 6963 6c65 206f 6e20 4269 6c69 6269 6c69  icle on Bilibili
-00000560: 2c20 7768 6963 6820 7461 6c6b 7320 6162  , which talks ab
-00000570: 6f75 7420 7468 6973 2070 726f 6a65 6374  out this project
-00000580: 2069 6e20 6d6f 7265 2064 6574 6169 6c3a   in more detail:
-00000590: 205f 2068 7474 7073 3a2f 2f77 7777 2e62   _ https://www.b
-000005a0: 696c 6962 696c 692e 636f 6d2f 7265 6164  ilibili.com/read
-000005b0: 2f63 7632 3035 3538 3437 330d 0a23 2323  /cv20558473..###
-000005c0: 2320 2a48 6f70 6520 676f 7420 736f 6d65  # *Hope got some
-000005d0: 2073 7461 7273 7e2a 0d0a 0d0a 2323 2320   stars~*....### 
-000005e0: f09f 8eb0 2044 656d 6f3a 0d0a 6874 7470  .... Demo:..http
-000005f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6c  s://github.com/l
-00000600: 6974 746c 6577 6869 7465 636c 6f75 642f  ittlewhitecloud/
-00000610: 4375 7374 6f6d 546b 696e 7465 7254 6974  CustomTkinterTit
-00000620: 6c65 6261 722d 4578 616d 706c 6573 0d0a  lebar-Examples..
-00000630: 0d0a 2323 2320 f09f 939a 205f 2a57 696b  ..### .... _*Wik
-00000640: 692a 5f3a 0d0a 2323 2323 2049 6620 796f  i*_:..#### If yo
-00000650: 7527 6420 6c69 6b65 2074 6f20 6b6e 6f77  u'd like to know
-00000660: 2068 6f77 2074 6f20 7573 6520 7468 6520   how to use the 
-00000670: 6675 6e63 7469 6f6e 7320 796f 7520 6361  functions you ca
-00000680: 6e20 6361 6c6c 2c20 7669 7369 7420 7468  n call, visit th
-00000690: 6520 5363 7269 7074 2073 6563 7469 6f6e  e Script section
-000006a0: 206f 6620 7468 6520 4375 7374 6f6d 546b   of the CustomTk
-000006b0: 696e 7465 7254 6974 6c65 6261 7220 7769  interTitlebar wi
-000006c0: 6b69 3a0d 0a68 7474 7073 3a2f 2f67 6974  ki:..https://git
-000006d0: 6875 622e 636f 6d2f 6c69 7474 6c65 7768  hub.com/littlewh
-000006e0: 6974 6563 6c6f 7564 2f43 7573 746f 6d54  itecloud/CustomT
-000006f0: 6b69 6e74 6572 5469 746c 6562 6172 2f77  kinterTitlebar/w
-00000700: 696b 692f 5363 7269 7074 0d0a 0d0a 2323  iki/Script....##
-00000710: 2320 f09f 93a5 2044 6f77 6e6c 6f61 643a  # .... Download:
-00000720: 0d0a 596f 7520 6361 6e20 7573 6520 7069  ..You can use pi
-00000730: 7020 746f 2069 6e73 7461 6c6c 0d0a 6060  p to install..``
-00000740: 6062 6174 6368 0d0a 7069 7020 696e 7374  `batch..pip inst
-00000750: 616c 6c20 4375 7374 6f6d 546b 696e 7465  all CustomTkinte
-00000760: 7254 6974 6c65 6261 723e 3d31 2e30 2e37  rTitlebar>=1.0.7
-00000770: 2e33 0d0a 6060 600d 0a59 6f75 2063 616e  .3..```..You can
-00000780: 2061 6c73 6f20 646f 776e 6c6f 6164 2074   also download t
-00000790: 6865 2063 6f64 6520 6672 6f6d 2067 6974  he code from git
-000007a0: 6875 6220 6f72 2063 6865 636b 2074 6865  hub or check the
-000007b0: 2072 6561 6c61 7365 0d0a 0d0a 2323 2320   realase....### 
-000007c0: 5669 6577 3a20 0d0a 6874 7470 733a 2f2f  View: ..https://
-000007d0: 7573 6572 2d69 6d61 6765 732e 6769 7468  user-images.gith
-000007e0: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
-000007f0: 6d2f 3731 3135 3936 3431 2f32 3332 3138  m/71159641/23218
-00000800: 3132 3638 2d63 6632 3064 3232 372d 6430  1268-cf20d227-d0
-00000810: 6264 2d34 3834 302d 3962 3331 2d66 6133  bd-4840-9b31-fa3
-00000820: 6166 3135 3065 3463 382e 6d70 340d 0a23  af150e4c8.mp4..#
-00000830: 2323 2320 696e 7365 7274 2063 6f6d 706f  ### insert compo
-00000840: 6e65 6e74 2074 6f20 7469 746c 6562 6172  nent to titlebar
-00000850: 3a0d 0a21 5b69 6d61 6765 5d28 6874 7470  :..![image](http
-00000860: 733a 2f2f 7573 6572 2d69 6d61 6765 732e  s://user-images.
-00000870: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
-00000880: 742e 636f 6d2f 3731 3135 3936 3431 2f32  t.com/71159641/2
-00000890: 3038 3233 3138 3939 2d63 3235 6661 3935  08231899-c25fa95
-000008a0: 302d 3537 6637 2d34 6139 302d 3830 3935  0-57f7-4a90-8095
-000008b0: 2d63 6365 6164 6266 3664 3337 312e 706e  -cceadbf6d371.pn
-000008c0: 6729 0d0a 2323 2323 2042 6c75 723a 0d0a  g)..#### Blur:..
-000008d0: 215b 696d 6167 655d 2868 7474 7073 3a2f  ![image](https:/
-000008e0: 2f75 7365 722d 696d 6167 6573 2e67 6974  /user-images.git
-000008f0: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00000900: 6f6d 2f37 3131 3539 3634 312f 3231 3533  om/71159641/2153
-00000910: 3138 3932 332d 3532 3163 3565 6664 2d38  18923-521c5efd-8
-00000920: 3536 622d 3432 6562 2d61 6162 382d 3032  56b-42eb-aab8-02
-00000930: 6263 3561 6434 3732 3765 2e70 6e67 290d  bc5ad4727e.png).
-00000940: 0a23 2323 2320 466c 7565 6e74 203a 0d0a  .#### Fluent :..
-00000950: 215b 696d 6167 655d 2868 7474 7073 3a2f  ![image](https:/
-00000960: 2f75 7365 722d 696d 6167 6573 2e67 6974  /user-images.git
-00000970: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00000980: 6f6d 2f37 3131 3539 3634 312f 3231 3533  om/71159641/2153
-00000990: 3138 3932 302d 6135 6263 6531 3139 2d63  18920-a5bce119-c
-000009a0: 3334 332d 3430 6664 2d62 3036 382d 3965  343-40fd-b068-9e
-000009b0: 6362 6534 3434 6136 3066 2e70 6e67 290d  cbe444a60f.png).
-000009c0: 0a23 2323 2069 636f 6e20 2620 7769 6e64  .### icon & wind
-000009d0: 6f77 7465 7874 3a0d 0a21 5b69 6d61 6765  owtext:..![image
-000009e0: 5d28 6874 7470 733a 2f2f 7573 6572 2d69  ](https://user-i
-000009f0: 6d61 6765 732e 6769 7468 7562 7573 6572  mages.githubuser
-00000a00: 636f 6e74 656e 742e 636f 6d2f 3731 3135  content.com/7115
-00000a10: 3936 3431 2f32 3039 3630 3539 3335 2d65  9641/209605935-e
-00000a20: 3832 3437 3063 652d 6530 6432 2d34 3234  82470ce-e0d2-424
-00000a30: 342d 3932 3939 2d64 6263 6636 3636 6337  4-9299-dbcf666c7
-00000a40: 6536 622e 706e 6729 0d0a 215b 696d 6167  e6b.png)..![imag
-00000a50: 655d 2868 7474 7073 3a2f 2f75 7365 722d  e](https://user-
-00000a60: 696d 6167 6573 2e67 6974 6875 6275 7365  images.githubuse
-00000a70: 7263 6f6e 7465 6e74 2e63 6f6d 2f37 3131  rcontent.com/711
-00000a80: 3539 3634 312f 3230 3936 3035 3934 302d  59641/209605940-
-00000a90: 6339 6335 3863 6439 2d36 6666 332d 3434  c9c58cd9-6ff3-44
-00000aa0: 3535 2d39 6637 662d 3232 3936 3131 6136  55-9f7f-229611a6
-00000ab0: 3763 6461 2e70 6e67 290d 0a21 5b69 6d61  7cda.png)..![ima
-00000ac0: 6765 5d28 6874 7470 733a 2f2f 7573 6572  ge](https://user
-00000ad0: 2d69 6d61 6765 732e 6769 7468 7562 7573  -images.githubus
-00000ae0: 6572 636f 6e74 656e 742e 636f 6d2f 3731  ercontent.com/71
-00000af0: 3135 3936 3431 2f32 3039 3630 3539 3431  159641/209605941
-00000b00: 2d64 3338 3733 3264 642d 3139 3137 2d34  -d38732dd-1917-4
-00000b10: 3265 302d 3938 3561 2d65 6261 3938 6532  2e0-985a-eba98e2
-00000b20: 3134 3934 622e 706e 6729 0d0a 2323 2323  1494b.png)..####
-00000b30: 2043 7573 746f 6d20 6d69 6e73 697a 6520   Custom minsize 
-00000b40: 2620 6d61 7873 697a 653a 0d0a 215b 696d  & maxsize:..![im
-00000b50: 6167 655d 2868 7474 7073 3a2f 2f75 7365  age](https://use
-00000b60: 722d 696d 6167 6573 2e67 6974 6875 6275  r-images.githubu
-00000b70: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f37  sercontent.com/7
-00000b80: 3131 3539 3634 312f 3230 3934 3534 3938  1159641/20945498
-00000b90: 332d 6261 3062 6161 3331 2d39 6330 372d  3-ba0baa31-9c07-
-00000ba0: 3435 6265 2d38 6466 662d 3437 6461 3736  45be-8dff-47da76
-00000bb0: 6266 3164 6266 2e70 6e67 290d 0a21 5b69  bf1dbf.png)..![i
-00000bc0: 6d61 6765 5d28 6874 7470 733a 2f2f 7573  mage](https://us
-00000bd0: 6572 2d69 6d61 6765 732e 6769 7468 7562  er-images.github
-00000be0: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00000bf0: 3731 3135 3936 3431 2f32 3039 3435 3439  71159641/2094549
-00000c00: 3834 2d65 3336 3938 6638 392d 3964 3064  84-e3698f89-9d0d
-00000c10: 2d34 6265 312d 3861 6633 2d31 6361 3738  -4be1-8af3-1ca78
-00000c20: 6331 3036 3864 632e 706e 6729 0d0a 215b  c1068dc.png)..![
-00000c30: 696d 6167 655d 2868 7474 7073 3a2f 2f75  image](https://u
-00000c40: 7365 722d 696d 6167 6573 2e67 6974 6875  ser-images.githu
-00000c50: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00000c60: 2f37 3131 3539 3634 312f 3230 3934 3534  /71159641/209454
-00000c70: 3938 352d 3764 3732 3530 3833 2d64 6263  985-7d725083-dbc
-00000c80: 622d 3438 3536 2d38 3865 342d 3230 3061  b-4856-88e4-200a
-00000c90: 3334 3131 3139 3338 2e70 6e67 290d 0a21  34111938.png)..!
-00000ca0: 5b69 6d61 6765 5d28 6874 7470 733a 2f2f  [image](https://
-00000cb0: 7573 6572 2d69 6d61 6765 732e 6769 7468  user-images.gith
-00000cc0: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
-00000cd0: 6d2f 3731 3135 3936 3431 2f32 3039 3435  m/71159641/20945
-00000ce0: 3530 3031 2d66 3438 6330 3736 612d 6361  5001-f48c076a-ca
-00000cf0: 6330 2d34 3331 302d 3937 3565 2d30 6662  c0-4310-975e-0fb
-00000d00: 3634 3835 3566 3463 642e 706e 6729 0d0a  64855f4cd.png)..
-00000d10: 2323 2323 204c 6967 6874 2054 6865 6d65  #### Light Theme
-00000d20: 3a0d 0a21 5b69 6d61 6765 5d28 6874 7470  :..![image](http
-00000d30: 733a 2f2f 7573 6572 2d69 6d61 6765 732e  s://user-images.
-00000d40: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
-00000d50: 742e 636f 6d2f 3731 3135 3936 3431 2f32  t.com/71159641/2
-00000d60: 3130 3238 3338 3633 2d35 3366 3436 3339  10283863-53f4639
-00000d70: 322d 6665 3734 2d34 6434 662d 3839 3339  2-fe74-4d4f-8939
-00000d80: 2d34 6234 3266 3665 3936 6330 622e 706e  -4b42f6e96c0b.pn
-00000d90: 6729 0d0a 215b 696d 6167 655d 2868 7474  g)..![image](htt
-00000da0: 7073 3a2f 2f75 7365 722d 696d 6167 6573  ps://user-images
-00000db0: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-00000dc0: 6e74 2e63 6f6d 2f37 3131 3539 3634 312f  nt.com/71159641/
-00000dd0: 3231 3032 3834 3135 372d 6130 3131 3137  210284157-a01117
-00000de0: 6235 2d32 6161 652d 3434 6366 2d38 3963  b5-2aae-44cf-89c
-00000df0: 652d 6265 3365 6430 3237 3630 3766 2e70  e-be3ed027607f.p
-00000e00: 6e67 290d 0a23 2323 2320 466f 6375 7320  ng)..#### Focus 
-00000e10: 6f6e 3a0d 0a21 5b69 6d61 6765 5d28 6874  on:..![image](ht
-00000e20: 7470 733a 2f2f 7573 6572 2d69 6d61 6765  tps://user-image
-00000e30: 732e 6769 7468 7562 7573 6572 636f 6e74  s.githubusercont
-00000e40: 656e 742e 636f 6d2f 3731 3135 3936 3431  ent.com/71159641
-00000e50: 2f32 3135 3331 3930 3032 2d31 6236 6432  /215319002-1b6d2
-00000e60: 6166 392d 3238 3935 2d34 6665 322d 3830  af9-2895-4fe2-80
-00000e70: 3065 2d36 3337 3736 3166 3038 6666 352e  0e-637761f08ff5.
-00000e80: 706e 6729 0d0a 2323 2323 2046 6f63 7573  png)..#### Focus
-00000e90: 206f 7574 3a0d 0a21 5b69 6d61 6765 5d28   out:..![image](
-00000ea0: 6874 7470 733a 2f2f 7573 6572 2d69 6d61  https://user-ima
-00000eb0: 6765 732e 6769 7468 7562 7573 6572 636f  ges.githubuserco
-00000ec0: 6e74 656e 742e 636f 6d2f 3731 3135 3936  ntent.com/711596
-00000ed0: 3431 2f32 3135 3331 3930 3030 2d33 3163  41/215319000-31c
-00000ee0: 3630 3831 642d 3361 6235 2d34 6361 382d  6081d-3ab5-4ca8-
-00000ef0: 3934 3333 2d61 3830 3333 6131 3532 6161  9433-a8033a152aa
-00000f00: 652e 706e 6729 0d0a 0d0a 2323 2320 f09f  e.png)....### ..
-00000f10: 93a6 2052 6571 7569 7265 3a0d 0a3e 202d  .. Require:..> -
-00000f20: 205f 5769 6e64 6f77 7320 3130 5f0d 0a3e   _Windows 10_..>
-00000f30: 202d 205f 5079 7468 6f6e 203e 3d20 332e   - _Python >= 3.
-00000f40: 382e 305f 0d0a 3e20 2d20 5f54 636c 2f54  8.0_..> - _Tcl/T
-00000f50: 6b20 3e3d 2038 2e36 2e30 5f0d 0a3e 202d  k >= 8.6.0_..> -
-00000f60: 205f 5069 6c6c 6f77 203e 3d20 392e 302e   _Pillow >= 9.0.
-00000f70: 305f 0d0a 3e20 2d20 5f64 6172 6b64 6574  0_..> - _darkdet
-00000f80: 6563 7420 3e3d 2030 2e38 2e30 5f0d 0a3e  ect >= 0.8.0_..>
-00000f90: 202d 205f 426c 7572 5769 6e64 6f77 203e   - _BlurWindow >
-00000fa0: 3d20 312e 322e 315f 2049 6620 796f 7520  = 1.2.1_ If you 
-00000fb0: 646f 6e27 7420 7573 6520 626c 7572 2c20  don't use blur, 
-00000fc0: 796f 7520 6361 6e20 6967 6e6f 7265 2069  you can ignore i
-00000fd0: 740d 0a60 6060 6261 7463 680d 0a70 7974  t..```batch..pyt
-00000fe0: 686f 6e20 2d6d 2070 6970 2069 6e73 7461  hon -m pip insta
-00000ff0: 6c6c 202d 2d75 7067 7261 6465 2070 6970  ll --upgrade pip
-00001000: 0d0a 7069 7020 696e 7374 616c 6c20 7069  ..pip install pi
-00001010: 6c6c 6f77 202d 2d75 7365 720d 0a70 6970  llow --user..pip
-00001020: 2069 6e73 7461 6c6c 2064 6172 6b64 6574   install darkdet
-00001030: 6563 7420 2d2d 7573 6572 0d0a 7069 7020  ect --user..pip 
-00001040: 696e 7374 616c 6c20 426c 7572 5769 6e64  install BlurWind
-00001050: 6f77 202d 2d75 7365 7220 0d0a 6060 600d  ow --user ..```.
-00001060: 0a0d 0a23 2323 20f0 9f93 9620 5573 6167  ...### .... Usag
-00001070: 653a 0d0a 6060 6070 7974 686f 6e0d 0a66  e:..```python..f
-00001080: 726f 6d20 6375 7374 6f6d 746b 696e 7465  rom customtkinte
-00001090: 7274 6974 6c65 6261 7220 696d 706f 7274  rtitlebar import
-000010a0: 2054 6b0d 0a66 726f 6d20 746b 696e 7465   Tk..from tkinte
-000010b0: 7220 696d 706f 7274 2074 746b 0d0a 6578  r import ttk..ex
-000010c0: 616d 706c 6520 3d20 546b 2829 0d0a 6578  ample = Tk()..ex
-000010d0: 616d 706c 652e 7469 746c 6528 2254 6974  ample.title("Tit
-000010e0: 6c65 4261 7222 290d 0a65 7861 6d70 6c65  leBar")..example
-000010f0: 2e67 656f 6d65 7472 7928 2231 3033 3078  .geometry("1030x
-00001100: 3537 3022 290d 0a65 6e20 3d20 7474 6b2e  570")..en = ttk.
-00001110: 456e 7472 7928 6578 616d 706c 652e 7469  Entry(example.ti
-00001120: 746c 6562 6172 290d 0a65 6e2e 7061 636b  tlebar)..en.pack
-00001130: 2866 696c 6c20 3d20 592c 2065 7870 616e  (fill = Y, expan
-00001140: 6420 3d20 5472 7565 2c20 6970 6164 7820  d = True, ipadx 
-00001150: 3d20 3330 2c20 7061 6479 203d 2035 290d  = 30, pady = 5).
-00001160: 0a65 7861 6d70 6c65 2e6d 6169 6e6c 6f6f  .example.mainloo
-00001170: 7028 290d 0a60 6060 0d0a 0d0a 2323 2320  p()..```....### 
-00001180: f09f 92be 2053 7570 706f 7274 3a0d 0a23  .... Support:..#
-00001190: 2323 2320 4974 2073 7570 706f 7274 2057  ### It support W
-000011a0: 696e 646f 7773 2031 3020 3332 202f 2036  indows 10 32 / 6
-000011b0: 3420 6269 7420 6e6f 772e 0d0a 3e20 2a2a  4 bit now...> **
-000011c0: 4d61 7962 6520 6974 2061 6c73 6f20 7375  Maybe it also su
-000011d0: 7070 6f72 7420 5769 6e64 6f77 7320 3131  pport Windows 11
-000011e0: 2c20 4920 616d 2075 7369 6e67 2057 696e  , I am using Win
-000011f0: 646f 7773 2031 302c 2049 2064 6964 6e27  dows 10, I didn'
-00001200: 7420 7465 7374 2074 6869 7320 7072 6f6a  t test this proj
-00001210: 6563 7420 6f6e 2057 696e 646f 7773 2031  ect on Windows 1
-00001220: 3120 7965 742a 2a0d 0a                   1 yet**..
+00000010: 3a20 322e 310a 4e61 6d65 3a20 4375 7374  : 2.1.Name: Cust
+00000020: 6f6d 546b 696e 7465 7254 6974 6c65 6261  omTkinterTitleba
+00000030: 720a 5665 7273 696f 6e3a 2031 2e30 2e37  r.Version: 1.0.7
+00000040: 2e39 0a53 756d 6d61 7279 3a20 5468 6973  .9.Summary: This
+00000050: 2069 7320 6120 f09f 939a 7072 6f6a 6563   is a ....projec
+00000060: 7420 6361 6e20 6865 6c70 2079 6f75 2074  t can help you t
+00000070: 6f20 6861 7665 2061 2063 7573 746f 6d20  o have a custom 
+00000080: 7469 746c 6562 6172 2120 e8bf 99e6 98af  titlebar! ......
+00000090: e4b8 80e4 b8aa e58f afe4 bba5 e588 9be5  ................
+000000a0: bbba e887 aae5 ae9a e4b9 89e6 a087 e9a2  ................
+000000b0: 98e6 a08f e79a 84f0 9f93 9ae9 a1b9 e79b  ................
+000000c0: ae0a 486f 6d65 2d70 6167 653a 2068 7474  ..Home-page: htt
+000000d0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000000e0: 6c69 7474 6c65 7768 6974 6563 6c6f 7564  littlewhitecloud
+000000f0: 2f43 7573 746f 6d54 6b69 6e74 6572 5469  /CustomTkinterTi
+00000100: 746c 6562 6172 0a41 7574 686f 723a 206c  tlebar.Author: l
+00000110: 6974 746c 6577 6869 7465 636c 6f75 640a  ittlewhitecloud.
+00000120: 4175 7468 6f72 2d65 6d61 696c 3a20 7131  Author-email: q1
+00000130: 3134 3139 3236 3634 3740 3136 332e 636f  141926647@163.co
+00000140: 6d0a 436c 6173 7369 6669 6572 3a20 4465  m.Classifier: De
+00000150: 7665 6c6f 706d 656e 7420 5374 6174 7573  velopment Status
+00000160: 203a 3a20 3520 2d20 5072 6f64 7563 7469   :: 5 - Producti
+00000170: 6f6e 2f53 7461 626c 650a 436c 6173 7369  on/Stable.Classi
+00000180: 6669 6572 3a20 496e 7465 6e64 6564 2041  fier: Intended A
+00000190: 7564 6965 6e63 6520 3a3a 2044 6576 656c  udience :: Devel
+000001a0: 6f70 6572 730a 436c 6173 7369 6669 6572  opers.Classifier
+000001b0: 3a20 4c69 6365 6e73 6520 3a3a 204f 5349  : License :: OSI
+000001c0: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
+000001d0: 204c 6963 656e 7365 0a43 6c61 7373 6966   License.Classif
+000001e0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+000001f0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000200: 686f 6e20 3a3a 2033 2e38 0a43 6c61 7373  hon :: 3.8.Class
+00000210: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00000220: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000230: 7974 686f 6e20 3a3a 2033 2e39 0a43 6c61  ython :: 3.9.Cla
+00000240: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+00000250: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000260: 2050 7974 686f 6e20 3a3a 2033 2e31 300a   Python :: 3.10.
+00000270: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000280: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000290: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+000002a0: 3131 0a44 6573 6372 6970 7469 6f6e 2d43  11.Description-C
+000002b0: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
+000002c0: 742f 6d61 726b 646f 776e 0a4c 6963 656e  t/markdown.Licen
+000002d0: 7365 2d46 696c 653a 204c 4943 454e 5345  se-File: LICENSE
+000002e0: 0a0a 2320 5fe8 87aa e5ae 9ae4 b989 e6a0  ..# _...........
+000002f0: 87e9 a298 e6a0 8f5f 205f 4375 7374 6f6d  ......._ _Custom
+00000300: 546b 696e 7465 7254 6974 6c65 6261 725f  TkinterTitlebar_
+00000310: 0a21 5b69 6d61 6765 5d28 6874 7470 733a  .![image](https:
+00000320: 2f2f 6769 7468 7562 2e63 6f6d 2f6c 6974  //github.com/lit
+00000330: 746c 6577 6869 7465 636c 6f75 642f 4375  tlewhitecloud/Cu
+00000340: 7374 6f6d 546b 696e 7465 7254 6974 6c65  stomTkinterTitle
+00000350: 6261 722f 6173 7365 7473 2f37 3131 3539  bar/assets/71159
+00000360: 3634 312f 3330 6637 6337 3835 2d64 3138  641/30f7c785-d18
+00000370: 392d 3438 3635 2d38 3039 352d 3338 3432  9-4865-8095-3842
+00000380: 3539 6539 6234 3139 290a 0a21 5b69 6d61  59e9b419)..![ima
+00000390: 6765 5d28 6874 7470 733a 2f2f 7573 6572  ge](https://user
+000003a0: 2d69 6d61 6765 732e 6769 7468 7562 7573  -images.githubus
+000003b0: 6572 636f 6e74 656e 742e 636f 6d2f 3731  ercontent.com/71
+000003c0: 3135 3936 3431 2f32 3039 3738 3333 3734  159641/209783374
+000003d0: 2d66 3565 6133 3631 332d 6562 3635 2d34  -f5ea3613-eb65-4
+000003e0: 6563 332d 3934 3632 2d30 6562 3738 3833  ec3-9462-0eb7883
+000003f0: 6433 6266 392e 706e 6729 0a21 5b69 6d61  d3bf9.png).![ima
+00000400: 6765 5d28 6874 7470 733a 2f2f 7573 6572  ge](https://user
+00000410: 2d69 6d61 6765 732e 6769 7468 7562 7573  -images.githubus
+00000420: 6572 636f 6e74 656e 742e 636f 6d2f 3731  ercontent.com/71
+00000430: 3135 3936 3431 2f32 3039 3132 3836 3733  159641/209128673
+00000440: 2d39 3361 3666 3164 622d 3636 6136 2d34  -93a6f1db-66a6-4
+00000450: 3636 372d 3962 6437 2d61 3363 3262 6130  667-9bd7-a3c2ba0
+00000460: 3936 6635 632e 706e 6729 0a0a 2323 2320  96f5c.png)..### 
+00000470: f09f 9383 202a e8bf 99e6 98af e4b8 80e4  .... *..........
+00000480: b8aa e9a1 b9e7 9bae e58f afe4 bba5 e5b8  ................
+00000490: aee5 8aa9 e4bd a0e6 8ba5 e69c 89e4 b880  ................
+000004a0: e4b8 aae8 87aa e5ae 9ae4 b989 e79a 84e6  ................
+000004b0: a087 e9a2 98e6 a08f efbc 81e5 b08f e7bb  ................
+000004c0: 84e4 bbb6 e58f afe4 bba5 e8a2 abe6 94be  ................
+000004d0: e588 b0e8 bf99 e4b8 aae6 a087 e9a2 98e6  ................
+000004e0: a08f e987 8ce9 9da2 2a20 2a54 6869 7320  ........* *This 
+000004f0: 6973 2061 2070 726f 6a65 6374 2063 616e  is a project can
+00000500: 2068 656c 7020 796f 7520 746f 2068 6176   help you to hav
+00000510: 6520 6120 6375 7374 6f6d 2074 6974 6c65  e a custom title
+00000520: 6261 7221 2057 6964 6765 7473 2063 616e  bar! Widgets can
+00000530: 2061 6464 2069 6e74 6f20 7469 746c 6562   add into titleb
+00000540: 6172 212a 0a23 2323 2320 5fe5 85b3 e4ba  ar!*.#### _.....
+00000550: 8ee6 9bb4 e5a4 9ae8 bf99 e4b8 aae9 a1b9  ................
+00000560: e79b aeef bc8c e688 91e5 8699 e4ba 86e4  ................
+00000570: b880 e7af 87e6 9687 e7ab a0e5 9ca8 4269  ..............Bi
+00000580: 6c69 6269 6c69 e4b8 8aef bc8c e5ae 83e5  libili..........
+00000590: be88 e8af a6e7 bb86 e79a 84e8 afb4 e4ba  ................
+000005a0: 86e8 bf99 e4b8 aae9 a1b9 e79b ae5f 205f  ............._ _
+000005b0: 4d6f 7265 2061 626f 7574 2074 6869 7320  More about this 
+000005c0: 7072 6f6a 6563 742c 2049 2077 726f 7465  project, I wrote
+000005d0: 2061 6e20 6172 7469 636c 6520 6f6e 2042   an article on B
+000005e0: 696c 6962 696c 692c 2077 6869 6368 2074  ilibili, which t
+000005f0: 616c 6b73 2061 626f 7574 2074 6869 7320  alks about this 
+00000600: 7072 6f6a 6563 7420 696e 206d 6f72 6520  project in more 
+00000610: 6465 7461 696c 3a5f 2068 7474 7073 3a2f  detail:_ https:/
+00000620: 2f77 7777 2e62 696c 6962 696c 692e 636f  /www.bilibili.co
+00000630: 6d2f 7265 6164 2f63 7632 3035 3538 3437  m/read/cv2055847
+00000640: 330a 2323 2323 20e5 a682 e69e 9ce4 bda0  3.#### .........
+00000650: e596 9ce6 aca2 e5ae 83ef bc8c e8af b7e7  ................
+00000660: bb99 e9a2 97e6 989f efbc 8120 6c65 6176  ........... leav
+00000670: 6520 6120 7374 6172 2069 6620 796f 7520  e a star if you 
+00000680: 6c69 6b65 2069 7421 0a0a 2323 2320 e9a2  like it!..### ..
+00000690: 84e8 a788 2056 6965 773a 200a 6874 7470  .... View: .http
+000006a0: 733a 2f2f 7573 6572 2d69 6d61 6765 732e  s://user-images.
+000006b0: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+000006c0: 742e 636f 6d2f 3731 3135 3936 3431 2f32  t.com/71159641/2
+000006d0: 3332 3138 3132 3638 2d63 6632 3064 3232  32181268-cf20d22
+000006e0: 372d 6430 6264 2d34 3834 302d 3962 3331  7-d0bd-4840-9b31
+000006f0: 2d66 6133 6166 3135 3065 3463 382e 6d70  -fa3af150e4c8.mp
+00000700: 340a 2323 2323 20e6 8f92 e585 a5e7 bb84  4.#### .........
+00000710: e4bb b620 496e 7365 7274 2063 6f6d 706f  ... Insert compo
+00000720: 6e65 6e74 2074 6f20 7469 746c 6562 6172  nent to titlebar
+00000730: 3a0a 215b 696d 6167 655d 2868 7474 7073  :.![image](https
+00000740: 3a2f 2f75 7365 722d 696d 6167 6573 2e67  ://user-images.g
+00000750: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00000760: 2e63 6f6d 2f37 3131 3539 3634 312f 3230  .com/71159641/20
+00000770: 3832 3331 3839 392d 6332 3566 6139 3530  8231899-c25fa950
+00000780: 2d35 3766 372d 3461 3930 2d38 3039 352d  -57f7-4a90-8095-
+00000790: 6363 6561 6462 6636 6433 3731 2e70 6e67  cceadbf6d371.png
+000007a0: 290a 2323 2323 20e8 87aa e5ae 9ae4 b989  ).#### .........
+000007b0: e69c 80e5 a4a7 e58c 96e6 9c80 e5b0 8fe5  ................
+000007c0: 8c96 2043 7573 746f 6d20 6d69 6e73 697a  .. Custom minsiz
+000007d0: 6520 2620 6d61 7873 697a 653a 0a21 5b69  e & maxsize:.![i
+000007e0: 6d61 6765 5d28 6874 7470 733a 2f2f 7573  mage](https://us
+000007f0: 6572 2d69 6d61 6765 732e 6769 7468 7562  er-images.github
+00000800: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00000810: 3731 3135 3936 3431 2f32 3039 3435 3439  71159641/2094549
+00000820: 3833 2d62 6130 6261 6133 312d 3963 3037  83-ba0baa31-9c07
+00000830: 2d34 3562 652d 3864 6666 2d34 3764 6137  -45be-8dff-47da7
+00000840: 3662 6631 6462 662e 706e 6729 0a21 5b69  6bf1dbf.png).![i
+00000850: 6d61 6765 5d28 6874 7470 733a 2f2f 7573  mage](https://us
+00000860: 6572 2d69 6d61 6765 732e 6769 7468 7562  er-images.github
+00000870: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00000880: 3731 3135 3936 3431 2f32 3039 3435 3439  71159641/2094549
+00000890: 3834 2d65 3336 3938 6638 392d 3964 3064  84-e3698f89-9d0d
+000008a0: 2d34 6265 312d 3861 6633 2d31 6361 3738  -4be1-8af3-1ca78
+000008b0: 6331 3036 3864 632e 706e 6729 0a21 5b69  c1068dc.png).![i
+000008c0: 6d61 6765 5d28 6874 7470 733a 2f2f 7573  mage](https://us
+000008d0: 6572 2d69 6d61 6765 732e 6769 7468 7562  er-images.github
+000008e0: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+000008f0: 3731 3135 3936 3431 2f32 3039 3435 3439  71159641/2094549
+00000900: 3835 2d37 6437 3235 3038 332d 6462 6362  85-7d725083-dbcb
+00000910: 2d34 3835 362d 3838 6534 2d32 3030 6133  -4856-88e4-200a3
+00000920: 3431 3131 3933 382e 706e 6729 0a21 5b69  4111938.png).![i
+00000930: 6d61 6765 5d28 6874 7470 733a 2f2f 7573  mage](https://us
+00000940: 6572 2d69 6d61 6765 732e 6769 7468 7562  er-images.github
+00000950: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00000960: 3731 3135 3936 3431 2f32 3039 3435 3530  71159641/2094550
+00000970: 3031 2d66 3438 6330 3736 612d 6361 6330  01-f48c076a-cac0
+00000980: 2d34 3331 302d 3937 3565 2d30 6662 3634  -4310-975e-0fb64
+00000990: 3835 3566 3463 642e 706e 6729 0a23 2323  855f4cd.png).###
+000009a0: 2320 e4ba aee4 b8bb e9a2 9820 4c69 6768  # ......... Ligh
+000009b0: 7420 5468 656d 653a 0a21 5b69 6d61 6765  t Theme:.![image
+000009c0: 5d28 6874 7470 733a 2f2f 7573 6572 2d69  ](https://user-i
+000009d0: 6d61 6765 732e 6769 7468 7562 7573 6572  mages.githubuser
+000009e0: 636f 6e74 656e 742e 636f 6d2f 3731 3135  content.com/7115
+000009f0: 3936 3431 2f32 3130 3238 3338 3633 2d35  9641/210283863-5
+00000a00: 3366 3436 3339 322d 6665 3734 2d34 6434  3f46392-fe74-4d4
+00000a10: 662d 3839 3339 2d34 6234 3266 3665 3936  f-8939-4b42f6e96
+00000a20: 6330 622e 706e 6729 0a21 5b69 6d61 6765  c0b.png).![image
+00000a30: 5d28 6874 7470 733a 2f2f 7573 6572 2d69  ](https://user-i
+00000a40: 6d61 6765 732e 6769 7468 7562 7573 6572  mages.githubuser
+00000a50: 636f 6e74 656e 742e 636f 6d2f 3731 3135  content.com/7115
+00000a60: 3936 3431 2f32 3130 3238 3431 3537 2d61  9641/210284157-a
+00000a70: 3031 3131 3762 352d 3261 6165 2d34 3463  01117b5-2aae-44c
+00000a80: 662d 3839 6365 2d62 6533 6564 3032 3736  f-89ce-be3ed0276
+00000a90: 3037 662e 706e 6729 0a23 2323 2320 e881  07f.png).#### ..
+00000aa0: 9ae7 84a6 e592 8ce6 9caa e881 9ae7 84a6  ................
+00000ab0: 2046 6f63 7573 2069 6e20 2620 6f75 743a   Focus in & out:
+00000ac0: 0a21 5b69 6d61 6765 5d28 6874 7470 733a  .![image](https:
+00000ad0: 2f2f 7573 6572 2d69 6d61 6765 732e 6769  //user-images.gi
+00000ae0: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+00000af0: 636f 6d2f 3731 3135 3936 3431 2f32 3335  com/71159641/235
+00000b00: 3334 3838 3837 2d62 6661 3231 3033 352d  348887-bfa21035-
+00000b10: 3534 6230 2d34 3032 312d 3863 3933 2d34  54b0-4021-8c93-4
+00000b20: 6362 3764 3431 6261 3131 612e 706e 6729  cb7d41ba11a.png)
+00000b30: 0a21 5b69 6d61 6765 5d28 6874 7470 733a  .![image](https:
+00000b40: 2f2f 7573 6572 2d69 6d61 6765 732e 6769  //user-images.gi
+00000b50: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+00000b60: 636f 6d2f 3731 3135 3936 3431 2f32 3335  com/71159641/235
+00000b70: 3334 3838 3838 2d38 6665 3264 6535 612d  348888-8fe2de5a-
+00000b80: 6435 6265 2d34 3265 632d 6261 3433 2d66  d5be-42ec-ba43-f
+00000b90: 3938 3364 6439 3363 3833 372e 706e 6729  983dd93c837.png)
+00000ba0: 0a23 2323 2320 e4ba 91e6 af8d 204d 6963  .#### ...... Mic
+00000bb0: 613a 0a21 5b69 6d61 6765 5d28 6874 7470  a:.![image](http
+00000bc0: 733a 2f2f 7573 6572 2d69 6d61 6765 732e  s://user-images.
+00000bd0: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00000be0: 742e 636f 6d2f 3836 3336 3234 3233 2f32  t.com/86362423/2
+00000bf0: 3335 3432 3831 3232 2d33 3334 6430 3563  35428122-334d05c
+00000c00: 322d 3839 3237 2d34 6234 342d 6263 3033  2-8927-4b44-bc03
+00000c10: 2d61 6230 6163 3066 3136 3837 662e 706e  -ab0ac0f1687f.pn
+00000c20: 6729 0a21 5b69 6d61 6765 5d28 6874 7470  g).![image](http
+00000c30: 733a 2f2f 7573 6572 2d69 6d61 6765 732e  s://user-images.
+00000c40: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00000c50: 742e 636f 6d2f 3836 3336 3234 3233 2f32  t.com/86362423/2
+00000c60: 3335 3432 3839 3934 2d36 3863 3334 6339  35428994-68c34c9
+00000c70: 642d 3162 3330 2d34 6339 662d 3861 3634  d-1b30-4c9f-8a64
+00000c80: 2d61 3661 3736 3036 3030 3732 362e 706e  -a6a760600726.pn
+00000c90: 6729 0a23 2323 2320 e6a8 a1e7 b38a 2042  g).#### ...... B
+00000ca0: 6c75 723a 0a21 5b69 6d61 6765 5d28 6874  lur:.![image](ht
+00000cb0: 7470 733a 2f2f 7573 6572 2d69 6d61 6765  tps://user-image
+00000cc0: 732e 6769 7468 7562 7573 6572 636f 6e74  s.githubusercont
+00000cd0: 656e 742e 636f 6d2f 3731 3135 3936 3431  ent.com/71159641
+00000ce0: 2f32 3135 3331 3839 3233 2d35 3231 6335  /215318923-521c5
+00000cf0: 6566 642d 3835 3662 2d34 3265 622d 6161  efd-856b-42eb-aa
+00000d00: 6238 2d30 3262 6335 6164 3437 3237 652e  b8-02bc5ad4727e.
+00000d10: 706e 6729 0a23 2323 2320 e4ba 9ae5 858b  png).#### ......
+00000d20: e58a 9b20 466c 7565 6e74 203a 0a21 5b69  ... Fluent :.![i
+00000d30: 6d61 6765 5d28 6874 7470 733a 2f2f 7573  mage](https://us
+00000d40: 6572 2d69 6d61 6765 732e 6769 7468 7562  er-images.github
+00000d50: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00000d60: 3731 3135 3936 3431 2f32 3135 3331 3839  71159641/2153189
+00000d70: 3230 2d61 3562 6365 3131 392d 6333 3433  20-a5bce119-c343
+00000d80: 2d34 3066 642d 6230 3638 2d39 6563 6265  -40fd-b068-9ecbe
+00000d90: 3434 3461 3630 662e 706e 6729 0a0a 2323  444a60f.png)..##
+00000da0: 2320 f09f 8eb0 20e6 a0b7 e4be 8b20 4578  # .... ...... Ex
+00000db0: 616d 706c 653a 0a68 7474 7073 3a2f 2f67  ample:.https://g
+00000dc0: 6974 6875 622e 636f 6d2f 6c69 7474 6c65  ithub.com/little
+00000dd0: 7768 6974 6563 6c6f 7564 2f43 7573 746f  whitecloud/Custo
+00000de0: 6d54 6b69 6e74 6572 5469 746c 6562 6172  mTkinterTitlebar
+00000df0: 2d45 7861 6d70 6c65 730a 0a23 2323 20f0  -Examples..### .
+00000e00: 9f93 9a20 5f2a e7bb b4e5 9fba 2a5f 205f  ... _*......*_ _
+00000e10: 2a57 696b 692a 5f3a 0a23 2323 2320 6874  *Wiki*_:.#### ht
+00000e20: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000e30: 2f6c 6974 746c 6577 6869 7465 636c 6f75  /littlewhiteclou
+00000e40: 642f 4375 7374 6f6d 546b 696e 7465 7254  d/CustomTkinterT
+00000e50: 6974 6c65 6261 722f 7769 6b69 2f53 6372  itlebar/wiki/Scr
+00000e60: 6970 740a 0a23 2323 20f0 9f93 a520 e4b8  ipt..### .... ..
+00000e70: 8be8 bdbd 2044 6f77 6e6c 6f61 643a 0ae4  .... Download:..
+00000e80: bda0 e58f afe4 bba5 e4bd bfe7 94a8 5069  ..............Pi
+00000e90: 70e6 9da5 e5ae 89e8 a385 2059 6f75 2063  p......... You c
+00000ea0: 616e 2075 7365 2070 6970 2074 6f20 696e  an use pip to in
+00000eb0: 7374 616c 6c0a 6060 6062 6174 6368 0a70  stall.```batch.p
+00000ec0: 6970 2069 6e73 7461 6c6c 2043 7573 746f  ip install Custo
+00000ed0: 6d54 6b69 6e74 6572 5469 746c 6562 6172  mTkinterTitlebar
+00000ee0: 3e3d 312e 302e 372e 330a 6060 600a e4bd  >=1.0.7.3.```...
+00000ef0: a0e4 b99f e58f afe4 bba5 e79b b4e6 8ea5  ................
+00000f00: e4bb 8e67 6974 6875 62e4 b88a e4b8 8be8  ...github.......
+00000f10: bdbd e58e 9fe7 a081 e688 96e6 9fa5 e79c  ................
+00000f20: 8be5 8f91 e5b8 8320 596f 7520 6361 6e20  ....... You can 
+00000f30: 616c 736f 2064 6f77 6e6c 6f61 6420 7468  also download th
+00000f40: 6520 636f 6465 2066 726f 6d20 6769 7468  e code from gith
+00000f50: 7562 206f 7220 6368 6563 6b20 7468 6520  ub or check the 
+00000f60: 7265 616c 6173 650a 2323 2320 f09f 93a6  realase.### ....
+00000f70: 20e4 be9d e8b5 9620 5265 7175 6972 653a   ...... Require:
+00000f80: 0a3e 202d 205f 5769 6e64 6f77 7320 3130  .> - _Windows 10
+00000f90: 5f0a 3e20 2d20 5f50 7974 686f 6e20 3e3d  _.> - _Python >=
+00000fa0: 2033 2e38 2e30 5f0a 3e20 2d20 5f54 636c   3.8.0_.> - _Tcl
+00000fb0: 2f54 6b20 3e3d 2038 2e36 2e30 5f0a 3e20  /Tk >= 8.6.0_.> 
+00000fc0: 2d20 5f50 696c 6c6f 7720 3e3d 2039 2e30  - _Pillow >= 9.0
+00000fd0: 2e30 5f0a 3e20 2d20 5f64 6172 6b64 6574  .0_.> - _darkdet
+00000fe0: 6563 7420 3e3d 2030 2e38 2e30 5f0a 3e20  ect >= 0.8.0_.> 
+00000ff0: 2d20 5f42 6c75 7257 696e 646f 7720 3e3d  - _BlurWindow >=
+00001000: 2031 2e32 2e31 5f0a 6060 6062 6174 6368   1.2.1_.```batch
+00001010: 0a70 7974 686f 6e20 2d6d 2070 6970 2069  .python -m pip i
+00001020: 6e73 7461 6c6c 202d 2d75 7067 7261 6465  nstall --upgrade
+00001030: 2070 6970 0a70 6970 2069 6e73 7461 6c6c   pip.pip install
+00001040: 2070 696c 6c6f 7720 2d2d 7573 6572 0a70   pillow --user.p
+00001050: 6970 2069 6e73 7461 6c6c 2064 6172 6b64  ip install darkd
+00001060: 6574 6563 7420 2d2d 7573 6572 0a70 6970  etect --user.pip
+00001070: 2069 6e73 7461 6c6c 2042 6c75 7257 696e   install BlurWin
+00001080: 646f 7720 2d2d 7573 6572 200a 6060 600a  dow --user .```.
+00001090: e688 96e8 8085 e58f aae8 bf90 e8a1 8c20  ............... 
+000010a0: 4f72 206a 7573 7420 7275 6e0a 6060 6062  Or just run.```b
+000010b0: 6174 6368 0a70 6970 2069 6e73 7461 6c6c  atch.pip install
+000010c0: 2043 7573 746f 6d54 6b69 6e74 6572 5469   CustomTkinterTi
+000010d0: 746c 6562 6172 202d 2d75 7365 720a 6060  tlebar --user.``
+000010e0: 600a 0a23 2323 20f0 9f93 9620 e794 a8e6  `..### .... ....
+000010f0: b395 2055 7361 6765 3a0a 6060 6070 7974  .. Usage:.```pyt
+00001100: 686f 6e0a 6672 6f6d 2063 7573 746f 6d74  hon.from customt
+00001110: 6b69 6e74 6572 7469 746c 6562 6172 2069  kintertitlebar i
+00001120: 6d70 6f72 7420 546b 0a66 726f 6d20 746b  mport Tk.from tk
+00001130: 696e 7465 7220 696d 706f 7274 2074 746b  inter import ttk
+00001140: 0a65 7861 6d70 6c65 203d 2054 6b28 290a  .example = Tk().
+00001150: 6578 616d 706c 652e 7469 746c 6528 2254  example.title("T
+00001160: 6974 6c65 4261 7222 290a 6578 616d 706c  itleBar").exampl
+00001170: 652e 6765 6f6d 6574 7279 2822 3130 3330  e.geometry("1030
+00001180: 7835 3730 2229 0a65 6e20 3d20 7474 6b2e  x570").en = ttk.
+00001190: 456e 7472 7928 6578 616d 706c 652e 7469  Entry(example.ti
+000011a0: 746c 6562 6172 290a 656e 2e70 6163 6b28  tlebar).en.pack(
+000011b0: 6669 6c6c 203d 2059 2c20 6578 7061 6e64  fill = Y, expand
+000011c0: 203d 2054 7275 652c 2069 7061 6478 203d   = True, ipadx =
+000011d0: 2033 302c 2070 6164 7920 3d20 3529 0a65   30, pady = 5).e
+000011e0: 7861 6d70 6c65 2e6d 6169 6e6c 6f6f 7028  xample.mainloop(
+000011f0: 290a 6060 600a 0a23 2323 20f0 9f92 be20  ).```..### .... 
+00001200: e694 afe6 8c81 2053 7570 706f 7274 3a0a  ...... Support:.
+00001210: 2323 2323 20e5 ae83 e78e b0e5 9ca8 e694  #### ...........
+00001220: afe6 8c81 2057 696e 646f 7773 2031 302f  .... Windows 10/
+00001230: 3131 2033 322f 3634 20e4 bd8d 2049 7420  11 32/64 ... It 
+00001240: 7375 7070 6f72 7420 5769 6e64 6f77 7320  support Windows 
+00001250: 3130 2f31 3120 3332 2f36 3420 6269 7473  10/11 32/64 bits
+00001260: 206e 6f77 2e0a 0ae6 849f e8b0 a220 4048   now......... @H
+00001270: 7579 4875 6e67 3134 3038 e88a b1e6 97b6  uyHung1408......
+00001280: e997 b4e6 9da5 e59c a857 696e 646f 7773  .........Windows
+00001290: 3131 e4b8 8ae6 b58b e8af 95e5 ae83 210a  11............!.
+000012a0: 5468 616e 6b73 2040 4875 7948 756e 6731  Thanks @HuyHung1
+000012b0: 3430 3820 666f 7220 7465 7374 696e 6720  408 for testing 
+000012c0: 6974 206f 6e20 7769 6e64 6f77 7320 3131  it on windows 11
+000012d0: 210a                                     !.
```

### Comparing `CustomTkinterTitlebar-1.0.7.8/README.md` & `CustomTkinterTitlebar-1.0.7.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,224 +1,255 @@
-00000000: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
-00000010: 223e 0a20 20f0 9f8c 8f0a 2020 3c61 2068  ">.  .....  <a h
-00000020: 7265 663d 2252 4541 444d 455f 4348 2e6d  ref="README_CH.m
-00000030: 6422 3ee7 ae80 e4bd 93e4 b8ad e696 873c  d">............<
-00000040: 2f61 3e0a 3c2f 703e 0a0a 2320 f09f 939c  /a>.</p>..# ....
-00000050: 205f 4375 7374 6f6d 546b 696e 7465 7254   _CustomTkinterT
-00000060: 6974 6c65 6261 725f 0a0a 215b 696d 6167  itlebar_..![imag
-00000070: 655d 2868 7474 7073 3a2f 2f75 7365 722d  e](https://user-
-00000080: 696d 6167 6573 2e67 6974 6875 6275 7365  images.githubuse
-00000090: 7263 6f6e 7465 6e74 2e63 6f6d 2f37 3131  rcontent.com/711
-000000a0: 3539 3634 312f 3230 3832 3331 3839 392d  59641/208231899-
-000000b0: 6332 3566 6139 3530 2d35 3766 372d 3461  c25fa950-57f7-4a
-000000c0: 3930 2d38 3039 352d 6363 6561 6462 6636  90-8095-cceadbf6
-000000d0: 6433 3731 2e70 6e67 290a 2323 2320 f09f  d371.png).### ..
-000000e0: 9383 202a 5468 6973 2069 7320 6120 7072  .. *This is a pr
-000000f0: 6f6a 6563 7420 6361 6e20 6865 6c70 2079  oject can help y
-00000100: 6f75 2074 6f20 6861 7665 2061 2063 7573  ou to have a cus
-00000110: 746f 6d20 7469 746c 6562 6172 2120 5769  tom titlebar! Wi
-00000120: 6467 6574 7320 6361 6e20 6164 6420 696e  dgets can add in
-00000130: 746f 2074 6974 6c65 6261 7221 2a0a 2323  to titlebar!*.##
-00000140: 2323 20e2 9d94 204d 6f72 6520 6162 6f75  ## ... More abou
-00000150: 7420 7468 6973 2070 726f 6a65 6374 2c20  t this project, 
-00000160: 4920 7772 6f74 6520 616e 2061 7274 6963  I wrote an artic
-00000170: 6c65 206f 6e20 4269 6c69 6269 6c69 2c20  le on Bilibili, 
-00000180: 7768 6963 6820 7461 6c6b 7320 6162 6f75  which talks abou
-00000190: 7420 7468 6973 2070 726f 6a65 6374 2069  t this project i
-000001a0: 6e20 6d6f 7265 2064 6574 6169 6c3a 205f  n more detail: _
-000001b0: 2068 7474 7073 3a2f 2f77 7777 2e62 696c   https://www.bil
-000001c0: 6962 696c 692e 636f 6d2f 7265 6164 2f63  ibili.com/read/c
-000001d0: 7632 3035 3538 3437 330a 2323 2323 202a  v20558473.#### *
-000001e0: 486f 7065 2067 6f74 2073 6f6d 6520 7374  Hope got some st
-000001f0: 6172 737e 2a0a 0a23 2323 20f0 9f8e b020  ars~*..### .... 
-00000200: 4465 6d6f 3a0a 6874 7470 733a 2f2f 6769  Demo:.https://gi
-00000210: 7468 7562 2e63 6f6d 2f6c 6974 746c 6577  thub.com/littlew
-00000220: 6869 7465 636c 6f75 642f 4375 7374 6f6d  hitecloud/Custom
-00000230: 546b 696e 7465 7254 6974 6c65 6261 722d  TkinterTitlebar-
-00000240: 4578 616d 706c 6573 0a0a 2323 2320 f09f  Examples..### ..
-00000250: 939a 205f 2a57 696b 692a 5f3a 0a23 2323  .. _*Wiki*_:.###
-00000260: 2320 4966 2079 6f75 2764 206c 696b 6520  # If you'd like 
-00000270: 746f 206b 6e6f 7720 686f 7720 746f 2075  to know how to u
-00000280: 7365 2074 6865 2066 756e 6374 696f 6e73  se the functions
-00000290: 2079 6f75 2063 616e 2063 616c 6c2c 2076   you can call, v
-000002a0: 6973 6974 2074 6865 2053 6372 6970 7420  isit the Script 
-000002b0: 7365 6374 696f 6e20 6f66 2074 6865 2043  section of the C
-000002c0: 7573 746f 6d54 6b69 6e74 6572 5469 746c  ustomTkinterTitl
-000002d0: 6562 6172 2077 696b 693a 0a68 7474 7073  ebar wiki:.https
-000002e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6c69  ://github.com/li
-000002f0: 7474 6c65 7768 6974 6563 6c6f 7564 2f43  ttlewhitecloud/C
-00000300: 7573 746f 6d54 6b69 6e74 6572 5469 746c  ustomTkinterTitl
-00000310: 6562 6172 2f77 696b 692f 5363 7269 7074  ebar/wiki/Script
-00000320: 0a0a 2323 2320 f09f 93a5 2044 6f77 6e6c  ..### .... Downl
-00000330: 6f61 643a 0a59 6f75 2063 616e 2075 7365  oad:.You can use
-00000340: 2070 6970 2074 6f20 696e 7374 616c 6c0a   pip to install.
-00000350: 6060 6062 6174 6368 0a70 6970 2069 6e73  ```batch.pip ins
-00000360: 7461 6c6c 2043 7573 746f 6d54 6b69 6e74  tall CustomTkint
-00000370: 6572 5469 746c 6562 6172 3e3d 312e 302e  erTitlebar>=1.0.
-00000380: 372e 330a 6060 600a 596f 7520 6361 6e20  7.3.```.You can 
-00000390: 616c 736f 2064 6f77 6e6c 6f61 6420 7468  also download th
-000003a0: 6520 636f 6465 2066 726f 6d20 6769 7468  e code from gith
-000003b0: 7562 206f 7220 6368 6563 6b20 7468 6520  ub or check the 
-000003c0: 7265 616c 6173 650a 0a23 2323 2056 6965  realase..### Vie
-000003d0: 773a 200a 6874 7470 733a 2f2f 7573 6572  w: .https://user
-000003e0: 2d69 6d61 6765 732e 6769 7468 7562 7573  -images.githubus
-000003f0: 6572 636f 6e74 656e 742e 636f 6d2f 3731  ercontent.com/71
-00000400: 3135 3936 3431 2f32 3332 3138 3132 3638  159641/232181268
-00000410: 2d63 6632 3064 3232 372d 6430 6264 2d34  -cf20d227-d0bd-4
-00000420: 3834 302d 3962 3331 2d66 6133 6166 3135  840-9b31-fa3af15
-00000430: 3065 3463 382e 6d70 340a 2323 2323 2069  0e4c8.mp4.#### i
-00000440: 6e73 6572 7420 636f 6d70 6f6e 656e 7420  nsert component 
-00000450: 746f 2074 6974 6c65 6261 723a 0a21 5b69  to titlebar:.![i
-00000460: 6d61 6765 5d28 6874 7470 733a 2f2f 7573  mage](https://us
-00000470: 6572 2d69 6d61 6765 732e 6769 7468 7562  er-images.github
-00000480: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00000490: 3731 3135 3936 3431 2f32 3038 3233 3138  71159641/2082318
-000004a0: 3939 2d63 3235 6661 3935 302d 3537 6637  99-c25fa950-57f7
-000004b0: 2d34 6139 302d 3830 3935 2d63 6365 6164  -4a90-8095-ccead
-000004c0: 6266 3664 3337 312e 706e 6729 0a23 2323  bf6d371.png).###
-000004d0: 2320 426c 7572 3a0a 215b 696d 6167 655d  # Blur:.![image]
-000004e0: 2868 7474 7073 3a2f 2f75 7365 722d 696d  (https://user-im
-000004f0: 6167 6573 2e67 6974 6875 6275 7365 7263  ages.githubuserc
-00000500: 6f6e 7465 6e74 2e63 6f6d 2f37 3131 3539  ontent.com/71159
-00000510: 3634 312f 3231 3533 3138 3932 332d 3532  641/215318923-52
-00000520: 3163 3565 6664 2d38 3536 622d 3432 6562  1c5efd-856b-42eb
-00000530: 2d61 6162 382d 3032 6263 3561 6434 3732  -aab8-02bc5ad472
-00000540: 3765 2e70 6e67 290a 2323 2323 2046 6c75  7e.png).#### Flu
-00000550: 656e 7420 3a0a 215b 696d 6167 655d 2868  ent :.![image](h
-00000560: 7474 7073 3a2f 2f75 7365 722d 696d 6167  ttps://user-imag
-00000570: 6573 2e67 6974 6875 6275 7365 7263 6f6e  es.githubusercon
-00000580: 7465 6e74 2e63 6f6d 2f37 3131 3539 3634  tent.com/7115964
-00000590: 312f 3231 3533 3138 3932 302d 6135 6263  1/215318920-a5bc
-000005a0: 6531 3139 2d63 3334 332d 3430 6664 2d62  e119-c343-40fd-b
-000005b0: 3036 382d 3965 6362 6534 3434 6136 3066  068-9ecbe444a60f
-000005c0: 2e70 6e67 290a 2323 2320 6963 6f6e 2026  .png).### icon &
-000005d0: 2077 696e 646f 7774 6578 743a 0a21 5b69   windowtext:.![i
-000005e0: 6d61 6765 5d28 6874 7470 733a 2f2f 7573  mage](https://us
-000005f0: 6572 2d69 6d61 6765 732e 6769 7468 7562  er-images.github
-00000600: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00000610: 3731 3135 3936 3431 2f32 3039 3630 3539  71159641/2096059
-00000620: 3335 2d65 3832 3437 3063 652d 6530 6432  35-e82470ce-e0d2
-00000630: 2d34 3234 342d 3932 3939 2d64 6263 6636  -4244-9299-dbcf6
-00000640: 3636 6337 6536 622e 706e 6729 0a21 5b69  66c7e6b.png).![i
-00000650: 6d61 6765 5d28 6874 7470 733a 2f2f 7573  mage](https://us
-00000660: 6572 2d69 6d61 6765 732e 6769 7468 7562  er-images.github
-00000670: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00000680: 3731 3135 3936 3431 2f32 3039 3630 3539  71159641/2096059
-00000690: 3430 2d63 3963 3538 6364 392d 3666 6633  40-c9c58cd9-6ff3
-000006a0: 2d34 3435 352d 3966 3766 2d32 3239 3631  -4455-9f7f-22961
-000006b0: 3161 3637 6364 612e 706e 6729 0a21 5b69  1a67cda.png).![i
-000006c0: 6d61 6765 5d28 6874 7470 733a 2f2f 7573  mage](https://us
-000006d0: 6572 2d69 6d61 6765 732e 6769 7468 7562  er-images.github
-000006e0: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-000006f0: 3731 3135 3936 3431 2f32 3039 3630 3539  71159641/2096059
-00000700: 3431 2d64 3338 3733 3264 642d 3139 3137  41-d38732dd-1917
-00000710: 2d34 3265 302d 3938 3561 2d65 6261 3938  -42e0-985a-eba98
-00000720: 6532 3134 3934 622e 706e 6729 0a23 2323  e21494b.png).###
-00000730: 2320 4375 7374 6f6d 206d 696e 7369 7a65  # Custom minsize
-00000740: 2026 206d 6178 7369 7a65 3a0a 215b 696d   & maxsize:.![im
-00000750: 6167 655d 2868 7474 7073 3a2f 2f75 7365  age](https://use
-00000760: 722d 696d 6167 6573 2e67 6974 6875 6275  r-images.githubu
-00000770: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f37  sercontent.com/7
-00000780: 3131 3539 3634 312f 3230 3934 3534 3938  1159641/20945498
-00000790: 332d 6261 3062 6161 3331 2d39 6330 372d  3-ba0baa31-9c07-
-000007a0: 3435 6265 2d38 6466 662d 3437 6461 3736  45be-8dff-47da76
-000007b0: 6266 3164 6266 2e70 6e67 290a 215b 696d  bf1dbf.png).![im
-000007c0: 6167 655d 2868 7474 7073 3a2f 2f75 7365  age](https://use
-000007d0: 722d 696d 6167 6573 2e67 6974 6875 6275  r-images.githubu
-000007e0: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f37  sercontent.com/7
-000007f0: 3131 3539 3634 312f 3230 3934 3534 3938  1159641/20945498
-00000800: 342d 6533 3639 3866 3839 2d39 6430 642d  4-e3698f89-9d0d-
-00000810: 3462 6531 2d38 6166 332d 3163 6137 3863  4be1-8af3-1ca78c
-00000820: 3130 3638 6463 2e70 6e67 290a 215b 696d  1068dc.png).![im
-00000830: 6167 655d 2868 7474 7073 3a2f 2f75 7365  age](https://use
-00000840: 722d 696d 6167 6573 2e67 6974 6875 6275  r-images.githubu
-00000850: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f37  sercontent.com/7
-00000860: 3131 3539 3634 312f 3230 3934 3534 3938  1159641/20945498
-00000870: 352d 3764 3732 3530 3833 2d64 6263 622d  5-7d725083-dbcb-
-00000880: 3438 3536 2d38 3865 342d 3230 3061 3334  4856-88e4-200a34
-00000890: 3131 3139 3338 2e70 6e67 290a 215b 696d  111938.png).![im
-000008a0: 6167 655d 2868 7474 7073 3a2f 2f75 7365  age](https://use
-000008b0: 722d 696d 6167 6573 2e67 6974 6875 6275  r-images.githubu
-000008c0: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f37  sercontent.com/7
-000008d0: 3131 3539 3634 312f 3230 3934 3535 3030  1159641/20945500
-000008e0: 312d 6634 3863 3037 3661 2d63 6163 302d  1-f48c076a-cac0-
-000008f0: 3433 3130 2d39 3735 652d 3066 6236 3438  4310-975e-0fb648
-00000900: 3535 6634 6364 2e70 6e67 290a 2323 2323  55f4cd.png).####
-00000910: 204c 6967 6874 2054 6865 6d65 3a0a 215b   Light Theme:.![
-00000920: 696d 6167 655d 2868 7474 7073 3a2f 2f75  image](https://u
-00000930: 7365 722d 696d 6167 6573 2e67 6974 6875  ser-images.githu
-00000940: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00000950: 2f37 3131 3539 3634 312f 3231 3032 3833  /71159641/210283
-00000960: 3836 332d 3533 6634 3633 3932 2d66 6537  863-53f46392-fe7
-00000970: 342d 3464 3466 2d38 3933 392d 3462 3432  4-4d4f-8939-4b42
-00000980: 6636 6539 3663 3062 2e70 6e67 290a 215b  f6e96c0b.png).![
-00000990: 696d 6167 655d 2868 7474 7073 3a2f 2f75  image](https://u
-000009a0: 7365 722d 696d 6167 6573 2e67 6974 6875  ser-images.githu
-000009b0: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-000009c0: 2f37 3131 3539 3634 312f 3231 3032 3834  /71159641/210284
-000009d0: 3135 372d 6130 3131 3137 6235 2d32 6161  157-a01117b5-2aa
-000009e0: 652d 3434 6366 2d38 3963 652d 6265 3365  e-44cf-89ce-be3e
-000009f0: 6430 3237 3630 3766 2e70 6e67 290a 2323  d027607f.png).##
-00000a00: 2323 2046 6f63 7573 206f 6e3a 0a21 5b69  ## Focus on:.![i
-00000a10: 6d61 6765 5d28 6874 7470 733a 2f2f 7573  mage](https://us
-00000a20: 6572 2d69 6d61 6765 732e 6769 7468 7562  er-images.github
-00000a30: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00000a40: 3731 3135 3936 3431 2f32 3135 3331 3930  71159641/2153190
-00000a50: 3032 2d31 6236 6432 6166 392d 3238 3935  02-1b6d2af9-2895
-00000a60: 2d34 6665 322d 3830 3065 2d36 3337 3736  -4fe2-800e-63776
-00000a70: 3166 3038 6666 352e 706e 6729 0a23 2323  1f08ff5.png).###
-00000a80: 2320 466f 6375 7320 6f75 743a 0a21 5b69  # Focus out:.![i
-00000a90: 6d61 6765 5d28 6874 7470 733a 2f2f 7573  mage](https://us
-00000aa0: 6572 2d69 6d61 6765 732e 6769 7468 7562  er-images.github
-00000ab0: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00000ac0: 3731 3135 3936 3431 2f32 3135 3331 3930  71159641/2153190
-00000ad0: 3030 2d33 3163 3630 3831 642d 3361 6235  00-31c6081d-3ab5
-00000ae0: 2d34 6361 382d 3934 3333 2d61 3830 3333  -4ca8-9433-a8033
-00000af0: 6131 3532 6161 652e 706e 6729 0a0a 2323  a152aae.png)..##
-00000b00: 2320 f09f 93a6 2052 6571 7569 7265 3a0a  # .... Require:.
-00000b10: 3e20 2d20 5f57 696e 646f 7773 2031 305f  > - _Windows 10_
-00000b20: 0a3e 202d 205f 5079 7468 6f6e 203e 3d20  .> - _Python >= 
-00000b30: 332e 382e 305f 0a3e 202d 205f 5463 6c2f  3.8.0_.> - _Tcl/
-00000b40: 546b 203e 3d20 382e 362e 305f 0a3e 202d  Tk >= 8.6.0_.> -
-00000b50: 205f 5069 6c6c 6f77 203e 3d20 392e 302e   _Pillow >= 9.0.
-00000b60: 305f 0a3e 202d 205f 6461 726b 6465 7465  0_.> - _darkdete
-00000b70: 6374 203e 3d20 302e 382e 305f 0a3e 202d  ct >= 0.8.0_.> -
-00000b80: 205f 426c 7572 5769 6e64 6f77 203e 3d20   _BlurWindow >= 
-00000b90: 312e 322e 315f 2049 6620 796f 7520 646f  1.2.1_ If you do
-00000ba0: 6e27 7420 7573 6520 626c 7572 2c20 796f  n't use blur, yo
-00000bb0: 7520 6361 6e20 6967 6e6f 7265 2069 740a  u can ignore it.
-00000bc0: 6060 6062 6174 6368 0a70 7974 686f 6e20  ```batch.python 
-00000bd0: 2d6d 2070 6970 2069 6e73 7461 6c6c 202d  -m pip install -
-00000be0: 2d75 7067 7261 6465 2070 6970 0a70 6970  -upgrade pip.pip
-00000bf0: 2069 6e73 7461 6c6c 2070 696c 6c6f 7720   install pillow 
-00000c00: 2d2d 7573 6572 0a70 6970 2069 6e73 7461  --user.pip insta
-00000c10: 6c6c 2064 6172 6b64 6574 6563 7420 2d2d  ll darkdetect --
-00000c20: 7573 6572 0a70 6970 2069 6e73 7461 6c6c  user.pip install
-00000c30: 2042 6c75 7257 696e 646f 7720 2d2d 7573   BlurWindow --us
-00000c40: 6572 200a 6060 600a 0a23 2323 20f0 9f93  er .```..### ...
-00000c50: 9620 5573 6167 653a 0a60 6060 7079 7468  . Usage:.```pyth
-00000c60: 6f6e 0a66 726f 6d20 6375 7374 6f6d 746b  on.from customtk
-00000c70: 696e 7465 7274 6974 6c65 6261 7220 696d  intertitlebar im
-00000c80: 706f 7274 2054 6b0a 6672 6f6d 2074 6b69  port Tk.from tki
-00000c90: 6e74 6572 2069 6d70 6f72 7420 7474 6b0a  nter import ttk.
-00000ca0: 6578 616d 706c 6520 3d20 546b 2829 0a65  example = Tk().e
-00000cb0: 7861 6d70 6c65 2e74 6974 6c65 2822 5469  xample.title("Ti
-00000cc0: 746c 6542 6172 2229 0a65 7861 6d70 6c65  tleBar").example
-00000cd0: 2e67 656f 6d65 7472 7928 2231 3033 3078  .geometry("1030x
-00000ce0: 3537 3022 290a 656e 203d 2074 746b 2e45  570").en = ttk.E
-00000cf0: 6e74 7279 2865 7861 6d70 6c65 2e74 6974  ntry(example.tit
-00000d00: 6c65 6261 7229 0a65 6e2e 7061 636b 2866  lebar).en.pack(f
-00000d10: 696c 6c20 3d20 592c 2065 7870 616e 6420  ill = Y, expand 
-00000d20: 3d20 5472 7565 2c20 6970 6164 7820 3d20  = True, ipadx = 
-00000d30: 3330 2c20 7061 6479 203d 2035 290a 6578  30, pady = 5).ex
-00000d40: 616d 706c 652e 6d61 696e 6c6f 6f70 2829  ample.mainloop()
-00000d50: 0a60 6060 0a0a 2323 2320 f09f 92be 2053  .```..### .... S
-00000d60: 7570 706f 7274 3a0a 2323 2323 2049 7420  upport:.#### It 
-00000d70: 7375 7070 6f72 7420 5769 6e64 6f77 7320  support Windows 
-00000d80: 3130 2033 3220 2f20 3634 2062 6974 206e  10 32 / 64 bit n
-00000d90: 6f77 2e0a 3e20 2a2a 4d61 7962 6520 6974  ow..> **Maybe it
-00000da0: 2061 6c73 6f20 7375 7070 6f72 7420 5769   also support Wi
-00000db0: 6e64 6f77 7320 3131 2c20 4920 616d 2075  ndows 11, I am u
-00000dc0: 7369 6e67 2057 696e 646f 7773 2031 302c  sing Windows 10,
-00000dd0: 2049 2064 6964 6e27 7420 7465 7374 2074   I didn't test t
-00000de0: 6869 7320 7072 6f6a 6563 7420 6f6e 2057  his project on W
-00000df0: 696e 646f 7773 2031 3120 7965 742a 2a0a  indows 11 yet**.
+00000000: 2320 5fe8 87aa e5ae 9ae4 b989 e6a0 87e9  # _.............
+00000010: a298 e6a0 8f5f 205f 4375 7374 6f6d 546b  ....._ _CustomTk
+00000020: 696e 7465 7254 6974 6c65 6261 725f 0a21  interTitlebar_.!
+00000030: 5b69 6d61 6765 5d28 6874 7470 733a 2f2f  [image](https://
+00000040: 6769 7468 7562 2e63 6f6d 2f6c 6974 746c  github.com/littl
+00000050: 6577 6869 7465 636c 6f75 642f 4375 7374  ewhitecloud/Cust
+00000060: 6f6d 546b 696e 7465 7254 6974 6c65 6261  omTkinterTitleba
+00000070: 722f 6173 7365 7473 2f37 3131 3539 3634  r/assets/7115964
+00000080: 312f 3330 6637 6337 3835 2d64 3138 392d  1/30f7c785-d189-
+00000090: 3438 3635 2d38 3039 352d 3338 3432 3539  4865-8095-384259
+000000a0: 6539 6234 3139 290a 0a21 5b69 6d61 6765  e9b419)..![image
+000000b0: 5d28 6874 7470 733a 2f2f 7573 6572 2d69  ](https://user-i
+000000c0: 6d61 6765 732e 6769 7468 7562 7573 6572  mages.githubuser
+000000d0: 636f 6e74 656e 742e 636f 6d2f 3731 3135  content.com/7115
+000000e0: 3936 3431 2f32 3039 3738 3333 3734 2d66  9641/209783374-f
+000000f0: 3565 6133 3631 332d 6562 3635 2d34 6563  5ea3613-eb65-4ec
+00000100: 332d 3934 3632 2d30 6562 3738 3833 6433  3-9462-0eb7883d3
+00000110: 6266 392e 706e 6729 0a21 5b69 6d61 6765  bf9.png).![image
+00000120: 5d28 6874 7470 733a 2f2f 7573 6572 2d69  ](https://user-i
+00000130: 6d61 6765 732e 6769 7468 7562 7573 6572  mages.githubuser
+00000140: 636f 6e74 656e 742e 636f 6d2f 3731 3135  content.com/7115
+00000150: 3936 3431 2f32 3039 3132 3836 3733 2d39  9641/209128673-9
+00000160: 3361 3666 3164 622d 3636 6136 2d34 3636  3a6f1db-66a6-466
+00000170: 372d 3962 6437 2d61 3363 3262 6130 3936  7-9bd7-a3c2ba096
+00000180: 6635 632e 706e 6729 0a0a 2323 2320 f09f  f5c.png)..### ..
+00000190: 9383 202a e8bf 99e6 98af e4b8 80e4 b8aa  .. *............
+000001a0: e9a1 b9e7 9bae e58f afe4 bba5 e5b8 aee5  ................
+000001b0: 8aa9 e4bd a0e6 8ba5 e69c 89e4 b880 e4b8  ................
+000001c0: aae8 87aa e5ae 9ae4 b989 e79a 84e6 a087  ................
+000001d0: e9a2 98e6 a08f efbc 81e5 b08f e7bb 84e4  ................
+000001e0: bbb6 e58f afe4 bba5 e8a2 abe6 94be e588  ................
+000001f0: b0e8 bf99 e4b8 aae6 a087 e9a2 98e6 a08f  ................
+00000200: e987 8ce9 9da2 2a20 2a54 6869 7320 6973  ......* *This is
+00000210: 2061 2070 726f 6a65 6374 2063 616e 2068   a project can h
+00000220: 656c 7020 796f 7520 746f 2068 6176 6520  elp you to have 
+00000230: 6120 6375 7374 6f6d 2074 6974 6c65 6261  a custom titleba
+00000240: 7221 2057 6964 6765 7473 2063 616e 2061  r! Widgets can a
+00000250: 6464 2069 6e74 6f20 7469 746c 6562 6172  dd into titlebar
+00000260: 212a 0a23 2323 2320 5fe5 85b3 e4ba 8ee6  !*.#### _.......
+00000270: 9bb4 e5a4 9ae8 bf99 e4b8 aae9 a1b9 e79b  ................
+00000280: aeef bc8c e688 91e5 8699 e4ba 86e4 b880  ................
+00000290: e7af 87e6 9687 e7ab a0e5 9ca8 4269 6c69  ............Bili
+000002a0: 6269 6c69 e4b8 8aef bc8c e5ae 83e5 be88  bili............
+000002b0: e8af a6e7 bb86 e79a 84e8 afb4 e4ba 86e8  ................
+000002c0: bf99 e4b8 aae9 a1b9 e79b ae5f 205f 4d6f  ..........._ _Mo
+000002d0: 7265 2061 626f 7574 2074 6869 7320 7072  re about this pr
+000002e0: 6f6a 6563 742c 2049 2077 726f 7465 2061  oject, I wrote a
+000002f0: 6e20 6172 7469 636c 6520 6f6e 2042 696c  n article on Bil
+00000300: 6962 696c 692c 2077 6869 6368 2074 616c  ibili, which tal
+00000310: 6b73 2061 626f 7574 2074 6869 7320 7072  ks about this pr
+00000320: 6f6a 6563 7420 696e 206d 6f72 6520 6465  oject in more de
+00000330: 7461 696c 3a5f 2068 7474 7073 3a2f 2f77  tail:_ https://w
+00000340: 7777 2e62 696c 6962 696c 692e 636f 6d2f  ww.bilibili.com/
+00000350: 7265 6164 2f63 7632 3035 3538 3437 330a  read/cv20558473.
+00000360: 2323 2323 20e5 a682 e69e 9ce4 bda0 e596  #### ...........
+00000370: 9ce6 aca2 e5ae 83ef bc8c e8af b7e7 bb99  ................
+00000380: e9a2 97e6 989f efbc 8120 6c65 6176 6520  ......... leave 
+00000390: 6120 7374 6172 2069 6620 796f 7520 6c69  a star if you li
+000003a0: 6b65 2069 7421 0a0a 2323 2320 e9a2 84e8  ke it!..### ....
+000003b0: a788 2056 6965 773a 200a 6874 7470 733a  .. View: .https:
+000003c0: 2f2f 7573 6572 2d69 6d61 6765 732e 6769  //user-images.gi
+000003d0: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+000003e0: 636f 6d2f 3731 3135 3936 3431 2f32 3332  com/71159641/232
+000003f0: 3138 3132 3638 2d63 6632 3064 3232 372d  181268-cf20d227-
+00000400: 6430 6264 2d34 3834 302d 3962 3331 2d66  d0bd-4840-9b31-f
+00000410: 6133 6166 3135 3065 3463 382e 6d70 340a  a3af150e4c8.mp4.
+00000420: 2323 2323 20e6 8f92 e585 a5e7 bb84 e4bb  #### ...........
+00000430: b620 496e 7365 7274 2063 6f6d 706f 6e65  . Insert compone
+00000440: 6e74 2074 6f20 7469 746c 6562 6172 3a0a  nt to titlebar:.
+00000450: 215b 696d 6167 655d 2868 7474 7073 3a2f  ![image](https:/
+00000460: 2f75 7365 722d 696d 6167 6573 2e67 6974  /user-images.git
+00000470: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00000480: 6f6d 2f37 3131 3539 3634 312f 3230 3832  om/71159641/2082
+00000490: 3331 3839 392d 6332 3566 6139 3530 2d35  31899-c25fa950-5
+000004a0: 3766 372d 3461 3930 2d38 3039 352d 6363  7f7-4a90-8095-cc
+000004b0: 6561 6462 6636 6433 3731 2e70 6e67 290a  eadbf6d371.png).
+000004c0: 2323 2323 20e8 87aa e5ae 9ae4 b989 e69c  #### ...........
+000004d0: 80e5 a4a7 e58c 96e6 9c80 e5b0 8fe5 8c96  ................
+000004e0: 2043 7573 746f 6d20 6d69 6e73 697a 6520   Custom minsize 
+000004f0: 2620 6d61 7873 697a 653a 0a21 5b69 6d61  & maxsize:.![ima
+00000500: 6765 5d28 6874 7470 733a 2f2f 7573 6572  ge](https://user
+00000510: 2d69 6d61 6765 732e 6769 7468 7562 7573  -images.githubus
+00000520: 6572 636f 6e74 656e 742e 636f 6d2f 3731  ercontent.com/71
+00000530: 3135 3936 3431 2f32 3039 3435 3439 3833  159641/209454983
+00000540: 2d62 6130 6261 6133 312d 3963 3037 2d34  -ba0baa31-9c07-4
+00000550: 3562 652d 3864 6666 2d34 3764 6137 3662  5be-8dff-47da76b
+00000560: 6631 6462 662e 706e 6729 0a21 5b69 6d61  f1dbf.png).![ima
+00000570: 6765 5d28 6874 7470 733a 2f2f 7573 6572  ge](https://user
+00000580: 2d69 6d61 6765 732e 6769 7468 7562 7573  -images.githubus
+00000590: 6572 636f 6e74 656e 742e 636f 6d2f 3731  ercontent.com/71
+000005a0: 3135 3936 3431 2f32 3039 3435 3439 3834  159641/209454984
+000005b0: 2d65 3336 3938 6638 392d 3964 3064 2d34  -e3698f89-9d0d-4
+000005c0: 6265 312d 3861 6633 2d31 6361 3738 6331  be1-8af3-1ca78c1
+000005d0: 3036 3864 632e 706e 6729 0a21 5b69 6d61  068dc.png).![ima
+000005e0: 6765 5d28 6874 7470 733a 2f2f 7573 6572  ge](https://user
+000005f0: 2d69 6d61 6765 732e 6769 7468 7562 7573  -images.githubus
+00000600: 6572 636f 6e74 656e 742e 636f 6d2f 3731  ercontent.com/71
+00000610: 3135 3936 3431 2f32 3039 3435 3439 3835  159641/209454985
+00000620: 2d37 6437 3235 3038 332d 6462 6362 2d34  -7d725083-dbcb-4
+00000630: 3835 362d 3838 6534 2d32 3030 6133 3431  856-88e4-200a341
+00000640: 3131 3933 382e 706e 6729 0a21 5b69 6d61  11938.png).![ima
+00000650: 6765 5d28 6874 7470 733a 2f2f 7573 6572  ge](https://user
+00000660: 2d69 6d61 6765 732e 6769 7468 7562 7573  -images.githubus
+00000670: 6572 636f 6e74 656e 742e 636f 6d2f 3731  ercontent.com/71
+00000680: 3135 3936 3431 2f32 3039 3435 3530 3031  159641/209455001
+00000690: 2d66 3438 6330 3736 612d 6361 6330 2d34  -f48c076a-cac0-4
+000006a0: 3331 302d 3937 3565 2d30 6662 3634 3835  310-975e-0fb6485
+000006b0: 3566 3463 642e 706e 6729 0a23 2323 2320  5f4cd.png).#### 
+000006c0: e4ba aee4 b8bb e9a2 9820 4c69 6768 7420  ......... Light 
+000006d0: 5468 656d 653a 0a21 5b69 6d61 6765 5d28  Theme:.![image](
+000006e0: 6874 7470 733a 2f2f 7573 6572 2d69 6d61  https://user-ima
+000006f0: 6765 732e 6769 7468 7562 7573 6572 636f  ges.githubuserco
+00000700: 6e74 656e 742e 636f 6d2f 3731 3135 3936  ntent.com/711596
+00000710: 3431 2f32 3130 3238 3338 3633 2d35 3366  41/210283863-53f
+00000720: 3436 3339 322d 6665 3734 2d34 6434 662d  46392-fe74-4d4f-
+00000730: 3839 3339 2d34 6234 3266 3665 3936 6330  8939-4b42f6e96c0
+00000740: 622e 706e 6729 0a21 5b69 6d61 6765 5d28  b.png).![image](
+00000750: 6874 7470 733a 2f2f 7573 6572 2d69 6d61  https://user-ima
+00000760: 6765 732e 6769 7468 7562 7573 6572 636f  ges.githubuserco
+00000770: 6e74 656e 742e 636f 6d2f 3731 3135 3936  ntent.com/711596
+00000780: 3431 2f32 3130 3238 3431 3537 2d61 3031  41/210284157-a01
+00000790: 3131 3762 352d 3261 6165 2d34 3463 662d  117b5-2aae-44cf-
+000007a0: 3839 6365 2d62 6533 6564 3032 3736 3037  89ce-be3ed027607
+000007b0: 662e 706e 6729 0a23 2323 2320 e881 9ae7  f.png).#### ....
+000007c0: 84a6 e592 8ce6 9caa e881 9ae7 84a6 2046  .............. F
+000007d0: 6f63 7573 2069 6e20 2620 6f75 743a 0a21  ocus in & out:.!
+000007e0: 5b69 6d61 6765 5d28 6874 7470 733a 2f2f  [image](https://
+000007f0: 7573 6572 2d69 6d61 6765 732e 6769 7468  user-images.gith
+00000800: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
+00000810: 6d2f 3731 3135 3936 3431 2f32 3335 3334  m/71159641/23534
+00000820: 3838 3837 2d62 6661 3231 3033 352d 3534  8887-bfa21035-54
+00000830: 6230 2d34 3032 312d 3863 3933 2d34 6362  b0-4021-8c93-4cb
+00000840: 3764 3431 6261 3131 612e 706e 6729 0a21  7d41ba11a.png).!
+00000850: 5b69 6d61 6765 5d28 6874 7470 733a 2f2f  [image](https://
+00000860: 7573 6572 2d69 6d61 6765 732e 6769 7468  user-images.gith
+00000870: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
+00000880: 6d2f 3731 3135 3936 3431 2f32 3335 3334  m/71159641/23534
+00000890: 3838 3838 2d38 6665 3264 6535 612d 6435  8888-8fe2de5a-d5
+000008a0: 6265 2d34 3265 632d 6261 3433 2d66 3938  be-42ec-ba43-f98
+000008b0: 3364 6439 3363 3833 372e 706e 6729 0a23  3dd93c837.png).#
+000008c0: 2323 2320 e4ba 91e6 af8d 204d 6963 613a  ### ...... Mica:
+000008d0: 0a21 5b69 6d61 6765 5d28 6874 7470 733a  .![image](https:
+000008e0: 2f2f 7573 6572 2d69 6d61 6765 732e 6769  //user-images.gi
+000008f0: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+00000900: 636f 6d2f 3836 3336 3234 3233 2f32 3335  com/86362423/235
+00000910: 3432 3831 3232 2d33 3334 6430 3563 322d  428122-334d05c2-
+00000920: 3839 3237 2d34 6234 342d 6263 3033 2d61  8927-4b44-bc03-a
+00000930: 6230 6163 3066 3136 3837 662e 706e 6729  b0ac0f1687f.png)
+00000940: 0a21 5b69 6d61 6765 5d28 6874 7470 733a  .![image](https:
+00000950: 2f2f 7573 6572 2d69 6d61 6765 732e 6769  //user-images.gi
+00000960: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+00000970: 636f 6d2f 3836 3336 3234 3233 2f32 3335  com/86362423/235
+00000980: 3432 3839 3934 2d36 3863 3334 6339 642d  428994-68c34c9d-
+00000990: 3162 3330 2d34 6339 662d 3861 3634 2d61  1b30-4c9f-8a64-a
+000009a0: 3661 3736 3036 3030 3732 362e 706e 6729  6a760600726.png)
+000009b0: 0a23 2323 2320 e6a8 a1e7 b38a 2042 6c75  .#### ...... Blu
+000009c0: 723a 0a21 5b69 6d61 6765 5d28 6874 7470  r:.![image](http
+000009d0: 733a 2f2f 7573 6572 2d69 6d61 6765 732e  s://user-images.
+000009e0: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+000009f0: 742e 636f 6d2f 3731 3135 3936 3431 2f32  t.com/71159641/2
+00000a00: 3135 3331 3839 3233 2d35 3231 6335 6566  15318923-521c5ef
+00000a10: 642d 3835 3662 2d34 3265 622d 6161 6238  d-856b-42eb-aab8
+00000a20: 2d30 3262 6335 6164 3437 3237 652e 706e  -02bc5ad4727e.pn
+00000a30: 6729 0a23 2323 2320 e4ba 9ae5 858b e58a  g).#### ........
+00000a40: 9b20 466c 7565 6e74 203a 0a21 5b69 6d61  . Fluent :.![ima
+00000a50: 6765 5d28 6874 7470 733a 2f2f 7573 6572  ge](https://user
+00000a60: 2d69 6d61 6765 732e 6769 7468 7562 7573  -images.githubus
+00000a70: 6572 636f 6e74 656e 742e 636f 6d2f 3731  ercontent.com/71
+00000a80: 3135 3936 3431 2f32 3135 3331 3839 3230  159641/215318920
+00000a90: 2d61 3562 6365 3131 392d 6333 3433 2d34  -a5bce119-c343-4
+00000aa0: 3066 642d 6230 3638 2d39 6563 6265 3434  0fd-b068-9ecbe44
+00000ab0: 3461 3630 662e 706e 6729 0a0a 2323 2320  4a60f.png)..### 
+00000ac0: f09f 8eb0 20e6 a0b7 e4be 8b20 4578 616d  .... ...... Exam
+00000ad0: 706c 653a 0a68 7474 7073 3a2f 2f67 6974  ple:.https://git
+00000ae0: 6875 622e 636f 6d2f 6c69 7474 6c65 7768  hub.com/littlewh
+00000af0: 6974 6563 6c6f 7564 2f43 7573 746f 6d54  itecloud/CustomT
+00000b00: 6b69 6e74 6572 5469 746c 6562 6172 2d45  kinterTitlebar-E
+00000b10: 7861 6d70 6c65 730a 0a23 2323 20f0 9f93  xamples..### ...
+00000b20: 9a20 5f2a e7bb b4e5 9fba 2a5f 205f 2a57  . _*......*_ _*W
+00000b30: 696b 692a 5f3a 0a23 2323 2320 6874 7470  iki*_:.#### http
+00000b40: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6c  s://github.com/l
+00000b50: 6974 746c 6577 6869 7465 636c 6f75 642f  ittlewhitecloud/
+00000b60: 4375 7374 6f6d 546b 696e 7465 7254 6974  CustomTkinterTit
+00000b70: 6c65 6261 722f 7769 6b69 2f53 6372 6970  lebar/wiki/Scrip
+00000b80: 740a 0a23 2323 20f0 9f93 a520 e4b8 8be8  t..### .... ....
+00000b90: bdbd 2044 6f77 6e6c 6f61 643a 0ae4 bda0  .. Download:....
+00000ba0: e58f afe4 bba5 e4bd bfe7 94a8 5069 70e6  ............Pip.
+00000bb0: 9da5 e5ae 89e8 a385 2059 6f75 2063 616e  ........ You can
+00000bc0: 2075 7365 2070 6970 2074 6f20 696e 7374   use pip to inst
+00000bd0: 616c 6c0a 6060 6062 6174 6368 0a70 6970  all.```batch.pip
+00000be0: 2069 6e73 7461 6c6c 2043 7573 746f 6d54   install CustomT
+00000bf0: 6b69 6e74 6572 5469 746c 6562 6172 3e3d  kinterTitlebar>=
+00000c00: 312e 302e 372e 330a 6060 600a e4bd a0e4  1.0.7.3.```.....
+00000c10: b99f e58f afe4 bba5 e79b b4e6 8ea5 e4bb  ................
+00000c20: 8e67 6974 6875 62e4 b88a e4b8 8be8 bdbd  .github.........
+00000c30: e58e 9fe7 a081 e688 96e6 9fa5 e79c 8be5  ................
+00000c40: 8f91 e5b8 8320 596f 7520 6361 6e20 616c  ..... You can al
+00000c50: 736f 2064 6f77 6e6c 6f61 6420 7468 6520  so download the 
+00000c60: 636f 6465 2066 726f 6d20 6769 7468 7562  code from github
+00000c70: 206f 7220 6368 6563 6b20 7468 6520 7265   or check the re
+00000c80: 616c 6173 650a 2323 2320 f09f 93a6 20e4  alase.### .... .
+00000c90: be9d e8b5 9620 5265 7175 6972 653a 0a3e  ..... Require:.>
+00000ca0: 202d 205f 5769 6e64 6f77 7320 3130 5f0a   - _Windows 10_.
+00000cb0: 3e20 2d20 5f50 7974 686f 6e20 3e3d 2033  > - _Python >= 3
+00000cc0: 2e38 2e30 5f0a 3e20 2d20 5f54 636c 2f54  .8.0_.> - _Tcl/T
+00000cd0: 6b20 3e3d 2038 2e36 2e30 5f0a 3e20 2d20  k >= 8.6.0_.> - 
+00000ce0: 5f50 696c 6c6f 7720 3e3d 2039 2e30 2e30  _Pillow >= 9.0.0
+00000cf0: 5f0a 3e20 2d20 5f64 6172 6b64 6574 6563  _.> - _darkdetec
+00000d00: 7420 3e3d 2030 2e38 2e30 5f0a 3e20 2d20  t >= 0.8.0_.> - 
+00000d10: 5f42 6c75 7257 696e 646f 7720 3e3d 2031  _BlurWindow >= 1
+00000d20: 2e32 2e31 5f0a 6060 6062 6174 6368 0a70  .2.1_.```batch.p
+00000d30: 7974 686f 6e20 2d6d 2070 6970 2069 6e73  ython -m pip ins
+00000d40: 7461 6c6c 202d 2d75 7067 7261 6465 2070  tall --upgrade p
+00000d50: 6970 0a70 6970 2069 6e73 7461 6c6c 2070  ip.pip install p
+00000d60: 696c 6c6f 7720 2d2d 7573 6572 0a70 6970  illow --user.pip
+00000d70: 2069 6e73 7461 6c6c 2064 6172 6b64 6574   install darkdet
+00000d80: 6563 7420 2d2d 7573 6572 0a70 6970 2069  ect --user.pip i
+00000d90: 6e73 7461 6c6c 2042 6c75 7257 696e 646f  nstall BlurWindo
+00000da0: 7720 2d2d 7573 6572 200a 6060 600a e688  w --user .```...
+00000db0: 96e8 8085 e58f aae8 bf90 e8a1 8c20 4f72  ............. Or
+00000dc0: 206a 7573 7420 7275 6e0a 6060 6062 6174   just run.```bat
+00000dd0: 6368 0a70 6970 2069 6e73 7461 6c6c 2043  ch.pip install C
+00000de0: 7573 746f 6d54 6b69 6e74 6572 5469 746c  ustomTkinterTitl
+00000df0: 6562 6172 202d 2d75 7365 720a 6060 600a  ebar --user.```.
+00000e00: 0a23 2323 20f0 9f93 9620 e794 a8e6 b395  .### .... ......
+00000e10: 2055 7361 6765 3a0a 6060 6070 7974 686f   Usage:.```pytho
+00000e20: 6e0a 6672 6f6d 2063 7573 746f 6d74 6b69  n.from customtki
+00000e30: 6e74 6572 7469 746c 6562 6172 2069 6d70  ntertitlebar imp
+00000e40: 6f72 7420 546b 0a66 726f 6d20 746b 696e  ort Tk.from tkin
+00000e50: 7465 7220 696d 706f 7274 2074 746b 0a65  ter import ttk.e
+00000e60: 7861 6d70 6c65 203d 2054 6b28 290a 6578  xample = Tk().ex
+00000e70: 616d 706c 652e 7469 746c 6528 2254 6974  ample.title("Tit
+00000e80: 6c65 4261 7222 290a 6578 616d 706c 652e  leBar").example.
+00000e90: 6765 6f6d 6574 7279 2822 3130 3330 7835  geometry("1030x5
+00000ea0: 3730 2229 0a65 6e20 3d20 7474 6b2e 456e  70").en = ttk.En
+00000eb0: 7472 7928 6578 616d 706c 652e 7469 746c  try(example.titl
+00000ec0: 6562 6172 290a 656e 2e70 6163 6b28 6669  ebar).en.pack(fi
+00000ed0: 6c6c 203d 2059 2c20 6578 7061 6e64 203d  ll = Y, expand =
+00000ee0: 2054 7275 652c 2069 7061 6478 203d 2033   True, ipadx = 3
+00000ef0: 302c 2070 6164 7920 3d20 3529 0a65 7861  0, pady = 5).exa
+00000f00: 6d70 6c65 2e6d 6169 6e6c 6f6f 7028 290a  mple.mainloop().
+00000f10: 6060 600a 0a23 2323 20f0 9f92 be20 e694  ```..### .... ..
+00000f20: afe6 8c81 2053 7570 706f 7274 3a0a 2323  .... Support:.##
+00000f30: 2323 20e5 ae83 e78e b0e5 9ca8 e694 afe6  ## .............
+00000f40: 8c81 2057 696e 646f 7773 2031 302f 3131  .. Windows 10/11
+00000f50: 2033 322f 3634 20e4 bd8d 2049 7420 7375   32/64 ... It su
+00000f60: 7070 6f72 7420 5769 6e64 6f77 7320 3130  pport Windows 10
+00000f70: 2f31 3120 3332 2f36 3420 6269 7473 206e  /11 32/64 bits n
+00000f80: 6f77 2e0a 0ae6 849f e8b0 a220 4048 7579  ow......... @Huy
+00000f90: 4875 6e67 3134 3038 e88a b1e6 97b6 e997  Hung1408........
+00000fa0: b4e6 9da5 e59c a857 696e 646f 7773 3131  .......Windows11
+00000fb0: e4b8 8ae6 b58b e8af 95e5 ae83 210a 5468  ............!.Th
+00000fc0: 616e 6b73 2040 4875 7948 756e 6731 3430  anks @HuyHung140
+00000fd0: 3820 666f 7220 7465 7374 696e 6720 6974  8 for testing it
+00000fe0: 206f 6e20 7769 6e64 6f77 7320 3131 210a   on windows 11!.
```

