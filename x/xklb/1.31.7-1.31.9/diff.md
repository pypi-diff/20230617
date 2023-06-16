# Comparing `tmp/xklb-1.31.7.tar.gz` & `tmp/xklb-1.31.9.tar.gz`

## Comparing `xklb-1.31.7.tar` & `xklb-1.31.9.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.31.7/.gitattributes
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 xklb-1.31.7/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.31.7/Windows.md
--rw-r--r--   0        0        0   490396 2020-02-02 00:00:00.000000 xklb-1.31.7/pdm.lock
--rw-r--r--   0        0        0    19420 2020-02-02 00:00:00.000000 xklb-1.31.7/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.31.7/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.31.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.31.7/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-1.31.7/.github/workflows/green.yaml
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 xklb-1.31.7/.github/workflows/push.yaml
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/__init__.py
--rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/av.py
--rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/books.py
--rw-r--r--   0        0        0     9396 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/consts.py
--rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/db.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/dl_config.py
--rw-r--r--   0        0        0    11755 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/dl_extract.py
--rw-r--r--   0        0        0    14103 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/fs_extract.py
--rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/gdl_backend.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/gdl_extract.py
--rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/gui.py
--rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/hn_extract.py
--rw-r--r--   0        0        0    11781 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/lb.py
--rw-r--r--   0        0        0     7643 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/media.py
--rw-r--r--   0        0        0    25448 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/play_actions.py
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/playback.py
--rw-r--r--   0        0        0    35233 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/player.py
--rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/playlists.py
--rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/praw_extract.py
--rw-r--r--   0        0        0     7949 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/search.py
--rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/subtitle.py
--rw-r--r--   0        0        0     6029 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/tabs_actions.py
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/tabs_extract.py
--rw-r--r--   0        0        0    15396 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/tube_backend.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/tube_extract.py
--rw-r--r--   0        0        0    76102 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/usage.py
--rw-r--r--   0        0        0    37347 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     5781 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/block.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/christen.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/cluster_sort.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/dedupe_db.py
--rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/download_status.py
--rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/history.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/playlists.py
--rw-r--r--   0        0        0     6044 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/relmv.py
--rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.31.7/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.31.7/LICENSE
--rw-r--r--   0        0        0    98892 2020-02-02 00:00:00.000000 xklb-1.31.7/README.md
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 xklb-1.31.7/pyproject.toml
--rw-r--r--   0        0        0   102519 2020-02-02 00:00:00.000000 xklb-1.31.7/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.31.9/.gitattributes
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 xklb-1.31.9/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.31.9/Windows.md
+-rw-r--r--   0        0        0   490396 2020-02-02 00:00:00.000000 xklb-1.31.9/pdm.lock
+-rw-r--r--   0        0        0    19420 2020-02-02 00:00:00.000000 xklb-1.31.9/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.31.9/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.31.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.31.9/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-1.31.9/.github/workflows/green.yaml
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 xklb-1.31.9/.github/workflows/push.yaml
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/__init__.py
+-rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/av.py
+-rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/books.py
+-rw-r--r--   0        0        0     9396 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/consts.py
+-rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/db.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/dl_config.py
+-rw-r--r--   0        0        0    11814 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/dl_extract.py
+-rw-r--r--   0        0        0    14167 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/fs_extract.py
+-rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/gdl_backend.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/gdl_extract.py
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/gui.py
+-rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/hn_extract.py
+-rw-r--r--   0        0        0    11781 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/lb.py
+-rw-r--r--   0        0        0     7649 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/media.py
+-rw-r--r--   0        0        0    25369 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/play_actions.py
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/playback.py
+-rw-r--r--   0        0        0    35233 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/player.py
+-rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/playlists.py
+-rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/praw_extract.py
+-rw-r--r--   0        0        0     7949 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/search.py
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/subtitle.py
+-rw-r--r--   0        0        0     6029 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    15396 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/tube_backend.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/tube_extract.py
+-rw-r--r--   0        0        0    76102 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/usage.py
+-rw-r--r--   0        0        0    37860 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     5781 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/block.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/cluster_sort.py
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/dedupe_db.py
+-rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/download_status.py
+-rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/history.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/playlists.py
+-rw-r--r--   0        0        0     6044 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.31.9/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.31.9/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.31.9/LICENSE
+-rw-r--r--   0        0        0    98892 2020-02-02 00:00:00.000000 xklb-1.31.9/README.md
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 xklb-1.31.9/pyproject.toml
+-rw-r--r--   0        0        0   102519 2020-02-02 00:00:00.000000 xklb-1.31.9/PKG-INFO
```

### Comparing `xklb-1.31.7/TODO` & `xklb-1.31.9/TODO`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/Windows.md` & `xklb-1.31.9/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/pdm.lock` & `xklb-1.31.9/pdm.lock`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/readme.py` & `xklb-1.31.9/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-1.31.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-1.31.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/.github/workflows/push.yaml` & `xklb-1.31.9/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/av.py` & `xklb-1.31.9/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/books.py` & `xklb-1.31.9/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/consts.py` & `xklb-1.31.9/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/db.py` & `xklb-1.31.9/xklb/db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/dl_config.py` & `xklb-1.31.9/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/dl_extract.py` & `xklb-1.31.9/xklb/dl_extract.py`

 * *Files 3% similar despite different names*

```diff
@@ -156,22 +156,22 @@
                 {', p.extractor_config' if 'extractor_config' in pl_columns else ''}
                 , p.extractor_key
             FROM media m
             LEFT JOIN playlists p on p.id = m.playlist_id
             WHERE 1=1
                 and COALESCE(m.time_downloaded,0) = 0
                 and COALESCE(m.time_deleted,0) = 0
