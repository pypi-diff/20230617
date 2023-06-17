# Comparing `tmp/bilibili-toolman-1.0.7.7.3.tar.gz` & `tmp/bilibili-toolman-1.0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bilibili-toolman-1.0.7.7.3.tar", last modified: Thu Jan 26 01:28:20 2023, max compression
+gzip compressed data, was "bilibili-toolman-1.0.7.8.tar", last modified: Sat Jun 17 13:42:47 2023, max compression
```

## Comparing `bilibili-toolman-1.0.7.7.3.tar` & `bilibili-toolman-1.0.7.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 01:28:20.314368 bilibili-toolman-1.0.7.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-01-26 01:27:46.000000 bilibili-toolman-1.0.7.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14523 2023-01-26 01:28:20.310368 bilibili-toolman-1.0.7.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14055 2023-01-26 01:27:46.000000 bilibili-toolman-1.0.7.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 01:28:20.310368 bilibili-toolman-1.0.7.7.3/bilibili_toolman/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-01-26 01:27:46.000000 bilibili-toolman-1.0.7.7.3/bilibili_toolman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-01-26 01:27:46.000000 bilibili-toolman-1.0.7.7.3/bilibili_toolman/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 01:28:20.310368 bilibili-toolman-1.0.7.7.3/bilibili_toolman/bilisession/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-01-26 01:27:46.000000 bilibili-toolman-1.0.7.7.3/bilibili_toolman/bilisession/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15452 2023-01-26 01:27:46.000000 bilibili-toolman-1.0.7.7.3/bilibili_toolman/bilisession/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 01:28:20.310368 bilibili-toolman-1.0.7.7.3/bilibili_toolman/bilisession/common/
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-01-26 01:27:46.000000 bilibili-toolman-1.0.7.7.3/bilibili_toolman/bilisession/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-01-26 01:27:46.000000 bilibili-toolman-1.0.7.7.3/bilibili_toolman/bilisession/common/submission.py
--rw-r--r--   0 runner    (1001) docker     (123)    22148 2023-01-26 01:27:46.000000 bilibili-toolman-1.0.7.7.3/bilibili_toolman/bilisession/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 01:28:20.310368 bilibili-toolman-1.0.7.7.3/bilibili_toolman/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-01-26 01:27:46.000000 bilibili-toolman-1.0.7.7.3/bilibili_toolman/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12692 2023-01-26 01:27:46.000000 bilibili-toolman-1.0.7.7.3/bilibili_toolman/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-01-26 01:27:46.000000 bilibili-toolman-1.0.7.7.3/bilibili_toolman/cli/precentage_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-01-26 01:27:46.000000 bilibili-toolman-1.0.7.7.3/bilibili_toolman/cli/sanitizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 01:28:20.310368 bilibili-toolman-1.0.7.7.3/bilibili_toolman/providers/
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-01-26 01:27:46.000000 bilibili-toolman-1.0.7.7.3/bilibili_toolman/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-01-26 01:27:46.000000 bilibili-toolman-1.0.7.7.3/bilibili_toolman/providers/localfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-01-26 01:27:46.000000 bilibili-toolman-1.0.7.7.3/bilibili_toolman/providers/youtube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 01:28:20.310368 bilibili-toolman-1.0.7.7.3/bilibili_toolman.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14523 2023-01-26 01:28:20.000000 bilibili-toolman-1.0.7.7.3/bilibili_toolman.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-01-26 01:28:20.000000 bilibili-toolman-1.0.7.7.3/bilibili_toolman.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 01:28:20.000000 bilibili-toolman-1.0.7.7.3/bilibili_toolman.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-01-26 01:28:20.000000 bilibili-toolman-1.0.7.7.3/bilibili_toolman.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-01-26 01:28:20.000000 bilibili-toolman-1.0.7.7.3/bilibili_toolman.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-26 01:28:20.000000 bilibili-toolman-1.0.7.7.3/bilibili_toolman.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-26 01:28:20.314368 bilibili-toolman-1.0.7.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-01-26 01:27:46.000000 bilibili-toolman-1.0.7.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:42:47.105503 bilibili-toolman-1.0.7.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-17 13:42:17.000000 bilibili-toolman-1.0.7.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-06-17 13:42:47.105503 bilibili-toolman-1.0.7.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14055 2023-06-17 13:42:17.000000 bilibili-toolman-1.0.7.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:42:47.105503 bilibili-toolman-1.0.7.8/bilibili_toolman/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-17 13:42:17.000000 bilibili-toolman-1.0.7.8/bilibili_toolman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-17 13:42:17.000000 bilibili-toolman-1.0.7.8/bilibili_toolman/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:42:47.105503 bilibili-toolman-1.0.7.8/bilibili_toolman/bilisession/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-17 13:42:17.000000 bilibili-toolman-1.0.7.8/bilibili_toolman/bilisession/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15452 2023-06-17 13:42:17.000000 bilibili-toolman-1.0.7.8/bilibili_toolman/bilisession/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:42:47.105503 bilibili-toolman-1.0.7.8/bilibili_toolman/bilisession/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-06-17 13:42:17.000000 bilibili-toolman-1.0.7.8/bilibili_toolman/bilisession/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-06-17 13:42:17.000000 bilibili-toolman-1.0.7.8/bilibili_toolman/bilisession/common/submission.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21797 2023-06-17 13:42:17.000000 bilibili-toolman-1.0.7.8/bilibili_toolman/bilisession/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:42:47.105503 bilibili-toolman-1.0.7.8/bilibili_toolman/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-06-17 13:42:17.000000 bilibili-toolman-1.0.7.8/bilibili_toolman/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12692 2023-06-17 13:42:17.000000 bilibili-toolman-1.0.7.8/bilibili_toolman/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-17 13:42:17.000000 bilibili-toolman-1.0.7.8/bilibili_toolman/cli/precentage_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-17 13:42:17.000000 bilibili-toolman-1.0.7.8/bilibili_toolman/cli/sanitizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:42:47.105503 bilibili-toolman-1.0.7.8/bilibili_toolman/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-17 13:42:17.000000 bilibili-toolman-1.0.7.8/bilibili_toolman/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-17 13:42:17.000000 bilibili-toolman-1.0.7.8/bilibili_toolman/providers/localfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-06-17 13:42:17.000000 bilibili-toolman-1.0.7.8/bilibili_toolman/providers/youtube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:42:47.105503 bilibili-toolman-1.0.7.8/bilibili_toolman.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-06-17 13:42:47.000000 bilibili-toolman-1.0.7.8/bilibili_toolman.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-17 13:42:47.000000 bilibili-toolman-1.0.7.8/bilibili_toolman.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 13:42:47.000000 bilibili-toolman-1.0.7.8/bilibili_toolman.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-17 13:42:47.000000 bilibili-toolman-1.0.7.8/bilibili_toolman.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-17 13:42:47.000000 bilibili-toolman-1.0.7.8/bilibili_toolman.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-17 13:42:47.000000 bilibili-toolman-1.0.7.8/bilibili_toolman.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 13:42:47.105503 bilibili-toolman-1.0.7.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-17 13:42:17.000000 bilibili-toolman-1.0.7.8/setup.py
```

### Comparing `bilibili-toolman-1.0.7.7.3/LICENSE` & `bilibili-toolman-1.0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bilibili-toolman-1.0.7.7.3/PKG-INFO` & `bilibili-toolman-1.0.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bilibili-toolman
-Version: 1.0.7.7.3
+Version: 1.0.7.8
 Summary: bilibili-toolman 哔哩哔哩搬运工具
 Home-page: https://github.com/greats3an/bilibili-toolman
 Author: greats3an
 Author-email: greats3an@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `bilibili-toolman-1.0.7.7.3/README.md` & `bilibili-toolman-1.0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `bilibili-toolman-1.0.7.7.3/bilibili_toolman/bilisession/client.py` & `bilibili-toolman-1.0.7.8/bilibili_toolman/bilisession/client.py`

 * *Files identical despite different names*

### Comparing `bilibili-toolman-1.0.7.7.3/bilibili_toolman/bilisession/common/__init__.py` & `bilibili-toolman-1.0.7.8/bilibili_toolman/bilisession/common/__init__.py`

 * *Files identical despite different names*

### Comparing `bilibili-toolman-1.0.7.7.3/bilibili_toolman/bilisession/common/submission.py` & `bilibili-toolman-1.0.7.8/bilibili_toolman/bilisession/common/submission.py`

 * *Files 7% similar despite different names*

```diff
@@ -132,16 +132,19 @@
     state = 0
     """status of video"""
     state_desc = ""
     """status but human readable"""
     video_duration = 0
     """duration of video"""
     desc_format_id = 0
