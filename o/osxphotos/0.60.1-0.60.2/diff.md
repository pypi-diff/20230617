# Comparing `tmp/osxphotos-0.60.1.tar.gz` & `tmp/osxphotos-0.60.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osxphotos-0.60.1.tar", last modified: Sun May 14 15:28:30 2023, max compression
+gzip compressed data, was "osxphotos-0.60.2.tar", last modified: Sat Jun 17 14:16:34 2023, max compression
```

## Comparing `osxphotos-0.60.1.tar` & `osxphotos-0.60.2.tar`

### file list

```diff
@@ -1,232 +1,232 @@
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-14 15:28:30.485674 osxphotos-0.60.1/
--rw-r--r--   0 rhet       (501) staff       (20)     1075 2021-01-12 14:41:12.000000 osxphotos-0.60.1/LICENSE
--rw-r--r--   0 rhet       (501) staff       (20)      212 2022-04-19 16:54:15.000000 osxphotos-0.60.1/MANIFEST.in
--rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-05-14 15:28:30.485482 osxphotos-0.60.1/PKG-INFO
--rw-r--r--   0 rhet       (501) staff       (20)   224064 2023-05-14 15:28:19.000000 osxphotos-0.60.1/README.md
--rw-r--r--   0 rhet       (501) staff       (20)    12887 2023-03-09 14:25:54.000000 osxphotos-0.60.1/README.rst
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-14 15:28:30.424011 osxphotos-0.60.1/osxphotos/
--rw-r--r--   0 rhet       (501) staff       (20)     1952 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)      118 2022-02-27 00:52:03.000000 osxphotos-0.60.1/osxphotos/__main__.py
--rw-r--r--   0 rhet       (501) staff       (20)    15945 2023-05-07 15:00:00.000000 osxphotos-0.60.1/osxphotos/_constants.py
--rw-r--r--   0 rhet       (501) staff       (20)       45 2023-05-14 15:28:16.000000 osxphotos-0.60.1/osxphotos/_version.py
--rw-r--r--   0 rhet       (501) staff       (20)     5986 2022-01-22 17:23:57.000000 osxphotos-0.60.1/osxphotos/adjustmentsinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    18200 2023-04-11 02:03:56.000000 osxphotos-0.60.1/osxphotos/albuminfo.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-14 15:28:30.435499 osxphotos-0.60.1/osxphotos/cli/
--rw-r--r--   0 rhet       (501) staff       (20)     3565 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/cli/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)    15763 2022-05-18 03:47:35.000000 osxphotos-0.60.1/osxphotos/cli/about.py
--rw-r--r--   0 rhet       (501) staff       (20)     6869 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/cli/add_locations.py
--rw-r--r--   0 rhet       (501) staff       (20)     1313 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/albums.py
--rw-r--r--   0 rhet       (501) staff       (20)     9933 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/cli/batch_edit.py
--rw-r--r--   0 rhet       (501) staff       (20)     3802 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/cli/cli.py
--rw-r--r--   0 rhet       (501) staff       (20)    10147 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/cli_commands.py
--rw-r--r--   0 rhet       (501) staff       (20)    26594 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/cli/cli_params.py
--rw-r--r--   0 rhet       (501) staff       (20)     8531 2023-05-07 14:33:19.000000 osxphotos-0.60.1/osxphotos/cli/click_rich_echo.py
--rw-r--r--   0 rhet       (501) staff       (20)     6843 2022-05-01 15:18:25.000000 osxphotos-0.60.1/osxphotos/cli/color_themes.py
--rw-r--r--   0 rhet       (501) staff       (20)     3555 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/common.py
--rw-r--r--   0 rhet       (501) staff       (20)      713 2023-05-07 14:33:19.000000 osxphotos-0.60.1/osxphotos/cli/darkmode.py
--rw-r--r--   0 rhet       (501) staff       (20)     3615 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/debug_dump.py
--rw-r--r--   0 rhet       (501) staff       (20)     2265 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/docs.py
--rw-r--r--   0 rhet       (501) staff       (20)     3452 2023-05-07 14:33:19.000000 osxphotos-0.60.1/osxphotos/cli/dump.py
--rw-r--r--   0 rhet       (501) staff       (20)    15185 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/exiftool_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)   106908 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/cli/export.py
--rw-r--r--   0 rhet       (501) staff       (20)    17529 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/exportdb.py
--rw-r--r--   0 rhet       (501) staff       (20)     1649 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/grep.py
--rw-r--r--   0 rhet       (501) staff       (20)    22101 2023-05-07 14:33:19.000000 osxphotos-0.60.1/osxphotos/cli/help.py
--rw-r--r--   0 rhet       (501) staff       (20)    61649 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/cli/import_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)     2292 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/info.py
--rw-r--r--   0 rhet       (501) staff       (20)     2479 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/install_uninstall_run.py
--rw-r--r--   0 rhet       (501) staff       (20)     1103 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/keywords.py
--rw-r--r--   0 rhet       (501) staff       (20)     1327 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/kvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)     1106 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/labels.py
--rw-r--r--   0 rhet       (501) staff       (20)     1720 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/list.py
--rw-r--r--   0 rhet       (501) staff       (20)     5119 2023-02-12 16:12:07.000000 osxphotos-0.60.1/osxphotos/cli/orphans.py
--rw-r--r--   0 rhet       (501) staff       (20)     9657 2023-05-07 14:33:19.000000 osxphotos-0.60.1/osxphotos/cli/param_types.py
--rw-r--r--   0 rhet       (501) staff       (20)     1101 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/persons.py
--rw-r--r--   0 rhet       (501) staff       (20)    20564 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/cli/photo_inspect.py
--rw-r--r--   0 rhet       (501) staff       (20)     1860 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/places.py
--rw-r--r--   0 rhet       (501) staff       (20)     4585 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/print_photo_info.py
--rw-r--r--   0 rhet       (501) staff       (20)     5674 2023-05-07 14:33:19.000000 osxphotos-0.60.1/osxphotos/cli/query.py
--rw-r--r--   0 rhet       (501) staff       (20)     7833 2023-05-07 14:33:19.000000 osxphotos-0.60.1/osxphotos/cli/repl.py
--rw-r--r--   0 rhet       (501) staff       (20)    23058 2023-05-07 14:33:19.000000 osxphotos-0.60.1/osxphotos/cli/report_writer.py
--rw-r--r--   0 rhet       (501) staff       (20)     1930 2022-03-06 01:00:55.000000 osxphotos-0.60.1/osxphotos/cli/rich_progress.py
--rw-r--r--   0 rhet       (501) staff       (20)     3355 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/cli/show_command.py
--rw-r--r--   0 rhet       (501) staff       (20)     5080 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/snap_diff.py
--rw-r--r--   0 rhet       (501) staff       (20)    26935 2023-05-07 14:33:19.000000 osxphotos-0.60.1/osxphotos/cli/sync.py
--rw-r--r--   0 rhet       (501) staff       (20)     5675 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/sync_results.py
--rw-r--r--   0 rhet       (501) staff       (20)     4054 2022-04-18 05:53:56.000000 osxphotos-0.60.1/osxphotos/cli/theme.py
--rw-r--r--   0 rhet       (501) staff       (20)    28044 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/cli/timewarp.py
--rw-r--r--   0 rhet       (501) staff       (20)     1212 2022-02-27 00:52:03.000000 osxphotos-0.60.1/osxphotos/cli/tutorial.py
--rw-r--r--   0 rhet       (501) staff       (20)      692 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/cli/uuid.py
--rw-r--r--   0 rhet       (501) staff       (20)     8720 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/verbose.py
--rw-r--r--   0 rhet       (501) staff       (20)     1260 2023-02-03 04:08:06.000000 osxphotos-0.60.1/osxphotos/cli/version.py
--rw-r--r--   0 rhet       (501) staff       (20)     5089 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/compare_exif.py
--rw-r--r--   0 rhet       (501) staff       (20)     8060 2023-04-08 16:08:11.000000 osxphotos-0.60.1/osxphotos/configoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)     2084 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/crash_reporter.py
--rw-r--r--   0 rhet       (501) staff       (20)     1631 2022-01-22 17:24:00.000000 osxphotos-0.60.1/osxphotos/datetime_formatter.py
--rw-r--r--   0 rhet       (501) staff       (20)     6211 2023-05-07 14:33:19.000000 osxphotos-0.60.1/osxphotos/datetime_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3612 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/debug.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-14 15:28:30.436446 osxphotos-0.60.1/osxphotos/docs/
--rw-r--r--   0 rhet       (501) staff       (20)      165 2022-05-24 06:26:41.000000 osxphotos-0.60.1/osxphotos/docs/README.md
--rw-r--r--   0 rhet       (501) staff       (20)  1467005 2023-05-14 15:28:27.000000 osxphotos-0.60.1/osxphotos/docs/docs.zip
--rw-r--r--   0 rhet       (501) staff       (20)    13126 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/exif_datetime_updater.py
--rw-r--r--   0 rhet       (501) staff       (20)      622 2022-01-22 17:22:59.000000 osxphotos-0.60.1/osxphotos/exifinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    18945 2023-04-02 19:36:56.000000 osxphotos-0.60.1/osxphotos/exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)   116283 2022-02-07 05:54:46.000000 osxphotos-0.60.1/osxphotos/exiftool_filetypes.json
--rw-r--r--   0 rhet       (501) staff       (20)    51790 2023-05-14 15:28:03.000000 osxphotos-0.60.1/osxphotos/export_db.py
--rw-r--r--   0 rhet       (501) staff       (20)    19809 2023-04-08 16:08:11.000000 osxphotos-0.60.1/osxphotos/export_db_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    10742 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/fileutil.py
--rw-r--r--   0 rhet       (501) staff       (20)     5936 2023-04-08 16:08:11.000000 osxphotos-0.60.1/osxphotos/frozen_photoinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5121 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/imageconverter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2514 2022-05-04 05:28:10.000000 osxphotos-0.60.1/osxphotos/momentinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     3787 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/path_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    16570 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/personinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     9696 2023-04-08 16:08:11.000000 osxphotos-0.60.1/osxphotos/photodates.py
--rw-r--r--   0 rhet       (501) staff       (20)    89066 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/photoexporter.py
--rw-r--r--   0 rhet       (501) staff       (20)    80700 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/photoinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    46258 2023-05-07 14:33:19.000000 osxphotos-0.60.1/osxphotos/photokit.py
--rw-r--r--   0 rhet       (501) staff       (20)     5542 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/photosalbum.py
--rw-r--r--   0 rhet       (501) staff       (20)     5332 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/photoscript_utils.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-14 15:28:30.439611 osxphotos-0.60.1/osxphotos/photosdb/
--rw-r--r--   0 rhet       (501) staff       (20)      215 2020-08-09 15:12:11.000000 osxphotos-0.60.1/osxphotos/photosdb/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)     5386 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/photosdb/_photosdb_process_comments.py
--rw-r--r--   0 rhet       (501) staff       (20)     1789 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/photosdb/_photosdb_process_exif.py
--rw-r--r--   0 rhet       (501) staff       (20)    10393 2023-05-07 14:33:19.000000 osxphotos-0.60.1/osxphotos/photosdb/_photosdb_process_faceinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     6082 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/photosdb/_photosdb_process_scoreinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     7615 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/photosdb/_photosdb_process_searchinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)   149146 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/photosdb/photosdb.py
--rw-r--r--   0 rhet       (501) staff       (20)     5460 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/photosdb/photosdb_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     8564 2023-04-16 16:05:18.000000 osxphotos-0.60.1/osxphotos/phototables.py
--rw-r--r--   0 rhet       (501) staff       (20)     9930 2022-05-28 01:33:26.000000 osxphotos-0.60.1/osxphotos/phototemplate.cog.md
--rw-r--r--   0 rhet       (501) staff       (20)    13636 2023-05-14 15:28:19.000000 osxphotos-0.60.1/osxphotos/phototemplate.md
--rw-r--r--   0 rhet       (501) staff       (20)    78791 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/phototemplate.py
--rw-r--r--   0 rhet       (501) staff       (20)     1899 2022-08-27 02:50:57.000000 osxphotos-0.60.1/osxphotos/phototemplate.tx
--rw-r--r--   0 rhet       (501) staff       (20)     6680 2023-04-08 16:08:11.000000 osxphotos-0.60.1/osxphotos/phototz.py
--rw-r--r--   0 rhet       (501) staff       (20)    21858 2023-05-07 14:33:19.000000 osxphotos-0.60.1/osxphotos/placeinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     4486 2022-01-22 17:24:20.000000 osxphotos-0.60.1/osxphotos/pyrepl.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-14 15:28:30.440980 osxphotos-0.60.1/osxphotos/queries/
--rw-r--r--   0 rhet       (501) staff       (20)      167 2021-09-26 05:30:35.000000 osxphotos-0.60.1/osxphotos/queries/README.md
--rw-r--r--   0 rhet       (501) staff       (20)      157 2021-09-26 03:53:10.000000 osxphotos-0.60.1/osxphotos/queries/cloud_album_owner.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)     1139 2021-09-26 20:40:00.000000 osxphotos-0.60.1/osxphotos/queries/shared_owner.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)      231 2021-09-25 19:22:39.000000 osxphotos-0.60.1/osxphotos/queries/title.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)     1416 2022-01-22 17:22:59.000000 osxphotos-0.60.1/osxphotos/query_builder.py
--rw-r--r--   0 rhet       (501) staff       (20)    13457 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/queryoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)      496 2022-03-06 05:45:15.000000 osxphotos-0.60.1/osxphotos/rich_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     1144 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/scoreinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     7866 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/searchinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     2413 2023-05-07 14:33:19.000000 osxphotos-0.60.1/osxphotos/sqlgrep.py
--rw-r--r--   0 rhet       (501) staff       (20)     1813 2023-04-08 16:08:11.000000 osxphotos-0.60.1/osxphotos/sqlite_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     8064 2023-04-08 16:08:11.000000 osxphotos-0.60.1/osxphotos/sqlitekvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)     4150 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/template_counter.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-14 15:28:30.442050 osxphotos-0.60.1/osxphotos/templates/
--rw-r--r--   0 rhet       (501) staff       (20)      356 2021-01-20 23:58:08.000000 osxphotos-0.60.1/osxphotos/templates/DESCRIPTION.txt
--rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/templates/xmp_sidecar.mako
--rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/templates/xmp_sidecar_beta.mako
--rw-r--r--   0 rhet       (501) staff       (20)     3242 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/text_detection.py
--rw-r--r--   0 rhet       (501) staff       (20)     2282 2022-05-05 03:55:31.000000 osxphotos-0.60.1/osxphotos/timeutils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3442 2023-05-07 14:33:19.000000 osxphotos-0.60.1/osxphotos/timezones.py
--rw-r--r--   0 rhet       (501) staff       (20)    39982 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/tutorial.md
--rw-r--r--   0 rhet       (501) staff       (20)    27213 2023-05-07 14:33:19.000000 osxphotos-0.60.1/osxphotos/uti.py
--rw-r--r--   0 rhet       (501) staff       (20)    18621 2023-05-07 14:33:19.000000 osxphotos-0.60.1/osxphotos/utils.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-14 15:28:30.424732 osxphotos-0.60.1/osxphotos.egg-info/
--rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-05-14 15:28:30.000000 osxphotos-0.60.1/osxphotos.egg-info/PKG-INFO
--rw-r--r--   0 rhet       (501) staff       (20)     6344 2023-05-14 15:28:30.000000 osxphotos-0.60.1/osxphotos.egg-info/SOURCES.txt
--rw-r--r--   0 rhet       (501) staff       (20)        1 2023-05-14 15:28:30.000000 osxphotos-0.60.1/osxphotos.egg-info/dependency_links.txt
--rw-r--r--   0 rhet       (501) staff       (20)       58 2023-05-14 15:28:30.000000 osxphotos-0.60.1/osxphotos.egg-info/entry_points.txt
--rw-r--r--   0 rhet       (501) staff       (20)      888 2023-05-14 15:28:30.000000 osxphotos-0.60.1/osxphotos.egg-info/requires.txt
--rw-r--r--   0 rhet       (501) staff       (20)       16 2023-05-14 15:28:30.000000 osxphotos-0.60.1/osxphotos.egg-info/top_level.txt
--rw-r--r--   0 rhet       (501) staff       (20)       38 2023-05-14 15:28:30.485709 osxphotos-0.60.1/setup.cfg
--rwxr-xr-x   0 rhet       (501) staff       (20)     4378 2023-03-09 14:25:54.000000 osxphotos-0.60.1/setup.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-14 15:28:30.484725 osxphotos-0.60.1/tests/
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-14 15:28:30.485158 osxphotos-0.60.1/tests/plugins/
--rw-r--r--   0 rhet       (501) staff       (20)        0 2022-03-06 06:50:07.000000 osxphotos-0.60.1/tests/plugins/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)      167 2022-03-06 06:50:24.000000 osxphotos-0.60.1/tests/plugins/env_vars.py
--rw-r--r--   0 rhet       (501) staff       (20)     4551 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_10_12_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    11012 2022-02-07 05:54:47.000000 osxphotos-0.60.1/tests/test_albums_folders_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     4849 2021-06-12 05:33:53.000000 osxphotos-0.60.1/tests/test_albums_folders_high_sierra_10_13_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     5334 2021-06-12 05:33:48.000000 osxphotos-0.60.1/tests/test_albums_folders_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    43710 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_bigsur_10_16_0_1.py
--rw-r--r--   0 rhet       (501) staff       (20)    54731 2023-05-07 13:56:16.000000 osxphotos-0.60.1/tests/test_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)   273142 2023-05-07 14:25:27.000000 osxphotos-0.60.1/tests/test_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)     1798 2023-05-07 13:56:16.000000 osxphotos-0.60.1/tests/test_cli_add_locations.py
--rw-r--r--   0 rhet       (501) staff       (20)     4571 2023-05-07 13:56:16.000000 osxphotos-0.60.1/tests/test_cli_add_to_album.py
--rw-r--r--   0 rhet       (501) staff       (20)     2218 2023-05-07 13:56:16.000000 osxphotos-0.60.1/tests/test_cli_all_commands.py
--rw-r--r--   0 rhet       (501) staff       (20)     6798 2023-05-07 13:56:16.000000 osxphotos-0.60.1/tests/test_cli_batch_edit.py
--rw-r--r--   0 rhet       (501) staff       (20)     3696 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_cli_dump.py
--rw-r--r--   0 rhet       (501) staff       (20)     8091 2022-05-21 14:25:18.000000 osxphotos-0.60.1/tests/test_cli_exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)     2914 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_cli_export_cloud.py
--rw-r--r--   0 rhet       (501) staff       (20)      670 2023-04-08 21:34:18.000000 osxphotos-0.60.1/tests/test_cli_export_projects.py
--rw-r--r--   0 rhet       (501) staff       (20)     1009 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_cli_exportdb.py
--rw-r--r--   0 rhet       (501) staff       (20)    29996 2023-05-07 13:56:16.000000 osxphotos-0.60.1/tests/test_cli_import.py
--rw-r--r--   0 rhet       (501) staff       (20)      953 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_cli_orphans.py
--rw-r--r--   0 rhet       (501) staff       (20)     6397 2022-05-05 04:33:28.000000 osxphotos-0.60.1/tests/test_cli_param_types.py
--rw-r--r--   0 rhet       (501) staff       (20)     3450 2023-05-07 13:56:16.000000 osxphotos-0.60.1/tests/test_cli_sync.py
--rw-r--r--   0 rhet       (501) staff       (20)    31670 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_cli_timewarp.py
--rw-r--r--   0 rhet       (501) staff       (20)      815 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_cli_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3057 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_cli_verbose.py
--rw-r--r--   0 rhet       (501) staff       (20)     1185 2021-09-26 04:07:28.000000 osxphotos-0.60.1/tests/test_cloud_owner_catalina.py
--rw-r--r--   0 rhet       (501) staff       (20)     2644 2021-09-26 20:50:17.000000 osxphotos-0.60.1/tests/test_comments.py
--rw-r--r--   0 rhet       (501) staff       (20)     2519 2023-04-08 16:08:11.000000 osxphotos-0.60.1/tests/test_concurrent_export.py
--rw-r--r--   0 rhet       (501) staff       (20)     2699 2023-02-05 16:52:41.000000 osxphotos-0.60.1/tests/test_configoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)     1946 2023-05-07 13:56:16.000000 osxphotos-0.60.1/tests/test_datetime_formatter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2748 2022-05-06 13:53:04.000000 osxphotos-0.60.1/tests/test_datetime_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)      742 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_debug.py
--rw-r--r--   0 rhet       (501) staff       (20)     2209 2023-01-21 18:04:00.000000 osxphotos-0.60.1/tests/test_empty_library_4_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     2439 2022-01-02 15:24:11.000000 osxphotos-0.60.1/tests/test_exif_info.py
--rw-r--r--   0 rhet       (501) staff       (20)    18508 2023-05-07 13:56:16.000000 osxphotos-0.60.1/tests/test_exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)     9781 2021-04-26 00:13:29.000000 osxphotos-0.60.1/tests/test_exiftool_caching.py
--rw-r--r--   0 rhet       (501) staff       (20)    18308 2022-05-21 05:13:12.000000 osxphotos-0.60.1/tests/test_export_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     5910 2023-05-07 13:56:16.000000 osxphotos-0.60.1/tests/test_export_catalina_10_15_7_use_photos_export.py
--rw-r--r--   0 rhet       (501) staff       (20)     2836 2022-01-29 16:49:11.000000 osxphotos-0.60.1/tests/test_export_convert_to_jpeg.py
--rw-r--r--   0 rhet       (501) staff       (20)    21901 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_export_db.py
--rw-r--r--   0 rhet       (501) staff       (20)    10301 2022-05-21 05:13:12.000000 osxphotos-0.60.1/tests/test_export_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3892 2021-03-14 19:20:10.000000 osxphotos-0.60.1/tests/test_export_raw_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2484 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_exportresults.py
--rw-r--r--   0 rhet       (501) staff       (20)   155137 2022-06-17 17:31:26.000000 osxphotos-0.60.1/tests/test_faceinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5148 2023-05-07 13:56:16.000000 osxphotos-0.60.1/tests/test_fileutil.py
--rw-r--r--   0 rhet       (501) staff       (20)     3634 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_highsierra.py
--rw-r--r--   0 rhet       (501) staff       (20)     4022 2022-01-01 04:28:52.000000 osxphotos-0.60.1/tests/test_image_converter.py
--rw-r--r--   0 rhet       (501) staff       (20)     1211 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_incloud_big_sur_10_16_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     1327 2021-06-12 05:41:38.000000 osxphotos-0.60.1/tests/test_incloud_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     1944 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_incloud_catalina_10_15_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     1270 2021-06-12 05:43:32.000000 osxphotos-0.60.1/tests/test_incloud_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3786 2021-06-12 05:44:48.000000 osxphotos-0.60.1/tests/test_live_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)      859 2021-06-12 05:45:42.000000 osxphotos-0.60.1/tests/test_modified_date_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)      930 2021-06-12 05:46:24.000000 osxphotos-0.60.1/tests/test_modified_date_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    18573 2023-04-16 16:05:18.000000 osxphotos-0.60.1/tests/test_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     1205 2020-01-12 08:00:41.000000 osxphotos-0.60.1/tests/test_mojave_10_14_6_path_edited.py
--rw-r--r--   0 rhet       (501) staff       (20)    43640 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_monterey_12_0_1.py
--rw-r--r--   0 rhet       (501) staff       (20)    50393 2023-05-07 13:56:16.000000 osxphotos-0.60.1/tests/test_monterey_dev_beta_12_0_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     4731 2020-06-27 19:46:37.000000 osxphotos-0.60.1/tests/test_movies_4_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     4870 2020-06-27 19:50:41.000000 osxphotos-0.60.1/tests/test_movies_5_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     3780 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_path_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     4377 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_personinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    13430 2023-05-07 13:56:16.000000 osxphotos-0.60.1/tests/test_photokit.py
--rw-r--r--   0 rhet       (501) staff       (20)     1460 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_photosdb_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    13801 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_placeinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5796 2020-10-27 13:37:01.000000 osxphotos-0.60.1/tests/test_places_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     7224 2020-03-28 15:14:51.000000 osxphotos-0.60.1/tests/test_places_high_sierra_10_13_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3431 2020-10-27 13:36:55.000000 osxphotos-0.60.1/tests/test_places_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     4762 2023-04-08 16:49:38.000000 osxphotos-0.60.1/tests/test_projects_catalina.py
--rw-r--r--   0 rhet       (501) staff       (20)     4224 2021-12-31 05:42:49.000000 osxphotos-0.60.1/tests/test_projects_sierra.py
--rw-r--r--   0 rhet       (501) staff       (20)     3376 2022-01-02 07:10:11.000000 osxphotos-0.60.1/tests/test_score_info.py
--rw-r--r--   0 rhet       (501) staff       (20)     3696 2020-05-11 01:55:25.000000 osxphotos-0.60.1/tests/test_search_info_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     7530 2020-12-25 19:00:06.000000 osxphotos-0.60.1/tests/test_search_info_10_15_4.py
--rw-r--r--   0 rhet       (501) staff       (20)    10047 2022-01-18 16:08:28.000000 osxphotos-0.60.1/tests/test_search_info_10_15_5.py
--rw-r--r--   0 rhet       (501) staff       (20)     2191 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_search_info_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     2791 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_shared_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     1744 2020-10-05 13:13:43.000000 osxphotos-0.60.1/tests/test_shared_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)      441 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_shared_ventura_13_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2100 2022-01-29 16:49:32.000000 osxphotos-0.60.1/tests/test_sidecar_xmp.py
--rw-r--r--   0 rhet       (501) staff       (20)     3017 2020-08-23 23:26:56.000000 osxphotos-0.60.1/tests/test_specials_bigsur_10_16_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     2535 2020-03-08 17:47:46.000000 osxphotos-0.60.1/tests/test_specials_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2621 2020-03-28 14:53:05.000000 osxphotos-0.60.1/tests/test_specials_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     2261 2020-03-08 19:17:16.000000 osxphotos-0.60.1/tests/test_specials_sierra_10_12.py
--rw-r--r--   0 rhet       (501) staff       (20)      489 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_sqlite_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     7328 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_sqlitekvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)    50016 2023-05-07 13:56:16.000000 osxphotos-0.60.1/tests/test_template.py
--rw-r--r--   0 rhet       (501) staff       (20)     2432 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_template_counter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2346 2023-05-07 13:56:16.000000 osxphotos-0.60.1/tests/test_template_today.py
--rw-r--r--   0 rhet       (501) staff       (20)     2032 2023-05-07 13:56:16.000000 osxphotos-0.60.1/tests/test_uti.py
--rw-r--r--   0 rhet       (501) staff       (20)     5514 2023-04-08 16:08:11.000000 osxphotos-0.60.1/tests/test_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    48316 2023-04-16 16:05:18.000000 osxphotos-0.60.1/tests/test_ventura_13_0_0.py
--rw-r--r--   0 rhet       (501) staff       (20)    43504 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_ventura_dev_preview_13_0_0.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-17 14:16:34.568291 osxphotos-0.60.2/
+-rw-r--r--   0 rhet       (501) staff       (20)     1075 2021-01-12 14:41:12.000000 osxphotos-0.60.2/LICENSE
+-rw-r--r--   0 rhet       (501) staff       (20)      212 2022-04-19 16:54:15.000000 osxphotos-0.60.2/MANIFEST.in
+-rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-06-17 14:16:34.568103 osxphotos-0.60.2/PKG-INFO
+-rw-r--r--   0 rhet       (501) staff       (20)   224169 2023-06-17 14:16:23.000000 osxphotos-0.60.2/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)    12887 2023-03-09 14:25:54.000000 osxphotos-0.60.2/README.rst
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-17 14:16:34.542224 osxphotos-0.60.2/osxphotos/
+-rw-r--r--   0 rhet       (501) staff       (20)     1952 2023-05-07 13:56:16.000000 osxphotos-0.60.2/osxphotos/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)      118 2022-02-27 00:52:03.000000 osxphotos-0.60.2/osxphotos/__main__.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15945 2023-05-07 15:00:00.000000 osxphotos-0.60.2/osxphotos/_constants.py
+-rw-r--r--   0 rhet       (501) staff       (20)       45 2023-06-17 14:16:19.000000 osxphotos-0.60.2/osxphotos/_version.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5986 2022-01-22 17:23:57.000000 osxphotos-0.60.2/osxphotos/adjustmentsinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18200 2023-04-11 02:03:56.000000 osxphotos-0.60.2/osxphotos/albuminfo.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-17 14:16:34.550678 osxphotos-0.60.2/osxphotos/cli/
+-rw-r--r--   0 rhet       (501) staff       (20)     3565 2023-06-16 15:10:56.000000 osxphotos-0.60.2/osxphotos/cli/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15763 2022-05-18 03:47:35.000000 osxphotos-0.60.2/osxphotos/cli/about.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6869 2023-05-07 13:56:16.000000 osxphotos-0.60.2/osxphotos/cli/add_locations.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1313 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/albums.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9933 2023-05-07 13:56:16.000000 osxphotos-0.60.2/osxphotos/cli/batch_edit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3802 2023-05-07 13:56:16.000000 osxphotos-0.60.2/osxphotos/cli/cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10147 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/cli_commands.py
+-rw-r--r--   0 rhet       (501) staff       (20)    26594 2023-06-16 15:10:56.000000 osxphotos-0.60.2/osxphotos/cli/cli_params.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8531 2023-05-07 14:33:19.000000 osxphotos-0.60.2/osxphotos/cli/click_rich_echo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6843 2022-05-01 15:18:25.000000 osxphotos-0.60.2/osxphotos/cli/color_themes.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3555 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/common.py
+-rw-r--r--   0 rhet       (501) staff       (20)      713 2023-06-16 15:10:56.000000 osxphotos-0.60.2/osxphotos/cli/darkmode.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3615 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/debug_dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2265 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/docs.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3452 2023-05-07 14:33:19.000000 osxphotos-0.60.2/osxphotos/cli/dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15185 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/exiftool_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)   106908 2023-05-07 13:56:16.000000 osxphotos-0.60.2/osxphotos/cli/export.py
+-rw-r--r--   0 rhet       (501) staff       (20)    17529 2023-06-16 15:10:56.000000 osxphotos-0.60.2/osxphotos/cli/exportdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1649 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/grep.py
+-rw-r--r--   0 rhet       (501) staff       (20)    22101 2023-05-07 14:33:19.000000 osxphotos-0.60.2/osxphotos/cli/help.py
+-rw-r--r--   0 rhet       (501) staff       (20)    61649 2023-05-07 13:56:16.000000 osxphotos-0.60.2/osxphotos/cli/import_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2292 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2479 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/install_uninstall_run.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1103 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/keywords.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1327 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/kvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1106 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/labels.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1720 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/list.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5119 2023-02-12 16:12:07.000000 osxphotos-0.60.2/osxphotos/cli/orphans.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9657 2023-05-07 14:33:19.000000 osxphotos-0.60.2/osxphotos/cli/param_types.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1101 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/persons.py
+-rw-r--r--   0 rhet       (501) staff       (20)    20564 2023-05-07 13:56:16.000000 osxphotos-0.60.2/osxphotos/cli/photo_inspect.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1860 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/places.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4585 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/print_photo_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5674 2023-06-16 15:10:56.000000 osxphotos-0.60.2/osxphotos/cli/query.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7833 2023-05-07 14:33:19.000000 osxphotos-0.60.2/osxphotos/cli/repl.py
+-rw-r--r--   0 rhet       (501) staff       (20)    23058 2023-05-07 14:33:19.000000 osxphotos-0.60.2/osxphotos/cli/report_writer.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1930 2022-03-06 01:00:55.000000 osxphotos-0.60.2/osxphotos/cli/rich_progress.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3355 2023-06-16 15:10:56.000000 osxphotos-0.60.2/osxphotos/cli/show_command.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5080 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/snap_diff.py
+-rw-r--r--   0 rhet       (501) staff       (20)    26935 2023-05-07 14:33:19.000000 osxphotos-0.60.2/osxphotos/cli/sync.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5675 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/sync_results.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4054 2022-04-18 05:53:56.000000 osxphotos-0.60.2/osxphotos/cli/theme.py
+-rw-r--r--   0 rhet       (501) staff       (20)    28044 2023-06-16 15:10:56.000000 osxphotos-0.60.2/osxphotos/cli/timewarp.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1212 2022-02-27 00:52:03.000000 osxphotos-0.60.2/osxphotos/cli/tutorial.py
+-rw-r--r--   0 rhet       (501) staff       (20)      692 2023-05-07 13:56:16.000000 osxphotos-0.60.2/osxphotos/cli/uuid.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8720 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/verbose.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1260 2023-06-16 15:10:56.000000 osxphotos-0.60.2/osxphotos/cli/version.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5089 2023-06-16 15:10:56.000000 osxphotos-0.60.2/osxphotos/compare_exif.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8060 2023-04-08 16:08:11.000000 osxphotos-0.60.2/osxphotos/configoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2084 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/crash_reporter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1631 2022-01-22 17:24:00.000000 osxphotos-0.60.2/osxphotos/datetime_formatter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6211 2023-05-07 14:33:19.000000 osxphotos-0.60.2/osxphotos/datetime_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3612 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/debug.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-17 14:16:34.551104 osxphotos-0.60.2/osxphotos/docs/
+-rw-r--r--   0 rhet       (501) staff       (20)      165 2022-05-24 06:26:41.000000 osxphotos-0.60.2/osxphotos/docs/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)  1467985 2023-06-17 14:16:30.000000 osxphotos-0.60.2/osxphotos/docs/docs.zip
+-rw-r--r--   0 rhet       (501) staff       (20)    13126 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/exif_datetime_updater.py
+-rw-r--r--   0 rhet       (501) staff       (20)      622 2022-01-22 17:22:59.000000 osxphotos-0.60.2/osxphotos/exifinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18945 2023-04-02 19:36:56.000000 osxphotos-0.60.2/osxphotos/exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)   116283 2022-02-07 05:54:46.000000 osxphotos-0.60.2/osxphotos/exiftool_filetypes.json
+-rw-r--r--   0 rhet       (501) staff       (20)    51790 2023-06-17 04:33:59.000000 osxphotos-0.60.2/osxphotos/export_db.py
+-rw-r--r--   0 rhet       (501) staff       (20)    19809 2023-04-08 16:08:11.000000 osxphotos-0.60.2/osxphotos/export_db_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10742 2023-05-07 13:56:16.000000 osxphotos-0.60.2/osxphotos/fileutil.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5936 2023-04-08 16:08:11.000000 osxphotos-0.60.2/osxphotos/frozen_photoinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5121 2023-06-16 15:10:56.000000 osxphotos-0.60.2/osxphotos/imageconverter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2514 2022-05-04 05:28:10.000000 osxphotos-0.60.2/osxphotos/momentinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3787 2023-05-07 13:56:16.000000 osxphotos-0.60.2/osxphotos/path_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    16570 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/personinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9696 2023-04-08 16:08:11.000000 osxphotos-0.60.2/osxphotos/photodates.py
+-rw-r--r--   0 rhet       (501) staff       (20)    91520 2023-06-17 14:14:35.000000 osxphotos-0.60.2/osxphotos/photoexporter.py
+-rw-r--r--   0 rhet       (501) staff       (20)    81384 2023-06-17 14:14:35.000000 osxphotos-0.60.2/osxphotos/photoinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    46258 2023-05-07 14:33:19.000000 osxphotos-0.60.2/osxphotos/photokit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5542 2023-05-07 13:56:16.000000 osxphotos-0.60.2/osxphotos/photosalbum.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5332 2023-05-07 13:56:16.000000 osxphotos-0.60.2/osxphotos/photoscript_utils.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-17 14:16:34.553485 osxphotos-0.60.2/osxphotos/photosdb/
+-rw-r--r--   0 rhet       (501) staff       (20)      215 2023-06-16 15:10:56.000000 osxphotos-0.60.2/osxphotos/photosdb/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5386 2023-06-16 15:10:56.000000 osxphotos-0.60.2/osxphotos/photosdb/_photosdb_process_comments.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1789 2023-06-16 15:10:56.000000 osxphotos-0.60.2/osxphotos/photosdb/_photosdb_process_exif.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10393 2023-05-07 14:33:19.000000 osxphotos-0.60.2/osxphotos/photosdb/_photosdb_process_faceinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6082 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/photosdb/_photosdb_process_scoreinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7615 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/photosdb/_photosdb_process_searchinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)   149146 2023-06-17 01:41:30.000000 osxphotos-0.60.2/osxphotos/photosdb/photosdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5460 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/photosdb/photosdb_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8564 2023-04-16 16:05:18.000000 osxphotos-0.60.2/osxphotos/phototables.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9930 2022-05-28 01:33:26.000000 osxphotos-0.60.2/osxphotos/phototemplate.cog.md
+-rw-r--r--   0 rhet       (501) staff       (20)    13636 2023-06-17 14:16:22.000000 osxphotos-0.60.2/osxphotos/phototemplate.md
+-rw-r--r--   0 rhet       (501) staff       (20)    78791 2023-05-07 13:56:16.000000 osxphotos-0.60.2/osxphotos/phototemplate.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1899 2022-08-27 02:50:57.000000 osxphotos-0.60.2/osxphotos/phototemplate.tx
+-rw-r--r--   0 rhet       (501) staff       (20)     6680 2023-04-08 16:08:11.000000 osxphotos-0.60.2/osxphotos/phototz.py
+-rw-r--r--   0 rhet       (501) staff       (20)    21858 2023-05-07 14:33:19.000000 osxphotos-0.60.2/osxphotos/placeinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4486 2022-01-22 17:24:20.000000 osxphotos-0.60.2/osxphotos/pyrepl.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-17 14:16:34.554480 osxphotos-0.60.2/osxphotos/queries/
+-rw-r--r--   0 rhet       (501) staff       (20)      167 2021-09-26 05:30:35.000000 osxphotos-0.60.2/osxphotos/queries/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)      157 2021-09-26 03:53:10.000000 osxphotos-0.60.2/osxphotos/queries/cloud_album_owner.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     1139 2021-09-26 20:40:00.000000 osxphotos-0.60.2/osxphotos/queries/shared_owner.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)      231 2021-09-25 19:22:39.000000 osxphotos-0.60.2/osxphotos/queries/title.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     1416 2022-01-22 17:22:59.000000 osxphotos-0.60.2/osxphotos/query_builder.py
+-rw-r--r--   0 rhet       (501) staff       (20)    13457 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/queryoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)      496 2022-03-06 05:45:15.000000 osxphotos-0.60.2/osxphotos/rich_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1144 2023-06-16 15:10:56.000000 osxphotos-0.60.2/osxphotos/scoreinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7866 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/searchinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2413 2023-05-07 14:33:19.000000 osxphotos-0.60.2/osxphotos/sqlgrep.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1813 2023-04-08 16:08:11.000000 osxphotos-0.60.2/osxphotos/sqlite_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8064 2023-04-08 16:08:11.000000 osxphotos-0.60.2/osxphotos/sqlitekvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4150 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/template_counter.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-17 14:16:34.555271 osxphotos-0.60.2/osxphotos/templates/
+-rw-r--r--   0 rhet       (501) staff       (20)      356 2021-01-20 23:58:08.000000 osxphotos-0.60.2/osxphotos/templates/DESCRIPTION.txt
+-rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/templates/xmp_sidecar.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/templates/xmp_sidecar_beta.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     3242 2023-05-07 13:56:16.000000 osxphotos-0.60.2/osxphotos/text_detection.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2282 2023-06-16 15:10:56.000000 osxphotos-0.60.2/osxphotos/timeutils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3442 2023-05-07 14:33:19.000000 osxphotos-0.60.2/osxphotos/timezones.py
+-rw-r--r--   0 rhet       (501) staff       (20)    39982 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/tutorial.md
+-rw-r--r--   0 rhet       (501) staff       (20)    27213 2023-06-16 15:10:56.000000 osxphotos-0.60.2/osxphotos/uti.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18621 2023-06-17 14:12:56.000000 osxphotos-0.60.2/osxphotos/utils.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-17 14:16:34.543048 osxphotos-0.60.2/osxphotos.egg-info/
+-rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-06-17 14:16:34.000000 osxphotos-0.60.2/osxphotos.egg-info/PKG-INFO
+-rw-r--r--   0 rhet       (501) staff       (20)     6344 2023-06-17 14:16:34.000000 osxphotos-0.60.2/osxphotos.egg-info/SOURCES.txt
+-rw-r--r--   0 rhet       (501) staff       (20)        1 2023-06-17 14:16:34.000000 osxphotos-0.60.2/osxphotos.egg-info/dependency_links.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       58 2023-06-17 14:16:34.000000 osxphotos-0.60.2/osxphotos.egg-info/entry_points.txt
+-rw-r--r--   0 rhet       (501) staff       (20)      888 2023-06-17 14:16:34.000000 osxphotos-0.60.2/osxphotos.egg-info/requires.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       16 2023-06-17 14:16:34.000000 osxphotos-0.60.2/osxphotos.egg-info/top_level.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       38 2023-06-17 14:16:34.568332 osxphotos-0.60.2/setup.cfg
+-rwxr-xr-x   0 rhet       (501) staff       (20)     4378 2023-03-09 14:25:54.000000 osxphotos-0.60.2/setup.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-17 14:16:34.567603 osxphotos-0.60.2/tests/
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-17 14:16:34.567873 osxphotos-0.60.2/tests/plugins/
+-rw-r--r--   0 rhet       (501) staff       (20)        0 2022-03-06 06:50:07.000000 osxphotos-0.60.2/tests/plugins/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)      167 2022-03-06 06:50:24.000000 osxphotos-0.60.2/tests/plugins/env_vars.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4551 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_10_12_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    11012 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_albums_folders_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4849 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_albums_folders_high_sierra_10_13_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5334 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_albums_folders_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43710 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_bigsur_10_16_0_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)    54731 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)   273142 2023-06-16 16:22:37.000000 osxphotos-0.60.2/tests/test_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1798 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_cli_add_locations.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4571 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_cli_add_to_album.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2218 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_cli_all_commands.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6798 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_cli_batch_edit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3696 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_cli_dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8091 2022-05-21 14:25:18.000000 osxphotos-0.60.2/tests/test_cli_exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2914 2023-03-09 14:25:57.000000 osxphotos-0.60.2/tests/test_cli_export_cloud.py
+-rw-r--r--   0 rhet       (501) staff       (20)      670 2023-04-08 21:34:18.000000 osxphotos-0.60.2/tests/test_cli_export_projects.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1009 2023-03-09 14:25:57.000000 osxphotos-0.60.2/tests/test_cli_exportdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)    29996 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_cli_import.py
+-rw-r--r--   0 rhet       (501) staff       (20)      953 2023-03-09 14:25:57.000000 osxphotos-0.60.2/tests/test_cli_orphans.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6397 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_cli_param_types.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3450 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_cli_sync.py
+-rw-r--r--   0 rhet       (501) staff       (20)    31670 2023-03-09 14:25:57.000000 osxphotos-0.60.2/tests/test_cli_timewarp.py
+-rw-r--r--   0 rhet       (501) staff       (20)      815 2023-03-09 14:25:57.000000 osxphotos-0.60.2/tests/test_cli_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3057 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_cli_verbose.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1185 2021-09-26 04:07:28.000000 osxphotos-0.60.2/tests/test_cloud_owner_catalina.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2644 2021-09-26 20:50:17.000000 osxphotos-0.60.2/tests/test_comments.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2519 2023-04-08 16:08:11.000000 osxphotos-0.60.2/tests/test_concurrent_export.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2699 2023-02-05 16:52:41.000000 osxphotos-0.60.2/tests/test_configoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1946 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_datetime_formatter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2748 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_datetime_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)      742 2023-03-09 14:25:57.000000 osxphotos-0.60.2/tests/test_debug.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2209 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_empty_library_4_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2439 2022-01-02 15:24:11.000000 osxphotos-0.60.2/tests/test_exif_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18508 2023-05-07 13:56:16.000000 osxphotos-0.60.2/tests/test_exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9781 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_exiftool_caching.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18308 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_export_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5910 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_export_catalina_10_15_7_use_photos_export.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2836 2022-01-29 16:49:11.000000 osxphotos-0.60.2/tests/test_export_convert_to_jpeg.py
+-rw-r--r--   0 rhet       (501) staff       (20)    21901 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_export_db.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10301 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_export_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3892 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_export_raw_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2484 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_exportresults.py
+-rw-r--r--   0 rhet       (501) staff       (20)   155137 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_faceinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5148 2023-05-07 13:56:16.000000 osxphotos-0.60.2/tests/test_fileutil.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3634 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_highsierra.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4022 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_image_converter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1211 2023-03-09 14:25:57.000000 osxphotos-0.60.2/tests/test_incloud_big_sur_10_16_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1327 2021-06-12 05:41:38.000000 osxphotos-0.60.2/tests/test_incloud_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1944 2023-03-09 14:25:57.000000 osxphotos-0.60.2/tests/test_incloud_catalina_10_15_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1270 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_incloud_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3786 2021-06-12 05:44:48.000000 osxphotos-0.60.2/tests/test_live_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)      859 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_modified_date_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)      930 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_modified_date_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18573 2023-04-16 16:05:18.000000 osxphotos-0.60.2/tests/test_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1205 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_mojave_10_14_6_path_edited.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43640 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_monterey_12_0_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)    50393 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_monterey_dev_beta_12_0_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4731 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_movies_4_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4870 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_movies_5_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3780 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_path_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4377 2023-03-09 14:25:57.000000 osxphotos-0.60.2/tests/test_personinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    13430 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_photokit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1460 2023-03-09 14:25:57.000000 osxphotos-0.60.2/tests/test_photosdb_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    13801 2023-03-09 14:25:57.000000 osxphotos-0.60.2/tests/test_placeinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5796 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_places_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7224 2020-03-28 15:14:51.000000 osxphotos-0.60.2/tests/test_places_high_sierra_10_13_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3431 2020-10-27 13:36:55.000000 osxphotos-0.60.2/tests/test_places_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4762 2023-04-08 16:49:38.000000 osxphotos-0.60.2/tests/test_projects_catalina.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4224 2021-12-31 05:42:49.000000 osxphotos-0.60.2/tests/test_projects_sierra.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3376 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_score_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3696 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_search_info_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7530 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_search_info_10_15_4.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10047 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_search_info_10_15_5.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2191 2023-03-09 14:25:57.000000 osxphotos-0.60.2/tests/test_search_info_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2791 2023-03-09 14:25:57.000000 osxphotos-0.60.2/tests/test_shared_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1744 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_shared_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)      441 2023-03-09 14:25:57.000000 osxphotos-0.60.2/tests/test_shared_ventura_13_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2100 2022-01-29 16:49:32.000000 osxphotos-0.60.2/tests/test_sidecar_xmp.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3017 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_specials_bigsur_10_16_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2535 2020-03-08 17:47:46.000000 osxphotos-0.60.2/tests/test_specials_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2621 2020-03-28 14:53:05.000000 osxphotos-0.60.2/tests/test_specials_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2261 2020-03-08 19:17:16.000000 osxphotos-0.60.2/tests/test_specials_sierra_10_12.py
+-rw-r--r--   0 rhet       (501) staff       (20)      489 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_sqlite_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7328 2023-03-09 14:25:57.000000 osxphotos-0.60.2/tests/test_sqlitekvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)    50016 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_template.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2432 2023-03-09 14:25:57.000000 osxphotos-0.60.2/tests/test_template_counter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2346 2023-05-07 13:56:16.000000 osxphotos-0.60.2/tests/test_template_today.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2032 2023-05-07 13:56:16.000000 osxphotos-0.60.2/tests/test_uti.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5514 2023-04-08 16:08:11.000000 osxphotos-0.60.2/tests/test_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    48316 2023-04-16 16:05:18.000000 osxphotos-0.60.2/tests/test_ventura_13_0_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43504 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_ventura_dev_preview_13_0_0.py
```

### Comparing `osxphotos-0.60.1/LICENSE` & `osxphotos-0.60.2/LICENSE`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/PKG-INFO` & `osxphotos-0.60.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osxphotos
-Version: 0.60.1
+Version: 0.60.2
 Summary: Export photos from Apple's macOS Photos app and query the Photos library database to access metadata about images.
 Home-page: https://github.com/RhetTbull/
 Download-URL: https://github.com/RhetTbull/osxphotos
 Author: Rhet Turnbull
 Author-email: rturnbull+git@gmail.com
 License: License :: OSI Approved :: MIT License
 Project-URL: GitHub, https://github.com/RhetTbull/osxphotos
```

