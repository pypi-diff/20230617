# Comparing `tmp/monthify-0.3.4.tar.gz` & `tmp/monthify-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monthify-0.3.4.tar", max compression
+gzip compressed data, was "monthify-0.3.5.tar", max compression
```

## Comparing `monthify-0.3.4.tar` & `monthify-0.3.5.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0     1133 2023-05-18 06:24:22.438685 monthify-0.3.4/README.md
--rw-r--r--   0        0        0       42 2023-05-18 06:24:22.439685 monthify-0.3.4/monthify/__init__.py
--rw-r--r--   0        0        0       68 2023-05-18 06:24:22.439685 monthify-0.3.4/monthify/__main__.py
--rw-r--r--   0        0        0     1106 2023-05-27 03:11:30.775267 monthify-0.3.4/monthify/auth.py
--rw-r--r--   0        0        0     4367 2023-05-27 02:45:32.298405 monthify-0.3.4/monthify/main.py
--rw-r--r--   0        0        0    18611 2023-05-27 03:11:30.776267 monthify-0.3.4/monthify/script.py
--rw-r--r--   0        0        0      764 2023-05-18 06:24:22.439685 monthify-0.3.4/monthify/track.py
--rw-r--r--   0        0        0     1185 2023-05-27 02:42:22.456255 monthify-0.3.4/monthify/utils.py
--rw-r--r--   0        0        0      815 2023-05-27 03:11:30.776267 monthify-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     1792 1970-01-01 00:00:00.000000 monthify-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1133 2023-05-18 06:24:22.438685 monthify-0.3.5/README.md
+-rw-r--r--   0        0        0      435 2023-05-28 05:00:16.109215 monthify-0.3.5/monthify/__init__.py
+-rw-r--r--   0        0        0       68 2023-05-18 06:24:22.439685 monthify-0.3.5/monthify/__main__.py
+-rw-r--r--   0        0        0     1610 2023-06-13 20:30:31.505128 monthify-0.3.5/monthify/args.py
+-rw-r--r--   0        0        0     1103 2023-05-28 04:45:17.054980 monthify-0.3.5/monthify/auth.py
+-rw-r--r--   0        0        0      811 2023-05-28 04:59:34.295576 monthify-0.3.5/monthify/config.py
+-rw-r--r--   0        0        0     2916 2023-06-13 20:36:34.279834 monthify-0.3.5/monthify/main.py
+-rw-r--r--   0        0        0    19056 2023-06-17 20:47:51.409566 monthify-0.3.5/monthify/script.py
+-rw-r--r--   0        0        0      769 2023-06-13 20:30:31.506127 monthify-0.3.5/monthify/track.py
+-rw-r--r--   0        0        0     1185 2023-05-27 02:42:22.456255 monthify-0.3.5/monthify/utils.py
+-rw-r--r--   0        0        0      815 2023-05-28 04:27:43.087494 monthify-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     1792 1970-01-01 00:00:00.000000 monthify-0.3.5/PKG-INFO
```

### Comparing `monthify-0.3.4/README.md` & `monthify-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `monthify-0.3.4/monthify/script.py` & `monthify-0.3.5/monthify/script.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,34 @@
 # Script
 import sys
-from collections.abc import Iterable
+
+# from collections.abc import Iterable
 from datetime import datetime
 from os import makedirs, remove, stat
 from os.path import exists
 from pathlib import Path
+from typing import Any, Generator, Iterable, List, Reversible, Tuple
 
-from appdirs import user_data_dir
 from cachetools import TTLCache, cached
 from loguru import logger
-from rich.console import Console
 
-from monthify import ERROR, SUCCESS
+from monthify import ERROR, SUCCESS, appdata_location, console
 from monthify.auth import Auth
 from monthify.track import Track
-from monthify.utils import (
-    conditional_decorator,
-    normalize_text,
-    sort_chronologically,
-)
-
-appname = "Monthify"
-appauthor = "madstone0-0"
-appdata_location = user_data_dir(appname, appauthor)
+from monthify.utils import conditional_decorator, normalize_text, sort_chronologically
 
 MAX_RESULTS = 10000
 CACHE_LIFETIME = 30
 
 makedirs(f"{appdata_location}/logs", exist_ok=True)
 logger.add(
-    sys.stderr,
-    format="{time} {level} {message}",
-    filter="monthify",
-    level="INFO",
+    sys.stderr, format="{time} {level} {message}", filter="monthify", level="INFO"
 )
 logger.remove()
 logger.add(f"{appdata_location}/logs/monthify.log", rotation="00:00", compression="zip")
-console = Console()
 existing_playlists_file = f"{appdata_location}/existing_playlists_file.dat"
 last_run_file = f"{appdata_location}/last_run.txt"
 last_run_format = "%Y-%m-%d %H:%M:%S"
 saved_tracks_cache: TTLCache = TTLCache(maxsize=1000, ttl=86400)
 saved_playlists_cache: TTLCache = TTLCache(maxsize=1000, ttl=86400)
 user_cache: TTLCache = TTLCache(maxsize=1, ttl=86400)
 
@@ -58,17 +46,17 @@
         self.LOGOUT = LOGOUT
         self.logout()
         authentication = auth
         self.sp = authentication.get_spotipy()
         self.SKIP_PLAYLIST_CREATION = SKIP_PLAYLIST_CREATION
         self.CREATE_PLAYLIST = CREATE_PLAYLIST
         self.has_created_playlists = False
-        self.current_username = ""
-        self.current_display_name = ""
-        self.playlist_names: Iterable[str] = []
+        self.current_username: str
+        self.current_display_name: str
+        self.playlist_names: List[Tuple[str, str]]
         self.already_created_playlists_exists = False
         if (
             exists(existing_playlists_file)
             and stat(existing_playlists_file).st_size != 0
         ):
             if (
                 datetime.now()
@@ -81,62 +69,62 @@
                 with open(existing_playlists_file, "r", encoding="utf_8") as f:
                     self.already_created_playlists = list(f.read().splitlines())
                     self.already_created_playlists_exists = True
         else:
             self.already_created_playlists = []
             self.already_created_playlists_exists = False
 
-        self.already_created_playlists_inter: Iterable[str] = []
+        self.already_created_playlists_inter: List[str] = []
         if exists(last_run_file):
             if stat(last_run_file).st_size != 0:
                 with open(last_run_file, "r", encoding="utf_8") as f:
                     self.last_run = f.read()
             else:
                 self.last_run = ""
         else:
             self.last_run = ""
 
-        self.playlist_names_with_id: Iterable[str] = []
+        self.playlist_names_with_id: List[Tuple[str, str, str]] = []
         self.name = """
         ___  ___            _   _     _  __       
         |  \/  |           | | | |   (_)/ _|      
         | .  . | ___  _ __ | |_| |__  _| |_ _   _ 
         | |\/| |/ _ \| '_ \| __| '_ \| |  _| | | |
         | |  | | (_) | | | | |_| | | | | | | |_| |
         \_|  |_/\___/|_| |_|\__|_| |_|_|_|  \__, |
                                              __/ |
                                             |___/ 
         written by [link=https://github.com/madstone0-0]madstone0-0[/link]
         """
 
-    def logout(self):
+    def logout(self) -> None:
         if self.LOGOUT is True:
             try:
                 remove(f"{appdata_location}/.cache")
                 console.print("Successfully logged out of saved account", style=SUCCESS)
                 logger.info("Successfully deleted .cache file, user logged out")
                 sys.exit(0)
             except FileNotFoundError:
                 console.print("Not logged into any account", style=ERROR)
                 logger.error("Cache file doesn't exist")
                 sys.exit(0)
 
-    def starting(self):
+    def starting(self) -> None:
         """
         Staring function
         Displays project name and current username
         """
         logger.info("Starting script execution")
         console.print(self.name, style="green")
         with console.status("Retrieving user information"):
             self.current_display_name = self.get_username()["display_name"]
             self.current_username = self.get_username()["uri"][13:]
         console.print(f"Username: [cyan]{self.current_display_name}[/cyan]\n")
 
-    def update_last_run(self):
+    def update_last_run(self) -> None:
         """
         Updates last run time to current time
         """
         self.last_run = datetime.now().strftime(last_run_format)
         with open(last_run_file, "w", encoding="utf_8") as f:
             f.write(self.last_run)
 
@@ -150,22 +138,22 @@
             if result["next"]:
                 result = self.sp.next(result)
             else:
                 result = None
         return results
 
     @cached(user_cache)
-    def get_username(self):
+    def get_username(self) -> dict:
         """
         Retrieves the current user's spotify information
         """
         return self.sp.current_user()
 
     @cached(saved_tracks_cache)
-    def get_user_saved_tracks(self):
+    def get_user_saved_tracks(self) -> List[dict]:
         """
         Retrieves the current user's saved spotify tracks
         """
         logger.info("Starting user saved tracks fetch")
         results = self.get_results(self.sp.current_user_saved_tracks(limit=50))
         logger.info("Ending user saved tracks fetch")
         return results
@@ -176,26 +164,26 @@
         Retrieves the current user's created or liked spotify playlists
         """
         logger.info("Starting user saved playlists fetch")
         results = self.get_results(self.sp.current_user_playlists(limit=50))
         logger.info("Ending user saved playlists fetch")
         return results
 
-    def get_playlist_items(self, playlist_id):
+    def get_playlist_items(self, playlist_id: str) -> List[dict]:
         """
         Retrieves all the tracks in a specified spotify playlist identified by playlist id
         """
         logger.info(f"Starting playlist item fetch\n id: {playlist_id}", playlist_id)
         results = self.get_results(
             self.sp.playlist_items(playlist_id=playlist_id, fields=None, limit=20)
         )
         logger.info(f"Ending playlist item fetch\n id: {playlist_id}")
         return results
 
-    def create_playlist(self, name):
+    def create_playlist(self, name: str) -> None:
         """
         Creates playlist with name var checking if the playlist already exists in the user's library,
         if it does the user is informed
         """
         sp = self.sp
         playlists = self.get_user_saved_playlists()
         already_created_playlists = []
@@ -223,22 +211,22 @@
             )
             created_playlists.append(playlist)
             console.print(f"Added {name} playlist")
             logger.info(f"Added {name} playlist")
         self.has_created_playlists = True if len(created_playlists) > 0 else False
         self.already_created_playlists_inter = already_created_playlists
 
-    def get_saved_track_info(self):
+    def get_saved_track_info(self) -> None:
         """
         Calls the get_saved_track_gen function at program's start to cache the user's saved tracks
         """
         with console.status("Retrieving user saved tracks"):
             self.get_saved_track_gen()
 
-    def get_saved_track_gen(self):
+    def get_saved_track_gen(self) -> Generator[Track, Any, None]:
         """
         Collates the user's saved tracks and adds them to a list as a Track type
         """
         tracks = self.get_user_saved_tracks()
         logger.info("Retrieving saved track info")
         track_list = (
             Track(
@@ -252,17 +240,17 @@
         return track_list
 
     def get_playlist_names_names(self):
         """
         Generates month playlist names using the added_at attribute of the Track type
         """
         logger.info("Generating playlist names")
-        self.playlist_names = [
+        self.playlist_names = tuple(
             track.track_month for track in self.get_saved_track_gen()
-        ]
+        )
         unsorted_playlist_names = [*set(self.playlist_names)]
         self.playlist_names = sort_chronologically(unsorted_playlist_names)
         logger.info("Removing duplicate playlist names")
         logger.info(f"Final list: {self.playlist_names}")
 
     def get_monthly_playlist_ids(self):
         """
@@ -279,110 +267,117 @@
                         self.playlist_names_with_id.append((month, year, item["id"]))
                         logger.info(
                             "Playlist name: {name} id: {id}",
                             name=str(month + " '" + year[2:]),
                             id=str(item["id"]),
                         )
 
-    def create_monthly_playlists(self):
-        """
-        Creates playlists in user's library based on generated playlist names
-        """
-        logger.info("Creating playlists")
-        with console.status("Generating playlists"):
-            spotify_playlists = [
-                item["name"] for item in self.get_user_saved_playlists()
-            ]
-
-        monthly_ran = False
-        if not self.last_run:
-            last_run = datetime.now().strftime(last_run_format)
+    def skip(self, status: bool, playlists: Iterable = None) -> None:
+        if status is True:
+            console.print("Playlist generation skipped")
+            logger.info("Playlist generation skipped")
         else:
-            last_run = self.last_run
-
-        def playlist_loop():
+            logger.info("Playlist generation starting")
+            if playlists is None:
+                RuntimeError("Playlists have not passed been passed to skip function")
             for month, year in reversed(self.playlist_names):
                 playlist_name = str(month + " '" + year[2:])
                 if (
                     playlist_name in self.already_created_playlists
-                    and playlist_name in spotify_playlists
+                    and playlist_name in playlists
                 ):
                     console.print(f"{month} '{year[2:]} playlist already exists")
                 else:
                     name = month + " '" + year[2:]
                     self.create_playlist(name)
 
-        def skip(status: bool) -> None:
-            if status is True:
-                console.print("Playlist generation skipped")
-                logger.info("Playlist generation skipped")
-            else:
-                logger.info("Playlist generation starting")
-                playlist_loop()
+    def create_monthly_playlists(self):
+        """
+        Creates playlists in user's library based on generated playlist names
+        """
+        logger.info("Creating playlists")
+        with console.status("Generating playlists"):
+            spotify_playlists = [
+                item["name"] for item in self.get_user_saved_playlists()
+            ]
 
-        if (
-            datetime.strptime(last_run, last_run_format).strftime("%B")
-            != datetime.now().strftime("%B")
-        ) and self.already_created_playlists_exists is False:
+        monthly_ran = False
+        last_run = (
+            datetime.now().strftime(last_run_format)
+            if not self.last_run
+            else self.last_run
+        )
+
+        has_month_passed = datetime.strptime(last_run, last_run_format).strftime(
+            "%B"
+        ) != datetime.now().strftime("%B")
+        if has_month_passed and self.already_created_playlists_exists is False:
+            self.skip(False, spotify_playlists)
+        elif has_month_passed is False and self.already_created_playlists_exists:
             monthly_ran = True
-            playlist_loop()
 
         if self.CREATE_PLAYLIST is False:
-            if (
-                self.SKIP_PLAYLIST_CREATION is False
-                and monthly_ran is False
-                or self.already_created_playlists_exists is False
-            ):
+            if self.SKIP_PLAYLIST_CREATION is False and monthly_ran is False:
                 console.print(
                     "Playlist generation has already occurred this month, do you still want to generate "
                     "playlists? (yes/no)"
                 )
                 logger.info("Requesting playlist creation")
 
                 if not console.input("> ").lower().startswith("y"):
-                    skip(True)
+                    self.skip(True)
                 else:
-                    skip(False)
+                    self.skip(False, spotify_playlists)
+
+            elif self.already_created_playlists_exists is False:
+                console.print(
+                    "Somehow the playlists do not exist. Generating Playlists..."
+                )
+                logger.info("Requesting playlist creation")
+                self.skip(False, spotify_playlists)
+
             else:
-                skip(True)
+                self.skip(True)
+
         else:
-            skip(False)
+            self.skip(False, spotify_playlists)
 
         if self.already_created_playlists_inter:
             self.already_created_playlists = [
                 *self.already_created_playlists,
                 *self.already_created_playlists_inter,
             ]
             self.already_created_playlists = list(
                 dict.fromkeys(self.already_created_playlists)
             )
 
         if self.already_created_playlists:
             with open(existing_playlists_file, "w", encoding="utf_8") as f:
                 f.write("\n".join(self.already_created_playlists))
 
-    def add_to_playlist(self, tracks: list[Track], playlist_id: str) -> None:
+    def add_to_playlist(self, tracks: Reversible[Track], playlist_id: str) -> None:
         """
         Add a list of tracks to a specified playlist using playlist id
         """
         logger.info(
             "Attempting to add tracks to playlist: {playlist}\ntracks: {tracks} ",
             tracks=tracks,
             playlist=str(playlist_id),
         )
         playlist_items = self.get_playlist_items(playlist_id)
         to_be_added_uris: list[str] = []
-        playlist_uris: Iterable[str] = []
 
-        playlist_uris = tuple(item["track"]["uri"] for item in playlist_items)
+        playlist_uris: Iterable[str] = tuple(
+            item["track"]["uri"] for item in playlist_items
+        )
 
         for track in reversed(tracks):
             if track.uri in playlist_uris:
                 logger.info(f"Track: {track} already in playlist: {str(playlist_id)}")
-                track_url = f'https://open.{track.uri. replace(":", "/").replace("spotify", "spotify.com")}'
+                track_url = f'https://open.{track.uri.replace(":", "/").replace("spotify", "spotify.com")}'
                 console.print(
                     f"[bold red][-][/bold red]\t[link={track_url}][cyan]{track.title} by {track.artist}[/cyan][/link]"
                     " already exists in the playlist"
                 )
             else:
                 logger.info(
                     f"Track: {track} will be added to playlist: {str(playlist_id)}"
@@ -443,16 +438,15 @@
                 style=ERROR,
             )
             sys.exit(1)
 
         with console.status("Sorting Tracks"):
             for month, year, playlist_id in self.playlist_names_with_id:
                 logger.info(
-                    "Sorting into playlist: {playlist}",
-                    playlist=(month, year[2:]),
+                    "Sorting into playlist: {playlist}", playlist=(month, year[2:])
                 )
                 playlist_url = f"https://open.spotify.com/playlist/{playlist_id}"
                 playlist_name = f"{month} '{year[2:]}"
 
                 console.rule(
                     f"Sorting into playlist [link={playlist_url}]{playlist_name}[/link]"
                 )
```

