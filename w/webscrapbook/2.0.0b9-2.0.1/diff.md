# Comparing `tmp/webscrapbook-2.0.0b9.tar.gz` & `tmp/webscrapbook-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscrapbook-2.0.0b9.tar", last modified: Sun May 21 17:25:21 2023, max compression
+gzip compressed data, was "webscrapbook-2.0.1.tar", last modified: Sat Jun 17 13:07:49 2023, max compression
```

## Comparing `webscrapbook-2.0.0b9.tar` & `webscrapbook-2.0.1.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.335563 webscrapbook-2.0.0b9/
--rw-rw-rw-   0        0        0     1092 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/LICENSE.txt
--rw-rw-rw-   0        0        0       13 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/MANIFEST.in
--rw-rw-rw-   0        0        0     5611 2023-05-21 17:25:21.336562 webscrapbook-2.0.0b9/PKG-INFO
--rw-rw-rw-   0        0        0     4300 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/README.md
--rw-rw-rw-   0        0        0     2507 2023-05-21 17:25:21.337561 webscrapbook-2.0.0b9/setup.cfg
--rw-rw-rw-   0        0        0       63 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.268177 webscrapbook-2.0.0b9/webscrapbook/
--rw-rw-rw-   0        0        0     7184 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/__init__.py
--rw-rw-rw-   0        0        0      165 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.276169 webscrapbook-2.0.0b9/webscrapbook/_polyfill/
--rw-rw-rw-   0        0        0        0 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/_polyfill/__init__.py
--rw-rw-rw-   0        0        0     1445 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/_polyfill/argparse.py
--rw-rw-rw-   0        0        0     2084 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/_polyfill/mimetypes.py
--rw-rw-rw-   0        0        0      393 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/_polyfill/zipfile.py
--rw-rw-rw-   0        0        0    58752 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/app.py
--rw-rw-rw-   0        0        0    46681 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/cli.py
--rw-rw-rw-   0        0        0     3131 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/locales.py
-drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.282163 webscrapbook-2.0.0b9/webscrapbook/resources/
--rw-rw-rw-   0        0        0      144 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/resources/app.py
--rw-rw-rw-   0        0        0     1040 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/resources/config.ini
--rw-rw-rw-   0        0        0    13234 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/resources/config.md
--rw-rw-rw-   0        0        0     1505 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/resources/mimetypes.md
--rw-rw-rw-   0        0        0      128 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/resources/serve.py
--rw-rw-rw-   0        0        0     1542 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/resources/themes.md
-drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.290155 webscrapbook-2.0.0b9/webscrapbook/scrapbook/
--rw-rw-rw-   0        0        0        0 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/__init__.py
--rw-rw-rw-   0        0        0    51817 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/book.py
--rw-rw-rw-   0        0        0    38522 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/cache.py
--rw-rw-rw-   0        0        0    27936 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/check.py
-drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.295150 webscrapbook-2.0.0b9/webscrapbook/scrapbook/convert/
--rw-rw-rw-   0        0        0        0 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/convert/__init__.py
--rw-rw-rw-   0        0        0    11866 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/convert/file2wsb.py
--rw-rw-rw-   0        0        0    13580 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/convert/items.py
--rw-rw-rw-   0        0        0    41549 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/convert/migrate.py
--rw-rw-rw-   0        0        0    15455 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/convert/sb2wsb.py
--rw-rw-rw-   0        0        0     5934 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/convert/wsb2file.py
--rw-rw-rw-   0        0        0    26003 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/convert/wsb2sb.py
--rw-rw-rw-   0        0        0     9025 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/exporter.py
--rw-rw-rw-   0        0        0     6939 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/exporter1.py
--rw-rw-rw-   0        0        0    16513 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/host.py
--rw-rw-rw-   0        0        0    20553 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/importer.py
--rw-rw-rw-   0        0        0    20146 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/importer1.py
--rw-rw-rw-   0        0        0    38988 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/indexer.py
--rw-rw-rw-   0        0        0    19941 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/search.py
--rw-rw-rw-   0        0        0     7722 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/util.py
--rw-rw-rw-   0        0        0     2356 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/server.py
-drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.254915 webscrapbook-2.0.0b9/webscrapbook/themes/
-drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.258910 webscrapbook-2.0.0b9/webscrapbook/themes/default/
-drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.257911 webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/
-drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.296149 webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/ar/
--rw-rw-rw-   0        0        0       36 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/ar/messages.py
-drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.298147 webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/en/
--rw-rw-rw-   0        0        0     7783 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/en/messages.py
-drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.299146 webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/es/
--rw-rw-rw-   0        0        0     8853 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/es/messages.py
-drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.300145 webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/fa/
--rw-rw-rw-   0        0        0       36 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/fa/messages.py
-drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.300145 webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/he/
--rw-rw-rw-   0        0        0       36 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/he/messages.py
-drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.301144 webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/zh/
--rw-rw-rw-   0        0        0     7912 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/zh/messages.py
-drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.302142 webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/zh_cn/
--rw-rw-rw-   0        0        0     7929 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/zh_cn/messages.py
-drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.321219 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/
--rw-rw-rw-   0        0        0      281 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/collapse.png
--rw-rw-rw-   0        0        0      728 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/comment.png
--rw-rw-rw-   0        0        0      877 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/common.css
--rw-rw-rw-   0        0        0     3900 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/common.js
--rw-rw-rw-   0        0        0     1055 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/edit.css
--rw-rw-rw-   0        0        0     1563 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/edit.js
--rw-rw-rw-   0        0        0     2438 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/editx.js
--rw-rw-rw-   0        0        0      279 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/expand.png
--rw-rw-rw-   0        0        0      523 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/external.png
--rw-rw-rw-   0        0        0      752 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/fclose.png
--rw-rw-rw-   0        0        0      449 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/file.png
--rw-rw-rw-   0        0        0      790 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/fopen.png
--rw-rw-rw-   0        0        0     3810 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/index-ex.css
--rw-rw-rw-   0        0        0    61757 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/index-ex.js
--rw-rw-rw-   0        0        0     2210 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/index.css
--rw-rw-rw-   0        0        0     2156 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/index.js
--rw-rw-rw-   0        0        0      502 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/item.png
--rw-rw-rw-   0        0        0      387 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/link.png
--rw-rw-rw-   0        0        0      445 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/note.png
--rw-rw-rw-   0        0        0      515 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/postit.png
--rw-rw-rw-   0        0        0      661 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/search.png
--rw-rw-rw-   0        0        0      807 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/toggle.png
-drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.331568 webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/
--rw-rw-rw-   0        0        0      482 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/base.html
--rw-rw-rw-   0        0        0      632 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/cli.html
--rw-rw-rw-   0        0        0     1053 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/edit.html
--rw-rw-rw-   0        0        0      965 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/editx.html
--rw-rw-rw-   0        0        0     5632 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/index.html
--rw-rw-rw-   0        0        0      510 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/maff_index.html
--rw-rw-rw-   0        0        0      490 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/markdown.html
--rw-rw-rw-   0        0        0      568 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/static_frame.html
--rw-rw-rw-   0        0        0     1751 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/static_index.html
--rw-rw-rw-   0        0        0    12917 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/static_map.html
--rw-rw-rw-   0        0        0    26766 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/static_search.html
-drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.335563 webscrapbook-2.0.0b9/webscrapbook/util/
--rw-rw-rw-   0        0        0       72 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/util/__init__.py
--rw-rw-rw-   0        0        0     5867 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/util/css.py
--rw-rw-rw-   0        0        0    44456 2023-05-21 13:34:24.000000 webscrapbook-2.0.0b9/webscrapbook/util/fs.py
--rw-rw-rw-   0        0        0    15308 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/util/html.py
--rw-rw-rw-   0        0        0    36829 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/util/util.py
-drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.273172 webscrapbook-2.0.0b9/webscrapbook.egg-info/
--rw-rw-rw-   0        0        0     5611 2023-05-21 17:25:21.000000 webscrapbook-2.0.0b9/webscrapbook.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3500 2023-05-21 17:25:21.000000 webscrapbook-2.0.0b9/webscrapbook.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 17:25:21.000000 webscrapbook-2.0.0b9/webscrapbook.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-05-21 17:25:21.000000 webscrapbook-2.0.0b9/webscrapbook.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      264 2023-05-21 17:25:21.000000 webscrapbook-2.0.0b9/webscrapbook.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-21 17:25:21.000000 webscrapbook-2.0.0b9/webscrapbook.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-17 13:07:49.436253 webscrapbook-2.0.1/
+-rw-rw-rw-   0        0        0     1092 2023-05-14 13:37:39.000000 webscrapbook-2.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       13 2023-06-04 12:28:32.000000 webscrapbook-2.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5609 2023-06-17 13:07:49.436253 webscrapbook-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4300 2023-06-17 13:05:10.000000 webscrapbook-2.0.1/README.md
+-rw-rw-rw-   0        0        0     2509 2023-06-17 13:07:49.446466 webscrapbook-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0       63 2023-06-04 12:28:32.000000 webscrapbook-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 13:07:49.376387 webscrapbook-2.0.1/webscrapbook/
+-rw-rw-rw-   0        0        0     7180 2023-06-17 13:05:10.000000 webscrapbook-2.0.1/webscrapbook/__init__.py
+-rw-rw-rw-   0        0        0      165 2023-05-14 13:37:39.000000 webscrapbook-2.0.1/webscrapbook/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 13:07:49.386438 webscrapbook-2.0.1/webscrapbook/_polyfill/
+-rw-rw-rw-   0        0        0        0 2023-06-04 12:28:32.000000 webscrapbook-2.0.1/webscrapbook/_polyfill/__init__.py
+-rw-rw-rw-   0        0        0     1445 2023-06-04 12:28:32.000000 webscrapbook-2.0.1/webscrapbook/_polyfill/argparse.py
+-rw-rw-rw-   0        0        0     2169 2023-06-05 16:40:26.000000 webscrapbook-2.0.1/webscrapbook/_polyfill/mimetypes.py
+-rw-rw-rw-   0        0        0      393 2023-06-04 12:28:32.000000 webscrapbook-2.0.1/webscrapbook/_polyfill/zipfile.py
+-rw-rw-rw-   0        0        0    61077 2023-06-17 13:05:10.000000 webscrapbook-2.0.1/webscrapbook/app.py
+-rw-rw-rw-   0        0        0    47360 2023-06-17 13:05:10.000000 webscrapbook-2.0.1/webscrapbook/cli.py
+-rw-rw-rw-   0        0        0     3131 2023-06-04 12:28:32.000000 webscrapbook-2.0.1/webscrapbook/locales.py
+drwxrwxrwx   0        0        0        0 2023-06-17 13:07:49.396093 webscrapbook-2.0.1/webscrapbook/resources/
+-rw-rw-rw-   0        0        0      144 2023-05-14 13:37:39.000000 webscrapbook-2.0.1/webscrapbook/resources/app.py
+-rw-rw-rw-   0        0        0     1024 2023-06-17 13:05:10.000000 webscrapbook-2.0.1/webscrapbook/resources/config.ini
+-rw-rw-rw-   0        0        0    12833 2023-06-17 13:05:10.000000 webscrapbook-2.0.1/webscrapbook/resources/config.md
+-rw-rw-rw-   0        0        0     1505 2023-05-14 13:37:39.000000 webscrapbook-2.0.1/webscrapbook/resources/mimetypes.md
+-rw-rw-rw-   0        0        0      128 2023-05-14 13:37:39.000000 webscrapbook-2.0.1/webscrapbook/resources/serve.py
+-rw-rw-rw-   0        0        0     1542 2023-06-04 12:28:32.000000 webscrapbook-2.0.1/webscrapbook/resources/themes.md
+drwxrwxrwx   0        0        0        0 2023-06-17 13:07:49.396093 webscrapbook-2.0.1/webscrapbook/scrapbook/
+-rw-rw-rw-   0        0        0        0 2023-04-08 19:20:00.000000 webscrapbook-2.0.1/webscrapbook/scrapbook/__init__.py
+-rw-rw-rw-   0        0        0    53174 2023-06-17 13:05:10.000000 webscrapbook-2.0.1/webscrapbook/scrapbook/book.py
+-rw-rw-rw-   0        0        0    38525 2023-06-17 13:05:10.000000 webscrapbook-2.0.1/webscrapbook/scrapbook/cache.py
+-rw-rw-rw-   0        0        0    27996 2023-06-17 13:05:10.000000 webscrapbook-2.0.1/webscrapbook/scrapbook/check.py
+drwxrwxrwx   0        0        0        0 2023-06-17 13:07:49.406494 webscrapbook-2.0.1/webscrapbook/scrapbook/convert/
+-rw-rw-rw-   0        0        0        0 2023-04-08 19:20:00.000000 webscrapbook-2.0.1/webscrapbook/scrapbook/convert/__init__.py
+-rw-rw-rw-   0        0        0    11915 2023-06-17 13:05:10.000000 webscrapbook-2.0.1/webscrapbook/scrapbook/convert/file2wsb.py
+-rw-rw-rw-   0        0        0    13635 2023-06-17 13:05:10.000000 webscrapbook-2.0.1/webscrapbook/scrapbook/convert/items.py
+-rw-rw-rw-   0        0        0    41602 2023-06-17 13:05:10.000000 webscrapbook-2.0.1/webscrapbook/scrapbook/convert/migrate.py
+-rw-rw-rw-   0        0        0    15430 2023-06-17 13:05:10.000000 webscrapbook-2.0.1/webscrapbook/scrapbook/convert/sb2wsb.py
+-rw-rw-rw-   0        0        0     5914 2023-06-17 13:05:10.000000 webscrapbook-2.0.1/webscrapbook/scrapbook/convert/wsb2file.py
+-rw-rw-rw-   0        0        0    25978 2023-06-17 13:05:10.000000 webscrapbook-2.0.1/webscrapbook/scrapbook/convert/wsb2sb.py
+-rw-rw-rw-   0        0        0     9372 2023-06-17 13:05:10.000000 webscrapbook-2.0.1/webscrapbook/scrapbook/exporter.py
+-rw-rw-rw-   0        0        0     6939 2023-06-17 13:05:10.000000 webscrapbook-2.0.1/webscrapbook/scrapbook/exporter1.py
+-rw-rw-rw-   0        0        0    16542 2023-06-17 13:05:10.000000 webscrapbook-2.0.1/webscrapbook/scrapbook/host.py
+-rw-rw-rw-   0        0        0    20670 2023-06-17 13:05:10.000000 webscrapbook-2.0.1/webscrapbook/scrapbook/importer.py
+-rw-rw-rw-   0        0        0    20236 2023-06-17 13:05:10.000000 webscrapbook-2.0.1/webscrapbook/scrapbook/importer1.py
+-rw-rw-rw-   0        0        0    38988 2023-06-17 13:05:10.000000 webscrapbook-2.0.1/webscrapbook/scrapbook/indexer.py
+-rw-rw-rw-   0        0        0    19979 2023-06-17 13:05:10.000000 webscrapbook-2.0.1/webscrapbook/scrapbook/search.py
+-rw-rw-rw-   0        0        0     7614 2023-06-17 13:05:10.000000 webscrapbook-2.0.1/webscrapbook/scrapbook/util.py
+-rw-rw-rw-   0        0        0     2356 2023-05-14 13:37:39.000000 webscrapbook-2.0.1/webscrapbook/server.py
+drwxrwxrwx   0        0        0        0 2023-06-17 13:07:49.366503 webscrapbook-2.0.1/webscrapbook/themes/
+drwxrwxrwx   0        0        0        0 2023-06-17 13:07:49.376387 webscrapbook-2.0.1/webscrapbook/themes/default/
+drwxrwxrwx   0        0        0        0 2023-06-17 13:07:49.376387 webscrapbook-2.0.1/webscrapbook/themes/default/locales/
+drwxrwxrwx   0        0        0        0 2023-06-17 13:07:49.406494 webscrapbook-2.0.1/webscrapbook/themes/default/locales/ar/
+-rw-rw-rw-   0        0        0       36 2023-05-14 13:37:39.000000 webscrapbook-2.0.1/webscrapbook/themes/default/locales/ar/messages.py
+drwxrwxrwx   0        0        0        0 2023-06-17 13:07:49.406494 webscrapbook-2.0.1/webscrapbook/themes/default/locales/en/
+-rw-rw-rw-   0        0        0     8087 2023-06-17 13:05:10.000000 webscrapbook-2.0.1/webscrapbook/themes/default/locales/en/messages.py
+drwxrwxrwx   0        0        0        0 2023-06-17 13:07:49.406494 webscrapbook-2.0.1/webscrapbook/themes/default/locales/es/
+-rw-rw-rw-   0        0        0     8853 2023-06-04 12:28:32.000000 webscrapbook-2.0.1/webscrapbook/themes/default/locales/es/messages.py
+drwxrwxrwx   0        0        0        0 2023-06-17 13:07:49.406494 webscrapbook-2.0.1/webscrapbook/themes/default/locales/fa/
+-rw-rw-rw-   0        0        0       36 2023-05-14 13:37:39.000000 webscrapbook-2.0.1/webscrapbook/themes/default/locales/fa/messages.py
+drwxrwxrwx   0        0        0        0 2023-06-17 13:07:49.406494 webscrapbook-2.0.1/webscrapbook/themes/default/locales/he/
+-rw-rw-rw-   0        0        0       36 2023-05-14 13:37:39.000000 webscrapbook-2.0.1/webscrapbook/themes/default/locales/he/messages.py
+drwxrwxrwx   0        0        0        0 2023-06-17 13:07:49.416494 webscrapbook-2.0.1/webscrapbook/themes/default/locales/zh/
+-rw-rw-rw-   0        0        0     8240 2023-06-17 13:05:10.000000 webscrapbook-2.0.1/webscrapbook/themes/default/locales/zh/messages.py
+drwxrwxrwx   0        0        0        0 2023-06-17 13:07:49.416494 webscrapbook-2.0.1/webscrapbook/themes/default/locales/zh_cn/
+-rw-rw-rw-   0        0        0     8263 2023-06-17 13:05:10.000000 webscrapbook-2.0.1/webscrapbook/themes/default/locales/zh_cn/messages.py
+drwxrwxrwx   0        0        0        0 2023-06-17 13:07:49.429710 webscrapbook-2.0.1/webscrapbook/themes/default/static/
+-rw-rw-rw-   0        0        0      281 2023-04-08 19:20:00.000000 webscrapbook-2.0.1/webscrapbook/themes/default/static/collapse.png
+-rw-rw-rw-   0        0        0      728 2023-04-08 19:20:00.000000 webscrapbook-2.0.1/webscrapbook/themes/default/static/comment.png
+-rw-rw-rw-   0        0        0      877 2023-05-14 13:37:39.000000 webscrapbook-2.0.1/webscrapbook/themes/default/static/common.css
+-rw-rw-rw-   0        0        0     3900 2023-06-17 13:05:10.000000 webscrapbook-2.0.1/webscrapbook/themes/default/static/common.js
+-rw-rw-rw-   0        0        0     1055 2023-04-08 19:20:00.000000 webscrapbook-2.0.1/webscrapbook/themes/default/static/edit.css
+-rw-rw-rw-   0        0        0     1563 2023-04-08 19:20:00.000000 webscrapbook-2.0.1/webscrapbook/themes/default/static/edit.js
+-rw-rw-rw-   0        0        0     2438 2023-04-08 19:20:00.000000 webscrapbook-2.0.1/webscrapbook/themes/default/static/editx.js
+-rw-rw-rw-   0        0        0      279 2023-04-08 19:20:00.000000 webscrapbook-2.0.1/webscrapbook/themes/default/static/expand.png
+-rw-rw-rw-   0        0        0      523 2023-04-08 19:20:00.000000 webscrapbook-2.0.1/webscrapbook/themes/default/static/external.png
+-rw-rw-rw-   0        0        0      752 2023-04-08 19:20:00.000000 webscrapbook-2.0.1/webscrapbook/themes/default/static/fclose.png
+-rw-rw-rw-   0        0        0      449 2023-04-08 19:20:00.000000 webscrapbook-2.0.1/webscrapbook/themes/default/static/file.png
+-rw-rw-rw-   0        0        0      790 2023-04-08 19:20:00.000000 webscrapbook-2.0.1/webscrapbook/themes/default/static/fopen.png
+-rw-rw-rw-   0        0        0     3810 2023-05-14 13:37:39.000000 webscrapbook-2.0.1/webscrapbook/themes/default/static/index-ex.css
+-rw-rw-rw-   0        0        0    61846 2023-06-17 13:05:10.000000 webscrapbook-2.0.1/webscrapbook/themes/default/static/index-ex.js
+-rw-rw-rw-   0        0        0     2210 2023-05-14 13:37:39.000000 webscrapbook-2.0.1/webscrapbook/themes/default/static/index.css
+-rw-rw-rw-   0        0        0     2156 2023-05-14 13:37:39.000000 webscrapbook-2.0.1/webscrapbook/themes/default/static/index.js
+-rw-rw-rw-   0        0        0      502 2023-04-08 19:20:00.000000 webscrapbook-2.0.1/webscrapbook/themes/default/static/item.png
+-rw-rw-rw-   0        0        0      387 2023-04-08 19:20:00.000000 webscrapbook-2.0.1/webscrapbook/themes/default/static/link.png
+-rw-rw-rw-   0        0        0      445 2023-04-08 19:20:00.000000 webscrapbook-2.0.1/webscrapbook/themes/default/static/note.png
+-rw-rw-rw-   0        0        0      515 2023-04-08 19:20:00.000000 webscrapbook-2.0.1/webscrapbook/themes/default/static/postit.png
+-rw-rw-rw-   0        0        0      661 2023-04-08 19:20:00.000000 webscrapbook-2.0.1/webscrapbook/themes/default/static/search.png
+-rw-rw-rw-   0        0        0      807 2023-04-08 19:20:00.000000 webscrapbook-2.0.1/webscrapbook/themes/default/static/toggle.png
+drwxrwxrwx   0        0        0        0 2023-06-17 13:07:49.436253 webscrapbook-2.0.1/webscrapbook/themes/default/templates/
+-rw-rw-rw-   0        0        0      482 2023-05-14 13:37:39.000000 webscrapbook-2.0.1/webscrapbook/themes/default/templates/base.html
+-rw-rw-rw-   0        0        0      632 2023-05-14 13:37:39.000000 webscrapbook-2.0.1/webscrapbook/themes/default/templates/cli.html
+-rw-rw-rw-   0        0        0     1053 2023-05-14 13:37:39.000000 webscrapbook-2.0.1/webscrapbook/themes/default/templates/edit.html
+-rw-rw-rw-   0        0        0      965 2023-05-14 13:37:39.000000 webscrapbook-2.0.1/webscrapbook/themes/default/templates/editx.html
+-rw-rw-rw-   0        0        0     6130 2023-06-17 13:05:10.000000 webscrapbook-2.0.1/webscrapbook/themes/default/templates/index.html
+-rw-rw-rw-   0        0        0      510 2023-05-14 13:37:39.000000 webscrapbook-2.0.1/webscrapbook/themes/default/templates/maff_index.html
+-rw-rw-rw-   0        0        0      490 2023-05-14 13:37:39.000000 webscrapbook-2.0.1/webscrapbook/themes/default/templates/markdown.html
+-rw-rw-rw-   0        0        0      568 2023-05-14 13:37:39.000000 webscrapbook-2.0.1/webscrapbook/themes/default/templates/static_frame.html
+-rw-rw-rw-   0        0        0     1751 2023-05-14 13:37:39.000000 webscrapbook-2.0.1/webscrapbook/themes/default/templates/static_index.html
+-rw-rw-rw-   0        0        0    12917 2023-05-14 13:37:39.000000 webscrapbook-2.0.1/webscrapbook/themes/default/templates/static_map.html
+-rw-rw-rw-   0        0        0    26414 2023-06-17 13:05:10.000000 webscrapbook-2.0.1/webscrapbook/themes/default/templates/static_search.html
+drwxrwxrwx   0        0        0        0 2023-06-17 13:07:49.436253 webscrapbook-2.0.1/webscrapbook/util/
+-rw-rw-rw-   0        0        0       72 2023-06-04 12:28:32.000000 webscrapbook-2.0.1/webscrapbook/util/__init__.py
+-rw-rw-rw-   0        0        0     5867 2023-05-14 13:37:39.000000 webscrapbook-2.0.1/webscrapbook/util/css.py
+-rw-rw-rw-   0        0        0    44447 2023-06-17 13:05:10.000000 webscrapbook-2.0.1/webscrapbook/util/fs.py
+-rw-rw-rw-   0        0        0    15308 2023-05-14 13:37:39.000000 webscrapbook-2.0.1/webscrapbook/util/html.py
+-rw-rw-rw-   0        0        0    34871 2023-06-17 13:05:10.000000 webscrapbook-2.0.1/webscrapbook/util/util.py
+drwxrwxrwx   0        0        0        0 2023-06-17 13:07:49.386438 webscrapbook-2.0.1/webscrapbook.egg-info/
+-rw-rw-rw-   0        0        0     5609 2023-06-17 13:07:49.000000 webscrapbook-2.0.1/webscrapbook.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3500 2023-06-17 13:07:49.000000 webscrapbook-2.0.1/webscrapbook.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 13:07:49.000000 webscrapbook-2.0.1/webscrapbook.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2023-06-17 13:07:49.000000 webscrapbook-2.0.1/webscrapbook.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      266 2023-06-17 13:07:49.000000 webscrapbook-2.0.1/webscrapbook.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-17 13:07:49.000000 webscrapbook-2.0.1/webscrapbook.egg-info/top_level.txt
```

### Comparing `webscrapbook-2.0.0b9/LICENSE.txt` & `webscrapbook-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b9/PKG-INFO` & `webscrapbook-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscrapbook
-Version: 2.0.0b9
+Version: 2.0.1
 Summary: A backend toolkit for management of WebScrapBook collection.
 Home-page: https://github.com/danny0838/PyWebScrapBook
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

