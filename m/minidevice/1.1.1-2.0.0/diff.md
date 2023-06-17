# Comparing `tmp/minidevice-1.1.1.tar.gz` & `tmp/minidevice-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minidevice-1.1.1.tar", last modified: Mon Jun 12 14:21:54 2023, max compression
+gzip compressed data, was "minidevice-2.0.0.tar", last modified: Sat Jun 17 06:56:59 2023, max compression
```

## Comparing `minidevice-1.1.1.tar` & `minidevice-2.0.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 14:21:54.349197 minidevice-1.1.1/
--rw-rw-rw-   0        0        0   181499 2023-06-10 03:07:02.000000 minidevice-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     2838 2023-06-12 14:21:54.347721 minidevice-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2523 2023-06-10 15:30:42.000000 minidevice-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 14:21:54.340355 minidevice-1.1.1/minidevice/
--rw-rw-rw-   0        0        0      141 2023-06-12 12:43:29.000000 minidevice-1.1.1/minidevice/__init__.py
--rw-rw-rw-   0        0        0    13767 2023-06-12 12:55:22.000000 minidevice-1.1.1/minidevice/adb.py
--rw-rw-rw-   0        0        0     2360 2023-06-12 12:45:18.000000 minidevice-1.1.1/minidevice/capture.py
--rw-rw-rw-   0        0        0      285 2023-06-01 04:18:26.000000 minidevice-1.1.1/minidevice/config.py
--rw-rw-rw-   0        0        0     3176 2023-06-12 12:56:12.000000 minidevice-1.1.1/minidevice/device.py
--rw-rw-rw-   0        0        0    19850 2023-06-12 12:44:40.000000 minidevice-1.1.1/minidevice/images.py
--rw-rw-rw-   0        0        0     2291 2023-06-12 12:33:40.000000 minidevice-1.1.1/minidevice/minicap.py
--rw-rw-rw-   0        0        0      666 2023-06-07 15:41:47.000000 minidevice-1.1.1/minidevice/minitouch.py
--rw-rw-rw-   0        0        0     1675 2023-06-12 12:44:55.000000 minidevice-1.1.1/minidevice/wincap.py
-drwxrwxrwx   0        0        0        0 2023-06-12 14:21:54.346211 minidevice-1.1.1/minidevice.egg-info/
--rw-rw-rw-   0        0        0     2838 2023-06-12 14:21:54.000000 minidevice-1.1.1/minidevice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2023-06-12 14:21:54.000000 minidevice-1.1.1/minidevice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 14:21:54.000000 minidevice-1.1.1/minidevice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-06-12 14:21:54.000000 minidevice-1.1.1/minidevice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-12 14:21:54.000000 minidevice-1.1.1/minidevice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 14:21:54.350178 minidevice-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      729 2023-06-12 14:21:38.000000 minidevice-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 06:56:59.764848 minidevice-2.0.0/
+-rw-rw-rw-   0        0        0     1967 2023-06-17 06:56:59.763848 minidevice-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1673 2023-06-17 06:56:51.000000 minidevice-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 06:56:59.749830 minidevice-2.0.0/minidevice/
+-rw-rw-rw-   0        0        0     2178 2023-06-17 02:36:57.000000 minidevice-2.0.0/minidevice/QueueUtils.py
+-rw-rw-rw-   0        0        0      184 2023-06-17 06:51:06.000000 minidevice-2.0.0/minidevice/__init__.py
+-rw-rw-rw-   0        0        0    20912 2023-06-17 06:49:35.000000 minidevice-2.0.0/minidevice/adb.py
+-rw-rw-rw-   0        0        0    20595 2023-06-17 06:00:01.000000 minidevice-2.0.0/minidevice/images.py
+-rw-rw-rw-   0        0        0       27 2023-06-17 05:48:23.000000 minidevice-2.0.0/minidevice/logger.py
+-rw-rw-rw-   0        0        0    12786 2023-06-17 06:49:51.000000 minidevice-2.0.0/minidevice/minicap.py
+-rw-rw-rw-   0        0        0     1678 2023-06-17 06:50:00.000000 minidevice-2.0.0/minidevice/minitouch.py
+-rw-rw-rw-   0        0        0      658 2023-06-17 06:08:54.000000 minidevice-2.0.0/minidevice/screencap.py
+-rw-rw-rw-   0        0        0      267 2023-06-17 05:58:10.000000 minidevice-2.0.0/minidevice/touch.py
+drwxrwxrwx   0        0        0        0 2023-06-17 06:56:59.762831 minidevice-2.0.0/minidevice.egg-info/
+-rw-rw-rw-   0        0        0     1967 2023-06-17 06:56:59.000000 minidevice-2.0.0/minidevice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-06-17 06:56:59.000000 minidevice-2.0.0/minidevice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 06:56:59.000000 minidevice-2.0.0/minidevice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-06-17 06:56:59.000000 minidevice-2.0.0/minidevice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-17 06:56:59.000000 minidevice-2.0.0/minidevice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-17 06:56:59.764848 minidevice-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      729 2023-06-17 06:47:30.000000 minidevice-2.0.0/setup.py
```

### Comparing `minidevice-1.1.1/minidevice/images.py` & `minidevice-2.0.0/minidevice/images.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,133 +1,133 @@
 import math
 import urllib.request