-                and COALESCE(p.time_deleted,0) = 0
+                {'and COALESCE(p.time_deleted, 0) = 0' if 'time_deleted' in pl_columns else ''}
                 and m.path like "http%"
                 {'AND (score IS NULL OR score > 7)' if 'score' in m_columns else ''}
                 {'AND (upvote_ratio IS NULL OR upvote_ratio > 0.73)' if 'upvote_ratio' in m_columns else ''}
                 {" ".join(args.filter_sql)}
             ORDER BY 1=1
-                , play_count
-                , COALESCE(m.time_modified,0) = 0 DESC
+                , COALESCE(m.time_modified, 0) = 0 DESC
+                , m.time_modified
                 {', ' + args.sort if args.sort else ''}
                 , random()
         {LIMIT}
         """
     else:
         query = f"""select
                 m.path
@@ -188,16 +188,16 @@
                 {'and COALESCE(m.time_downloaded,0) = 0' if 'time_downloaded' in m_columns else ''}
                 {'and COALESCE(m.time_deleted,0) = 0' if 'time_deleted' in m_columns else ''}
                 and m.path like "http%"
                 {'AND (score IS NULL OR score > 7)' if 'score' in m_columns else ''}
                 {'AND (upvote_ratio IS NULL OR upvote_ratio > 0.73)' if 'upvote_ratio' in m_columns else ''}
                 {" ".join(args.filter_sql)}
             ORDER BY 1=1
-                {', play_count' if 'play_count' in m_columns else ''}
                 {', COALESCE(m.time_modified,0) = 0 DESC' if 'time_modified' in m_columns else ''}
+                {', m.time_modified' if 'time_modified' in m_columns else ''}
                 {', ' + args.sort if args.sort else ''}
                 , random()
         {LIMIT}
         """
 
     return query, args.filter_bindings
```

### Comparing `xklb-1.31.7/xklb/fs_extract.py` & `xklb-1.31.9/xklb/fs_extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import argparse, math, os, sys
+import argparse, json, math, os, sys
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
 from functools import partial
 from multiprocessing import TimeoutError as mp_TimeoutError
 from pathlib import Path
 from shutil import which
 from timeit import default_timer as timer
 from typing import Dict, List, Optional
@@ -403,12 +403,13 @@
                 length(path)-length(REPLACE(path, '/', '')) desc
                 , path
             """,
         ),
     )
 
     for playlist in fs_playlists:
+        extractor_config = json.loads((playlist.get("extractor_config") or "{}"))
         args_env = argparse.Namespace(
-            **{**(playlist.get("extractor_config") or {}), **args.__dict__, "profile": playlist["profile"]},
+            **{**extractor_config, **args.__dict__, "profile": playlist["profile"]},
         )
 
         extractor(args_env, [playlist["path"]])