### Comparing `webscrapbook-2.0.0b9/README.md` & `webscrapbook-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b9/setup.cfg` & `webscrapbook-2.0.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -67,91 +67,91 @@
 00000420: 6572 732f 4465 736b 746f 700d 0a09 496e  ers/Desktop...In
 00000430: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
 00000440: 3a3a 2053 6369 656e 6365 2f52 6573 6561  :: Science/Resea
 00000450: 7263 680d 0a0d 0a5b 6f70 7469 6f6e 735d  rch....[options]
 00000460: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
 00000470: 7320 3d20 7e3d 332e 370d 0a69 6e73 7461  s = ~=3.7..insta
 00000480: 6c6c 5f72 6571 7569 7265 7320 3d20 0d0a  ll_requires = ..
-00000490: 0966 6c61 736b 203e 3d20 312e 310d 0a09  .flask >= 1.1...
-000004a0: 7765 726b 7a65 7567 203e 3d20 312e 302e  werkzeug >= 1.0.
-000004b0: 300d 0a09 6a69 6e6a 6132 203e 3d20 322e  0...jinja2 >= 2.
-000004c0: 3130 2e31 0d0a 096c 786d 6c20 3e3d 2034  10.1...lxml >= 4
-000004d0: 2e30 0d0a 0963 6f6d 6d6f 6e6d 6172 6b20  .0...commonmark 
-000004e0: 3e3d 2030 2e38 0d0a 7061 636b 6167 6573  >= 0.8..packages
-000004f0: 203d 2066 696e 643a 0d0a 0d0a 5b6f 7074   = find:....[opt
-00000500: 696f 6e73 2e65 7874 7261 735f 7265 7175  ions.extras_requ
-00000510: 6972 655d 0d0a 6164 686f 635f 7373 6c20  ire]..adhoc_ssl 
-00000520: 3d20 0d0a 0963 7279 7074 6f67 7261 7068  = ...cryptograph
-00000530: 790d 0a64 6576 203d 200d 0a09 666c 616b  y..dev = ...flak
-00000540: 6538 203e 3d20 342e 300d 0a09 7065 7038  e8 >= 4.0...pep8
-00000550: 2d6e 616d 696e 6720 3e3d 2030 2e31 332e  -naming >= 0.13.
-00000560: 320d 0a09 666c 616b 6538 2d63 6f6d 7072  2...flake8-compr
-00000570: 6568 656e 7369 6f6e 7320 3e3d 2033 2e37  ehensions >= 3.7
-00000580: 0d0a 0966 6c61 6b65 382d 7374 7269 6e67  ...flake8-string
-00000590: 2d66 6f72 6d61 7420 3e3d 2030 2e33 0d0a  -format >= 0.3..
-000005a0: 0966 6c61 6b65 382d 7175 6f74 6573 203e  .flake8-quotes >
-000005b0: 3d20 332e 300d 0a09 666c 616b 6538 2d62  = 3.0...flake8-b
-000005c0: 7567 6265 6172 203e 3d20 3232 2e30 0d0a  ugbear >= 22.0..
-000005d0: 0966 6c61 6b65 382d 6973 6f72 7420 3e3d  .flake8-isort >=
-000005e0: 2034 2e32 0d0a 0969 736f 7274 203e 3d20   4.2...isort >= 
-000005f0: 352e 350d 0a09 746f 7820 3e3d 2034 2e30  5.5...tox >= 4.0
-00000600: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
-00000610: 6b61 6765 732e 6669 6e64 5d0d 0a69 6e63  kages.find]..inc
-00000620: 6c75 6465 203d 2077 6562 7363 7261 7062  lude = webscrapb
-00000630: 6f6f 6b2a 0d0a 0d0a 5b6f 7074 696f 6e73  ook*....[options
-00000640: 2e70 6163 6b61 6765 5f64 6174 615d 0d0a  .package_data]..
-00000650: 7765 6273 6372 6170 626f 6f6b 203d 200d  webscrapbook = .
-00000660: 0a09 7265 736f 7572 6365 732f 2a2e 2a0d  ..resources/*.*.
-00000670: 0a09 7468 656d 6573 2f64 6566 6175 6c74  ..themes/default
-00000680: 2f73 7461 7469 632f 2a2e 2a0d 0a09 7468  /static/*.*...th
-00000690: 656d 6573 2f64 6566 6175 6c74 2f74 656d  emes/default/tem
-000006a0: 706c 6174 6573 2f2a 2e2a 0d0a 0974 6865  plates/*.*...the
-000006b0: 6d65 732f 6465 6661 756c 742f 6c6f 6361  mes/default/loca
-000006c0: 6c65 732f 2a2f 2a2e 7079 0d0a 0d0a 5b6f  les/*/*.py....[o
-000006d0: 7074 696f 6e73 2e65 6e74 7279 5f70 6f69  ptions.entry_poi
-000006e0: 6e74 735d 0d0a 636f 6e73 6f6c 655f 7363  nts]..console_sc
-000006f0: 7269 7074 7320 3d20 0d0a 0977 6562 7363  ripts = ...websc
-00000700: 7261 7062 6f6f 6b20 3d20 7765 6273 6372  rapbook = webscr
-00000710: 6170 626f 6f6b 2e63 6c69 3a6d 6169 6e0d  apbook.cli:main.
-00000720: 0a09 7773 6220 3d20 7765 6273 6372 6170  ..wsb = webscrap
-00000730: 626f 6f6b 2e63 6c69 3a6d 6169 6e0d 0a09  book.cli:main...
-00000740: 7773 6276 6965 7720 3d20 7765 6273 6372  wsbview = webscr
-00000750: 6170 626f 6f6b 2e63 6c69 3a76 6965 770d  apbook.cli:view.
-00000760: 0a0d 0a5b 666c 616b 6538 5d0d 0a65 7863  ...[flake8]..exc
-00000770: 6c75 6465 203d 2062 7569 6c64 2c20 2e67  lude = build, .g
-00000780: 6974 0d0a 6d61 782d 6c69 6e65 2d6c 656e  it..max-line-len
-00000790: 6774 6820 3d20 3136 300d 0a69 676e 6f72  gth = 160..ignor
-000007a0: 652d 6e61 6d65 7320 3d20 0d0a 0973 6574  e-names = ...set
-000007b0: 5570 0d0a 0974 6561 7244 6f77 6e0d 0a09  Up...tearDown...
-000007c0: 7365 7455 7043 6c61 7373 0d0a 0974 6561  setUpClass...tea
-000007d0: 7244 6f77 6e43 6c61 7373 0d0a 0973 6574  rDownClass...set
-000007e0: 5570 4d6f 6475 6c65 0d0a 0974 6561 7244  UpModule...tearD
-000007f0: 6f77 6e4d 6f64 756c 650d 0a09 6173 796e  ownModule...asyn
-00000800: 6353 6574 5570 0d0a 0961 7379 6e63 5465  cSetUp...asyncTe
-00000810: 6172 446f 776e 0d0a 0973 6574 5570 5465  arDown...setUpTe
-00000820: 7374 4461 7461 0d0a 0966 6169 6c75 7265  stData...failure
-00000830: 4578 6365 7074 696f 6e0d 0a09 6c6f 6e67  Exception...long
-00000840: 4d65 7373 6167 650d 0a09 6d61 7844 6966  Message...maxDif
-00000850: 660d 0a65 7874 656e 642d 7365 6c65 6374  f..extend-select
-00000860: 203d 200d 0a09 4531 3233 0d0a 6967 6e6f   = ...E123..igno
-00000870: 7265 203d 200d 0a09 5735 3033 0d0a 7065  re = ...W503..pe
-00000880: 722d 6669 6c65 2d69 676e 6f72 6573 203d  r-file-ignores =
-00000890: 200d 0a09 7765 6273 6372 6170 626f 6f6b   ...webscrapbook
-000008a0: 2f5f 706f 6c79 6669 6c6c 2f2a 2a3a 2046  /_polyfill/**: F
-000008b0: 3430 312c 2046 3430 332c 2046 3430 352c  401, F403, F405,
-000008c0: 2051 3030 300d 0a09 7765 6273 6372 6170   Q000...webscrap
-000008d0: 626f 6f6b 2f74 6865 6d65 732f 6465 6661  book/themes/defa
-000008e0: 756c 742f 6c6f 6361 6c65 732f 2a3a 2050  ult/locales/*: P
-000008f0: 3130 332c 2045 3530 310d 0a09 7765 6273  103, E501...webs
-00000900: 6372 6170 626f 6f6b 2f75 7469 6c2f 5f5f  crapbook/util/__
-00000910: 696e 6974 5f5f 2e70 793a 2046 3430 312c  init__.py: F401,
-00000920: 2046 3430 330d 0a09 7465 7374 732f 7465   F403...tests/te
-00000930: 7374 5f63 6c69 2e70 793a 2043 3430 380d  st_cli.py: C408.
-00000940: 0a09 7465 7374 732f 7465 7374 5f6c 6f63  ..tests/test_loc
-00000950: 616c 6573 2f2a 3a20 5031 3033 0d0a 0d0a  ales/*: P103....
-00000960: 5b69 736f 7274 5d0d 0a6d 756c 7469 5f6c  [isort]..multi_l
-00000970: 696e 655f 6f75 7470 7574 203d 2033 0d0a  ine_output = 3..
-00000980: 696e 636c 7564 655f 7472 6169 6c69 6e67  include_trailing
-00000990: 5f63 6f6d 6d61 203d 2074 7275 650d 0a0d  _comma = true...
-000009a0: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
-000009b0: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
-000009c0: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
+00000490: 0966 6c61 736b 203e 3d20 322e 302e 300d  .flask >= 2.0.0.
+000004a0: 0a09 7765 726b 7a65 7567 203e 3d20 322e  ..werkzeug >= 2.
+000004b0: 302e 310d 0a09 6a69 6e6a 6132 203e 3d20  0.1...jinja2 >= 
+000004c0: 322e 3130 2e31 0d0a 096c 786d 6c20 3e3d  2.10.1...lxml >=
+000004d0: 2034 2e30 0d0a 0963 6f6d 6d6f 6e6d 6172   4.0...commonmar
+000004e0: 6b20 3e3d 2030 2e38 0d0a 7061 636b 6167  k >= 0.8..packag
+000004f0: 6573 203d 2066 696e 643a 0d0a 0d0a 5b6f  es = find:....[o
+00000500: 7074 696f 6e73 2e65 7874 7261 735f 7265  ptions.extras_re
+00000510: 7175 6972 655d 0d0a 6164 686f 635f 7373  quire]..adhoc_ss
+00000520: 6c20 3d20 0d0a 0963 7279 7074 6f67 7261  l = ...cryptogra
+00000530: 7068 790d 0a64 6576 203d 200d 0a09 666c  phy..dev = ...fl
+00000540: 616b 6538 203e 3d20 342e 300d 0a09 7065  ake8 >= 4.0...pe
+00000550: 7038 2d6e 616d 696e 6720 3e3d 2030 2e31  p8-naming >= 0.1
+00000560: 332e 320d 0a09 666c 616b 6538 2d63 6f6d  3.2...flake8-com
+00000570: 7072 6568 656e 7369 6f6e 7320 3e3d 2033  prehensions >= 3
+00000580: 2e37 0d0a 0966 6c61 6b65 382d 7374 7269  .7...flake8-stri
+00000590: 6e67 2d66 6f72 6d61 7420 3e3d 2030 2e33  ng-format >= 0.3
+000005a0: 0d0a 0966 6c61 6b65 382d 7175 6f74 6573  ...flake8-quotes
+000005b0: 203e 3d20 332e 300d 0a09 666c 616b 6538   >= 3.0...flake8
+000005c0: 2d62 7567 6265 6172 203e 3d20 3232 2e30  -bugbear >= 22.0
+000005d0: 0d0a 0966 6c61 6b65 382d 6973 6f72 7420  ...flake8-isort 
+000005e0: 3e3d 2034 2e32 0d0a 0969 736f 7274 203e  >= 4.2...isort >
+000005f0: 3d20 352e 350d 0a09 746f 7820 3e3d 2034  = 5.5...tox >= 4
+00000600: 2e30 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  .0....[options.p
+00000610: 6163 6b61 6765 732e 6669 6e64 5d0d 0a69  ackages.find]..i
+00000620: 6e63 6c75 6465 203d 2077 6562 7363 7261  nclude = webscra
+00000630: 7062 6f6f 6b2a 0d0a 0d0a 5b6f 7074 696f  pbook*....[optio
+00000640: 6e73 2e70 6163 6b61 6765 5f64 6174 615d  ns.package_data]
+00000650: 0d0a 7765 6273 6372 6170 626f 6f6b 203d  ..webscrapbook =
+00000660: 200d 0a09 7265 736f 7572 6365 732f 2a2e   ...resources/*.
+00000670: 2a0d 0a09 7468 656d 6573 2f64 6566 6175  *...themes/defau
+00000680: 6c74 2f73 7461 7469 632f 2a2e 2a0d 0a09  lt/static/*.*...
+00000690: 7468 656d 6573 2f64 6566 6175 6c74 2f74  themes/default/t
+000006a0: 656d 706c 6174 6573 2f2a 2e2a 0d0a 0974  emplates/*.*...t
+000006b0: 6865 6d65 732f 6465 6661 756c 742f 6c6f  hemes/default/lo
+000006c0: 6361 6c65 732f 2a2f 2a2e 7079 0d0a 0d0a  cales/*/*.py....
+000006d0: 5b6f 7074 696f 6e73 2e65 6e74 7279 5f70  [options.entry_p
+000006e0: 6f69 6e74 735d 0d0a 636f 6e73 6f6c 655f  oints]..console_
+000006f0: 7363 7269 7074 7320 3d20 0d0a 0977 6562  scripts = ...web
+00000700: 7363 7261 7062 6f6f 6b20 3d20 7765 6273  scrapbook = webs
+00000710: 6372 6170 626f 6f6b 2e63 6c69 3a6d 6169  crapbook.cli:mai
+00000720: 6e0d 0a09 7773 6220 3d20 7765 6273 6372  n...wsb = webscr
+00000730: 6170 626f 6f6b 2e63 6c69 3a6d 6169 6e0d  apbook.cli:main.
+00000740: 0a09 7773 6276 6965 7720 3d20 7765 6273  ..wsbview = webs
+00000750: 6372 6170 626f 6f6b 2e63 6c69 3a76 6965  crapbook.cli:vie
+00000760: 770d 0a0d 0a5b 666c 616b 6538 5d0d 0a65  w....[flake8]..e
+00000770: 7863 6c75 6465 203d 2062 7569 6c64 2c20  xclude = build, 
+00000780: 2e67 6974 0d0a 6d61 782d 6c69 6e65 2d6c  .git..max-line-l
+00000790: 656e 6774 6820 3d20 3136 300d 0a69 676e  ength = 160..ign
+000007a0: 6f72 652d 6e61 6d65 7320 3d20 0d0a 0973  ore-names = ...s
+000007b0: 6574 5570 0d0a 0974 6561 7244 6f77 6e0d  etUp...tearDown.
+000007c0: 0a09 7365 7455 7043 6c61 7373 0d0a 0974  ..setUpClass...t
+000007d0: 6561 7244 6f77 6e43 6c61 7373 0d0a 0973  earDownClass...s
+000007e0: 6574 5570 4d6f 6475 6c65 0d0a 0974 6561  etUpModule...tea
+000007f0: 7244 6f77 6e4d 6f64 756c 650d 0a09 6173  rDownModule...as
+00000800: 796e 6353 6574 5570 0d0a 0961 7379 6e63  yncSetUp...async
+00000810: 5465 6172 446f 776e 0d0a 0973 6574 5570  TearDown...setUp
+00000820: 5465 7374 4461 7461 0d0a 0966 6169 6c75  TestData...failu
+00000830: 7265 4578 6365 7074 696f 6e0d 0a09 6c6f  reException...lo
+00000840: 6e67 4d65 7373 6167 650d 0a09 6d61 7844  ngMessage...maxD
+00000850: 6966 660d 0a65 7874 656e 642d 7365 6c65  iff..extend-sele
+00000860: 6374 203d 200d 0a09 4531 3233 0d0a 6967  ct = ...E123..ig
+00000870: 6e6f 7265 203d 200d 0a09 5735 3033 0d0a  nore = ...W503..
+00000880: 7065 722d 6669 6c65 2d69 676e 6f72 6573  per-file-ignores
+00000890: 203d 200d 0a09 7765 6273 6372 6170 626f   = ...webscrapbo
+000008a0: 6f6b 2f5f 706f 6c79 6669 6c6c 2f2a 2a3a  ok/_polyfill/**:
+000008b0: 2046 3430 312c 2046 3430 332c 2046 3430   F401, F403, F40
+000008c0: 352c 2051 3030 300d 0a09 7765 6273 6372  5, Q000...webscr
+000008d0: 6170 626f 6f6b 2f74 6865 6d65 732f 6465  apbook/themes/de
+000008e0: 6661 756c 742f 6c6f 6361 6c65 732f 2a3a  fault/locales/*:
+000008f0: 2050 3130 332c 2045 3530 310d 0a09 7765   P103, E501...we
+00000900: 6273 6372 6170 626f 6f6b 2f75 7469 6c2f  bscrapbook/util/
+00000910: 5f5f 696e 6974 5f5f 2e70 793a 2046 3430  __init__.py: F40
+00000920: 312c 2046 3430 330d 0a09 7465 7374 732f  1, F403...tests/
+00000930: 7465 7374 5f63 6c69 2e70 793a 2043 3430  test_cli.py: C40
+00000940: 380d 0a09 7465 7374 732f 7465 7374 5f6c  8...tests/test_l
+00000950: 6f63 616c 6573 2f2a 3a20 5031 3033 0d0a  ocales/*: P103..
+00000960: 0d0a 5b69 736f 7274 5d0d 0a6d 756c 7469  ..[isort]..multi
+00000970: 5f6c 696e 655f 6f75 7470 7574 203d 2033  _line_output = 3
+00000980: 0d0a 696e 636c 7564 655f 7472 6169 6c69  ..include_traili
+00000990: 6e67 5f63 6f6d 6d61 203d 2074 7275 650d  ng_comma = true.
+000009a0: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
+000009b0: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
+000009c0: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

### Comparing `webscrapbook-2.0.0b9/webscrapbook/__init__.py` & `webscrapbook-2.0.1/webscrapbook/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import re
 from collections import OrderedDict
 from configparser import ConfigParser
 from copy import deepcopy
 
 __all__ = ['WSB_EXTENSION_MIN_VERSION', 'WSB_USER_DIR', 'WSB_USER_CONFIG', 'WSB_DIR', 'WSB_CONFIG', 'config']
 
-__version__ = '2.0.0b9'
+__version__ = '2.0.1'
 
-WSB_EXTENSION_MIN_VERSION = '2.0.0.9'
+WSB_EXTENSION_MIN_VERSION = '2.0.1'
 WSB_USER_DIR = os.path.join(os.path.expanduser('~'), '.config', 'wsb')  # affected by $HOME
 WSB_USER_CONFIG = os.path.join(os.path.expanduser('~'), '.wsbconfig')  # affected by $HOME
 WSB_DIR = os.environ.get('WSB_DIR') or '.wsb'
 WSB_CONFIG = os.environ.get('WSB_CONFIG') or 'config.ini'
 
 
 class Config():
```

### Comparing `webscrapbook-2.0.0b9/webscrapbook/_polyfill/argparse.py` & `webscrapbook-2.0.1/webscrapbook/_polyfill/argparse.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b9/webscrapbook/_polyfill/mimetypes.py` & `webscrapbook-2.0.1/webscrapbook/_polyfill/mimetypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 _mimetypes.add_type('audio/weba', '.weba')
 _mimetypes.add_type('video/webm', '.webm')
 _mimetypes.add_type('audio/ogg', '.oga')
 _mimetypes.add_type('video/ogg', '.ogv')
 _mimetypes.add_type('application/ogg', '.ogx')  # IANA
 _mimetypes.add_type('application/ogg', '.ogg')  # MAFF
 _mimetypes.add_type('text/vtt', '.vtt')
+_mimetypes.add_type('application/x-shockwave-flash', '.swf')  # Apache, nginx, etc.
 _mimetypes.add_type('application/java-archive', '.jar')
 _mimetypes.add_type('application/java-vm', '.class')
 _mimetypes.add_type('application/epub+zip', '.epub')
 _mimetypes.add_type('application/x-7z-compressed', '.7z')
 _mimetypes.add_type('application/vnd.rar', '.rar')
 
 # .js is mapped to application/x-javascript in some mime types sources
```

### Comparing `webscrapbook-2.0.0b9/webscrapbook/app.py` & `webscrapbook-2.0.1/webscrapbook/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """The WGSI application.
 """
 import functools
+import hashlib
 import json
 import os
 import time
 import traceback
 import types
-from collections import namedtuple
+from collections import defaultdict, namedtuple
 from contextlib import nullcontext
 from secrets import token_urlsafe
 from urllib.parse import quote, unquote, urljoin, urlsplit, urlunsplit
 from zlib import adler32
 
 import commonmark
 import flask
@@ -29,14 +30,15 @@
     dump_options_header,
     http_date,
     is_resource_modified,
     parse_options_header,
 )
 from werkzeug.local import LocalProxy
 from werkzeug.middleware.proxy_fix import ProxyFix
+from werkzeug.security import check_password_hash
 from werkzeug.utils import cached_property
 
 from . import WSB_CONFIG, WSB_DIR, WSB_EXTENSION_MIN_VERSION, __version__, util
 from ._polyfill import mimetypes, zipfile
 from .scrapbook import cache as wsb_cache
 from .scrapbook import check as wsb_check
 from .scrapbook import exporter as wsb_exporter
@@ -51,14 +53,21 @@
     ZIP_SUBPATH_FILE,
 )
 
 # see: https://url.spec.whatwg.org/#percent-encoded-bytes
 quote_path = functools.partial(quote, safe=":/[]@!$&'()*+,;=")
 quote_path.__doc__ = 'Escape reserved chars for the path part of a URL.'
 
+jsonify = functools.partial(
+    json.dumps,
+    ensure_ascii=False,
+    check_circular=False,
+    separators=(',', ':'),
+)
+
 bp = flask.Blueprint('default', __name__)
 host = LocalProxy(lambda: current_app.config['WEBSCRAPBOOK_HOST'])
 
 
 def static_url(path):
     return f'{quote_path(request.script_root)}/{quote_path(path)}?a=static'
 
@@ -133,15 +142,15 @@
 def generate_server_sent_events(gen):
     try:
         for data in gen:
             yield 'data: ' + data + '\n\n'
     except Exception:
         traceback.print_exc()
         err = {'type': 'critical', 'msg': 'Internal Server Error'}
-        yield 'data: ' + json.dumps(err, ensure_ascii=False) + '\n\n'
+        yield 'data: ' + jsonify(err) + '\n\n'
 
     yield 'event: complete' + '\n'
     yield 'data: ' + '\n\n'
 
 
 def http_response(body=None, status=None, headers=None, format=None):
     """Handle formatted response.
@@ -157,17 +166,15 @@
     elif format == 'json':
         mimetype = 'application/json'
 
         if status == 204:
             status = None
             body = None
 
-        body = json.dumps({
-            'data': body,
-        }, ensure_ascii=False)
+        body = jsonify({'data': body})
 
     # expect body to be a generator of text (mostly JSON) data
     elif format == 'sse':
         mimetype = 'text/event-stream'
 
         if status == 204:
             status = None
@@ -233,57 +240,14 @@
     """Determine if the client is in same device.
     """
     server_host = request.host.partition(':')[0]
     client_host = request.remote_addr
     return util.is_localhost(server_host) or util.is_localhost(client_host) or server_host == client_host
 
 
-def get_permission(auth_info, auth_config):
-    """Calculate effective permission from provided auth info and config.
-    """
-    auth = auth_info or {}
-    user = auth.get('username') or ''
-    pw = auth.get('password') or ''
-
-    for _, entry in auth_config.items():
-        entry_user = entry.get('user', '')
-        if user != entry_user:
-            continue
-
-        entry_pw = entry.get('pw', '')
-        entry_pw_salt = entry.get('pw_salt', '')
-        entry_pw_type = entry.get('pw_type', '')
-        if util.encrypt(pw, entry_pw_salt, entry_pw_type) != entry_pw:
-            continue
-
-        entry_permission = entry.get('permission', 'all')
-        return entry_permission
-
-    return ''
-
-
-def verify_authorization(perm, action):
-    """Check if authorized or not.
-    """
-    if perm == 'all':
-        return True
-
-    if perm == 'read':
-        return action not in {
-            'token', 'lock', 'unlock',
-            'mkdir', 'mkzip', 'save', 'delete', 'move', 'copy',
-            'backup', 'unbackup', 'cache', 'check', 'export', 'import', 'query',
-        }
-
-    if perm == 'view':
-        return action in {'view', 'info', 'source', 'download', 'static', 'unknown'}
-
-    return False
-
-
 def handle_directory_listing(localpaths, zh=None, redirect_slash=True, format=None):
     """List contents in a directory.
 
     Args:
         localpaths: a CPath
         zh: an opened zipfile.ZipFile object for faster reading
     """
@@ -332,15 +296,15 @@
 
         subentries = listdir(localpaths[0])
 
     if format == 'sse':
         def gen():
             for entry in subentries:
                 data = entry._asdict()
-                yield json.dumps(data, ensure_ascii=False)
+                yield jsonify(data)
 
         return http_response(gen(), headers=headers, format=format)
 
     if format == 'json':
         data = [e._asdict() for e in subentries]
         return http_response(data, headers=headers, format=format)
 
@@ -731,24 +695,26 @@
                 filename = os.path.basename(request.localrealpath)
                 response = zip_static_file(zh, localpaths[-1], mimetype=request.localmimetype)
             else:
                 abort(404)
 
         if not response:
             def gen():
+                zs = util.fs.ZipStream()
                 with util.fs.open_archive_path(localpaths) as zh:
-                    yield from util.fs.zip_copy(zh, localpaths[-1], None, '', filter)
+                    yield from util.fs.zip_copy(zh, localpaths[-1], zs, '', filter, stream=zs)
 
             response = Response(gen(), mimetype=mimetype)
             response.headers.set('Cache-Control', 'no-store')
     else:
         if os.path.isdir(localpaths[0]):
             filename = os.path.basename(request.localrealpath) + '.zip'
             mimetype, _ = mimetypes.guess_type(filename)
-            gen = util.fs.zip_compress(None, localpaths[0], '', filter)
+            zs = util.fs.ZipStream()
+            gen = util.fs.zip_compress(zs, localpaths[0], '', filter, stream=zs)
             response = Response(gen, mimetype=mimetype)
             response.headers.set('Cache-Control', 'no-store')
         else:
             filename = os.path.basename(request.localrealpath)
             response = static_file(localpaths[0])
 
     filename = quote_path(filename)
@@ -1245,18 +1211,18 @@
         static_index=request.values.get('static_index', default=None, type=bool),
         rss=request.values.get('rss', default=None, type=bool),
     )
 
     if format == 'sse':
         def wrapper():
             for info in gen:
-                yield json.dumps({
+                yield jsonify({
                     'type': info.type,
                     'msg': info.msg,
-                }, ensure_ascii=False)
+                })
 
         return http_response(wrapper(), format=format)
 
     elif format:
         for info in gen:
             if info.type == 'critical':
                 abort(500, info.msg)
@@ -1294,18 +1260,18 @@
         resolve_absolute_icon=request.values.get('resolve_absolute_icon', default=False, type=bool),
         resolve_unused_icon=request.values.get('resolve_unused_icon', default=False, type=bool),
     )
 
     if format == 'sse':
         def wrapper():
             for info in gen:
-                yield json.dumps({
+                yield jsonify({
                     'type': info.type,
                     'msg': info.msg,
-                }, ensure_ascii=False)
+                })
 
         return http_response(wrapper(), format=format)
 
     elif format:
         for info in gen:
             if info.type == 'critical':
                 abort(500, info.msg)
@@ -1319,87 +1285,91 @@
 
     return Response(stream)
 
 
 @handle_action_advanced
 @handle_action_token
 def action_export():
-    """Invoke the exporter."""
+    """Export items as an archive file."""
     format = request.format
 
     if format:
         abort(400, 'Action not supported.')
 
     book_id = request.values.get('book', default='')
-    export_dir = os.path.join(host.books[book_id].tree_dir, 'exports')
-    if os.path.lexists(export_dir):
-        util.fs.delete(export_dir)
+
+    zs = util.fs.ZipStream()
     gen = wsb_exporter.run(
-        (host.root, host.config), export_dir,
+        (host.root, host.config), zs,
         book_id=book_id,
-        items=request.values.get('items', type=json.loads),
+        items=request.values.get('items', default=(), type=json.loads),
         scheme=wsb_exporter.SCHEME_ROOT_INDEXES,
         recursive=request.values.get('recursive', default=False, type=bool),
         singleton=request.values.get('singleton', default=False, type=bool),
         lock=request.values.get('lock', default=True),
+        stream=zs,
     )
 
     def wrapper():
         for info in gen:
             if info.type == 'critical':
                 abort(500, info.msg)
-        yield from util.fs.zip_compress(None, export_dir, '')
-        if os.path.lexists(export_dir):
-            util.fs.delete(export_dir)
+            if isinstance(info.data, bytes):
+                yield info.data
 
-    filename = 'exports.zip'
+    filename = 'exports.wsba'
     mimetype, _ = mimetypes.guess_type(filename)
     filename = quote_path(filename)
     response = Response(wrapper(), mimetype=mimetype)
     response.headers.set('Content-Disposition',
                          f'''attachment; filename*=UTF-8''{filename}; filename="{filename}"''')
     return response
 
 
 @handle_action_advanced
 @handle_action_token
 def action_import():
-    """Invoke the importer."""
+    """Import items from the archive files in the "exports" directory."""
     format = request.format
 
     book_id = request.values.get('book', default='')
     target_id = request.values.get('target')
     target_index = request.values.get('index', type=int)
     rebuild_folders = request.values.get('rebuild', default=False, type=bool)
     resolve_id_used = request.values.get('resolve', default='new')
     lock = request.values.get('lock', default=True)
 
     export_dir = os.path.join(host.books[book_id].tree_dir, 'exports')
     os.makedirs(export_dir, exist_ok=True)
+    with os.scandir(export_dir) as it:
+        files = sorted(f.path for f in it)
+
     _gen = wsb_importer.run(
-        (host.root, host.config), [export_dir],
+        (host.root, host.config), files,
         book_id=book_id,
         target_id=target_id,
         target_index=target_index,
         rebuild_folders=rebuild_folders,
         resolve_id_used=resolve_id_used,
         lock=lock,
     )
 
     def gen():
-        yield from _gen
-        util.fs.delete(export_dir)
+        try:
+            yield from _gen
+        finally:
+            util.fs.delete(export_dir)
 
     if format == 'sse':
         def wrapper():
             for info in gen():
-                yield json.dumps({
+                yield jsonify({
                     'type': info.type,
                     'msg': info.msg,
-                }, ensure_ascii=False)
+                })
 
         return http_response(wrapper(), format=format)
 
     elif format:
         for info in gen():
             if info.type == 'critical':
                 abort(500, info.msg)
@@ -1435,58 +1405,70 @@
 
 
 @handle_action_advanced
 def action_search():
     """Search in scrapbooks."""
     format = request.format
 
-    if format != 'json':
-        abort(400, 'Action not supported.')
-
     gen = wsb_search.search(
         (host.root, host.config),
         query=request.values.get('q', default=''),
         context={
             'title': -1,
             'file': -1,
             'comment': request.values.get('comment', default=None, type=int),
             'source': request.values.get('source', default=None, type=int),
             'fulltext': request.values.get('fulltext', default=None, type=int),
         },
         lock=request.values.get('lock', default=True),
     )
 
-    data = {}
-    try:
-        for item in gen:
-            data.setdefault(item.book_id, []).append({
-                'id': item.id,
-                'file': item.file,
-                'context': item.context,
-            })
-    except wsb_search.QueryError as exc:
-        abort(400, str(exc))
+    if format == 'json':
+        data = defaultdict(list)
+        try:
+            for item in gen:
+                data[item.book_id].append({
+                    'id': item.id,
+                    'file': item.file,
+                    'context': item.context,
+                })
+        except wsb_search.QueryError as exc:
+            abort(400, str(exc))
 
-    return http_response(data, format=format)
+        return http_response(data, format=format)
+
+    elif format == 'sse':
+        def wrapper():
+            try:
+                for item in gen:
+                    yield jsonify({
+                        'type': 'info',
+                        'msg': '',
+                        'data': {
+                            'book_id': item.book_id,
+                            'id': item.id,
+                            'file': item.file,
+                            'context': item.context,
+                        },
+                    })
+            except wsb_search.QueryError as exc:
+                yield jsonify({
+                    'type': 'critical',
+                    'msg': str(exc),
+                })
+
+        return http_response(wrapper(), format=format)
+
+    else:
+        abort(400, 'Action not supported.')
 
 
 @bp.before_request
 def handle_before_request():
-    # handle authorization
-    try:
-        auth_config = host.config['auth']
-    except KeyError:
-        # auth not required
-        return
-
-    perm = get_permission(request.authorization, auth_config)
-    if not verify_authorization(perm, request.action):
-        auth = WWWAuthenticate()
-        auth.set_basic(host.config['app']['name'])
-        abort(401, 'You are not authorized.', www_authenticate=auth)
+    host.verify_authorization()
 
 
 @bp.route('/', methods=['GET', 'HEAD', 'POST'])
 @bp.route('/<path:filepath>', methods=['GET', 'HEAD', 'POST'])
 def handle_request(filepath=''):
     """Handle an HTTP request (HEAD, GET, POST).
     """
@@ -1510,27 +1492,37 @@
 
 @bp.errorhandler(HTTPException)
 def handle_error(exc):
     """Handle formatted error if requested by client.
     """
     if request.format == 'json':
         response = exc.get_response()
-        response.data = json.dumps({
+        response.data = jsonify({
             'error': {
                 'status': exc.code,
                 'message': exc.description,
             },
-        }, ensure_ascii=False)
+        })
         response.content_type = 'application/json'
         return response
 
     if request.format == 'sse':
+        _code = exc.code
+
+        # use 200 for common errors for the client API to parse the content
+        if exc.code in (400, 403, 404, 500):
+            exc.code = 200
+
         response = exc.get_response()
         response.data = ''.join(generate_server_sent_events((
-            json.dumps({'type': 'critical', 'msg': exc.description}, ensure_ascii=False),
+            jsonify({
+                'type': 'critical',
+                'msg': exc.description,
+                'data': {'status': _code},
+            }),
         )))
         response.content_type = 'text/event-stream'
         return response
 
     return exc
 
 
@@ -1545,14 +1537,17 @@
     def __init__(self, root, config=None):
         super().__init__(root, config=config)
 
         # token handling
         self.tokens = os.path.join(self.root, WSB_DIR, 'server', 'tokens')
         self.token_last_purge = 0
 
+        # cache
+        self._get_permission_cache = {}
+
     def token_acquire(self, now=None):
         if now is None:
             now = int(time.time())
 
         self.token_check_delete_expire(now)
 
         token = token_urlsafe()
@@ -1615,14 +1610,91 @@
         if now is None:
             now = int(time.time())
 
         if now >= self.token_last_purge + self.TOKEN_PURGE_INTERVAL:
             self.token_last_purge = now
             self.token_delete_expire(now)
 
+    def verify_authorization(self):
+        """Verify that the current request is adequately authorized.
+
+        - Must run in a request context.
+        - Abort the request if not authorized.
+        """
+        if 'auth' not in self.config:
+            return
+
+        auth = request.authorization or {}
+        username = auth.get('username') or ''
+        password = auth.get('password') or ''
+        perm = self.get_permission(username, password)
+        if not self.check_permission(perm, request.action):
+            auth = WWWAuthenticate('basic', {'realm': self.config['app']['name']})
+            abort(401, 'You are not authorized.', www_authenticate=auth)
+
+    def get_permission(self, username, password):
+        """Calculate effective permission from provided auth info.
+
+        - A valid username-password combinations will be cached (in hashed
+          form) in the memory to prevent a slow down due to repeated slow
+          hash checking.
+        """
+        # return cached value if exists
+        try:
+            return self._get_permission_cache[
+                self._get_permission_hash(username, password)
+            ]
+        except KeyError:
+            pass
+
+        for _, entry in self.config['auth'].items():
+            entry_user = entry.get('user', '')
+            if username != entry_user:
+                continue
+
+            entry_pw = entry.get('pw', '')
+            if entry_pw:
+                if not check_password_hash(entry_pw, password):
+                    continue
+            else:
+                if password != entry_pw:
+                    continue
+
+            entry_permission = entry.get('permission', 'all')
+
+            # cach a successful match
+            self._get_permission_cache[
+                self._get_permission_hash(username, password)
+            ] = entry_permission
+
+            return entry_permission
+
+        return ''
+
+    def _get_permission_hash(self, username, password):
+        return hashlib.sha512(f'{username}\0{password}'.encode('UTF-8')).digest()
+
+    @staticmethod
+    def check_permission(perm, action):
+        """Check authorization for the provided perm and action."""
+        if perm == 'all':
+            return True
+
+        if perm == 'read':
+            return action not in {
+                'token', 'lock', 'unlock',
+                'mkdir', 'mkzip', 'save', 'delete', 'move', 'copy',
+                'backup', 'unbackup', 'cache', 'check', 'export', 'import', 'query',
+            }
+
+        if perm == 'view':
+            return action in {'view', 'info', 'source', 'download', 'static', 'unknown'}
+
+        return False
+
 
 def make_app(root='.', config=None):
     _host = WebHost(root, config=config)
 
     # main app instance
     app = flask.Flask(__name__, instance_path=_host.chroot)
     app.register_blueprint(bp)
```

### Comparing `webscrapbook-2.0.0b9/webscrapbook/cli.py` & `webscrapbook-2.0.1/webscrapbook/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,25 +137,33 @@
 
 
 def cmd_encrypt(args):
     """Generate an encrypted password string.
 
     Primilarly to be used in auth config.
     """
+    kwargs = {}
+
     pw = args['password']
     if pw is None:
-        pw1 = getpass('Enter a password: ')
+        pw = getpass('Enter a password: ')
         pw2 = getpass('Confirm the password: ')
-
-        if pw1 != pw2:
+        if pw != pw2:
             die('Entered passwords do not match.')
+    kwargs['password'] = pw
+
+    if args['method'] is not None:
+        kwargs['method'] = args['method']
 
-        pw = pw1
+    if args['salt'] is not None:
+        kwargs['salt_length'] = args['salt']
 
-    print(util.encrypt(pw, salt=args['salt'], method=args['method']))
+    from werkzeug.security import generate_password_hash
+    result = generate_password_hash(**kwargs)
+    print(result)
 
 
 def cmd_cache(args):
     """Generate (or update) fulltext cache and/or static site pages."""
     kwargs = args.copy()
     root = kwargs.pop('root')
     debug = kwargs.pop('debug')
@@ -173,41 +181,51 @@
     from .scrapbook import cache
     for info in cache.generate(root, book_items, **kwargs):
         if info.type != 'debug' or debug:
             log(f'{info.type.upper()}: {info.msg}')
 
 
 def cmd_export(args):
-    """Export data items into archive files (*.wsba).
+    """Export data items into an archive file (*.wsba).
 
     The export/import utilities provide a basic way to backup and restore the
     data and metadata (i.e. item properties) of specific item(s). To
     reconstruct the original scrapbook tree the exported archive files should
-    be re-imported together using the original Unicode filename order.
+    be re-imported together using the original order.
 
     For a reliable way to backup and restore the scrapbook tree as well as the
     items, it's generally more recommended to create another scrapbook and copy
     items between them.
     """
     kwargs = args.copy()
     root = kwargs.pop('root')
     debug = kwargs.pop('debug')
 
+    if kwargs['output'] is None:
+        kwargs['output'] = sys.stdout.buffer
+
     from .scrapbook import exporter
     for info in exporter.run(root, **kwargs):
         if info.type != 'debug' or debug:
             log(f'{info.type.upper()}: {info.msg}')
 
 
 def cmd_import(args):
     """Import data items from archive files (*.wsba).
 
     To faithfully reconstruct the original scrapbook tree, the archive files
     should be imported together using the same Unicode filename order as how
     they have been exported.
+
+    To faithfully restore the timestamps for the imported files, the system
+    timezone should be configured to be identical to the original timezone
+    (i.e. the one where the archive has been generated in), as the ZIP archive
+    does not record timezone information for the internal files. The 'timezone'
+    property of the internal 'export.json' in the archive file can be consulted
+    to infer the original timezone.
     """
     kwargs = args.copy()
     root = kwargs.pop('root')
     debug = kwargs.pop('debug')
 
     from .scrapbook import importer
     for info in importer.run(root, **kwargs):
@@ -558,21 +576,20 @@
         description=getdoc(cmd_encrypt),
         help="""generate an encrypted password""")
     parser_encrypt.set_defaults(func=cmd_encrypt)
     parser_encrypt.add_argument(
         '-p', '--password', nargs='?', default=None, action='store',
         help="""the password to encrypt. Skip to provide via an interactive prompt.""")
     parser_encrypt.add_argument(
-        '-m', '--method', default='sha1', action='store',
-        help="""the encrypt method to use, which is one of: plain, md5, sha1,
-sha224, sha256, sha384, sha512, sha3_224, sha3_256, sha3_384, and sha3_512
-(default: %(default)s)""")
+        '-m', '--method', default='pbkdf2', action='store',
+        help="""the encrypt method to use, such as 'pbkdf2:sha256:600000', 'scrypt:32768:8:1',
+etc. (default: %(default)r)""")
     parser_encrypt.add_argument(
-        '-s', '--salt', default='', action='store',
-        help="""the salt to add during encryption""")
+        '-s', '--salt', default=32, action='store', type=int,
+        help="""the length of the salt for encryption (default: %(default)r)""")
 
     # subcommand: cache
     parser_cache = subparsers.add_parser(
         'cache', aliases=['a'],
         formatter_class=argparse.RawDescriptionHelpFormatter,
         description=getdoc(cmd_cache),
         help="""update fulltext cache and/or static site pages""")
@@ -669,16 +686,16 @@
     parser_export = subparsers.add_parser(
         'export', aliases=['x'],
         formatter_class=argparse.RawDescriptionHelpFormatter,
         description=getdoc(cmd_export),
         help="""export data items into archive files (*.wsba)""")
     parser_export.set_defaults(func=cmd_export)
     parser_export.add_argument(
-        'output', action='store',
-        help="""the output directory""")
+        'output', action='store', default=None, nargs='?',
+        help="""the output file (default: stdout)""")
     parser_export.add_argument(
         '--book', dest='book_id', metavar='ID', default='', action='store',
         help="""the book ID to export (default: "")""")
     parser_export.add_argument(
         '--item', dest='items',
         metavar='ID', action='store', default=None, nargs='+',
         help="""the items ID(s) to export (default: all)""")
@@ -728,16 +745,15 @@
 
 All SUBPATTERNs can be prepended with "UTC_" for UTC time instead of local
 time. For example, "%CREATE:UTC_DATE%".
 """)
     parser_import.set_defaults(func=cmd_import)
     parser_import.add_argument(
         'files', metavar='file', action='store', nargs='+',
-        help="""the file(s) to import in order. If a directory is provided, all
-child files are imported in unicode filename order.""")
+        help="""the file(s) to import in order.""")
     parser_import.add_argument(
         '--book', dest='book_id', metavar='ID', default='', action='store',
         help="""the book ID to import into (default: "")""")
     parser_import.add_argument(
         '--target', dest='target_id', metavar='ID',
         default='root', action='store',
         help="""the target item ID to insert the imported items under (default: "%(default)s")""")
```

### Comparing `webscrapbook-2.0.0b9/webscrapbook/locales.py` & `webscrapbook-2.0.1/webscrapbook/locales.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b9/webscrapbook/resources/config.ini` & `webscrapbook-2.0.1/webscrapbook/resources/config.ini`

 * *Files 20% similar despite different names*

```diff
@@ -25,24 +25,20 @@
 inclusive_frames = true
 static_index = false
 rss_root = 
 rss_item_count = 50
 
 ; [auth "user1"]
 ; user = myuser1
-; pw = 73337dfdaf99b87be97cb4b4f16645e059da6e5f
-; pw_salt = mysalt1
-; pw_type = sha1
+; pw = pbkdf2:sha256:1000$jlbk3RVDGdR6TVDvRAie3HPSMejGTedw$2f3935a508c20c63c5bcdf7d96d853fc1df7d6dcab824e43a2aa2570bfcd0bef
 ; permission = all
 
 ; [auth "user2"]
 ; user = myuser2
-; pw = pass2mysalt2
-; pw_salt = mysalt2
-; pw_type = plain
+; pw =
 ; permission = read
 
 [server]
 ; port = 8080
 ; host = localhost
 ; ssl_on = true
 ; ssl_key = ./wsb/webscrapbook.key
```

### Comparing `webscrapbook-2.0.0b9/webscrapbook/resources/config.md` & `webscrapbook-2.0.1/webscrapbook/resources/config.md`

 * *Files 3% similar despite different names*

```diff
@@ -289,59 +289,43 @@
 
 The `[auth]` section(s) define authorization rules. It can be subsected as
 `[auth "identifier"]` (with an identifier being alphanumeric and starts with an
 alphabet). Authorization requirement is activated when at least one `[auth]`
 section exists. Each section defines a rule, and the user must fullfill at
 least one to be allowed to access.
 
-An encrypted password can be generated via the `encrypt` sub-command, For
+An encrypted password can be generated with the `encrypt` sub-command. For
 example:
 
-    webscrapbook encrypt -m sha1 -s mysalt
+    webscrapbook encrypt -m pbkdf2:sha256:600000 -s 32
 
-You'll then be promopted to input a password, and then you can use the output
-for `pw`, "mysalt" for `pw_salt`, and "sha1" for `pw_type`.
+You'll then be prompted to input a password, and the output can be used as the
+value of `pw`.
 
 To specify permission for an anonymous user, create an `[auth]` section with
-empty user and a password matching an empty string (e.g. "plain" `pw_type`,
-empty `pw`, and empty `pw_salt`.)
+empty user and password.
 
 NOTE: Use HTTPS protocol as possible when password authorization is activated,
 as input user name and password are unencrypted during HTTP transmission.
 
 
 #### `user`
 
 The user's name.
 
 (default: )
 
 
 #### `pw`
 
-The user's password, in encrypted form.
+The user's password in hashed form, or empty for no password.
 
 (default: )
 
 
-#### `pw_salt`
-
-A "salt" string which is added during encryption for better security.
-
-(default: )
-
-
-#### `pw_type`
-
-The encryption method for password. Supported methods are: plain, md5, sha1,
-sha224, sha256, sha384, sha512, sha3_224, sha3_256, sha3_384, and sha3_512.
-
-(default: `sha1`)
-
-
 #### `permission`
 
 The permission for those who fullfills this authorization condition.
 * `all`: unrestricted access.
 * `read`: read-only. APIs for data modification are disabled. Note that
   essential server information is still exposed. Recommended for read-only
   WebScrapBook browser extension access.
```

### Comparing `webscrapbook-2.0.0b9/webscrapbook/resources/mimetypes.md` & `webscrapbook-2.0.1/webscrapbook/resources/mimetypes.md`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b9/webscrapbook/resources/themes.md` & `webscrapbook-2.0.1/webscrapbook/resources/themes.md`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b9/webscrapbook/scrapbook/book.py` & `webscrapbook-2.0.1/webscrapbook/scrapbook/book.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Scrapbook book handler.
 """
 import functools
 import glob
+import hashlib
 import html
 import json
 import os
 import re
 from datetime import datetime, timedelta, timezone
 from urllib.parse import unquote, urlsplit
 from urllib.request import pathname2url
@@ -146,14 +147,27 @@
         self.toc = None
         self.fulltext = None
 
     def __repr__(self):
         repr_str = ', '.join(f'{attr}={repr(getattr(self, attr))}' for attr in self.REPR_ATTRS)
         return f'{self.__class__.__name__}({repr_str})'
 
+    @staticmethod
+    def checksum(obj, method='sha1'):
+        """Get a checksum of an object (by its JSONified string)."""
+        m = hashlib.new(method)
+        gen = json.JSONEncoder(
+            ensure_ascii=False,
+            check_circular=False,
+            separators=(',', ':'),
+        ).iterencode(obj)
+        for chunk in gen:
+            m.update(chunk.encode('UTF-8'))
+        return m.digest()
+
     def get_subpath(self, file):
         """Get subpath of a file related to root.
         """
         return self.host.get_subpath(file)
 
     def get_tree_file(self, name, index=0):
         return os.path.join(self.tree_dir, f'{name}{index or ""}.js')
@@ -205,15 +219,15 @@
     def load_tree_files(self, name):
         data = {}
         for file in self.iter_tree_files(name):
             data.update(self.load_tree_file(file))
 
         # remove top-level None values to allow quick clear by appending file
         # e.g. add meta1.js with {'id1': None} to quickly delete 'id1' in meta.js
-        for k in list(data):
+        for k in tuple(data):
             if data[k] is None:
                 del data[k]
 
         return data
 
     def load_meta_files(self, refresh=False):
         if refresh or self.meta is None:
@@ -223,131 +237,147 @@
         if refresh or self.toc is None:
             self.toc = self.load_tree_files('toc')
 
     def load_fulltext_files(self, refresh=False):
         if refresh or self.fulltext is None:
             self.fulltext = self.load_tree_files('fulltext')
 
-    def save_tree_file(self, name, index, data):
+    def save_tree_file(self, name, index, gen):
         """Save a tree file.
 
         Raises:
             OSError: failed to write
         """
         file = self.get_tree_file(name, index)
         self.backup(file)
         with open(file, 'w', encoding='UTF-8', newline='\n') as fh:
-            fh.write(data)
+            for chunk in gen:
+                fh.write(chunk.translate(self.JSON_TRANSLATER))
 
-    def save_meta_file(self, i, data):
-        self.save_tree_file('meta', i, f"""/**
- * Feel free to edit this file, but keep data code valid JSON format.
- */
-scrapbook.meta({json.dumps(data, ensure_ascii=False, indent=2).translate(self.JSON_TRANSLATER)})""")
+    def _gen_meta_file(self, data):
+        yield '/* Feel free to edit this file, but keep data code valid JSON format. */\n'
+        yield 'scrapbook.meta('
+        yield from json.JSONEncoder(
+            ensure_ascii=False,
+            check_circular=False,
+            indent=2,
+        ).iterencode(data)
+        yield ')'
 
     def save_meta_files(self):
         """Save to tree/meta#.js
         """
         os.makedirs(os.path.join(self.tree_dir), exist_ok=True)
         i = 0
         size = 1
         meta = {}
-        for id in list(self.meta):
+        for id in tuple(self.meta):
             if self.meta[id] is None:
                 del self.meta[id]
                 continue
             meta[id] = self.meta[id]
             size += 1
             if size >= self.SAVE_META_THRESHOLD:
-                self.save_meta_file(i, meta)
+                self.save_tree_file('meta', i, self._gen_meta_file(meta))
                 i += 1
                 size = 0
                 meta = {}
 
         if size:
-            self.save_meta_file(i, meta)
+            self.save_tree_file('meta', i, self._gen_meta_file(meta))
             i += 1
 
         # remove unused tree/meta#.js
         while True:
             file = self.get_tree_file('meta', i)
             try:
                 self.backup(file)
                 os.remove(file)
             except FileNotFoundError:
                 break
             i += 1
 
-    def save_toc_file(self, i, data):
-        self.save_tree_file('toc', i, f"""/**
- * Feel free to edit this file, but keep data code valid JSON format.
- */
-scrapbook.toc({json.dumps(data, ensure_ascii=False, indent=2).translate(self.JSON_TRANSLATER)})""")
+    def _gen_toc_file(self, data):
+        yield '/* Feel free to edit this file, but keep data code valid JSON format. */\n'
+        yield 'scrapbook.toc('
+        yield from json.JSONEncoder(
+            ensure_ascii=False,
+            check_circular=False,
+            indent=2,
+        ).iterencode(data)
+        yield ')'
 
     def save_toc_files(self):
         """Save to tree/toc#.js
         """
         os.makedirs(os.path.join(self.tree_dir), exist_ok=True)
         i = 0
         size = 1
         toc = {}
-        for id in list(self.toc):
+        for id in tuple(self.toc):
             if self.toc[id] is None:
                 del self.toc[id]
                 continue
             toc[id] = self.toc[id]
             size += 1 + len(toc[id])
             if size >= self.SAVE_TOC_THRESHOLD:
-                self.save_toc_file(i, toc)
+                self.save_tree_file('toc', i, self._gen_toc_file(toc))
                 i += 1
                 size = 0
                 toc = {}
 
         if size:
-            self.save_toc_file(i, toc)
+            self.save_tree_file('toc', i, self._gen_toc_file(toc))
             i += 1
 
         # remove unused tree/toc#.js
         while True:
             file = self.get_tree_file('toc', i)
             try:
                 self.backup(file)
                 os.remove(file)
             except FileNotFoundError:
                 break
             i += 1
 
+    def _gen_fulltext_file(self, data):
+        yield '/* This file is generated by WebScrapBook and is not intended to be edited. */\n'
+        yield 'scrapbook.fulltext('
+        yield from json.JSONEncoder(
+            ensure_ascii=False,
+            check_circular=False,
+            indent=1,
+        ).iterencode(data)
+        yield ')'
+
     def save_fulltext_file(self, i, data):
-        self.save_tree_file('fulltext', i, f"""/**
- * This file is generated by WebScrapBook and is not intended to be edited.
- */
-scrapbook.fulltext({json.dumps(data, ensure_ascii=False, indent=1).translate(self.JSON_TRANSLATER)})""")
+        self.save_tree_file('fulltext', i, self._gen_fulltext_file(data))
 
     def save_fulltext_files(self):
         """Save to tree/fulltext#.js
         """
         os.makedirs(os.path.join(self.tree_dir), exist_ok=True)
         i = 0
         size = 1
         fulltext = {}
-        for id in list(self.fulltext):
+        for id in tuple(self.fulltext):
             if self.fulltext[id] is None:
                 del self.fulltext[id]
                 continue
             fulltext[id] = self.fulltext[id]
             for path in fulltext[id]:
                 size += len(fulltext[id][path]['content'])
             if size >= self.SAVE_FULLTEXT_THRESHOLD:
-                self.save_fulltext_file(i, fulltext)
+                self.save_tree_file('fulltext', i, self._gen_fulltext_file(fulltext))
                 i += 1
                 size = 0
                 fulltext = {}
 
         if size:
-            self.save_fulltext_file(i, fulltext)
+            self.save_tree_file('fulltext', i, self._gen_fulltext_file(fulltext))
             i += 1
 
         # remove unused tree/fulltext#.js
         while True:
             file = self.get_tree_file('fulltext', i)
             try:
                 self.backup(file)
@@ -560,15 +590,15 @@
     def add_items(self, items, target_parent_id=ROOT_ITEM_ID, target_index=None):
         """Add items to the book.
 
         Args:
             items: an iterable of dict with item properties (or None to
                 generate a new item).
             target_parent_id: None to not insert to any parent