### Comparing `osxphotos-0.60.1/README.md` & `osxphotos-0.60.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2095,15 +2095,15 @@
 {openbracket}                   An open bracket: '['
 {closebracket}                  A close bracket: ']'
 {newline}                       A newline: '\n'
 {lf}                            A line feed: '\n', alias for {newline}
 {cr}                            A carriage return: '\r'
 {crlf}                          A carriage return + line feed: '\r\n'
 {tab}                           :A tab: '\t'
-{osxphotos_version}             The osxphotos version, e.g. '0.60.1'
+{osxphotos_version}             The osxphotos version, e.g. '0.60.2'
 {osxphotos_cmd_line}            The full command line used to run osxphotos
 
 The following substitutions may result in multiple values. Thus if specified
 for --directory these could result in multiple copies of a photo being being
 exported, one to each directory.  For example: --directory
 '{created.year}/{album}' could result in the same photo being exported to each
 of the following directories if the photos were created in 2019 and were in
@@ -2582,15 +2582,15 @@
 |{openbracket}|An open bracket: '['|
 |{closebracket}|A close bracket: ']'|
 |{newline}|A newline: '\n'|
 |{lf}|A line feed: '\n', alias for {newline}|
 |{cr}|A carriage return: '\r'|
 |{crlf}|A carriage return + line feed: '\r\n'|
 |{tab}|:A tab: '\t'|
