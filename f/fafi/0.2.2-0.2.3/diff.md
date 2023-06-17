# Comparing `tmp/fafi-0.2.2.tar.gz` & `tmp/fafi-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fafi-0.2.2.tar", max compression
+gzip compressed data, was "fafi-0.2.3.tar", max compression
```

## Comparing `fafi-0.2.2.tar` & `fafi-0.2.3.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1296 2022-06-29 10:46:09.121408 fafi-0.2.2/README.rst
--rw-r--r--   0        0        0      483 2022-09-10 11:41:45.524337 fafi-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       22 2022-09-10 11:42:00.545663 fafi-0.2.2/src/fafi/__init__.py
--rw-r--r--   0        0        0     2382 2022-09-10 11:38:24.949796 fafi-0.2.2/src/fafi/appdata.py
--rw-r--r--   0        0        0     1614 2022-09-10 11:38:24.950362 fafi-0.2.2/src/fafi/core.py
--rw-r--r--   0        0        0     1668 2022-09-10 11:38:24.950672 fafi-0.2.2/src/fafi/db.py
--rw-r--r--   0        0        0      296 2022-09-10 11:38:24.951028 fafi-0.2.2/src/fafi/input.py
--rwxr-xr-x   0        0        0     1751 2022-09-10 11:38:24.951667 fafi-0.2.2/src/fafi/main.py
--rw-r--r--   0        0        0     2163 2022-09-10 11:42:53.254035 fafi-0.2.2/setup.py
--rw-r--r--   0        0        0     1938 2022-09-10 11:42:53.254459 fafi-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1236 2023-06-17 18:05:31.737631 fafi-0.2.3/README.rst
+-rw-r--r--   0        0        0      573 2023-06-17 18:23:47.883505 fafi-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-17 18:23:40.393259 fafi-0.2.3/src/fafi/__init__.py
+-rw-r--r--   0        0        0     1298 2023-06-17 18:05:48.554677 fafi-0.2.3/src/fafi/appdata.py
+-rw-r--r--   0        0        0     1290 2023-06-17 18:05:48.554917 fafi-0.2.3/src/fafi/core.py
+-rw-r--r--   0        0        0     1908 2023-06-17 17:42:44.024454 fafi-0.2.3/src/fafi/db.py
+-rw-r--r--   0        0        0     2629 2023-06-17 18:05:48.555180 fafi-0.2.3/src/fafi/import_firefox.py
+-rw-r--r--   0        0        0      674 2023-06-17 18:05:48.555418 fafi-0.2.3/src/fafi/import_list.py
+-rw-r--r--   0        0        0      296 2022-09-10 11:38:24.951028 fafi-0.2.3/src/fafi/input.py
+-rwxr-xr-x   0        0        0     3218 2023-06-17 18:05:48.555760 fafi-0.2.3/src/fafi/main.py
+-rw-r--r--   0        0        0     1771 1970-01-01 00:00:00.000000 fafi-0.2.3/PKG-INFO
```

### Comparing `fafi-0.2.2/README.rst` & `fafi-0.2.3/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,45 @@
 
 Fafi
 ====
 
-Search Firefox bookmark contents, with this commandline client. Fafi extracts the content of the bookmarks and stores them into a searchable SQLite database.
+Fafi (short for Favorites Finder) is a commandline client to search indexed webpages. Fafi extracts the content of the webpage and stores them into a full-text search database.
 
 Things it does:
 
-
-* Detects your places database from the Firefox profile folder. (support for picking a profile from multiple profiles)
-* Extract main text content from all bookmarks into ``<user_data_dir>/fafi/data.sqlite``.
-* Skips .local and .test domains.
-* Skips pages that are already indexed.
+* Index single urls, text files containing urls, firefox profiles.
+* Incrementally indexing the places database from the Firefox profile folder. (The browser bookmarks) It supports picking a profile from multiple profiles.
+* Extract main text content.
+* Skips .local, localhost and .test domains.
+* Deduplication
 * Search results are ranked by relevance and displayed with snippets.
 