-            index: None to append to last
+            target_index: None to append to last
 
         Returns:
             dict: ID and meta of the added items
 
         Raises:
             ValueError: if the provided item ID already exists, the target
                 parent does not exist, the target index is invalid, etc.
@@ -634,15 +664,15 @@
         elif item.get('create') is None:
             item['create'] = _id_now()
 
         if item.get('modify') is None:
             item['modify'] = item['create']
 
         # remove None keys
-        for key in list(item):
+        for key in tuple(item):
             if item[key] is None:
                 del item[key]
 
         # add to meta
         self.meta[item['id']] = item
 
         # remove ID field
@@ -715,15 +745,15 @@
     def move_items(self, items, target_parent_id, target_index=None):
         """Move items.
 
         Args:
             items: an iterable of tuple (current_parent_id, current_index) in
                 tree order
             target_parent_id: the parent to insert at
-            index: the position to insert at, or None to append to last
+            target_index: the position to insert at, or None to append to last
 
         Returns:
             int: index that the items are inserted at
 
         Raises:
             ValueError: if the item does not exist, the target parent does not
                 exist, the target index is invalid, etc.
@@ -815,15 +845,15 @@
     def link_items(self, items, target_parent_id, target_index=None):
         """Create links for items.
 
         Args:
             items: an iterable of tuple (current_parent_id, current_index) in
                 tree order
             target_parent_id: the parent to insert at