-|{osxphotos_version}|The osxphotos version, e.g. '0.60.1'|
+|{osxphotos_version}|The osxphotos version, e.g. '0.60.2'|
 |{osxphotos_cmd_line}|The full command line used to run osxphotos|
 |{album}|Album(s) photo is contained in|
 |{folder_album}|Folder path + album photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder|
 |{project}|Project(s) photo is contained in (such as greeting cards, calendars, slideshows)|
 |{album_project}|Album(s) and project(s) photo is contained in; treats projects as regular albums|
 |{folder_album_project}|Folder path + album (includes projects as albums) photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder|
 |{keyword}|Keyword(s) assigned to photo|
@@ -2622,15 +2622,15 @@
 
 Contributing is easy!  if you find bugs or want to suggest additional features/changes, please open an [issue](https://github.com/rhettbull/osxphotos/issues/) or join the [discussion](https://github.com/RhetTbull/osxphotos/discussions).
 
 I'll gladly consider pull requests for bug fixes or feature implementations.  
 
 If you have an interesting example that shows usage of this package, submit an issue or pull request and i'll include it or link to it.
 
-Testing against "real world" Photos libraries would be especially helpful.  If you discover issues in testing against your Photos libraries, please open an issue.  I've done extensive testing against my own Photos library but that's a since data point and I'm certain there are issues lurking in various edge cases I haven't discovered yet.
+Testing against "real world" Photos libraries would be especially helpful.  If you discover issues in testing against your Photos libraries, please open an issue.  I've done extensive testing against my own Photos library but that's a single data point and I'm certain there are issues lurking in various edge cases I haven't discovered yet.
 
 ### Contributors ✨
 
 Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
@@ -2708,15 +2708,15 @@
       <td align="center" valign="top" width="14.28%"><a href="http://www.projany.com"><img src="https://avatars.githubusercontent.com/u/15144745?v=4?s=75" width="75px;" alt="Ian Moir"/><br /><sub><b>Ian Moir</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Aianmmoir" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/pekingduck"><img src="https://avatars.githubusercontent.com/u/2597142?v=4?s=75" width="75px;" alt="Peking Duck"/><br /><sub><b>Peking Duck</b></sub></a><br /><a href="#ideas-pekingduck" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Apekingduck" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.patreon.com/cclauss"><img src="https://avatars.githubusercontent.com/u/3709715?v=4?s=75" width="75px;" alt="Christian Clauss"/><br /><sub><b>Christian Clauss</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/commits?author=cclauss" title="Code">💻</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/dvdkon"><img src="https://avatars.githubusercontent.com/u/3526303?v=4?s=75" width="75px;" alt="dvdkon"/><br /><sub><b>dvdkon</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/commits?author=dvdkon" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/wernerzj"><img src="https://avatars.githubusercontent.com/u/130370930?v=4?s=75" width="75px;" alt="wernerzj"/><br /><sub><b>wernerzj</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Awernerzj" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/rajscode"><img src="https://avatars.githubusercontent.com/u/99123253?v=4?s=75" width="75px;" alt="rajscode"/><br /><sub><b>rajscode</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Arajscode" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/rajscode"><img src="https://avatars.githubusercontent.com/u/99123253?v=4?s=75" width="75px;" alt="rajscode"/><br /><sub><b>rajscode</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Arajscode" title="Bug reports">🐛</a> <a href="https://github.com/RhetTbull/osxphotos/commits?author=rajscode" title="Documentation">📖</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `osxphotos-0.60.1/README.rst` & `osxphotos-0.60.2/README.rst`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/__init__.py` & `osxphotos-0.60.2/osxphotos/__init__.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/_constants.py` & `osxphotos-0.60.2/osxphotos/_constants.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/adjustmentsinfo.py` & `osxphotos-0.60.2/osxphotos/adjustmentsinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/albuminfo.py` & `osxphotos-0.60.2/osxphotos/albuminfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/__init__.py` & `osxphotos-0.60.2/osxphotos/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/about.py` & `osxphotos-0.60.2/osxphotos/cli/about.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/add_locations.py` & `osxphotos-0.60.2/osxphotos/cli/add_locations.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/albums.py` & `osxphotos-0.60.2/osxphotos/cli/albums.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/batch_edit.py` & `osxphotos-0.60.2/osxphotos/cli/batch_edit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/cli.py` & `osxphotos-0.60.2/osxphotos/cli/cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/cli_commands.py` & `osxphotos-0.60.2/osxphotos/cli/cli_commands.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/cli_params.py` & `osxphotos-0.60.2/osxphotos/cli/cli_params.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/click_rich_echo.py` & `osxphotos-0.60.2/osxphotos/cli/click_rich_echo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/color_themes.py` & `osxphotos-0.60.2/osxphotos/cli/color_themes.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/common.py` & `osxphotos-0.60.2/osxphotos/cli/common.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/darkmode.py` & `osxphotos-0.60.2/osxphotos/cli/darkmode.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/debug_dump.py` & `osxphotos-0.60.2/osxphotos/cli/debug_dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/docs.py` & `osxphotos-0.60.2/osxphotos/cli/docs.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/dump.py` & `osxphotos-0.60.2/osxphotos/cli/dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/exiftool_cli.py` & `osxphotos-0.60.2/osxphotos/cli/exiftool_cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/export.py` & `osxphotos-0.60.2/osxphotos/cli/export.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/exportdb.py` & `osxphotos-0.60.2/osxphotos/cli/exportdb.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/grep.py` & `osxphotos-0.60.2/osxphotos/cli/grep.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/help.py` & `osxphotos-0.60.2/osxphotos/cli/help.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/import_cli.py` & `osxphotos-0.60.2/osxphotos/cli/import_cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/info.py` & `osxphotos-0.60.2/osxphotos/cli/info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/install_uninstall_run.py` & `osxphotos-0.60.2/osxphotos/cli/install_uninstall_run.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/keywords.py` & `osxphotos-0.60.2/osxphotos/cli/keywords.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/kvstore.py` & `osxphotos-0.60.2/osxphotos/cli/kvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/labels.py` & `osxphotos-0.60.2/osxphotos/cli/labels.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/list.py` & `osxphotos-0.60.2/osxphotos/cli/list.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/orphans.py` & `osxphotos-0.60.2/osxphotos/cli/orphans.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/param_types.py` & `osxphotos-0.60.2/osxphotos/cli/param_types.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/persons.py` & `osxphotos-0.60.2/osxphotos/cli/persons.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/photo_inspect.py` & `osxphotos-0.60.2/osxphotos/cli/photo_inspect.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/places.py` & `osxphotos-0.60.2/osxphotos/cli/places.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/print_photo_info.py` & `osxphotos-0.60.2/osxphotos/cli/print_photo_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/query.py` & `osxphotos-0.60.2/osxphotos/cli/query.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/repl.py` & `osxphotos-0.60.2/osxphotos/cli/repl.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/report_writer.py` & `osxphotos-0.60.2/osxphotos/cli/report_writer.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/rich_progress.py` & `osxphotos-0.60.2/osxphotos/cli/rich_progress.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/show_command.py` & `osxphotos-0.60.2/osxphotos/cli/show_command.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/snap_diff.py` & `osxphotos-0.60.2/osxphotos/cli/snap_diff.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/sync.py` & `osxphotos-0.60.2/osxphotos/cli/sync.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/sync_results.py` & `osxphotos-0.60.2/osxphotos/cli/sync_results.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/theme.py` & `osxphotos-0.60.2/osxphotos/cli/theme.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/timewarp.py` & `osxphotos-0.60.2/osxphotos/cli/timewarp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/tutorial.py` & `osxphotos-0.60.2/osxphotos/cli/tutorial.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/uuid.py` & `osxphotos-0.60.2/osxphotos/cli/uuid.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/verbose.py` & `osxphotos-0.60.2/osxphotos/cli/verbose.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/cli/version.py` & `osxphotos-0.60.2/osxphotos/cli/version.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/compare_exif.py` & `osxphotos-0.60.2/osxphotos/compare_exif.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/configoptions.py` & `osxphotos-0.60.2/osxphotos/configoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/crash_reporter.py` & `osxphotos-0.60.2/osxphotos/crash_reporter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/datetime_formatter.py` & `osxphotos-0.60.2/osxphotos/datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/datetime_utils.py` & `osxphotos-0.60.2/osxphotos/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/debug.py` & `osxphotos-0.60.2/osxphotos/debug.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/docs/docs.zip` & `osxphotos-0.60.2/osxphotos/docs/docs.zip`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,101 +1,101 @@
-Zip file size: 1467005 bytes, number of entries: 99
+Zip file size: 1467985 bytes, number of entries: 99
 -rw-r--r--  3.0 unx   331458 tx defN 23-Feb-12 16:23 docs/API_README.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:17 docs/_modules/
--rw-r--r--  3.0 unx    11779 tx defN 23-May-14 15:28 docs/_modules/index.html
+-rw-r--r--  3.0 unx    11779 tx defN 23-Jun-17 14:16 docs/_modules/index.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:15 docs/_modules/osxphotos/
--rw-r--r--  3.0 unx   317579 tx defN 23-May-07 14:38 docs/_modules/osxphotos/photoexporter.html
+-rw-r--r--  3.0 unx   324766 tx defN 23-Jun-17 14:16 docs/_modules/osxphotos/photoexporter.html
 -rw-r--r--  3.0 unx   296439 tx defN 23-May-07 14:38 docs/_modules/osxphotos/phototemplate.html
--rw-r--r--  3.0 unx   201027 tx defN 23-May-14 15:28 docs/_modules/osxphotos/export_db.html
--rw-r--r--  3.0 unx    14791 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/scoreinfo.html
+-rw-r--r--  3.0 unx   201027 tx defN 23-Jun-17 14:16 docs/_modules/osxphotos/export_db.html
+-rw-r--r--  3.0 unx    14791 tx defN 23-Jun-17 14:16 docs/_modules/osxphotos/scoreinfo.html
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:55 docs/_modules/osxphotos/photoinfo/
 -rw-r--r--  3.0 unx    14017 tx defN 21-Mar-22 05:50 docs/_modules/osxphotos/photoinfo/_photoinfo_exifinfo.html
 -rw-r--r--  3.0 unx   284197 tx defN 21-Dec-11 03:36 docs/_modules/osxphotos/photoinfo/_photoinfo_export.html
 -rw-r--r--  3.0 unx   195566 tx defN 21-Dec-11 03:36 docs/_modules/osxphotos/photoinfo/photoinfo.html
 -rw-r--r--  3.0 unx    33978 tx defN 21-Mar-22 05:50 docs/_modules/osxphotos/photoinfo/_photoinfo_searchinfo.html
 -rw-r--r--  3.0 unx    17959 tx defN 21-Mar-22 05:50 docs/_modules/osxphotos/photoinfo/_photoinfo_scoreinfo.html
 -rw-r--r--  3.0 unx    43160 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/searchinfo.html
 -rw-r--r--  3.0 unx    52325 tx defN 23-May-07 14:38 docs/_modules/osxphotos/fileutil.html
--rw-r--r--  3.0 unx   299834 tx defN 23-May-07 14:38 docs/_modules/osxphotos/photoinfo.html
+-rw-r--r--  3.0 unx   302896 tx defN 23-Jun-17 14:16 docs/_modules/osxphotos/photoinfo.html
 -rw-r--r--  3.0 unx     5599 tx defN 22-Apr-21 04:10 docs/_modules/osxphotos/exifinfo.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-16 03:03 docs/_modules/osxphotos/photosdb/
--rw-r--r--  3.0 unx    29240 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/photosdb/_photosdb_process_comments.html
--rw-r--r--  3.0 unx   523106 tx defN 23-May-07 14:38 docs/_modules/osxphotos/photosdb/photosdb.html
+-rw-r--r--  3.0 unx    29240 tx defN 23-Jun-17 14:16 docs/_modules/osxphotos/photosdb/_photosdb_process_comments.html
+-rw-r--r--  3.0 unx   523106 tx defN 23-Jun-17 14:16 docs/_modules/osxphotos/photosdb/photosdb.html
 -rw-r--r--  3.0 unx    36244 tx defN 23-May-07 14:38 docs/_modules/osxphotos/photosalbum.html
 -rw-r--r--  3.0 unx    92802 tx defN 23-May-07 14:38 docs/_modules/osxphotos/placeinfo.html
 -rw-r--r--  3.0 unx    21299 tx defN 22-May-06 00:24 docs/_modules/osxphotos/momentinfo.html
 -rw-r--r--  3.0 unx    82289 tx defN 23-Apr-11 02:04 docs/_modules/osxphotos/albuminfo.html
 -rw-r--r--  3.0 unx    78750 tx defN 23-Apr-03 02:59 docs/_modules/osxphotos/exiftool.html
 -rw-r--r--  3.0 unx    26012 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/debug.html
 -rw-r--r--  3.0 unx    59723 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/queryoptions.html
 -rw-r--r--  3.0 unx    80476 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/personinfo.html
 -rw-r--r--  3.0 unx    61850 tx defN 23-May-14 15:28 docs/_modules/osxphotos/_constants.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-12 16:20 docs/_sources/
 -rw-r--r--  3.0 unx      198 tx defN 22-Apr-23 14:44 docs/_sources/cli.rst.txt
--rw-r--r--  3.0 unx    31854 tx defN 23-May-14 15:28 docs/_sources/template_help.rst.txt
+-rw-r--r--  3.0 unx    31854 tx defN 23-Jun-17 14:16 docs/_sources/template_help.rst.txt
 -rw-r--r--  3.0 unx    31240 tx defN 21-Apr-26 18:30 docs/_sources/tutorial.md.txt
 -rw-r--r--  3.0 unx       52 tx defN 21-Jan-24 17:13 docs/_sources/modules.rst.txt
 -rw-r--r--  3.0 unx    41238 tx defN 22-Aug-27 16:24 docs/_sources/tutorial.rst.txt
 -rw-r--r--  3.0 unx       93 tx defN 23-Feb-12 16:23 docs/_sources/reference.rst.txt
 -rw-r--r--  3.0 unx     7548 tx defN 22-Apr-23 18:28 docs/_sources/package_overview.rst.txt
 -rw-r--r--  3.0 unx      149 tx defN 22-Apr-21 04:29 docs/_sources/cli_export.rst.txt
 -rw-r--r--  3.0 unx   147706 tx defN 23-Feb-12 16:20 docs/_sources/API_README.rst.txt
 -rw-r--r--  3.0 unx      502 tx defN 23-Feb-12 16:24 docs/_sources/index.rst.txt
 -rw-r--r--  3.0 unx     4241 tx defN 22-May-01 15:46 docs/_sources/overview.rst.txt
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:17 docs/_static/
 -rw-r--r--  3.0 unx       90 bx defN 21-Mar-14 19:14 docs/_static/plus.png
 -rw-r--r--  3.0 unx     4712 tx defN 22-Nov-13 03:13 docs/_static/sphinx_highlight.js
 -rw-r--r--  3.0 unx    19530 tx defN 21-Jun-05 18:07 docs/_static/underscore.js
 -rw-r--r--  3.0 unx    11185 tx defN 21-Mar-22 05:50 docs/_static/alabaster.css
--rw-r--r--  3.0 unx      421 tx defN 23-May-14 15:28 docs/_static/documentation_options.js
+-rw-r--r--  3.0 unx      421 tx defN 23-Jun-17 14:16 docs/_static/documentation_options.js
 -rw-r--r--  3.0 unx    18215 tx defN 22-Nov-13 03:13 docs/_static/searchtools.js
 -rw-r--r--  3.0 unx     1266 tx defN 22-Nov-13 03:13 docs/_static/debug.css
 -rw-r--r--  3.0 unx      313 tx defN 22-Apr-21 05:12 docs/_static/check-solid.svg
 -rw-r--r--  3.0 unx     9031 tx defN 22-Apr-21 05:12 docs/_static/clipboard.min.js
 -rw-r--r--  3.0 unx      286 bx stor 21-Mar-14 19:14 docs/_static/file.png
 -rw-r--r--  3.0 unx     4418 tx defN 22-Nov-13 03:13 docs/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--  3.0 unx     8472 tx defN 23-May-14 15:28 docs/_static/copybutton.js
+-rw-r--r--  3.0 unx     8472 tx defN 23-Jun-17 14:16 docs/_static/copybutton.js
 -rw-r--r--  3.0 unx   287630 tx defN 21-Mar-14 19:14 docs/_static/jquery-3.5.1.js
 -rw-r--r--  3.0 unx       42 tx stor 21-Mar-14 19:14 docs/_static/custom.css
--rw-r--r--  3.0 unx     4758 tx defN 23-May-14 15:28 docs/_static/language_data.js
+-rw-r--r--  3.0 unx     4758 tx defN 23-Jun-17 14:16 docs/_static/language_data.js
 -rw-r--r--  3.0 unx      411 tx defN 22-Apr-21 05:12 docs/_static/copy-button.svg
 -rw-r--r--  3.0 unx     2698 tx defN 22-Dec-03 06:57 docs/_static/copybutton_funcs.js
 -rw-r--r--  3.0 unx       90 bx defN 21-Mar-14 19:14 docs/_static/minus.png
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-24 15:32 docs/_static/styles/
 -rw-r--r--  3.0 unx    72647 tx defN 22-Dec-03 06:57 docs/_static/styles/furo.css.map
 -rw-r--r--  3.0 unx     5529 tx defN 22-Apr-21 04:34 docs/_static/styles/furo-extensions.css
 -rw-r--r--  3.0 unx    48032 tx defN 22-Dec-03 06:57 docs/_static/styles/furo.css
 -rw-r--r--  3.0 unx     7809 tx defN 22-Apr-21 04:34 docs/_static/styles/furo-extensions.css.map
 -rw-r--r--  3.0 unx     6034 tx defN 22-Nov-13 03:13 docs/_static/skeleton.css
 -rw-r--r--  3.0 unx   288580 tx defN 22-Nov-13 03:13 docs/_static/jquery-3.6.0.js
--rw-r--r--  3.0 unx    14810 tx defN 23-May-14 15:28 docs/_static/basic.css
+-rw-r--r--  3.0 unx    14810 tx defN 23-Jun-17 14:16 docs/_static/basic.css
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:21 docs/_static/scripts/
 -rw-r--r--  3.0 unx      187 tx defN 22-Apr-21 04:34 docs/_static/scripts/furo.js.LICENSE.txt
 -rw-r--r--  3.0 unx    28242 tx defN 22-Nov-13 03:13 docs/_static/scripts/furo.js.map
 -rw-r--r--  3.0 unx        0 bx stor 22-Apr-21 04:34 docs/_static/scripts/furo-extensions.js
 -rw-r--r--  3.0 unx     5265 tx defN 22-Apr-21 04:34 docs/_static/scripts/furo.js
--rw-r--r--  3.0 unx    21072 tx defN 23-May-14 15:28 docs/_static/pygments.css
+-rw-r--r--  3.0 unx    21072 tx defN 23-Jun-17 14:16 docs/_static/pygments.css
 -rw-r--r--  3.0 unx     2060 tx defN 22-Dec-03 06:57 docs/_static/copybutton.css
 -rw-r--r--  3.0 unx     4472 tx defN 22-Nov-13 03:13 docs/_static/doctools.js
 -rw-r--r--  3.0 unx    67692 tx defN 21-Mar-14 19:14 docs/_static/underscore-1.12.0.js
 -rw-r--r--  3.0 unx    89501 tx defN 22-Nov-13 03:13 docs/_static/jquery.js
 -rw-r--r--  3.0 unx    68420 tx defN 21-Jun-05 18:07 docs/_static/underscore-1.13.1.js
--rw-r--r--  3.0 unx   414459 tx defN 23-May-14 15:28 docs/cli.html
+-rw-r--r--  3.0 unx   414459 tx defN 23-Jun-17 14:16 docs/cli.html
 -rw-r--r--  3.0 unx    85854 tx defN 22-Apr-21 04:30 docs/cli_export.html
--rw-r--r--  3.0 unx   243869 tx defN 23-May-14 15:28 docs/genindex.html
--rw-r--r--  3.0 unx   103976 tx defN 23-May-14 15:28 docs/index.html
+-rw-r--r--  3.0 unx   243869 tx defN 23-Jun-17 14:16 docs/genindex.html
+-rw-r--r--  3.0 unx   103976 tx defN 23-Jun-17 14:16 docs/index.html
 -rw-r--r--  3.0 unx     2984 tx defN 22-Apr-20 14:01 docs/modules.html
--rw-r--r--  3.0 unx     9396 bx stor 23-May-14 15:28 docs/objects.inv
+-rw-r--r--  3.0 unx     9396 bx stor 23-Jun-17 14:16 docs/objects.inv
 -rw-r--r--  3.0 unx   267506 bx defN 21-May-10 00:50 docs/osxphotos.pdf
--rw-r--r--  3.0 unx    26446 tx defN 23-May-14 15:28 docs/overview.html
--rw-r--r--  3.0 unx    32469 tx defN 23-May-14 15:28 docs/package_overview.html
--rw-r--r--  3.0 unx    10831 tx defN 23-May-14 15:28 docs/py-modindex.html
--rw-r--r--  3.0 unx   438606 tx defN 23-May-14 15:28 docs/reference.html
+-rw-r--r--  3.0 unx    26446 tx defN 23-Jun-17 14:16 docs/overview.html
+-rw-r--r--  3.0 unx    32469 tx defN 23-Jun-17 14:16 docs/package_overview.html
+-rw-r--r--  3.0 unx    10831 tx defN 23-Jun-17 14:16 docs/py-modindex.html
+-rw-r--r--  3.0 unx   438608 tx defN 23-Jun-17 14:16 docs/reference.html
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:53 docs/screencast/
 -rw-r--r--  3.0 unx     8007 tx defN 21-Jan-24 17:13 docs/screencast/terminalizer-demo.yml
 -rw-r--r--  3.0 unx    77927 bx defN 21-Jan-24 17:13 docs/screencast/osx-screenshot.png
 -rw-r--r--  3.0 unx   224316 bx defN 21-Jan-24 17:13 docs/screencast/demo.gif
--rw-r--r--  3.0 unx    10567 tx defN 23-May-14 15:28 docs/search.html
--rw-r--r--  3.0 unx   215976 tx defN 23-May-14 15:28 docs/searchindex.js
--rw-r--r--  3.0 unx    64566 tx defN 23-May-14 15:28 docs/template_help.html
--rw-r--r--  3.0 unx    84995 tx defN 23-May-14 15:28 docs/tutorial.html
-99 files, 6902990 bytes uncompressed, 1448273 bytes compressed:  79.0%
+-rw-r--r--  3.0 unx    10567 tx defN 23-Jun-17 14:16 docs/search.html
+-rw-r--r--  3.0 unx   215976 tx defN 23-Jun-17 14:16 docs/searchindex.js
+-rw-r--r--  3.0 unx    64566 tx defN 23-Jun-17 14:16 docs/template_help.html
+-rw-r--r--  3.0 unx    84995 tx defN 23-Jun-17 14:16 docs/tutorial.html
+99 files, 6913241 bytes uncompressed, 1449253 bytes compressed:  79.0%
```

#### docs/_modules/index.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../genindex.html" /><link rel="search" title="Search" href="../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>Overview: module code - osxphotos 0.60.1 documentation</title>
+        <title>Overview: module code - osxphotos 0.60.2 documentation</title>
       <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../index.html"><div class="brand">osxphotos 0.60.1 documentation</div></a>
+      <a href="../index.html"><div class="brand">osxphotos 0.60.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.1_documentation
+osxphotos_0.60.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.1_documentation
+osxphotos_0.60.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_modules/osxphotos/photoexporter.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.photoexporter - osxphotos 0.60.0 documentation</title>
+        <title>osxphotos.photoexporter - osxphotos 0.60.2 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.60.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -194,23 +194,23 @@
           </label>
         </div>
         <article role="main">
           <h1>Source code for osxphotos.photoexporter</h1><div class="highlight"><pre>
 <span></span><span class="sd">&quot;&quot;&quot; PhotoExport class to export photos</span>
 <span class="sd">&quot;&quot;&quot;</span>
 
+<span class="kn">from</span> <span class="nn">__future__</span> <span class="kn">import</span> <span class="n">annotations</span>
+
 <span class="kn">import</span> <span class="nn">dataclasses</span>
 <span class="kn">import</span> <span class="nn">json</span>
 <span class="kn">import</span> <span class="nn">logging</span>
 <span class="kn">import</span> <span class="nn">os</span>
 <span class="kn">import</span> <span class="nn">pathlib</span>
 <span class="kn">import</span> <span class="nn">re</span>
-<span class="kn">import</span> <span class="nn">sys</span>
 <span class="kn">import</span> <span class="nn">typing</span> <span class="k">as</span> <span class="nn">t</span>
-<span class="kn">from</span> <span class="nn">collections</span> <span class="kn">import</span> <span class="n">namedtuple</span>  <span class="c1"># pylint: disable=syntax-error</span>
 <span class="kn">from</span> <span class="nn">dataclasses</span> <span class="kn">import</span> <span class="n">asdict</span><span class="p">,</span> <span class="n">dataclass</span>
 <span class="kn">from</span> <span class="nn">datetime</span> <span class="kn">import</span> <span class="n">datetime</span>
 <span class="kn">from</span> <span class="nn">enum</span> <span class="kn">import</span> <span class="n">Enum</span>
 <span class="kn">from</span> <span class="nn">types</span> <span class="kn">import</span> <span class="n">SimpleNamespace</span>
 
 <span class="kn">from</span> <span class="nn">mako.template</span> <span class="kn">import</span> <span class="n">Template</span>
 
@@ -232,18 +232,18 @@
 <span class="kn">from</span> <span class="nn">.exiftool</span> <span class="kn">import</span> <span class="n">ExifTool</span><span class="p">,</span> <span class="n">ExifToolCaching</span><span class="p">,</span> <span class="n">exiftool_can_write</span><span class="p">,</span> <span class="n">get_exiftool_path</span>
 <span class="kn">from</span> <span class="nn">.export_db</span> <span class="kn">import</span> <span class="n">ExportDB</span><span class="p">,</span> <span class="n">ExportDBTemp</span>
 <span class="kn">from</span> <span class="nn">.fileutil</span> <span class="kn">import</span> <span class="n">FileUtil</span>
 <span class="kn">from</span> <span class="nn">.phototemplate</span> <span class="kn">import</span> <span class="n">RenderOptions</span>
 <span class="kn">from</span> <span class="nn">.rich_utils</span> <span class="kn">import</span> <span class="n">add_rich_markup_tag</span>
 <span class="kn">from</span> <span class="nn">.uti</span> <span class="kn">import</span> <span class="n">get_preferred_uti_extension</span>
 <span class="kn">from</span> <span class="nn">.utils</span> <span class="kn">import</span> <span class="p">(</span>
-    <span class="n">is_macos</span><span class="p">,</span>
     <span class="n">hexdigest</span><span class="p">,</span>
     <span class="n">increment_filename</span><span class="p">,</span>
     <span class="n">increment_filename_with_count</span><span class="p">,</span>
+    <span class="n">is_macos</span><span class="p">,</span>
     <span class="n">lineno</span><span class="p">,</span>
     <span class="n">list_directory</span><span class="p">,</span>
     <span class="n">lock_filename</span><span class="p">,</span>
     <span class="n">normalize_fs_path</span><span class="p">,</span>
     <span class="n">unlock_filename</span><span class="p">,</span>
 <span class="p">)</span>
 
@@ -269,14 +269,18 @@
 
 <span class="k">if</span> <span class="n">t</span><span class="o">.</span><span class="n">TYPE_CHECKING</span><span class="p">:</span>
     <span class="kn">from</span> <span class="nn">.photoinfo</span> <span class="kn">import</span> <span class="n">PhotoInfo</span>
 
 <span class="c1"># retry if download_missing/use_photos_export fails the first time (which sometimes it does)</span>
 <span class="n">MAX_PHOTOSCRIPT_RETRIES</span> <span class="o">=</span> <span class="mi">3</span>
 
+<span class="c1"># Global to hold the compiled XMP template</span>
+<span class="c1"># This is expensive to compile so we only want to do it once</span>
+<span class="n">_global_xmp_template</span><span class="p">:</span> <span class="n">Template</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+
 
 <span class="c1"># return values for _should_update_photo</span>
 <span class="k">class</span> <span class="nc">ShouldUpdate</span><span class="p">(</span><span class="n">Enum</span><span class="p">):</span>
     <span class="n">NOT_IN_DATABASE</span> <span class="o">=</span> <span class="mi">1</span>
     <span class="n">HARDLINK_DIFFERENT_FILES</span> <span class="o">=</span> <span class="mi">2</span>
     <span class="n">NOT_HARDLINK_SAME_FILES</span> <span class="o">=</span> <span class="mi">3</span>
     <span class="n">DEST_SIG_DIFFERENT</span> <span class="o">=</span> <span class="mi">4</span>
@@ -437,14 +441,17 @@
         <span class="bp">self</span><span class="o">.</span><span class="n">raw</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">raw</span> <span class="ow">or</span> <span class="n">other</span><span class="o">.</span><span class="n">raw</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">error</span> <span class="o">+=</span> <span class="n">other</span><span class="o">.</span><span class="n">error</span>
         <span class="k">return</span> <span class="bp">self</span>
 
     <span class="k">def</span> <span class="fm">__str__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="k">return</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">asdict</span><span class="p">())</span>
 
+    <span class="k">def</span> <span class="fm">__repr__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;StagedFiles(</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">asdict</span><span class="p">()</span><span class="si">}</span><span class="s2">)&quot;</span>
+
     <span class="k">def</span> <span class="nf">asdict</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="k">return</span> <span class="p">{</span>
             <span class="s2">&quot;original&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">original</span><span class="p">,</span>
             <span class="s2">&quot;original_live&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">original_live</span><span class="p">,</span>
             <span class="s2">&quot;edited&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">edited</span><span class="p">,</span>
             <span class="s2">&quot;edited_live&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">edited_live</span><span class="p">,</span>
             <span class="s2">&quot;preview&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">preview</span><span class="p">,</span>
@@ -672,14 +679,19 @@
             <span class="n">filename</span> <span class="o">=</span> <span class="n">filename</span> <span class="ow">or</span> <span class="bp">self</span><span class="o">.</span><span class="n">photo</span><span class="o">.</span><span class="n">original_filename</span>
         <span class="n">dest</span> <span class="o">=</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">(</span><span class="n">dest</span><span class="p">)</span> <span class="o">/</span> <span class="n">filename</span>
 
         <span class="c1"># Is there something to convert with convert_to_jpeg?</span>
         <span class="n">dest</span><span class="p">,</span> <span class="n">options</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_should_convert_to_jpeg</span><span class="p">(</span><span class="n">dest</span><span class="p">,</span> <span class="n">options</span><span class="p">)</span>
 
         <span class="c1"># stage files for export by finding path in local library or downloading from iCloud as appropriate</span>
+        <span class="c1"># for `--download-missing` and `--update` case, this may cause unnecessary downloads</span>
+        <span class="c1"># as it will download the file even if it&#39;s not needed (won&#39;t be checked until the _should_update_photo() call from _export_photo()</span>
+        <span class="c1"># fixing this will require major refactoring of the export code, see #1086</span>
+        <span class="c1"># leaving it for now as this should not be a common use case</span>
+        <span class="c1"># (if using `--update` it is much better to be using &quot;Download originals to this Mac&quot; in Photos)</span>
         <span class="n">staged_files</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_stage_photos_for_export</span><span class="p">(</span><span class="n">options</span><span class="p">)</span>
         <span class="n">src</span> <span class="o">=</span> <span class="n">staged_files</span><span class="o">.</span><span class="n">edited</span> <span class="k">if</span> <span class="n">options</span><span class="o">.</span><span class="n">edited</span> <span class="k">else</span> <span class="n">staged_files</span><span class="o">.</span><span class="n">original</span>
 
         <span class="c1"># get the right destination path depending on options.update, etc.</span>
         <span class="n">dest</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_dest_path</span><span class="p">(</span><span class="n">dest</span><span class="p">,</span> <span class="n">options</span><span class="p">)</span>
 
         <span class="bp">self</span><span class="o">.</span><span class="n">_render_options</span><span class="o">.</span><span class="n">filepath</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">dest</span><span class="p">)</span>
@@ -858,16 +870,24 @@
         <span class="n">lock</span> <span class="o">=</span> <span class="ow">not</span> <span class="n">options</span><span class="o">.</span><span class="n">dry_run</span>
 
         <span class="k">def</span> <span class="nf">_lock_filename</span><span class="p">(</span><span class="n">filename</span><span class="p">):</span>
             <span class="sd">&quot;&quot;&quot;Lock filename if not in dry_run mode&quot;&quot;&quot;</span>
             <span class="k">return</span> <span class="n">lock_filename</span><span class="p">(</span><span class="n">filename</span><span class="p">)</span> <span class="k">if</span> <span class="n">lock</span> <span class="k">else</span> <span class="n">filename</span>
 
         <span class="c1"># if overwrite==False and #increment==False, export should fail if file exists</span>
-        <span class="k">if</span> <span class="n">dest</span><span class="o">.</span><span class="n">exists</span><span class="p">()</span> <span class="ow">and</span> <span class="ow">not</span> <span class="nb">any</span><span class="p">(</span>
-            <span class="p">[</span><span class="n">options</span><span class="o">.</span><span class="n">increment</span><span class="p">,</span> <span class="n">options</span><span class="o">.</span><span class="n">update</span><span class="p">,</span> <span class="n">options</span><span class="o">.</span><span class="n">force_update</span><span class="p">,</span> <span class="n">options</span><span class="o">.</span><span class="n">overwrite</span><span class="p">]</span>
+        <span class="k">if</span> <span class="p">(</span>
+            <span class="ow">not</span> <span class="nb">any</span><span class="p">(</span>
+                <span class="p">[</span>
+                    <span class="n">options</span><span class="o">.</span><span class="n">increment</span><span class="p">,</span>
+                    <span class="n">options</span><span class="o">.</span><span class="n">update</span><span class="p">,</span>
+                    <span class="n">options</span><span class="o">.</span><span class="n">force_update</span><span class="p">,</span>
+                    <span class="n">options</span><span class="o">.</span><span class="n">overwrite</span><span class="p">,</span>
+                <span class="p">]</span>
+            <span class="p">)</span>
+            <span class="ow">and</span> <span class="n">dest</span><span class="o">.</span><span class="n">exists</span><span class="p">()</span>
         <span class="p">):</span>
             <span class="k">raise</span> <span class="ne">FileExistsError</span><span class="p">(</span>
                 <span class="sa">f</span><span class="s2">&quot;destination exists (</span><span class="si">{</span><span class="n">dest</span><span class="si">}</span><span class="s2">); overwrite=</span><span class="si">{</span><span class="n">options</span><span class="o">.</span><span class="n">overwrite</span><span class="si">}</span><span class="s2">, increment=</span><span class="si">{</span><span class="n">options</span><span class="o">.</span><span class="n">increment</span><span class="si">}</span><span class="s2">&quot;</span>
             <span class="p">)</span>
 
         <span class="c1"># if overwrite, we don&#39;t care if the file exists or not</span>
         <span class="k">if</span> <span class="n">options</span><span class="o">.</span><span class="n">overwrite</span> <span class="ow">and</span> <span class="n">_lock_filename</span><span class="p">(</span><span class="n">dest</span><span class="p">):</span>
@@ -918,34 +938,44 @@
             <span class="k">return</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">(</span><span class="n">dest</span><span class="p">)</span>
 
         <span class="c1"># fail safe...I can&#39;t think of a case that gets here</span>
         <span class="n">_lock_filename</span><span class="p">(</span><span class="n">dest</span><span class="p">)</span>
         <span class="k">return</span> <span class="n">dest</span>
 
     <span class="k">def</span> <span class="nf">_should_update_photo</span><span class="p">(</span>
-        <span class="bp">self</span><span class="p">,</span> <span class="n">src</span><span class="p">:</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">,</span> <span class="n">dest</span><span class="p">:</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">,</span> <span class="n">options</span><span class="p">:</span> <span class="n">ExportOptions</span>
-    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">t</span><span class="o">.</span><span class="n">Literal</span><span class="p">[</span><span class="kc">True</span><span class="p">,</span> <span class="kc">False</span><span class="p">]:</span>
-        <span class="sd">&quot;&quot;&quot;Return True if photo should be updated, else False&quot;&quot;&quot;</span>
+        <span class="bp">self</span><span class="p">,</span> <span class="n">src</span><span class="p">:</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span> <span class="o">|</span> <span class="kc">None</span><span class="p">,</span> <span class="n">dest</span><span class="p">:</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">,</span> <span class="n">options</span><span class="p">:</span> <span class="n">ExportOptions</span>
+    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span> <span class="o">|</span> <span class="n">ShouldUpdate</span><span class="p">:</span>
+        <span class="sd">&quot;&quot;&quot;Return True if photo should be updated, else False</span>
+
+<span class="sd">        Args:</span>
+<span class="sd">            src (pathlib.Path | None): source path; if None, photo is missing and</span>
+<span class="sd">                any checks that require src will return True</span>
+<span class="sd">            dest (pathlib.Path): destination path</span>
+
+<span class="sd">        Returns:</span>
+<span class="sd">            False if photo should not be updated otherwise a truthy ShouldUpdate value</span>
+<span class="sd">        &quot;&quot;&quot;</span>
+
         <span class="c1"># NOTE: The order of certain checks is important</span>
         <span class="c1"># read the comments below to understand why before changing</span>
 
         <span class="n">export_db</span> <span class="o">=</span> <span class="n">options</span><span class="o">.</span><span class="n">export_db</span>
         <span class="n">fileutil</span> <span class="o">=</span> <span class="n">options</span><span class="o">.</span><span class="n">fileutil</span>
 
         <span class="n">file_record</span> <span class="o">=</span> <span class="n">export_db</span><span class="o">.</span><span class="n">get_file_record</span><span class="p">(</span><span class="n">dest</span><span class="p">)</span>
 
         <span class="k">if</span> <span class="ow">not</span> <span class="n">file_record</span><span class="p">:</span>
             <span class="c1"># photo doesn&#39;t exist in database, should update</span>
             <span class="k">return</span> <span class="n">ShouldUpdate</span><span class="o">.</span><span class="n">NOT_IN_DATABASE</span>
 
-        <span class="k">if</span> <span class="n">options</span><span class="o">.</span><span class="n">export_as_hardlink</span> <span class="ow">and</span> <span class="ow">not</span> <span class="n">dest</span><span class="o">.</span><span class="n">samefile</span><span class="p">(</span><span class="n">src</span><span class="p">):</span>
+        <span class="k">if</span> <span class="n">options</span><span class="o">.</span><span class="n">export_as_hardlink</span> <span class="ow">and</span> <span class="p">(</span><span class="ow">not</span> <span class="n">src</span> <span class="ow">or</span> <span class="ow">not</span> <span class="n">dest</span><span class="o">.</span><span class="n">samefile</span><span class="p">(</span><span class="n">src</span><span class="p">)):</span>
             <span class="c1"># different files, should update</span>
             <span class="k">return</span> <span class="n">ShouldUpdate</span><span class="o">.</span><span class="n">HARDLINK_DIFFERENT_FILES</span>
 
-        <span class="k">if</span> <span class="ow">not</span> <span class="n">options</span><span class="o">.</span><span class="n">export_as_hardlink</span> <span class="ow">and</span> <span class="n">dest</span><span class="o">.</span><span class="n">samefile</span><span class="p">(</span><span class="n">src</span><span class="p">):</span>
+        <span class="k">if</span> <span class="ow">not</span> <span class="n">options</span><span class="o">.</span><span class="n">export_as_hardlink</span> <span class="ow">and</span> <span class="p">(</span><span class="ow">not</span> <span class="n">src</span> <span class="ow">or</span> <span class="n">dest</span><span class="o">.</span><span class="n">samefile</span><span class="p">(</span><span class="n">src</span><span class="p">)):</span>
             <span class="c1"># same file but not exporting as hardlink, should update</span>
             <span class="k">return</span> <span class="n">ShouldUpdate</span><span class="o">.</span><span class="n">NOT_HARDLINK_SAME_FILES</span>
 
         <span class="k">if</span> <span class="ow">not</span> <span class="n">options</span><span class="o">.</span><span class="n">ignore_signature</span> <span class="ow">and</span> <span class="ow">not</span> <span class="n">fileutil</span><span class="o">.</span><span class="n">cmp_file_sig</span><span class="p">(</span>
             <span class="n">dest</span><span class="p">,</span> <span class="n">file_record</span><span class="o">.</span><span class="n">dest_sig</span>
         <span class="p">):</span>
             <span class="c1"># destination file doesn&#39;t match what was last exported</span>
@@ -969,15 +999,17 @@
         <span class="k">if</span> <span class="n">options</span><span class="o">.</span><span class="n">exiftool</span><span class="p">:</span>
             <span class="n">current_exifdata</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">exiftool_json_sidecar</span><span class="p">(</span><span class="n">options</span><span class="o">=</span><span class="n">options</span><span class="p">)</span>
             <span class="n">rv</span> <span class="o">=</span> <span class="n">current_exifdata</span> <span class="o">!=</span> <span class="n">file_record</span><span class="o">.</span><span class="n">exifdata</span>
             <span class="c1"># if using exiftool, don&#39;t need to continue checking edited below</span>
             <span class="c1"># as exiftool will be used to update edited file</span>
             <span class="k">return</span> <span class="n">ShouldUpdate</span><span class="o">.</span><span class="n">EXIFTOOL_DIFFERENT</span> <span class="k">if</span> <span class="n">rv</span> <span class="k">else</span> <span class="kc">False</span>
 
-        <span class="k">if</span> <span class="n">options</span><span class="o">.</span><span class="n">edited</span> <span class="ow">and</span> <span class="ow">not</span> <span class="n">fileutil</span><span class="o">.</span><span class="n">cmp_file_sig</span><span class="p">(</span><span class="n">src</span><span class="p">,</span> <span class="n">file_record</span><span class="o">.</span><span class="n">src_sig</span><span class="p">):</span>
+        <span class="k">if</span> <span class="n">options</span><span class="o">.</span><span class="n">edited</span> <span class="ow">and</span> <span class="p">(</span>
+            <span class="ow">not</span> <span class="n">src</span> <span class="ow">or</span> <span class="ow">not</span> <span class="n">fileutil</span><span class="o">.</span><span class="n">cmp_file_sig</span><span class="p">(</span><span class="n">src</span><span class="p">,</span> <span class="n">file_record</span><span class="o">.</span><span class="n">src_sig</span><span class="p">)</span>
+        <span class="p">):</span>
             <span class="c1"># edited file in Photos doesn&#39;t match what was last exported</span>
             <span class="k">return</span> <span class="n">ShouldUpdate</span><span class="o">.</span><span class="n">EDITED_SIG_DIFFERENT</span>
 
         <span class="k">if</span> <span class="n">options</span><span class="o">.</span><span class="n">force_update</span><span class="p">:</span>
             <span class="n">current_digest</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">photo</span><span class="o">.</span><span class="n">hexdigest</span>
             <span class="k">if</span> <span class="n">current_digest</span> <span class="o">!=</span> <span class="n">file_record</span><span class="o">.</span><span class="n">digest</span><span class="p">:</span>
                 <span class="c1"># metadata in Photos changed, force update</span>
@@ -1020,30 +1052,54 @@
             <span class="c1"># edited file</span>
             <span class="n">staged</span><span class="o">.</span><span class="n">edited</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">photo</span><span class="o">.</span><span class="n">path_edited</span>
             <span class="k">if</span> <span class="n">options</span><span class="o">.</span><span class="n">live_photo</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">photo</span><span class="o">.</span><span class="n">live_photo</span><span class="p">:</span>
                 <span class="n">staged</span><span class="o">.</span><span class="n">edited_live</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">photo</span><span class="o">.</span><span class="n">path_edited_live_photo</span>
 
         <span class="c1"># download any missing files</span>
         <span class="k">if</span> <span class="n">options</span><span class="o">.</span><span class="n">download_missing</span><span class="p">:</span>
-            <span class="n">live_photo</span> <span class="o">=</span> <span class="n">staged</span><span class="o">.</span><span class="n">edited_live</span> <span class="k">if</span> <span class="n">options</span><span class="o">.</span><span class="n">edited</span> <span class="k">else</span> <span class="n">staged</span><span class="o">.</span><span class="n">original_live</span>
-            <span class="n">missing_options</span> <span class="o">=</span> <span class="n">ExportOptions</span><span class="p">(</span>
-                <span class="n">edited</span><span class="o">=</span><span class="n">options</span><span class="o">.</span><span class="n">edited</span><span class="p">,</span>
-                <span class="n">preview</span><span class="o">=</span><span class="n">options</span><span class="o">.</span><span class="n">preview</span> <span class="ow">and</span> <span class="ow">not</span> <span class="n">staged</span><span class="o">.</span><span class="n">preview</span><span class="p">,</span>
-                <span class="n">raw_photo</span><span class="o">=</span><span class="n">options</span><span class="o">.</span><span class="n">raw_photo</span> <span class="ow">and</span> <span class="ow">not</span> <span class="n">staged</span><span class="o">.</span><span class="n">raw</span><span class="p">,</span>
-                <span class="n">live_photo</span><span class="o">=</span><span class="n">options</span><span class="o">.</span><span class="n">live_photo</span> <span class="ow">and</span> <span class="ow">not</span> <span class="n">live_photo</span><span class="p">,</span>
-            <span class="p">)</span>
-            <span class="k">if</span> <span class="n">options</span><span class="o">.</span><span class="n">use_photokit</span><span class="p">:</span>
-                <span class="n">missing_staged</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_stage_photo_for_export_with_photokit</span><span class="p">(</span>
-                    <span class="n">options</span><span class="o">=</span><span class="n">missing_options</span>
-                <span class="p">)</span>
-            <span class="k">else</span><span class="p">:</span>
-                <span class="n">missing_staged</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_stage_photo_for_export_with_applescript</span><span class="p">(</span>
-                    <span class="n">options</span><span class="o">=</span><span class="n">missing_options</span>
-                <span class="p">)</span>
-            <span class="n">staged</span> <span class="o">|=</span> <span class="n">missing_staged</span>
+            <span class="n">staged</span> <span class="o">|=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_stage_missing_photos_for_export</span><span class="p">(</span>
+                <span class="n">staged</span><span class="o">=</span><span class="n">staged</span><span class="p">,</span> <span class="n">options</span><span class="o">=</span><span class="n">options</span>
+            <span class="p">)</span>
+
+        <span class="k">return</span> <span class="n">staged</span>
+
+    <span class="k">def</span> <span class="nf">_stage_missing_photos_for_export</span><span class="p">(</span>
+        <span class="bp">self</span><span class="p">,</span> <span class="n">staged</span><span class="p">:</span> <span class="n">StagedFiles</span><span class="p">,</span> <span class="n">options</span><span class="p">:</span> <span class="n">ExportOptions</span>
+    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">StagedFiles</span><span class="p">:</span>
+        <span class="sd">&quot;&quot;&quot;Download and stage any missing files for export&quot;&quot;&quot;</span>
+
+        <span class="c1"># if live photo and requesting edited version need the edited live photo</span>
+        <span class="n">live_photo</span> <span class="o">=</span> <span class="n">staged</span><span class="o">.</span><span class="n">edited_live</span> <span class="k">if</span> <span class="n">options</span><span class="o">.</span><span class="n">edited</span> <span class="k">else</span> <span class="n">staged</span><span class="o">.</span><span class="n">original_live</span>
+
+        <span class="c1"># is there actually a missing file? (#1086)</span>
+        <span class="n">something_to_download</span> <span class="o">=</span> <span class="p">(</span>
+            <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">photo</span><span class="o">.</span><span class="n">hasadjustments</span> <span class="ow">and</span> <span class="n">options</span><span class="o">.</span><span class="n">edited</span> <span class="ow">and</span> <span class="ow">not</span> <span class="n">staged</span><span class="o">.</span><span class="n">edited</span><span class="p">)</span>
+            <span class="ow">or</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">photo</span><span class="o">.</span><span class="n">live_photo</span> <span class="ow">and</span> <span class="n">options</span><span class="o">.</span><span class="n">live_photo</span> <span class="ow">and</span> <span class="ow">not</span> <span class="n">live_photo</span><span class="p">)</span>
+            <span class="ow">or</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">photo</span><span class="o">.</span><span class="n">has_raw</span> <span class="ow">and</span> <span class="n">options</span><span class="o">.</span><span class="n">raw_photo</span> <span class="ow">and</span> <span class="ow">not</span> <span class="n">staged</span><span class="o">.</span><span class="n">raw</span><span class="p">)</span>
+            <span class="ow">or</span> <span class="p">(</span><span class="n">options</span><span class="o">.</span><span class="n">preview</span> <span class="ow">and</span> <span class="ow">not</span> <span class="n">staged</span><span class="o">.</span><span class="n">preview</span><span class="p">)</span>
+            <span class="ow">or</span> <span class="p">(</span><span class="ow">not</span> <span class="n">options</span><span class="o">.</span><span class="n">edited</span> <span class="ow">and</span> <span class="ow">not</span> <span class="n">staged</span><span class="o">.</span><span class="n">original</span><span class="p">)</span>
+        <span class="p">)</span>
+        <span class="k">if</span> <span class="ow">not</span> <span class="n">something_to_download</span><span class="p">:</span>
+            <span class="k">return</span> <span class="n">staged</span>
+
+        <span class="n">missing_options</span> <span class="o">=</span> <span class="n">ExportOptions</span><span class="p">(</span>
+            <span class="n">edited</span><span class="o">=</span><span class="n">options</span><span class="o">.</span><span class="n">edited</span><span class="p">,</span>
+            <span class="n">preview</span><span class="o">=</span><span class="n">options</span><span class="o">.</span><span class="n">preview</span> <span class="ow">and</span> <span class="ow">not</span> <span class="n">staged</span><span class="o">.</span><span class="n">preview</span><span class="p">,</span>
+            <span class="n">raw_photo</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">photo</span><span class="o">.</span><span class="n">has_raw</span> <span class="ow">and</span> <span class="n">options</span><span class="o">.</span><span class="n">raw_photo</span> <span class="ow">and</span> <span class="ow">not</span> <span class="n">staged</span><span class="o">.</span><span class="n">raw</span><span class="p">,</span>
+            <span class="n">live_photo</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">photo</span><span class="o">.</span><span class="n">live_photo</span> <span class="ow">and</span> <span class="n">options</span><span class="o">.</span><span class="n">live_photo</span> <span class="ow">and</span> <span class="ow">not</span> <span class="n">live_photo</span><span class="p">,</span>
+        <span class="p">)</span>
+        <span class="k">if</span> <span class="n">options</span><span class="o">.</span><span class="n">use_photokit</span><span class="p">:</span>
+            <span class="n">missing_staged</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_stage_photo_for_export_with_photokit</span><span class="p">(</span>
+                <span class="n">options</span><span class="o">=</span><span class="n">missing_options</span>
+            <span class="p">)</span>
+        <span class="k">else</span><span class="p">:</span>
+            <span class="n">missing_staged</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_stage_photo_for_export_with_applescript</span><span class="p">(</span>
+                <span class="n">options</span><span class="o">=</span><span class="n">missing_options</span>
+            <span class="p">)</span>
+        <span class="n">staged</span> <span class="o">|=</span> <span class="n">missing_staged</span>
         <span class="k">return</span> <span class="n">staged</span>
 
     <span class="k">def</span> <span class="nf">_stage_photo_for_export_with_photokit</span><span class="p">(</span>
         <span class="bp">self</span><span class="p">,</span>
         <span class="n">options</span><span class="p">:</span> <span class="n">ExportOptions</span><span class="p">,</span>
     <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">StagedFiles</span><span class="p">:</span>
         <span class="sd">&quot;&quot;&quot;Stage a photo for export with photokit to a temporary directory&quot;&quot;&quot;</span>
@@ -2152,18 +2208,15 @@
 <span class="sd">        Args:</span>
 <span class="sd">            options (ExportOptions): options for export</span>
 <span class="sd">            extension (t.Optional[str]): which extension to use for SidecarForExtension property</span>
 <span class="sd">        &quot;&quot;&quot;</span>
 
         <span class="n">options</span> <span class="o">=</span> <span class="n">options</span> <span class="ow">or</span> <span class="n">ExportOptions</span><span class="p">()</span>
 
-        <span class="n">xmp_template_file</span> <span class="o">=</span> <span class="p">(</span>
-            <span class="n">_XMP_TEMPLATE_NAME</span> <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">photo</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_beta</span> <span class="k">else</span> <span class="n">_XMP_TEMPLATE_NAME_BETA</span>
-        <span class="p">)</span>
-        <span class="n">xmp_template</span> <span class="o">=</span> <span class="n">Template</span><span class="p">(</span><span class="n">filename</span><span class="o">=</span><span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">_TEMPLATE_DIR</span><span class="p">,</span> <span class="n">xmp_template_file</span><span class="p">))</span>
+        <span class="n">xmp_template</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_xmp_template</span><span class="p">()</span>
 
         <span class="k">if</span> <span class="n">extension</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
             <span class="n">extension</span> <span class="o">=</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">photo</span><span class="o">.</span><span class="n">original_filename</span><span class="p">)</span>
             <span class="n">extension</span> <span class="o">=</span> <span class="n">extension</span><span class="o">.</span><span class="n">suffix</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span> <span class="k">if</span> <span class="n">extension</span><span class="o">.</span><span class="n">suffix</span> <span class="k">else</span> <span class="kc">None</span>
 
         <span class="k">if</span> <span class="n">options</span><span class="o">.</span><span class="n">description_template</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
             <span class="n">render_options</span> <span class="o">=</span> <span class="n">dataclasses</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span>
@@ -2262,14 +2315,28 @@
             <span class="n">rating</span><span class="o">=</span><span class="n">rating</span><span class="p">,</span>
         <span class="p">)</span>
 
         <span class="c1"># remove extra lines that mako inserts from template</span>
         <span class="n">xmp_str</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">line</span> <span class="k">for</span> <span class="n">line</span> <span class="ow">in</span> <span class="n">xmp_str</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span> <span class="k">if</span> <span class="n">line</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="o">!=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span>
         <span class="k">return</span> <span class="n">xmp_str</span>
 
+    <span class="k">def</span> <span class="nf">_xmp_template</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+        <span class="sd">&quot;&quot;&quot;Return the mako template for XMP sidecar, creating it if necessary&quot;&quot;&quot;</span>
+        <span class="k">global</span> <span class="n">_global_xmp_template</span>
+        <span class="k">if</span> <span class="n">_global_xmp_template</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
+            <span class="k">return</span> <span class="n">_global_xmp_template</span>
+
+        <span class="n">xmp_template_file</span> <span class="o">=</span> <span class="p">(</span>
+            <span class="n">_XMP_TEMPLATE_NAME_BETA</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">photo</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_beta</span> <span class="k">else</span> <span class="n">_XMP_TEMPLATE_NAME</span>
+        <span class="p">)</span>
+        <span class="n">_global_xmp_template</span> <span class="o">=</span> <span class="n">Template</span><span class="p">(</span>
+            <span class="n">filename</span><span class="o">=</span><span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">_TEMPLATE_DIR</span><span class="p">,</span> <span class="n">xmp_template_file</span><span class="p">)</span>
+        <span class="p">)</span>
+        <span class="k">return</span> <span class="n">_global_xmp_template</span>
+
     <span class="k">def</span> <span class="nf">_write_sidecar</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">filename</span><span class="p">,</span> <span class="n">sidecar_str</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;write sidecar_str to filename</span>
 <span class="sd">        used for exporting sidecar info&quot;&quot;&quot;</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="p">(</span><span class="n">filename</span> <span class="ow">or</span> <span class="n">sidecar_str</span><span class="p">):</span>
             <span class="k">raise</span> <span class="p">(</span>
                 <span class="ne">ValueError</span><span class="p">(</span>
                     <span class="sa">f</span><span class="s2">&quot;filename </span><span class="si">{</span><span class="n">filename</span><span class="si">}</span><span class="s2"> and sidecar_str </span><span class="si">{</span><span class="n">sidecar_str</span><span class="si">}</span><span class="s2"> must not be None&quot;</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -35,23 +35,23 @@
 
 Toggle table of contents sidebar
 
 ****** Source code for osxphotos.photoexporter ******
 """ PhotoExport class to export photos
 """
 
+from __future__ import annotations
+
 import dataclasses
 import json
 import logging
 import os
 import pathlib
 import re
-import sys
 import typing as t
-from collections import namedtuple  # pylint: disable=syntax-error
 from dataclasses import asdict, dataclass
 from datetime import datetime
 from enum import Enum
 from types import SimpleNamespace
 
 from mako.template import Template
 
@@ -74,18 +74,18 @@
 get_exiftool_path
 from .export_db import ExportDB, ExportDBTemp
 from .fileutil import FileUtil
 from .phototemplate import RenderOptions
 from .rich_utils import add_rich_markup_tag
 from .uti import get_preferred_uti_extension
 from .utils import (
-    is_macos,
     hexdigest,
     increment_filename,
     increment_filename_with_count,
+    is_macos,
     lineno,
     list_directory,
     lock_filename,
     normalize_fs_path,
     unlock_filename,
 )
 
@@ -112,14 +112,18 @@
 if t.TYPE_CHECKING:
     from .photoinfo import PhotoInfo
 
 # retry if download_missing/use_photos_export fails the first time (which
 sometimes it does)
 MAX_PHOTOSCRIPT_RETRIES = 3
 
+# Global to hold the compiled XMP template
+# This is expensive to compile so we only want to do it once
+_global_xmp_template: Template | None = None
+
 
 # return values for _should_update_photo
 class ShouldUpdate(Enum):
     NOT_IN_DATABASE = 1
     HARDLINK_DIFFERENT_FILES = 2
     NOT_HARDLINK_SAME_FILES = 3
     DEST_SIG_DIFFERENT = 4
@@ -331,14 +335,17 @@
         self.raw = self.raw or other.raw
         self.error += other.error
         return self
 
     def __str__(self):
         return str(self.asdict())
 
+    def __repr__(self):
+        return f"StagedFiles({self.asdict()})"
+
     def asdict(self):
         return {
             "original": self.original,
             "original_live": self.original_live,
             "edited": self.edited,
             "edited_live": self.edited_live,
             "preview": self.preview,
@@ -583,14 +590,23 @@
         dest = pathlib.Path(dest) / filename
 
         # Is there something to convert with convert_to_jpeg?
         dest, options = self._should_convert_to_jpeg(dest, options)
 
         # stage files for export by finding path in local library or
 downloading from iCloud as appropriate
+        # for `--download-missing` and `--update` case, this may cause
+unnecessary downloads
+        # as it will download the file even if it's not needed (won't be
+checked until the _should_update_photo() call from _export_photo()
+        # fixing this will require major refactoring of the export code, see
+#1086
+        # leaving it for now as this should not be a common use case
+        # (if using `--update` it is much better to be using "Download
+originals to this Mac" in Photos)
         staged_files = self._stage_photos_for_export(options)
         src = staged_files.edited if options.edited else staged_files.original
 
         # get the right destination path depending on options.update, etc.
         dest = self._get_dest_path(dest, options)
 
         self._render_options.filepath = str(dest)
@@ -791,17 +807,24 @@
 
         def _lock_filename(filename):
             """Lock filename if not in dry_run mode"""
             return lock_filename(filename) if lock else filename
 
         # if overwrite==False and #increment==False, export should fail if file
 exists
-        if dest.exists() and not any(
-            [options.increment, options.update, options.force_update,
-options.overwrite]
+        if (
+            not any(
+                [
+                    options.increment,
+                    options.update,
+                    options.force_update,
+                    options.overwrite,
+                ]
+            )
+            and dest.exists()
         ):
             raise FileExistsError(
                 f"destination exists ({dest}); overwrite={options.overwrite},
 increment={options.increment}"
             )
 
         # if overwrite, we don't care if the file exists or not
@@ -866,34 +889,47 @@
             return pathlib.Path(dest)
 
         # fail safe...I can't think of a case that gets here
         _lock_filename(dest)
         return dest
 
     def _should_update_photo(
-        self, src: pathlib.Path, dest: pathlib.Path, options: ExportOptions
-    ) -> t.Literal[True, False]:
-        """Return True if photo should be updated, else False"""
+        self, src: pathlib.Path | None, dest: pathlib.Path, options:
+ExportOptions
+    ) -> bool | ShouldUpdate:
+        """Return True if photo should be updated, else False
+
+        Args:
+            src (pathlib.Path | None): source path; if None, photo is missing
+and
+                any checks that require src will return True
+            dest (pathlib.Path): destination path
+
+        Returns:
+            False if photo should not be updated otherwise a truthy
+ShouldUpdate value
+        """
+
         # NOTE: The order of certain checks is important
         # read the comments below to understand why before changing
 
         export_db = options.export_db
         fileutil = options.fileutil
 
         file_record = export_db.get_file_record(dest)
 
         if not file_record:
             # photo doesn't exist in database, should update
             return ShouldUpdate.NOT_IN_DATABASE
 
-        if options.export_as_hardlink and not dest.samefile(src):
+        if options.export_as_hardlink and (not src or not dest.samefile(src)):
             # different files, should update
             return ShouldUpdate.HARDLINK_DIFFERENT_FILES
 
-        if not options.export_as_hardlink and dest.samefile(src):
+        if not options.export_as_hardlink and (not src or dest.samefile(src)):
             # same file but not exporting as hardlink, should update
             return ShouldUpdate.NOT_HARDLINK_SAME_FILES
 
         if not options.ignore_signature and not fileutil.cmp_file_sig(
             dest, file_record.dest_sig
         ):
             # destination file doesn't match what was last exported
@@ -921,16 +957,17 @@
         if options.exiftool:
             current_exifdata = self.exiftool_json_sidecar(options=options)
             rv = current_exifdata != file_record.exifdata
             # if using exiftool, don't need to continue checking edited below
             # as exiftool will be used to update edited file
             return ShouldUpdate.EXIFTOOL_DIFFERENT if rv else False
 
-        if options.edited and not fileutil.cmp_file_sig(src,
-file_record.src_sig):
+        if options.edited and (
+            not src or not fileutil.cmp_file_sig(src, file_record.src_sig)
+        ):
             # edited file in Photos doesn't match what was last exported
             return ShouldUpdate.EDITED_SIG_DIFFERENT
 
         if options.force_update:
             current_digest = self.photo.hexdigest
             if current_digest != file_record.digest:
                 # metadata in Photos changed, force update
@@ -976,31 +1013,60 @@
             # edited file
             staged.edited = self.photo.path_edited
             if options.live_photo and self.photo.live_photo:
                 staged.edited_live = self.photo.path_edited_live_photo
 
         # download any missing files
         if options.download_missing:
-            live_photo = staged.edited_live if options.edited else
+            staged |= self._stage_missing_photos_for_export(
+                staged=staged, options=options
+            )
+
+        return staged
+
+    def _stage_missing_photos_for_export(
+        self, staged: StagedFiles, options: ExportOptions
+    ) -> StagedFiles:
+        """Download and stage any missing files for export"""
+
+        # if live photo and requesting edited version need the edited live
+photo
+        live_photo = staged.edited_live if options.edited else
 staged.original_live
-            missing_options = ExportOptions(
-                edited=options.edited,
-                preview=options.preview and not staged.preview,
-                raw_photo=options.raw_photo and not staged.raw,
-                live_photo=options.live_photo and not live_photo,
-            )
-            if options.use_photokit:
-                missing_staged = self._stage_photo_for_export_with_photokit(
-                    options=missing_options
-                )
-            else:
-                missing_staged = self._stage_photo_for_export_with_applescript(
-                    options=missing_options
-                )
-            staged |= missing_staged
+
+        # is there actually a missing file? (#1086)
+        something_to_download = (
+            (self.photo.hasadjustments and options.edited and not
+staged.edited)
+            or (self.photo.live_photo and options.live_photo and not
+live_photo)
+            or (self.photo.has_raw and options.raw_photo and not staged.raw)
+            or (options.preview and not staged.preview)
+            or (not options.edited and not staged.original)
+        )
+        if not something_to_download:
+            return staged
+
+        missing_options = ExportOptions(
+            edited=options.edited,
+            preview=options.preview and not staged.preview,
+            raw_photo=self.photo.has_raw and options.raw_photo and not
+staged.raw,
+            live_photo=self.photo.live_photo and options.live_photo and not
+live_photo,
+        )
+        if options.use_photokit:
+            missing_staged = self._stage_photo_for_export_with_photokit(
+                options=missing_options
+            )
+        else:
+            missing_staged = self._stage_photo_for_export_with_applescript(
+                options=missing_options
+            )
+        staged |= missing_staged
         return staged
 
     def _stage_photo_for_export_with_photokit(
         self,
         options: ExportOptions,
     ) -> StagedFiles:
         """Stage a photo for export with photokit to a temporary directory"""
@@ -2204,20 +2270,15 @@
             options (ExportOptions): options for export
             extension (t.Optional[str]): which extension to use for
 SidecarForExtension property
         """
 
         options = options or ExportOptions()
 
-        xmp_template_file = (
-            _XMP_TEMPLATE_NAME if not self.photo._db._beta else
-_XMP_TEMPLATE_NAME_BETA
-        )
-        xmp_template = Template(filename=os.path.join(_TEMPLATE_DIR,
-xmp_template_file))
+        xmp_template = self._xmp_template()
 
         if extension is None:
             extension = pathlib.Path(self.photo.original_filename)
             extension = extension.suffix[1:] if extension.suffix else None
 
         if options.description_template is not None:
             render_options = dataclasses.replace(
@@ -2322,14 +2383,30 @@
         )
 
         # remove extra lines that mako inserts from template
         xmp_str = "\n".join(line for line in xmp_str.split("\n") if line.strip
 () != "")
         return xmp_str
 
+    def _xmp_template(self):
+        """Return the mako template for XMP sidecar, creating it if
+necessary"""
+        global _global_xmp_template
+        if _global_xmp_template is not None:
+            return _global_xmp_template
+
+        xmp_template_file = (
+            _XMP_TEMPLATE_NAME_BETA if self.photo._db._beta else
+_XMP_TEMPLATE_NAME
+        )
+        _global_xmp_template = Template(
+            filename=os.path.join(_TEMPLATE_DIR, xmp_template_file)
+        )
+        return _global_xmp_template
+
     def _write_sidecar(self, filename, sidecar_str):
         """write sidecar_str to filename
         used for exporting sidecar info"""
         if not (filename or sidecar_str):
             raise (
                 ValueError(
                     f"filename {filename} and sidecar_str {sidecar_str} must
```

#### docs/_modules/osxphotos/export_db.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.export_db - osxphotos 0.60.1 documentation</title>
+        <title>osxphotos.export_db - osxphotos 0.60.2 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.60.1 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.60.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.1_documentation
+osxphotos_0.60.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.1_documentation
+osxphotos_0.60.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_modules/osxphotos/scoreinfo.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.scoreinfo - osxphotos 0.58.1 documentation</title>
+        <title>osxphotos.scoreinfo - osxphotos 0.60.2 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.58.1 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.60.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.58.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.58.1_documentation
+osxphotos_0.60.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.58.1_documentation
+osxphotos_0.60.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_modules/osxphotos/photoinfo.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.photoinfo - osxphotos 0.60.0 documentation</title>
+        <title>osxphotos.photoinfo - osxphotos 0.60.2 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.60.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -1070,54 +1070,75 @@
     <span class="k">def</span> <span class="nf">path_live_photo</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;Returns path to the associated video file for a live photo</span>
 <span class="sd">        If photo is not a live photo, returns None</span>
 <span class="sd">        If photo is missing, returns None&quot;&quot;&quot;</span>
 
         <span class="n">photopath</span> <span class="o">=</span> <span class="kc">None</span>
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_db_version</span> <span class="o">&lt;=</span> <span class="n">_PHOTOS_4_VERSION</span><span class="p">:</span>
-            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">live_photo</span> <span class="ow">and</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">ismissing</span><span class="p">:</span>
-                <span class="n">live_model_id</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;live_model_id&quot;</span><span class="p">]</span>
-                <span class="k">if</span> <span class="n">live_model_id</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
-                    <span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;missing live_model_id: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_uuid</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-                    <span class="n">photopath</span> <span class="o">=</span> <span class="kc">None</span>
-                <span class="k">else</span><span class="p">:</span>
-                    <span class="n">folder_id</span><span class="p">,</span> <span class="n">file_id</span><span class="p">,</span> <span class="n">nn_id</span> <span class="o">=</span> <span class="n">_get_resource_loc</span><span class="p">(</span><span class="n">live_model_id</span><span class="p">)</span>
-                    <span class="n">library_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">library_path</span>
-                    <span class="n">photopath</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
-                        <span class="n">library_path</span><span class="p">,</span>
-                        <span class="s2">&quot;resources&quot;</span><span class="p">,</span>
-                        <span class="s2">&quot;media&quot;</span><span class="p">,</span>
-                        <span class="s2">&quot;master&quot;</span><span class="p">,</span>
-                        <span class="n">folder_id</span><span class="p">,</span>
-                        <span class="n">nn_id</span><span class="p">,</span>
-                        <span class="sa">f</span><span class="s2">&quot;jpegvideocomplement_</span><span class="si">{</span><span class="n">file_id</span><span class="si">}</span><span class="s2">.mov&quot;</span><span class="p">,</span>
-                    <span class="p">)</span>
-                    <span class="k">if</span> <span class="ow">not</span> <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">isfile</span><span class="p">(</span><span class="n">photopath</span><span class="p">):</span>
-                        <span class="c1"># In testing, I&#39;ve seen occasional missing movie for live photo</span>
-                        <span class="c1"># These appear to be valid -- e.g. live component hasn&#39;t been downloaded from iCloud</span>
-                        <span class="c1"># photos 4 has &quot;isOnDisk&quot; column we could check</span>
-                        <span class="c1"># or could do the actual check with &quot;isfile&quot;</span>
-                        <span class="c1"># TODO: should this be a warning or debug?</span>
-                        <span class="n">photopath</span> <span class="o">=</span> <span class="kc">None</span>
-            <span class="k">else</span><span class="p">:</span>
-                <span class="n">photopath</span> <span class="o">=</span> <span class="kc">None</span>
+            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_path_live_photo_4</span><span class="p">()</span>
         <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">live_photo</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">path</span> <span class="ow">and</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">ismissing</span><span class="p">:</span>