-
 import cv2
 import numpy as np
 
 
-class Colors():
-    BLACK = "#FF000000"#黑色
-    DKGRAY = "#FF444444"#深灰色
-    GRAY = "#FF888888"#灰色
-    LTGRAY = "#FFCCCCCC"#亮灰色
-    WHITE ="#FFFFFFFF"#白色
-    RED = "#FFFF0000"#红色
-    GREEN= "#FF00FF00"#绿色
-    BLUE ="#FF0000FF"#蓝色
-    YELLOW ="#FFFFFF00"#黄色
-    CYAN ="#FF00FFFF"#青色
-    MAGENTA="#FFFF00FF"#品红色
-    TRANSPARENT="#00000000"#透明
+class Colors:
+    BLACK = "#FF000000"  # 黑色
+    DKGRAY = "#FF444444"  # 深灰色
+    GRAY = "#FF888888"  # 灰色
+    LTGRAY = "#FFCCCCCC"  # 亮灰色
+    WHITE = "#FFFFFFFF"  # 白色
+    RED = "#FFFF0000"  # 红色
+    GREEN = "#FF00FF00"  # 绿色
+    BLUE = "#FF0000FF"  # 蓝色
+    YELLOW = "#FFFFFF00"  # 黄色
+    CYAN = "#FF00FFFF"  # 青色
+    MAGENTA = "#FFFF00FF"  # 品红色
+    TRANSPARENT = "#00000000"  # 透明
+
     def to_string(color):
         """
         to_string 16进制转颜色值的字符串
 
         Args:
             color (int): 0xFF112233
 
         Returns:
             str: 返回颜色值的字符串，格式为 "#AARRGGBB"。
         """
         # 将整数RGB颜色值转换为16进制字符串
         hex_color = hex(color)[2:].upper().zfill(8)
         # 将16进制字符串转换为"AARRGGBB"格式的字符串
-        a, r, g, b = [hex_color[i:i+2] for i in range(0, 8, 2)]
+        a, r, g, b = [hex_color[i : i + 2] for i in range(0, 8, 2)]
         return f"#{a}{r}{g}{b}"
-    
+
     def get_red(color):
         """
         get_red 返回颜色color的R通道的值,范围0~255.
 
         Args:
             color (int): 0xFF112233
 
         Returns:
             int: 返回颜色color的R通道的值,范围0~255.
         """
         # 右移24位获取红色通道的值
         red = (color >> 16) & 0xFF
         return red
-    
+
     def get_green(color):
         """
         get_green 返回颜色color的g通道的值,范围0~255.
 
         Args:
             color (int): 0xFF112233
 
         Returns:
             int: 颜色color的g通道的值,范围0~255.
         """
         # 右移24位获取绿色通道的值
         green = (color >> 8) & 0xFF
         return green
-    
+
     def get_blue(color):
         """
         get_blue 返回颜色color的b通道的值,范围0~255.
 
         Args:
             color (int): 0xFF112233
 
         Returns:
             int: 颜色color的b通道的值,范围0~255.
         """
         # 右移24位获取蓝色通道的值
         blue = (color >> 0) & 0xFF
         return blue
 
