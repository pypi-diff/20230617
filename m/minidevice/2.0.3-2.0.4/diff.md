# Comparing `tmp/minidevice-2.0.3.tar.gz` & `tmp/minidevice-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minidevice-2.0.3.tar", last modified: Sat Jun 17 14:49:00 2023, max compression
+gzip compressed data, was "minidevice-2.0.4.tar", last modified: Sat Jun 17 15:29:10 2023, max compression
```

## Comparing `minidevice-2.0.3.tar` & `minidevice-2.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 14:49:00.051511 minidevice-2.0.3/
--rw-rw-rw-   0        0        0     2263 2023-06-17 14:49:00.051511 minidevice-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1969 2023-06-17 14:48:33.000000 minidevice-2.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 14:49:00.036788 minidevice-2.0.3/minidevice/
--rw-rw-rw-   0        0        0     2745 2023-06-17 13:52:23.000000 minidevice-2.0.3/minidevice/DroidCast.py
--rw-rw-rw-   0        0        0     2178 2023-06-17 02:36:57.000000 minidevice-2.0.3/minidevice/QueueUtils.py
--rw-rw-rw-   0        0        0      226 2023-06-17 14:47:51.000000 minidevice-2.0.3/minidevice/__init__.py
--rw-rw-rw-   0        0        0    20907 2023-06-17 11:44:42.000000 minidevice-2.0.3/minidevice/adb.py
--rw-rw-rw-   0        0        0    20709 2023-06-17 14:09:56.000000 minidevice-2.0.3/minidevice/images.py
--rw-rw-rw-   0        0        0       27 2023-06-17 05:48:23.000000 minidevice-2.0.3/minidevice/logger.py
--rw-rw-rw-   0        0        0    12786 2023-06-17 06:49:51.000000 minidevice-2.0.3/minidevice/minicap.py
--rw-rw-rw-   0        0        0     1678 2023-06-17 06:50:00.000000 minidevice-2.0.3/minidevice/minitouch.py
--rw-rw-rw-   0        0        0      658 2023-06-17 06:08:54.000000 minidevice-2.0.3/minidevice/screencap.py
--rw-rw-rw-   0        0        0      267 2023-06-17 05:58:10.000000 minidevice-2.0.3/minidevice/touch.py
-drwxrwxrwx   0        0        0        0 2023-06-17 14:49:00.049560 minidevice-2.0.3/minidevice.egg-info/
--rw-rw-rw-   0        0        0     2263 2023-06-17 14:48:59.000000 minidevice-2.0.3/minidevice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2023-06-17 14:48:59.000000 minidevice-2.0.3/minidevice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 14:48:59.000000 minidevice-2.0.3/minidevice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-06-17 14:48:59.000000 minidevice-2.0.3/minidevice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-17 14:48:59.000000 minidevice-2.0.3/minidevice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-17 14:49:00.052487 minidevice-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0      754 2023-06-17 14:47:58.000000 minidevice-2.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 15:29:10.361579 minidevice-2.0.4/
+-rw-rw-rw-   0        0        0     2392 2023-06-17 15:29:10.360183 minidevice-2.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2098 2023-06-17 15:02:43.000000 minidevice-2.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 15:29:10.342630 minidevice-2.0.4/minidevice/
+-rw-rw-rw-   0        0        0     2745 2023-06-17 13:52:23.000000 minidevice-2.0.4/minidevice/DroidCast.py
+-rw-rw-rw-   0        0        0     2178 2023-06-17 02:36:57.000000 minidevice-2.0.4/minidevice/QueueUtils.py
+-rw-rw-rw-   0        0        0      226 2023-06-17 14:47:51.000000 minidevice-2.0.4/minidevice/__init__.py
+-rw-rw-rw-   0        0        0    20907 2023-06-17 11:44:42.000000 minidevice-2.0.4/minidevice/adb.py
+-rw-rw-rw-   0        0        0    20739 2023-06-17 15:28:08.000000 minidevice-2.0.4/minidevice/images.py
+-rw-rw-rw-   0        0        0       27 2023-06-17 05:48:23.000000 minidevice-2.0.4/minidevice/logger.py
+-rw-rw-rw-   0        0        0    12786 2023-06-17 06:49:51.000000 minidevice-2.0.4/minidevice/minicap.py
+-rw-rw-rw-   0        0        0     1678 2023-06-17 06:50:00.000000 minidevice-2.0.4/minidevice/minitouch.py
+-rw-rw-rw-   0        0        0      658 2023-06-17 06:08:54.000000 minidevice-2.0.4/minidevice/screencap.py
+-rw-rw-rw-   0        0        0      267 2023-06-17 05:58:10.000000 minidevice-2.0.4/minidevice/touch.py
+drwxrwxrwx   0        0        0        0 2023-06-17 15:29:10.359184 minidevice-2.0.4/minidevice.egg-info/
+-rw-rw-rw-   0        0        0     2392 2023-06-17 15:29:10.000000 minidevice-2.0.4/minidevice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2023-06-17 15:29:10.000000 minidevice-2.0.4/minidevice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 15:29:10.000000 minidevice-2.0.4/minidevice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-06-17 15:29:10.000000 minidevice-2.0.4/minidevice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-17 15:29:10.000000 minidevice-2.0.4/minidevice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-17 15:29:10.361579 minidevice-2.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      754 2023-06-17 15:28:26.000000 minidevice-2.0.4/setup.py
```

### Comparing `minidevice-2.0.3/PKG-INFO` & `minidevice-2.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 2.0.3
+Version: 2.0.4
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku/minidevice
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Requires-Python: >=3
@@ -46,25 +46,25 @@
 
 加上uiautomator已许久未更新,移除这一方法
 ## requirements
 `opencv-python` [`pyminitouch`](https://github.com/williamfzc/pyminitouch)
 ## 使用实例
 采用抽象类定义截图基类
 
-所以DroidCast,Minicap,ADBcap使用方法一模一样
+所以[DroidCast](https://github.com/rayworks/DroidCast),[Minicap](https://github.com/DeviceFarmer/minicap),ADBcap使用方法一模一样
 ```python
 from minidevice import Minicap
 #创建截图对象
 capdevice = Minicap("127.0.0.1:16834")
 #截图
 cap = capdevice.screen_opencv()
 #截图并保存本地
 capdevice.save_screen()
 ```
-当然minitouh,ADBtouch使用方法一模一样
+当然[minitouh](https://github.com/DeviceFarmer/minitouch),ADBtouch使用方法一模一样
 ```python
 from minidevice import Minitouch
 #创建截图对象
 touchdevice = Minitouch("127.0.0.1:16834")
 #点击
 touchdevice.click(x=101,y=101,duration=150)
 #长按
```

### Comparing `minidevice-2.0.3/README.md` & `minidevice-2.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -34,25 +34,25 @@
 
 加上uiautomator已许久未更新,移除这一方法
 ## requirements
 `opencv-python` [`pyminitouch`](https://github.com/williamfzc/pyminitouch)
 ## 使用实例
 采用抽象类定义截图基类
 
-所以DroidCast,Minicap,ADBcap使用方法一模一样
+所以[DroidCast](https://github.com/rayworks/DroidCast),[Minicap](https://github.com/DeviceFarmer/minicap),ADBcap使用方法一模一样
 ```python
 from minidevice import Minicap
 #创建截图对象
 capdevice = Minicap("127.0.0.1:16834")
 #截图
 cap = capdevice.screen_opencv()
 #截图并保存本地
 capdevice.save_screen()
 ```
-当然minitouh,ADBtouch使用方法一模一样
+当然[minitouh](https://github.com/DeviceFarmer/minitouch),ADBtouch使用方法一模一样
 ```python
 from minidevice import Minitouch
 #创建截图对象
 touchdevice = Minitouch("127.0.0.1:16834")
 #点击
 touchdevice.click(x=101,y=101,duration=150)
 #长按
```

### Comparing `minidevice-2.0.3/minidevice/DroidCast.py` & `minidevice-2.0.4/minidevice/DroidCast.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.3/minidevice/QueueUtils.py` & `minidevice-2.0.4/minidevice/QueueUtils.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.3/minidevice/adb.py` & `minidevice-2.0.4/minidevice/adb.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.3/minidevice/images.py` & `minidevice-2.0.4/minidevice/images.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             algorithm (str, optional): 比较算法. Defaults to 'diff'.
                 algorithm包括:
                     "diff": 差值匹配。与给定颜色的R、G、B差的绝对值之和小于threshold时匹配。
                     "rgb": rgb欧拉距离相似度。与给定颜色color的rgb欧拉距离小于等于threshold时匹配。
                     "rgb+": 加权rgb欧拉距离匹配(LAB Delta E)。
                     "hs": hs欧拉距离匹配。hs为HSV空间的色调值。
         - Returns:
-            (两个颜色是否相似) bool: 
+            (两个颜色是否相似) bool:
         """
         # 差值匹配算法
         if algorithm == "diff":
             r1 = (color1 >> 16) & 0xFF
             g1 = (color1 >> 8) & 0xFF
             b1 = color1 & 0xFF
             r2 = (color2 >> 16) & 0xFF
@@ -131,15 +131,15 @@
         """
         parse_color 解析颜色值为16进制
 
         Args:
             color_str (str): "#112233"
 
         Returns:
-            16进制颜色值 (int): 
+            16进制颜色值 (int):
         """
         color_str = color_str.strip("#")  # 移除字符串开头的 "#"
         red = int(color_str[0:2], 16)  # 提取红色分量并转换为整数
         green = int(color_str[2:4], 16)  # 提取绿色分量并转换为整数
         blue = int(color_str[4:6], 16)  # 提取蓝色分量并转换为整数
         color_value = (red << 16) + (green << 8) + blue  # 将分量组合为整数值
         return color_value
@@ -249,15 +249,15 @@
 def raw2opencv(raw):
     """raw to opencv
 
     Args:
         raw (byte): raw
 
     Returns:
-        opencv格式图像 (np.array): 
+        opencv格式图像 (np.array):
     """
     return cv2.imdecode(np.frombuffer(raw, dtype=np.uint8), cv2.IMREAD_COLOR)
 
 
 class Images:
     def read(path, flag=cv2.IMREAD_COLOR):
         """
@@ -266,27 +266,27 @@
         Args:
             path (str): 图像路径
             flag (int) :
                 - cv2.IMREAD_COLOR (默认)
                 - cv2.IMREAD_GRAYSCALE
 
         Returns:
-            opencv格式图像 (np.array): 
+            opencv格式图像 (np.array):
         """
-        return cv2.imread(path, flags=flag)
+        return cv2.imdecode(np.fromfile(path, dtype=np.uint8), flag)
 
     def load(path):
         """
         load 加载网络图片
 
         Args:
             path (str): 图像路径
 
         Returns:
-            opencv格式图像 (np.array): 
+            opencv格式图像 (np.array):
         """
 
         # 下载图片数据
         response = urllib.request.urlopen(path)
         image_data = response.read()
         return raw2opencv(image_data)
 
@@ -305,27 +305,27 @@
         """
         save 保存图像到路径
 
         Args:
             path (str): 路径
             img (mat): opencv格式图像 默认保存到当前路径下save.png
         """
-        cv2.imwrite(path, img)
+        cv2.imencode(ext=".jpg", img=img)[1].tofile(path)
 
     def pixel(img, x, y):
         """
         pixel 返回图片image在点(x, y)处的像素的RGB值。
 
         Args:
             img (Mat): opencv图像
             x (int): 横坐标
             y (int): 纵坐标
 
         Returns:
-            坐标颜色值 (str): 
+            坐标颜色值 (str):
         """
         b, g, r = img[y, x]
         return "#{:02x}{:02x}{:02x}".format(r, g, b)
 
     def find_color(img, color, region=None, threshold=4):
         """
         find_color 找色功能
@@ -333,16 +333,16 @@
         Args:
             img (mat): opencv格式图像
             color (str): 颜色值字符串
             region (list, optional): [xmin,ymin,xmax,ymax]. Defaults to None.
             threshold (int, optional): 颜色相似度. Defaults to 4.
 
         Returns:
-            x (int): 
-            y (int): 
+            x (int):
+            y (int):
         """
         x_min, y_min, x_max, y_max = region or (0, 0, img.shape[1], img.shape[0])
         img = img[y_min:y_max, x_min:x_max]
         # 将颜色值转换为 RGB 分量值
         r, g, b = np.array([int(color[i : i + 2], 16) for i in (1, 3, 5)])
         # 计算颜色差
         diff = np.abs(img - [b, g, r])
@@ -391,15 +391,15 @@
             colors (list): [(x,y,color),(x,y,color)] x为相对第一个点偏移的坐标值,color为颜色值"#112233"
             region (list, optional): 范围数组[xmin,ymin,xmax,ymax]. Defaults to None.
             threshold (int, optional): 相似度. Defaults to 4.
 
         Returns:
             x (int): 第一个点的横坐标
             y (int): 第一个点的纵坐标
-            
+
         """
         first_color_points = Images.find_all_color(
             img, first_color, region=region, threshold=threshold
         )
         if first_color_points is None:
             return None
         for x0, y0 in first_color_points:
@@ -487,16 +487,16 @@
             region (list, optional): 特征点计算范围[x_min, y_min, x_max, y_max]. Defaults to None.
             scale (int, optional): 图像缩放. Defaults to '1'. 分辨率较大时,计算效率与这个成正比
 
         Raises:
             ValueError: "Invalid feature detection method"
 
         Returns:
-            特征点 (keypoints): 
-            描述值 (descriptors): 
+            特征点 (keypoints):
+            描述值 (descriptors):
         """
         # 转换为灰度图像
         if grayscale:
             if len(img.shape) == 3:
                 img = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
 
         # 选择特征计算方法
```

### Comparing `minidevice-2.0.3/minidevice/minicap.py` & `minidevice-2.0.4/minidevice/minicap.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.3/minidevice/minitouch.py` & `minidevice-2.0.4/minidevice/minitouch.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.3/minidevice/screencap.py` & `minidevice-2.0.4/minidevice/screencap.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.3/minidevice.egg-info/PKG-INFO` & `minidevice-2.0.4/minidevice.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 2.0.3
+Version: 2.0.4
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku/minidevice
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Requires-Python: >=3
@@ -46,25 +46,25 @@
 
 加上uiautomator已许久未更新,移除这一方法
 ## requirements
 `opencv-python` [`pyminitouch`](https://github.com/williamfzc/pyminitouch)
 ## 使用实例
 采用抽象类定义截图基类
 
-所以DroidCast,Minicap,ADBcap使用方法一模一样
+所以[DroidCast](https://github.com/rayworks/DroidCast),[Minicap](https://github.com/DeviceFarmer/minicap),ADBcap使用方法一模一样
 ```python
 from minidevice import Minicap
 #创建截图对象
 capdevice = Minicap("127.0.0.1:16834")
 #截图
 cap = capdevice.screen_opencv()
 #截图并保存本地
 capdevice.save_screen()
 ```
-当然minitouh,ADBtouch使用方法一模一样
+当然[minitouh](https://github.com/DeviceFarmer/minitouch),ADBtouch使用方法一模一样
 ```python
 from minidevice import Minitouch
 #创建截图对象
 touchdevice = Minitouch("127.0.0.1:16834")
 #点击
 touchdevice.click(x=101,y=101,duration=150)
 #长按
```

### Comparing `minidevice-2.0.3/setup.py` & `minidevice-2.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(name='minidevice',
-      version='2.0.3',
+      version='2.0.4',
       description='Android Auto Pypi',
       author='KateTseng',
       author_email='Kate.TsengK@outlook.com',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/NakanoSanku/minidevice',
       license='MIT',
```