### Comparing `monthify-0.3.4/monthify/track.py` & `monthify-0.3.5/monthify/track.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Parses and stores data such as title and artist about tracks retrieved from the spotify api
     """
 
     title: str
     artist: str
     added_at: str
     uri: str
-    track_month: tuple[str] = field(init=False, repr=False)
+    track_month: tuple[str, str] = field(init=False, repr=False)
 
     def __post_init__(self):
         self.track_month = extract_month_and_year(self.added_at)
 
     def __repr__(self):
         cls = self.__class__
         cls_name = cls.__name__
```

### Comparing `monthify-0.3.4/monthify/utils.py` & `monthify-0.3.5/monthify/utils.py`

 * *Files identical despite different names*

### Comparing `monthify-0.3.4/pyproject.toml` & `monthify-0.3.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "monthify"
-version = "0.3.4"
+version = "0.3.5"
 description = "Sorts liked spotify tracks into playlists by the month they were liked."
 authors = ["Madiba Hudson-Quansah <mhquansah@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 loguru = "^0.6.0"
```

### Comparing `monthify-0.3.4/PKG-INFO` & `monthify-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monthify
-Version: 0.3.4
+Version: 0.3.5
 Summary: Sorts liked spotify tracks into playlists by the month they were liked.
 Author: Madiba Hudson-Quansah
 Author-email: mhquansah@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