-    def is_similar(color1, color2, threshold=4, algorithm='diff'):
+    def is_similar(color1, color2, threshold=4, algorithm="diff"):
         """
         is_similar 返回两个颜色是否相似
         Args:
             color1 (int): 16进制颜色值
             color2 (int): 16进制颜色值
             threshold (int, optional): 相似度. Defaults to 4.
             algorithm (str, optional): 比较算法. Defaults to 'diff'.
                 algorithm包括:
                     "diff": 差值匹配。与给定颜色的R、G、B差的绝对值之和小于threshold时匹配。
                     "rgb": rgb欧拉距离相似度。与给定颜色color的rgb欧拉距离小于等于threshold时匹配。
                     "rgb+": 加权rgb欧拉距离匹配(LAB Delta E)。
-                    "hs": hs欧拉距离匹配。hs为HSV空间的色调值。       
+                    "hs": hs欧拉距离匹配。hs为HSV空间的色调值。
         - Returns:
             bool: 返回两个颜色是否相似
         """
         # 差值匹配算法
-        if algorithm == 'diff':
+        if algorithm == "diff":
             r1 = (color1 >> 16) & 0xFF
             g1 = (color1 >> 8) & 0xFF
             b1 = color1 & 0xFF
             r2 = (color2 >> 16) & 0xFF
             g2 = (color2 >> 8) & 0xFF
             b2 = color2 & 0xFF
             diff = abs(r1 - r2) + abs(g1 - g2) + abs(b1 - b2)
-            return (diff <= threshold)
+            return diff <= threshold
         # RGB欧拉距离相似度算法
-        elif algorithm == 'rgb':
+        elif algorithm == "rgb":
             r1 = (color1 >> 16) & 0xFF
             g1 = (color1 >> 8) & 0xFF
             b1 = color1 & 0xFF
             r2 = (color2 >> 16) & 0xFF
             g2 = (color2 >> 8) & 0xFF
             b2 = color2 & 0xFF
             diff = math.sqrt(pow(r1 - r2, 2) + pow(g1 - g2, 2) + pow(b1 - b2, 2))
-            return (diff <= threshold)
+            return diff <= threshold
         # 加权RGB欧拉距离相似度算法
-        elif algorithm == 'rgb+':
+        elif algorithm == "rgb+":
             lab1 = rgb2lab(color1)
             lab2 = rgb2lab(color2)
             diff = deltaE(lab1, lab2)
-            return (diff <= threshold)
+            return diff <= threshold
         # HS欧拉距离相似度算法
-        elif algorithm == 'hs':
+        elif algorithm == "hs":
             hs1 = rgb2hs(color1)
             hs2 = rgb2hs(color2)
             diff = math.sqrt(pow(hs1[0] - hs2[0], 2) + pow(hs1[1] - hs2[1], 2))
