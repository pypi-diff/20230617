# Comparing `tmp/plib3.ui-0.15.8.1.tar.gz` & `tmp/plib3.ui-0.15.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/pdonis/git/plib3-ui/dist/tmpupr5yj4z/plib3.ui-0.15.8.1.tar", last modified: Thu May 18 02:31:21 2023, max compression
+gzip compressed data, was "/home/pdonis/git/plib3-ui/dist/tmpipi030ti/plib3.ui-0.15.8.2.tar", last modified: Sat Jun 17 03:08:51 2023, max compression
```

## Comparing `plib3.ui-0.15.8.1.tar` & `plib3.ui-0.15.8.2.tar`

### file list

```diff
@@ -1,336 +1,336 @@
-drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-05-18 02:31:21.000000 plib3.ui-0.15.8.1/
-drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-05-18 02:31:20.000000 plib3.ui-0.15.8.1/plib/
-drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-05-18 02:31:21.000000 plib3.ui-0.15.8.1/plib/ui/
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     6745 2022-07-09 05:35:22.000000 plib3.ui-0.15.8.1/plib/ui/prefs.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     2576 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/custom.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)      266 2023-05-18 02:02:46.000000 plib3.ui-0.15.8.1/plib/ui/__init__.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     2319 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/dialogs.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     2422 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/socket.py
-drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-05-18 02:31:21.000000 plib3.ui-0.15.8.1/plib/ui/base/
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     3333 2022-07-09 05:25:43.000000 plib3.ui-0.15.8.1/plib/ui/base/button.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)      529 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/base/mouse.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     2928 2022-07-10 03:01:32.000000 plib3.ui-0.15.8.1/plib/ui/base/tabwidget.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     1396 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/base/display.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)    14312 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/base/helpers.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     1684 2022-07-09 05:25:43.000000 plib3.ui-0.15.8.1/plib/ui/base/listbox.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      245 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/base/__init__.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      951 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/base/socket.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     3554 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/base/form.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     1966 2022-07-10 03:01:58.000000 plib3.ui-0.15.8.1/plib/ui/base/groupbox.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      954 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/base/container.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     7962 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/base/mainwin.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     3991 2022-07-30 18:34:01.000000 plib3.ui-0.15.8.1/plib/ui/base/group.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     5378 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/base/table.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     5506 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/base/editctrl.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     8681 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/base/listview.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)    24031 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/base/app.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     3462 2022-07-10 04:27:02.000000 plib3.ui-0.15.8.1/plib/ui/base/pagewidget.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      936 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/base/label.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     2539 2022-07-09 05:25:43.000000 plib3.ui-0.15.8.1/plib/ui/base/combo.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     1302 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/base/scroller.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     1500 2022-01-09 05:35:26.000000 plib3.ui-0.15.8.1/plib/ui/base/imageview.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)      409 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/base/focus.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     2445 2022-07-10 03:03:14.000000 plib3.ui-0.15.8.1/plib/ui/base/dialog.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)    15014 2022-07-30 18:34:01.000000 plib3.ui-0.15.8.1/plib/ui/widgets.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     8231 2022-07-30 18:34:01.000000 plib3.ui-0.15.8.1/plib/ui/defs.py
-drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-05-18 02:31:21.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     3733 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/__init__.py
-drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-05-18 02:31:21.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     2381 2022-07-09 05:25:43.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/button.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     1625 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/mouse.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     1638 2022-07-10 01:46:10.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/tabwidget.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     1421 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/display.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     2365 2022-07-09 05:25:43.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/listbox.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      313 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/__init__.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     2139 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/socket.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     3238 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/form.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1499 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/groupbox.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1084 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/container.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     4799 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/mainwin.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     2150 2022-07-30 18:34:01.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/group.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     5049 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/table.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2581 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/header.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     5219 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/editctrl.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     5232 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/listview.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)    16030 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/app.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     1513 2022-07-10 01:39:26.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/pagewidget.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      922 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/label.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2926 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/combo.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     1541 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/scroller.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     2292 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/imageview.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)      806 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/focus.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1140 2022-07-10 03:03:29.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/dialog.py
-drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-05-18 02:31:21.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/wx/
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     2392 2022-07-09 05:25:43.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/wx/button.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     1654 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/wx/mouse.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1515 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/wx/tabwidget.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1353 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/wx/display.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     2204 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/wx/listbox.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      310 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/wx/__init__.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     3407 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/wx/socket.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     4496 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/wx/form.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2701 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/wx/groupbox.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     7166 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/wx/mainwin.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     3948 2022-07-30 18:34:01.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/wx/group.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     8564 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/wx/table.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     7366 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/wx/editctrl.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     8487 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/wx/listview.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)    25325 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/wx/app.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     1452 2022-07-09 05:25:43.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/wx/pagewidget.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      957 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/wx/label.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2624 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/wx/combo.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     1694 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/wx/scroller.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     2623 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/wx/imageview.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)      489 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/wx/focus.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     1737 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/wx/dialog.py
-drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-05-18 02:31:21.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     2587 2022-07-09 05:25:43.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/button.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     1562 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/mouse.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     1711 2022-07-10 01:46:58.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/tabwidget.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     1512 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/display.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     2493 2022-07-09 05:25:43.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/listbox.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      305 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/__init__.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1632 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/socket.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     3228 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/form.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1582 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/groupbox.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1078 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/container.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     4973 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/mainwin.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     2161 2022-07-30 18:34:01.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/group.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     5120 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/table.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2563 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/header.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     5852 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/editctrl.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     5548 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/listview.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)    16633 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/app.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     1590 2022-07-10 01:40:06.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/pagewidget.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1003 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/label.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     3092 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/combo.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     1531 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/scroller.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     2128 2022-01-09 05:35:26.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/imageview.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)      743 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/focus.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1223 2022-07-10 03:03:35.000000 plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/dialog.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     1888 2022-04-21 04:56:54.000000 plib3.ui-0.15.8.1/plib/ui/textfile.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     1767 2022-07-09 05:25:43.000000 plib3.ui-0.15.8.1/plib/ui/coll.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     1312 2022-05-28 05:28:12.000000 plib3.ui-0.15.8.1/plib/ui/output.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)      781 2022-07-10 04:04:26.000000 plib3.ui-0.15.8.1/plib/ui/manager.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)      478 2022-01-20 06:02:08.000000 plib3.ui-0.15.8.1/plib/ui/examples.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)      711 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/imp.py
-drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-05-18 02:31:21.000000 plib3.ui-0.15.8.1/plib/ui/images/
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2207 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/cancel-qt4.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1409 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_close-darwin.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2207 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/cancel-kde4.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1608 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_redo-gtk.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2293 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/refresh-gtk.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2406 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/about-win32.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1700 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit-pyside.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1473 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit-darwin.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1393 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_new-wx.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1246 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/ok-kde4.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      315 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/cancel-win32.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2207 2020-08-13 19:52:05.000000 plib3.ui-0.15.8.1/plib/ui/images/cancel-pyside2.png
--rw-r--r--   0 pdonis    (1002) pdonis    (1002)     1473 2016-01-01 20:09:09.000000 plib3.ui-0.15.8.1/plib/ui/images/commit-pyside.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2293 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/refresh-wx.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      567 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_copy-wx.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      971 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_open-gtk.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1491 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/about-qt4.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      596 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/add-wx.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2362 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/about-posix.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1810 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit-posix.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1956 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit-wx.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      335 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_overwrite-pyside2.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1410 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_new-qt4.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2138 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/commit-posix.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1571 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_open-darwin.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1618 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/about_toolkit-gtk.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1207 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/exit-gtk.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      254 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/ok-darwin.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2085 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_close-pyside.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2020 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_undo-qt4.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1218 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/apply-pyside.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1257 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/prefs-darwin.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      860 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_copy-pyside.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1205 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_save-win32.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1594 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_close-posix.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1491 2020-08-13 19:52:05.000000 plib3.ui-0.15.8.1/plib/ui/images/about-pyside2.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      298 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/ok-win32.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      596 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/add-pyside2.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      937 2020-08-13 19:52:05.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_paste-pyside2.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      335 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/remove-pyside.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2549 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/about_toolkit-kde4.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1985 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/about_toolkit-wx.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2158 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/remove-posix.png
--rw-r--r--   0 pdonis    (1002) pdonis    (1002)     1536 2016-01-01 20:09:09.000000 plib3.ui-0.15.8.1/plib/ui/images/rollback-pyside.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1458 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_paste-posix.png
--rw-r--r--   0 pdonis    (1002) pdonis    (1002)     2044 2016-03-10 22:30:20.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_clear-pyside.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1700 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit-kde4.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1348 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_save-posix.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1372 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/prefs-wx.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2152 2020-08-13 19:52:05.000000 plib3.ui-0.15.8.1/plib/ui/images/file_saveas-pyside2.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      860 2020-08-13 19:52:05.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_copy-pyside2.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1218 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/apply-qt4.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1608 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_redo-pyside.png
--rw-r--r--   0 pdonis    (1002) pdonis    (1002)     1536 2016-01-01 20:09:09.000000 plib3.ui-0.15.8.1/plib/ui/images/rollback-pyside2.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2319 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/apply-gtk.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      860 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_copy-qt4.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      892 2020-08-13 19:52:05.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_cut-pyside2.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      335 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/remove-gtk.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1682 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/exit-qt4.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1248 2019-09-19 23:46:59.000000 plib3.ui-0.15.8.1/plib/ui/images/about_toolkit-qt5.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2152 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_saveas-pyside.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      185 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit-win32-base.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2182 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/refresh-qt4.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1357 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/apply-posix.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1431 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit-win32.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1577 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/remove-darwin.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1754 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_delete-wx.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1248 2020-08-13 19:52:32.000000 plib3.ui-0.15.8.1/plib/ui/images/about_toolkit-pyside2.png
--rw-r--r--   0 pdonis    (1002) pdonis    (1002)     1473 2016-01-01 20:09:09.000000 plib3.ui-0.15.8.1/plib/ui/images/commit-pyside2.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1798 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/about-darwin.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2169 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_cut-posix.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1710 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/about-gtk.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1368 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_delete-posix.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2024 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_saveas-gtk.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1207 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/exit-wx.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      335 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/remove-pyside2.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1675 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_close-wx.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      787 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/view-darwin.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1263 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_save-pyside.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1998 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_redo-qt4.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1088 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_open-pyside.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1532 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_cut-gtk.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1608 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_redo-wx.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      937 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_paste-qt4.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1610 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/exit-posix.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1246 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/ok-qt4.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2024 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_saveas-wx.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1754 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_delete-gtk.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1700 2020-08-13 19:52:05.000000 plib3.ui-0.15.8.1/plib/ui/images/edit-pyside2.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      892 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_cut-pyside.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1218 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/apply-kde4.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1919 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/exit-darwin.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2293 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/refresh-pyside2.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2641 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/refresh-win32.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      722 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_new-win32.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2026 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/cancel-wx.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1682 2020-08-13 19:52:05.000000 plib3.ui-0.15.8.1/plib/ui/images/exit-pyside2.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2319 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/apply-wx.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1218 2020-08-13 19:52:05.000000 plib3.ui-0.15.8.1/plib/ui/images/apply-pyside2.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1682 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/exit-pyside.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      342 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_close-win32.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1956 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit-gtk.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2278 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/prefs-win32.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1097 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_selectall-wx.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1246 2020-08-13 19:52:05.000000 plib3.ui-0.15.8.1/plib/ui/images/ok-pyside2.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      335 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/remove-wx.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1393 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_new-gtk.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      892 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_cut-qt4.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1944 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_save-gtk.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1097 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_selectall-gtk.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1065 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/remove-qt4.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1799 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/refresh-darwin.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1491 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/about-pyside.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1277 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_selectall-posix.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      726 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/about_toolkit-qt.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1630 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/rollback-posix.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1246 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/ok-pyside.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2085 2020-08-13 19:52:05.000000 plib3.ui-0.15.8.1/plib/ui/images/file_close-pyside2.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2026 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/cancel-gtk.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1279 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/add-posix.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1333 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_delete-pyside.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2213 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/view-win32.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1377 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/exit-win32.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2216 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/ok-wx.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1532 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_cut-wx.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1172 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_redo-posix.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1263 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_save-qt4.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2037 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/about_toolkit-pyside.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      898 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_save-darwin.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1487 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/add-qt4.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1555 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_undo-pyside.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2158 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_overwrite-posix.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1712 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/add-darwin.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      596 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/add-gtk.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1944 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_save-wx.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1143 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_paste-gtk.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2152 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_saveas-qt4.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1675 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_close-gtk.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1555 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_undo-pyside2.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2037 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/about_toolkit-qt4.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2232 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_open-posix.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1555 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_undo-wx.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      596 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/add-pyside.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1901 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/refresh-posix.png
--rw-r--r--   0 pdonis    (1002) pdonis    (1002)      205 2020-04-10 23:08:30.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_clear-posix.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2207 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/cancel-pyside.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      937 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_paste-pyside.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      952 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/view-posix.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      335 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_overwrite-wx.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1608 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_redo-pyside2.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1088 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_open-qt4.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2069 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_saveas-posix.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1333 2020-08-13 19:52:05.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_delete-pyside2.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      971 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_open-wx.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     3044 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/about_toolkit-kde.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1491 2019-09-19 23:46:59.000000 plib3.ui-0.15.8.1/plib/ui/images/about-qt5.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1393 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/ok-posix.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1333 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_delete-qt4.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1372 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/prefs-gtk.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      879 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_copy-posix.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1173 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_new-darwin.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1012 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/prefs-posix.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2293 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/refresh-pyside.png
--rw-r--r--   0 pdonis    (1002) pdonis    (1002)     1800 2016-03-10 22:30:23.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_selectnone-posix.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1710 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/about-wx.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1555 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_undo-gtk.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1410 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_new-pyside.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1468 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/cancel-posix.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2216 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/ok-gtk.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1410 2020-08-13 19:52:05.000000 plib3.ui-0.15.8.1/plib/ui/images/file_new-pyside2.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      567 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_copy-gtk.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1143 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_paste-wx.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1207 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_saveas-win32.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1875 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_saveas-darwin.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1160 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit_undo-posix.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2085 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_close-qt4.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1263 2020-08-13 19:52:05.000000 plib3.ui-0.15.8.1/plib/ui/images/file_save-pyside2.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1700 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/edit-qt4.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1088 2020-08-13 19:52:05.000000 plib3.ui-0.15.8.1/plib/ui/images/file_open-pyside2.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1177 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_new-posix.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1378 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/file_open-win32.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      353 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/plib/ui/images/cancel-darwin.png
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     2784 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/plib/ui/app.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     3217 2022-01-09 05:35:26.000000 plib3.ui-0.15.8.1/plib/ui/fileaware.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     4933 2022-01-09 05:35:26.000000 plib3.ui-0.15.8.1/plib/ui/common.py
-drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-05-18 02:31:20.000000 plib3.ui-0.15.8.1/examples/
-drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-05-18 02:31:21.000000 plib3.ui-0.15.8.1/examples/pyidserver/
--rwxrwx---   0 pdonis    (1002) pdonis    (1002)    11339 2022-07-09 05:25:43.000000 plib3.ui-0.15.8.1/examples/pyidserver/pyidserver-ui3.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      576 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/examples/pyidserver/pyidserver.png
-drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-05-18 02:31:20.000000 plib3.ui-0.15.8.1/examples/pnotepad/
--rwxrwx---   0 pdonis    (1002) pdonis    (1002)     9131 2022-04-21 04:56:54.000000 plib3.ui-0.15.8.1/examples/pnotepad/pnotepad3.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1069 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/examples/pnotepad/pnotepad.png
-drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-05-18 02:31:21.000000 plib3.ui-0.15.8.1/examples/scrips/
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      952 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/examples/scrips/scrips.png
--rwxrwx---   0 pdonis    (1002) pdonis    (1002)    10336 2022-02-22 05:03:22.000000 plib3.ui-0.15.8.1/examples/scrips/scrips-edit3.py
-drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-05-18 02:31:20.000000 plib3.ui-0.15.8.1/examples/pimgview/
--rwxrwx---   0 pdonis    (1002) pdonis    (1002)     5547 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/examples/pimgview/pimgview3.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     1473 2022-01-09 05:35:26.000000 plib3.ui-0.15.8.1/examples/pimgview/rotate_left.png
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     1552 2022-01-09 05:35:26.000000 plib3.ui-0.15.8.1/examples/pimgview/pimgview.png
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     1474 2022-01-09 05:35:26.000000 plib3.ui-0.15.8.1/examples/pimgview/rotate_right.png
-drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-05-18 02:31:21.000000 plib3.ui-0.15.8.1/examples/ui/
--rwxrwx---   0 pdonis    (1002) pdonis    (1002)    24114 2022-07-30 18:11:39.000000 plib3.ui-0.15.8.1/examples/ui/ui-signals3.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     2901 2022-01-03 06:32:01.000000 plib3.ui-0.15.8.1/examples/ui/ui-text3.py
--rwxrwxr-x   0 pdonis    (1002) pdonis    (1002)     6384 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/examples/ui/ui-display3.py
-drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-05-18 02:31:21.000000 plib3.ui-0.15.8.1/examples/pxmlview/
--rwxrwx---   0 pdonis    (1002) pdonis    (1002)     4464 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.1/examples/pxmlview/pxmlview3.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      207 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/examples/pxmlview/test-other.xml
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2444 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/examples/pxmlview/pxmlview.png
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      179 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.1/examples/pxmlview/test.xml
-drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-05-18 02:31:20.000000 plib3.ui-0.15.8.1/examples/container/
--rwxrwxr-x   0 pdonis    (1002) pdonis    (1002)     4720 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.1/examples/container/graphics3.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)    18010 2022-01-03 06:07:28.000000 plib3.ui-0.15.8.1/LICENSE.txt
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     3608 2023-05-18 02:04:57.000000 plib3.ui-0.15.8.1/README.rst
--rw-rw----   0 pdonis    (1002) pdonis    (1002)       37 2022-01-09 05:35:26.000000 plib3.ui-0.15.8.1/MANIFEST.in
--rw-rw----   0 pdonis    (1002) pdonis    (1002)      334 2023-05-18 02:29:27.000000 plib3.ui-0.15.8.1/TODO.rst
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     4648 2023-05-18 02:31:21.000000 plib3.ui-0.15.8.1/PKG-INFO
--rw-rw----   0 pdonis    (1002) pdonis    (1002)      117 2022-01-22 04:09:05.000000 plib3.ui-0.15.8.1/pyproject.toml
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     2445 2023-05-18 02:31:21.000000 plib3.ui-0.15.8.1/setup.cfg
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     9771 2023-05-18 02:31:01.000000 plib3.ui-0.15.8.1/CHANGES.rst
+drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-06-17 03:08:51.000000 plib3.ui-0.15.8.2/
+drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-06-17 03:08:51.000000 plib3.ui-0.15.8.2/plib/
+drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-06-17 03:08:51.000000 plib3.ui-0.15.8.2/plib/ui/
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     6745 2022-07-09 05:35:22.000000 plib3.ui-0.15.8.2/plib/ui/prefs.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     2576 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/custom.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)      266 2023-06-17 03:07:49.000000 plib3.ui-0.15.8.2/plib/ui/__init__.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     2319 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/dialogs.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     2422 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/socket.py
+drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-06-17 03:08:51.000000 plib3.ui-0.15.8.2/plib/ui/base/
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     3333 2022-07-09 05:25:43.000000 plib3.ui-0.15.8.2/plib/ui/base/button.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)      529 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/base/mouse.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     2928 2022-07-10 03:01:32.000000 plib3.ui-0.15.8.2/plib/ui/base/tabwidget.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     1396 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/base/display.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)    14312 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/base/helpers.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     1684 2022-07-09 05:25:43.000000 plib3.ui-0.15.8.2/plib/ui/base/listbox.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      245 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/base/__init__.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      951 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/base/socket.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     3554 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/base/form.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     1966 2022-07-10 03:01:58.000000 plib3.ui-0.15.8.2/plib/ui/base/groupbox.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      954 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/base/container.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     7962 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/base/mainwin.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     3991 2022-07-30 18:34:01.000000 plib3.ui-0.15.8.2/plib/ui/base/group.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     5378 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/base/table.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     5506 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/base/editctrl.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     8681 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/base/listview.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)    24031 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/base/app.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     3462 2022-07-10 04:27:02.000000 plib3.ui-0.15.8.2/plib/ui/base/pagewidget.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      936 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/base/label.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     2539 2022-07-09 05:25:43.000000 plib3.ui-0.15.8.2/plib/ui/base/combo.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     1302 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/base/scroller.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     1500 2022-01-09 05:35:26.000000 plib3.ui-0.15.8.2/plib/ui/base/imageview.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)      409 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/base/focus.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     2445 2022-07-10 03:03:14.000000 plib3.ui-0.15.8.2/plib/ui/base/dialog.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)    15014 2022-07-30 18:34:01.000000 plib3.ui-0.15.8.2/plib/ui/widgets.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     8231 2022-07-30 18:34:01.000000 plib3.ui-0.15.8.2/plib/ui/defs.py
+drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-06-17 03:08:51.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     3733 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/__init__.py
+drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-06-17 03:08:51.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     2381 2022-07-09 05:25:43.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/button.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     1625 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/mouse.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     1638 2022-07-10 01:46:10.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/tabwidget.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     1421 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/display.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     2365 2022-07-09 05:25:43.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/listbox.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      313 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/__init__.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     2139 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/socket.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     3238 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/form.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1499 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/groupbox.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1084 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/container.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     4799 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/mainwin.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     2150 2022-07-30 18:34:01.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/group.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     5049 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/table.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2581 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/header.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     5219 2023-06-17 03:03:21.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/editctrl.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     5232 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/listview.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)    16030 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/app.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     1513 2022-07-10 01:39:26.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/pagewidget.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      922 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/label.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2926 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/combo.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     1541 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/scroller.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     2292 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/imageview.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)      806 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/focus.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1140 2022-07-10 03:03:29.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/dialog.py
+drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-06-17 03:08:51.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/wx/
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     2392 2022-07-09 05:25:43.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/wx/button.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     1654 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/wx/mouse.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1515 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/wx/tabwidget.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1353 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/wx/display.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     2204 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/wx/listbox.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      310 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/wx/__init__.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     3407 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/wx/socket.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     4496 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/wx/form.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2701 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/wx/groupbox.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     7166 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/wx/mainwin.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     3948 2022-07-30 18:34:01.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/wx/group.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     8564 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/wx/table.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     7566 2023-06-17 03:06:22.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/wx/editctrl.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     8487 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/wx/listview.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)    25325 2023-06-17 03:03:21.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/wx/app.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     1453 2023-06-16 04:00:53.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/wx/pagewidget.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      957 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/wx/label.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2624 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/wx/combo.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     1694 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/wx/scroller.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     2623 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/wx/imageview.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)      489 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/wx/focus.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     1737 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/wx/dialog.py
+drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-06-17 03:08:51.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     2587 2022-07-09 05:25:43.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/button.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     1562 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/mouse.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     1711 2022-07-10 01:46:58.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/tabwidget.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     1512 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/display.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     2493 2022-07-09 05:25:43.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/listbox.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      305 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/__init__.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1632 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/socket.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     3228 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/form.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1582 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/groupbox.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1078 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/container.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     4973 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/mainwin.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     2161 2022-07-30 18:34:01.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/group.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     5120 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/table.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2563 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/header.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     5852 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/editctrl.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     5548 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/listview.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)    16633 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/app.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     1591 2023-06-16 04:00:45.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/pagewidget.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1003 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/label.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     3092 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/combo.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     1531 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/scroller.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     2128 2022-01-09 05:35:26.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/imageview.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)      743 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/focus.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1223 2022-07-10 03:03:35.000000 plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/dialog.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     1888 2022-04-21 04:56:54.000000 plib3.ui-0.15.8.2/plib/ui/textfile.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     1767 2022-07-09 05:25:43.000000 plib3.ui-0.15.8.2/plib/ui/coll.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     1312 2022-05-28 05:28:12.000000 plib3.ui-0.15.8.2/plib/ui/output.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)      781 2022-07-10 04:04:26.000000 plib3.ui-0.15.8.2/plib/ui/manager.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)      478 2022-01-20 06:02:08.000000 plib3.ui-0.15.8.2/plib/ui/examples.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)      711 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/imp.py
+drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-06-17 03:08:51.000000 plib3.ui-0.15.8.2/plib/ui/images/
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2207 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/cancel-qt4.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1409 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_close-darwin.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2207 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/cancel-kde4.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1608 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_redo-gtk.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2293 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/refresh-gtk.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2406 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/about-win32.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1700 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit-pyside.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1473 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit-darwin.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1393 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_new-wx.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1246 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/ok-kde4.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      315 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/cancel-win32.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2207 2020-08-13 19:52:05.000000 plib3.ui-0.15.8.2/plib/ui/images/cancel-pyside2.png
+-rw-r--r--   0 pdonis    (1002) pdonis    (1002)     1473 2016-01-01 20:09:09.000000 plib3.ui-0.15.8.2/plib/ui/images/commit-pyside.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2293 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/refresh-wx.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      567 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_copy-wx.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      971 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_open-gtk.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1491 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/about-qt4.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      596 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/add-wx.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2362 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/about-posix.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1810 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit-posix.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1956 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit-wx.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      335 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_overwrite-pyside2.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1410 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_new-qt4.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2138 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/commit-posix.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1571 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_open-darwin.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1618 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/about_toolkit-gtk.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1207 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/exit-gtk.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      254 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/ok-darwin.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2085 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_close-pyside.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2020 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_undo-qt4.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1218 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/apply-pyside.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1257 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/prefs-darwin.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      860 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_copy-pyside.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1205 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_save-win32.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1594 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_close-posix.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1491 2020-08-13 19:52:05.000000 plib3.ui-0.15.8.2/plib/ui/images/about-pyside2.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      298 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/ok-win32.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      596 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/add-pyside2.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      937 2020-08-13 19:52:05.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_paste-pyside2.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      335 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/remove-pyside.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2549 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/about_toolkit-kde4.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1985 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/about_toolkit-wx.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2158 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/remove-posix.png
+-rw-r--r--   0 pdonis    (1002) pdonis    (1002)     1536 2016-01-01 20:09:09.000000 plib3.ui-0.15.8.2/plib/ui/images/rollback-pyside.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1458 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_paste-posix.png
+-rw-r--r--   0 pdonis    (1002) pdonis    (1002)     2044 2016-03-10 22:30:20.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_clear-pyside.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1700 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit-kde4.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1348 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_save-posix.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1372 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/prefs-wx.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2152 2020-08-13 19:52:05.000000 plib3.ui-0.15.8.2/plib/ui/images/file_saveas-pyside2.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      860 2020-08-13 19:52:05.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_copy-pyside2.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1218 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/apply-qt4.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1608 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_redo-pyside.png
+-rw-r--r--   0 pdonis    (1002) pdonis    (1002)     1536 2016-01-01 20:09:09.000000 plib3.ui-0.15.8.2/plib/ui/images/rollback-pyside2.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2319 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/apply-gtk.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      860 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_copy-qt4.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      892 2020-08-13 19:52:05.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_cut-pyside2.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      335 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/remove-gtk.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1682 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/exit-qt4.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1248 2019-09-19 23:46:59.000000 plib3.ui-0.15.8.2/plib/ui/images/about_toolkit-qt5.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2152 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_saveas-pyside.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      185 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit-win32-base.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2182 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/refresh-qt4.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1357 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/apply-posix.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1431 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit-win32.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1577 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/remove-darwin.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1754 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_delete-wx.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1248 2020-08-13 19:52:32.000000 plib3.ui-0.15.8.2/plib/ui/images/about_toolkit-pyside2.png
+-rw-r--r--   0 pdonis    (1002) pdonis    (1002)     1473 2016-01-01 20:09:09.000000 plib3.ui-0.15.8.2/plib/ui/images/commit-pyside2.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1798 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/about-darwin.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2169 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_cut-posix.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1710 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/about-gtk.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1368 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_delete-posix.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2024 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_saveas-gtk.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1207 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/exit-wx.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      335 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/remove-pyside2.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1675 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_close-wx.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      787 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/view-darwin.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1263 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_save-pyside.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1998 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_redo-qt4.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1088 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_open-pyside.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1532 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_cut-gtk.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1608 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_redo-wx.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      937 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_paste-qt4.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1610 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/exit-posix.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1246 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/ok-qt4.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2024 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_saveas-wx.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1754 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_delete-gtk.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1700 2020-08-13 19:52:05.000000 plib3.ui-0.15.8.2/plib/ui/images/edit-pyside2.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      892 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_cut-pyside.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1218 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/apply-kde4.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1919 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/exit-darwin.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2293 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/refresh-pyside2.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2641 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/refresh-win32.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      722 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_new-win32.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2026 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/cancel-wx.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1682 2020-08-13 19:52:05.000000 plib3.ui-0.15.8.2/plib/ui/images/exit-pyside2.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2319 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/apply-wx.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1218 2020-08-13 19:52:05.000000 plib3.ui-0.15.8.2/plib/ui/images/apply-pyside2.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1682 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/exit-pyside.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      342 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_close-win32.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1956 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit-gtk.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2278 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/prefs-win32.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1097 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_selectall-wx.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1246 2020-08-13 19:52:05.000000 plib3.ui-0.15.8.2/plib/ui/images/ok-pyside2.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      335 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/remove-wx.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1393 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_new-gtk.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      892 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_cut-qt4.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1944 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_save-gtk.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1097 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_selectall-gtk.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1065 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/remove-qt4.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1799 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/refresh-darwin.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1491 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/about-pyside.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1277 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_selectall-posix.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      726 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/about_toolkit-qt.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1630 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/rollback-posix.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1246 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/ok-pyside.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2085 2020-08-13 19:52:05.000000 plib3.ui-0.15.8.2/plib/ui/images/file_close-pyside2.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2026 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/cancel-gtk.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1279 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/add-posix.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1333 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_delete-pyside.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2213 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/view-win32.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1377 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/exit-win32.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2216 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/ok-wx.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1532 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_cut-wx.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1172 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_redo-posix.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1263 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_save-qt4.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2037 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/about_toolkit-pyside.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      898 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_save-darwin.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1487 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/add-qt4.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1555 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_undo-pyside.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2158 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_overwrite-posix.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1712 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/add-darwin.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      596 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/add-gtk.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1944 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_save-wx.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1143 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_paste-gtk.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2152 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_saveas-qt4.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1675 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_close-gtk.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1555 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_undo-pyside2.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2037 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/about_toolkit-qt4.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2232 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_open-posix.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1555 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_undo-wx.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      596 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/add-pyside.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1901 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/refresh-posix.png
+-rw-r--r--   0 pdonis    (1002) pdonis    (1002)      205 2020-04-10 23:08:30.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_clear-posix.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2207 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/cancel-pyside.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      937 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_paste-pyside.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      952 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/view-posix.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      335 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_overwrite-wx.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1608 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_redo-pyside2.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1088 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_open-qt4.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2069 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_saveas-posix.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1333 2020-08-13 19:52:05.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_delete-pyside2.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      971 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_open-wx.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     3044 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/about_toolkit-kde.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1491 2019-09-19 23:46:59.000000 plib3.ui-0.15.8.2/plib/ui/images/about-qt5.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1393 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/ok-posix.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1333 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_delete-qt4.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1372 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/prefs-gtk.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      879 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_copy-posix.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1173 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_new-darwin.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1012 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/prefs-posix.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2293 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/refresh-pyside.png
+-rw-r--r--   0 pdonis    (1002) pdonis    (1002)     1800 2016-03-10 22:30:23.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_selectnone-posix.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1710 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/about-wx.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1555 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_undo-gtk.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1410 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_new-pyside.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1468 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/cancel-posix.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2216 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/ok-gtk.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1410 2020-08-13 19:52:05.000000 plib3.ui-0.15.8.2/plib/ui/images/file_new-pyside2.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      567 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_copy-gtk.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1143 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_paste-wx.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1207 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_saveas-win32.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1875 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_saveas-darwin.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1160 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit_undo-posix.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2085 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_close-qt4.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1263 2020-08-13 19:52:05.000000 plib3.ui-0.15.8.2/plib/ui/images/file_save-pyside2.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1700 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/edit-qt4.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1088 2020-08-13 19:52:05.000000 plib3.ui-0.15.8.2/plib/ui/images/file_open-pyside2.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1177 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_new-posix.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1378 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/file_open-win32.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      353 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/plib/ui/images/cancel-darwin.png
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     2784 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/plib/ui/app.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     3217 2022-01-09 05:35:26.000000 plib3.ui-0.15.8.2/plib/ui/fileaware.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     4933 2022-01-09 05:35:26.000000 plib3.ui-0.15.8.2/plib/ui/common.py
+drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-06-17 03:08:51.000000 plib3.ui-0.15.8.2/examples/
+drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-06-17 03:08:51.000000 plib3.ui-0.15.8.2/examples/pyidserver/
+-rwxrwx---   0 pdonis    (1002) pdonis    (1002)    11339 2022-07-09 05:25:43.000000 plib3.ui-0.15.8.2/examples/pyidserver/pyidserver-ui3.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      576 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/examples/pyidserver/pyidserver.png
+drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-06-17 03:08:51.000000 plib3.ui-0.15.8.2/examples/pnotepad/
+-rwxrwx---   0 pdonis    (1002) pdonis    (1002)     9131 2022-04-21 04:56:54.000000 plib3.ui-0.15.8.2/examples/pnotepad/pnotepad3.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1069 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/examples/pnotepad/pnotepad.png
+drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-06-17 03:08:51.000000 plib3.ui-0.15.8.2/examples/scrips/
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      952 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/examples/scrips/scrips.png
+-rwxrwx---   0 pdonis    (1002) pdonis    (1002)    10336 2022-02-22 05:03:22.000000 plib3.ui-0.15.8.2/examples/scrips/scrips-edit3.py
+drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-06-17 03:08:51.000000 plib3.ui-0.15.8.2/examples/pimgview/
+-rwxrwx---   0 pdonis    (1002) pdonis    (1002)     5547 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/examples/pimgview/pimgview3.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     1473 2022-01-09 05:35:26.000000 plib3.ui-0.15.8.2/examples/pimgview/rotate_left.png
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     1552 2022-01-09 05:35:26.000000 plib3.ui-0.15.8.2/examples/pimgview/pimgview.png
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     1474 2022-01-09 05:35:26.000000 plib3.ui-0.15.8.2/examples/pimgview/rotate_right.png
+drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-06-17 03:08:51.000000 plib3.ui-0.15.8.2/examples/ui/
+-rwxrwx---   0 pdonis    (1002) pdonis    (1002)    24114 2022-07-30 18:11:39.000000 plib3.ui-0.15.8.2/examples/ui/ui-signals3.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     2901 2022-01-03 06:32:01.000000 plib3.ui-0.15.8.2/examples/ui/ui-text3.py
+-rwxrwxr-x   0 pdonis    (1002) pdonis    (1002)     6384 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/examples/ui/ui-display3.py
+drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-06-17 03:08:51.000000 plib3.ui-0.15.8.2/examples/pxmlview/
+-rwxrwx---   0 pdonis    (1002) pdonis    (1002)     4464 2022-07-29 23:10:44.000000 plib3.ui-0.15.8.2/examples/pxmlview/pxmlview3.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      207 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/examples/pxmlview/test-other.xml
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2444 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/examples/pxmlview/pxmlview.png
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      179 2018-10-23 04:10:25.000000 plib3.ui-0.15.8.2/examples/pxmlview/test.xml
+drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-06-17 03:08:51.000000 plib3.ui-0.15.8.2/examples/container/
+-rwxrwxr-x   0 pdonis    (1002) pdonis    (1002)     4720 2022-01-03 06:32:10.000000 plib3.ui-0.15.8.2/examples/container/graphics3.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)    18010 2022-01-03 06:07:28.000000 plib3.ui-0.15.8.2/LICENSE.txt
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     3608 2023-05-18 02:04:57.000000 plib3.ui-0.15.8.2/README.rst
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)       37 2022-01-09 05:35:26.000000 plib3.ui-0.15.8.2/MANIFEST.in
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)      334 2023-05-18 02:29:27.000000 plib3.ui-0.15.8.2/TODO.rst
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     4648 2023-06-17 03:08:51.000000 plib3.ui-0.15.8.2/PKG-INFO
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)      117 2022-01-22 04:09:05.000000 plib3.ui-0.15.8.2/pyproject.toml
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     2445 2023-06-17 03:08:51.000000 plib3.ui-0.15.8.2/setup.cfg
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     9871 2023-06-17 03:08:20.000000 plib3.ui-0.15.8.2/CHANGES.rst
```

### Comparing `plib3.ui-0.15.8.1/plib/ui/prefs.py` & `plib3.ui-0.15.8.2/plib/ui/prefs.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/custom.py` & `plib3.ui-0.15.8.2/plib/ui/custom.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/dialogs.py` & `plib3.ui-0.15.8.2/plib/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/socket.py` & `plib3.ui-0.15.8.2/plib/ui/socket.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/base/button.py` & `plib3.ui-0.15.8.2/plib/ui/base/button.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/base/mouse.py` & `plib3.ui-0.15.8.2/plib/ui/base/mouse.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/base/tabwidget.py` & `plib3.ui-0.15.8.2/plib/ui/base/tabwidget.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/base/display.py` & `plib3.ui-0.15.8.2/plib/ui/base/display.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/base/helpers.py` & `plib3.ui-0.15.8.2/plib/ui/base/helpers.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/base/listbox.py` & `plib3.ui-0.15.8.2/plib/ui/base/listbox.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/base/socket.py` & `plib3.ui-0.15.8.2/plib/ui/base/socket.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/base/form.py` & `plib3.ui-0.15.8.2/plib/ui/base/form.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/base/groupbox.py` & `plib3.ui-0.15.8.2/plib/ui/base/groupbox.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/base/container.py` & `plib3.ui-0.15.8.2/plib/ui/base/container.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/base/mainwin.py` & `plib3.ui-0.15.8.2/plib/ui/base/mainwin.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/base/group.py` & `plib3.ui-0.15.8.2/plib/ui/base/group.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/base/table.py` & `plib3.ui-0.15.8.2/plib/ui/base/table.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/base/editctrl.py` & `plib3.ui-0.15.8.2/plib/ui/base/editctrl.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/base/listview.py` & `plib3.ui-0.15.8.2/plib/ui/base/listview.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/base/app.py` & `plib3.ui-0.15.8.2/plib/ui/base/app.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/base/pagewidget.py` & `plib3.ui-0.15.8.2/plib/ui/base/pagewidget.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/base/label.py` & `plib3.ui-0.15.8.2/plib/ui/base/label.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/base/combo.py` & `plib3.ui-0.15.8.2/plib/ui/base/combo.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/base/scroller.py` & `plib3.ui-0.15.8.2/plib/ui/base/scroller.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/base/imageview.py` & `plib3.ui-0.15.8.2/plib/ui/base/imageview.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/base/dialog.py` & `plib3.ui-0.15.8.2/plib/ui/base/dialog.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/widgets.py` & `plib3.ui-0.15.8.2/plib/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/defs.py` & `plib3.ui-0.15.8.2/plib/ui/defs.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/__init__.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/__init__.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/button.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/button.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/mouse.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/mouse.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/tabwidget.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/tabwidget.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/display.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/display.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/listbox.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/listbox.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/socket.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/socket.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/form.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/form.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/groupbox.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/groupbox.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/container.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/container.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/mainwin.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/mainwin.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/group.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/group.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/table.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/table.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/header.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/header.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/editctrl.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/editctrl.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/listview.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/listview.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/app.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/app.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/pagewidget.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/pagewidget.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/label.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/label.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/combo.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/combo.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/scroller.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/scroller.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/imageview.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/imageview.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/focus.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/focus.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/pyside2/dialog.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/pyside2/dialog.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/wx/button.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/wx/button.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/wx/mouse.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/wx/mouse.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/wx/tabwidget.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/wx/tabwidget.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/wx/display.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/wx/display.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/wx/listbox.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/wx/listbox.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/wx/socket.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/wx/socket.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/wx/form.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/wx/form.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/wx/groupbox.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/wx/groupbox.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/wx/mainwin.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/wx/mainwin.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/wx/group.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/wx/group.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/wx/table.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/wx/table.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/wx/editctrl.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/wx/editctrl.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,14 +109,19 @@
         eventManager.Register(val.OnTextEvent, wx.EVT_TEXT, self)
         PNumEditBoxBase.__init__(self, manager, parent, value,
                                  geometry=geometry, expand=expand)
     
     def set_value(self, value):
         super(PNumEditBox, self).set_value(value)
         self.val.value = value
