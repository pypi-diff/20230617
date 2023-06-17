# Comparing `tmp/terminal_typing_tutor-0.3.0.tar.gz` & `tmp/terminal_typing_tutor-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminal_typing_tutor-0.3.0.tar", max compression
+gzip compressed data, was "terminal_typing_tutor-0.3.1.tar", max compression
```

## Comparing `terminal_typing_tutor-0.3.0.tar` & `terminal_typing_tutor-0.3.1.tar`

### file list

```diff
@@ -1,120 +1,120 @@
--rw-r--r--   0        0        0    35149 2023-06-11 22:25:13.467755 terminal_typing_tutor-0.3.0/LICENSE
--rw-r--r--   0        0        0     2927 2023-06-11 22:34:08.347744 terminal_typing_tutor-0.3.0/README.md
--rw-r--r--   0        0        0      798 2023-06-11 22:48:19.751726 terminal_typing_tutor-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       69 2023-06-11 21:09:06.071850 terminal_typing_tutor-0.3.0/terminal_typing_tutor/__init__.py
--rw-r--r--   0        0        0       31 2023-06-11 04:25:58.607685 terminal_typing_tutor-0.3.0/terminal_typing_tutor/__main__.py
--rw-r--r--   0        0        0     1565 2023-06-11 22:45:19.419730 terminal_typing_tutor-0.3.0/terminal_typing_tutor/constants.py
--rwxr-xr-x   0        0        0      201 2023-06-11 04:11:52.927703 terminal_typing_tutor-0.3.0/terminal_typing_tutor/main.py
--rw-r--r--   0        0        0     3364 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/M/1/data.yaml
--rw-r--r--   0        0        0     3377 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/M/10/data.yaml
--rw-r--r--   0        0        0     4191 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/M/11/data.yaml
--rw-r--r--   0        0        0     2861 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/M/2/data.yaml
--rw-r--r--   0        0        0     3201 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/M/3/data.yaml
--rw-r--r--   0        0        0     2680 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/M/4/data.yaml
--rw-r--r--   0        0        0     3175 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/M/5/data.yaml
--rw-r--r--   0        0        0     3017 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/M/6/data.yaml
--rw-r--r--   0        0        0     2591 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/M/7/data.yaml
--rw-r--r--   0        0        0     3028 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/M/8/data.yaml
--rw-r--r--   0        0        0     3861 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/M/9/data.yaml
--rw-r--r--   0        0        0        3 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/M/lesson_count
--rw-r--r--   0        0        0    36212 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/M/m.typ
--rw-r--r--   0        0        0      520 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/M/menu.json
--rw-r--r--   0        0        0       14 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/M/title
--rw-r--r--   0        0        0     5885 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/Q/1/data.yaml
--rw-r--r--   0        0        0     2445 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/Q/2/data.yaml
--rw-r--r--   0        0        0     3099 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/Q/3/data.yaml
--rw-r--r--   0        0        0     3034 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/Q/4/data.yaml
--rw-r--r--   0        0        0     2004 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/Q/5/data.yaml
--rw-r--r--   0        0        0        2 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/Q/lesson_count
--rw-r--r--   0        0        0      293 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/Q/menu.json
--rw-r--r--   0        0        0    16803 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/Q/q.typ
--rw-r--r--   0        0        0       20 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/Q/title
--rw-r--r--   0        0        0     2650 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/R/1/data.yaml
--rw-r--r--   0        0        0     3389 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/R/10/data.yaml
--rw-r--r--   0        0        0     2608 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/R/11/data.yaml
--rw-r--r--   0        0        0     2975 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/R/12/data.yaml
--rw-r--r--   0        0        0     2659 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/R/13/data.yaml
--rw-r--r--   0        0        0     3307 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/R/14/data.yaml
--rw-r--r--   0        0        0     2721 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/R/2/data.yaml
--rw-r--r--   0        0        0     3181 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/R/3/data.yaml
--rw-r--r--   0        0        0     2764 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/R/4/data.yaml
--rw-r--r--   0        0        0     3166 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/R/5/data.yaml
--rw-r--r--   0        0        0     2920 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/R/6/data.yaml
--rw-r--r--   0        0        0     2852 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/R/7/data.yaml
--rw-r--r--   0        0        0     3119 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/R/8/data.yaml
--rw-r--r--   0        0        0     3491 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/R/9/data.yaml
--rw-r--r--   0        0        0        3 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/R/lesson_count
--rw-r--r--   0        0        0      672 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/R/menu.json
--rw-r--r--   0        0        0    41316 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/R/r.typ
--rw-r--r--   0        0        0       19 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/R/title
--rw-r--r--   0        0        0     2762 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/S/1/data.yaml
--rw-r--r--   0        0        0     3364 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/S/2/data.yaml
--rw-r--r--   0        0        0     4005 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/S/3/data.yaml
--rw-r--r--   0        0        0     6793 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/S/4/data.yaml
--rw-r--r--   0        0        0        2 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/S/lesson_count
--rw-r--r--   0        0        0      203 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/S/menu.json
--rw-r--r--   0        0        0    18263 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/S/s.typ
--rw-r--r--   0        0        0       13 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/S/title
--rw-r--r--   0        0        0     4694 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/1/data.yaml
--rw-r--r--   0        0        0     4139 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/10/data.yaml
--rw-r--r--   0        0        0     3081 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/11/data.yaml
--rw-r--r--   0        0        0     3842 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/12/data.yaml
--rw-r--r--   0        0        0      741 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/13/data.yaml
--rw-r--r--   0        0        0     1669 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/14/data.yaml
--rw-r--r--   0        0        0     3331 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/15/data.yaml
--rw-r--r--   0        0        0     3828 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/16/data.yaml
--rw-r--r--   0        0        0     2344 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/2/data.yaml
--rw-r--r--   0        0        0     3296 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/3/data.yaml
--rw-r--r--   0        0        0     2254 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/4/data.yaml
--rw-r--r--   0        0        0     2633 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/5/data.yaml
--rw-r--r--   0        0        0     2227 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/6/data.yaml
--rw-r--r--   0        0        0     3282 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/7/data.yaml
--rw-r--r--   0        0        0     3137 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/8/data.yaml
--rw-r--r--   0        0        0     2791 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/9/data.yaml
--rw-r--r--   0        0        0        3 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/lesson_count
--rw-r--r--   0        0        0      932 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/menu.json
--rw-r--r--   0        0        0    40881 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/t.typ
--rw-r--r--   0        0        0       20 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/title
--rw-r--r--   0        0        0      416 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/U/1/data.yaml
--rw-r--r--   0        0        0     1376 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/U/10/data.yaml
--rw-r--r--   0        0        0     1324 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/U/11/data.yaml
--rw-r--r--   0        0        0     1400 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/U/12/data.yaml
--rw-r--r--   0        0        0     3117 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/U/13/data.yaml
--rw-r--r--   0        0        0      996 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/U/2/data.yaml
--rw-r--r--   0        0        0     1295 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/U/3/data.yaml
--rw-r--r--   0        0        0      631 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/U/4/data.yaml
--rw-r--r--   0        0        0     1119 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/U/5/data.yaml
--rw-r--r--   0        0        0     1166 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/U/6/data.yaml
--rw-r--r--   0        0        0     1189 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/U/7/data.yaml
--rw-r--r--   0        0        0     1239 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/U/8/data.yaml
--rw-r--r--   0        0        0     1343 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/U/9/data.yaml
--rw-r--r--   0        0        0        3 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/U/lesson_count
--rw-r--r--   0        0        0     1030 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/U/menu.json
--rw-r--r--   0        0        0       15 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/U/title
--rw-r--r--   0        0        0    19159 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/U/u.typ
--rw-r--r--   0        0        0      581 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/1/data.yaml
--rw-r--r--   0        0        0     2382 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/10/data.yaml
--rw-r--r--   0        0        0     2467 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/11/data.yaml
--rw-r--r--   0        0        0     2535 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/12/data.yaml
--rw-r--r--   0        0        0     2915 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/13/data.yaml
--rw-r--r--   0        0        0     3006 2023-06-11 03:21:12.343766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/14/data.yaml
--rw-r--r--   0        0        0     5525 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/15/data.yaml
--rw-r--r--   0        0        0     3465 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/16/data.yaml
--rw-r--r--   0        0        0     3747 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/17/data.yaml
--rw-r--r--   0        0        0     3711 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/18/data.yaml
--rw-r--r--   0        0        0     2927 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/19/data.yaml
--rw-r--r--   0        0        0     1598 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/2/data.yaml
--rw-r--r--   0        0        0     2077 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/3/data.yaml
--rw-r--r--   0        0        0     1873 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/4/data.yaml
--rw-r--r--   0        0        0     2103 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/5/data.yaml
--rw-r--r--   0        0        0     1831 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/6/data.yaml
--rw-r--r--   0        0        0     2071 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/7/data.yaml
--rw-r--r--   0        0        0     1780 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/8/data.yaml
--rw-r--r--   0        0        0     2053 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/9/data.yaml
--rw-r--r--   0        0        0        3 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/lesson_count
--rw-r--r--   0        0        0     1295 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/menu.json
--rw-r--r--   0        0        0       16 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/title
--rw-r--r--   0        0        0    47250 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/v.typ
--rw-r--r--   0        0        0    18422 2023-06-11 22:45:09.643730 terminal_typing_tutor-0.3.0/terminal_typing_tutor/tutor.py
--rw-r--r--   0        0        0       95 2023-06-11 22:43:02.971733 terminal_typing_tutor-0.3.0/terminal_typing_tutor/update.json
--rw-r--r--   0        0        0     4009 1970-01-01 00:00:00.000000 terminal_typing_tutor-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-11 22:25:13.467755 terminal_typing_tutor-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2943 2023-06-13 00:49:15.307992 terminal_typing_tutor-0.3.1/README.md
+-rw-r--r--   0        0        0      798 2023-06-17 00:49:27.391971 terminal_typing_tutor-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-06-11 21:09:06.071850 terminal_typing_tutor-0.3.1/terminal_typing_tutor/__init__.py
+-rw-r--r--   0        0        0       31 2023-06-11 04:25:58.607685 terminal_typing_tutor-0.3.1/terminal_typing_tutor/__main__.py
+-rw-r--r--   0        0        0     1565 2023-06-17 00:49:07.415971 terminal_typing_tutor-0.3.1/terminal_typing_tutor/constants.py
+-rwxr-xr-x   0        0        0      201 2023-06-11 04:11:52.927703 terminal_typing_tutor-0.3.1/terminal_typing_tutor/main.py
+-rw-r--r--   0        0        0     3364 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/M/1/data.yaml
+-rw-r--r--   0        0        0     3377 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/M/10/data.yaml
+-rw-r--r--   0        0        0     4191 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/M/11/data.yaml
+-rw-r--r--   0        0        0     2861 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/M/2/data.yaml
+-rw-r--r--   0        0        0     3201 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/M/3/data.yaml
+-rw-r--r--   0        0        0     2680 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/M/4/data.yaml
+-rw-r--r--   0        0        0     3175 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/M/5/data.yaml
+-rw-r--r--   0        0        0     3017 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/M/6/data.yaml
+-rw-r--r--   0        0        0     2591 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/M/7/data.yaml
+-rw-r--r--   0        0        0     3028 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/M/8/data.yaml
+-rw-r--r--   0        0        0     3861 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/M/9/data.yaml
+-rw-r--r--   0        0        0        3 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/M/lesson_count
+-rw-r--r--   0        0        0    36212 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/M/m.typ
+-rw-r--r--   0        0        0      520 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/M/menu.json
+-rw-r--r--   0        0        0       14 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/M/title
+-rw-r--r--   0        0        0     5885 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/Q/1/data.yaml
+-rw-r--r--   0        0        0     2445 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/Q/2/data.yaml
+-rw-r--r--   0        0        0     3099 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/Q/3/data.yaml
+-rw-r--r--   0        0        0     3034 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/Q/4/data.yaml
+-rw-r--r--   0        0        0     2004 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/Q/5/data.yaml
+-rw-r--r--   0        0        0        2 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/Q/lesson_count
+-rw-r--r--   0        0        0      293 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/Q/menu.json
+-rw-r--r--   0        0        0    16803 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/Q/q.typ
+-rw-r--r--   0        0        0       20 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/Q/title
+-rw-r--r--   0        0        0     2650 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/R/1/data.yaml
+-rw-r--r--   0        0        0     3389 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/R/10/data.yaml
+-rw-r--r--   0        0        0     2608 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/R/11/data.yaml
+-rw-r--r--   0        0        0     2975 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/R/12/data.yaml
+-rw-r--r--   0        0        0     2659 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/R/13/data.yaml
+-rw-r--r--   0        0        0     3307 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/R/14/data.yaml
+-rw-r--r--   0        0        0     2721 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/R/2/data.yaml
+-rw-r--r--   0        0        0     3181 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/R/3/data.yaml
+-rw-r--r--   0        0        0     2764 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/R/4/data.yaml
+-rw-r--r--   0        0        0     3166 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/R/5/data.yaml
+-rw-r--r--   0        0        0     2920 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/R/6/data.yaml
+-rw-r--r--   0        0        0     2852 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/R/7/data.yaml
+-rw-r--r--   0        0        0     3119 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/R/8/data.yaml
+-rw-r--r--   0        0        0     3491 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/R/9/data.yaml
+-rw-r--r--   0        0        0        3 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/R/lesson_count
+-rw-r--r--   0        0        0      672 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/R/menu.json
+-rw-r--r--   0        0        0    41316 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/R/r.typ
+-rw-r--r--   0        0        0       19 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/R/title
+-rw-r--r--   0        0        0     2762 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/S/1/data.yaml
+-rw-r--r--   0        0        0     3364 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/S/2/data.yaml
+-rw-r--r--   0        0        0     4005 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/S/3/data.yaml
+-rw-r--r--   0        0        0     6793 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/S/4/data.yaml
+-rw-r--r--   0        0        0        2 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/S/lesson_count
+-rw-r--r--   0        0        0      203 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/S/menu.json
+-rw-r--r--   0        0        0    18263 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/S/s.typ
+-rw-r--r--   0        0        0       13 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/S/title
+-rw-r--r--   0        0        0     4694 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/1/data.yaml
+-rw-r--r--   0        0        0     4139 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/10/data.yaml
+-rw-r--r--   0        0        0     3081 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/11/data.yaml
+-rw-r--r--   0        0        0     3842 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/12/data.yaml
+-rw-r--r--   0        0        0      741 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/13/data.yaml
+-rw-r--r--   0        0        0     1669 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/14/data.yaml
+-rw-r--r--   0        0        0     3331 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/15/data.yaml
+-rw-r--r--   0        0        0     3828 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/16/data.yaml
+-rw-r--r--   0        0        0     2344 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/2/data.yaml
+-rw-r--r--   0        0        0     3296 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/3/data.yaml
+-rw-r--r--   0        0        0     2254 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/4/data.yaml
+-rw-r--r--   0        0        0     2633 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/5/data.yaml
+-rw-r--r--   0        0        0     2227 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/6/data.yaml
+-rw-r--r--   0        0        0     3282 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/7/data.yaml
+-rw-r--r--   0        0        0     3137 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/8/data.yaml
+-rw-r--r--   0        0        0     2791 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/9/data.yaml
+-rw-r--r--   0        0        0        3 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/lesson_count
+-rw-r--r--   0        0        0      932 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/menu.json
+-rw-r--r--   0        0        0    40881 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/t.typ
+-rw-r--r--   0        0        0       20 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/title
+-rw-r--r--   0        0        0      416 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/U/1/data.yaml
+-rw-r--r--   0        0        0     1376 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/U/10/data.yaml
+-rw-r--r--   0        0        0     1324 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/U/11/data.yaml
+-rw-r--r--   0        0        0     1400 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/U/12/data.yaml
+-rw-r--r--   0        0        0     3117 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/U/13/data.yaml
+-rw-r--r--   0        0        0      996 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/U/2/data.yaml
+-rw-r--r--   0        0        0     1295 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/U/3/data.yaml
+-rw-r--r--   0        0        0      631 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/U/4/data.yaml
+-rw-r--r--   0        0        0     1119 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/U/5/data.yaml
+-rw-r--r--   0        0        0     1166 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/U/6/data.yaml
+-rw-r--r--   0        0        0     1189 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/U/7/data.yaml
+-rw-r--r--   0        0        0     1239 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/U/8/data.yaml
+-rw-r--r--   0        0        0     1343 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/U/9/data.yaml
+-rw-r--r--   0        0        0        3 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/U/lesson_count
+-rw-r--r--   0        0        0     1030 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/U/menu.json
+-rw-r--r--   0        0        0       15 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/U/title
+-rw-r--r--   0        0        0    19159 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/U/u.typ
+-rw-r--r--   0        0        0      581 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/1/data.yaml
+-rw-r--r--   0        0        0     2382 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/10/data.yaml
+-rw-r--r--   0        0        0     2467 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/11/data.yaml
+-rw-r--r--   0        0        0     2535 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/12/data.yaml
+-rw-r--r--   0        0        0     2915 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/13/data.yaml
+-rw-r--r--   0        0        0     3006 2023-06-11 03:21:12.343766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/14/data.yaml
+-rw-r--r--   0        0        0     5525 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/15/data.yaml
+-rw-r--r--   0        0        0     3465 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/16/data.yaml
+-rw-r--r--   0        0        0     3747 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/17/data.yaml
+-rw-r--r--   0        0        0     3711 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/18/data.yaml
+-rw-r--r--   0        0        0     2927 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/19/data.yaml
+-rw-r--r--   0        0        0     1598 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/2/data.yaml
+-rw-r--r--   0        0        0     2077 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/3/data.yaml
+-rw-r--r--   0        0        0     1873 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/4/data.yaml
+-rw-r--r--   0        0        0     2103 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/5/data.yaml
+-rw-r--r--   0        0        0     1831 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/6/data.yaml
+-rw-r--r--   0        0        0     2071 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/7/data.yaml
+-rw-r--r--   0        0        0     1780 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/8/data.yaml
+-rw-r--r--   0        0        0     2053 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/9/data.yaml
+-rw-r--r--   0        0        0        3 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/lesson_count
+-rw-r--r--   0        0        0     1295 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/menu.json
+-rw-r--r--   0        0        0       16 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/title
+-rw-r--r--   0        0        0    47250 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/v.typ
+-rw-r--r--   0        0        0    18413 2023-06-17 00:48:13.095971 terminal_typing_tutor-0.3.1/terminal_typing_tutor/tutor.py
+-rw-r--r--   0        0        0       94 2023-06-17 00:48:16.395971 terminal_typing_tutor-0.3.1/terminal_typing_tutor/update.json
+-rw-r--r--   0        0        0     4025 1970-01-01 00:00:00.000000 terminal_typing_tutor-0.3.1/PKG-INFO
```

### Comparing `terminal_typing_tutor-0.3.0/LICENSE` & `terminal_typing_tutor-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/README.md` & `terminal_typing_tutor-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 ## Install
 
 in your terminal:
 
 ```
 $ pip install --user terminal-typing-tutor
 ---> 100%
-Successfully installed typer
+Successfully installed terminal-typing-tutor
 
 $ ttt
 ```
 
 upgrade:
 
 ```
```

