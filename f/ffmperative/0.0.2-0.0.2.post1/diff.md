# Comparing `tmp/ffmperative-0.0.2-py3-none-any.whl.zip` & `tmp/ffmperative-0.0.2.post1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 7161 bytes, number of entries: 10
+Zip file size: 7349 bytes, number of entries: 10
 -rw-r--r--  2.0 unx     1004 b- defN 23-Jun-11 20:26 ffmperative/__init__.py
 -rw-r--r--  2.0 unx      824 b- defN 23-Jun-01 03:20 ffmperative/cli.py
--rw-r--r--  2.0 unx    10900 b- defN 23-Jun-17 17:46 ffmperative/tools.py
--rw-r--r--  2.0 unx      466 b- defN 23-Jun-17 16:42 ffmperative/utils.py
--rw-rw-r--  2.0 unx     1065 b- defN 23-Jun-17 18:04 ffmperative-0.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     2589 b- defN 23-Jun-17 18:04 ffmperative-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-17 18:04 ffmperative-0.0.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       46 b- defN 23-Jun-17 18:04 ffmperative-0.0.2.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       12 b- defN 23-Jun-17 18:04 ffmperative-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      813 b- defN 23-Jun-17 18:04 ffmperative-0.0.2.dist-info/RECORD
-10 files, 17811 bytes uncompressed, 5771 bytes compressed:  67.6%
+-rw-r--r--  2.0 unx    11193 b- defN 23-Jun-17 21:19 ffmperative/tools.py
+-rw-r--r--  2.0 unx      466 b- defN 23-Jun-17 18:35 ffmperative/utils.py
+-rw-rw-r--  2.0 unx     1065 b- defN 23-Jun-17 21:20 ffmperative-0.0.2.post1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2595 b- defN 23-Jun-17 21:20 ffmperative-0.0.2.post1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-17 21:20 ffmperative-0.0.2.post1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       46 b- defN 23-Jun-17 21:20 ffmperative-0.0.2.post1.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       12 b- defN 23-Jun-17 21:20 ffmperative-0.0.2.post1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      849 b- defN 23-Jun-17 21:20 ffmperative-0.0.2.post1.dist-info/RECORD
+10 files, 18146 bytes uncompressed, 5887 bytes compressed:  67.6%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: ffmperative/tools.py
 Comment: 
 
 Filename: ffmperative/utils.py
 Comment: 
 
-Filename: ffmperative-0.0.2.dist-info/LICENSE
+Filename: ffmperative-0.0.2.post1.dist-info/LICENSE
 Comment: 
 
-Filename: ffmperative-0.0.2.dist-info/METADATA
+Filename: ffmperative-0.0.2.post1.dist-info/METADATA
 Comment: 
 
-Filename: ffmperative-0.0.2.dist-info/WHEEL
+Filename: ffmperative-0.0.2.post1.dist-info/WHEEL
 Comment: 
 
-Filename: ffmperative-0.0.2.dist-info/entry_points.txt
+Filename: ffmperative-0.0.2.post1.dist-info/entry_points.txt
 Comment: 
 
-Filename: ffmperative-0.0.2.dist-info/top_level.txt
+Filename: ffmperative-0.0.2.post1.dist-info/top_level.txt
 Comment: 
 
-Filename: ffmperative-0.0.2.dist-info/RECORD
+Filename: ffmperative-0.0.2.post1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ffmperative/tools.py

```diff
@@ -223,19 +223,27 @@
     start_time, and end_time. Format start(end)_time: HH:MM:SS
     """
     inputs = ["text", "text", "text", "text"]
     outputs = ["None"]
 
     def __call__(
         self, input_path: str, output_path: str, start_time: str, end_time: str
-    ):
+    ):                                  
         stream = ffmpeg.input(input_path)
-        stream = ffmpeg.trim(stream, start=start_time, end=end_time)
-        stream = ffmpeg.output(stream, output_path)
-        ffmpeg.run(stream)
+        v = stream.trim(start=start_time, end=end_time).setpts("PTS-STARTPTS")         
+        a = stream.filter_("atrim", start=start_time, end=end_time).filter_(
+            "asetpts", "PTS-STARTPTS"    
+        )
+        joined = ffmpeg.concat(v, a, v=1, a=1).node
+        out = ffmpeg.output(          
+            joined[0],
+            joined[1],
+            output_path,
+        )
+        out.run()
 
 
 class VideoFadeInTool(Tool):
     name = "video_fade_in_tool"
     description = """
     This tool applies a fade-in effect to a video.
     Inputs are input_path, output_path, fade_duration.
```

## Comparing `ffmperative-0.0.2.dist-info/LICENSE` & `ffmperative-0.0.2.post1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ffmperative-0.0.2.dist-info/METADATA` & `ffmperative-0.0.2.post1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmperative
-Version: 0.0.2
+Version: 0.0.2.post1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pillow
 Requires-Dist: opencv-python
 Requires-Dist: ffprobe-python
 Requires-Dist: ffmpeg-python
```