-            return (diff <= threshold)
+            return diff <= threshold
         else:
             return False
 
     def parse_color(color_str):
         """
         parse_color 解析颜色值为16进制
 
@@ -140,14 +140,15 @@
         color_str = color_str.strip("#")  # 移除字符串开头的 "#"
         red = int(color_str[0:2], 16)  # 提取红色分量并转换为整数
         green = int(color_str[2:4], 16)  # 提取绿色分量并转换为整数
         blue = int(color_str[4:6], 16)  # 提取蓝色分量并转换为整数
         color_value = (red << 16) + (green << 8) + blue  # 将分量组合为整数值
         return color_value
 
+
 # RGB转LAB
 def rgb2lab(color):
     r = (color >> 16) & 0xFF
     g = (color >> 8) & 0xFF
     b = color & 0xFF
     r = r / 255
     g = g / 255
@@ -167,30 +168,31 @@
     x = r * 0.4124 + g * 0.3576 + b * 0.1805
     y = r * 0.2126 + g * 0.7152 + b * 0.0722
     z = r * 0.0193 + g * 0.1192 + b * 0.9505
     x = x / 0.95047
     y = y / 1.00000
     z = z / 1.08883
     if x > 0.008856:
-        x = pow(x, 1/3)
+        x = pow(x, 1 / 3)
     else:
         x = (7.787 * x) + (16 / 116)
     if y > 0.008856:
-        y = pow(y, 1/3)
+        y = pow(y, 1 / 3)
     else:
         y = (7.787 * y) + (16 / 116)
     if z > 0.008856:
-        z = pow(z, 1/3)
+        z = pow(z, 1 / 3)
     else:
         z = (7.787 * z) + (16 / 116)
     l = (116 * y) - 16
     a = 500 * (x - y)
     b = 200 * (y - z)
     return [l, a, b]
 
+
 # LAB Delta E
 def deltaE(lab1, lab2):
     l1 = lab1[0]
     a1 = lab1[1]
     b1 = lab1[2]
     l2 = lab2[0]
     a2 = lab2[1]
@@ -208,16 +210,19 @@
     kc = 1
     kh = 1
     if l1 < 16:
         sl = (k1 * pow(l1 - 16, 2)) / 100
     if c1 < 16:
         kc = k1 * pow(c1, 2) / 100 + 1
     if dh < 180:
-        kh = k2 * (dh ** 2) / 100 + 1
-    return math.sqrt(pow(dl / (sl * k1), 2) + pow(dc / (kc * kc), 2) + pow(dh / (kh * kh), 2))
+        kh = k2 * (dh**2) / 100 + 1
+    return math.sqrt(
+        pow(dl / (sl * k1), 2) + pow(dc / (kc * kc), 2) + pow(dh / (kh * kh), 2)
+    )
+
 
 # RGB转HS
 def rgb2hs(color):
     r = (color >> 16) & 0xFF
     g = (color >> 8) & 0xFF
     b = color & 0xFF
     r = r / 255
@@ -248,30 +253,31 @@
         raw (byte): raw
 
     Returns:
         mat: opencv格式图像
     """
     return cv2.imdecode(np.frombuffer(raw, dtype=np.uint8), cv2.IMREAD_COLOR)
 
-class Images():
-    def read(path,flag=cv2.IMREAD_COLOR):
+
+class Images:
+    def read(path, flag=cv2.IMREAD_COLOR):
         """
         read 读取图像
 
         Args:
             path (str): 图像路径
-            flag (int) : 
+            flag (int) :
                 - cv2.IMREAD_COLOR (默认)
                 - cv2.IMREAD_GRAYSCALE
 
         Returns:
             mat: opencv格式图像
         """
-        return cv2.imread(path,flags=flag)
-    
+        return cv2.imread(path, flags=flag)
+
     def load(path):
         """
         load 加载网络图片
 
         Args:
             path (str): 图像路径
 
@@ -279,51 +285,51 @@
             mat: opencv格式图像
         """
 
         # 下载图片数据
         response = urllib.request.urlopen(path)
         image_data = response.read()
         return raw2opencv(image_data)
-        
-    def show(img,title=""):
+
+    def show(img, title=""):
         """
         show 显示图像
 
         Args:
             img (mat): opencv格式图像
             title (str, optional): 显示的标题. Defaults to "".
         """
-        cv2.imshow(title,img)
+        cv2.imshow(title, img)
         cv2.waitKey()
 
-    def save(img,path="save.png"):
+    def save(img, path="save.png"):
         """
         save 保存图像到路径
 
         Args:
             path (str): 路径
             img (mat): opencv格式图像 默认保存到当前路径下save.png
         """
-        cv2.imwrite(img,path)
-    
-    def pixel(img,x,y):
+        cv2.imwrite(path, img)
+
+    def pixel(img, x, y):
         """
         pixel 返回图片image在点(x, y)处的像素的RGB值。
 
         Args:
             img (Mat): opencv图像
             x (int): 横坐标
             y (int): 纵坐标
 
         Returns:
             str: 返回坐标颜色值
         """
-        b, g, r = img[y,x]
-        return '#{:02x}{:02x}{:02x}'.format(r, g, b)    
-    
+        b, g, r = img[y, x]
+        return "#{:02x}{:02x}{:02x}".format(r, g, b)
+
     def find_color(img, color, region=None, threshold=4):
         """
         find_color 找色功能
 
         Args:
             img (mat): opencv格式图像
             color (str): 颜色值字符串
@@ -333,23 +339,23 @@
         Returns:
             int: x
             int: y
         """
         x_min, y_min, x_max, y_max = region or (0, 0, img.shape[1], img.shape[0])
         img = img[y_min:y_max, x_min:x_max]
         # 将颜色值转换为 RGB 分量值