+            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">shared</span><span class="p">:</span>
+                <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_path_live_photo_shared_5</span><span class="p">()</span>
             <span class="n">filename</span> <span class="o">=</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">path</span><span class="p">)</span>
             <span class="n">photopath</span> <span class="o">=</span> <span class="n">filename</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">joinpath</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">filename</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">_3.mov&quot;</span><span class="p">)</span>
             <span class="n">photopath</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">photopath</span><span class="p">)</span>
             <span class="k">if</span> <span class="ow">not</span> <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">isfile</span><span class="p">(</span><span class="n">photopath</span><span class="p">):</span>
                 <span class="c1"># In testing, I&#39;ve seen occasional missing movie for live photo</span>
                 <span class="c1"># these appear to be valid -- e.g. video component not yet downloaded from iCloud</span>
                 <span class="c1"># TODO: should this be a warning or debug?</span>
                 <span class="n">photopath</span> <span class="o">=</span> <span class="kc">None</span>
         <span class="k">else</span><span class="p">:</span>
             <span class="n">photopath</span> <span class="o">=</span> <span class="kc">None</span>
 
         <span class="k">return</span> <span class="n">photopath</span>
 
+    <span class="k">def</span> <span class="nf">_path_live_photo_shared_5</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+        <span class="sd">&quot;&quot;&quot;Return path for live photo for shared photos&quot;&quot;&quot;</span>
+        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">shared</span><span class="p">:</span>
+            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;photo </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">uuid</span><span class="si">}</span><span class="s2"> is not a shared photo&quot;</span><span class="p">)</span>
+        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">live_photo</span><span class="p">:</span>
+            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;photo </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">uuid</span><span class="si">}</span><span class="s2"> is not a live photo&quot;</span><span class="p">)</span>
+
+        <span class="n">photopath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_path_5_shared</span><span class="p">()</span>
+        <span class="k">if</span> <span class="n">photopath</span><span class="p">:</span>
+            <span class="n">photopath</span> <span class="o">=</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">(</span><span class="n">photopath</span><span class="p">)</span><span class="o">.</span><span class="n">with_suffix</span><span class="p">(</span><span class="s2">&quot;.MOV&quot;</span><span class="p">)</span>
+            <span class="k">if</span> <span class="ow">not</span> <span class="n">photopath</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+                <span class="n">photopath</span> <span class="o">=</span> <span class="kc">None</span>
+        <span class="k">return</span> <span class="n">photopath</span>
+
+    <span class="k">def</span> <span class="nf">_path_live_photo_4</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+        <span class="sd">&quot;&quot;&quot;Return path for live edited photo for Photos &lt;= 4&quot;&quot;&quot;</span>
+        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">live_photo</span> <span class="ow">and</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">ismissing</span><span class="p">:</span>
+            <span class="n">live_model_id</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;live_model_id&quot;</span><span class="p">]</span>
+            <span class="k">if</span> <span class="n">live_model_id</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
+                <span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;missing live_model_id: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_uuid</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+                <span class="n">photopath</span> <span class="o">=</span> <span class="kc">None</span>
+            <span class="k">else</span><span class="p">:</span>
+                <span class="n">folder_id</span><span class="p">,</span> <span class="n">file_id</span><span class="p">,</span> <span class="n">nn_id</span> <span class="o">=</span> <span class="n">_get_resource_loc</span><span class="p">(</span><span class="n">live_model_id</span><span class="p">)</span>
+                <span class="n">library_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">library_path</span>
+                <span class="n">photopath</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+                    <span class="n">library_path</span><span class="p">,</span>
+                    <span class="s2">&quot;resources&quot;</span><span class="p">,</span>
+                    <span class="s2">&quot;media&quot;</span><span class="p">,</span>
+                    <span class="s2">&quot;master&quot;</span><span class="p">,</span>
+                    <span class="n">folder_id</span><span class="p">,</span>
+                    <span class="n">nn_id</span><span class="p">,</span>
+                    <span class="sa">f</span><span class="s2">&quot;jpegvideocomplement_</span><span class="si">{</span><span class="n">file_id</span><span class="si">}</span><span class="s2">.mov&quot;</span><span class="p">,</span>
+                <span class="p">)</span>
+                <span class="k">if</span> <span class="ow">not</span> <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">isfile</span><span class="p">(</span><span class="n">photopath</span><span class="p">):</span>
+                    <span class="c1"># In testing, I&#39;ve seen occasional missing movie for live photo</span>
+                    <span class="c1"># These appear to be valid -- e.g. live component hasn&#39;t been downloaded from iCloud</span>
+                    <span class="c1"># photos 4 has &quot;isOnDisk&quot; column we could check</span>
+                    <span class="c1"># or could do the actual check with &quot;isfile&quot;</span>
+                    <span class="c1"># TODO: should this be a warning or debug?</span>
+                    <span class="n">photopath</span> <span class="o">=</span> <span class="kc">None</span>
+        <span class="k">else</span><span class="p">:</span>
+            <span class="n">photopath</span> <span class="o">=</span> <span class="kc">None</span>
+        <span class="k">return</span> <span class="n">photopath</span>
+
     <span class="nd">@cached_property</span>
     <span class="k">def</span> <span class="nf">path_derivatives</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;Return any derivative (preview) images associated with the photo as a list of paths, sorted by file size (largest first)&quot;&quot;&quot;</span>
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_db_version</span> <span class="o">&lt;=</span> <span class="n">_PHOTOS_4_VERSION</span><span class="p">:</span>
             <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_path_derivatives_4</span><span class="p">()</span>
 
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">shared</span><span class="p">:</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -969,58 +969,78 @@
     def path_live_photo(self):
         """Returns path to the associated video file for a live photo
         If photo is not a live photo, returns None
         If photo is missing, returns None"""
 
         photopath = None
         if self._db._db_version <= _PHOTOS_4_VERSION:
-            if self.live_photo and not self.ismissing:
-                live_model_id = self._info["live_model_id"]
-                if live_model_id is None:
-                    logger.debug(f"missing live_model_id: {self._uuid}")
-                    photopath = None
-                else:
-                    folder_id, file_id, nn_id = _get_resource_loc
-(live_model_id)
-                    library_path = self._db.library_path
-                    photopath = os.path.join(
-                        library_path,
-                        "resources",
-                        "media",
-                        "master",
-                        folder_id,
-                        nn_id,
-                        f"jpegvideocomplement_{file_id}.mov",
-                    )
-                    if not os.path.isfile(photopath):
-                        # In testing, I've seen occasional missing movie for
-live photo
-                        # These appear to be valid -- e.g. live component
-hasn't been downloaded from iCloud
-                        # photos 4 has "isOnDisk" column we could check
-                        # or could do the actual check with "isfile"
-                        # TODO: should this be a warning or debug?
-                        photopath = None
-            else:
-                photopath = None
+            return self._path_live_photo_4()
         elif self.live_photo and self.path and not self.ismissing:
+            if self.shared:
+                return self._path_live_photo_shared_5()
             filename = pathlib.Path(self.path)
             photopath = filename.parent.joinpath(f"{filename.stem}_3.mov")
             photopath = str(photopath)
             if not os.path.isfile(photopath):
                 # In testing, I've seen occasional missing movie for live photo
                 # these appear to be valid -- e.g. video component not yet
 downloaded from iCloud
                 # TODO: should this be a warning or debug?
                 photopath = None
         else:
             photopath = None
 
         return photopath
 