-URLs are stored together with the main page context as determined by `Newspaper <https://github.com/codelucas/newspaper>`_.
+Content extraction courtesy of `Newspaper <https://github.com/codelucas/newspaper>`_.
 
 Users
 -----
 
 .. code-block::
 
    pipx install fafi
    fafi --help
-   fafi index
+   fafi index --firefox
+   fafi index --url=https://mylink
+   fafi index --list=bookmarks.html
    fafi search 'linux'
 
 Developers
 ----------
 
 .. code-block::
 
    # Install project requirements.
    poetry install
 
-   # Log in to a python shell
-   poetry shell
-
-   # Help on commands
-   ./fafi.py --help
-   
-   # Index bookmarks
-   ./fafi.py index
-
-   # Search for linux
-   ./fafi.py search 'linux'
-
-
-.. image:: https://user-images.githubusercontent.com/594871/76201330-ffcba880-61ea-11ea-9fdd-cc32a90deecd.png
-   :target: https://user-images.githubusercontent.com/594871/76201330-ffcba880-61ea-11ea-9fdd-cc32a90deecd.png
-   :alt: search query
+   # Help
+   poetry run fafi --help
+ 
+
+.. image:: https://github.com/svandragt/fafi/assets/594871/d70bd34c-009c-4ead-9083-1ddc9a88ec29
+   :target: https://github.com/svandragt/fafi/assets/594871/d70bd34c-009c-4ead-9083-1ddc9a88ec29
+   :alt: TUI results for search query "linux"
```

### Comparing `fafi-0.2.2/src/fafi/appdata.py` & `fafi-0.2.3/src/fafi/import_firefox.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,103 +1,96 @@
-import appdirs
-import configparser
+"""
+Import Firefox bookmarks by indexing the user profile's placesdb.
+"""
+
 import datetime
 import os
-import shutil
-import tempfile
+from contextlib import closing
+
+import appdirs
 
-# fafi
-from . import db
+from fafi import appdata, db, core, input
 
-config = None
 
-def get_firefox_path():
+def _get_application_data_path():
     return appdirs.user_data_dir("Firefox")
 
 
-def get_places_dbs():
+def _get_places_dbs():
     # set the path of firefox folder with databases
-    ff_path = get_firefox_path()
+    ff_path = _get_application_data_path()
 
     # recursively walk tha path
     db_paths = []
     for root, dirs, files in os.walk(ff_path + "/Profiles/"):
         for name in files:
             if name == "places.sqlite":
                 db_path = str(root + os.sep + name).strip()
                 db_paths.append(db_path)
 
     return db_paths
 
 
-def data_path(silent=False):
-    sqlite_path = get_data_dir() + "/data.sqlite"
-    if not silent:
-        print("Store: " + sqlite_path)
-    return sqlite_path
-
-
-def get_data_dir():
-    data_dir = appdirs.user_data_dir("fafi")
-    if not os.path.exists(data_dir):
-        os.makedirs(data_dir)
-    return data_dir
+def index():
+    places_dbs = _get_places_dbs()
+    if places_dbs:
+        config = appdata.load_config()
+        try:
+            places_db = config['DEFAULT']['firefox_places_db']
+        except KeyError:
+            try:
+                places_db = config['DEFAULT']['places_db']
+                appdata.save_config('places_db', None)
+            except KeyError:
+                places_db = None
+
+        # Handle profile deletion
+        if not os.path.exists(places_db):
+            places_db = None
+
+        if not places_db:
+            choice = input.let_user_pick(places_dbs)
+            places_db = places_dbs[choice - 1]
+            appdata.save_config('firefox_places_db', places_db)
+
+        print('Places:', places_db)
+        _index_with_places(places_db)
+    else:
+        print('ERROR: Places database not found')
+
+
+def _index_with_places(places_db):
+    temp_path = appdata.create_temporary_copy(places_db)
+
+    with db.connect(temp_path) as places:
+        with closing(places.cursor()) as ff_cursor:
+            ff_cursor = _select_bookmarks(ff_cursor)
+
+            for row in ff_cursor:
+                core.index_site(url=row[0], date_bm_added=row[2])
+            else:
+                print('\nAll bookmarks are indexed.')
+
+    os.remove(temp_path)
 
 
-# get bookmarks from firefox sqlite database file and print all
-def select_bookmarks(cursor):
+def _select_bookmarks(cursor):
+    # get bookmarks from firefox sqlite database file and print all
     bookmarks_query = """
     SELECT DISTINCT
         url, moz_places.title, dateAdded from moz_places  
     JOIN 
         moz_bookmarks on moz_bookmarks.fk=moz_places.id 
     WHERE 
         moz_places.url like 'http%' and dateAdded > ?
     ORDER BY 
         dateAdded ASC
     """