-    """description format IDs    
-    TODO : Document the IDs with corrosponding Threads"""
+    """description format IDs"""
+    topic_id = 0
+    """topic(?) ID"""
+    topic_name = ""
+    """topic(?) Name"""    
     _parent = None
 
     @property
     def parent(self):
         self._parent: Submission
         return self._parent
 
@@ -176,15 +179,22 @@
             "title": self.title,
             "tag": ",".join(set(self.tags)),
             "desc_format_id": self.desc_format_id,
             "desc": self.description,
             # "up_close_reply": self.close_reply,
             # "up_close_danmu": self.close_danmu
             "no_reprint": self.no_reprint,
-            "cover": self.cover_url
+            "cover": self.cover_url,
+            **({
+                "topic_detail":{
+                    "from_source":"arc.web.recommend", # let's leave it be for now
+                    "from_topic_id" : int(self.topic_id)
+                },
+                "topic_id": int(self.topic_id)
+            } if self.topic_id and self.topic_name else {})            
         }
         return kv_pair
 
     def __repr__(self) -> str:
         return '< bvid : "%s" , thread : %s , title : "%s", desc : "%s" , video_endpoint : "%s" >' % (
             self.bvid,
             self.thread,
@@ -217,8 +227,10 @@
         submission.state_desc = arc["archive"]["state_desc"]
         submission.state = arc["archive"]["state"]
         submission.reject_reason = arc["archive"]["reject_reason"]
         submission.no_reprint = arc["archive"]["no_reprint"]
         if "Videos" in arc:
             arc["videos"] = arc["Videos"]
         submission.videos.extend(arc["videos"])
+        submission.topic_id = arc["archive"].get("topic_id",0)
+        submission.topic_name = arc["archive"].get("topic_name","")
     return submission
```

### Comparing `bilibili-toolman-1.0.7.7.3/bilibili_toolman/bilisession/web.py` & `bilibili-toolman-1.0.7.8/bilibili_toolman/bilisession/web.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,24 +209,17 @@
             submission (Submission): 可由 `ViewArchive` 取得
 
         Returns:
             dict
         """
         return self._edit_archive(
             {
+                **submission.archive,
                 "aid": submission.aid,
-                "copyright": submission.copyright,
-                "videos": submission.videos.archive,
-                "source": submission.source,
-                "tid": int(submission.thread),
-                "cover": submission.cover_url,
-                "title": submission.title,
-                "tag": ",".join(set(submission.tags)),
                 "desc_format_id": 31,
-                "desc": submission.description,
             }
         )
 
     def ViewSubmission(self, bvid) -> Submission:
         """以 BVid 获取作品信息
 
         Notes:
```

### Comparing `bilibili-toolman-1.0.7.7.3/bilibili_toolman/cli/__init__.py` & `bilibili-toolman-1.0.7.8/bilibili_toolman/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `bilibili-toolman-1.0.7.7.3/bilibili_toolman/cli/main.py` & `bilibili-toolman-1.0.7.8/bilibili_toolman/cli/main.py`

 * *Files identical despite different names*

### Comparing `bilibili-toolman-1.0.7.7.3/bilibili_toolman/cli/sanitizers.py` & `bilibili-toolman-1.0.7.8/bilibili_toolman/cli/sanitizers.py`

 * *Files identical despite different names*

### Comparing `bilibili-toolman-1.0.7.7.3/bilibili_toolman/providers/__init__.py` & `bilibili-toolman-1.0.7.8/bilibili_toolman/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `bilibili-toolman-1.0.7.7.3/bilibili_toolman/providers/localfile.py` & `bilibili-toolman-1.0.7.8/bilibili_toolman/providers/localfile.py`

 * *Files identical despite different names*

### Comparing `bilibili-toolman-1.0.7.7.3/bilibili_toolman/providers/youtube.py` & `bilibili-toolman-1.0.7.8/bilibili_toolman/providers/youtube.py`

 * *Files identical despite different names*

### Comparing `bilibili-toolman-1.0.7.7.3/bilibili_toolman.egg-info/PKG-INFO` & `bilibili-toolman-1.0.7.8/bilibili_toolman.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bilibili-toolman
-Version: 1.0.7.7.3
+Version: 1.0.7.8
 Summary: bilibili-toolman 哔哩哔哩搬运工具
 Home-page: https://github.com/greats3an/bilibili-toolman
 Author: greats3an
 Author-email: greats3an@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `bilibili-toolman-1.0.7.7.3/bilibili_toolman.egg-info/SOURCES.txt` & `bilibili-toolman-1.0.7.8/bilibili_toolman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bilibili-toolman-1.0.7.7.3/setup.py` & `bilibili-toolman-1.0.7.8/setup.py`

 * *Files identical despite different names*