+    def _path_live_photo_shared_5(self):
+        """Return path for live photo for shared photos"""
+        if not self.shared:
+            raise ValueError(f"photo {self.uuid} is not a shared photo")
+        if not self.live_photo:
+            raise ValueError(f"photo {self.uuid} is not a live photo")
+
+        photopath = self._path_5_shared()
+        if photopath:
+            photopath = pathlib.Path(photopath).with_suffix(".MOV")
+            if not photopath.exists():
+                photopath = None
+        return photopath
+
+    def _path_live_photo_4(self):
+        """Return path for live edited photo for Photos <= 4"""
+        if self.live_photo and not self.ismissing:
+            live_model_id = self._info["live_model_id"]
+            if live_model_id is None:
+                logger.debug(f"missing live_model_id: {self._uuid}")
+                photopath = None
+            else:
+                folder_id, file_id, nn_id = _get_resource_loc(live_model_id)
+                library_path = self._db.library_path
+                photopath = os.path.join(
+                    library_path,
+                    "resources",
+                    "media",
+                    "master",
+                    folder_id,
+                    nn_id,
+                    f"jpegvideocomplement_{file_id}.mov",
+                )
+                if not os.path.isfile(photopath):
+                    # In testing, I've seen occasional missing movie for live
+photo
+                    # These appear to be valid -- e.g. live component hasn't
+been downloaded from iCloud
+                    # photos 4 has "isOnDisk" column we could check
+                    # or could do the actual check with "isfile"
+                    # TODO: should this be a warning or debug?
+                    photopath = None
+        else:
+            photopath = None
+        return photopath
+
     @cached_property
     def path_derivatives(self):
         """Return any derivative (preview) images associated with the photo as
 a list of paths, sorted by file size (largest first)"""
         if self._db._db_version <= _PHOTOS_4_VERSION:
             return self._path_derivatives_4()