+    
+    def wrap_target(self, signal, target):
+        target = PNumEditBoxBase.wrap_target(self, signal, target)
+        target = PWxEditBase.wrap_target(self, signal, target)
+        return target
 
 
 class PEditControl(PWxEditBase, PEditControlBase):
     
     _style = wx.TE_MULTILINE | wx.TE_PROCESS_TAB
     
     _align = True  # used by panel to determine placement
```

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/wx/listview.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/wx/listview.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/wx/app.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/wx/app.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/wx/pagewidget.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/wx/pagewidget.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Module WX.TABWIDGET -- Python wxWidgets Tab Widget
 Sub-Package UI.TOOLKITS.QT of Package PLIB3 -- Python GUI Toolkits
 Copyright (C) 2008-2022 by Peter A. Donis
 
 Released under the GNU General Public License, Version 2
 See the LICENSE and README files for more information
 
-This module contains the wxWidgets UI objects for the tab widget.
+This module contains the wxWidgets UI objects for the page widget.
 """
 
 import wx
 
 from plib.ui.defs import *
 from plib.ui.base.pagewidget import PPageWidgetBase
```

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/wx/label.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/wx/label.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/wx/combo.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/wx/combo.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/wx/scroller.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/wx/scroller.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/wx/imageview.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/wx/imageview.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/wx/dialog.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/wx/dialog.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/button.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/button.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/mouse.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/mouse.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/tabwidget.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/tabwidget.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/display.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/display.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/listbox.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/listbox.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/socket.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/socket.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/form.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/form.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/groupbox.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/groupbox.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/container.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/container.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/mainwin.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/mainwin.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/group.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/group.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/table.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/table.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/header.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/header.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/editctrl.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/editctrl.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/listview.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/listview.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/app.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/app.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/pagewidget.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/pagewidget.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Module QT5.PAGEWIDGET -- Python Qt 5 Page Widget
 Sub-Package UI.TOOLKITS.QT5 of Package PLIB3 -- Python UI Toolkits
 Copyright (C) 2008-2022 by Peter A. Donis
 
 Released under the GNU General Public License, Version 2
 See the LICENSE and README files for more information
 