```

### Comparing `xklb-1.31.7/xklb/gdl_backend.py` & `xklb-1.31.9/xklb/gdl_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/gdl_extract.py` & `xklb-1.31.9/xklb/gdl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/gui.py` & `xklb-1.31.9/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/hn_extract.py` & `xklb-1.31.9/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/lb.py` & `xklb-1.31.9/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/media.py` & `xklb-1.31.9/xklb/media.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,15 @@
 
     v = {
         k: v
         for k, v in v.items()
         if not (k.startswith(("_", "reblogged_")) or k in consts.MEDIA_KNOWN_KEYS or v is None)
     }
     if v != {}:
-        log.info("Extra data %s", v)
+        log.info("Extra media data %s", v)
         # breakpoint()
 
     return utils.dict_filter_bool(cv)
 
 
 def _add(args, entry):
     tags = entry.pop("tags", None) or ""
```

### Comparing `xklb-1.31.7/xklb/play_actions.py` & `xklb-1.31.9/xklb/play_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-import argparse, shlex, shutil, sys, time
-import os
+import argparse, os, shlex, shutil, sys, time
 from collections import deque
 from concurrent.futures import ThreadPoolExecutor
 from pathlib import Path
 from random import random
 from typing import Dict, Tuple
 
 from xklb import consts, db, player, subtitle, tube_backend, usage, utils
@@ -44,17 +43,14 @@
                 consts.PYTEST_RUNNING,
                 "subtitle_count" in args.where,
                 args.limit != consts.DEFAULT_PLAY_QUEUE,
             ],
         )
         else None,
         args.sort,
-        "time_downloaded > 0 desc"
-        if "time_downloaded" in m_columns and "time_downloaded" not in " ".join(sys.argv)
-        else None,
         "duration desc" if args.action in (SC.listen, SC.watch) and args.include else None,
         "size desc" if args.action in (SC.listen, SC.watch) and args.include else None,
         "play_count" if args.action in (SC.listen, SC.watch) and "play_count" in m_columns else None,
         "size desc, duration"
         if args.action in (SC.listen, SC.watch) and "size" in m_columns and "duration" in m_columns
         else None,
         "sparseness" if args.action == SC.filesystem else None,
@@ -601,17 +597,19 @@
         media_keyed = {d["path"]: d for d in media}
         dirs = process_bigdirs(args, media)
         dirs = list(reversed([d["path"] for d in dirs]))
         if "limit" in args.defaults:
             media = player.get_dir_media(args, dirs)
         else:
             media = []
-            for dir in dirs:
-                for key in media_keyed:
-                    if os.sep not in key.replace(dir, '') and key.startswith(dir):
+            for key in media_keyed:
+                for dir in dirs:
+                    if len(dir) == 1:
+                        continue
+                    if os.sep not in key.replace(dir, "") and key.startswith(dir):
                         media.append(media_keyed[key])
                         break
         log.debug("big_dirs: %s", t.elapsed())
 
     if args.related >= consts.RELATED:
         media = player.get_related_media(args, media[0])
         log.debug("player.get_related_media: %s", t.elapsed())
```

### Comparing `xklb-1.31.7/xklb/playback.py` & `xklb-1.31.9/xklb/playback.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/player.py` & `xklb-1.31.9/xklb/player.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/playlists.py` & `xklb-1.31.9/xklb/playlists.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
     v = {
         k: v
         for k, v in v.items()
         if not (k.startswith("_") or k in consts.MEDIA_KNOWN_KEYS + consts.PLAYLIST_KNOWN_KEYS or v is None)
     }
     if v != {}:
-        log.info("Extra data %s", v)
+        log.info("Extra playlists data %s", v)
         # breakpoint()
 
     return utils.dict_filter_bool(cv) or {}
 
 
 def get_id(args, playlist_path) -> int:
     return args.db.pop("select id from playlists where path=?", [str(playlist_path)])