-    bm_date = get_last_row_bm_date()
+    bm_date = appdata.get_last_row_bm_date()
     if not bm_date:
         bm_date = 100000
     d = datetime.datetime.fromtimestamp(bm_date / 1000000)
-    print("Indexing bookmarks added after: " + str(d))
-    db.execute_query(cursor, bookmarks_query, [bm_date])
-    return cursor
-
-
-def create_temporary_copy(path):
-    temp_dir = tempfile.gettempdir()
-    temp_path = os.path.join(temp_dir, "temp_file_name")
-    shutil.copy2(path, temp_path)
-    return temp_path
-
-
-def get_last_row_bm_date():
-    sqlite_path = data_path(silent=True)
-    with db.connect(sqlite_path) as fafi:
-        db.create_table(fafi)
 
-        return db.last_row_bm_date(fafi)
-
-
-def get_config_path():
-    return get_data_dir() + "/config.ini"
-
-
-def load_config():
-    global config
-
-    if not config:
-        config = configparser.ConfigParser()
-        config.read(get_config_path())
-
-    return config
-
-
-def save_config(name, value):
-    global config
-    config = load_config()
-
-    config['DEFAULT'][name] = value
+    print("Indexing bookmarks added after:", str(d))
+    db.execute_query(cursor, bookmarks_query, [bm_date])
 
-    with open(get_config_path(), 'w') as configfile:  # save
-        config.write(configfile)
+    return cursor
```

### Comparing `fafi-0.2.2/src/fafi/db.py` & `fafi-0.2.3/src/fafi/db.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,18 +19,19 @@
 
 def create_table(conn):
     """ create a table from the table_sql statement
     :param conn: Connection object
     :return:
     """
     c = conn.cursor()
-    c.execute(
-        "CREATE VIRTUAL TABLE IF NOT EXISTS sites USING FTS5(url, text, date_bm_added)"
-    )
+    c.execute( "CREATE VIRTUAL TABLE IF NOT EXISTS sites2 USING FTS5(title, url, text, date_bm_added)")
+    c.execute( "INSERT OR IGNORE INTO sites2 (url, text, date_bm_added) SELECT url, text, date_bm_added FROM sites")
+    c.execute( "DELETE FROM sites")
     conn.commit()
+    c.execute("VACUUM")
 
 
 # execute a query on sqlite cursor
 def execute_query(cursor, query, args=None):
     try:
         if args:
             cursor.execute(query, args)
@@ -39,37 +40,39 @@
     except Exception as error:
         print(str(error) + "\n " + query)
 
 
 def search(conn, keywords, max_results):
     cursor = conn.execute(
         """SELECT 
+                title,
                 url, 
-                snippet(sites, 1,'[', ']', '...',32) 
+                snippet(sites2, 2,'[', ']', '...',64) 
             FROM 
-                sites 
+                sites2 
             WHERE 
-                text MATCH ? 
+                title MATCH ? OR
+                text MATCH ?
             ORDER BY 
                 rank 
             LIMIT ?
         """,
-        (keywords, max_results),
+        (keywords, keywords, max_results),
     )
     if cursor.rowcount == 0:
         return None
     return cursor
 
 
 def last_row_bm_date(conn):
     cursor = conn.execute(
         """SELECT 
                 date_bm_added
             FROM 
-                sites
+                sites2
             ORDER by date_bm_added DESC
             LIMIT 1
         """
     )
     if cursor.rowcount == 0:
         return None
```

