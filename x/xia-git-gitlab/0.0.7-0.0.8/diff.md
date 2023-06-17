# Comparing `tmp/xia_git_gitlab-0.0.7-cp39-none-win_amd64.whl.zip` & `tmp/xia_git_gitlab-0.0.8-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 170089 bytes, number of entries: 7
--rw-r--r--  2.0 unx       95 b- defN 23-Jun-10 15:34 xia_git_gitlab/__init__.py
--rw-r--r--  2.0 unx   442368 b- defN 23-Jun-10 15:40 xia_git_gitlab/git.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-10 15:40 xia_git_gitlab-0.0.7.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      700 b- defN 23-Jun-10 15:40 xia_git_gitlab-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-10 15:40 xia_git_gitlab-0.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Jun-10 15:40 xia_git_gitlab-0.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      600 b- defN 23-Jun-10 15:40 xia_git_gitlab-0.0.7.dist-info/RECORD
-7 files, 444028 bytes uncompressed, 169013 bytes compressed:  61.9%
+Zip file size: 170629 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       95 b- defN 23-Jun-10 17:25 xia_git_gitlab/__init__.py
+-rw-r--r--  2.0 unx   444416 b- defN 23-Jun-10 17:27 xia_git_gitlab/git.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-10 17:27 xia_git_gitlab-0.0.8.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      700 b- defN 23-Jun-10 17:27 xia_git_gitlab-0.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-10 17:27 xia_git_gitlab-0.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-10 17:27 xia_git_gitlab-0.0.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      600 b- defN 23-Jun-10 17:27 xia_git_gitlab-0.0.8.dist-info/RECORD
+7 files, 446076 bytes uncompressed, 169553 bytes compressed:  62.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_git_gitlab/__init__.py
 Comment: 
 
 Filename: xia_git_gitlab/git.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_git_gitlab-0.0.7.dist-info/LICENSE.txt
+Filename: xia_git_gitlab-0.0.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_git_gitlab-0.0.7.dist-info/METADATA
+Filename: xia_git_gitlab-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: xia_git_gitlab-0.0.7.dist-info/WHEEL
+Filename: xia_git_gitlab-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: xia_git_gitlab-0.0.7.dist-info/top_level.txt
+Filename: xia_git_gitlab-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_git_gitlab-0.0.7.dist-info/RECORD
+Filename: xia_git_gitlab-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_git_gitlab/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_git_gitlab.git import GitlabGit
 
 __all__ = [
     "GitlabGit"
 ]
 
-__version__ = "0.0.7"
+__version__ = "0.0.8"
```

## Comparing `xia_git_gitlab-0.0.7.dist-info/METADATA` & `xia_git_gitlab-0.0.8.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-git-gitlab
-Version: 0.0.7
+Version: 0.0.8
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-git-gitlab/0.0.7/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-git-gitlab/0.0.8/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