-This module contains the Qt 5 UI objects for the tab widget.
+This module contains the Qt 5 UI objects for the page widget.
 """
 
 from PyQt5 import QtWidgets as qt
 
 from plib.ui.defs import *
 from plib.ui.base.pagewidget import PPageWidgetBase
```

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/label.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/label.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/combo.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/combo.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/scroller.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/scroller.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/imageview.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/imageview.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/focus.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/focus.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/toolkits/qt5/dialog.py` & `plib3.ui-0.15.8.2/plib/ui/toolkits/qt5/dialog.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/textfile.py` & `plib3.ui-0.15.8.2/plib/ui/textfile.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/coll.py` & `plib3.ui-0.15.8.2/plib/ui/coll.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/output.py` & `plib3.ui-0.15.8.2/plib/ui/output.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/manager.py` & `plib3.ui-0.15.8.2/plib/ui/manager.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/imp.py` & `plib3.ui-0.15.8.2/plib/ui/imp.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/cancel-qt4.png` & `plib3.ui-0.15.8.2/plib/ui/images/cancel-qt4.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_close-darwin.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_close-darwin.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/cancel-kde4.png` & `plib3.ui-0.15.8.2/plib/ui/images/cancel-kde4.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_redo-gtk.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_redo-gtk.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/refresh-gtk.png` & `plib3.ui-0.15.8.2/plib/ui/images/refresh-gtk.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/about-win32.png` & `plib3.ui-0.15.8.2/plib/ui/images/about-win32.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit-pyside.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit-pyside.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit-darwin.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit-darwin.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_new-wx.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_new-wx.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/ok-kde4.png` & `plib3.ui-0.15.8.2/plib/ui/images/ok-kde4.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/cancel-pyside2.png` & `plib3.ui-0.15.8.2/plib/ui/images/cancel-pyside2.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/commit-pyside.png` & `plib3.ui-0.15.8.2/plib/ui/images/commit-pyside.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/refresh-wx.png` & `plib3.ui-0.15.8.2/plib/ui/images/refresh-wx.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_copy-wx.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_copy-wx.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_open-gtk.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_open-gtk.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/about-qt4.png` & `plib3.ui-0.15.8.2/plib/ui/images/about-qt4.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/add-wx.png` & `plib3.ui-0.15.8.2/plib/ui/images/add-wx.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/about-posix.png` & `plib3.ui-0.15.8.2/plib/ui/images/about-posix.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit-posix.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit-posix.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit-wx.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit-wx.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_new-qt4.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_new-qt4.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/commit-posix.png` & `plib3.ui-0.15.8.2/plib/ui/images/commit-posix.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_open-darwin.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_open-darwin.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/about_toolkit-gtk.png` & `plib3.ui-0.15.8.2/plib/ui/images/about_toolkit-gtk.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/exit-gtk.png` & `plib3.ui-0.15.8.2/plib/ui/images/exit-gtk.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_close-pyside.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_close-pyside.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_undo-qt4.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_undo-qt4.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/apply-pyside.png` & `plib3.ui-0.15.8.2/plib/ui/images/apply-pyside.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/prefs-darwin.png` & `plib3.ui-0.15.8.2/plib/ui/images/prefs-darwin.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_copy-pyside.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_copy-pyside.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_save-win32.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_save-win32.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_close-posix.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_close-posix.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/about-pyside2.png` & `plib3.ui-0.15.8.2/plib/ui/images/about-pyside2.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/add-pyside2.png` & `plib3.ui-0.15.8.2/plib/ui/images/add-pyside2.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_paste-pyside2.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_paste-pyside2.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/about_toolkit-kde4.png` & `plib3.ui-0.15.8.2/plib/ui/images/about_toolkit-kde4.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/about_toolkit-wx.png` & `plib3.ui-0.15.8.2/plib/ui/images/about_toolkit-wx.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/remove-posix.png` & `plib3.ui-0.15.8.2/plib/ui/images/remove-posix.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/rollback-pyside.png` & `plib3.ui-0.15.8.2/plib/ui/images/rollback-pyside.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_paste-posix.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_paste-posix.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_clear-pyside.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_clear-pyside.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit-kde4.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit-kde4.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_save-posix.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_save-posix.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/prefs-wx.png` & `plib3.ui-0.15.8.2/plib/ui/images/prefs-wx.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_saveas-pyside2.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_saveas-pyside2.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_copy-pyside2.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_copy-pyside2.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/apply-qt4.png` & `plib3.ui-0.15.8.2/plib/ui/images/apply-qt4.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_redo-pyside.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_redo-pyside.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/rollback-pyside2.png` & `plib3.ui-0.15.8.2/plib/ui/images/rollback-pyside2.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/apply-gtk.png` & `plib3.ui-0.15.8.2/plib/ui/images/apply-gtk.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_copy-qt4.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_copy-qt4.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_cut-pyside2.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_cut-pyside2.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/exit-qt4.png` & `plib3.ui-0.15.8.2/plib/ui/images/exit-qt4.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/about_toolkit-qt5.png` & `plib3.ui-0.15.8.2/plib/ui/images/about_toolkit-qt5.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_saveas-pyside.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_saveas-pyside.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/refresh-qt4.png` & `plib3.ui-0.15.8.2/plib/ui/images/refresh-qt4.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/apply-posix.png` & `plib3.ui-0.15.8.2/plib/ui/images/apply-posix.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit-win32.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit-win32.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/remove-darwin.png` & `plib3.ui-0.15.8.2/plib/ui/images/remove-darwin.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_delete-wx.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_delete-wx.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/about_toolkit-pyside2.png` & `plib3.ui-0.15.8.2/plib/ui/images/about_toolkit-pyside2.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/commit-pyside2.png` & `plib3.ui-0.15.8.2/plib/ui/images/commit-pyside2.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/about-darwin.png` & `plib3.ui-0.15.8.2/plib/ui/images/about-darwin.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_cut-posix.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_cut-posix.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/about-gtk.png` & `plib3.ui-0.15.8.2/plib/ui/images/about-gtk.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_delete-posix.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_delete-posix.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_saveas-gtk.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_saveas-gtk.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/exit-wx.png` & `plib3.ui-0.15.8.2/plib/ui/images/exit-wx.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_close-wx.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_close-wx.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/view-darwin.png` & `plib3.ui-0.15.8.2/plib/ui/images/view-darwin.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_save-pyside.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_save-pyside.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_redo-qt4.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_redo-qt4.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_open-pyside.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_open-pyside.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_cut-gtk.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_cut-gtk.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_redo-wx.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_redo-wx.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_paste-qt4.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_paste-qt4.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/exit-posix.png` & `plib3.ui-0.15.8.2/plib/ui/images/exit-posix.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/ok-qt4.png` & `plib3.ui-0.15.8.2/plib/ui/images/ok-qt4.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_saveas-wx.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_saveas-wx.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_delete-gtk.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_delete-gtk.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit-pyside2.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit-pyside2.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_cut-pyside.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_cut-pyside.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/apply-kde4.png` & `plib3.ui-0.15.8.2/plib/ui/images/apply-kde4.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/exit-darwin.png` & `plib3.ui-0.15.8.2/plib/ui/images/exit-darwin.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/refresh-pyside2.png` & `plib3.ui-0.15.8.2/plib/ui/images/refresh-pyside2.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/refresh-win32.png` & `plib3.ui-0.15.8.2/plib/ui/images/refresh-win32.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_new-win32.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_new-win32.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/cancel-wx.png` & `plib3.ui-0.15.8.2/plib/ui/images/cancel-wx.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/exit-pyside2.png` & `plib3.ui-0.15.8.2/plib/ui/images/exit-pyside2.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/apply-wx.png` & `plib3.ui-0.15.8.2/plib/ui/images/apply-wx.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/apply-pyside2.png` & `plib3.ui-0.15.8.2/plib/ui/images/apply-pyside2.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/exit-pyside.png` & `plib3.ui-0.15.8.2/plib/ui/images/exit-pyside.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit-gtk.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit-gtk.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/prefs-win32.png` & `plib3.ui-0.15.8.2/plib/ui/images/prefs-win32.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_selectall-wx.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_selectall-wx.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/ok-pyside2.png` & `plib3.ui-0.15.8.2/plib/ui/images/ok-pyside2.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_new-gtk.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_new-gtk.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_cut-qt4.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_cut-qt4.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_save-gtk.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_save-gtk.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_selectall-gtk.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_selectall-gtk.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/remove-qt4.png` & `plib3.ui-0.15.8.2/plib/ui/images/remove-qt4.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/refresh-darwin.png` & `plib3.ui-0.15.8.2/plib/ui/images/refresh-darwin.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/about-pyside.png` & `plib3.ui-0.15.8.2/plib/ui/images/about-pyside.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_selectall-posix.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_selectall-posix.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/about_toolkit-qt.png` & `plib3.ui-0.15.8.2/plib/ui/images/about_toolkit-qt.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/rollback-posix.png` & `plib3.ui-0.15.8.2/plib/ui/images/rollback-posix.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/ok-pyside.png` & `plib3.ui-0.15.8.2/plib/ui/images/ok-pyside.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_close-pyside2.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_close-pyside2.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/cancel-gtk.png` & `plib3.ui-0.15.8.2/plib/ui/images/cancel-gtk.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/add-posix.png` & `plib3.ui-0.15.8.2/plib/ui/images/add-posix.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_delete-pyside.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_delete-pyside.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/view-win32.png` & `plib3.ui-0.15.8.2/plib/ui/images/view-win32.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/exit-win32.png` & `plib3.ui-0.15.8.2/plib/ui/images/exit-win32.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/ok-wx.png` & `plib3.ui-0.15.8.2/plib/ui/images/ok-wx.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_cut-wx.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_cut-wx.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_redo-posix.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_redo-posix.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_save-qt4.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_save-qt4.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/about_toolkit-pyside.png` & `plib3.ui-0.15.8.2/plib/ui/images/about_toolkit-pyside.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_save-darwin.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_save-darwin.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/add-qt4.png` & `plib3.ui-0.15.8.2/plib/ui/images/add-qt4.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_undo-pyside.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_undo-pyside.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_overwrite-posix.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_overwrite-posix.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/add-darwin.png` & `plib3.ui-0.15.8.2/plib/ui/images/add-darwin.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/add-gtk.png` & `plib3.ui-0.15.8.2/plib/ui/images/add-gtk.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_save-wx.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_save-wx.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_paste-gtk.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_paste-gtk.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_saveas-qt4.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_saveas-qt4.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_close-gtk.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_close-gtk.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_undo-pyside2.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_undo-pyside2.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/about_toolkit-qt4.png` & `plib3.ui-0.15.8.2/plib/ui/images/about_toolkit-qt4.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_open-posix.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_open-posix.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_undo-wx.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_undo-wx.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/add-pyside.png` & `plib3.ui-0.15.8.2/plib/ui/images/add-pyside.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/refresh-posix.png` & `plib3.ui-0.15.8.2/plib/ui/images/refresh-posix.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/cancel-pyside.png` & `plib3.ui-0.15.8.2/plib/ui/images/cancel-pyside.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_paste-pyside.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_paste-pyside.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/view-posix.png` & `plib3.ui-0.15.8.2/plib/ui/images/view-posix.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_redo-pyside2.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_redo-pyside2.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_open-qt4.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_open-qt4.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_saveas-posix.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_saveas-posix.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_delete-pyside2.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_delete-pyside2.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_open-wx.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_open-wx.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/about_toolkit-kde.png` & `plib3.ui-0.15.8.2/plib/ui/images/about_toolkit-kde.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/about-qt5.png` & `plib3.ui-0.15.8.2/plib/ui/images/about-qt5.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/ok-posix.png` & `plib3.ui-0.15.8.2/plib/ui/images/ok-posix.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_delete-qt4.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_delete-qt4.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/prefs-gtk.png` & `plib3.ui-0.15.8.2/plib/ui/images/prefs-gtk.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_copy-posix.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_copy-posix.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_new-darwin.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_new-darwin.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/prefs-posix.png` & `plib3.ui-0.15.8.2/plib/ui/images/prefs-posix.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/refresh-pyside.png` & `plib3.ui-0.15.8.2/plib/ui/images/refresh-pyside.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_selectnone-posix.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_selectnone-posix.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/about-wx.png` & `plib3.ui-0.15.8.2/plib/ui/images/about-wx.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_undo-gtk.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_undo-gtk.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_new-pyside.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_new-pyside.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/cancel-posix.png` & `plib3.ui-0.15.8.2/plib/ui/images/cancel-posix.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/ok-gtk.png` & `plib3.ui-0.15.8.2/plib/ui/images/ok-gtk.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_new-pyside2.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_new-pyside2.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_copy-gtk.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_copy-gtk.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_paste-wx.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_paste-wx.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_saveas-win32.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_saveas-win32.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_saveas-darwin.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_saveas-darwin.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit_undo-posix.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit_undo-posix.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_close-qt4.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_close-qt4.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_save-pyside2.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_save-pyside2.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/edit-qt4.png` & `plib3.ui-0.15.8.2/plib/ui/images/edit-qt4.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_open-pyside2.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_open-pyside2.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_new-posix.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_new-posix.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/images/file_open-win32.png` & `plib3.ui-0.15.8.2/plib/ui/images/file_open-win32.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/app.py` & `plib3.ui-0.15.8.2/plib/ui/app.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/fileaware.py` & `plib3.ui-0.15.8.2/plib/ui/fileaware.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/plib/ui/common.py` & `plib3.ui-0.15.8.2/plib/ui/common.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/examples/pyidserver/pyidserver-ui3.py` & `plib3.ui-0.15.8.2/examples/pyidserver/pyidserver-ui3.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/examples/pyidserver/pyidserver.png` & `plib3.ui-0.15.8.2/examples/pyidserver/pyidserver.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/examples/pnotepad/pnotepad3.py` & `plib3.ui-0.15.8.2/examples/pnotepad/pnotepad3.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/examples/pnotepad/pnotepad.png` & `plib3.ui-0.15.8.2/examples/pnotepad/pnotepad.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/examples/scrips/scrips.png` & `plib3.ui-0.15.8.2/examples/scrips/scrips.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/examples/scrips/scrips-edit3.py` & `plib3.ui-0.15.8.2/examples/scrips/scrips-edit3.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/examples/pimgview/pimgview3.py` & `plib3.ui-0.15.8.2/examples/pimgview/pimgview3.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/examples/pimgview/rotate_left.png` & `plib3.ui-0.15.8.2/examples/pimgview/rotate_left.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/examples/pimgview/pimgview.png` & `plib3.ui-0.15.8.2/examples/pimgview/pimgview.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/examples/pimgview/rotate_right.png` & `plib3.ui-0.15.8.2/examples/pimgview/rotate_right.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/examples/ui/ui-signals3.py` & `plib3.ui-0.15.8.2/examples/ui/ui-signals3.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/examples/ui/ui-text3.py` & `plib3.ui-0.15.8.2/examples/ui/ui-text3.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/examples/ui/ui-display3.py` & `plib3.ui-0.15.8.2/examples/ui/ui-display3.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/examples/pxmlview/pxmlview3.py` & `plib3.ui-0.15.8.2/examples/pxmlview/pxmlview3.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/examples/pxmlview/pxmlview.png` & `plib3.ui-0.15.8.2/examples/pxmlview/pxmlview.png`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/examples/container/graphics3.py` & `plib3.ui-0.15.8.2/examples/container/graphics3.py`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/LICENSE.txt` & `plib3.ui-0.15.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/README.rst` & `plib3.ui-0.15.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/PKG-INFO` & `plib3.ui-0.15.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plib3.ui
-Version: 0.15.8.1
+Version: 0.15.8.2
 Summary: A simple Python 3 UI framework.
 Home-page: http://pypi.org/project/plib3.ui
 Author: Peter A. Donis
 Author-email: peterdonis@alum.mit.edu
 License: GPLv2
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `plib3.ui-0.15.8.1/setup.cfg` & `plib3.ui-0.15.8.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `plib3.ui-0.15.8.1/CHANGES.rst` & `plib3.ui-0.15.8.2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 plib3.ui Change Log
 ===================
 
+Version 0.15.8.2
+----------------
+
+- Fix bug in signal handling for ``PNumEditBox`` in wx toolkit.
+
 Version 0.15.8.1
 ----------------
 
 - Added note in ``README`` explaining why example programs are
   installed as console scripts instead of GUI scripts.
 
 - Updated TODO to remove items implemented in version 0.15.8.
```