```

#### docs/_modules/osxphotos/photosdb/_photosdb_process_comments.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../../genindex.html" /><link rel="search" title="Search" href="../../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.photosdb._photosdb_process_comments - osxphotos 0.58.1 documentation</title>
+        <title>osxphotos.photosdb._photosdb_process_comments - osxphotos 0.60.2 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../../index.html"><div class="brand">osxphotos 0.58.1 documentation</div></a>
+      <a href="../../../index.html"><div class="brand">osxphotos 0.60.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.58.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.58.1_documentation
+osxphotos_0.60.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.58.1_documentation
+osxphotos_0.60.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_modules/osxphotos/photosdb/photosdb.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../../genindex.html" /><link rel="search" title="Search" href="../../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.photosdb.photosdb - osxphotos 0.60.0 documentation</title>
+        <title>osxphotos.photosdb.photosdb - osxphotos 0.60.2 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../../index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
+      <a href="../../../index.html"><div class="brand">osxphotos 0.60.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_sources/template_help.rst.txt

```diff
@@ -357,15 +357,15 @@
    * - {cr}
      - A carriage return: '\r'
    * - {crlf}
      - A carriage return + line feed: '\r\n'
    * - {tab}
      - :A tab: '\t'
    * - {osxphotos_version}
-     - The osxphotos version, e.g. '0.60.1'
+     - The osxphotos version, e.g. '0.60.2'
    * - {osxphotos_cmd_line}
      - The full command line used to run osxphotos
    * - {album}
      - Album(s) photo is contained in
    * - {folder_album}
      - Folder path + album photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder
    * - {project}
```

#### docs/_static/documentation_options.js

##### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 var DOCUMENTATION_OPTIONS = {
     URL_ROOT: document.getElementById("documentation_options").getAttribute('data-url_root'),
-    VERSION: '0.60.1',
+    VERSION: '0.60.2',
     LANGUAGE: 'en',
     COLLAPSE_INDEX: false,
     BUILDER: 'html',
     FILE_SUFFIX: '.html',
     LINK_SUFFIX: '.html',
     HAS_SOURCE: true,
     SOURCELINK_SUFFIX: '.txt',
```

#### docs/cli.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Template System" href="template_help.html" /><link rel="prev" title="OSXPhotos Tutorial" href="tutorial.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Command Line Interface (CLI) - osxphotos 0.60.1 documentation</title>
+        <title>OSXPhotos Command Line Interface (CLI) - osxphotos 0.60.2 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.1 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.1_documentation
+osxphotos_0.60.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.1_documentation
+osxphotos_0.60.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/genindex.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="#" /><link rel="search" title="Search" href="search.html" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Index - osxphotos 0.60.1 documentation</title>
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Index - osxphotos 0.60.2 documentation</title>
 <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -118,15 +118,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.1 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -141,15 +141,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.1_documentation
+osxphotos_0.60.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.1_documentation
+osxphotos_0.60.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/index.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos" href="overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos 0.60.1 documentation</title>
+        <title>osxphotos 0.60.2 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="#"><div class="brand">osxphotos 0.60.1 documentation</div></a>
+      <a href="#"><div class="brand">osxphotos 0.60.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="#">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.1_documentation
+osxphotos_0.60.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.1_documentation
+osxphotos_0.60.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/overview.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Tutorial" href="tutorial.html" /><link rel="prev" title="Welcome to OSXPhotos’s documentation!" href="index.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos - osxphotos 0.60.1 documentation</title>
+        <title>OSXPhotos - osxphotos 0.60.2 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.1 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.1_documentation
+osxphotos_0.60.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.1_documentation
+osxphotos_0.60.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/package_overview.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Python Reference" href="reference.html" /><link rel="prev" title="OSXPhotos Template System" href="template_help.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Python Package Overview - osxphotos 0.60.1 documentation</title>
+        <title>OSXPhotos Python Package Overview - osxphotos 0.60.2 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.1 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.1_documentation
+osxphotos_0.60.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.1_documentation
+osxphotos_0.60.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/py-modindex.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Python Module Index - osxphotos 0.60.1 documentation</title>
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Python Module Index - osxphotos 0.60.2 documentation</title>
 <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -118,15 +118,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.1 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -141,15 +141,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.1_documentation
+osxphotos_0.60.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.1_documentation
+osxphotos_0.60.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/reference.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="prev" title="OSXPhotos Python Package Overview" href="package_overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Python Reference - osxphotos 0.60.1 documentation</title>
+        <title>OSXPhotos Python Reference - osxphotos 0.60.2 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.1 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -1369,15 +1369,15 @@
 <dd><p>Returns sort order of person; favorite persons are sorted before non-favorite persons”; Photos 5+ only; returns 0 on Photos &lt;= 4</p>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="osxphotos.PhotoExporter">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">osxphotos.</span></span><span class="sig-name descname"><span class="pre">PhotoExporter</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">photo</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#osxphotos.PhotoInfo" title="osxphotos.PhotoInfo"><span class="pre">PhotoInfo</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">tmpdir</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/osxphotos/photoexporter.html#PhotoExporter"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.PhotoExporter" title="Permalink to this definition">#</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">osxphotos.</span></span><span class="sig-name descname"><span class="pre">PhotoExporter</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">photo</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#osxphotos.PhotoInfo" title="osxphotos.PhotoInfo"><span class="pre">PhotoInfo</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">tmpdir</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">t.Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/osxphotos/photoexporter.html#PhotoExporter"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.PhotoExporter" title="Permalink to this definition">#</a></dt>
 <dd><p>Export a photo</p>
 <dl class="py method">
 <dt class="sig sig-object py" id="osxphotos.PhotoExporter.exiftool_json_sidecar">
 <span class="sig-name descname"><span class="pre">exiftool_json_sidecar</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">options</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#osxphotos.ExportOptions" title="osxphotos.photoexporter.ExportOptions"><span class="pre">ExportOptions</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">tag_groups</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">filename</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/osxphotos/photoexporter.html#PhotoExporter.exiftool_json_sidecar"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.PhotoExporter.exiftool_json_sidecar" title="Permalink to this definition">#</a></dt>
 <dd><dl class="simple">
 <dt>Return dict of EXIF details for building exiftool JSON sidecar or sending commands to ExifTool.</dt><dd><p>Does not include all the EXIF fields as those are likely already in the image.</p>
 </dd>
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.1_documentation
+osxphotos_0.60.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.1_documentation
+osxphotos_0.60.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -584,16 +584,16 @@
         json()[source]#
             Returns JSON representation of class instance
         propertyphotos#
             Returns list of PhotoInfo objects associated with this person
         propertysort_order#
             Returns sort order of person; favorite persons are sorted before
             non-favorite personsâ; Photos 5+ only; returns 0 on Photos <= 4
-  classosxphotos.PhotoExporter(photo: PhotoInfo, tmpdir: Optional[str] = None)
-  [source]#
+  classosxphotos.PhotoExporter(photo: PhotoInfo, tmpdir: t.Optional[str] =
+  None)[source]#
       Export a photo
         exiftool_json_sidecar(options: Optional[ExportOptions] = None,
         tag_groups: bool = True, filename: Optional[str] = None)[source]#
               Return dict of EXIF details for building exiftool JSON sidecar or
               sending commands to ExifTool.
                   Does not include all the EXIF fields as those are likely
                   already in the image.
```

#### docs/search.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="#" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Search - osxphotos 0.60.1 documentation</title><link rel="stylesheet" type="text/css" href="_static/pygments.css" />
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Search - osxphotos 0.60.2 documentation</title><link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
 
@@ -117,15 +117,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.1 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -140,15 +140,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="#" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.1_documentation
+osxphotos_0.60.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.1_documentation
+osxphotos_0.60.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/template_help.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Python Package Overview" href="package_overview.html" /><link rel="prev" title="OSXPhotos Command Line Interface (CLI)" href="cli.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Template System - osxphotos 0.60.1 documentation</title>
+        <title>OSXPhotos Template System - osxphotos 0.60.2 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.1 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -609,15 +609,15 @@
 <dt class="field-odd">A tab<span class="colon">:</span></dt>
 <dd class="field-odd"><p>‘t’</p>
 </dd>
 </dl>
 </td>
 </tr>
 <tr class="row-odd"><td><p>{osxphotos_version}</p></td>
-<td><p>The osxphotos version, e.g. ‘0.60.1’</p></td>
+<td><p>The osxphotos version, e.g. ‘0.60.2’</p></td>
 </tr>
 <tr class="row-even"><td><p>{osxphotos_cmd_line}</p></td>
 <td><p>The full command line used to run osxphotos</p></td>
 </tr>
 <tr class="row-odd"><td><p>{album}</p></td>
 <td><p>Album(s) photo is contained in</p></td>
 </tr>
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.1_documentation
+osxphotos_0.60.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.1_documentation
+osxphotos_0.60.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -428,15 +428,15 @@
 {closebracket}                 A close bracket: â]â
 {newline}                      A newline: ânâ
 {lf}                           A line feed: ânâ, alias for {newline}
 {cr}                           A carriage return: ârâ
 {crlf}                         A carriage return + line feed: ârnâ
 {tab}                            A tab:
                                      âtâ
-{osxphotos_version}            The osxphotos version, e.g. â0.60.1â
+{osxphotos_version}            The osxphotos version, e.g. â0.60.2â
 {osxphotos_cmd_line}           The full command line used to run osxphotos
 {album}                        Album(s) photo is contained in
 {folder_album}                 Folder path + album photo is contained in. e.g. âFolder/Subfolder/Albumâ or just âAlbumâ if
                                no enclosing folder
 {project}                      Project(s) photo is contained in (such as greeting cards, calendars, slideshows)
 {album_project}                Album(s) and project(s) photo is contained in; treats projects as regular albums
 {folder_album_project}         Folder path + album (includes projects as albums) photo is contained in. e.g. âFolder/Subfolder/
```

#### docs/tutorial.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Command Line Interface (CLI)" href="cli.html" /><link rel="prev" title="OSXPhotos" href="overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Tutorial - osxphotos 0.60.1 documentation</title>
+        <title>OSXPhotos Tutorial - osxphotos 0.60.2 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.1 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.1_documentation
+osxphotos_0.60.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.1_documentation
+osxphotos_0.60.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

### Comparing `osxphotos-0.60.1/osxphotos/exif_datetime_updater.py` & `osxphotos-0.60.2/osxphotos/exif_datetime_updater.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/exifinfo.py` & `osxphotos-0.60.2/osxphotos/exifinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/exiftool.py` & `osxphotos-0.60.2/osxphotos/exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/exiftool_filetypes.json` & `osxphotos-0.60.2/osxphotos/exiftool_filetypes.json`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/export_db.py` & `osxphotos-0.60.2/osxphotos/export_db.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/export_db_utils.py` & `osxphotos-0.60.2/osxphotos/export_db_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/fileutil.py` & `osxphotos-0.60.2/osxphotos/fileutil.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/frozen_photoinfo.py` & `osxphotos-0.60.2/osxphotos/frozen_photoinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/imageconverter.py` & `osxphotos-0.60.2/osxphotos/imageconverter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/momentinfo.py` & `osxphotos-0.60.2/osxphotos/momentinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/path_utils.py` & `osxphotos-0.60.2/osxphotos/path_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/personinfo.py` & `osxphotos-0.60.2/osxphotos/personinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/photodates.py` & `osxphotos-0.60.2/osxphotos/photodates.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/photoexporter.py` & `osxphotos-0.60.2/osxphotos/photoexporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """ PhotoExport class to export photos
 """
 
+from __future__ import annotations
+
 import dataclasses
 import json
 import logging
 import os
 import pathlib
 import re
-import sys
 import typing as t
-from collections import namedtuple  # pylint: disable=syntax-error
 from dataclasses import asdict, dataclass
 from datetime import datetime
 from enum import Enum
 from types import SimpleNamespace
 
 from mako.template import Template
 
@@ -35,18 +35,18 @@
 from .exiftool import ExifTool, ExifToolCaching, exiftool_can_write, get_exiftool_path
 from .export_db import ExportDB, ExportDBTemp
 from .fileutil import FileUtil
 from .phototemplate import RenderOptions
 from .rich_utils import add_rich_markup_tag
 from .uti import get_preferred_uti_extension
 from .utils import (
-    is_macos,
     hexdigest,
     increment_filename,
     increment_filename_with_count,
+    is_macos,
     lineno,
     list_directory,
     lock_filename,
     normalize_fs_path,
     unlock_filename,
 )
 
@@ -72,14 +72,18 @@
 
 if t.TYPE_CHECKING:
     from .photoinfo import PhotoInfo
 
 # retry if download_missing/use_photos_export fails the first time (which sometimes it does)
 MAX_PHOTOSCRIPT_RETRIES = 3
 
+# Global to hold the compiled XMP template
+# This is expensive to compile so we only want to do it once
+_global_xmp_template: Template | None = None
+
 
 # return values for _should_update_photo
 class ShouldUpdate(Enum):
     NOT_IN_DATABASE = 1
     HARDLINK_DIFFERENT_FILES = 2
     NOT_HARDLINK_SAME_FILES = 3
     DEST_SIG_DIFFERENT = 4
@@ -240,14 +244,17 @@
         self.raw = self.raw or other.raw
         self.error += other.error
         return self
 
     def __str__(self):
         return str(self.asdict())
 
+    def __repr__(self):
+        return f"StagedFiles({self.asdict()})"
+
     def asdict(self):
         return {
             "original": self.original,
             "original_live": self.original_live,
             "edited": self.edited,
             "edited_live": self.edited_live,
             "preview": self.preview,
@@ -475,14 +482,19 @@
             filename = filename or self.photo.original_filename
         dest = pathlib.Path(dest) / filename
 
         # Is there something to convert with convert_to_jpeg?
         dest, options = self._should_convert_to_jpeg(dest, options)
 
         # stage files for export by finding path in local library or downloading from iCloud as appropriate
+        # for `--download-missing` and `--update` case, this may cause unnecessary downloads
+        # as it will download the file even if it's not needed (won't be checked until the _should_update_photo() call from _export_photo()
+        # fixing this will require major refactoring of the export code, see #1086
+        # leaving it for now as this should not be a common use case
+        # (if using `--update` it is much better to be using "Download originals to this Mac" in Photos)
         staged_files = self._stage_photos_for_export(options)
         src = staged_files.edited if options.edited else staged_files.original
 
         # get the right destination path depending on options.update, etc.
         dest = self._get_dest_path(dest, options)
 
         self._render_options.filepath = str(dest)
@@ -661,16 +673,24 @@
         lock = not options.dry_run
 
         def _lock_filename(filename):
             """Lock filename if not in dry_run mode"""
             return lock_filename(filename) if lock else filename
 
         # if overwrite==False and #increment==False, export should fail if file exists
-        if dest.exists() and not any(
-            [options.increment, options.update, options.force_update, options.overwrite]
+        if (
+            not any(
+                [
+                    options.increment,
+                    options.update,
+                    options.force_update,
+                    options.overwrite,
+                ]
+            )
+            and dest.exists()
         ):
             raise FileExistsError(
                 f"destination exists ({dest}); overwrite={options.overwrite}, increment={options.increment}"
             )
 
         # if overwrite, we don't care if the file exists or not
         if options.overwrite and _lock_filename(dest):
@@ -721,34 +741,44 @@
             return pathlib.Path(dest)
 
         # fail safe...I can't think of a case that gets here
         _lock_filename(dest)
         return dest
 
     def _should_update_photo(
-        self, src: pathlib.Path, dest: pathlib.Path, options: ExportOptions
-    ) -> t.Literal[True, False]:
-        """Return True if photo should be updated, else False"""
+        self, src: pathlib.Path | None, dest: pathlib.Path, options: ExportOptions
+    ) -> bool | ShouldUpdate:
+        """Return True if photo should be updated, else False
+
+        Args:
+            src (pathlib.Path | None): source path; if None, photo is missing and
+                any checks that require src will return True
+            dest (pathlib.Path): destination path
+
+        Returns:
+            False if photo should not be updated otherwise a truthy ShouldUpdate value
+        """
+
         # NOTE: The order of certain checks is important
         # read the comments below to understand why before changing
 
         export_db = options.export_db
         fileutil = options.fileutil
 
         file_record = export_db.get_file_record(dest)
 
         if not file_record:
             # photo doesn't exist in database, should update
             return ShouldUpdate.NOT_IN_DATABASE
 
-        if options.export_as_hardlink and not dest.samefile(src):
+        if options.export_as_hardlink and (not src or not dest.samefile(src)):
             # different files, should update
             return ShouldUpdate.HARDLINK_DIFFERENT_FILES
 
-        if not options.export_as_hardlink and dest.samefile(src):
+        if not options.export_as_hardlink and (not src or dest.samefile(src)):
             # same file but not exporting as hardlink, should update
             return ShouldUpdate.NOT_HARDLINK_SAME_FILES
 
         if not options.ignore_signature and not fileutil.cmp_file_sig(
             dest, file_record.dest_sig
         ):
             # destination file doesn't match what was last exported
@@ -772,15 +802,17 @@
         if options.exiftool:
             current_exifdata = self.exiftool_json_sidecar(options=options)
             rv = current_exifdata != file_record.exifdata
             # if using exiftool, don't need to continue checking edited below
             # as exiftool will be used to update edited file
             return ShouldUpdate.EXIFTOOL_DIFFERENT if rv else False
 
-        if options.edited and not fileutil.cmp_file_sig(src, file_record.src_sig):
+        if options.edited and (
+            not src or not fileutil.cmp_file_sig(src, file_record.src_sig)
+        ):
             # edited file in Photos doesn't match what was last exported
             return ShouldUpdate.EDITED_SIG_DIFFERENT
 
         if options.force_update:
             current_digest = self.photo.hexdigest
             if current_digest != file_record.digest:
                 # metadata in Photos changed, force update
@@ -823,30 +855,54 @@
             # edited file
             staged.edited = self.photo.path_edited
             if options.live_photo and self.photo.live_photo:
                 staged.edited_live = self.photo.path_edited_live_photo
 
         # download any missing files
         if options.download_missing:
-            live_photo = staged.edited_live if options.edited else staged.original_live
-            missing_options = ExportOptions(
-                edited=options.edited,
-                preview=options.preview and not staged.preview,
-                raw_photo=options.raw_photo and not staged.raw,
-                live_photo=options.live_photo and not live_photo,
-            )
-            if options.use_photokit:
-                missing_staged = self._stage_photo_for_export_with_photokit(
-                    options=missing_options
-                )
-            else:
-                missing_staged = self._stage_photo_for_export_with_applescript(
-                    options=missing_options
-                )
-            staged |= missing_staged
+            staged |= self._stage_missing_photos_for_export(
+                staged=staged, options=options
+            )
+
+        return staged
+
+    def _stage_missing_photos_for_export(
+        self, staged: StagedFiles, options: ExportOptions
+    ) -> StagedFiles:
+        """Download and stage any missing files for export"""
+
+        # if live photo and requesting edited version need the edited live photo
+        live_photo = staged.edited_live if options.edited else staged.original_live
+
+        # is there actually a missing file? (#1086)
+        something_to_download = (
+            (self.photo.hasadjustments and options.edited and not staged.edited)
+            or (self.photo.live_photo and options.live_photo and not live_photo)
+            or (self.photo.has_raw and options.raw_photo and not staged.raw)
+            or (options.preview and not staged.preview)
+            or (not options.edited and not staged.original)
+        )
+        if not something_to_download:
+            return staged
+
+        missing_options = ExportOptions(
+            edited=options.edited,
+            preview=options.preview and not staged.preview,
+            raw_photo=self.photo.has_raw and options.raw_photo and not staged.raw,
+            live_photo=self.photo.live_photo and options.live_photo and not live_photo,
+        )
+        if options.use_photokit:
+            missing_staged = self._stage_photo_for_export_with_photokit(
+                options=missing_options
+            )
+        else:
+            missing_staged = self._stage_photo_for_export_with_applescript(
+                options=missing_options
+            )
+        staged |= missing_staged
         return staged
 
     def _stage_photo_for_export_with_photokit(
         self,
         options: ExportOptions,
     ) -> StagedFiles:
         """Stage a photo for export with photokit to a temporary directory"""
@@ -1955,18 +2011,15 @@
         Args:
             options (ExportOptions): options for export
             extension (t.Optional[str]): which extension to use for SidecarForExtension property
         """
 
         options = options or ExportOptions()
 