-            index: the position to insert at, or None to append to last
+            target_index: the position to insert at, or None to append to last
 
         Returns:
             int: index that the items are inserted at
 
         Raises:
             ValueError: if the item does not exist, the target parent does not
                 exist, the target index is invalid, etc.
@@ -882,15 +912,15 @@
                    target_book_id=None, recursively=True):
         """Copy items.
 
         Args:
             items: an iterable of tuple (current_parent_id, current_index) in
                 tree order
             target_parent_id: the parent to insert at
-            index: the position to insert at, or None to append to last
+            target_index: the position to insert at, or None to append to last
             target_book_id: the ID of the scrapbook copy to
             recursively: also copy descendant items
 
         Returns:
             int: index that the items are inserted at
             str: ID of the target book
             list: ID of the generated items
@@ -1103,15 +1133,15 @@
                 recycled[item_id] = current_parent_id
                 self.meta[item_id]['parent'] = current_parent_id
                 self.meta[item_id]['recycled'] = recycle_ts
 
         if recycled:
             target_parent_id = self.RECYCLE_ITEM_ID
             target_index = 0 if self.config['new_at_top'] else len(self.toc.get(target_parent_id, ()))
-            self.toc.setdefault(target_parent_id, [])[target_index:target_index] = list(recycled)
+            self.toc.setdefault(target_parent_id, [])[target_index:target_index] = recycled
 
         return recycled
 
     def unrecycle_item(self, current_parent_id, current_index):
         """Singular version shortcut of unrecycle_items()."""
         return self.unrecycle_items(((current_parent_id, current_index),))
 
@@ -1289,14 +1319,15 @@
     def sort_items(self, items, key=None, reverse=False, recursively=False):
         """Sort given items.
 
         Args:
             items: an iterable of container item_id in tree order
             key: the key to sort, which can be 'reverse', 'type', 'title',
                 'index', 'source', 'create', 'modify', or 'marked'
+            reverse: sort in reverse order
             recursively: also sort items in all descendant items
 
         Raises:
             ValueError: if the item does not exist
         """
         if recursively:
             item_ids = {}
@@ -1394,14 +1425,15 @@
 
     def save_item_postit(self, item_id, content, auto_modify=True):
         """Save content for a postit item.
 
         Args:
             item_id: ID of the postit item
             content: new content to save
+            auto_modify: automatically update the 'modify' property
 
         Returns:
             dict: ID and updated meta of the saved postit item
 
         Raises:
             ValueError: if the provided item does not exist, item is not a
                 postit, item index missing, etc.
@@ -1459,24 +1491,27 @@
         if not index.endswith('/index.html'):
             raise ValueError(f"Index page is not '*/index.html': {item_id!r}")
 
         item_dir = os.path.normpath(os.path.join(self.data_dir, os.path.dirname(index)))
 
         if base is None:
             base = index
-        base = os.path.join(self.data_dir, base)
+        base_dir = os.path.normpath(os.path.dirname(os.path.join(self.data_dir, base)))
+
+        if not os.path.normcase(base_dir).startswith(os.path.normcase(os.path.join(self.data_dir, ''))):
+            raise ValueError(f'base not under data directory: {base!r}')
 
         dst = util.validate_filename(('index' if title is None else title) + ext)
-        dst = os.path.normpath(os.path.join(os.path.dirname(base), dst))
+        dst = os.path.join(base_dir, dst)
 
         if os.path.lexists(dst):
             raise ValueError(f'Page already exists: {self.get_subpath(dst)!r}')
 
         try:
-            tpl = self.get_template(item.get('type'), ext)
+            tpl = self.get_template(item.get('type', ''), ext)
         except ValueError:
             data = ''
         else:
             data = util.format_string(tpl, {
                 'NOTE_TITLE': html.escape(item.get('title', '') if title is None else title),
                 'SCRAPBOOK_DIR': html.escape(util.get_relative_url(self.top_dir, dst, start_is_dir=False)),
                 'TREE_DIR': html.escape(util.get_relative_url(self.tree_dir, dst, start_is_dir=False)),
```

### Comparing `webscrapbook-2.0.0b9/webscrapbook/scrapbook/cache.py` & `webscrapbook-2.0.1/webscrapbook/scrapbook/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Generator of fulltext cache and/or static site pages.
 """
-import copy
 import functools
 import html
 import io
 import itertools
 import os
 import re
 import shutil
@@ -315,15 +314,15 @@
 
             entries.append({
                 'id': id,
                 'modify': meta.get('modify', meta.get('create', '')),
                 'item': meta,
             })
         entries = sorted(entries, key=lambda d: d['modify'])
-        entries = list(reversed(entries))[:self.item_count]
+        entries = tuple(reversed(entries))[:self.item_count]
 
         # generate tree
         root = etree.XML(f'<feed xmlns="{self.NS}"></feed>'.encode('UTF-8'))
 
         elem = etree.SubElement(root, 'id')
         elem.text = id_prefix
 
@@ -442,27 +441,27 @@
         book.load_meta_files()
         book.load_toc_files()
         if self.recreate:
             book.fulltext = {}
             book_fulltext_orig = None
         else:
             book.load_fulltext_files()
-            book_fulltext_orig = copy.deepcopy(book.fulltext)
+            book_fulltext_orig = book.checksum(book.fulltext)
 
         # generate cache for each item
         if item_ids:
             id_pool = dict.fromkeys(id for id in item_ids if id in book.meta or id in book.fulltext)
         else:
             id_pool = dict.fromkeys(itertools.chain(book.meta, book.fulltext))
 
         for id in id_pool:
             yield from self._cache_item(id)
 
         # update fulltext files
-        if book.fulltext != book_fulltext_orig:
+        if book.checksum(book.fulltext) != book_fulltext_orig:
             # changed => save new files
             yield Info('info', 'Saving fulltext files...')
             book.save_fulltext_files()
         else:
             # no change => touch files to prevent falsely detected as outdated
             yield Info('info', 'Touching fulltext files...')
             for file in book.iter_fulltext_files():
```

### Comparing `webscrapbook-2.0.0b9/webscrapbook/scrapbook/check.py` & `webscrapbook-2.0.1/webscrapbook/scrapbook/check.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """Generator of integrity check for scrapbook data.
 """
-import copy
 import os
 import time
 import traceback
 from contextlib import nullcontext
 from datetime import datetime
 from urllib.parse import unquote, urlsplit
 
 from .. import WSB_DIR, util
 from .._polyfill import zipfile
 from ..util import Info
-from .book import Book, TreeFileError
+from .book import TreeFileError
 from .host import Host
 from .indexer import (
     SUPPORT_FOLDER_SUFFIXES,
     FavIconCacher,
     Indexer,
     generate_item_create,
     generate_item_modify,
@@ -70,16 +69,16 @@
         self.cnt_dirs = 0
         self.cnt_files = 0
         self.cnt_bytes = 0
 
         yield Info('info', 'Loading tree...')
         self._load_tree()
 
-        book_meta_orig = copy.deepcopy(self.book.meta)
-        book_toc_orig = copy.deepcopy(self.book.toc)
+        book_meta_orig = self.book.checksum(self.book.meta)
+        book_toc_orig = self.book.checksum(self.book.toc)
 
         yield Info('info', 'Checking metadata...')
         yield from self._check_meta()
 
         yield Info('info', 'Checking data files...')
         yield from self._check_data_dir()
 
@@ -87,19 +86,19 @@
         yield from self._check_toc()
         yield from self._check_toc_empty_subtree()
 
         yield Info('info', 'Checking favicon cache...')
         yield from self._check_favicon_cache()
 
         # update files
-        if self.book.meta != book_meta_orig:
+        if self.book.checksum(self.book.meta) != book_meta_orig:
             yield Info('info', 'Saving changed meta files...')
             self.book.save_meta_files()
 
-        if self.book.toc != book_toc_orig:
+        if self.book.checksum(self.book.toc) != book_toc_orig:
             yield Info('info', 'Saving changed TOC files...')
             self.book.save_toc_files()
 
         yield Info('info',
                    f'Totally {self.cnt_items} items, {self.cnt_dirs} folders, '
                    f'{self.cnt_files} files, {util.format_filesize(self.cnt_bytes)}.')
 
@@ -145,15 +144,15 @@
         for id, meta in self.book.meta.items():
             if meta is None:
                 continue
 
             yield Info('debug', f'Checking item meta for {id!r}')
 
             # id
-            if id in Book.SPECIAL_ITEM_ID:
+            if id in self.book.SPECIAL_ITEM_ID:
                 yield Info('error', f'{id!r}: invalid ID (special item)')
                 self.cnt_errors += 1
                 items_invalid_id[id] = True
 
             # type
             type = meta.get('type', '')
 
@@ -173,15 +172,15 @@
                 if type in {'folder', 'separator'}:
                     yield Info('warn', f'{id!r}: a {type!r} item should not have an index file.')
                     self.cnt_warns += 1
                 elif type == 'bookmark' and not index.lower().endswith('.htm'):
                     yield Info('warn', f"{id!r}: a bookmark item should use '*.htm' as index file.")
                     self.cnt_warns += 1
             else:
-                if type not in Book.ITEM_TYPES_WITH_OPTIONAL_INDEX:
+                if type not in self.book.ITEM_TYPES_WITH_OPTIONAL_INDEX:
                     yield Info('error', f"{id!r}: missing 'index' property.")
                     self.cnt_errors += 1
                     items_missing_index[id] = True
 
             # icon
             icon = meta.get('icon')
             if icon:
@@ -308,40 +307,40 @@
         for id, ref_ids in self.book.toc.items():
             if ref_ids is None:
                 continue
 
             yield Info('debug', f'Checking item TOC for {id!r}')
 
             # missing meta
-            if not self.book.meta.get(id) and id not in Book.SPECIAL_ITEM_ID:
+            if not self.book.meta.get(id) and id not in self.book.SPECIAL_ITEM_ID:
                 yield Info('error', f'{id!r}: invalid ID (missing metadata entry)')
                 self.cnt_errors += 1
                 items_missing_meta[id] = True
 
             # check referenced IDs
             for ref_id in ref_ids:
                 self.seen_in_toc.add(ref_id)
 
                 # special item ID is invalid
-                if ref_id in Book.SPECIAL_ITEM_ID:
+                if ref_id in self.book.SPECIAL_ITEM_ID:
                     yield Info('error', f'{id!r}: invalid reference ID {ref_id!r} (special item)')
                     self.cnt_errors += 1
                     ref_items_invalid.setdefault(id, {})[ref_id] = True
                     continue
 
                 # missing meta
                 if not self.book.meta.get(ref_id):
                     yield Info('error', f'{id!r}: invalid reference ID {ref_id!r} (missing metadata entry)')
                     self.cnt_errors += 1
                     ref_items_invalid.setdefault(id, {})[ref_id] = True
                     continue
 
         # items not reachable from TOC
         for id in self.book.meta:
-            if id not in self.seen_in_toc and id not in Book.SPECIAL_ITEM_ID:
+            if id not in self.seen_in_toc and id not in self.book.SPECIAL_ITEM_ID:
                 yield Info('error', f'{id!r}: not recheable from TOC.')
                 self.cnt_errors += 1
                 items_unreachable[id] = True
 
         if (items_missing_meta or ref_items_invalid) and self.resolve_toc_invalid:
             yield from self._resolve_toc_invalid(items_missing_meta, ref_items_invalid)
 
@@ -674,18 +673,18 @@
                 # skip invalid book ID
                 yield Info('warn', f'Skipped invalid book {book_id!r}.')
                 continue
 
             yield Info('debug', f'Loading book {book_id!r}...')
 
             if book.no_tree:
-                yield Info('info', f'Skipped book {book_id!r} ({book.name}) (no_tree).')
+                yield Info('info', f'Skipped book {book_id!r} ({book.name!r}) (no_tree).')
                 continue
 
-            yield Info('info', f'Checking book {book_id!r} ({book.name}).')
+            yield Info('info', f'Checking book {book_id!r} ({book.name!r}).')
             lh = book.get_tree_lock(persist=lock).acquire() if lock else nullcontext()
             with lh:
                 generator = BookChecker(book, **kwargs)
                 yield from generator.run()
 
             yield Info('info', 'Done.')
     except Exception as exc:
```

### Comparing `webscrapbook-2.0.0b9/webscrapbook/scrapbook/convert/file2wsb.py` & `webscrapbook-2.0.1/webscrapbook/scrapbook/convert/file2wsb.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         self.handle_savepagewe_meta = handle_savepagewe_meta
         self.handle_maoxian_meta = handle_maoxian_meta
         self.wsb_dir = os.path.join(self.input, WSB_DIR)
         self.host = None
         self.book = None
 
     def run(self):
+        os.makedirs(self.output, exist_ok=True)
         self.host = Host(self.output)
         self.book = self.host.books['']
 
         self.book.load_meta_files()
         self.book.load_toc_files()
 
         yield Info('info', 'Inspecting data files...')
```

### Comparing `webscrapbook-2.0.0b9/webscrapbook/scrapbook/convert/items.py` & `webscrapbook-2.0.1/webscrapbook/scrapbook/convert/items.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import copy
 import html
 import os
 import shutil
 import time
 import traceback
 from datetime import datetime, timezone
 from email.utils import format_datetime
@@ -22,14 +21,15 @@
         self.book_items = book_items
         self.types = set(types) if types else {}
         self.format = format
 
     def run(self):
         if self.input != self.output:
             yield Info('info', 'Copying files...')
+            os.makedirs(self.output, exist_ok=True)
             self._copy_files()
 
         yield Info('info', 'Applying conversion...')
         host = Host(self.output)
 
         for book_id, item_ids in (self.book_items or dict.fromkeys(host.books)).items():
             try:
@@ -38,15 +38,15 @@
                 # skip invalid book ID
                 yield Info('warn', f'Skipped invalid book {book_id!r}.')
                 continue
 
             yield Info('info', f'Handling book {book_id!r}...')
             book.load_meta_files()
 
-            book_meta_orig = copy.deepcopy(book.meta)
+            book_meta_orig = book.checksum(book.meta)
 
             for id in (item_ids or book.meta):
                 if id not in book.meta:
                     # skip invalid item ID
                     yield Info('debug', f'Skipped invalid item {id!r}.')
                     continue
 
@@ -64,15 +64,15 @@
                         except OSError as exc:
                             raise RuntimeError(exc.strerror) from exc
                     except Exception as exc:
                         traceback.print_exc()
                         yield Info('error', f'Failed to convert {id!r}: {exc}', exc=exc)
 
             # update files
-            if book.meta != book_meta_orig:
+            if book.checksum(book.meta) != book_meta_orig:
                 yield Info('info', 'Saving changed meta files...')
                 book.save_meta_files()
 
     def _copy_files(self):
         with os.scandir(self.input) as dirs:
             for src in dirs:
                 dst = os.path.join(self.output, src.name)
```

### Comparing `webscrapbook-2.0.0b9/webscrapbook/scrapbook/convert/migrate.py` & `webscrapbook-2.0.1/webscrapbook/scrapbook/convert/migrate.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,14 +150,15 @@
         self.convert_legacy = convert_legacy
         self.convert_v1 = convert_v1
         self.use_native_tags = use_native_tags
 
     def run(self):
         if self.input != self.output:
             yield Info('info', 'Copying files...')
+            os.makedirs(self.output, exist_ok=True)
             self._copy_files()
 
         yield Info('info', 'Applying migration...')
         host = Host(self.output)
 
         # handle all books if none specified
         for book_id in self.book_ids or host.books:
```

### Comparing `webscrapbook-2.0.0b9/webscrapbook/scrapbook/convert/sb2wsb.py` & `webscrapbook-2.0.1/webscrapbook/scrapbook/convert/sb2wsb.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from urllib.parse import unquote
 from urllib.request import pathname2url
 
 from lxml import etree
 
 from ... import WSB_CONFIG, WSB_DIR, util
 from ...util import Info
-from ..book import Book
 from ..host import Host
 
 RDF = '{http://www.w3.org/1999/02/22-rdf-syntax-ns#}'
 NS1 = '{http://amb.vis.ne.jp/mozilla/scrapbook-rdf#}'
 NS2 = '{scrapbee@163.com}'  # ScrapBee
 NC = '{http://home.netscape.com/NC-rdf#}'
 RES_PROTOCOL_BASE = 'resource://scrapbook/'
@@ -248,15 +247,15 @@
             meta['type'] = LEGACY_TYPE_MAP.get(meta.get('type'), meta.get('type', ''))
             if meta['type'] == 'marked':
                 # if sitemap exists, type should be site
                 meta['type'] = 'site' if id in book0.sitemaps else ''
                 meta['marked'] = True
 
             # meta['index']
-            if meta['type'] not in Book.ITEM_TYPES_WITH_OPTIONAL_INDEX:
+            if meta['type'] not in book.ITEM_TYPES_WITH_OPTIONAL_INDEX:
                 meta['index'] = f'{id}/index.html'
             elif meta.get('icon', '').startswith(f'{RES_PROTOCOL_BASE}data/{id}/'):
                 # Add a dummy index.html to relate the icon file with the item
                 # if it's saved in the item directory. (mainly for ScrapBee)
                 meta['index'] = f'{id}/index.html'
                 self.index_files[os.path.normpath(os.path.join(book.data_dir, id, 'index.html'))] = True
                 yield Info('debug', f'Registering dummy file {meta["index"]!r}')
```

### Comparing `webscrapbook-2.0.0b9/webscrapbook/scrapbook/convert/wsb2file.py` & `webscrapbook-2.0.1/webscrapbook/scrapbook/convert/wsb2file.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import os
 import shutil
 import time
 import traceback
 
 from ... import util
 from ...util import Info
-from ..book import Book
 from ..host import Host
 
 
 class Converter:
     def __init__(self, input, output, book_id='', prefix=True):
         self.input = input
         self.output = output
@@ -35,15 +34,15 @@
         path_chain = []
         ref_ids = self.book.toc.get(self.book.ROOT_ITEM_ID, [])
         idx_len = len(str(len(ref_ids)))
         for idx, ref_id in enumerate(ref_ids):
             yield from self._export_item(ref_id, idx, idx_len, id_chain, path_chain)
 
     def _export_item(self, id, idx, idx_len, id_chain, path_chain):
-        if id not in self.book.meta or id in Book.SPECIAL_ITEM_ID:
+        if id not in self.book.meta or id in self.book.SPECIAL_ITEM_ID:
             return
 
         yield Info('debug', f'Exporting item {id!r}')
 
         meta = self.book.meta[id]
         type = meta.get('type', '')
         prefix = f'{idx + 1:0{idx_len}d}-' if self.prefix else ''
```

### Comparing `webscrapbook-2.0.0b9/webscrapbook/scrapbook/convert/wsb2sb.py` & `webscrapbook-2.0.1/webscrapbook/scrapbook/convert/wsb2sb.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from urllib.request import pathname2url
 
 from lxml import etree
 
 from ... import util
 from ...util import Info
 from ...util.html import HtmlRewriter, Markup, MarkupTag
-from ..book import Book
 from ..host import Host
 
 RDF = '{http://www.w3.org/1999/02/22-rdf-syntax-ns#}'
 NS1 = '{http://amb.vis.ne.jp/mozilla/scrapbook-rdf#}'
 NC = '{http://home.netscape.com/NC-rdf#}'
 
 LEGACY_TYPE_MAP = {
@@ -204,15 +203,15 @@
         os.makedirs(os.path.dirname(file), exist_ok=True)
         tree.write(file, encoding='UTF-8', xml_declaration=True, pretty_print=True)
 
     def _copy_data_files(self, book):
         for id, oid in self.id_to_oid.items():
             yield Info('debug', f'Copying data files for {id!r} => {oid!r}')
             type = book.meta[id].get('type', '')
-            if type in Book.ITEM_TYPES_WITH_OPTIONAL_INDEX:
+            if type in book.ITEM_TYPES_WITH_OPTIONAL_INDEX:
                 yield Info('debug', f'Skipped copying data for {id!r}: type is {type!r}')
                 continue
 
             index = book.meta[id].get('index', '')
             if not index:
                 yield Info('debug', f'Skipped copying data for {id!r}: no index')
                 continue
```

### Comparing `webscrapbook-2.0.0b9/webscrapbook/scrapbook/exporter.py` & `webscrapbook-2.0.1/webscrapbook/scrapbook/exporter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import os
 import time
 import traceback
 from collections import OrderedDict
 from contextlib import nullcontext
-from datetime import datetime, timedelta
+from datetime import timedelta
 
 from .. import util
 from .._polyfill import mimetypes, zipfile
 from ..util import Info
 from .book import _id_now
 from .host import Host
 
@@ -16,35 +16,43 @@
 
 SCHEME_ITEM_IDS = 0
 SCHEME_ROOT_INDEXES = 1
 
 
 class Exporter():
     """Main class for generating exports."""
-    def __init__(self, output, book, *, scheme=SCHEME_ITEM_IDS, singleton=False):
+    def __init__(self, output, book, *, scheme=SCHEME_ITEM_IDS, singleton=False, stream=None):
         self.output = output
         self.book = book
         self.scheme = scheme
         self.singleton = singleton
+        self.stream = stream
 
     def run(self, items=None, recursive=False):
         self.book.load_meta_files()
         self.book.load_toc_files()
 
-        os.makedirs(self.output, exist_ok=True)
-
         self.used_ts = set()
         self.map_id_to_eid = {}
 
-        if self.scheme == SCHEME_ITEM_IDS:
-            yield from self._export_from_item_ids(items, recursive)
-        elif self.scheme == SCHEME_ROOT_INDEXES:
-            yield from self._export_from_root_indexes(items, recursive)
+        if isinstance(self.output, zipfile.ZipFile):
+            cm = nullcontext(self.output)
         else:
-            raise ValueError(f'Unknown items scheme: {self.scheme!r}')
+            cm = zipfile.ZipFile(self.output, 'w')
+
+        with cm as self._zh:
+            if self.scheme == SCHEME_ITEM_IDS:
+                yield from self._export_from_item_ids(items, recursive)
+            elif self.scheme == SCHEME_ROOT_INDEXES:
+                yield from self._export_from_root_indexes(items, recursive)
+            else:
+                raise ValueError(f'Unknown items scheme: {self.scheme!r}')
+
+        if self.stream is not None:
+            yield Info('debug', 'Streaming...', self.stream.get())
 
     def _export_from_item_ids(self, items, recursive):
         id_pool = set(self.book.meta)
         if items:
             # add descendant id if recursive mode
             if recursive:
                 dict_ = {}
@@ -151,66 +159,68 @@
             ets = util.datetime_to_id(dt)
         self.used_ts.add(ets)
 
         # setup an export id (eid), which is unique and is same among all
         # occurrences of the same id, to the ets of the first occurrence
         eid = self.map_id_to_eid.setdefault(id, ets)
 
-        # generate a unique timestamp prefix
-        basename = ets + '-' + meta.get('title', meta.get('id', ''))
-        basename = util.crop(util.validate_filename(basename), 128)
-
-        # generate a unique filename
-        i = 0
-        dst = os.path.join(self.output, f'{basename}.wsba')
-        while os.path.lexists(dst):
-            i += 1
-            dst = os.path.join(self.output, f'{basename}-{i}.wsba')
-
-        yield Info('info', f'Exporting {id!r} to {os.path.basename(dst)!r}')
+        yield Info('info', f'Exporting {id!r} to {ets!r}')
         parents = [{'id': id, 'title': self.book.meta.get(id, {}).get('title', '')} for id in parent_ids]
         meta_data = {'id': id, **meta}
         export_data = {
             'version': EXPORTER_VERSION,
             'id': eid,
             'timestamp': ets,
-            'timezone': int(datetime.now().astimezone().utcoffset().total_seconds()),
+            'timezone': int(util.id_to_datetime(ets).astimezone().utcoffset().total_seconds()),
             'path': parents,
             'index': pos,
         }
-        with zipfile.ZipFile(dst, 'w') as zh:
-            fn = 'meta.json'
-            zh.writestr(fn, json.dumps(meta_data, ensure_ascii=False, indent=2),
-                        **util.fs.zip_compression_params(mimetypes.guess_type(fn)[0]))
-            fn = 'export.json'
-            zh.writestr(fn, json.dumps(export_data, ensure_ascii=False, indent=2),
-                        **util.fs.zip_compression_params(mimetypes.guess_type(fn)[0]))
-
-            # include data file(s)
-            if index:
-                zh.writestr('data/', '')
-                src = os.path.join(self.book.data_dir, os.path.dirname(index) if index.endswith('/index.html') else index)
-                yield Info('debug', f'Saving data files for {id!r}: {self.book.get_subpath(src)!r}')
-                util.fs.zip_compress(zh, src, f'data/{os.path.basename(src)}')
-
-            # include favicon cache
-            iconfile = self.book.get_icon_file(meta)
-            if not iconfile:
-                return
 
-            favicon_dir = os.path.join(self.book.tree_dir, 'favicon', '')
-            if not os.path.normcase(iconfile).startswith(os.path.normcase(favicon_dir)):
-                return
+        zh = self._zh
+
+        # add topdir and info files
+        zh.writestr(f'{ets}/', '')
+        fn = f'{ets}/meta.json'
+        zh.writestr(fn, json.dumps(meta_data, ensure_ascii=False, indent=2),
+                    **util.fs.zip_compression_params(mimetypes.guess_type(fn)[0]))
+        fn = f'{ets}/export.json'
+        zh.writestr(fn, json.dumps(export_data, ensure_ascii=False, indent=2),
+                    **util.fs.zip_compression_params(mimetypes.guess_type(fn)[0]))
+        if self.stream is not None:
+            yield Info('debug', 'Streaming...', self.stream.get())
+
+        # include data file(s)
+        if index:
+            zh.writestr(f'{ets}/data/', '')
+            src = os.path.join(self.book.data_dir, os.path.dirname(index) if index.endswith('/index.html') else index)
+            yield Info('debug', f'Saving data files for {id!r}: {self.book.get_subpath(src)!r}')
+            gen = util.fs.zip_compress(zh, src, f'{ets}/data/{os.path.basename(src)}', stream=self.stream)
+            if self.stream is not None:
+                for bytes_ in gen:
+                    yield Info('debug', 'Streaming...', bytes_)
+
+        # include favicon cache
+        iconfile = self.book.get_icon_file(meta)
+        if not iconfile:
+            return
+
+        favicon_dir = os.path.join(self.book.tree_dir, 'favicon', '')
+        if not os.path.normcase(iconfile).startswith(os.path.normcase(favicon_dir)):
+            return
 
-            zh.writestr('favicon/', '')
-            util.fs.zip_compress(zh, iconfile, f'favicon/{os.path.basename(iconfile)}')
+        zh.writestr(f'{ets}/favicon/', '')
+        gen = util.fs.zip_compress(zh, iconfile, f'{ets}/favicon/{os.path.basename(iconfile)}', stream=self.stream)
+        if self.stream is not None:
+            for bytes_ in gen:
+                yield Info('debug', 'Streaming...', bytes_)
 
 
 def run(host, output, book_id='', items=None, *,
-        scheme=SCHEME_ITEM_IDS, recursive=False, singleton=False, lock=True):
+        scheme=SCHEME_ITEM_IDS, recursive=False, singleton=False, stream=None,
+        lock=True):
     start = time.time()
 
     if isinstance(host, Host):
         pass
     elif isinstance(host, str):
         host = Host(host)
     else:
@@ -229,15 +239,15 @@
         if book.no_tree:
             yield Info('error', f'Unable to export book {book_id!r} ({book.name!r}) (no_tree).')
             return
 
         yield Info('info', f'Exporting from book {book_id!r} ({book.name!r}).')
         lh = book.get_tree_lock(persist=lock).acquire() if lock else nullcontext()
         with lh:
-            generator = Exporter(output, book, scheme=scheme, singleton=singleton)
+            generator = Exporter(output, book, scheme=scheme, singleton=singleton, stream=stream)
             yield from generator.run(items, recursive)
 
     except Exception as exc:
         traceback.print_exc()
         yield Info('critical', str(exc), exc=exc)
         return
     else:
```

### Comparing `webscrapbook-2.0.0b9/webscrapbook/scrapbook/exporter1.py` & `webscrapbook-2.0.1/webscrapbook/scrapbook/exporter1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Legacy module for exporting version 1 *.wsba"""
 import json
 import os
 import time
 import traceback
 from collections import OrderedDict
 from contextlib import nullcontext
-from datetime import datetime, timedelta
+from datetime import timedelta
 
 from .. import util
 from .._polyfill import mimetypes, zipfile
 from ..util import Info
 from .book import _id_now
 from .host import Host
 
@@ -112,15 +112,15 @@
         yield Info('info', f'Exporting {id!r} to {os.path.basename(dst)!r}')
         parents = [{'id': id, 'title': self.book.meta.get(id, {}).get('title', '')} for id in parent_ids]
         meta_data = {'id': id, **meta}
         export_data = {
             'version': EXPORTER_VERSION,
             'id': eid,
             'timestamp': ets,
-            'timezone': datetime.now().astimezone().utcoffset().total_seconds(),
+            'timezone': util.id_to_datetime(ets).astimezone().utcoffset().total_seconds(),
             'path': parents,
         }
         with zipfile.ZipFile(dst, 'w') as zh:
             fn = 'meta.json'
             zh.writestr(fn, json.dumps(meta_data, ensure_ascii=False, indent=2),
                         **util.fs.zip_compression_params(mimetypes.guess_type(fn)[0]))
             fn = 'export.json'
```

### Comparing `webscrapbook-2.0.0b9/webscrapbook/scrapbook/host.py` & `webscrapbook-2.0.1/webscrapbook/scrapbook/host.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Scrapbook host handler.
 """
+import hashlib
 import os
 import shutil
 import stat
 import time
 from collections import UserDict
 from secrets import token_urlsafe
 from threading import Thread
 
 from .. import WSB_DIR, WSB_USER_DIR, Config, util
 from ..locales import I18N
-from .book import Book
+from . import book
 
 
 class LockError(Exception):
     def __init__(self, msg, name=None, file=None, id=None):
         self.msg = msg
         self.name = name
         self.file = file
@@ -94,15 +95,15 @@
     """
     def __init__(self, host, name, *,
                  timeout=5, stale=60, persist=False):
         self.host = host
         self.name = name
         self.timeout = timeout
         self.stale = stale
-        self.file = os.path.join(host.locks, f'{util.encrypt(name, method="md5")}.lock')
+        self.file = os.path.join(host.locks, f'{hashlib.md5(name.encode("utf8")).hexdigest()}.lock')
         self._keeper = None
 
         if isinstance(persist, str) and persist:
             try:
                 with open(self.file, encoding='UTF-8') as fh:
                     assert fh.read() == persist
             except OSError as exc:
@@ -337,15 +338,15 @@
         self.host = host
         for book_id in host.config['book']:
             self.data[book_id] = NotImplemented
 
     def __getitem__(self, key):
         rv = self.data[key]
         if rv is NotImplemented:
-            rv = self.data[key] = Book(self.host, key)
+            rv = self.data[key] = book.Book(self.host, key)
         return rv
 
 
 class Host:
     """Controller for a scrapbook set defined by a root directory and configs.
     """
     REPR_ATTRS = ('name', 'root')
```

### Comparing `webscrapbook-2.0.0b9/webscrapbook/scrapbook/importer.py` & `webscrapbook-2.0.1/webscrapbook/scrapbook/importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-import copy
 import json
 import os
 import re
-import shutil
 import time
 import traceback
 import uuid
 from contextlib import nullcontext
 from urllib.request import pathname2url
 
 from .. import util
@@ -38,64 +36,45 @@
     def run(self, files=None):
         self.book.load_meta_files()
         self.book.load_toc_files()
 
         self.map_eid_to_info = {}
         self.map_id_to_new_id = {}
 
-        book_meta_orig = copy.deepcopy(self.book.meta)
-        book_toc_orig = copy.deepcopy(self.book.toc)
+        book_meta_orig = self.book.checksum(self.book.meta)
+        book_toc_orig = self.book.checksum(self.book.toc)
 
         # fix target_id
         if not self.rebuild_folders:
             if self.target_id is None:
                 self.target_id = self.book.ROOT_ITEM_ID
             elif not (self.target_id in self.book.meta or self.target_id in self.book.SPECIAL_ITEM_ID):
                 yield Info('warn', f'Target ID {self.target_id!r} is invalid. Use {self.book.ROOT_ITEM_ID!r} instead.')
                 self.target_id = self.book.ROOT_ITEM_ID
 
         for file in files:
-            if os.path.isdir(file):
-                with os.scandir(file) as entries:
-                    srcs = sorted(f.path for f in entries if util.is_wsba(f.path))
-            elif os.path.isfile(file):
-                if not util.is_wsba(file):
-                    yield Info('warn', f'Skipped invalid file {os.path.basename(file)!r}')
-                    continue
-                srcs = [file]
+            yield Info('info', f'Importing archive file {os.path.basename(file)!r}')
+            try:
+                successful = yield from self._import_file(file)
+            except Exception as exc:
+                # unexpected error
+                traceback.print_exc()
+                yield Info('error', f'Failed to import file {os.path.basename(file)!r}: {exc}', exc=exc)
             else:
-                yield Info('error', f'Failed to import file {os.path.basename(file)!r}: unable to access file')
-                continue
-
-            for src in srcs:
-                try:
-                    yield Info('debug', f'Importing file {os.path.basename(src)!r}')
-                    id, eid, parent_id = yield from self._import_file(src)
-                except RuntimeError as exc:
-                    # intended raise to skip the import
-                    yield Info('error', f'Failed to import file {os.path.basename(src)!r}: {exc}', exc=exc)
-                except Exception as exc:
-                    # unexpected error
-                    traceback.print_exc()
-                    yield Info('error', f'Failed to import file {os.path.basename(src)!r}: {exc}', exc=exc)
-                else:
-                    # finalize a successful import
-                    text_parent = '' if parent_id is None else f' (under {parent_id!r})'
-                    yield Info('info', f'Imported {id!r}{text_parent}')
-                    self.map_eid_to_info.setdefault(eid, {}).setdefault('id', id)
-                    if self.prune:
-                        yield Info('debug', f'Removing {os.path.basename(src)!r} (prune)')
-                        os.remove(src)
+                # finalize a successfully imported file
+                if successful and self.prune:
+                    yield Info('debug', f'Removing {os.path.basename(file)!r} (prune)')
+                    os.remove(file)
 
         # update files
-        if self.book.meta != book_meta_orig:
+        if self.book.checksum(self.book.meta) != book_meta_orig:
             yield Info('info', 'Saving changed meta files...')
             self.book.save_meta_files()
 
-        if self.book.toc != book_toc_orig:
+        if self.book.checksum(self.book.toc) != book_toc_orig:
             yield Info('info', 'Saving changed TOC files...')
             self.book.save_toc_files()
 
     def generate_imported_filename(self, id, meta, export_info):
         """Generate an adequate filename (without file extension) for an
         importing item.
         """
@@ -195,63 +174,94 @@
             return ''
 
         filename = REGEX_TARGET_FILENAME_FORMATTER.sub(formatter, self.target_filename)
         filename = '/'.join(util.validate_filename(s) for s in filename.split('/'))
         return filename
 
     def _import_file(self, file):
+        successful = True
         with zipfile.ZipFile(file) as zh:
-            with zh.open('meta.json') as fh:
-                meta = json.load(fh)
+            topdirs = set()
+            for zinfo in zh.infolist():
+                topdir, _, _ = zinfo.filename.partition('/')
+                topdirs.add(topdir)
+
+            for topdir in sorted(topdirs):
+                yield Info('debug', f'Importing entry {topdir!r}')
+                try:
+                    yield from self._import_topdir(zh, topdir)
+                except RuntimeError as exc:
+                    # intended raise to skip the import
+                    yield Info('error', f'Failed to import entry {topdir!r}: {exc}', exc=exc)
+                    successful = False
+                except Exception as exc:
+                    # unexpected error
+                    traceback.print_exc()
+                    yield Info('error', f'Failed to import entry {topdir!r}: {exc}', exc=exc)
+                    successful = False
+
+        return successful
 
-            with zh.open('export.json') as fh:
+    def _import_topdir(self, zh, topdir):
+        try:
+            with zh.open(f'{topdir}/export.json') as fh:
                 export_info = json.load(fh)
+        except Exception as exc:
+            raise RuntimeError(f"Unable to read 'export.json': {exc}") from exc
 
-            if export_info['version'] == 2:
-                try:
-                    assert isinstance(export_info['id'], str)
-                    assert isinstance(export_info['timestamp'], str)
-                    assert isinstance(export_info['timezone'], int)
-                    assert isinstance(export_info['path'], list)
-                    assert isinstance(export_info['index'], int)
-                except (AssertionError, KeyError):
-                    raise RuntimeError('Malformed archive')
+        if export_info['version'] == 2:
+            try:
+                assert isinstance(export_info['id'], str)
+                assert isinstance(export_info['timestamp'], str)
+                assert isinstance(export_info['timezone'], int)
+                assert isinstance(export_info['path'], list)
+                assert isinstance(export_info['index'], int)
+            except (AssertionError, KeyError) as exc:
+                raise RuntimeError("Malformed 'export.json'") from exc
 
-            else:
-                raise RuntimeError(f'Unsupported archive version: {export_info["version"]!r}')
+        else:
+            raise RuntimeError(f'Unsupported archive version: {export_info["version"]!r}')
 
-            id = meta.pop('id')
-            if id in self.book.SPECIAL_ITEM_ID:
-                raise RuntimeError(f'invalid ID {id!r}')
-
-            # skip importing data for a duplicated occurrence of a previously
-            # imported item
-            imported_id = self.map_eid_to_info.setdefault(export_info['id'], {}).get('id')
-            if imported_id is not None:
-                id = imported_id
-                yield Info('debug', f'Skipped importing data for multi-referenced {id!r}')
-            else:
-                id = yield from self._import_meta_and_data(id, meta, zh, export_info)
+        try:
+            with zh.open(f'{topdir}/meta.json') as fh:
+                meta = json.load(fh)
+        except Exception as exc:
+            raise RuntimeError(f"Unable to read 'meta.json': {exc}") from exc
+
+        id = meta.pop('id')
+        if id in self.book.SPECIAL_ITEM_ID:
+            raise RuntimeError(f'invalid ID {id!r}')
+
+        # skip importing data for a duplicated occurrence of a previously
+        # imported item
+        imported_id = self.map_eid_to_info.setdefault(export_info['id'], {}).get('id')
+        if imported_id is not None:
+            id = imported_id
+            yield Info('debug', f'Skipped importing data for multi-referenced {id!r}')
+        else:
+            id = yield from self._import_meta_and_data(id, meta, zh, topdir, export_info)
 
-            parent_id = yield from self._insert_to_toc(id, export_info)
-            return id, export_info['id'], parent_id
+        parent_id = yield from self._insert_to_toc(id, export_info)
+        text_parent = '' if parent_id is None else f' (under {parent_id!r})'
+        yield Info('info', f'Imported {id!r}{text_parent}')
+        self.map_eid_to_info.setdefault(export_info['id'], {}).setdefault('id', id)
 
-    def _import_meta_and_data(self, id, meta, zh, export_info):
+    def _import_meta_and_data(self, id, meta, zh, topdir, export_info):
         """Import meta and data
 
         Returns:
             string: ID of the imported item
         """
         index = meta.get('index', '')
 
         if index:
             if index.endswith('/index.html'):
-                src = f'data/{os.path.dirname(index)}'
+                src = f'{topdir}/data/{os.path.dirname(index)}'
             else:
-                src = f'data/{index}'
+                src = f'{topdir}/data/{index}'
 
             # determine normal copy dst
             _, ext = os.path.splitext(src)
             filename = self.generate_imported_filename(id, meta, export_info) + ext
             dst = os.path.normpath(os.path.join(self.book.data_dir, filename))
             meta['index'] = filename + ('/index.html' if index.endswith('/index.html') else '')
 
@@ -268,39 +278,35 @@
                 # replace only if index type matches
                 if os.path.splitext(index)[1] != os.path.splitext(index_old)[1]:
                     raise RuntimeError('index type not match')
 
                 if index_old.endswith('/index.html') != index.endswith('/index.html'):
                     raise RuntimeError('index type not match')
 
-                yield Info('info', f'Force importing duplicated {id!r}...')
+                yield Info('warn', f'Importing duplicated {id!r} in place of the current...')
 
                 if index:
                     # use original index
                     meta['index'] = index_old
 
                     # remove current index file or folder
                     if index.endswith('/index.html'):
                         dst = os.path.normpath(os.path.join(self.book.data_dir, os.path.dirname(index_old)))
-                        try:
-                            shutil.rmtree(dst)
-                        except FileNotFoundError:
-                            pass
                     else:
                         dst = os.path.normpath(os.path.join(self.book.data_dir, index_old))
-                        try:
-                            os.remove(dst)
-                        except FileNotFoundError:
-                            pass
+                    try:
+                        util.fs.delete(dst)
+                    except util.fs.FSEntryNotFoundError:
+                        pass
 
                 self.map_eid_to_info.setdefault(export_info['id'], {}).setdefault('replaced', True)
 
             elif self.resolve_id_used == 'new':
                 new_id = self.book.get_unique_id()
-                yield Info('info', f'Importing duplicated {id!r} as {new_id!r}...')
+                yield Info('warn', f'Importing duplicated {id!r} as {new_id!r}...')
 
                 if index:
                     # overwrite dst and index
                     filename = self.generate_imported_filename(new_id, meta, export_info) + ext
                     dst = os.path.normpath(os.path.join(self.book.data_dir, filename))
                     meta['index'] = filename + ('/index.html' if index.endswith('/index.html') else '')
 
@@ -336,25 +342,25 @@
         # import data files
         if index:
             if os.path.lexists(dst):
                 raise RuntimeError(f'file {dst!r} already exists')
 
             yield Info('debug', f'Extracting data files to {self.book.get_subpath(dst)!r}')
             os.makedirs(os.path.dirname(dst), exist_ok=True)
-            util.fs.zip_extract(zh, dst, src, tzoffset=export_info['timezone'])
+            util.fs.zip_extract(zh, dst, src)
 
         # import favicon
         for f in zh.namelist():
-            if f.startswith('favicon/') and not f.endswith('/'):
+            if f.startswith(f'{topdir}/favicon/') and not f.endswith('/'):
                 basename = os.path.basename(f)
                 iconfile = os.path.join(self.book.tree_dir, 'favicon', basename)
                 os.makedirs(os.path.dirname(iconfile), exist_ok=True)
 
                 try:
-                    util.fs.zip_extract(zh, iconfile, f, tzoffset=export_info['timezone'])
+                    util.fs.zip_extract(zh, iconfile, f)
                 except FileExistsError:
                     yield Info('debug', f'Skipped existing favicon cache {basename!r}')
                 else:
                     yield Info('info', f'Added favicon cache {basename!r}')
 
                 # rewrite icon property to be consistent with the importing book
                 try:
```

### Comparing `webscrapbook-2.0.0b9/webscrapbook/scrapbook/importer1.py` & `webscrapbook-2.0.1/webscrapbook/scrapbook/importer1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Legacy module for importing version 1 *.wsba"""
 import copy
 import json
 import os
 import re
-import shutil
 import time
 import traceback
 import uuid
 from contextlib import nullcontext
 from urllib.request import pathname2url
 
 from .. import util
@@ -221,32 +220,38 @@
 
         filename = REGEX_TARGET_FILENAME_FORMATTER.sub(formatter, self.target_filename)
         filename = '/'.join(util.validate_filename(s) for s in filename.split('/'))
         return filename
 
     def _import_file(self, file):
         with zipfile.ZipFile(file) as zh:
-            with zh.open('meta.json') as fh:
-                meta = json.load(fh)
-
-            with zh.open('export.json') as fh:
-                export_info = json.load(fh)
+            try:
+                with zh.open('export.json') as fh:
+                    export_info = json.load(fh)
+            except Exception as exc:
+                raise RuntimeError(f"Unable to read 'export.json': {exc}") from exc
 
             if export_info['version'] == 1:
                 try:
                     assert isinstance(export_info['id'], str)
                     assert isinstance(export_info['timestamp'], str)
                     assert isinstance(export_info['timezone'], float)
                     assert isinstance(export_info['path'], list)
-                except (AssertionError, KeyError):
-                    raise RuntimeError('Malformed archive')
+                except (AssertionError, KeyError) as exc:
+                    raise RuntimeError("Malformed 'export.json'") from exc
 
             else:
                 raise RuntimeError(f'Unsupported archive version: {export_info["version"]!r}')
 
+            try:
+                with zh.open('meta.json') as fh:
+                    meta = json.load(fh)
+            except Exception as exc:
+                raise RuntimeError(f"Unable to read 'meta.json': {exc}") from exc
+
             id = meta.pop('id')
             if id in self.book.SPECIAL_ITEM_ID:
                 raise RuntimeError(f'invalid ID {id!r}')
 
             # skip importing data for a duplicated occurrence of a previously
             # imported item
             imported_id = self.map_eid_to_info.setdefault(export_info['id'], {}).get('id')
@@ -292,39 +297,35 @@
                 # replace only if index type matches
                 if os.path.splitext(index)[1] != os.path.splitext(index_old)[1]:
                     raise RuntimeError('index type not match')
 
                 if index_old.endswith('/index.html') != index.endswith('/index.html'):
                     raise RuntimeError('index type not match')
 
-                yield Info('info', f'Force importing duplicated {id!r}...')
+                yield Info('warn', f'Importing duplicated {id!r} in place of the current...')
 
                 if index:
                     # use original index
                     meta['index'] = index_old
 
                     # remove current index file or folder
                     if index.endswith('/index.html'):
                         dst = os.path.normpath(os.path.join(self.book.data_dir, os.path.dirname(index_old)))
-                        try:
-                            shutil.rmtree(dst)
-                        except FileNotFoundError:
-                            pass
                     else:
                         dst = os.path.normpath(os.path.join(self.book.data_dir, index_old))
-                        try:
-                            os.remove(dst)
-                        except FileNotFoundError:
-                            pass
+                    try:
+                        util.fs.delete(dst)
+                    except util.fs.FSEntryNotFoundError:
+                        pass
 
                 self.map_eid_to_info.setdefault(export_info['id'], {}).setdefault('replaced', True)
 
             elif self.resolve_id_used == 'new':
                 new_id = self.book.get_unique_id()
-                yield Info('info', f'Importing duplicated {id!r} as {new_id!r}...')
+                yield Info('warn', f'Importing duplicated {id!r} as {new_id!r}...')
 
                 if index:
                     # overwrite dst and index
                     filename = self.generate_imported_filename(new_id, meta, export_info) + ext
                     dst = os.path.normpath(os.path.join(self.book.data_dir, filename))
                     meta['index'] = filename + ('/index.html' if index.endswith('/index.html') else '')
 
@@ -360,25 +361,25 @@
         # import data files
         if index:
             if os.path.lexists(dst):
                 raise RuntimeError(f'file {dst!r} already exists')
 
             yield Info('debug', f'Extracting data files to {self.book.get_subpath(dst)!r}')
             os.makedirs(os.path.dirname(dst), exist_ok=True)
-            util.fs.zip_extract(zh, dst, src, tzoffset=export_info['timezone'])
+            util.fs.zip_extract(zh, dst, src)
 
         # import favicon
         for f in zh.namelist():
             if f.startswith('favicon/') and not f.endswith('/'):
                 basename = os.path.basename(f)
                 iconfile = os.path.join(self.book.tree_dir, 'favicon', basename)
                 os.makedirs(os.path.dirname(iconfile), exist_ok=True)
 
                 try:
-                    util.fs.zip_extract(zh, iconfile, f, tzoffset=export_info['timezone'])
+                    util.fs.zip_extract(zh, iconfile, f)
                 except FileExistsError:
                     yield Info('debug', f'Skipped existing favicon cache {basename!r}')
                 else:
                     yield Info('info', f'Added favicon cache {basename!r}')
 
                 # rewrite icon property to be consistent with the importing book
                 try:
```

### Comparing `webscrapbook-2.0.0b9/webscrapbook/scrapbook/indexer.py` & `webscrapbook-2.0.1/webscrapbook/scrapbook/indexer.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b9/webscrapbook/scrapbook/search.py` & `webscrapbook-2.0.1/webscrapbook/scrapbook/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         self.default = 'tcc'
         self.mc = False
         self.re = False
         self.books = {}
         self.roots = {}
         self.rules = {}
         self.sorts = []
-        self.limit = 0
+        self.limit = -1
 
         self.PARSE_TEXT_REGEX.sub(self._parse_query, query_text)
         self.roots.setdefault('include', ['root'])
 
         self.markers = {
             'title': [
                 *self.rules.get('tcc', {}).get('include', []),
@@ -125,16 +125,21 @@
                 self.sorts.append(Sort(key='fulltext', subkey=term, order=order))
             elif term in ('title', 'comment', 'source', 'type', 'create', 'modify'):
                 self.sorts.append(Sort(key='meta', subkey=term, order=order))
             else:
                 raise ValueError(f'Invalid sort: {term}')
         elif cmd == 'limit':
             try:
-                self.limit = int(term, 10) if pos else 0
-            except ValueError:
+                if pos:
+                    limit = int(term, 10)
+                    assert limit >= 0
+                    self.limit = limit
+                else:
+                    self.limit = -1
+            except (ValueError, AssertionError):
                 raise ValueError(f'Invalid limit: {term}') from None
         elif cmd in ('id', 'type'):
             inclusion = 'include' if pos else 'exclude'
             value = self._parse_str(term, True)
             self.rules.setdefault(cmd, {}).setdefault(inclusion, []).append(value)
         elif cmd in ('file', 'tc', 'tcc', 'title', 'comment', 'content',
                      'index', 'charset', 'source', 'icon'):
@@ -446,25 +451,22 @@
         """
         for item in self.search():
             self._generate_context(item)
             yield item
 
     def search(self):
         results = self.search_books()
-        if self.query.limit:
-            limit = self.query.limit
-            if limit > 0:
-                i = 0
-                for item in results:
-                    i += 1
-                    if i > limit:
-                        break
-                    yield item
-            else:
-                yield from list(results)[:limit]
+        limit = self.query.limit
+        if limit >= 0:
+            i = 0
+            for item in results:
+                i += 1
+                if i > limit:
+                    break
+                yield item
             return
         yield from results
 
     def search_books(self):
         if self.query.books.setdefault('include', []):
             book_ids = {id: None for id in self.query.books['include'] if id in self.host.books}
         else:
```

### Comparing `webscrapbook-2.0.0b9/webscrapbook/scrapbook/util.py` & `webscrapbook-2.0.1/webscrapbook/scrapbook/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Miscellaneous Scrapbook book handler.
 """
-import copy
-from collections import deque
+from collections import defaultdict, deque
 from contextlib import nullcontext
 
 from . import cache as wsb_cache
 from .host import Host
 
 
 class HostQuery:
@@ -20,17 +19,17 @@
 
         self.host = host
         self.query = query
         self.auto_cache = auto_cache
         self.lock = lock
 
         self.tasks = []
-        self.loads = {}
-        self.changes = {}
-        self.modified = {}
+        self.loads = defaultdict(set)
+        self.changes = defaultdict(set)
+        self.modified = defaultdict(set)
         self.results = []
 
     def run(self):
         for q in self.query:
             book_id = q.get('book', '')
             cmd = q.get('cmd', '')
             args = q.get('args', ())
@@ -49,18 +48,18 @@
             except AttributeError:
                 raise ValueError(f'Invalid command: {cmd!r}') from None
 
             task = (book_id, cmd, func, args, kwargs)
             self.tasks.append(task)
 
             changes = getattr(self, f'_cmd_{cmd}_changes', ())
-            self.changes.setdefault(book_id, set()).update(changes)
+            self.changes[book_id].update(changes)
 
             loads = getattr(self, f'_cmd_{cmd}_loads', changes)
-            self.loads.setdefault(book_id, set()).update(loads)
+            self.loads[book_id].update(loads)
 
             try:
                 prehandler = getattr(self, f'_cmd_{cmd}_prehandler')
             except AttributeError:
                 pass
             else:
                 prehandler(book_id, args, kwargs)
@@ -88,27 +87,27 @@
             if 'meta' in self.loads[book_id]:
                 book.load_meta_files()
 
             if 'toc' in self.loads[book_id]:
                 book.load_toc_files()
 
             if 'meta' in self.changes[book_id]:
-                book_meta_orig = copy.deepcopy(book.meta)
+                book_meta_orig = book.checksum(book.meta)
 
             if 'toc' in self.changes[book_id]:
-                book_toc_orig = copy.deepcopy(book.toc)
+                book_toc_orig = book.checksum(book.toc)
 
             self._with_next_book(book_ids)
 
             if 'meta' in self.changes[book_id]:
-                if book.meta != book_meta_orig:
+                if book.checksum(book.meta) != book_meta_orig:
                     book.save_meta_files()
 
             if 'toc' in self.changes[book_id]:
-                if book.toc != book_toc_orig:
+                if book.checksum(book.toc) != book_toc_orig:
                     book.save_toc_files()
 
     def _run_tasks(self):
         for book_id, cmd, func, args, kwargs in self.tasks:
             try:
                 rv = func(*args, **kwargs)
             except Exception as exc:
@@ -149,24 +148,24 @@
     _cmd_get_item_loads = {'meta', 'toc'}
 
     _cmd_get_items_loads = _cmd_get_item_loads
 
     _cmd_add_item_changes = {'meta', 'toc'}
 
     def _cmd_add_item_posthandler(self, book_id, args, kwargs, rv):
-        self.modified.setdefault(book_id, set()).update(rv)
+        self.modified[book_id].update(rv)
 
     _cmd_add_items_changes = _cmd_add_item_changes
 
     _cmd_add_items_posthandler = _cmd_add_item_posthandler
 
     _cmd_update_item_changes = {'meta'}
 
     def _cmd_update_item_posthandler(self, book_id, args, kwargs, rv):
-        self.modified.setdefault(book_id, set()).update(rv)
+        self.modified[book_id].update(rv)
 
     _cmd_update_items_changes = _cmd_update_item_changes
 
     _cmd_update_items_posthandler = _cmd_update_item_posthandler
 
     _cmd_move_item_loads = {'meta', 'toc'}
 
@@ -185,20 +184,20 @@
     _cmd_link_items_changes = _cmd_link_item_changes
 
     _cmd_copy_item_changes = {'meta', 'toc'}
 
     def _cmd_copy_item_prehandler(self, book_id, args, kwargs):
         target_book_id = kwargs.get('target_book_id')
         if target_book_id not in (None, book_id):
-            self.loads.setdefault(target_book_id, set()).update({'meta', 'toc'})
-            self.changes.setdefault(target_book_id, set()).update({'meta', 'toc'})
+            self.loads[target_book_id].update({'meta', 'toc'})
+            self.changes[target_book_id].update({'meta', 'toc'})
 
     def _cmd_copy_item_posthandler(self, book_id, args, kwargs, rv):
         _, target_book_id, item_ids = rv
-        self.modified.setdefault(target_book_id, set()).update(item_ids)
+        self.modified[target_book_id].update(item_ids)
 
     _cmd_copy_items_changes = _cmd_copy_item_changes
 
     _cmd_copy_items_prehandler = _cmd_copy_item_prehandler
 
     _cmd_copy_items_posthandler = _cmd_copy_item_posthandler
 
@@ -209,15 +208,15 @@
     _cmd_unrecycle_item_changes = {'meta', 'toc'}
 
     _cmd_unrecycle_items_changes = _cmd_unrecycle_item_changes
 
     _cmd_delete_item_changes = {'meta', 'toc'}
 
     def _cmd_delete_item_posthandler(self, book_id, args, kwargs, rv):
-        self.modified.setdefault(book_id, set()).update(rv)
+        self.modified[book_id].update(rv)
 
     _cmd_delete_items_changes = _cmd_delete_item_changes
 
     _cmd_delete_items_posthandler = _cmd_delete_item_posthandler
 
     _cmd_sort_item_loads = {'meta', 'toc'}
 
@@ -228,13 +227,13 @@
     _cmd_sort_items_changes = _cmd_sort_item_changes
 
     _cmd_load_item_postit_loads = {'meta'}
 
     _cmd_save_item_postit_changes = {'meta'}
 
     def _cmd_save_item_postit_posthandler(self, book_id, args, kwargs, rv):
-        self.modified.setdefault(book_id, set()).update(rv)
+        self.modified[book_id].update(rv)
 
     _cmd_add_item_subpage_loads = {'meta'}
 
     def _cmd_add_item_subpage_posthandler(self, book_id, args, kwargs, rv):
-        self.modified.setdefault(book_id, set()).add(rv)
+        self.modified[book_id].add(rv)
```

### Comparing `webscrapbook-2.0.0b9/webscrapbook/server.py` & `webscrapbook-2.0.1/webscrapbook/server.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/en/messages.py` & `webscrapbook-2.0.1/webscrapbook/themes/default/locales/en/messages.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 tools_preview_off = 'Disable preview'
 tools_select_all = 'Select all'
 tools_deselect_all = 'Deselect all'
 tools_expand_all = 'Expand all'
 tools_filter = 'Filter'
 tools_filter_clear = 'Clear filter'
 
+tools_filter_prompt = 'Filter with the keyword (string or "/pattern/flags" for regex):'
+
 command_tooltip = 'Commands [{}]'
 command_mkdir = 'New folder'
 command_mkzip = 'New zip'
 command_mkfile = 'New file'
 command_upload = 'Upload'
 command_uploaddir = 'Upload folder'
 command_source = 'View source'
@@ -35,14 +37,20 @@
 command_edit = 'Edit'
 command_editx = 'Edit page'
 command_move = 'Move'
 command_copy = 'Copy'
 command_link = 'Create link'
 command_delete = 'Delete'
 
+command_mkdir_prompt = 'Create a new folder with name:'
+command_mkdir_default = 'new-folder'
+command_mkzip_prompt = 'Create a ZIP file with name:'
+command_mkzip_default = 'new-archive.zip'
+command_mkfile_prompt = 'Create a file with name:'
+command_mkfile_default = 'new-file.txt'
 command_move_prompt = 'Move to the path or folder:'
 command_move_prompt_multi = 'Move to the folder:'
 command_copy_prompt = 'Copy to the path or folder:'
 command_copy_prompt_multi = 'Copy to the folder:'
 command_link_prompt = 'Create a link at the path or under the folder:'
 command_link_prompt_multi = 'Create links under the folder:'
 
@@ -122,15 +130,15 @@
   • marked: marked items.
   • locked: locked items.
   • location: items with geolocation information.
   • file: items whose filename contains the keyword.
   • root: items under the item of ID. Multiple values are “or”-connected.
   • book: items in the specific scrapbook (by ID). Multiple values are “or”-connected.
   • sort: sort search results using the specific condition, which can be id, title, comment, file, content, source, type, create, or modify. For example, “sort:id -sort:modify” means sorting by ID in acending order and then sorting by modify time in descending order.
-  • limit: set a limit on the search result number. For example, “limit:10” means showing the first 10 results, “limit:-20” means removing the last 20 results, and “limit:0” or “-limit:” means unsetting the limit."""
+  • limit: set a limit on the search result number. For example, “limit:10” means showing the first 10 results. “-limit:” means unsetting the limit."""
 cache_search_result = 'Found %length% results:'
 cache_search_result_named = '(%name%) Found %length% results:'
 cache_search_sort_last_created = 'Last Created'
 cache_search_sort_last_modified = 'Last Modified'
 cache_search_sort_title = 'Sort by title'
 cache_search_sort_id = 'Sort by ID'
 cache_search_confirm_remote = 'Loading remote fulltext cache may require large network flow. Continue?'
```

### Comparing `webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/es/messages.py` & `webscrapbook-2.0.1/webscrapbook/themes/default/locales/es/messages.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/zh/messages.py` & `webscrapbook-2.0.1/webscrapbook/themes/default/locales/zh/messages.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 tools_preview_off = '停用預覽'
 tools_select_all = '全選'
 tools_deselect_all = '取消全選'
 tools_expand_all = '展開所有項目'
 tools_filter = '篩選'
 tools_filter_clear = '清除篩選'
 
+tools_filter_prompt = '用關鍵詞篩選（字串或用「/表示式/標幟」表示正規表示式）:'
+
 command_tooltip = '命令 [{}]'
 command_mkdir = '新資料夾'
 command_mkzip = '新壓縮檔'
 command_mkfile = '新檔案'
 command_upload = '上傳'
 command_uploaddir = '上傳資料夾'
 command_source = '檢視原始碼'
@@ -35,14 +37,20 @@
 command_edit = '編輯'
 command_editx = '編輯頁面'
 command_move = '移動'
 command_copy = '複製'
 command_link = '建立超連結'
 command_delete = '刪除'
 
+command_mkdir_prompt = '建立新資料夾並命名為:'
+command_mkdir_default = 'new-folder'
+command_mkzip_prompt = '建立 ZIP 壓縮檔並命名為:'
+command_mkzip_default = 'new-archive.zip'
+command_mkfile_prompt = '建立檔案並命名為:'
+command_mkfile_default = 'new-file.txt'
 command_move_prompt = '移動至此路徑或資料夾:'
 command_move_prompt_multi = '移動至此資料夾:'
 command_copy_prompt = '複製至此路徑或資料夾:'
 command_copy_prompt_multi = '複製至此資料夾:'
 command_link_prompt = '建立超連結於此路徑或資料夾:'
 command_link_prompt_multi = '建立超連結於此資料夾:'
 
@@ -122,15 +130,15 @@
   • marked：搜尋強調標示的項目。
   • locked：搜尋鎖定的項目。
   • location：搜尋含有地理位置資訊的項目。
   • file：搜尋檔名含有關鍵詞的項目。
   • root：搜尋此 ID 項目下的子項目。多次指定時以「或」連接。
   • book：搜尋指定剪貼簿（依 ID）中的項目。多次指定時以「或」連接。
   • sort：將搜尋結果按指定方式排序，負號表示倒序。可填入 id、title、comment、file、content、source、type、create、modify。例如「sort:id -sort:modify」表示先按 ID 遞增排序再按修改時間遞減排序。
-  • limit：設定搜尋結果筆數限制。例如「limit:10」表示只呈現前 10 筆搜尋結果，「limit:-20」表示不呈現最後 20 筆搜尋結果，「limit:0」或「-limit:」表示移除之前設定的限制。"""
+  • limit：設定搜尋結果筆數限制。例如「limit:10」表示只呈現前 10 筆搜尋結果。「-limit:」表示移除之前設定的限制。"""
 cache_search_result = '找到 %length% 筆結果：'
 cache_search_result_named = '(%name%) 找到 %length% 筆結果：'
 cache_search_sort_last_created = '最後建立'
 cache_search_sort_last_modified = '最後修改'
 cache_search_sort_title = '標題排序'
 cache_search_sort_id = 'ID 排序'
 cache_search_confirm_remote = '載入遠端全文快取可能使用較大的網路流量。要繼續嗎？'
```

### Comparing `webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/zh_cn/messages.py` & `webscrapbook-2.0.1/webscrapbook/themes/default/locales/zh_cn/messages.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 tools_preview_off = '停用预览'
 tools_select_all = '全选'
 tools_deselect_all = '取消全选'
 tools_expand_all = '展开所有项目'
 tools_filter = '筛选'
 tools_filter_clear = '清除筛选'
 
+tools_filter_prompt = '用关键词筛选（字符串或用“/表达式/标帜”表示正则表达式）:'
+
 command_tooltip = '命令 [{}]'
 command_mkdir = '新文件夹'
 command_mkzip = '新压缩文件'
 command_mkfile = '新文件'
 command_upload = '上传'
 command_uploaddir = '上传文件夹'
 command_source = '检视源代码'
@@ -35,14 +37,20 @@
 command_edit = '编辑'
 command_editx = '编辑页面'
 command_move = '移动'
 command_copy = '复制'
 command_link = '建立链接'
 command_delete = '删除'
 
+command_mkdir_prompt = '创建新文件夹并命名为:'
+command_mkdir_default = 'new-folder'
+command_mkzip_prompt = '创建 ZIP 压缩文件并命名为:'
+command_mkzip_default = 'new-archive.zip'
+command_mkfile_prompt = '创建文件并命名为:'
+command_mkfile_default = 'new-file.txt'
 command_move_prompt = '移动至此路径或文件夹:'
 command_move_prompt_multi = '移动至此文件夹:'
 command_copy_prompt = '复制至此路径或文件夹:'
 command_copy_prompt_multi = '复制至此文件夹:'
 command_link_prompt = '建立链接于此路径或文件夹:'
 command_link_prompt_multi = '建立链接于此文件夹:'
 
@@ -122,15 +130,15 @@
   • marked：搜索强调标示的项目。
   • locked：搜索锁定的项目。
   • location：搜索含有地理位置信息的项目。
   • file：搜索文件名含有关键词的项目。
   • root：搜索此 ID 项目下的子项目。多次指定时以“或”连接。
   • book：搜索指定剪贴簿（依 ID）中的项目。多次指定时以“或”连接。
   • sort：将搜索结果按指定方式排序，负号表示倒序。可填入 id、title、comment、file、content、source、type、create、modify。例如“sort:id -sort:modify”表示先按 ID 递增排序再按修改时间递减排序。
-  • limit：设置搜索结果笔数限制。例如“limit:10”表示只呈现前 10 笔搜索结果，“limit:-20”表示不呈现最后 20 笔搜索结果，“limit:0”或“-limit:”表示移除之前设置的限制。"""
+  • limit：设置搜索结果笔数限制。例如“limit:10”表示只呈现前 10 笔搜索结果。“-limit:”表示移除之前设置的限制。"""
 cache_search_result = '找到 %length% 笔结果：'
 cache_search_result_named = '(%name%) 找到 %length% 笔结果：'
 cache_search_sort_last_created = '最后创建'
 cache_search_sort_last_modified = '最后修改'
 cache_search_sort_title = '标题排序'
 cache_search_sort_id = 'ID 排序'
 cache_search_confirm_remote = '加载远程全文缓存可能使用较大的网络流量。要继续吗？'
```

### Comparing `webscrapbook-2.0.0b9/webscrapbook/themes/default/static/comment.png` & `webscrapbook-2.0.1/webscrapbook/themes/default/static/comment.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b9/webscrapbook/themes/default/static/common.css` & `webscrapbook-2.0.1/webscrapbook/themes/default/static/common.css`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b9/webscrapbook/themes/default/static/common.js` & `webscrapbook-2.0.1/webscrapbook/themes/default/static/common.js`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b9/webscrapbook/themes/default/static/edit.css` & `webscrapbook-2.0.1/webscrapbook/themes/default/static/edit.css`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b9/webscrapbook/themes/default/static/edit.js` & `webscrapbook-2.0.1/webscrapbook/themes/default/static/edit.js`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b9/webscrapbook/themes/default/static/editx.js` & `webscrapbook-2.0.1/webscrapbook/themes/default/static/editx.js`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b9/webscrapbook/themes/default/static/external.png` & `webscrapbook-2.0.1/webscrapbook/themes/default/static/external.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b9/webscrapbook/themes/default/static/fclose.png` & `webscrapbook-2.0.1/webscrapbook/themes/default/static/fclose.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b9/webscrapbook/themes/default/static/fopen.png` & `webscrapbook-2.0.1/webscrapbook/themes/default/static/fopen.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b9/webscrapbook/themes/default/static/index-ex.css` & `webscrapbook-2.0.1/webscrapbook/themes/default/static/index-ex.css`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b9/webscrapbook/themes/default/static/index-ex.js` & `webscrapbook-2.0.1/webscrapbook/themes/default/static/index-ex.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1324,15 +1324,15 @@
     },
 
     'expand-all': async function expandAll() {
         await explorer.expandDirs();
     },
 
     'filter': function filter() {
-        const kw = prompt('Filter with the keyword (string or "/pattern/flags" for regex):');
+        const kw = prompt(utils.lang('tools_filter_prompt'));
         if (kw === null) {
             return;
         }
         let regex;
         if (/^\/(.*)\/([a-z]*)$/i.test(kw)) {
             try {
                 regex = new RegExp(RegExp.$1, RegExp.$2);
@@ -1593,15 +1593,15 @@
             });
         } catch (ex) {
             alert(`Unable to browse "${oldPath}": ${ex.message}`);
         }
     },
 
     async mkdir(selectedEntries) {
-        let newPath = prompt('Input a name:', 'new-folder');
+        let newPath = prompt(utils.lang('command_mkdir_prompt'), utils.lang('command_mkdir_default'));
         if (!newPath) {
             return;
         }
 
         const base = document.querySelector('main').dataset.base;
         const dir = document.querySelector('main').dataset.path;
         newPath = dir + newPath;
@@ -1621,15 +1621,15 @@
             alert(`Unable to create directory "${newPath}": ${ex.message}`);
             return;
         }
         location.reload();
     },
 
     async mkzip(selectedEntries) {
-        let newPath = prompt('Input a name:', 'new-archive.zip');
+        let newPath = prompt(utils.lang('command_mkzip_prompt'), utils.lang('command_mkzip_default'));
         if (!newPath) {
             return;
         }
 
         const base = document.querySelector('main').dataset.base;
         const dir = document.querySelector('main').dataset.path;
         newPath = dir + newPath;
@@ -1659,15 +1659,15 @@
             alert(`Unable to create ZIP "${newPath}": ${ex.message}`);
             return;
         }
         location.reload();
     },
 
     async mkfile(selectedEntries) {
-        let newPath = prompt('Input a name:', 'new-file.txt');
+        let newPath = prompt(utils.lang('command_mkfile_prompt'), utils.lang('command_mkfile_default'));
         if (!newPath) {
             return;
         }
 
         const base = document.querySelector('main').dataset.base;
         const dir = document.querySelector('main').dataset.path;
         newPath = dir + newPath;
```

### Comparing `webscrapbook-2.0.0b9/webscrapbook/themes/default/static/index.css` & `webscrapbook-2.0.1/webscrapbook/themes/default/static/index.css`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b9/webscrapbook/themes/default/static/index.js` & `webscrapbook-2.0.1/webscrapbook/themes/default/static/index.js`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b9/webscrapbook/themes/default/static/postit.png` & `webscrapbook-2.0.1/webscrapbook/themes/default/static/postit.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b9/webscrapbook/themes/default/static/search.png` & `webscrapbook-2.0.1/webscrapbook/themes/default/static/search.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b9/webscrapbook/themes/default/static/toggle.png` & `webscrapbook-2.0.1/webscrapbook/themes/default/static/toggle.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/cli.html` & `webscrapbook-2.0.1/webscrapbook/themes/default/templates/cli.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/edit.html` & `webscrapbook-2.0.1/webscrapbook/themes/default/templates/edit.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/editx.html` & `webscrapbook-2.0.1/webscrapbook/themes/default/templates/editx.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/index.html` & `webscrapbook-2.0.1/webscrapbook/themes/default/templates/index.html`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 <link rel="stylesheet" type="text/css" href="{{ static_url('index.css') }}">
 <link rel="stylesheet" type="text/css" href="{{ static_url('index-ex.css') }}">
 {%- endblock %}
 {% block scripts %}
 <script>
 const LANG = {
   label_selected: {{ i18n('label_selected') | tojson }},
+  tools_filter_prompt: {{ i18n('tools_filter_prompt') | tojson }},
+  command_mkdir_prompt: {{ i18n('command_mkdir_prompt') | tojson }},
+  command_mkdir_default: {{ i18n('command_mkdir_default') | tojson }},
+  command_mkzip_prompt: {{ i18n('command_mkzip_prompt') | tojson }},
+  command_mkzip_default: {{ i18n('command_mkzip_default') | tojson }},
+  command_mkfile_prompt: {{ i18n('command_mkfile_prompt') | tojson }},
+  command_mkfile_default: {{ i18n('command_mkfile_default') | tojson }},
   command_move_prompt: {{ i18n('command_move_prompt') | tojson }},
   command_move_prompt_multi: {{ i18n('command_move_prompt_multi') | tojson }},
   command_copy_prompt: {{ i18n('command_copy_prompt') | tojson }},
   command_copy_prompt_multi: {{ i18n('command_copy_prompt_multi') | tojson }},
   command_link_prompt: {{ i18n('command_link_prompt') | tojson }},
   command_link_prompt_multi: {{ i18n('command_link_prompt_multi') | tojson }},
   previewer_toolbar_title: {{ i18n('previewer_toolbar_title') | tojson }},
```

### Comparing `webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/static_frame.html` & `webscrapbook-2.0.1/webscrapbook/themes/default/templates/static_frame.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/static_index.html` & `webscrapbook-2.0.1/webscrapbook/themes/default/templates/static_index.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/static_map.html` & `webscrapbook-2.0.1/webscrapbook/themes/default/templates/static_map.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/static_search.html` & `webscrapbook-2.0.1/webscrapbook/themes/default/templates/static_search.html`

 * *Files 4% similar despite different names*

```diff
@@ -167,15 +167,15 @@
     this.data.meta = Object.assign(this.data.meta, data);
   },
 
   fulltext(data) {
     this.data.fulltext = Object.assign(this.data.fulltext, data);
   },
 
-  init() {
+  async init() {
     document.getElementById('searchForm').addEventListener('submit', (event) => {
       event.preventDefault();
       this.search();
     });
  
     document.getElementById('helper').addEventListener('change', (event) => {
       event.preventDefault();
@@ -187,113 +187,113 @@
       	id,
         toc: {},
         meta: {},
         fulltext: {},
       })
     );
 
-    return this.loadBooks().then(() => {
-      document.getElementById('search').disabled = false;
-    });
+    await this.loadBooks();
+    document.getElementById('search').disabled = false;
   },
 
-  loadBooks() {
-    let p = Promise.resolve();
+  async loadBooks(noCache) {
     for (const book of this.books) {
-      p = p.then(() => {
-        return this.loadBook(book);
-      }).catch((ex) => {
+      try {
+        await this.loadBook(book, noCache);
+      } catch (ex) {
         console.error(ex);
-        this.addMsg("Error: " + ex.message);
-      });
+        this.addMsg(`Error: ${ex.message}`);
+      }
     }
-    return p;
   },
 
-  loadBook(book) {
-    return Promise.resolve().then(() => {
-      let base = this.resolveUrl(book.path, location.href);
-
-      const loadMeta = () => {
-        const loop = () => {
-          const url = this.resolveUrl(book.treeDir + "meta" + (i || "") + ".js", base);
-          return this.loadScript(url, true).then(() => {
-            i += 1;
-            return loop();
-          }).catch((ex) => {
-            if (i === 0) { throw ex; }
-            console.log("Unable to load '" + url + "'");
-          });
-        };
-
-        let i = 0;
-        return loop();
-      };
-
-      const loadToc = () => {
-        const loop = () => {
-          const url = this.resolveUrl(book.treeDir + "toc" + (i || "") + ".js", base);
-          return this.loadScript(url, true).then(() => {
-            i += 1;
-            return loop();
-          }).catch((ex) => {
-            if (i === 0) { throw ex; }
-            console.log("Unable to load '" + url + "'");
-          });
-        };
+  async loadBook(book, noCache) {
+    const base = this.resolveUrl(book.path, location.href);
 
-        let i = 0;
-        return loop();
-      };
-
-      const loadFulltext = () => {
-        const loop = () => {
-          const url = this.resolveUrl(book.treeDir + "fulltext" + (i || "") + ".js", base);
-          return this.loadScript(url, true).then(() => {
-            i += 1;
-            return loop();
-          }).catch((ex) => {
-            console.log("Unable to load '" + url + "'");
-          });
-        };
+    const loadMeta = async () => {
+      let i = 0;
+      while (true) {
+        const url = this.resolveUrl(`${book.treeDir}meta${i || ''}.js`, base);
+        try {
+          await this.loadScript(url, noCache);
+        } catch (ex) {
+          if (i === 0) { throw ex; }
+          console.debug(`Unable to load '${url}'`);
+          break;
+        }
+        i++;
+      }
+    };
 
-        let i = 0;
-        return loop();
-      };
+    const loadToc = async () => {
+      let i = 0;
+      while (true) {
+        const url = this.resolveUrl(`${book.treeDir}toc${i || ''}.js`, base);
+        try {
+          await this.loadScript(url, noCache);
+        } catch (ex) {
+          if (i === 0) { throw ex; }
+          console.debug(`Unable to load '${url}'`);
+          break;
+        }
+        i++;
+      }
+    };
 
-      scrapbook.data = book;
-      if (!this.checkHttp(base)) {
-        this.addMsg("Rejected to load remote fulltext cache: " + base);
-        return Promise.all([
-          loadMeta(),
-          loadToc(),
-        ]);
-      } else {
-        return Promise.all([
-          loadMeta(),
-          loadToc(),
-          loadFulltext(),
-        ]);
+    const loadFulltext = async () => {
+      let i = 0;
+      while (true) {
+        const url = this.resolveUrl(`${book.treeDir}fulltext${i || ''}.js`, base);
+        try {
+          await this.loadScript(url, noCache);
+        } catch (ex) {
+          if (i === 0) {
+            console.log(`Unable to load '${url}'`);
+          } else {
+            console.debug(`Unable to load '${url}'`);
+          }
+          break;
+        }
+        i++;
       }
-    });
+    };
+
+    scrapbook.data = book;
+    if (!this.checkHttp(base)) {
+      this.addMsg(`Rejected to load remote fulltext cache: ${base}`);
+      return Promise.all([
+        loadMeta(),
+        loadToc(),
+      ]);
+    } else {
+      return Promise.all([
+        loadMeta(),
+        loadToc(),
+        loadFulltext(),
+      ]);
+    }
   },
 
-  loadScript(url, noCache) {
+  async loadScript(url, noCache) {
     return new Promise((resolve, reject) => {
+      url = new URL(url);
+      if (noCache) {
+        url.searchParams.append('ts', Date.now());
+      }
       const elem = document.createElement("script");
       document.getElementsByTagName("head")[0].appendChild(elem);
       elem.onload = (event) => {
-        console.log("Loaded '" + url + "'");
+        console.log(`Loaded '${url}'`);
         resolve();
       };
       elem.onerror = (event) => {
         elem.remove();
-        reject(new Error("Failed to load '" + url + "'"));
+        reject(new Error(`Failed to load '${url}'`));
       };
-      elem.src = url + (noCache ? "?ts=" + Date.now() : "");
+      elem.src = url;
     });
   },
 
   checkHttp(url) {
     const targetUrl = this.resolveUrl(url, location.href);
     const targetUrlObj = new URL(targetUrl);
     if (['http:', 'https:'].indexOf(targetUrlObj.protocol) !== -1 &&
@@ -307,40 +307,40 @@
       }
       if (conf.allowHttp > 0) { return true; }
       return false;
     }
     return true;
   },
 
-  search() {
-    return Promise.resolve().then(() => {
+  async search() {
+    try {
       this.clearResult();
 
       // set query string
       let queryStr = document.getElementById("keyword").value;
       if (conf.defaultSearch) {
         queryStr = conf.defaultSearch + " " + queryStr;
       }
 
       // parse query
       const query = searchEngine.parseQuery(queryStr);
       if (query.error.length) {
         for (const err of query.error) {
-          this.addMsg("Error: " + err);
+          this.addMsg(`Error: ${err}`);
         }
         return;
       }
-      console.log("Search:", query);
 
-      // search and get result
-      return searchEngine.search(query);
-    }).catch((ex) => {
+      // search and show results
+      console.log("Search:", query);
+      await searchEngine.search(query, this.showResults.bind(this));
+    } catch (ex) {
       console.error(ex);
-      this.addMsg("Error: " + ex.message);
-    });
+      this.addMsg(`Error: ${ex.message}`);
+    }
   },
 
   showResults(results, book) {
     const info = {
       "": "%",
       name: book.name,
       length: results.length,
@@ -490,15 +490,15 @@
   },
 
   parseQuery(queryStr) {
     const query = {
       error: [],
       rules: {},
       sorts: [],
-      limit: 0,
+      limit: -1,
       books: {
         include: [],
         exclude: [],
       },
       roots: {
         include: [],
         exclude: [],
@@ -524,30 +524,30 @@
           query.sorts.push({key: "fulltext", subkey: key, order});
           break;
         case "title": case "comment": case "source":
         case "type": case "create": case "modify":
           query.sorts.push({key: "meta", subkey: key, order});
           break;
         default:
-          addError("Invalid sort: " + key);
+          addError(`Invalid sort: ${key}`);
           break;
       }
     };
 
     const setLimit = (value, positive) => {
       if (!positive) {
-        query.limit = 0;
+        query.limit = -1;
         return; 
       }
 
       const newValue = parseInt(value, 10);
-      if (Number.isInteger(newValue)) {
+      if (newValue >= 0) {
         query.limit = newValue;
       } else {
-        addError("Invalid limit: " + value);
+        addError(`Invalid limit: ${value}`);
       }
     };
 
     const addError = (msg) => {
       query.error.push(msg);
     };
 
@@ -555,29 +555,29 @@
       let flags = query.mc ? "m" : "im";
       if (this.supportRegexUnicodeFlag) { flags += "u"; }
       let regex = "";
       if (query.re) {
         try {
           regex = new RegExp(term, flags);
         } catch(ex) {
-          addError("Invalid RegExp: " + term);
+          addError(`Invalid RegExp: ${term}`);
           return null;
         }
       } else {
         let key = scrapbook.escapeRegExp(term);
         if (exactMatch) { key = "^" + key + "$"; }
         regex = new RegExp(key, flags);
       }
       return regex;
     };
 
     const parseDate = (term) => {
       const match = term.match(/^(\d{0,17})(?:-(\d{0,17}))?$/);
       if (!match) {
-        addError("Invalid date format: " + term);
+        addError(`Invalid date format: ${term}`);
         return null;
       }
       const since = match[1] ? this.idLocalToUtc(pad(match[1], 17)) : pad("", 17);
       const until = match[2] ? this.idLocalToUtc(pad(match[2], 17)) : pad("", 17, "9");
       return [since, until];
     };
 
@@ -680,98 +680,92 @@
       }
 
       return "";
     });
     return query;
   },
 
-  search(query) {
+  async search(query, callback) {
   	let books = new Set(scrapbook.books);
   	if (query.books.include.length) {
   	  books = new Set(
         query.books.include
           .map(id => conf.scrapbooks[id])
           .filter(book => books.has(book))
       );
   	}
     for (const book of books) {
       if (query.books.exclude.includes(book.id)) {
         books.delete(book);
       }
     }
 
-    let p = Promise.resolve();
-    books.forEach((book) => {
-      p = p.then(() => {
-        return this.searchBook(query, book).then((results) => {
-          scrapbook.showResults(results, book);
-        });
-      });
-    });
-    return p;
+    for (const book of books) {
+      const results = this.searchBook(query, book);
+      callback(results, book);
+    }
   },
 
   searchBook(query, book) {
-    return Promise.resolve().then(() => {
-      const results = [];
+    const results = [];
 
-      const idPool = new Set();
-      {
-        if (!query.roots.include.length) {
-          query.roots.include.push('root');
-        }
+    const idPool = new Set();
+    {
+      if (!query.roots.include.length) {
+        query.roots.include.push('root');
+      }
 
-        for (const root of query.roots.include) {
-          for (const id of this.getReachableItems(book, root)) {
-            idPool.add(id);
-          }
+      for (const root of query.roots.include) {
+        for (const id of this.getReachableItems(book, root)) {
+          idPool.add(id);
         }
+      }
 
-        for (const root of query.roots.exclude) {
-          for (const id of this.getReachableItems(book, root)) {
-            idPool.delete(id);
-          }
+      for (const root of query.roots.exclude) {
+        for (const id of this.getReachableItems(book, root)) {
+          idPool.delete(id);
         }
       }
+    }
 
-      for (const id of idPool) {
-        let subfiles = book.fulltext[id] || {};
-        if (!Object.keys(subfiles).length) { subfiles[""] = {}; }
-
-        for (const file in subfiles) {
-          const item = {
-            id,
-            file,
-            meta: book.meta[id],
-            fulltext: subfiles[file],
-          };
-          if (this.matchItem(item, query)) {
-            results.push(item);
-          }
+    for (const id of idPool) {
+      let subfiles = book.fulltext[id] || {};
+      if (!Object.keys(subfiles).length) { subfiles[""] = {}; }
+
+      for (const file in subfiles) {
+        const item = {
+          id,
+          file,
+          meta: book.meta[id],
+          fulltext: subfiles[file],
+        };
+        if (this.matchItem(item, query)) {
+          results.push(item);
         }
       }
+    }
 
-      // sort results
-      for (const {key, subkey, order} of query.sorts) {
-        results.sort((a, b) => {
-          a = a[key]; if (subkey) { a = a[subkey]; } a = a || "";
-          b = b[key]; if (subkey) { b = b[subkey]; } b = b || "";
-          if (a > b) { return order; }
-          if (a < b) { return -order; }
-          return 0;
-        });
-      }
-
-      // limit results
-      if (query.limit) {
-        results.splice(query.limit);
-      }
+    // sort results
+    for (const {key, subkey, order} of query.sorts) {
+      results.sort((a, b) => {
+        a = a[key]; if (subkey) { a = a[subkey]; } a = a || "";
+        b = b[key]; if (subkey) { b = b[subkey]; } b = b || "";
+        if (a > b) { return order; }
+        if (a < b) { return -order; }
+        return 0;
+      });
+    }
 
-      return results;
-    });
+    // limit results
+    if (query.limit >= 0) {
+      results.splice(query.limit);
+      query.limit -= results.length;
+    }
+
+    return results;
   },
 
   getReachableItems(book, root, set = new Set()) {
     const addIdRecursively = (id) => {
       for (const refId of book.toc[id]) {
         if (book.meta[refId] && !set.has(refId)) {
           set.add(refId);
@@ -987,14 +981,15 @@
     <option value="marked:">marked:</option>
     <option value="locked:">locked:</option>
     <option value="location:">location:</option>
     <option value="re:">re:</option>
     <option value="mc:">mc:</option>
     <option value="file:">file:</option>
     <option value="root:">root:</option>
+    <option value="limit:">limit:</option>
     <option value="sort:">sort:</option>
     <option value="-sort:modify">{{ i18n('cache_search_sort_last_modified') }}</option>
     <option value="-sort:create">{{ i18n('cache_search_sort_last_created') }}</option>
     <option value="sort:title">{{ i18n('cache_search_sort_title') }}</option>
     <option value="sort:id">{{ i18n('cache_search_sort_id') }}</option>
   </select>
   <input id="search" type="submit" value="{{ i18n('cache_search_start') }}" disabled autocomplete="off">
```

#### html2text {}

```diff
@@ -15,14 +15,15 @@
 marked:
 locked:
 location:
 re:
 mc:
 file:
 root:
+limit:
 sort:
 {{ i18n('cache_search_sort_last_modified') }}
 {{ i18n('cache_search_sort_last_created') }}
 {{ i18n('cache_search_sort_title') }}
 {{ i18n('cache_search_sort_id') }}
  [{{ i18n('cache_search_start') }}]
  {{ i18n('cache_search_help_label') }}
```

### Comparing `webscrapbook-2.0.0b9/webscrapbook/util/css.py` & `webscrapbook-2.0.1/webscrapbook/util/css.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b9/webscrapbook/util/fs.py` & `webscrapbook-2.0.1/webscrapbook/util/fs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Virtual filesystem for complex file operation."""
 import copy as _copy
 import functools
 import io
 import itertools
 import os
-import re
 import shutil
 import stat
 import subprocess
 import sys
 import tempfile
 import time
 from contextlib import contextmanager, nullcontext
@@ -186,26 +185,26 @@
     def __getitem__(self, key):
         return self._path[key]
 
     def __eq__(self, other):
         return self._path == other
 
     def copy(self):
-        return CPath(self._path)
+        return self.__class__(self._path)
 
     @property
     def path(self):
         return self._path
 
     @property
     def file(self):
         return self._path[0]
 
-    @staticmethod
-    def resolve(plainpath, resolver=None):
+    @classmethod
+    def resolve(cls, plainpath, resolver=None):
         """Resolves a plainpath with '!/' to a CPath.
 
         - Priority:
           entry.zip!/entry1.zip!/ = entry.zip!/entry1.zip! >
           entry.zip!/entry1.zip >
           entry.zip!/ = entry.zip! >
           entry.zip
@@ -217,18 +216,18 @@
             plainpath: a path string that may contain '!/'
             resolver: a function that resolves a path to real filesystem path
 
         Returns:
             CPath
         """
         paths = []
-        for m in reversed(list(re.finditer(r'!/', plainpath, flags=re.I))):
-            archivepath = plainpath[:m.start(0)]
+        for start, end in cls._resolve_iter_sep(plainpath):
+            archivepath = plainpath[:start]
             if resolver:
-                archivepath = CPath._resolve_tidy_subpath(archivepath)
+                archivepath = cls._resolve_tidy_subpath(archivepath)
                 archivefile = resolver(archivepath)
             else:
                 archivepath = archivefile = os.path.normpath(archivepath)
             conflicting = archivefile + '!'
 
             if os.path.lexists(conflicting):
                 break
@@ -238,29 +237,29 @@
             try:
                 zh = zipfile.ZipFile(archivefile, 'r')
             except (zipfile.BadZipFile, FileNotFoundError, NotADirectoryError):
                 continue
 
             with zh as zh:
                 paths.append(archivepath)
-                CPath._resolve_add_subpath(paths, zh, plainpath[m.end(0):])
-                return CPath(paths)
+                cls._resolve_add_subpath(paths, zh, plainpath[end:])
+                return cls(paths)
 
         archivepath = plainpath
         if resolver:
-            archivepath = CPath._resolve_tidy_subpath(archivepath)
+            archivepath = cls._resolve_tidy_subpath(archivepath)
         else:
             archivepath = os.path.normpath(archivepath)
         paths.append(archivepath)
-        return CPath(paths)
+        return cls(paths)
 
-    @staticmethod
-    def _resolve_add_subpath(paths, zh, subpath):
-        for m in reversed(list(re.finditer(r'!/', subpath, flags=re.I))):
-            archivepath = CPath._resolve_tidy_subpath(subpath[:m.start(0)], True)
+    @classmethod
+    def _resolve_add_subpath(cls, paths, zh, subpath):
+        for start, end in cls._resolve_iter_sep(subpath):
+            archivepath = cls._resolve_tidy_subpath(subpath[:start], True)
             conflicting = archivepath + '!/'
 
             if any(i.startswith(conflicting) for i in zh.namelist()):
                 break
 
             try:
                 fh = zh.open(archivepath)
@@ -271,21 +270,31 @@
                 try:
                     zh1 = zipfile.ZipFile(fh)
                 except zipfile.BadZipFile:
                     continue
 
                 with zh1 as zh1:
                     paths.append(archivepath)
-                    CPath._resolve_add_subpath(paths, zh1, subpath[m.end(0):])
+                    cls._resolve_add_subpath(paths, zh1, subpath[end:])
                     return
 
-        paths.append(CPath._resolve_tidy_subpath(subpath, True))
+        paths.append(cls._resolve_tidy_subpath(subpath, True))
 
-    @staticmethod
-    def _resolve_tidy_subpath(path, striproot=False):
+    @classmethod
+    def _resolve_iter_sep(cls, path):
+        pos = None
+        while True:
+            try:
+                pos = path.rindex('!/', 0, pos)
+            except ValueError:
+                break
+            yield pos, pos + 2
+
+    @classmethod
+    def _resolve_tidy_subpath(cls, path, striproot=False):
         """Tidy a subpath with possible '.', '..', '//', etc."""
         has_initial_slash = path.startswith('/')
         comps = path.split('/')
         new_comps = []
         for comp in comps:
             if comp in ('', '.'):
                 continue
@@ -963,45 +972,43 @@
         for path in zh.namelist():
             if path.startswith(base):
                 return ZIP_SUBPATH_DIR_IMPLICIT
 
     return ZIP_SUBPATH_NONE
 
 
-def zip_compress(zip, filename, subpath, filter=None, *, buffer_size=io.DEFAULT_BUFFER_SIZE):
+def zip_compress(zip, filename, subpath, filter=None, *,
+                 stream=None, buffer_size=io.DEFAULT_BUFFER_SIZE):
     """Compress src to be the subpath in the zip.
 
     Args:
-        zip: path, file-like object, or zipfile.ZipFile, or None to generate
-            bytes of the output ZIP file
+        zip: path, file-like object, or zipfile.ZipFile
         filename: path of the source file or directory
         subpath: internal path to a file or folder (without trailing slash)
         filter: an iterable of permitted subentries if filename is a directory
             (with normcase'd absolute path)
+        stream: a ZipStream for streaming output
 
     Raises:
         shutil.Error: if any child file cannot be added to the zip
     """
     filename = os.path.abspath(filename)
 
-    if zip is None:
-        zs = ZipStream()
-        cm = zipfile.ZipFile(zs, 'w')
-        return _zip_compress_gen(cm, filename, subpath, filter,
-                                 stream=zs, buffer_size=buffer_size)
-
     if isinstance(zip, zipfile.ZipFile):
-        zs = None
         cm = nullcontext(zip)
     else:
-        zs = None
         cm = zipfile.ZipFile(zip, 'w')
 
-    for _ in _zip_compress_gen(cm, filename, subpath, filter,
-                               buffer_size=buffer_size):
+    gen = _zip_compress_gen(cm, filename, subpath, filter,
+                            stream=stream, buffer_size=buffer_size)
+
+    if stream is not None:
+        return gen
+
+    for _ in gen:
         pass
 
 
 def _zip_compress_gen(zh, filename, subpath, filter, *,
                       stream=None, buffer_size=io.DEFAULT_BUFFER_SIZE):
     with zh as zh:
         errors = []
@@ -1063,52 +1070,48 @@
             # determine target subpath as dst
             dst = util.unify_pathsep(src[cut:])
             dst = subpath + dst
 
             yield src, dst
 
 
-def zip_copy(zsrc, base, zdst, subpath, filter=None, *, buffer_size=io.DEFAULT_BUFFER_SIZE):
+def zip_copy(zsrc, base, zdst, subpath, filter=None, *,
+             stream=None, buffer_size=io.DEFAULT_BUFFER_SIZE):
     """Coopy entries from zsrc to be the subpath in zdst.
 
     Args:
         zsrc: path, file-like object, or zipfile.ZipFile
         base: internal path to a file or folder (without trailing slash)
-        zdst: path, file-like object, or zipfile.ZipFile, or None to generate
-            bytes of the output ZIP file
+        zdst: path, file-like object, or zipfile.ZipFile
         subpath: internal path to a file or folder (without trailing slash)
         filter: an iterable of permitted subentries if zsrcpath is a directory
             (without trailing slash)
+        stream: a ZipStream for streaming output
 
     Returns:
         set: names that are copied
     """
     base = base.rstrip('/')
-    if zdst is None:
-        zs = ZipStream()
-        cm = zipfile.ZipFile(zs, 'w')
-        return _zip_copy_gen(zsrc, base, cm, subpath, filter,
-                             stream=zs, buffer_size=buffer_size)
 
     if isinstance(zdst, zipfile.ZipFile):
         cm = nullcontext(zdst)
     else:
         cm = zipfile.ZipFile(zdst, 'w')
 
-    copied = None
-
-    def gen():
-        nonlocal copied
-        copied = yield from _zip_copy_gen(zsrc, base, cm, subpath, filter,
-                                          buffer_size=buffer_size)
+    gen = _zip_copy_gen(zsrc, base, cm, subpath, filter,
+                        stream=stream, buffer_size=buffer_size)
 
-    for _ in gen():
-        pass
+    if stream is not None:
+        return gen
 
-    return copied
+    try:
+        while True:
+            next(gen)
+    except StopIteration as exc:
+        return exc.value
 
 
 def _zip_copy_gen(zsrc, base, zdst, subpath, filter=None, *,
                   stream=None, buffer_size=io.DEFAULT_BUFFER_SIZE):
     copied = set()
     with nullcontext(zsrc) if isinstance(zsrc, zipfile.ZipFile) else zipfile.ZipFile(zsrc) as zi,\
          zdst as zh:
@@ -1205,18 +1208,20 @@
 
             # extract entries and recover mtime
             zh.extractall(tempdir, entries)
             for entry in entries:
                 file = os.path.join(tempdir, entry)
                 zinfo = zh.getinfo(entry)
 
+                # @FIXME: utcoffset may be different across timestamps when DST
+                #         is used
                 ts = zip_timestamp(zinfo)
                 if tzoffset is not None:
-                    delta = datetime.now().astimezone().utcoffset().total_seconds()
-                    ts = ts - tzoffset + delta
+                    utcoffset = datetime.fromtimestamp(ts).astimezone().utcoffset().total_seconds()
+                    ts = ts + utcoffset - tzoffset
                 os.utime(file, (ts, ts))
 
                 # @TODO: recover mode?
                 # It may be ignored in some OS and setting the mode for a file
                 # can prevent another file from being set.
 
         # move to target path
```

### Comparing `webscrapbook-2.0.0b9/webscrapbook/util/html.py` & `webscrapbook-2.0.1/webscrapbook/util/html.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b9/webscrapbook/util/util.py` & `webscrapbook-2.0.1/webscrapbook/util/util.py`

 * *Files 9% similar despite different names*

```diff
@@ -569,28 +569,25 @@
 
     Args:
         file: str, path-like, or file-like bytes object
     """
     try:
         fh = open(file, 'rb')
     except TypeError:
-        fh = file
+        fh = nullcontext(file)
 
-    try:
+    with fh as fh:
         h = hashlib.new(method)
         while True:
             chunk = fh.read(chunk_size)
             if not chunk:
                 break
             h.update(chunk)
 
         return h.hexdigest()
-    finally:
-        if fh != file:
-            fh.close()
 
 
 def format_filesize(bytes, si=False, space=' '):
     """Convert file size from bytes to human readable presentation.
     """
     try:
         bytes = int(bytes)
@@ -878,20 +875,20 @@
         none_from_bom: True to return None if charset is determined from BOM
             (to prevent error for lxml)
         quickly: True to exit early for normal HTML files
     """
     try:
         fh = open(file, 'rb')
     except TypeError:
-        fh = file
+        fh = nullcontext(file)
     except FileNotFoundError:
         fh = None
 
     if fh:
-        try:
+        with fh as fh:
             # Seek for the correct charset (encoding).
             # If a charset is not specified, lxml may select a wrong encoding for
             # the entire document if there is text before first meta charset.
             charset = sniff_bom(fh)
             if charset:
                 if none_from_bom:
                     # lxml does not accept "UTF-16-LE" or so, but can auto-detect
@@ -906,49 +903,43 @@
             if charset is None:
                 charset = default
 
             if charset is not None:
                 charset = fix_codec(charset)
 
             return charset
-        finally:
-            if fh != file:
-                fh.close()
 
     return default
 
 
 def load_html_tree(file, options=None):
     """Load HTML document tree.
 
     Args:
         file: str, path-like, or file-like bytes object
         options: additional options for the HTML parser
     """
     try:
         fh = open(file, 'rb')
     except TypeError:
-        fh = file
+        fh = nullcontext(file)
     except FileNotFoundError:
         fh = None
 
     if not fh:
         return None
 
-    try:
+    with fh as fh:
         charset = get_html_charset(fh)
         fh.seek(0)
 
         try:
             return lxml.html.parse(fh, lxml.html.HTMLParser(encoding=charset, **(options or {})))
         except etree.Error:
             return None
-    finally:
-        if fh != file:
-            fh.close()
 
 
 MetaRefreshInfo = namedtuple('MetaRefreshInfo', ('time', 'target', 'context'))
 
 # ref: https://html.spec.whatwg.org/multipage/semantics.html#attr-meta-http-equiv-refresh
 META_REFRESH_REGEX = re.compile(r"""
     ^
@@ -1035,22 +1026,22 @@
     Args:
         file: str, path-like, or file-like bytes object
         encoding: encoding for the HTML file
     """
     try:
         fh = open(file, 'rb')
     except TypeError:
-        fh = file
+        fh = nullcontext(file)
     except FileNotFoundError:
         fh = None
 
     if not fh:
         return
 
-    try:
+    with fh as fh:
         if not encoding:
             encoding = get_html_charset(fh, default='ISO-8859-1')
             fh.seek(0)
 
         contexts = []
         for event, elem in etree.iterparse(fh, encoding=encoding, html=True, events=('start', 'end')):
             if event == 'start':
@@ -1070,17 +1061,14 @@
                 elem.clear()
                 while elem.getprevious() is not None:
                     try:
                         del elem.getparent()[0]
                     except TypeError:
                         # broken html may generate extra root elem
                         break
-    finally:
-        if fh != file:
-            fh.close()
 
 
 def get_meta_refresh(file):
     """Retrieve a general redirect-like meta refresh from a file.
 
     According to spec, the document should take only the first meta refresh.
     This is also more performant. Though many browsers accept multiple meta
@@ -1217,60 +1205,7 @@
     return MaffPageInfo(
         load_attr('title'),
         load_attr('originalurl'),
         load_attr('archivetime'),
         load_attr('indexfilename'),
         load_attr('charset'),
     )
-
-
-#########################################################################
-# Encrypt and security
-#########################################################################
-
-class Encrypt():
-    """Simple hash encryption with salt.
-    """
-    def md5(self, text, salt=''):
-        return hashlib.md5((text + salt).encode('UTF-8')).hexdigest()
-
-    def sha1(self, text, salt=''):
-        return hashlib.sha1((text + salt).encode('UTF-8')).hexdigest()
-
-    def sha224(self, text, salt=''):
-        return hashlib.sha224((text + salt).encode('UTF-8')).hexdigest()
-
-    def sha256(self, text, salt=''):
-        return hashlib.sha256((text + salt).encode('UTF-8')).hexdigest()
-
-    def sha384(self, text, salt=''):
-        return hashlib.sha384((text + salt).encode('UTF-8')).hexdigest()
-
-    def sha512(self, text, salt=''):
-        return hashlib.sha512((text + salt).encode('UTF-8')).hexdigest()
-
-    def sha3_224(self, text, salt=''):
-        return hashlib.sha3_224((text + salt).encode('UTF-8')).hexdigest()
-
-    def sha3_256(self, text, salt=''):
-        return hashlib.sha3_256((text + salt).encode('UTF-8')).hexdigest()
-
-    def sha3_384(self, text, salt=''):
-        return hashlib.sha3_384((text + salt).encode('UTF-8')).hexdigest()
-
-    def sha3_512(self, text, salt=''):
-        return hashlib.sha3_512((text + salt).encode('UTF-8')).hexdigest()
-
-    def plain(self, text, salt=''):
-        return text + salt
-
-    def encrypt(self, text, salt='', method='plain'):
-        fn = getattr(self, method, None)
-
-        if not callable(fn):
-            print(f"Encrypt method {method!r} not implemented, fallback to 'plain'.", file=sys.stderr)
-            fn = self.plain
-
-        return fn(text, salt)
-
-
-encrypt = Encrypt().encrypt
```

### Comparing `webscrapbook-2.0.0b9/webscrapbook.egg-info/PKG-INFO` & `webscrapbook-2.0.1/webscrapbook.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscrapbook
-Version: 2.0.0b9
+Version: 2.0.1
 Summary: A backend toolkit for management of WebScrapBook collection.
 Home-page: https://github.com/danny0838/PyWebScrapBook
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

### Comparing `webscrapbook-2.0.0b9/webscrapbook.egg-info/SOURCES.txt` & `webscrapbook-2.0.1/webscrapbook.egg-info/SOURCES.txt`

 * *Files identical despite different names*