-        r, g, b = np.array([int(color[i:i+2], 16) for i in (1, 3, 5)])
+        r, g, b = np.array([int(color[i : i + 2], 16) for i in (1, 3, 5)])
         # 计算颜色差
         diff = np.abs(img - [b, g, r])
         # 判断颜色是否匹配
         match = np.logical_and.reduce(diff <= threshold, axis=2)
         # 获取匹配像素点的坐标
         y, x = np.where(match)
-        return None if len(x) == 0 else x[0]+x_min, y[0]+y_min
-    
+        return None if len(x) == 0 else x[0] + x_min, y[0] + y_min
+
     def find_all_color(img, color, region=None, threshold=4):
         """
         find_all_color 找到全图中所有符合要求的像素点
 
         Args:
             img (mat): opencv格式图像
             color (str): 颜色值字符串
@@ -358,24 +364,28 @@
 
         Returns:
             list: 颜色值所有点[(x,y),(x,y),(x,y)]
         """
         x_min, y_min, x_max, y_max = region or (0, 0, img.shape[1], img.shape[0])
         img = img[y_min:y_max, x_min:x_max]
         # 将颜色值转换为 RGB 分量值
-        r, g, b = np.array([int(color[i:i+2], 16) for i in (1, 3, 5)])
+        r, g, b = np.array([int(color[i : i + 2], 16) for i in (1, 3, 5)])
         # 计算颜色差
         diff = np.abs(img - [b, g, r])
         # 判断颜色是否匹配
         match = np.logical_and.reduce(diff <= threshold, axis=2)
         # 获取匹配像素点的坐标
         y, x = np.where(match)
-        return None if len(x) == 0 else [(x[i]+x_min, y[i]+y_min) for i in range(len(x))]
-            
-    def find_multi_colors(img, first_color, colors,region=None,threshold=4):
+        return (
+            None
+            if len(x) == 0
+            else [(x[i] + x_min, y[i] + y_min) for i in range(len(x))]
+        )
+
+    def find_multi_colors(img, first_color, colors, region=None, threshold=4):
         """
         find_multi_colors 多点找色
 
         Args:
             img (mat): opencv格式图像
             first_color (str): 第一个图像的颜色值
             colors (list): [(x,y,color),(x,y,color)] x为相对第一个点偏移的坐标值,color为颜色值"#112233"
@@ -383,31 +393,31 @@
             threshold (int, optional): 相似度. Defaults to 4.
 
         Returns:
             int: x
             int: y
             第一个点的坐标
         """
-        first_color_points=Images.find_all_color(img,
-                                                 first_color,
-                                                 region=region,
-                                                 threshold=threshold)
+        first_color_points = Images.find_all_color(
+            img, first_color, region=region, threshold=threshold
+        )
         if first_color_points is None:
             return None
-        for x0,y0 in first_color_points:
-            for x,y,target_color in colors:
+        for x0, y0 in first_color_points:
+            for x, y, target_color in colors:
                 if not Colors.is_similar(
-                   Colors.parse_color(target_color),
-                    Colors.parse_color(Images.pixel(img,x+x0,y+y0)),
-                    threshold=threshold):
+                    Colors.parse_color(target_color),
+                    Colors.parse_color(Images.pixel(img, x + x0, y + y0)),
+                    threshold=threshold,
+                ):
                     break
-            return x0,y0
+            return x0, y0
         return None
 
-    def find_image(img, template, threshold=0.8, region=None, level=3,debug=False):
+    def find_image(img, template, threshold=0.8, region=None, level=3, debug=False):
         """
         find_image 模板匹配
 
         Args:
             img (mat): opencv格式图像
             template (mat): opencv格式图像
             threshold (float, optional): 匹配度. Defaults to 0.8.
@@ -417,41 +427,60 @@
         Returns:
             max_loc: (x,y)
         """
         # 设置查找区域
         x_min, y_min, x_max, y_max = region or (0, 0, img.shape[1], img.shape[0])
         img = img[y_min:y_max, x_min:x_max]
 
-        img_array=[img]
-        template_array=[template]
+        img_array = [img]
+        template_array = [template]
 
-        for i in range(1,level):
-            img = cv2.pyrDown(img) 
+        for i in range(1, level):
+            img = cv2.pyrDown(img)
             template = cv2.pyrDown(template)
             img_array.append(img)
             template_array.append(template)
 