### Comparing `terminal_typing_tutor-0.3.0/pyproject.toml` & `terminal_typing_tutor-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "terminal-typing-tutor"
-version = "0.3.0"
+version = "0.3.1"
 description = "Improve your touch-typing skills in the terminal, based on the GNU Typist program"
 authors = ["Justin Angeles <justinaawd@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-only"
 homepage = "https://github.com/justinsgithub/terminal-typing-tutor"
 repository = "https://github.com/justinsgithub/terminal-typing-tutor"
 documentation = "https://github.com/justinsgithub/terminal-typing-tutor"
```

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/constants.py` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from blessed import Terminal
 from typing import Literal, TypedDict
 
-CURRENT_VERSION = "0.3.0"
+CURRENT_VERSION = "0.3.1"
 
 MAIN_MENU_TITLE = "Series selection menu"
 
 MAIN_MENU = [
     {
         "title": "Series Q    Quick QWERTY course  (Q1 - Q5) ",
         "series": "Q",
```

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/M/1/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/M/1/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/M/10/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/M/10/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/M/11/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/M/11/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/M/2/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/M/2/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/M/3/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/M/3/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/M/4/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/M/4/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/M/5/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/M/5/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/M/6/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/M/6/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/M/7/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/M/7/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/M/8/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/M/8/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/M/9/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/M/9/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/M/m.typ` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/M/m.typ`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/M/menu.json` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/M/menu.json`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/Q/1/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/Q/1/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/Q/2/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/Q/2/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/Q/3/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/Q/3/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/Q/4/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/Q/4/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/Q/5/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/Q/5/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/Q/q.typ` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/Q/q.typ`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/R/1/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/R/1/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/R/10/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/R/10/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/R/11/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/R/11/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/R/12/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/R/12/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/R/13/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/R/13/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/R/14/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/R/14/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/R/2/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/R/2/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/R/3/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/R/3/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/R/4/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/R/4/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/R/5/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/R/5/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/R/6/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/R/6/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/R/7/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/R/7/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/R/8/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/R/8/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/R/9/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/R/9/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/R/menu.json` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/R/menu.json`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/R/r.typ` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/R/r.typ`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/S/1/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/S/1/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/S/2/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/S/2/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/S/3/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/S/3/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/S/4/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/S/4/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/S/s.typ` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/S/s.typ`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/1/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/1/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/10/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/10/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/11/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/11/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/12/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/12/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/13/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/13/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/14/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/14/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/15/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/15/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/16/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/16/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/2/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/2/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/3/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/3/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/4/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/4/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/5/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/5/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/6/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/6/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/7/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/7/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/8/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/8/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/9/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/9/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/menu.json` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/menu.json`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/T/t.typ` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/T/t.typ`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/U/10/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/U/10/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/U/11/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/U/11/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/U/12/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/U/12/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/U/13/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/U/13/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/U/2/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/U/2/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/U/3/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/U/3/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/U/4/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/U/4/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/U/5/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/U/5/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/U/6/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/U/6/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/U/7/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/U/7/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/U/8/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/U/8/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/U/9/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/U/9/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/U/menu.json` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/U/menu.json`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/U/u.typ` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/U/u.typ`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/1/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/1/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/10/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/10/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/11/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/11/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/12/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/12/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/13/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/13/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/14/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/14/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/15/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/15/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/16/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/16/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/17/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/17/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/18/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/18/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/19/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/19/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/2/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/2/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/3/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/3/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/4/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/4/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/5/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/5/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/6/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/6/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/7/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/7/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/8/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/8/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/9/data.yaml` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/9/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/menu.json` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/menu.json`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/series/V/v.typ` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/series/V/v.typ`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.3.0/terminal_typing_tutor/tutor.py` & `terminal_typing_tutor-0.3.1/terminal_typing_tutor/tutor.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,29 +207,24 @@
                 return "menu"
             if key.lower() == "n" and confirming_exit:
                 print(HOME + XY(0, HEIGHT), end="", flush=True)
                 print( TERM.black_on_white( " Press R to repeat, N for next exercise or E to exit "), end="", flush=True,)
                 confirming_exit = False
 
 
-def pressed_key(key: Keystroke, target_character: str):
-    line_break = target_character == "\n"
-    pressed_enter = key.name == "KEY_ENTER"
-    pressed_space = key == " "
-    if (key == target_character) or (line_break and pressed_enter):
-        return {
+def pressed_info(key: Keystroke, target_char: str):
+    pressed_space = key == ' '
+    pressed_enter = key.name == 'KEY_ENTER' 
+    hit_target = key == target_char or (pressed_enter and target_char == '\n') 
+
+    return {
             "pressed_enter": pressed_enter,
             "pressed_space": pressed_space,
-            "hit_target": True,
-        }
-    return {
-        "pressed_enter": pressed_enter,
-        "pressed_space": pressed_space,
-        "hit_target": False,
-    }
+            "hit_target": hit_target,
+            }
 
 def print_lines(test_string: str) -> int:
     lines = test_string.split("\n")
     line_count = len(lines)
     longest_line = lines[0]
     for line in lines:
         if len(line) > len(longest_line):
@@ -267,45 +262,48 @@
     while True:
         # first check to see if all characters typed, end drill
         if len(correct_pressed_keys) == len(test_string):
             action = end_drill(start_time, test_string, incorrect_pressed_keys)
             return action
 
         target_character = test_string[len(correct_pressed_keys)]
-        print(f"{TERM.black_on_white(target_character)}{LEFT(1)}", end="", flush=True)
+        if target_character == '\n':
+            print(f"{TERM.white_on_white('x')}{LEFT(1)}", end="", flush=True)
+        else:
+            print(f"{TERM.black_on_white(target_character)}{LEFT(1)}", end="", flush=True)
         key = get_key()
 
         if key.name == "KEY_ESCAPE":
             # start test over if in middle of test, else confirm exit
             if drill_started:
                 return "repeat"
             else:
                 action = end_drill(0.0, test_string, incorrect_pressed_keys)
                 return action
 
-        _pressed_key = pressed_key(key, target_character)
+        pressed_key = pressed_info(key, target_character)
 
         # Set the start time on first key press
         if drill_started == False:
             start_time = time.time()
             drill_started = True
 
-        if _pressed_key["hit_target"]:
+        if pressed_key["hit_target"]:
             if pressed_wrong_key == False:
-                if not _pressed_key["pressed_enter"]:
-                    print(TERM.green(key), end="", flush=True)
+                if pressed_key["pressed_enter"]:
+                    print(f" \n{X(left_padding)}", end="", flush=True)
                 else:
-                    print(f"{TERM.green(key)}{RIGHT(left_padding)}", end="", flush=True)
+                    print(TERM.green(key), end="", flush=True)
 
             if pressed_wrong_key == True:
-                if _pressed_key["pressed_space"]:
+                if pressed_key["pressed_space"]:
                     print(TERM.red_on_red("x"), end="", flush=True)
-                elif _pressed_key["pressed_enter"]:
+                elif pressed_key["pressed_enter"]:
                     # may not want down here
-                    print(TERM.red_on_red("x"))
+                    print(f"{TERM.red_on_red('x')}\n{X(left_padding)}", end="", flush=True)
                 else:
                     print(TERM.red(key), end="", flush=True)
 
             correct_pressed_keys.append(key)
             pressed_wrong_key = False
 
         else:
@@ -508,21 +506,22 @@
     Path(__file__).parent.joinpath("update.json").write_text(update_data_to_dump)
     if update["available"] and (update["last_shown"] == "" or days_difference(update["last_shown"],today) >= 2):
         update["last_shown"] = today
         update_data_to_dump = json.dumps(update)
         Path(__file__).parent.joinpath("update.json").write_text(update_data_to_dump)
         print(f"\n\n{TERM.green('Upgrade available!')} To upgrade run:\n")
         print(f"pip install --user --upgrade terminal-typing-tutor\n\n")
+
 def tutor():
     """
     runs typing tutor program
     """
     update_check()
-    # with TERM.fullscreen(), TERM.hidden_cursor():
-    with TERM.fullscreen(), TERM.cbreak(), TERM.hidden_cursor():  # hidden cursor off during development
+    with TERM.fullscreen(), TERM.cbreak():  # hidden cursor off during development
+    # with TERM.fullscreen(), TERM.cbreak(), TERM.hidden_cursor():
         num = 0
         while True:
             if num == 0:
                 run_series_menu()
                 num = run_lesson()
             if num == 1:
                 exit()
```

### Comparing `terminal_typing_tutor-0.3.0/PKG-INFO` & `terminal_typing_tutor-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminal-typing-tutor
-Version: 0.3.0
+Version: 0.3.1
 Summary: Improve your touch-typing skills in the terminal, based on the GNU Typist program
 Home-page: https://github.com/justinsgithub/terminal-typing-tutor
 License: GPL-3.0-only
 Author: Justin Angeles
 Author-email: justinaawd@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -48,15 +48,15 @@
 ## Install
 
 in your terminal:
 
 ```
 $ pip install --user terminal-typing-tutor
 ---> 100%
-Successfully installed typer
+Successfully installed terminal-typing-tutor
 
 $ ttt
 ```
 
 upgrade:
 
 ```
```