```

### Comparing `xklb-1.31.7/xklb/praw_extract.py` & `xklb-1.31.9/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/search.py` & `xklb-1.31.9/xklb/search.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/subtitle.py` & `xklb-1.31.9/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/tabs_actions.py` & `xklb-1.31.9/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/tabs_extract.py` & `xklb-1.31.9/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/tube_backend.py` & `xklb-1.31.9/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/tube_extract.py` & `xklb-1.31.9/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/usage.py` & `xklb-1.31.9/xklb/usage.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/utils.py` & `xklb-1.31.9/xklb/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1101,16 +1101,28 @@
 
 def cluster_paths(paths, n_clusters=None):
     from sklearn.cluster import KMeans
     from sklearn.feature_extraction.text import TfidfVectorizer
 
     sentence_strings = (path_to_sentence(s) for s in paths)
 
-    vectorizer = TfidfVectorizer(min_df=2, strip_accents="unicode", stop_words="english")
-    X = vectorizer.fit_transform(sentence_strings)
+    try:
+        vectorizer = TfidfVectorizer(min_df=2, strip_accents="unicode", stop_words="english")
+        X = vectorizer.fit_transform(sentence_strings)
+    except ValueError:
+        try:
+            vectorizer = TfidfVectorizer(strip_accents="unicode", stop_words="english")
+            X = vectorizer.fit_transform(sentence_strings)
+        except ValueError:
+            try:
+                vectorizer = TfidfVectorizer()
+                X = vectorizer.fit_transform(sentence_strings)
+            except ValueError:
+                vectorizer = TfidfVectorizer(analyzer="char_wb")
+                X = vectorizer.fit_transform(sentence_strings)
 
     clusterizer = KMeans(n_clusters=n_clusters or int(X.shape[0] ** 0.5), random_state=0, n_init=10).fit(X)
     clusters = clusterizer.labels_
 
     grouped_strings = {}
     for i, string in enumerate(paths):
         cluster_id = clusters[i]
```

### Comparing `xklb-1.31.7/xklb/scripts/bigdirs.py` & `xklb-1.31.9/xklb/scripts/bigdirs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/scripts/block.py` & `xklb-1.31.9/xklb/scripts/block.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/scripts/christen.py` & `xklb-1.31.9/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/scripts/cluster_sort.py` & `xklb-1.31.9/xklb/scripts/cluster_sort.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/scripts/copy_play_counts.py` & `xklb-1.31.9/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/scripts/dedupe.py` & `xklb-1.31.9/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/scripts/dedupe_db.py` & `xklb-1.31.9/xklb/scripts/dedupe_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/scripts/download_status.py` & `xklb-1.31.9/xklb/scripts/download_status.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/scripts/history.py` & `xklb-1.31.9/xklb/scripts/history.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/scripts/merge_dbs.py` & `xklb-1.31.9/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/scripts/merge_online_local.py` & `xklb-1.31.9/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/scripts/move_list.py` & `xklb-1.31.9/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/scripts/optimize_db.py` & `xklb-1.31.9/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/scripts/playlists.py` & `xklb-1.31.9/xklb/scripts/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/scripts/redownload.py` & `xklb-1.31.9/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/scripts/relmv.py` & `xklb-1.31.9/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/scripts/scatter.py` & `xklb-1.31.9/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/scripts/streaming_tab_loader.py` & `xklb-1.31.9/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/scripts/mining/data.py` & `xklb-1.31.9/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/scripts/mining/extract_links.py` & `xklb-1.31.9/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/scripts/mining/nouns.py` & `xklb-1.31.9/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/scripts/mining/pushshift.py` & `xklb-1.31.9/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/scripts/mining/reddit_selftext.py` & `xklb-1.31.9/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/xklb/assets/kotobago.png` & `xklb-1.31.9/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/.gitignore` & `xklb-1.31.9/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/LICENSE` & `xklb-1.31.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/README.md` & `xklb-1.31.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.31.007)
+    xk media library subcommands (v1.31.009)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

### Comparing `xklb-1.31.7/pyproject.toml` & `xklb-1.31.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-1.31.7/PKG-INFO` & `xklb-1.31.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.31.7
+Version: 1.31.9
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library/wiki/Usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library/
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -224,15 +224,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.31.007)
+    xk media library subcommands (v1.31.009)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