-        for i,img_level, template_level in list(zip(range(level),img_array, template_array))[::-1]:
+        for i, img_level, template_level in list(
+            zip(range(level), img_array, template_array)
+        )[::-1]:
             # 匹配模板图像
             res = cv2.matchTemplate(img_level, template_level, cv2.TM_CCOEFF_NORMED)
             # 选择相似度最高的一个结果
             min_val, max_val, min_loc, max_loc = cv2.minMaxLoc(res)
             if max_val > threshold:
                 # 转换坐标系
-                max_loc = (max_loc[0]*(2**i), max_loc[1]*(2**i))
+                max_loc = (max_loc[0] * (2**i), max_loc[1] * (2**i))
                 if region is not None:
                     max_loc = (max_loc[0] + x_min, max_loc[1] + y_min)
                 if debug:
                     copy = img_array[0].copy()
-                    cv2.rectangle(copy,[max_loc[0],max_loc[1],template_array[0].shape[1],template_array[0].shape[0]] , (0, 255, 0), 2)
+                    cv2.rectangle(
+                        copy,
+                        [
+                            max_loc[0],
+                            max_loc[1],
+                            template_array[0].shape[1],
+                            template_array[0].shape[0],
+                        ],
+                        (0, 255, 0),
+                        2,
+                    )
                     Images.save(copy)
-                return max_loc
+                return [
+                    max_loc[0],
+                    max_loc[1],
+                    max_loc[0] + template_array[0].shape[1],
+                    max_loc[1] + template_array[0].shape[0],
+                ]
         return None
-    
-    def detect_and_compute_features(img, grayscale=True, method='SIFT', region=None, scale=1):
+
+    def detect_and_compute_features(
+        img, grayscale=True, method="SIFT", region=None, scale=1
+    ):
         """
         detect_and_compute_features 计算特征点和描述值
 
         Args:
             img (mat): opencv格式图像
             grayscale (bool, optional): 是否灰度化图像. Defaults to True.
             method (str, optional): 特征点计算方法. Defaults to 'SIFT'.
@@ -467,104 +496,119 @@
         """
         # 转换为灰度图像
         if grayscale:
             if len(img.shape) == 3:
                 img = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
 
         # 选择特征计算方法
-        if method == 'SIFT':
+        if method == "SIFT":
             feature_detector = cv2.SIFT_create()
-        elif method == 'ORB':
+        elif method == "ORB":
             feature_detector = cv2.ORB_create()
         else:
             raise ValueError("Invalid feature detection method")
 
         x_min, y_min, x_max, y_max = region or (0, 0, img.shape[1], img.shape[0])
         img = img[y_min:y_max, x_min:x_max]
-        img_new = cv2.resize(img,None,fx=scale,fy=scale)
+        img_new = cv2.resize(img, None, fx=scale, fy=scale)
         keypoints = feature_detector.detect(img_new)
 
         # 调整关键点坐标
         for kp in keypoints:
-            kp.pt = ((kp.pt[0])*(1/scale) , (kp.pt[1])*(1/scale))
+            kp.pt = ((kp.pt[0]) * (1 / scale), (kp.pt[1]) * (1 / scale))
 
         _, descriptors = feature_detector.compute(img, keypoints)
         # img = cv2.drawKeypoints(img,keypoints,img)
         # Images.save(f"{random.randint(8,100)}.png",img)
         # 返回特征信息
         return keypoints, descriptors
-        
-    def match_features(img,template,region=None,threshold = 0.75,method="FLANNBASED",debug=False,scale=1):
+
+    def match_features(
+        img,
+        template,
+        region=None,
+        threshold=0.75,
+        method="FLANNBASED",
+        scale=1,
+        debug=False,
+    ):
         """
-        match_features 特征匹配 
+        match_features 特征匹配
         (计算小图花费不了多少资源,重要的是计算大图特,所以请务必区域特征计算)
         由于orb效果不尽人意,只采用sift计算特征
         计算2400x1080的大图消耗0.6s 500x1080的图消耗0.1s
 
         Args:
             img (mat): opencv格式图像 大图
             template (mat): opencv格式图像 小图
             region (list, optional): 大图特征范围[x_min, y_min, x_max, y_max ]. Defaults to None.
             threshold (float, optional): 相似度. Defaults to 0.75.
             method (str, optional): 特征匹配算法. Defaults to "FLANNBASED".其他可选"BRUTEFORCE","BRUTEFORCE_L1"
-            debug (bool,optional): 调试模式(方框绘制并显示) Defaults to False.
             scale (int, optional): 图像缩放. Defaults to '1'. 分辨率较大时,计算效率与这个成正比
+            debug (bool,optional): 调试模式(方框绘制并显示) Defaults to False.
 
         Raises:
             ValueError: 算法不存在
 
         Returns:
             list: 小图在大图中的范围[x, y, w, h ]
         """
         # 计算关键点和描述符