-        xmp_template_file = (
-            _XMP_TEMPLATE_NAME if not self.photo._db._beta else _XMP_TEMPLATE_NAME_BETA
-        )
-        xmp_template = Template(filename=os.path.join(_TEMPLATE_DIR, xmp_template_file))
+        xmp_template = self._xmp_template()
 
         if extension is None:
             extension = pathlib.Path(self.photo.original_filename)
             extension = extension.suffix[1:] if extension.suffix else None
 
         if options.description_template is not None:
             render_options = dataclasses.replace(
@@ -2065,14 +2118,28 @@
             rating=rating,
         )
 
         # remove extra lines that mako inserts from template
         xmp_str = "\n".join(line for line in xmp_str.split("\n") if line.strip() != "")
         return xmp_str
 
+    def _xmp_template(self):
+        """Return the mako template for XMP sidecar, creating it if necessary"""
+        global _global_xmp_template
+        if _global_xmp_template is not None:
+            return _global_xmp_template
+
+        xmp_template_file = (
+            _XMP_TEMPLATE_NAME_BETA if self.photo._db._beta else _XMP_TEMPLATE_NAME
+        )
+        _global_xmp_template = Template(
+            filename=os.path.join(_TEMPLATE_DIR, xmp_template_file)
+        )
+        return _global_xmp_template
+
     def _write_sidecar(self, filename, sidecar_str):
         """write sidecar_str to filename
         used for exporting sidecar info"""
         if not (filename or sidecar_str):
             raise (
                 ValueError(
                     f"filename {filename} and sidecar_str {sidecar_str} must not be None"
```

### Comparing `osxphotos-0.60.1/osxphotos/photoinfo.py` & `osxphotos-0.60.2/osxphotos/photoinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -873,54 +873,75 @@
     def path_live_photo(self):
         """Returns path to the associated video file for a live photo
         If photo is not a live photo, returns None
         If photo is missing, returns None"""
 
         photopath = None
         if self._db._db_version <= _PHOTOS_4_VERSION:
-            if self.live_photo and not self.ismissing:
-                live_model_id = self._info["live_model_id"]
-                if live_model_id is None:
-                    logger.debug(f"missing live_model_id: {self._uuid}")
-                    photopath = None
-                else:
-                    folder_id, file_id, nn_id = _get_resource_loc(live_model_id)
-                    library_path = self._db.library_path
-                    photopath = os.path.join(
-                        library_path,
-                        "resources",
-                        "media",
-                        "master",
-                        folder_id,
-                        nn_id,
-                        f"jpegvideocomplement_{file_id}.mov",
-                    )
-                    if not os.path.isfile(photopath):
-                        # In testing, I've seen occasional missing movie for live photo
-                        # These appear to be valid -- e.g. live component hasn't been downloaded from iCloud
-                        # photos 4 has "isOnDisk" column we could check
-                        # or could do the actual check with "isfile"
-                        # TODO: should this be a warning or debug?
-                        photopath = None
-            else:
-                photopath = None
+            return self._path_live_photo_4()
         elif self.live_photo and self.path and not self.ismissing:
+            if self.shared:
+                return self._path_live_photo_shared_5()
             filename = pathlib.Path(self.path)
             photopath = filename.parent.joinpath(f"{filename.stem}_3.mov")
             photopath = str(photopath)
             if not os.path.isfile(photopath):
                 # In testing, I've seen occasional missing movie for live photo
                 # these appear to be valid -- e.g. video component not yet downloaded from iCloud
                 # TODO: should this be a warning or debug?
                 photopath = None
         else:
             photopath = None
 
         return photopath
 
+    def _path_live_photo_shared_5(self):
+        """Return path for live photo for shared photos"""
+        if not self.shared:
+            raise ValueError(f"photo {self.uuid} is not a shared photo")
+        if not self.live_photo:
+            raise ValueError(f"photo {self.uuid} is not a live photo")
+
+        photopath = self._path_5_shared()
+        if photopath:
+            photopath = pathlib.Path(photopath).with_suffix(".MOV")
+            if not photopath.exists():
+                photopath = None
+        return photopath
+
+    def _path_live_photo_4(self):
+        """Return path for live edited photo for Photos <= 4"""
+        if self.live_photo and not self.ismissing:
+            live_model_id = self._info["live_model_id"]
+            if live_model_id is None:
+                logger.debug(f"missing live_model_id: {self._uuid}")
+                photopath = None
+            else:
+                folder_id, file_id, nn_id = _get_resource_loc(live_model_id)
+                library_path = self._db.library_path
+                photopath = os.path.join(
+                    library_path,
+                    "resources",
+                    "media",
+                    "master",
+                    folder_id,
+                    nn_id,
+                    f"jpegvideocomplement_{file_id}.mov",
+                )
+                if not os.path.isfile(photopath):
+                    # In testing, I've seen occasional missing movie for live photo
+                    # These appear to be valid -- e.g. live component hasn't been downloaded from iCloud
+                    # photos 4 has "isOnDisk" column we could check
+                    # or could do the actual check with "isfile"
+                    # TODO: should this be a warning or debug?
+                    photopath = None
+        else:
+            photopath = None
+        return photopath
+
     @cached_property
     def path_derivatives(self):
         """Return any derivative (preview) images associated with the photo as a list of paths, sorted by file size (largest first)"""
         if self._db._db_version <= _PHOTOS_4_VERSION:
             return self._path_derivatives_4()
 
         if self.shared:
```

### Comparing `osxphotos-0.60.1/osxphotos/photokit.py` & `osxphotos-0.60.2/osxphotos/photokit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/photosalbum.py` & `osxphotos-0.60.2/osxphotos/photosalbum.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/photoscript_utils.py` & `osxphotos-0.60.2/osxphotos/photoscript_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/photosdb/_photosdb_process_comments.py` & `osxphotos-0.60.2/osxphotos/photosdb/_photosdb_process_comments.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/photosdb/_photosdb_process_exif.py` & `osxphotos-0.60.2/osxphotos/photosdb/_photosdb_process_exif.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/photosdb/_photosdb_process_faceinfo.py` & `osxphotos-0.60.2/osxphotos/photosdb/_photosdb_process_faceinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/photosdb/_photosdb_process_scoreinfo.py` & `osxphotos-0.60.2/osxphotos/photosdb/_photosdb_process_scoreinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/photosdb/_photosdb_process_searchinfo.py` & `osxphotos-0.60.2/osxphotos/photosdb/_photosdb_process_searchinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/photosdb/photosdb.py` & `osxphotos-0.60.2/osxphotos/photosdb/photosdb.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/photosdb/photosdb_utils.py` & `osxphotos-0.60.2/osxphotos/photosdb/photosdb_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/phototables.py` & `osxphotos-0.60.2/osxphotos/phototables.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/phototemplate.cog.md` & `osxphotos-0.60.2/osxphotos/phototemplate.cog.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/phototemplate.md` & `osxphotos-0.60.2/osxphotos/phototemplate.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/phototemplate.py` & `osxphotos-0.60.2/osxphotos/phototemplate.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/phototemplate.tx` & `osxphotos-0.60.2/osxphotos/phototemplate.tx`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/phototz.py` & `osxphotos-0.60.2/osxphotos/phototz.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/placeinfo.py` & `osxphotos-0.60.2/osxphotos/placeinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/pyrepl.py` & `osxphotos-0.60.2/osxphotos/pyrepl.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/queries/shared_owner.sql.mako` & `osxphotos-0.60.2/osxphotos/queries/shared_owner.sql.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/query_builder.py` & `osxphotos-0.60.2/osxphotos/query_builder.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/queryoptions.py` & `osxphotos-0.60.2/osxphotos/queryoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/scoreinfo.py` & `osxphotos-0.60.2/osxphotos/scoreinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/searchinfo.py` & `osxphotos-0.60.2/osxphotos/searchinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/sqlgrep.py` & `osxphotos-0.60.2/osxphotos/sqlgrep.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/sqlite_utils.py` & `osxphotos-0.60.2/osxphotos/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/sqlitekvstore.py` & `osxphotos-0.60.2/osxphotos/sqlitekvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/template_counter.py` & `osxphotos-0.60.2/osxphotos/template_counter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/templates/xmp_sidecar.mako` & `osxphotos-0.60.2/osxphotos/templates/xmp_sidecar.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/templates/xmp_sidecar_beta.mako` & `osxphotos-0.60.2/osxphotos/templates/xmp_sidecar_beta.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/text_detection.py` & `osxphotos-0.60.2/osxphotos/text_detection.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/timeutils.py` & `osxphotos-0.60.2/osxphotos/timeutils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/timezones.py` & `osxphotos-0.60.2/osxphotos/timezones.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/tutorial.md` & `osxphotos-0.60.2/osxphotos/tutorial.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/uti.py` & `osxphotos-0.60.2/osxphotos/uti.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos/utils.py` & `osxphotos-0.60.2/osxphotos/utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos.egg-info/PKG-INFO` & `osxphotos-0.60.2/osxphotos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osxphotos
-Version: 0.60.1
+Version: 0.60.2
 Summary: Export photos from Apple's macOS Photos app and query the Photos library database to access metadata about images.
 Home-page: https://github.com/RhetTbull/
 Download-URL: https://github.com/RhetTbull/osxphotos
 Author: Rhet Turnbull
 Author-email: rturnbull+git@gmail.com
 License: License :: OSI Approved :: MIT License
 Project-URL: GitHub, https://github.com/RhetTbull/osxphotos
```

### Comparing `osxphotos-0.60.1/osxphotos.egg-info/SOURCES.txt` & `osxphotos-0.60.2/osxphotos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/osxphotos.egg-info/requires.txt` & `osxphotos-0.60.2/osxphotos.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/setup.py` & `osxphotos-0.60.2/setup.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_10_12_6.py` & `osxphotos-0.60.2/tests/test_10_12_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_albums_folders_catalina_10_15_7.py` & `osxphotos-0.60.2/tests/test_albums_folders_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_albums_folders_high_sierra_10_13_6.py` & `osxphotos-0.60.2/tests/test_albums_folders_high_sierra_10_13_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_albums_folders_mojave_10_14_6.py` & `osxphotos-0.60.2/tests/test_albums_folders_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_bigsur_10_16_0_1.py` & `osxphotos-0.60.2/tests/test_bigsur_10_16_0_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_catalina_10_15_7.py` & `osxphotos-0.60.2/tests/test_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_cli.py` & `osxphotos-0.60.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_cli_add_locations.py` & `osxphotos-0.60.2/tests/test_cli_add_locations.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_cli_add_to_album.py` & `osxphotos-0.60.2/tests/test_cli_add_to_album.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_cli_all_commands.py` & `osxphotos-0.60.2/tests/test_cli_all_commands.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_cli_batch_edit.py` & `osxphotos-0.60.2/tests/test_cli_batch_edit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_cli_dump.py` & `osxphotos-0.60.2/tests/test_cli_dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_cli_exiftool.py` & `osxphotos-0.60.2/tests/test_cli_exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_cli_export_cloud.py` & `osxphotos-0.60.2/tests/test_cli_export_cloud.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_cli_export_projects.py` & `osxphotos-0.60.2/tests/test_cli_export_projects.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_cli_exportdb.py` & `osxphotos-0.60.2/tests/test_cli_exportdb.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_cli_import.py` & `osxphotos-0.60.2/tests/test_cli_import.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_cli_orphans.py` & `osxphotos-0.60.2/tests/test_cli_orphans.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_cli_param_types.py` & `osxphotos-0.60.2/tests/test_cli_param_types.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_cli_sync.py` & `osxphotos-0.60.2/tests/test_cli_sync.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_cli_timewarp.py` & `osxphotos-0.60.2/tests/test_cli_timewarp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_cli_utils.py` & `osxphotos-0.60.2/tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_cli_verbose.py` & `osxphotos-0.60.2/tests/test_cli_verbose.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_cloud_owner_catalina.py` & `osxphotos-0.60.2/tests/test_cloud_owner_catalina.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_comments.py` & `osxphotos-0.60.2/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_concurrent_export.py` & `osxphotos-0.60.2/tests/test_concurrent_export.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_configoptions.py` & `osxphotos-0.60.2/tests/test_configoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_datetime_formatter.py` & `osxphotos-0.60.2/tests/test_datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_datetime_utils.py` & `osxphotos-0.60.2/tests/test_datetime_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_debug.py` & `osxphotos-0.60.2/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_empty_library_4_0.py` & `osxphotos-0.60.2/tests/test_empty_library_4_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_exif_info.py` & `osxphotos-0.60.2/tests/test_exif_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_exiftool.py` & `osxphotos-0.60.2/tests/test_exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_exiftool_caching.py` & `osxphotos-0.60.2/tests/test_exiftool_caching.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_export_catalina_10_15_7.py` & `osxphotos-0.60.2/tests/test_export_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_export_catalina_10_15_7_use_photos_export.py` & `osxphotos-0.60.2/tests/test_export_catalina_10_15_7_use_photos_export.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_export_convert_to_jpeg.py` & `osxphotos-0.60.2/tests/test_export_convert_to_jpeg.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_export_db.py` & `osxphotos-0.60.2/tests/test_export_db.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_export_mojave_10_14_6.py` & `osxphotos-0.60.2/tests/test_export_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_export_raw_catalina_10_15_1.py` & `osxphotos-0.60.2/tests/test_export_raw_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_exportresults.py` & `osxphotos-0.60.2/tests/test_exportresults.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_faceinfo.py` & `osxphotos-0.60.2/tests/test_faceinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_fileutil.py` & `osxphotos-0.60.2/tests/test_fileutil.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_highsierra.py` & `osxphotos-0.60.2/tests/test_highsierra.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_image_converter.py` & `osxphotos-0.60.2/tests/test_image_converter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_incloud_big_sur_10_16_0.py` & `osxphotos-0.60.2/tests/test_incloud_big_sur_10_16_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_incloud_catalina_10_15_1.py` & `osxphotos-0.60.2/tests/test_incloud_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_incloud_catalina_10_15_6.py` & `osxphotos-0.60.2/tests/test_incloud_catalina_10_15_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_incloud_mojave_10_14_6.py` & `osxphotos-0.60.2/tests/test_incloud_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_live_catalina_10_15_1.py` & `osxphotos-0.60.2/tests/test_live_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_modified_date_catalina_10_15_7.py` & `osxphotos-0.60.2/tests/test_modified_date_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_modified_date_mojave_10_14_6.py` & `osxphotos-0.60.2/tests/test_modified_date_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_mojave_10_14_6.py` & `osxphotos-0.60.2/tests/test_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_mojave_10_14_6_path_edited.py` & `osxphotos-0.60.2/tests/test_mojave_10_14_6_path_edited.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_monterey_12_0_1.py` & `osxphotos-0.60.2/tests/test_monterey_12_0_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_monterey_dev_beta_12_0_0.py` & `osxphotos-0.60.2/tests/test_monterey_dev_beta_12_0_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_movies_4_0.py` & `osxphotos-0.60.2/tests/test_movies_4_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_movies_5_0.py` & `osxphotos-0.60.2/tests/test_movies_5_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_path_utils.py` & `osxphotos-0.60.2/tests/test_path_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_personinfo.py` & `osxphotos-0.60.2/tests/test_personinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_photokit.py` & `osxphotos-0.60.2/tests/test_photokit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_photosdb_utils.py` & `osxphotos-0.60.2/tests/test_photosdb_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_placeinfo.py` & `osxphotos-0.60.2/tests/test_placeinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_places_catalina_10_15_1.py` & `osxphotos-0.60.2/tests/test_places_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_places_high_sierra_10_13_6.py` & `osxphotos-0.60.2/tests/test_places_high_sierra_10_13_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_places_mojave_10_14_6.py` & `osxphotos-0.60.2/tests/test_places_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_projects_catalina.py` & `osxphotos-0.60.2/tests/test_projects_catalina.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_projects_sierra.py` & `osxphotos-0.60.2/tests/test_projects_sierra.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_score_info.py` & `osxphotos-0.60.2/tests/test_score_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_search_info_10_14_6.py` & `osxphotos-0.60.2/tests/test_search_info_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_search_info_10_15_4.py` & `osxphotos-0.60.2/tests/test_search_info_10_15_4.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_search_info_10_15_5.py` & `osxphotos-0.60.2/tests/test_search_info_10_15_5.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_search_info_10_15_7.py` & `osxphotos-0.60.2/tests/test_search_info_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_shared_catalina_10_15_1.py` & `osxphotos-0.60.2/tests/test_shared_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_shared_mojave_10_14_6.py` & `osxphotos-0.60.2/tests/test_shared_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_sidecar_xmp.py` & `osxphotos-0.60.2/tests/test_sidecar_xmp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_specials_bigsur_10_16_0.py` & `osxphotos-0.60.2/tests/test_specials_bigsur_10_16_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_specials_catalina_10_15_1.py` & `osxphotos-0.60.2/tests/test_specials_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_specials_mojave_10_14_6.py` & `osxphotos-0.60.2/tests/test_specials_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_specials_sierra_10_12.py` & `osxphotos-0.60.2/tests/test_specials_sierra_10_12.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_sqlitekvstore.py` & `osxphotos-0.60.2/tests/test_sqlitekvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_template.py` & `osxphotos-0.60.2/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_template_counter.py` & `osxphotos-0.60.2/tests/test_template_counter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_template_today.py` & `osxphotos-0.60.2/tests/test_template_today.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_uti.py` & `osxphotos-0.60.2/tests/test_uti.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_utils.py` & `osxphotos-0.60.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_ventura_13_0_0.py` & `osxphotos-0.60.2/tests/test_ventura_13_0_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.1/tests/test_ventura_dev_preview_13_0_0.py` & `osxphotos-0.60.2/tests/test_ventura_dev_preview_13_0_0.py`

 * *Files identical despite different names*