-        kp_template, des_template = Images.detect_and_compute_features(template,scale=scale)
-        kp_target, des_target = Images.detect_and_compute_features(img,region=region,scale=scale)
+        kp_template, des_template = Images.detect_and_compute_features(
+            template, scale=scale
+        )
+        kp_target, des_target = Images.detect_and_compute_features(
+            img, region=region, scale=scale
+        )
 
         if method == "FLANNBASED":
             matcher = cv2.FlannBasedMatcher()
         elif method == "BRUTEFORCE_L1":
             matcher = cv2.BFMatcher(cv2.NORM_L1)
         elif method == "BRUTEFORCE":
             matcher = cv2.BFMatcher(cv2.NORM_L2)
-        else :
+        else:
             raise ValueError("Invalid matching method provided.")
 
         matches = matcher.knnMatch(des_template, des_target, k=2)
 
         # 应用Lowe的比例测试
         good_matches = []
         for m, n in matches:
             if m.distance < threshold * n.distance:
                 good_matches.append(m)
 
         # 如果找到足够的好匹配，则计算单应性矩阵
         if len(good_matches) > 10:
-            src_pts = np.float32([kp_template[m.queryIdx].pt for m in good_matches]).reshape(-1, 1, 2)
-            dst_pts = np.float32([kp_target[m.trainIdx].pt for m in good_matches]).reshape(-1, 1, 2)
+            src_pts = np.float32(
+                [kp_template[m.queryIdx].pt for m in good_matches]
+            ).reshape(-1, 1, 2)
+            dst_pts = np.float32(
+                [kp_target[m.trainIdx].pt for m in good_matches]
+            ).reshape(-1, 1, 2)
 
             # 计算单应性矩阵
             M, mask = cv2.findHomography(src_pts, dst_pts, cv2.RANSAC, 5.0)
 
             # 将模板图像的角点映射到目标图像中的相应位置
             h, w = template.shape[:2]
-            pts = np.float32([[0, 0], [0, h - 1], [w - 1, h - 1], [w - 1, 0]]).reshape(-1, 1, 2)
+            pts = np.float32([[0, 0], [0, h - 1], [w - 1, h - 1], [w - 1, 0]]).reshape(
+                -1, 1, 2
+            )
             dst = cv2.perspectiveTransform(pts, M)
 
-            x_min, y_min, x_max, y_max = region or (0, 0, img.shape[1], img.shape[0])
+            x_min, y_min, _, _ = region or (0, 0, img.shape[1], img.shape[0])
             # 计算矩形区域坐标
             x, y, w, h = cv2.boundingRect(dst)
             if debug:
-                    copy = img.copy()
-                    cv2.rectangle(copy,[x+x_min,y+y_min,w,h] , (0, 255, 0), 2)
-                    Images.save(copy)
-            return [x+x_min,y+y_min, w, h]
+                copy = img.copy()
+                cv2.rectangle(copy, [x + x_min, y + y_min, w, h], (0, 255, 0), 2)
+                Images.save(copy)
+            return [x + x_min, y + y_min, w + x + x_min, h + y + y_min]
 
         else:
             print("Not enough matches are found - {}/{}".format(len(good_matches), 10))
             return None
 
 
-
-
-
-if __name__=="__main__":
+if __name__ == "__main__":
     pass
```

### Comparing `minidevice-1.1.1/setup.py` & `minidevice-2.0.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(name='minidevice',
-      version='1.1.1',
+      version='2.0.0',
       description='Android Auto Pypi',
       author='KateTseng',
       author_email='Kate.TsengK@outlook.com',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/NakanoSanku/minidevice',
       license='MIT',
```

