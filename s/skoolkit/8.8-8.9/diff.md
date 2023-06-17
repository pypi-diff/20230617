# Comparing `tmp/skoolkit-8.8.tar.gz` & `tmp/skoolkit-8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skoolkit-8.8.tar", last modified: Sat Nov 19 13:34:18 2022, max compression
+gzip compressed data, was "skoolkit-8.9.tar", last modified: Sun Feb 19 13:05:11 2023, max compression
```

## Comparing `skoolkit-8.8.tar` & `skoolkit-8.9.tar`

### file list

```diff
@@ -1,231 +1,233 @@
-drwxr-xr-x   0 rjd       (1000) rjd       (1000)        0 2022-11-19 13:34:18.088618 skoolkit-8.8/
--rw-r--r--   0 rjd       (1000) rjd       (1000)    35147 2010-03-03 00:59:14.000000 skoolkit-8.8/COPYING
--rw-r--r--   0 rjd       (1000) rjd       (1000)       64 2014-12-31 18:28:35.000000 skoolkit-8.8/MANIFEST.in
--rw-r--r--   0 rjd       (1000) rjd       (1000)     6711 2022-11-19 13:34:18.088618 skoolkit-8.8/PKG-INFO
--rwxr-xr-x   0 rjd       (1000) rjd       (1000)      886 2017-01-12 22:31:18.000000 skoolkit-8.8/bin2sna.py
--rwxr-xr-x   0 rjd       (1000) rjd       (1000)      892 2017-01-12 22:31:18.000000 skoolkit-8.8/bin2tap.py
-drwxr-xr-x   0 rjd       (1000) rjd       (1000)        0 2022-11-19 13:34:18.068618 skoolkit-8.8/docs/
-drwxr-xr-x   0 rjd       (1000) rjd       (1000)        0 2022-11-19 13:34:18.068618 skoolkit-8.8/docs/_sources/
--rw-r--r--   0 rjd       (1000) rjd       (1000)     4165 2022-08-12 20:16:11.000000 skoolkit-8.8/docs/_sources/asm-templates.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)    51542 2022-09-19 23:34:08.000000 skoolkit-8.8/docs/_sources/asm.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)     2862 2019-05-14 21:07:25.000000 skoolkit-8.8/docs/_sources/assemblers.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)    15794 2022-11-19 13:22:43.000000 skoolkit-8.8/docs/_sources/changelog.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)     3491 2015-11-20 12:50:08.000000 skoolkit-8.8/docs/_sources/changelog1.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)    11437 2019-07-08 20:36:08.000000 skoolkit-8.8/docs/_sources/changelog2.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)    11778 2019-07-08 20:36:08.000000 skoolkit-8.8/docs/_sources/changelog3.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)     7233 2020-10-07 20:20:25.000000 skoolkit-8.8/docs/_sources/changelog4.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)     6124 2020-10-07 20:20:25.000000 skoolkit-8.8/docs/_sources/changelog5.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)     9323 2020-10-07 20:20:25.000000 skoolkit-8.8/docs/_sources/changelog6.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)     6307 2020-10-07 20:20:25.000000 skoolkit-8.8/docs/_sources/changelog7.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)    78562 2022-11-14 21:27:35.000000 skoolkit-8.8/docs/_sources/commands.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)    13441 2021-05-18 21:36:14.000000 skoolkit-8.8/docs/_sources/components.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)    32224 2022-08-17 20:15:36.000000 skoolkit-8.8/docs/_sources/control-files.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)    13398 2022-08-18 23:11:24.000000 skoolkit-8.8/docs/_sources/diy.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)    16637 2021-06-23 20:02:28.000000 skoolkit-8.8/docs/_sources/extending.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)    27424 2022-08-29 20:54:25.000000 skoolkit-8.8/docs/_sources/html-templates.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)      426 2019-08-09 20:57:13.000000 skoolkit-8.8/docs/_sources/index.rst.txt
-drwxr-xr-x   0 rjd       (1000) rjd       (1000)        0 2022-11-19 13:34:18.072618 skoolkit-8.8/docs/_sources/man/
--rw-r--r--   0 rjd       (1000) rjd       (1000)     3024 2018-01-05 21:54:04.000000 skoolkit-8.8/docs/_sources/man/bin2sna.py.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)     2923 2020-09-15 20:03:51.000000 skoolkit-8.8/docs/_sources/man/bin2tap.py.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)     7680 2021-05-18 21:36:14.000000 skoolkit-8.8/docs/_sources/man/skool2asm.py.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)     1558 2020-02-25 22:04:07.000000 skoolkit-8.8/docs/_sources/man/skool2bin.py.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)     3065 2021-05-18 21:36:14.000000 skoolkit-8.8/docs/_sources/man/skool2ctl.py.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)     7266 2022-08-08 18:01:45.000000 skoolkit-8.8/docs/_sources/man/skool2html.py.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)     3388 2021-05-18 21:36:14.000000 skoolkit-8.8/docs/_sources/man/sna2ctl.py.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)     2297 2019-07-08 21:10:05.000000 skoolkit-8.8/docs/_sources/man/sna2img.py.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)     6538 2022-09-07 19:43:47.000000 skoolkit-8.8/docs/_sources/man/sna2skool.py.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)     4353 2021-05-18 21:36:14.000000 skoolkit-8.8/docs/_sources/man/snapinfo.py.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)     2305 2017-11-03 20:57:10.000000 skoolkit-8.8/docs/_sources/man/snapmod.py.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)     9172 2022-10-04 20:36:26.000000 skoolkit-8.8/docs/_sources/man/tap2sna.py.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)      916 2020-09-17 20:17:10.000000 skoolkit-8.8/docs/_sources/man/tapinfo.py.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)     3495 2022-11-14 21:27:35.000000 skoolkit-8.8/docs/_sources/man/trace.py.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)     5297 2019-11-05 22:00:31.000000 skoolkit-8.8/docs/_sources/migration.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)     3327 2022-09-19 23:27:01.000000 skoolkit-8.8/docs/_sources/parsing.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)    51648 2022-10-25 12:02:01.000000 skoolkit-8.8/docs/_sources/ref-files.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)    11571 2020-03-08 12:27:23.000000 skoolkit-8.8/docs/_sources/skool-files.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)   115169 2022-10-05 18:39:07.000000 skoolkit-8.8/docs/_sources/skool-macros.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)     2544 2022-07-26 20:00:49.000000 skoolkit-8.8/docs/_sources/usage.rst.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)     4993 2022-11-13 15:52:53.000000 skoolkit-8.8/docs/_sources/whatis.rst.txt
-drwxr-xr-x   0 rjd       (1000) rjd       (1000)        0 2022-11-19 13:34:18.072618 skoolkit-8.8/docs/_static/
--rw-r--r--   0 rjd       (1000) rjd       (1000)    13646 2022-11-19 13:23:35.000000 skoolkit-8.8/docs/_static/basic.css
--rw-r--r--   0 rjd       (1000) rjd       (1000)     4256 2022-11-19 13:23:35.000000 skoolkit-8.8/docs/_static/classic.css
--rw-r--r--   0 rjd       (1000) rjd       (1000)      368 2021-09-12 11:18:57.000000 skoolkit-8.8/docs/_static/custom.css
--rw-r--r--   0 rjd       (1000) rjd       (1000)     9416 2021-01-02 17:13:01.000000 skoolkit-8.8/docs/_static/doctools.js
--rw-r--r--   0 rjd       (1000) rjd       (1000)      353 2022-11-19 13:23:35.000000 skoolkit-8.8/docs/_static/documentation_options.js
--rw-r--r--   0 rjd       (1000) rjd       (1000)      286 2021-01-01 06:53:29.000000 skoolkit-8.8/docs/_static/file.png
--rw-r--r--   0 rjd       (1000) rjd       (1000)   287600 2021-01-12 20:55:26.000000 skoolkit-8.8/docs/_static/jquery.js
--rw-r--r--   0 rjd       (1000) rjd       (1000)    10847 2022-11-19 13:23:35.000000 skoolkit-8.8/docs/_static/language_data.js
--rw-r--r--   0 rjd       (1000) rjd       (1000)       90 2021-01-01 06:53:29.000000 skoolkit-8.8/docs/_static/minus.png
--rw-r--r--   0 rjd       (1000) rjd       (1000)       90 2021-01-01 06:53:29.000000 skoolkit-8.8/docs/_static/plus.png
--rw-r--r--   0 rjd       (1000) rjd       (1000)     4780 2022-11-19 13:23:35.000000 skoolkit-8.8/docs/_static/pygments.css
--rw-r--r--   0 rjd       (1000) rjd       (1000)    16323 2021-01-04 13:20:58.000000 skoolkit-8.8/docs/_static/searchtools.js
--rw-r--r--   0 rjd       (1000) rjd       (1000)     4803 2022-11-19 13:23:35.000000 skoolkit-8.8/docs/_static/sidebar.js
--rw-r--r--   0 rjd       (1000) rjd       (1000)    58881 2021-03-31 12:21:21.000000 skoolkit-8.8/docs/_static/underscore.js
--rw-r--r--   0 rjd       (1000) rjd       (1000)    15265 2022-11-19 13:23:33.000000 skoolkit-8.8/docs/asm-templates.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)   109092 2022-11-19 13:23:33.000000 skoolkit-8.8/docs/asm.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)    10762 2022-11-19 13:23:33.000000 skoolkit-8.8/docs/assemblers.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)    44932 2022-11-19 13:23:33.000000 skoolkit-8.8/docs/changelog.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)    13248 2022-11-19 13:23:33.000000 skoolkit-8.8/docs/changelog1.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)    31682 2022-11-19 13:23:33.000000 skoolkit-8.8/docs/changelog2.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)    31918 2022-11-19 13:23:33.000000 skoolkit-8.8/docs/changelog3.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)    21605 2022-11-19 13:23:33.000000 skoolkit-8.8/docs/changelog4.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)    19904 2022-11-19 13:23:33.000000 skoolkit-8.8/docs/changelog5.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)    28657 2022-11-19 13:23:33.000000 skoolkit-8.8/docs/changelog6.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)    19653 2022-11-19 13:23:34.000000 skoolkit-8.8/docs/changelog7.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)   120019 2022-11-19 13:23:34.000000 skoolkit-8.8/docs/commands.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)    64292 2022-11-19 13:23:34.000000 skoolkit-8.8/docs/components.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)    69665 2022-11-19 13:23:34.000000 skoolkit-8.8/docs/control-files.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)    24938 2022-11-19 13:23:34.000000 skoolkit-8.8/docs/diy.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)    81048 2022-11-19 13:23:34.000000 skoolkit-8.8/docs/extending.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)    15999 2022-11-19 13:23:35.000000 skoolkit-8.8/docs/genindex.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)    66063 2022-11-19 13:23:34.000000 skoolkit-8.8/docs/html-templates.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)     6380 2022-11-19 13:23:34.000000 skoolkit-8.8/docs/index.html
-drwxr-xr-x   0 rjd       (1000) rjd       (1000)        0 2022-11-19 13:34:18.072618 skoolkit-8.8/docs/man/
--rw-r--r--   0 rjd       (1000) rjd       (1000)    13404 2022-11-19 13:23:34.000000 skoolkit-8.8/docs/man/bin2sna.py.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)     9380 2022-11-19 13:23:34.000000 skoolkit-8.8/docs/man/bin2tap.py.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)    23234 2022-11-19 13:23:34.000000 skoolkit-8.8/docs/man/skool2asm.py.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)     8185 2022-11-19 13:23:34.000000 skoolkit-8.8/docs/man/skool2bin.py.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)    11957 2022-11-19 13:23:34.000000 skoolkit-8.8/docs/man/skool2ctl.py.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)    22789 2022-11-19 13:23:34.000000 skoolkit-8.8/docs/man/skool2html.py.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)    11483 2022-11-19 13:23:34.000000 skoolkit-8.8/docs/man/sna2ctl.py.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)     9015 2022-11-19 13:23:34.000000 skoolkit-8.8/docs/man/sna2img.py.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)    20548 2022-11-19 13:23:34.000000 skoolkit-8.8/docs/man/sna2skool.py.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)    13276 2022-11-19 13:23:34.000000 skoolkit-8.8/docs/man/snapinfo.py.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)    12152 2022-11-19 13:23:34.000000 skoolkit-8.8/docs/man/snapmod.py.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)    28730 2022-11-19 13:23:34.000000 skoolkit-8.8/docs/man/tap2sna.py.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)     6471 2022-11-19 13:23:34.000000 skoolkit-8.8/docs/man/tapinfo.py.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)    13370 2022-11-19 13:23:34.000000 skoolkit-8.8/docs/man/trace.py.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)    19592 2022-11-19 13:23:34.000000 skoolkit-8.8/docs/migration.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)    12321 2022-11-19 13:23:34.000000 skoolkit-8.8/docs/parsing.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)     4402 2022-11-19 13:23:35.000000 skoolkit-8.8/docs/py-modindex.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)   104051 2022-11-19 13:23:34.000000 skoolkit-8.8/docs/ref-files.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)     3363 2022-11-19 13:23:35.000000 skoolkit-8.8/docs/search.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)    53229 2022-11-19 13:23:35.000000 skoolkit-8.8/docs/searchindex.js
--rw-r--r--   0 rjd       (1000) rjd       (1000)    25190 2022-11-19 13:23:34.000000 skoolkit-8.8/docs/skool-files.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)   230928 2022-11-19 13:23:35.000000 skoolkit-8.8/docs/skool-macros.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)     9038 2022-11-19 13:23:35.000000 skoolkit-8.8/docs/usage.html
--rw-r--r--   0 rjd       (1000) rjd       (1000)    12910 2022-11-19 13:23:35.000000 skoolkit-8.8/docs/whatis.html
-drwxr-xr-x   0 rjd       (1000) rjd       (1000)        0 2022-11-19 13:34:18.076618 skoolkit-8.8/examples/
--rw-r--r--   0 rjd       (1000) rjd       (1000)     2454 2015-12-04 12:16:10.000000 skoolkit-8.8/examples/hungry_horace.ctl
--rw-r--r--   0 rjd       (1000) rjd       (1000)      696 2016-01-09 11:54:00.000000 skoolkit-8.8/examples/hungry_horace.ref
--rw-r--r--   0 rjd       (1000) rjd       (1000)      214 2022-10-01 14:05:49.000000 skoolkit-8.8/examples/hungry_horace.t2s
-drwxr-xr-x   0 rjd       (1000) rjd       (1000)        0 2022-11-19 13:34:18.060618 skoolkit-8.8/man/
-drwxr-xr-x   0 rjd       (1000) rjd       (1000)        0 2022-11-19 13:34:18.076618 skoolkit-8.8/man/man1/
--rw-r--r--   0 rjd       (1000) rjd       (1000)     4435 2022-11-19 13:23:29.000000 skoolkit-8.8/man/man1/bin2sna.py.1
--rw-r--r--   0 rjd       (1000) rjd       (1000)     4085 2022-11-19 13:23:29.000000 skoolkit-8.8/man/man1/bin2tap.py.1
--rw-r--r--   0 rjd       (1000) rjd       (1000)     9606 2022-11-19 13:23:29.000000 skoolkit-8.8/man/man1/skool2asm.py.1
--rw-r--r--   0 rjd       (1000) rjd       (1000)     2827 2022-11-19 13:23:29.000000 skoolkit-8.8/man/man1/skool2bin.py.1
--rw-r--r--   0 rjd       (1000) rjd       (1000)     4460 2022-11-19 13:23:29.000000 skoolkit-8.8/man/man1/skool2ctl.py.1
--rw-r--r--   0 rjd       (1000) rjd       (1000)     9467 2022-11-19 13:23:29.000000 skoolkit-8.8/man/man1/skool2html.py.1
--rw-r--r--   0 rjd       (1000) rjd       (1000)     4795 2022-11-19 13:23:29.000000 skoolkit-8.8/man/man1/sna2ctl.py.1
--rw-r--r--   0 rjd       (1000) rjd       (1000)     3683 2022-11-19 13:23:29.000000 skoolkit-8.8/man/man1/sna2img.py.1
--rw-r--r--   0 rjd       (1000) rjd       (1000)     8140 2022-11-19 13:23:29.000000 skoolkit-8.8/man/man1/sna2skool.py.1
--rw-r--r--   0 rjd       (1000) rjd       (1000)     5960 2022-11-19 13:23:29.000000 skoolkit-8.8/man/man1/snapinfo.py.1
--rw-r--r--   0 rjd       (1000) rjd       (1000)     3648 2022-11-19 13:23:29.000000 skoolkit-8.8/man/man1/snapmod.py.1
--rw-r--r--   0 rjd       (1000) rjd       (1000)    11117 2022-11-19 13:23:29.000000 skoolkit-8.8/man/man1/tap2sna.py.1
--rw-r--r--   0 rjd       (1000) rjd       (1000)     1971 2022-11-19 13:23:29.000000 skoolkit-8.8/man/man1/tapinfo.py.1
--rw-r--r--   0 rjd       (1000) rjd       (1000)     4974 2022-11-19 13:23:29.000000 skoolkit-8.8/man/man1/trace.py.1
--rw-r--r--   0 rjd       (1000) rjd       (1000)       90 2021-11-16 20:02:53.000000 skoolkit-8.8/pyproject.toml
--rw-r--r--   0 rjd       (1000) rjd       (1000)     1153 2022-11-19 13:34:18.088618 skoolkit-8.8/setup.cfg
--rwxr-xr-x   0 rjd       (1000) rjd       (1000)      896 2017-01-12 22:31:18.000000 skoolkit-8.8/skool2asm.py
--rwxr-xr-x   0 rjd       (1000) rjd       (1000)      891 2017-01-12 22:31:18.000000 skoolkit-8.8/skool2bin.py
--rwxr-xr-x   0 rjd       (1000) rjd       (1000)      896 2017-01-12 22:31:18.000000 skoolkit-8.8/skool2ctl.py
--rwxr-xr-x   0 rjd       (1000) rjd       (1000)      898 2017-01-12 22:31:18.000000 skoolkit-8.8/skool2html.py
-drwxr-xr-x   0 rjd       (1000) rjd       (1000)        0 2022-11-19 13:34:18.080618 skoolkit-8.8/skoolkit/
--rw-r--r--   0 rjd       (1000) rjd       (1000)     6271 2022-11-19 13:22:43.000000 skoolkit-8.8/skoolkit/__init__.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)     5765 2022-11-13 15:54:44.000000 skoolkit-8.8/skoolkit/audio.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    10745 2020-09-03 20:18:52.000000 skoolkit-8.8/skoolkit/basic.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)     4682 2020-02-27 22:10:07.000000 skoolkit-8.8/skoolkit/bin2sna.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)     8940 2020-09-15 20:03:51.000000 skoolkit-8.8/skoolkit/bin2tap.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)     1783 2021-02-03 21:14:45.000000 skoolkit-8.8/skoolkit/components.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)     6360 2022-08-08 20:12:19.000000 skoolkit-8.8/skoolkit/config.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    18478 2022-09-18 12:36:07.000000 skoolkit-8.8/skoolkit/ctlparser.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    16008 2022-10-25 12:02:01.000000 skoolkit-8.8/skoolkit/defaults.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    37276 2021-04-13 20:39:36.000000 skoolkit-8.8/skoolkit/disassembler.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    16581 2021-07-23 19:51:54.000000 skoolkit-8.8/skoolkit/graphics.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    11792 2021-04-25 13:05:19.000000 skoolkit-8.8/skoolkit/image.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)     9687 2022-11-13 12:44:17.000000 skoolkit-8.8/skoolkit/loadtracer.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    36547 2019-01-03 21:48:08.000000 skoolkit-8.8/skoolkit/opcodes.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    21763 2021-02-10 21:01:21.000000 skoolkit-8.8/skoolkit/pngwriter.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)     7744 2021-07-22 20:05:54.000000 skoolkit-8.8/skoolkit/refparser.py
-drwxr-xr-x   0 rjd       (1000) rjd       (1000)        0 2022-11-19 13:34:18.080618 skoolkit-8.8/skoolkit/resources/
--rw-r--r--   0 rjd       (1000) rjd       (1000)    16384 2019-02-10 22:35:13.000000 skoolkit-8.8/skoolkit/resources/48.rom
--rw-r--r--   0 rjd       (1000) rjd       (1000)     1164 2019-07-14 11:45:10.000000 skoolkit-8.8/skoolkit/resources/skoolkit-dark.css
--rw-r--r--   0 rjd       (1000) rjd       (1000)     1164 2019-07-14 11:45:10.000000 skoolkit-8.8/skoolkit/resources/skoolkit-green.css
--rw-r--r--   0 rjd       (1000) rjd       (1000)     1164 2019-07-14 11:45:10.000000 skoolkit-8.8/skoolkit/resources/skoolkit-plum.css
--rw-r--r--   0 rjd       (1000) rjd       (1000)       80 2017-02-15 21:53:32.000000 skoolkit-8.8/skoolkit/resources/skoolkit-wide.css
--rw-r--r--   0 rjd       (1000) rjd       (1000)     3578 2021-01-28 21:19:34.000000 skoolkit-8.8/skoolkit/resources/skoolkit.css
--rw-r--r--   0 rjd       (1000) rjd       (1000)     7710 2022-11-13 15:44:09.000000 skoolkit-8.8/skoolkit/simtables.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)   186540 2022-11-17 21:31:16.000000 skoolkit-8.8/skoolkit/simulator.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)     7940 2021-09-19 12:27:42.000000 skoolkit-8.8/skoolkit/skool2asm.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    14224 2021-05-18 21:36:14.000000 skoolkit-8.8/skoolkit/skool2bin.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)     4790 2019-03-04 21:42:17.000000 skoolkit-8.8/skoolkit/skool2ctl.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    19437 2022-08-08 18:01:45.000000 skoolkit-8.8/skoolkit/skool2html.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    26018 2022-08-12 20:16:11.000000 skoolkit-8.8/skoolkit/skoolasm.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    29529 2022-09-19 23:23:13.000000 skoolkit-8.8/skoolkit/skoolctl.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    60015 2022-10-06 14:56:03.000000 skoolkit-8.8/skoolkit/skoolhtml.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    57111 2022-11-13 17:12:46.000000 skoolkit-8.8/skoolkit/skoolmacro.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    67118 2022-10-15 23:38:53.000000 skoolkit-8.8/skoolkit/skoolparser.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)     4599 2021-02-16 20:57:03.000000 skoolkit-8.8/skoolkit/sna2ctl.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)     8343 2021-02-03 21:14:45.000000 skoolkit-8.8/skoolkit/sna2img.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)     5666 2022-09-07 19:43:47.000000 skoolkit-8.8/skoolkit/sna2skool.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    16472 2021-02-16 21:11:08.000000 skoolkit-8.8/skoolkit/snactl.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    23210 2022-11-11 19:34:36.000000 skoolkit-8.8/skoolkit/snapinfo.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)     4418 2017-10-23 21:09:54.000000 skoolkit-8.8/skoolkit/snapmod.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    12816 2022-10-01 13:59:00.000000 skoolkit-8.8/skoolkit/snapshot.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    26812 2022-08-16 20:32:40.000000 skoolkit-8.8/skoolkit/snaskool.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    27268 2022-11-13 19:34:24.000000 skoolkit-8.8/skoolkit/tap2sna.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    18155 2022-09-27 21:18:14.000000 skoolkit-8.8/skoolkit/tapinfo.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)     2137 2018-01-26 22:16:31.000000 skoolkit-8.8/skoolkit/textutils.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    12696 2022-11-17 21:14:11.000000 skoolkit-8.8/skoolkit/trace.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)   119491 2022-11-12 19:07:02.000000 skoolkit-8.8/skoolkit/traceutils.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    39626 2022-10-02 10:34:22.000000 skoolkit-8.8/skoolkit/z80.py
-drwxr-xr-x   0 rjd       (1000) rjd       (1000)        0 2022-11-19 13:34:18.080618 skoolkit-8.8/skoolkit.egg-info/
--rw-r--r--   0 rjd       (1000) rjd       (1000)     6711 2022-11-19 13:34:18.000000 skoolkit-8.8/skoolkit.egg-info/PKG-INFO
--rw-r--r--   0 rjd       (1000) rjd       (1000)     5228 2022-11-19 13:34:18.000000 skoolkit-8.8/skoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)        1 2022-11-19 13:34:18.000000 skoolkit-8.8/skoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 rjd       (1000) rjd       (1000)        9 2022-11-19 13:34:18.000000 skoolkit-8.8/skoolkit.egg-info/top_level.txt
--rwxr-xr-x   0 rjd       (1000) rjd       (1000)      881 2018-09-16 12:11:45.000000 skoolkit-8.8/sna2ctl.py
--rwxr-xr-x   0 rjd       (1000) rjd       (1000)      886 2017-01-12 22:31:18.000000 skoolkit-8.8/sna2img.py
--rwxr-xr-x   0 rjd       (1000) rjd       (1000)      896 2017-01-12 22:31:18.000000 skoolkit-8.8/sna2skool.py
--rwxr-xr-x   0 rjd       (1000) rjd       (1000)      888 2017-01-12 22:31:18.000000 skoolkit-8.8/snapinfo.py
--rwxr-xr-x   0 rjd       (1000) rjd       (1000)      886 2017-01-12 22:31:18.000000 skoolkit-8.8/snapmod.py
--rwxr-xr-x   0 rjd       (1000) rjd       (1000)      887 2017-01-12 22:31:18.000000 skoolkit-8.8/tap2sna.py
--rwxr-xr-x   0 rjd       (1000) rjd       (1000)      887 2017-01-12 22:31:18.000000 skoolkit-8.8/tapinfo.py
-drwxr-xr-x   0 rjd       (1000) rjd       (1000)        0 2022-11-19 13:34:18.088618 skoolkit-8.8/tests/
--rw-r--r--   0 rjd       (1000) rjd       (1000)   113727 2022-09-19 19:37:19.000000 skoolkit-8.8/tests/macrotest.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    15554 2022-11-09 20:51:42.000000 skoolkit-8.8/tests/skoolkittest.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)     6174 2022-10-25 12:02:01.000000 skoolkit-8.8/tests/test_audio.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    28394 2020-09-03 20:18:52.000000 skoolkit-8.8/tests/test_basic.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    16280 2020-02-27 22:03:54.000000 skoolkit-8.8/tests/test_bin2sna.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    22895 2020-09-15 20:03:51.000000 skoolkit-8.8/tests/test_bin2tap.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    83740 2022-09-19 23:25:52.000000 skoolkit-8.8/tests/test_ctlparser.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    90233 2021-04-13 20:39:36.000000 skoolkit-8.8/tests/test_disassembler.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)     8472 2018-03-25 11:29:25.000000 skoolkit-8.8/tests/test_graphics.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    50384 2021-04-25 13:12:55.000000 skoolkit-8.8/tests/test_image.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)     9703 2019-04-03 21:13:21.000000 skoolkit-8.8/tests/test_refparser.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)   105509 2022-11-17 21:10:57.000000 skoolkit-8.8/tests/test_simulator.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    34438 2021-05-18 21:36:14.000000 skoolkit-8.8/tests/test_skool2asm.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    55820 2020-03-10 20:51:11.000000 skoolkit-8.8/tests/test_skool2bin.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)     9183 2019-03-04 21:42:17.000000 skoolkit-8.8/tests/test_skool2ctl.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    76179 2022-08-08 18:01:45.000000 skoolkit-8.8/tests/test_skool2html.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)   137186 2022-08-12 20:16:11.000000 skoolkit-8.8/tests/test_skoolasm.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    76967 2022-09-19 23:22:58.000000 skoolkit-8.8/tests/test_skoolctl.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)   445324 2022-10-25 12:02:01.000000 skoolkit-8.8/tests/test_skoolhtml.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)     2440 2019-10-13 13:50:42.000000 skoolkit-8.8/tests/test_skoolkit.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    22924 2020-10-02 20:06:53.000000 skoolkit-8.8/tests/test_skoolmacro.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)   188769 2022-09-19 23:18:22.000000 skoolkit-8.8/tests/test_skoolparser.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    36727 2021-05-18 21:36:14.000000 skoolkit-8.8/tests/test_sna2ctl.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    33413 2022-08-16 20:15:51.000000 skoolkit-8.8/tests/test_sna2img.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    32348 2022-09-07 19:43:47.000000 skoolkit-8.8/tests/test_sna2skool.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    80378 2021-05-18 21:36:14.000000 skoolkit-8.8/tests/test_snapinfo.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    18092 2020-02-13 22:02:35.000000 skoolkit-8.8/tests/test_snapmod.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    10218 2019-08-30 19:43:27.000000 skoolkit-8.8/tests/test_snapshot.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)   160476 2022-09-19 23:24:39.000000 skoolkit-8.8/tests/test_snaskool.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    68869 2022-11-13 19:35:36.000000 skoolkit-8.8/tests/test_tap2sna.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    25529 2022-09-21 20:15:52.000000 skoolkit-8.8/tests/test_tapinfo.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)     3109 2018-01-26 22:16:31.000000 skoolkit-8.8/tests/test_textutils.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    28845 2022-11-17 21:14:11.000000 skoolkit-8.8/tests/test_trace.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)   171930 2022-11-12 19:05:58.000000 skoolkit-8.8/tests/test_traceutils.py
--rw-r--r--   0 rjd       (1000) rjd       (1000)    77008 2022-09-10 10:42:39.000000 skoolkit-8.8/tests/test_z80.py
--rwxr-xr-x   0 rjd       (1000) rjd       (1000)      877 2022-10-30 12:43:11.000000 skoolkit-8.8/trace.py
+drwxr-xr-x   0 rjd       (1000) rjd       (1000)        0 2023-02-19 13:05:11.560390 skoolkit-8.9/
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    35147 2010-03-03 00:59:14.000000 skoolkit-8.9/COPYING
+-rw-r--r--   0 rjd       (1000) rjd       (1000)       64 2014-12-31 18:28:35.000000 skoolkit-8.9/MANIFEST.in
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     6711 2023-02-19 13:05:11.560390 skoolkit-8.9/PKG-INFO
+-rwxr-xr-x   0 rjd       (1000) rjd       (1000)      886 2017-01-12 22:31:18.000000 skoolkit-8.9/bin2sna.py
+-rwxr-xr-x   0 rjd       (1000) rjd       (1000)      892 2017-01-12 22:31:18.000000 skoolkit-8.9/bin2tap.py
+drwxr-xr-x   0 rjd       (1000) rjd       (1000)        0 2023-02-19 13:05:11.540391 skoolkit-8.9/docs/
+drwxr-xr-x   0 rjd       (1000) rjd       (1000)        0 2023-02-19 13:05:11.544391 skoolkit-8.9/docs/_sources/
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     4165 2022-08-12 20:16:11.000000 skoolkit-8.9/docs/_sources/asm-templates.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    51542 2022-09-19 23:34:08.000000 skoolkit-8.9/docs/_sources/asm.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     2862 2019-05-14 21:07:25.000000 skoolkit-8.9/docs/_sources/assemblers.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    18150 2023-02-19 12:52:16.000000 skoolkit-8.9/docs/_sources/changelog.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     3491 2015-11-20 12:50:08.000000 skoolkit-8.9/docs/_sources/changelog1.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    11437 2019-07-08 20:36:08.000000 skoolkit-8.9/docs/_sources/changelog2.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    11778 2019-07-08 20:36:08.000000 skoolkit-8.9/docs/_sources/changelog3.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     7233 2020-10-07 20:20:25.000000 skoolkit-8.9/docs/_sources/changelog4.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     6124 2020-10-07 20:20:25.000000 skoolkit-8.9/docs/_sources/changelog5.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     9323 2020-10-07 20:20:25.000000 skoolkit-8.9/docs/_sources/changelog6.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     6307 2020-10-07 20:20:25.000000 skoolkit-8.9/docs/_sources/changelog7.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    83385 2023-02-16 21:07:47.000000 skoolkit-8.9/docs/_sources/commands.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    13441 2021-05-18 21:36:14.000000 skoolkit-8.9/docs/_sources/components.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    32224 2022-08-17 20:15:36.000000 skoolkit-8.9/docs/_sources/control-files.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    13398 2022-08-18 23:11:24.000000 skoolkit-8.9/docs/_sources/diy.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    16637 2021-06-23 20:02:28.000000 skoolkit-8.9/docs/_sources/extending.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    27424 2022-08-29 20:54:25.000000 skoolkit-8.9/docs/_sources/html-templates.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)      426 2019-08-09 20:57:13.000000 skoolkit-8.9/docs/_sources/index.rst.txt
+drwxr-xr-x   0 rjd       (1000) rjd       (1000)        0 2023-02-19 13:05:11.544391 skoolkit-8.9/docs/_sources/man/
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     3171 2023-01-24 20:32:20.000000 skoolkit-8.9/docs/_sources/man/bin2sna.py.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     2923 2020-09-15 20:03:51.000000 skoolkit-8.9/docs/_sources/man/bin2tap.py.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     7680 2021-05-18 21:36:14.000000 skoolkit-8.9/docs/_sources/man/skool2asm.py.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     1558 2020-02-25 22:04:07.000000 skoolkit-8.9/docs/_sources/man/skool2bin.py.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     3065 2021-05-18 21:36:14.000000 skoolkit-8.9/docs/_sources/man/skool2ctl.py.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     7266 2022-08-08 18:01:45.000000 skoolkit-8.9/docs/_sources/man/skool2html.py.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     3388 2021-05-18 21:36:14.000000 skoolkit-8.9/docs/_sources/man/sna2ctl.py.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     2297 2019-07-08 21:10:05.000000 skoolkit-8.9/docs/_sources/man/sna2img.py.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     6538 2022-09-07 19:43:47.000000 skoolkit-8.9/docs/_sources/man/sna2skool.py.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     4353 2021-05-18 21:36:14.000000 skoolkit-8.9/docs/_sources/man/snapinfo.py.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     2464 2023-01-24 20:32:20.000000 skoolkit-8.9/docs/_sources/man/snapmod.py.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    12572 2023-02-16 21:07:47.000000 skoolkit-8.9/docs/_sources/man/tap2sna.py.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)      916 2020-09-17 20:17:10.000000 skoolkit-8.9/docs/_sources/man/tapinfo.py.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     3543 2023-01-20 19:34:18.000000 skoolkit-8.9/docs/_sources/man/trace.py.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     5297 2019-11-05 22:00:31.000000 skoolkit-8.9/docs/_sources/migration.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     3327 2022-09-19 23:27:01.000000 skoolkit-8.9/docs/_sources/parsing.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    51648 2022-10-25 12:02:01.000000 skoolkit-8.9/docs/_sources/ref-files.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    11571 2020-03-08 12:27:23.000000 skoolkit-8.9/docs/_sources/skool-files.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)   115169 2022-10-05 18:39:07.000000 skoolkit-8.9/docs/_sources/skool-macros.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     2544 2022-07-26 20:00:49.000000 skoolkit-8.9/docs/_sources/usage.rst.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     4993 2022-11-13 15:52:53.000000 skoolkit-8.9/docs/_sources/whatis.rst.txt
+drwxr-xr-x   0 rjd       (1000) rjd       (1000)        0 2023-02-19 13:05:11.548390 skoolkit-8.9/docs/_static/
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    13646 2023-02-19 12:55:40.000000 skoolkit-8.9/docs/_static/basic.css
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     4256 2023-02-19 12:55:40.000000 skoolkit-8.9/docs/_static/classic.css
+-rw-r--r--   0 rjd       (1000) rjd       (1000)      368 2021-09-12 11:18:57.000000 skoolkit-8.9/docs/_static/custom.css
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     9416 2021-01-02 17:13:01.000000 skoolkit-8.9/docs/_static/doctools.js
+-rw-r--r--   0 rjd       (1000) rjd       (1000)      353 2023-02-19 12:55:40.000000 skoolkit-8.9/docs/_static/documentation_options.js
+-rw-r--r--   0 rjd       (1000) rjd       (1000)      286 2021-01-01 06:53:29.000000 skoolkit-8.9/docs/_static/file.png
+-rw-r--r--   0 rjd       (1000) rjd       (1000)   287600 2021-01-12 20:55:26.000000 skoolkit-8.9/docs/_static/jquery.js
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    10847 2023-02-19 12:55:40.000000 skoolkit-8.9/docs/_static/language_data.js
+-rw-r--r--   0 rjd       (1000) rjd       (1000)       90 2021-01-01 06:53:29.000000 skoolkit-8.9/docs/_static/minus.png
+-rw-r--r--   0 rjd       (1000) rjd       (1000)       90 2021-01-01 06:53:29.000000 skoolkit-8.9/docs/_static/plus.png
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     4780 2023-02-19 12:55:40.000000 skoolkit-8.9/docs/_static/pygments.css
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    16323 2021-01-04 13:20:58.000000 skoolkit-8.9/docs/_static/searchtools.js
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     4803 2023-02-19 12:55:40.000000 skoolkit-8.9/docs/_static/sidebar.js
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    58881 2021-03-31 12:21:21.000000 skoolkit-8.9/docs/_static/underscore.js
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    15265 2023-02-19 12:55:38.000000 skoolkit-8.9/docs/asm-templates.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)   109092 2023-02-19 12:55:38.000000 skoolkit-8.9/docs/asm.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    10762 2023-02-19 12:55:38.000000 skoolkit-8.9/docs/assemblers.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    50374 2023-02-19 12:55:38.000000 skoolkit-8.9/docs/changelog.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    13248 2023-02-19 12:55:38.000000 skoolkit-8.9/docs/changelog1.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    31682 2023-02-19 12:55:39.000000 skoolkit-8.9/docs/changelog2.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    31918 2023-02-19 12:55:39.000000 skoolkit-8.9/docs/changelog3.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    21605 2023-02-19 12:55:39.000000 skoolkit-8.9/docs/changelog4.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    19904 2023-02-19 12:55:39.000000 skoolkit-8.9/docs/changelog5.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    28657 2023-02-19 12:55:39.000000 skoolkit-8.9/docs/changelog6.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    19653 2023-02-19 12:55:39.000000 skoolkit-8.9/docs/changelog7.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)   128401 2023-02-19 12:55:39.000000 skoolkit-8.9/docs/commands.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    64292 2023-02-19 12:55:39.000000 skoolkit-8.9/docs/components.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    69665 2023-02-19 12:55:39.000000 skoolkit-8.9/docs/control-files.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    24938 2023-02-19 12:55:39.000000 skoolkit-8.9/docs/diy.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    81048 2023-02-19 12:55:39.000000 skoolkit-8.9/docs/extending.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    15999 2023-02-19 12:55:40.000000 skoolkit-8.9/docs/genindex.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    66063 2023-02-19 12:55:39.000000 skoolkit-8.9/docs/html-templates.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     6380 2023-02-19 12:55:39.000000 skoolkit-8.9/docs/index.html
+drwxr-xr-x   0 rjd       (1000) rjd       (1000)        0 2023-02-19 13:05:11.548390 skoolkit-8.9/docs/man/
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    13706 2023-02-19 12:55:39.000000 skoolkit-8.9/docs/man/bin2sna.py.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     9380 2023-02-19 12:55:39.000000 skoolkit-8.9/docs/man/bin2tap.py.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    23234 2023-02-19 12:55:39.000000 skoolkit-8.9/docs/man/skool2asm.py.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     8185 2023-02-19 12:55:39.000000 skoolkit-8.9/docs/man/skool2bin.py.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    11957 2023-02-19 12:55:39.000000 skoolkit-8.9/docs/man/skool2ctl.py.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    22789 2023-02-19 12:55:39.000000 skoolkit-8.9/docs/man/skool2html.py.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    11483 2023-02-19 12:55:39.000000 skoolkit-8.9/docs/man/sna2ctl.py.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     9015 2023-02-19 12:55:39.000000 skoolkit-8.9/docs/man/sna2img.py.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    20548 2023-02-19 12:55:39.000000 skoolkit-8.9/docs/man/sna2skool.py.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    13276 2023-02-19 12:55:39.000000 skoolkit-8.9/docs/man/snapinfo.py.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    12679 2023-02-19 12:55:39.000000 skoolkit-8.9/docs/man/snapmod.py.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    36610 2023-02-19 12:55:39.000000 skoolkit-8.9/docs/man/tap2sna.py.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     6471 2023-02-19 12:55:39.000000 skoolkit-8.9/docs/man/tapinfo.py.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    13565 2023-02-19 12:55:39.000000 skoolkit-8.9/docs/man/trace.py.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    19592 2023-02-19 12:55:39.000000 skoolkit-8.9/docs/migration.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    12321 2023-02-19 12:55:39.000000 skoolkit-8.9/docs/parsing.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     4402 2023-02-19 12:55:40.000000 skoolkit-8.9/docs/py-modindex.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)   104051 2023-02-19 12:55:40.000000 skoolkit-8.9/docs/ref-files.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     3363 2023-02-19 12:55:40.000000 skoolkit-8.9/docs/search.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    54344 2023-02-19 12:55:40.000000 skoolkit-8.9/docs/searchindex.js
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    25190 2023-02-19 12:55:40.000000 skoolkit-8.9/docs/skool-files.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)   230928 2023-02-19 12:55:40.000000 skoolkit-8.9/docs/skool-macros.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     9038 2023-02-19 12:55:40.000000 skoolkit-8.9/docs/usage.html
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    12910 2023-02-19 12:55:40.000000 skoolkit-8.9/docs/whatis.html
+drwxr-xr-x   0 rjd       (1000) rjd       (1000)        0 2023-02-19 13:05:11.548390 skoolkit-8.9/examples/
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     2454 2015-12-04 12:16:10.000000 skoolkit-8.9/examples/hungry_horace.ctl
+-rw-r--r--   0 rjd       (1000) rjd       (1000)      696 2016-01-09 11:54:00.000000 skoolkit-8.9/examples/hungry_horace.ref
+-rw-r--r--   0 rjd       (1000) rjd       (1000)      214 2022-10-01 14:05:49.000000 skoolkit-8.9/examples/hungry_horace.t2s
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     5789 2022-11-13 15:52:53.000000 skoolkit-8.9/long_description.rst
+drwxr-xr-x   0 rjd       (1000) rjd       (1000)        0 2023-02-19 13:05:11.536391 skoolkit-8.9/man/
+drwxr-xr-x   0 rjd       (1000) rjd       (1000)        0 2023-02-19 13:05:11.552390 skoolkit-8.9/man/man1/
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     4567 2023-02-19 12:55:34.000000 skoolkit-8.9/man/man1/bin2sna.py.1
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     4085 2023-02-19 12:55:34.000000 skoolkit-8.9/man/man1/bin2tap.py.1
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     9606 2023-02-19 12:55:34.000000 skoolkit-8.9/man/man1/skool2asm.py.1
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     2827 2023-02-19 12:55:34.000000 skoolkit-8.9/man/man1/skool2bin.py.1
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     4460 2023-02-19 12:55:34.000000 skoolkit-8.9/man/man1/skool2ctl.py.1
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     9467 2023-02-19 12:55:34.000000 skoolkit-8.9/man/man1/skool2html.py.1
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     4795 2023-02-19 12:55:34.000000 skoolkit-8.9/man/man1/sna2ctl.py.1
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     3683 2023-02-19 12:55:34.000000 skoolkit-8.9/man/man1/sna2img.py.1
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     8140 2023-02-19 12:55:34.000000 skoolkit-8.9/man/man1/sna2skool.py.1
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     5960 2023-02-19 12:55:34.000000 skoolkit-8.9/man/man1/snapinfo.py.1
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     3798 2023-02-19 12:55:34.000000 skoolkit-8.9/man/man1/snapmod.py.1
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    14742 2023-02-19 12:55:34.000000 skoolkit-8.9/man/man1/tap2sna.py.1
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     1971 2023-02-19 12:55:34.000000 skoolkit-8.9/man/man1/tapinfo.py.1
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     5080 2023-02-19 12:55:34.000000 skoolkit-8.9/man/man1/trace.py.1
+-rw-r--r--   0 rjd       (1000) rjd       (1000)       90 2021-11-16 20:02:53.000000 skoolkit-8.9/pyproject.toml
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     1153 2023-02-19 13:05:11.560390 skoolkit-8.9/setup.cfg
+-rwxr-xr-x   0 rjd       (1000) rjd       (1000)      896 2017-01-12 22:31:18.000000 skoolkit-8.9/skool2asm.py
+-rwxr-xr-x   0 rjd       (1000) rjd       (1000)      891 2017-01-12 22:31:18.000000 skoolkit-8.9/skool2bin.py
+-rwxr-xr-x   0 rjd       (1000) rjd       (1000)      896 2017-01-12 22:31:18.000000 skoolkit-8.9/skool2ctl.py
+-rwxr-xr-x   0 rjd       (1000) rjd       (1000)      898 2017-01-12 22:31:18.000000 skoolkit-8.9/skool2html.py
+drwxr-xr-x   0 rjd       (1000) rjd       (1000)        0 2023-02-19 13:05:11.556390 skoolkit-8.9/skoolkit/
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     6271 2023-02-19 12:54:42.000000 skoolkit-8.9/skoolkit/__init__.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     5765 2022-11-13 15:54:44.000000 skoolkit-8.9/skoolkit/audio.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    10745 2020-09-03 20:18:52.000000 skoolkit-8.9/skoolkit/basic.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     4682 2020-02-27 22:10:07.000000 skoolkit-8.9/skoolkit/bin2sna.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     8940 2020-09-15 20:03:51.000000 skoolkit-8.9/skoolkit/bin2tap.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     1783 2021-02-03 21:14:45.000000 skoolkit-8.9/skoolkit/components.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     6360 2022-08-08 20:12:19.000000 skoolkit-8.9/skoolkit/config.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    18478 2022-09-18 12:36:07.000000 skoolkit-8.9/skoolkit/ctlparser.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    16008 2022-10-25 12:02:01.000000 skoolkit-8.9/skoolkit/defaults.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    37276 2021-04-13 20:39:36.000000 skoolkit-8.9/skoolkit/disassembler.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    16581 2021-07-23 19:51:54.000000 skoolkit-8.9/skoolkit/graphics.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    11792 2021-04-25 13:05:19.000000 skoolkit-8.9/skoolkit/image.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     9633 2023-02-16 21:07:47.000000 skoolkit-8.9/skoolkit/loadsample.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    17708 2023-02-13 21:12:35.000000 skoolkit-8.9/skoolkit/loadtracer.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    36547 2019-01-03 21:48:08.000000 skoolkit-8.9/skoolkit/opcodes.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    21763 2021-02-10 21:01:21.000000 skoolkit-8.9/skoolkit/pngwriter.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     7744 2021-07-22 20:05:54.000000 skoolkit-8.9/skoolkit/refparser.py
+drwxr-xr-x   0 rjd       (1000) rjd       (1000)        0 2023-02-19 13:05:11.556390 skoolkit-8.9/skoolkit/resources/
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    16384 2019-02-10 22:35:13.000000 skoolkit-8.9/skoolkit/resources/48.rom
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     1164 2019-07-14 11:45:10.000000 skoolkit-8.9/skoolkit/resources/skoolkit-dark.css
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     1164 2019-07-14 11:45:10.000000 skoolkit-8.9/skoolkit/resources/skoolkit-green.css
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     1164 2019-07-14 11:45:10.000000 skoolkit-8.9/skoolkit/resources/skoolkit-plum.css
+-rw-r--r--   0 rjd       (1000) rjd       (1000)       80 2017-02-15 21:53:32.000000 skoolkit-8.9/skoolkit/resources/skoolkit-wide.css
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     3578 2021-01-28 21:19:34.000000 skoolkit-8.9/skoolkit/resources/skoolkit.css
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     7710 2022-11-13 15:44:09.000000 skoolkit-8.9/skoolkit/simtables.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)   189484 2023-02-04 12:48:26.000000 skoolkit-8.9/skoolkit/simulator.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     7940 2021-09-19 12:27:42.000000 skoolkit-8.9/skoolkit/skool2asm.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    14224 2021-05-18 21:36:14.000000 skoolkit-8.9/skoolkit/skool2bin.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     4790 2019-03-04 21:42:17.000000 skoolkit-8.9/skoolkit/skool2ctl.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    19437 2022-08-08 18:01:45.000000 skoolkit-8.9/skoolkit/skool2html.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    26018 2022-08-12 20:16:11.000000 skoolkit-8.9/skoolkit/skoolasm.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    29529 2022-09-19 23:23:13.000000 skoolkit-8.9/skoolkit/skoolctl.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    60015 2022-10-06 14:56:03.000000 skoolkit-8.9/skoolkit/skoolhtml.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    57111 2022-11-13 17:12:46.000000 skoolkit-8.9/skoolkit/skoolmacro.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    67118 2022-10-15 23:38:53.000000 skoolkit-8.9/skoolkit/skoolparser.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     4599 2021-02-16 20:57:03.000000 skoolkit-8.9/skoolkit/sna2ctl.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     8343 2021-02-03 21:14:45.000000 skoolkit-8.9/skoolkit/sna2img.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     5666 2022-09-07 19:43:47.000000 skoolkit-8.9/skoolkit/sna2skool.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    16472 2021-02-16 21:11:08.000000 skoolkit-8.9/skoolkit/snactl.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    23554 2023-01-24 20:32:20.000000 skoolkit-8.9/skoolkit/snapinfo.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     4418 2017-10-23 21:09:54.000000 skoolkit-8.9/skoolkit/snapmod.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    13208 2023-01-24 20:32:20.000000 skoolkit-8.9/skoolkit/snapshot.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    26812 2022-08-16 20:32:40.000000 skoolkit-8.9/skoolkit/snaskool.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    35069 2023-02-11 18:15:52.000000 skoolkit-8.9/skoolkit/tap2sna.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    18942 2022-12-09 20:58:51.000000 skoolkit-8.9/skoolkit/tapinfo.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     2137 2018-01-26 22:16:31.000000 skoolkit-8.9/skoolkit/textutils.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    13383 2023-01-27 20:25:21.000000 skoolkit-8.9/skoolkit/trace.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)   119491 2022-11-12 19:07:02.000000 skoolkit-8.9/skoolkit/traceutils.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    39626 2022-10-02 10:34:22.000000 skoolkit-8.9/skoolkit/z80.py
+drwxr-xr-x   0 rjd       (1000) rjd       (1000)        0 2023-02-19 13:05:11.556390 skoolkit-8.9/skoolkit.egg-info/
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     6711 2023-02-19 13:05:11.000000 skoolkit-8.9/skoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     5272 2023-02-19 13:05:11.000000 skoolkit-8.9/skoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)        1 2023-02-19 13:05:11.000000 skoolkit-8.9/skoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 rjd       (1000) rjd       (1000)        9 2023-02-19 13:05:11.000000 skoolkit-8.9/skoolkit.egg-info/top_level.txt
+-rwxr-xr-x   0 rjd       (1000) rjd       (1000)      881 2018-09-16 12:11:45.000000 skoolkit-8.9/sna2ctl.py
+-rwxr-xr-x   0 rjd       (1000) rjd       (1000)      886 2017-01-12 22:31:18.000000 skoolkit-8.9/sna2img.py
+-rwxr-xr-x   0 rjd       (1000) rjd       (1000)      896 2017-01-12 22:31:18.000000 skoolkit-8.9/sna2skool.py
+-rwxr-xr-x   0 rjd       (1000) rjd       (1000)      888 2017-01-12 22:31:18.000000 skoolkit-8.9/snapinfo.py
+-rwxr-xr-x   0 rjd       (1000) rjd       (1000)      886 2017-01-12 22:31:18.000000 skoolkit-8.9/snapmod.py
+-rwxr-xr-x   0 rjd       (1000) rjd       (1000)      887 2017-01-12 22:31:18.000000 skoolkit-8.9/tap2sna.py
+-rwxr-xr-x   0 rjd       (1000) rjd       (1000)      887 2017-01-12 22:31:18.000000 skoolkit-8.9/tapinfo.py
+drwxr-xr-x   0 rjd       (1000) rjd       (1000)        0 2023-02-19 13:05:11.560390 skoolkit-8.9/tests/
+-rw-r--r--   0 rjd       (1000) rjd       (1000)   113727 2023-02-04 13:07:40.000000 skoolkit-8.9/tests/macrotest.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    15964 2023-01-24 20:32:20.000000 skoolkit-8.9/tests/skoolkittest.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     6174 2022-10-25 12:02:01.000000 skoolkit-8.9/tests/test_audio.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    28394 2020-09-03 20:18:52.000000 skoolkit-8.9/tests/test_basic.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    16545 2023-01-24 20:42:25.000000 skoolkit-8.9/tests/test_bin2sna.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    22895 2020-09-15 20:03:51.000000 skoolkit-8.9/tests/test_bin2tap.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    83740 2022-09-19 23:25:52.000000 skoolkit-8.9/tests/test_ctlparser.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    90233 2021-04-13 20:39:36.000000 skoolkit-8.9/tests/test_disassembler.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     8472 2018-03-25 11:29:25.000000 skoolkit-8.9/tests/test_graphics.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    50384 2021-04-25 13:12:55.000000 skoolkit-8.9/tests/test_image.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     9703 2019-04-03 21:13:21.000000 skoolkit-8.9/tests/test_refparser.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)   111652 2023-02-04 13:20:03.000000 skoolkit-8.9/tests/test_simulator.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    34438 2021-05-18 21:36:14.000000 skoolkit-8.9/tests/test_skool2asm.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    55820 2020-03-10 20:51:11.000000 skoolkit-8.9/tests/test_skool2bin.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     9183 2019-03-04 21:42:17.000000 skoolkit-8.9/tests/test_skool2ctl.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    76179 2022-08-08 18:01:45.000000 skoolkit-8.9/tests/test_skool2html.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)   137186 2022-08-12 20:16:11.000000 skoolkit-8.9/tests/test_skoolasm.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    76967 2022-09-19 23:22:58.000000 skoolkit-8.9/tests/test_skoolctl.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)   445324 2022-10-25 12:02:01.000000 skoolkit-8.9/tests/test_skoolhtml.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     2440 2019-10-13 13:50:42.000000 skoolkit-8.9/tests/test_skoolkit.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    22924 2020-10-02 20:06:53.000000 skoolkit-8.9/tests/test_skoolmacro.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)   188769 2022-09-19 23:18:22.000000 skoolkit-8.9/tests/test_skoolparser.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    36727 2021-05-18 21:36:14.000000 skoolkit-8.9/tests/test_sna2ctl.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    33413 2022-08-16 20:15:51.000000 skoolkit-8.9/tests/test_sna2img.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    32348 2022-09-07 19:43:47.000000 skoolkit-8.9/tests/test_sna2skool.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    81349 2022-11-29 21:07:34.000000 skoolkit-8.9/tests/test_snapinfo.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    18237 2023-01-24 20:44:52.000000 skoolkit-8.9/tests/test_snapmod.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    11792 2023-01-24 20:32:20.000000 skoolkit-8.9/tests/test_snapshot.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)   160476 2022-09-19 23:24:39.000000 skoolkit-8.9/tests/test_snaskool.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    84435 2023-02-13 21:12:35.000000 skoolkit-8.9/tests/test_tap2sna.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    27669 2022-12-09 20:58:51.000000 skoolkit-8.9/tests/test_tapinfo.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)     3109 2018-01-26 22:16:31.000000 skoolkit-8.9/tests/test_textutils.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    44804 2023-02-04 13:04:31.000000 skoolkit-8.9/tests/test_trace.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)   171930 2022-11-12 19:05:58.000000 skoolkit-8.9/tests/test_traceutils.py
+-rw-r--r--   0 rjd       (1000) rjd       (1000)    77008 2022-09-10 10:42:39.000000 skoolkit-8.9/tests/test_z80.py
+-rwxr-xr-x   0 rjd       (1000) rjd       (1000)      877 2022-10-30 12:43:11.000000 skoolkit-8.9/trace.py
```

### Comparing `skoolkit-8.8/COPYING` & `skoolkit-8.9/COPYING`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/PKG-INFO` & `skoolkit-8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skoolkit
-Version: 8.8
+Version: 8.9
 Summary: A suite of tools for creating disassemblies of ZX Spectrum games
 Home-page: https://skoolkit.ca
 Author: Richard Dymond
 Author-email: rjdymond@gmail.com
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `skoolkit-8.8/bin2sna.py` & `skoolkit-8.9/bin2sna.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/bin2tap.py` & `skoolkit-8.9/bin2tap.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_sources/asm-templates.rst.txt` & `skoolkit-8.9/docs/_sources/asm-templates.rst.txt`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_sources/asm.rst.txt` & `skoolkit-8.9/docs/_sources/asm.rst.txt`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_sources/assemblers.rst.txt` & `skoolkit-8.9/docs/_sources/assemblers.rst.txt`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_sources/changelog.rst.txt` & `skoolkit-8.9/docs/_sources/changelog.rst.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,51 @@
 Changelog
 =========
 
+8.9 (2023-02-19)
+----------------
+* Added support to :ref:`tap2sna.py` for TZX loops (block types 0x24 and 0x25),
+  pauses (block types 0x10, 0x11, 0x14 and 0x20), and unused bits in data
+  blocks (block types 0x11 and 0x14)
+* :ref:`tap2sna.py` now accelerates the simulation of tape-sampling loops in
+  loading routines, and also simulates the execution of interrupt routines when
+  interrupts are enabled
+* Added the ``--sim-load-config`` option to :ref:`tap2sna.py` (to set the value
+  of a ``--sim-load`` configuration parameter: ``accelerator``, ``fast-load``,
+  ``first-edge``, ``pause``, ``timeout``, ``trace``)
+* Added the ``--tape-name`` option to :ref:`tap2sna.py` (to specify the name of
+  a TAP/TZX file in a zip archive, in case there is more than one)
+* Added the ``--tape-start`` and ``--tape-stop`` options to :ref:`tap2sna.py`
+  (to start or stop the tape at a specific block number)
+* Added the ``--tape-sum`` option to :ref:`tap2sna.py` (to specify the MD5
+  checksum of the TAP/TZX file)
+* Added support to :ref:`tap2sna.py` for quoted arguments in an arguments file
+* Added the ``--interrupts`` option to :ref:`trace.py` (to enable the execution
+  of interrupt routines)
+* :ref:`trace.py` now reads and writes the T-states counter in Z80 snapshots
+  and reads the T-states counter in SZX snapshots
+* Added support to :ref:`bin2sna.py`, :ref:`snapmod.py` and :ref:`tap2sna.py`
+  for setting the ``tstates`` hardware attribute (i.e. the T-states counter in
+  Z80 snapshots)
+* :ref:`tapinfo.py` now shows full info for TZX block types 0x10 (standard
+  speed data) and 0x11 (turbo speed data)
+* Fixed how the Z80 instruction set simulator updates the A and R registers in
+  the 'LD A,R' and 'LD R,A' instructions
+* Fixed how the Z80 instruction set simulator handles a CALL instruction that
+  overwrites its own address operand
+* Fixed how a Z80 snapshot memory block that ends with a single 0xED byte is
+  decompressed
+* Fixed how the ``--sim-load`` option of :ref:`tap2sna.py` transitions from a
+  tape block that ends with data to the next block when there is no pause
+  between them
+* Fixed the bug that prevents the ``--find`` option of :ref:`snapinfo.py` from
+  finding byte sequences below address 16384
+* Fixed the bug that prevents the ``--find-text`` option of :ref:`snapinfo.py`
+  from finding text strings below address 16384
+
 8.8 (2022-11-19)
 ----------------
 * Added the :ref:`trace.py` command (for tracing the execution of machine code
   in a 48K memory snapshot)
 * The ``--sim-load`` option of :ref:`tap2sna.py` now performs any ``call``,
   ``move``, ``poke`` and ``sysvars`` operations specified by the ``--ram``
   option
```

### Comparing `skoolkit-8.8/docs/_sources/changelog1.rst.txt` & `skoolkit-8.9/docs/_sources/changelog1.rst.txt`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_sources/changelog2.rst.txt` & `skoolkit-8.9/docs/_sources/changelog2.rst.txt`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_sources/changelog3.rst.txt` & `skoolkit-8.9/docs/_sources/changelog3.rst.txt`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_sources/changelog4.rst.txt` & `skoolkit-8.9/docs/_sources/changelog4.rst.txt`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_sources/changelog5.rst.txt` & `skoolkit-8.9/docs/_sources/changelog5.rst.txt`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_sources/changelog6.rst.txt` & `skoolkit-8.9/docs/_sources/changelog6.rst.txt`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_sources/changelog7.rst.txt` & `skoolkit-8.9/docs/_sources/changelog7.rst.txt`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_sources/commands.rst.txt` & `skoolkit-8.9/docs/_sources/commands.rst.txt`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,16 @@
                           more information. This option may be used multiple
                           times.
     -V, --version         Show SkoolKit version number and exit.
 
 +---------+-------------------------------------------------------------------+
 | Version | Changes                                                           |
 +=========+===================================================================+
+| 8.9     | Added the ``tstates`` hardware state attribute                    |
++---------+-------------------------------------------------------------------+
 | 6.3     | Added the ``--poke`` option                                       |
 +---------+-------------------------------------------------------------------+
 | 6.2     | Added the ``--reg`` and ``--state`` options; the ``--org``,       |
 |         | ``--stack`` and ``--start`` options accept a hexadecimal integer  |
 |         | prefixed by '0x'                                                  |
 +---------+-------------------------------------------------------------------+
 | 5.2     | New                                                               |
@@ -1240,14 +1242,16 @@
                           more information. This option may be used multiple
                           times.
     -V, --version         Show SkoolKit version number and exit.
 
 +---------+-------------------------------------------------------------------+
 | Version | Changes                                                           |
 +=========+===================================================================+
+| 8.9     | Added the ``tstates`` hardware state attribute                    |
++---------+-------------------------------------------------------------------+
 | 6.2     | The ``--move``, ``--poke`` and ``--reg`` options accept           |
 |         | hexadecimal integers prefixed by '0x'                             |
 +---------+-------------------------------------------------------------------+
 | 5.3     | New                                                               |
 +---------+-------------------------------------------------------------------+
 
 .. _tap2sna.py:
@@ -1267,14 +1271,18 @@
 
   Convert a TAP or TZX file (which may be inside a zip archive) into a Z80
   snapshot. INPUT may be the full URL to a remote zip archive or TAP/TZX file,
   or the path to a local file. Arguments may be read from FILE instead of (or as
   well as) being given on the command line.
 
   Options:
+    -c name=value, --sim-load-config name=value
+                          Set the value of a --sim-load configuration parameter.
+                          Do '-c help' for more information. This option may be
+                          used multiple times.
     -d DIR, --output-dir DIR
                           Write the snapshot file in this directory.
     -f, --force           Overwrite an existing snapshot.
     -p STACK, --stack STACK
                           Set the stack pointer.
     --ram OPERATION       Perform a load operation or otherwise modify the
                           memory snapshot being built. Do '--ram help' for more
@@ -1283,52 +1291,38 @@
                           information. This option may be used multiple times.
     -s START, --start START
                           Set the start address to JP to.
     --sim-load            Simulate a 48K ZX Spectrum running LOAD "".
     --state name=value    Set a hardware state attribute. Do '--state help' for
                           more information. This option may be used multiple
                           times.
+    --tape-name NAME      Specify the name of a TAP/TZX file in a zip archive.
+    --tape-start BLOCK    Start the tape at this block number.
+    --tape-stop BLOCK     Stop the tape at this block number.
+    --tape-sum MD5SUM     Specify the MD5 checksum of the TAP/TZX file.
     -u AGENT, --user-agent AGENT
                           Set the User-Agent header.
     -V, --version         Show SkoolKit version number and exit.
 
-Note that support for TZX files is limited to block types 0x10 (standard speed
-data), 0x11 (turbo speed data) and 0x14 (pure data).
+Note that `tap2sna.py` can read data from TZX block types 0x10 (standard speed
+data), 0x11 (turbo speed data) and 0x14 (pure data), but not block types 0x15
+(direct recording), 0x18 (CSW recording) or 0x19 (generalized data block).
 
 By default, `tap2sna.py` loads bytes from every data block on the tape, using
 the start address given in the corresponding header. For tapes that contain
 headerless data blocks, headers with incorrect start addresses, or irrelevant
 blocks, the ``--ram`` option can be used to load bytes from specific blocks at
 the appropriate addresses. For example::
 
   $ tap2sna.py --ram load=3,30000 game.tzx game.z80
 
 loads the third block on the tape at address 30000, and ignores all other
 blocks. (To see information on the blocks in a TAP or TZX file, use the
 :ref:`tapinfo.py` command.)
 
-An alternative to the ``--ram load`` approach is the ``--sim-load`` option. It
-simulates a freshly booted 48K ZX Spectrum running LOAD "" (or LOAD ""CODE, if
-the first block on the tape is a 'Bytes' header). Whenever the Spectrum ROM's
-load routine at $0556 is called, a shortcut is taken by fast loading the next
-block on the tape. All other code (including any custom loader) is fully
-simulated. Simulation continues until the program counter hits the start
-address given by the ``--start`` option, or 10 minutes of simulated Z80 CPU
-time has elapsed, or the end of the tape is reached and one of the following
-conditions is satisfied:
-
-* a custom loader was detected
-* the program counter hits an address outside the ROM
-* more than one second of simulated Z80 CPU time has elapsed since the end of
-  the tape was reached
-
-The simulation can also be aborted by pressing Ctrl-C. When a simulated LOAD
-has completed or been aborted, the values of the registers (including the
-program counter) in the simulator are used to populate the Z80 snapshot.
-
 In addition to loading specific blocks, the ``--ram`` option can also be used
 to move blocks of bytes from one location to another, POKE values into
 individual addresses or address ranges, modify memory with XOR and ADD
 operations, initialise the system variables, or call a Python function to
 modify the memory snapshot in an arbitrary way before it is saved. For more
 information on these operations, run::
 
@@ -1354,17 +1348,96 @@
 then::
 
   $ tap2sna.py @game.t2s
 
 will create `game.z80` as if the arguments specified in `game.t2s` had been
 given on the command line.
 
+Simulated LOAD
+^^^^^^^^^^^^^^
+An alternative to the ``--ram load`` approach is the ``--sim-load`` option. It
+simulates a freshly booted 48K ZX Spectrum running LOAD "" (or LOAD ""CODE, if
+the first block on the tape is a 'Bytes' header). Whenever the Spectrum ROM's
+load routine at $0556 is called, a shortcut is taken by "fast loading" the next
+block on the tape. All other code (including any custom loader) is fully
+simulated. Simulation continues until the program counter hits the start
+address given by the ``--start`` option, or 15 minutes of simulated Z80 CPU
+time has elapsed, or the end of the tape is reached and one of the following
+conditions is satisfied:
+
+* a custom loader was detected
+* the program counter hits an address outside the ROM
+* more than one second of simulated Z80 CPU time has elapsed since the end of
+  the tape was reached
+
+A simulated LOAD can also be aborted by pressing Ctrl-C. When a simulated LOAD
+has completed or been aborted, the values of the registers (including the
+program counter) in the simulator are used to populate the Z80 snapshot.
+
+A simulated LOAD can be configured via parameters that are set by the
+``--sim-load-config`` (or ``-c``) option. The recognised configuration
+parameters are:
+
+* ``accelerator`` - the tape-sampling loop accelerator to use (default:
+  automatically selected - see below); use this to specify a particular
+  accelerator (which may produce a faster simulated LOAD), or to disable
+  acceleration entirely (``accelerator=none``)
+* ``fast-load`` - enable fast loading (``1``, the default), or disable it
+  (``0``); fast loading significantly reduces the load time for many tapes, but
+  can also cause some loaders to fail
+* ``first-edge`` - the time (in T-states) from the start of the tape at which
+  to place the leading edge of the first pulse (default: ``-2168``); the
+  default value places the trailing edge of the first pulse at time 0, but some
+  loaders (e.g. polarity-sensitive loaders) require ``first-edge=0``
+* ``pause`` - pause the tape between blocks and resume playback when port 254
+  is read (``1``, the default), or run the tape continuously (``0``); pausing
+  can help with tapes that require (but do not actually contain) long pauses
+  between blocks, but can cause some loaders to fail
+* ``timeout`` - the number of seconds of Z80 CPU time after which to abort the
+  simulated LOAD if it's still in progress (default: 900)
+* ``trace`` - the file to which to log all instructions executed during the
+  simulated LOAD (default: none)
+
+The names of the available tape-sampling loop accelerators are:
+
+* ``alkatraz`` (Alkatraz)
+* ``alkatraz2`` (Alkatraz 2)
+* ``bleepload`` (Firebird BleepLoad)
+* ``cyberlode`` (Cyberlode 1.1)
+* ``digital-integration`` (Digital Integration)
+* ``dinaload`` (Dinaload)
+* ``edge`` (Edge)
+* ``elite-uni-loader`` (Elite Uni-Loader)
+* ``excelerator`` (The Excelerator Loader)
+* ``flash-loader`` (Flash Loader)
+* ``ftl`` (FTL)
+* ``gargoyle`` (Gargoyle)
+* ``gremlin`` (various games published by Gremlin Graphics)
+* ``hewson-slowload`` (Hewson Slowload)
+* ``injectaload`` (Injectaload)
+* ``microsphere`` (Back to Skool, Skool Daze, Sky Ranger)
+* ``none`` (no accelerator)
+* ``paul-owens`` (Paul Owens Protection System)
+* ``poliload`` (Poliload)
+* ``power-load`` (Power-Load)
+* ``rom`` (any loader whose sampling loop is the same as the ROM's)
+* ``search-loader`` (Search Loader)
+* ``softlock`` (SoftLock)
+* ``speedlock`` (Speedlock - all versions)
+* ``zydroload`` (Zydroload)
+
 +---------+-------------------------------------------------------------------+
 | Version | Changes                                                           |
 +=========+===================================================================+
+| 8.9     | Added the ``--sim-load-config``, ``--tape-name``,                 |
+|         | ``--tape-start``, ``--tape-stop`` and ``--tape-sum`` options;     |
+|         | added support for TZX loops, pauses, and unused bits in data      |
+|         | blocks; added support for quoted arguments in an arguments file;  |
+|         | added the ``tstates`` hardware state attribute                    |
++---------+-------------------------------------------------------------------+
 | 8.8     | The ``--sim-load`` option performs any ``call/move/poke/sysvars`` |
 |         | operations specified by ``--ram``                                 |
 +---------+-------------------------------------------------------------------+
 | 8.7     | Added the ``--sim-load`` option; when a headerless block is       |
 |         | ignored because no ``--ram load`` options have been specified, a  |
 |         | warning is printed                                                |
 +---------+-------------------------------------------------------------------+
@@ -1412,14 +1485,16 @@
                           (default 23755).
     -d, --data            Show the entire contents of header and data blocks.
     -V, --version         Show SkoolKit version number and exit.
 
 +---------+-------------------------------------------------------------------+
 | Version | Changes                                                           |
 +=========+===================================================================+
+| 8.9     | Shows full info for TZX block types 0x10 and 0x11                 |
++---------+-------------------------------------------------------------------+
 | 8.3     | Added the ``--data`` option                                       |
 +---------+-------------------------------------------------------------------+
 | 8.1     | Shows contents of TZX block types 0x33 (hardware type) and 0x35   |
 |         | (custom info)                                                     |
 +---------+-------------------------------------------------------------------+
 | 7.1     | Shows pulse lengths in TZX block type 0x13 and full info for TZX  |
 |         | block type 0x14                                                   |
@@ -1449,14 +1524,15 @@
   SNA, SZX or Z80 snapshot, or '.' for no snapshot.
 
   Options:
     --audio               Show audio delays.
     --depth DEPTH         Simplify audio delays to this depth (default: 2).
     -D, --decimal         Show decimal values in verbose mode.
     --dump FILE           Dump a Z80 snapshot to this file after execution.
+    -i, --interrupts      Execute interrupt routines.
     --max-operations MAX  Maximum number of instructions to execute.
     --max-tstates MAX     Maximum number of T-states to run for.
     -o ADDR, --org ADDR   Specify the origin address of a binary (raw memory)
                           file (default: 65536 - length).
     -p a[-b[-c]],[^+]v, --poke a[-b[-c]],[^+]v
                           POKE N,v for N in {a, a+c, a+2c..., b}. Prefix 'v'
                           with '^' to perform an XOR operation, or '+' to
@@ -1474,22 +1550,27 @@
     -v, --verbose         Show executed instructions. Repeat this option to show
                           register values too.
     -V, --version         Show SkoolKit version number and exit.
 
 By default, `trace.py` silently simulates code execution beginning with the
 instruction at the address specified by the ``--start`` option (or the program
 counter in the snapshot) and ending when the instruction at the address
-specified by ``--stop`` (if any) is reached. Use the ``--verbose`` option to
-show each instruction executed. Repeat the ``--verbose`` option (``-vv``) to
-show register values too.
+specified by ``--stop`` (if any) is reached, and does not execute interrupt
+routines. Use the ``--verbose`` option to show each instruction executed.
+Repeat the ``--verbose`` option (``-vv``) to show register values too. Use the
+``--interrupts`` option to enable the execution of interrupt routines.
 
 When the ``--audio`` option is given, `trace.py` tracks changes in the state
 of the ZX Spectrum speaker, and then prints a list of the delays (in T-states)
 between those changes. This list can be supplied to the :ref:`AUDIO` macro to
 produce a WAV file for the sound effect that would be produced by the same code
 running on a real ZX Spectrum.
 
-+---------+---------+
-| Version | Changes |
-+=========+=========+
-| 8.8     | New     |
-+---------+---------+
++---------+-------------------------------------------------------------------+
+| Version | Changes                                                           |
++=========+===================================================================+
+| 8.9     | Added the ``--interrupts`` option; reads and writes the T-states  |
+|         | counter in Z80 snapshots and reads the T-states counter in SZX    |
+|         | snapshots                                                         |
++---------+-------------------------------------------------------------------+
+| 8.8     | New                                                               |
++---------+-------------------------------------------------------------------+
```

### Comparing `skoolkit-8.8/docs/_sources/components.rst.txt` & `skoolkit-8.9/docs/_sources/components.rst.txt`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_sources/control-files.rst.txt` & `skoolkit-8.9/docs/_sources/control-files.rst.txt`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_sources/diy.rst.txt` & `skoolkit-8.9/docs/_sources/diy.rst.txt`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_sources/extending.rst.txt` & `skoolkit-8.9/docs/_sources/extending.rst.txt`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_sources/html-templates.rst.txt` & `skoolkit-8.9/docs/_sources/html-templates.rst.txt`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_sources/man/bin2sna.py.rst.txt` & `skoolkit-8.9/docs/_sources/man/bin2sna.py.rst.txt`

 * *Files 8% similar despite different names*

```diff
@@ -83,24 +83,21 @@
 HARDWARE STATE
 ==============
 The ``--state`` option sets a hardware state attribute.
 
 |
 |  ``--state name=value``
 
-Recognised attribute names are:
+Recognised attribute names and their default values are:
 
-``border``
-  border colour
-
-``iff``
-  interrupt flip-flop: 0=disabled, 1=enabled
-
-``im``
-  interrupt mode
+|
+|  ``border``  - border colour (default=0)
+|  ``iff``     - interrupt flip-flop: 0=disabled, 1=enabled (default=1)
+|  ``im``      - interrupt mode (default=1)
+|  ``tstates`` - T-states elapsed since start of frame (default=0)
 
 EXAMPLES
 ========
 1. Convert ``game.bin`` into a Z80 snapshot named ``game.z80``:
 
    |
    |   ``bin2sna.py game.bin``
```

### Comparing `skoolkit-8.8/docs/_sources/man/bin2tap.py.rst.txt` & `skoolkit-8.9/docs/_sources/man/bin2tap.py.rst.txt`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_sources/man/skool2asm.py.rst.txt` & `skoolkit-8.9/docs/_sources/man/skool2asm.py.rst.txt`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_sources/man/skool2bin.py.rst.txt` & `skoolkit-8.9/docs/_sources/man/skool2bin.py.rst.txt`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_sources/man/skool2ctl.py.rst.txt` & `skoolkit-8.9/docs/_sources/man/skool2ctl.py.rst.txt`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_sources/man/skool2html.py.rst.txt` & `skoolkit-8.9/docs/_sources/man/skool2html.py.rst.txt`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_sources/man/sna2ctl.py.rst.txt` & `skoolkit-8.9/docs/_sources/man/sna2ctl.py.rst.txt`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_sources/man/sna2img.py.rst.txt` & `skoolkit-8.9/docs/_sources/man/sna2img.py.rst.txt`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_sources/man/sna2skool.py.rst.txt` & `skoolkit-8.9/docs/_sources/man/sna2skool.py.rst.txt`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_sources/man/snapinfo.py.rst.txt` & `skoolkit-8.9/docs/_sources/man/snapinfo.py.rst.txt`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_sources/man/snapmod.py.rst.txt` & `skoolkit-8.9/docs/_sources/man/snapmod.py.rst.txt`

 * *Files 13% similar despite different names*

```diff
@@ -68,30 +68,27 @@
 HARDWARE STATE
 ==============
 The ``--state`` option sets a hardware state attribute.
 
 |
 |  ``--state name=value``
 
-Recognised attribute names are:
+Recognised attribute names and their default values are:
 
-``border``
-  border colour
-
-``iff``
-  interrupt flip-flop: 0=disabled, 1=enabled
-
-``im``
-  interrupt mode
+|
+|  ``border``  - border colour (default=0)
+|  ``iff``     - interrupt flip-flop: 0=disabled, 1=enabled (default=1)
+|  ``im``      - interrupt mode (default=1)
+|  ``tstates`` - T-states elapsed since start of frame (default=0)
 
 EXAMPLES
 ========
-1. Set the value of the HL register pair to 0 in game.z80:
+1. Set the value of the HL register pair to 0 in ``game.z80``:
 
    |
    |   ``snapmod.py -f -r hl=0 game.z80``
 
-2. POKE the value 23 into address 32768 in game.z80, and write the resultant
-   snapshot to poked.z80:
+2. POKE the value 23 into address 32768 in ``game.z80``, and write the
+   resultant snapshot to ``poked.z80``:
 
    |
    |   ``snapmod.py -p 32768,23 game.z80 poked.z80``
```

### Comparing `skoolkit-8.8/docs/_sources/man/tapinfo.py.rst.txt` & `skoolkit-8.9/docs/_sources/man/tapinfo.py.rst.txt`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_sources/man/trace.py.rst.txt` & `skoolkit-8.9/docs/_sources/man/trace.py.rst.txt`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,17 @@
 
 -D, --decimal
   Show decimal values in verbose (``-v``, ``-vv``) mode.
 
 --dump `FILE`
   Dump a Z80 snapshot to this file after execution.
 
+-i, --interrupts
+  Execute interrupt routines.
+
 --max-operations `MAX`
   Maximum number of instructions to execute. Overrides the `STOP` address (if
   given).
 
 --max-tstates `MAX`
   Maximum number of (simulated) T-states to run for. Overrides the `STOP`
   address (if given).
```

### Comparing `skoolkit-8.8/docs/_sources/migration.rst.txt` & `skoolkit-8.9/docs/_sources/migration.rst.txt`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_sources/parsing.rst.txt` & `skoolkit-8.9/docs/_sources/parsing.rst.txt`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_sources/ref-files.rst.txt` & `skoolkit-8.9/docs/_sources/ref-files.rst.txt`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_sources/skool-files.rst.txt` & `skoolkit-8.9/docs/_sources/skool-files.rst.txt`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_sources/skool-macros.rst.txt` & `skoolkit-8.9/docs/_sources/skool-macros.rst.txt`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_sources/usage.rst.txt` & `skoolkit-8.9/docs/_sources/usage.rst.txt`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_sources/whatis.rst.txt` & `skoolkit-8.9/docs/_sources/whatis.rst.txt`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_static/basic.css` & `skoolkit-8.9/docs/_static/basic.css`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_static/classic.css` & `skoolkit-8.9/docs/_static/classic.css`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_static/doctools.js` & `skoolkit-8.9/docs/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_static/jquery.js` & `skoolkit-8.9/docs/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_static/language_data.js` & `skoolkit-8.9/docs/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_static/pygments.css` & `skoolkit-8.9/docs/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_static/searchtools.js` & `skoolkit-8.9/docs/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_static/sidebar.js` & `skoolkit-8.9/docs/_static/sidebar.js`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/_static/underscore.js` & `skoolkit-8.9/docs/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/docs/asm-templates.html` & `skoolkit-8.9/docs/asm-templates.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>ASM templates &#8212; SkoolKit 8.8 documentation</title>
+    <title>ASM templates &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
@@ -31,15 +31,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="html-templates.html" title="HTML templates"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="asm.html" title="ASM modes and directives"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">ASM templates</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -228,17 +228,17 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="html-templates.html" title="HTML templates"
              >next</a> |</li>
         <li class="right" >
           <a href="asm.html" title="ASM modes and directives"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">ASM templates</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * ASM templates
 ****** ASM templatesÂ¶ ******
 Each line of output produced by skool2asm.py is built from a template. A
 template contains âreplacement fieldsâ - identifiers enclosed by braces (
 { and }) - that are replaced by appropriate content (such as a label or
 register name) when the template is formatted.
 The default templates can be overridden by custom templates read from a file by
@@ -108,10 +108,10 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * ASM templates
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/asm.html` & `skoolkit-8.9/docs/asm.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>ASM modes and directives &#8212; SkoolKit 8.8 documentation</title>
+    <title>ASM modes and directives &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
@@ -31,15 +31,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="asm-templates.html" title="ASM templates"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="ref-files.html" title="Ref files"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">ASM modes and directives</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -1643,17 +1643,17 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="asm-templates.html" title="ASM templates"
              >next</a> |</li>
         <li class="right" >
           <a href="ref-files.html" title="Ref files"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">ASM modes and directives</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * ASM modes and directives
 ****** ASM modes and directivesÂ¶ ******
 A skool file may contain directives that are processed during the parsing
 phase. Exactly how a directive is processed (and whether it is executed)
 depends on the âsubstitution modeâ and âbugfix modeâ in which the skool
 file is being parsed.
 ***** Substitution modesÂ¶ *****
@@ -921,10 +921,10 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * ASM modes and directives
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/assemblers.html` & `skoolkit-8.9/docs/assemblers.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Supported assemblers &#8212; SkoolKit 8.8 documentation</title>
+    <title>Supported assemblers &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
@@ -31,15 +31,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="migration.html" title="Migrating from SkoolKit 7"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="commands.html" title="Commands"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Supported assemblers</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -194,17 +194,17 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="migration.html" title="Migrating from SkoolKit 7"
              >next</a> |</li>
         <li class="right" >
           <a href="commands.html" title="Commands"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Supported assemblers</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Supported assemblers
 ****** Supported assemblersÂ¶ ******
 If you use SkoolKit to generate an ASM version of your disassembly, and you
 want to assemble it, you will need to use a supported assembler. At the time of
 writing, the assemblers listed below are known to work with the ASM format
 generated by skool2asm.py:
     * pasmo (v0.5.3)
@@ -83,10 +83,10 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Supported assemblers
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/changelog.html` & `skoolkit-8.9/docs/changelog.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Changelog &#8212; SkoolKit 8.8 documentation</title>
+    <title>Changelog &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
@@ -31,44 +31,87 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="changelog7.html" title="SkoolKit 7.x changelog"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="migration.html" title="Migrating from SkoolKit 7"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Changelog</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body" role="main">
             
   <div class="section" id="changelog">
 <h1>Changelog<a class="headerlink" href="#changelog" title="Permalink to this headline">¶</a></h1>
 <div class="section" id="id1">
-<h2>8.8 (2022-11-19)<a class="headerlink" href="#id1" title="Permalink to this headline">¶</a></h2>
+<h2>8.9 (2023-02-19)<a class="headerlink" href="#id1" title="Permalink to this headline">¶</a></h2>
+<ul class="simple">
+<li><p>Added support to <a class="reference internal" href="commands.html#tap2sna-py"><span class="std std-ref">tap2sna.py</span></a> for TZX loops (block types 0x24 and 0x25),
+pauses (block types 0x10, 0x11, 0x14 and 0x20), and unused bits in data
+blocks (block types 0x11 and 0x14)</p></li>
+<li><p><a class="reference internal" href="commands.html#tap2sna-py"><span class="std std-ref">tap2sna.py</span></a> now accelerates the simulation of tape-sampling loops in
+loading routines, and also simulates the execution of interrupt routines when
+interrupts are enabled</p></li>
+<li><p>Added the <code class="docutils literal notranslate"><span class="pre">--sim-load-config</span></code> option to <a class="reference internal" href="commands.html#tap2sna-py"><span class="std std-ref">tap2sna.py</span></a> (to set the value
+of a <code class="docutils literal notranslate"><span class="pre">--sim-load</span></code> configuration parameter: <code class="docutils literal notranslate"><span class="pre">accelerator</span></code>, <code class="docutils literal notranslate"><span class="pre">fast-load</span></code>,
+<code class="docutils literal notranslate"><span class="pre">first-edge</span></code>, <code class="docutils literal notranslate"><span class="pre">pause</span></code>, <code class="docutils literal notranslate"><span class="pre">timeout</span></code>, <code class="docutils literal notranslate"><span class="pre">trace</span></code>)</p></li>
+<li><p>Added the <code class="docutils literal notranslate"><span class="pre">--tape-name</span></code> option to <a class="reference internal" href="commands.html#tap2sna-py"><span class="std std-ref">tap2sna.py</span></a> (to specify the name of
+a TAP/TZX file in a zip archive, in case there is more than one)</p></li>
+<li><p>Added the <code class="docutils literal notranslate"><span class="pre">--tape-start</span></code> and <code class="docutils literal notranslate"><span class="pre">--tape-stop</span></code> options to <a class="reference internal" href="commands.html#tap2sna-py"><span class="std std-ref">tap2sna.py</span></a>
+(to start or stop the tape at a specific block number)</p></li>
+<li><p>Added the <code class="docutils literal notranslate"><span class="pre">--tape-sum</span></code> option to <a class="reference internal" href="commands.html#tap2sna-py"><span class="std std-ref">tap2sna.py</span></a> (to specify the MD5
+checksum of the TAP/TZX file)</p></li>
+<li><p>Added support to <a class="reference internal" href="commands.html#tap2sna-py"><span class="std std-ref">tap2sna.py</span></a> for quoted arguments in an arguments file</p></li>
+<li><p>Added the <code class="docutils literal notranslate"><span class="pre">--interrupts</span></code> option to <a class="reference internal" href="commands.html#trace-py"><span class="std std-ref">trace.py</span></a> (to enable the execution
+of interrupt routines)</p></li>
+<li><p><a class="reference internal" href="commands.html#trace-py"><span class="std std-ref">trace.py</span></a> now reads and writes the T-states counter in Z80 snapshots
+and reads the T-states counter in SZX snapshots</p></li>
+<li><p>Added support to <a class="reference internal" href="commands.html#bin2sna-py"><span class="std std-ref">bin2sna.py</span></a>, <a class="reference internal" href="commands.html#snapmod-py"><span class="std std-ref">snapmod.py</span></a> and <a class="reference internal" href="commands.html#tap2sna-py"><span class="std std-ref">tap2sna.py</span></a>
+for setting the <code class="docutils literal notranslate"><span class="pre">tstates</span></code> hardware attribute (i.e. the T-states counter in
+Z80 snapshots)</p></li>
+<li><p><a class="reference internal" href="commands.html#tapinfo-py"><span class="std std-ref">tapinfo.py</span></a> now shows full info for TZX block types 0x10 (standard
+speed data) and 0x11 (turbo speed data)</p></li>
+<li><p>Fixed how the Z80 instruction set simulator updates the A and R registers in
+the ‘LD A,R’ and ‘LD R,A’ instructions</p></li>
+<li><p>Fixed how the Z80 instruction set simulator handles a CALL instruction that
+overwrites its own address operand</p></li>
+<li><p>Fixed how a Z80 snapshot memory block that ends with a single 0xED byte is
+decompressed</p></li>
+<li><p>Fixed how the <code class="docutils literal notranslate"><span class="pre">--sim-load</span></code> option of <a class="reference internal" href="commands.html#tap2sna-py"><span class="std std-ref">tap2sna.py</span></a> transitions from a
+tape block that ends with data to the next block when there is no pause
+between them</p></li>
+<li><p>Fixed the bug that prevents the <code class="docutils literal notranslate"><span class="pre">--find</span></code> option of <a class="reference internal" href="commands.html#snapinfo-py"><span class="std std-ref">snapinfo.py</span></a> from
+finding byte sequences below address 16384</p></li>
+<li><p>Fixed the bug that prevents the <code class="docutils literal notranslate"><span class="pre">--find-text</span></code> option of <a class="reference internal" href="commands.html#snapinfo-py"><span class="std std-ref">snapinfo.py</span></a>
+from finding text strings below address 16384</p></li>
+</ul>
+</div>
+<div class="section" id="id2">
+<h2>8.8 (2022-11-19)<a class="headerlink" href="#id2" title="Permalink to this headline">¶</a></h2>
 <ul class="simple">
 <li><p>Added the <a class="reference internal" href="commands.html#trace-py"><span class="std std-ref">trace.py</span></a> command (for tracing the execution of machine code
 in a 48K memory snapshot)</p></li>
 <li><p>The <code class="docutils literal notranslate"><span class="pre">--sim-load</span></code> option of <a class="reference internal" href="commands.html#tap2sna-py"><span class="std std-ref">tap2sna.py</span></a> now performs any <code class="docutils literal notranslate"><span class="pre">call</span></code>,
 <code class="docutils literal notranslate"><span class="pre">move</span></code>, <code class="docutils literal notranslate"><span class="pre">poke</span></code> and <code class="docutils literal notranslate"><span class="pre">sysvars</span></code> operations specified by the <code class="docutils literal notranslate"><span class="pre">--ram</span></code>
 option</p></li>
 <li><p>Improved the performance of the <code class="docutils literal notranslate"><span class="pre">--sim-load</span></code> option of <a class="reference internal" href="commands.html#tap2sna-py"><span class="std std-ref">tap2sna.py</span></a></p></li>
 <li><p>Improved the performance of the <a class="reference internal" href="skool-macros.html#sim"><span class="std std-ref">#SIM</span></a> macro</p></li>
 <li><p>Improved the performance of the <a class="reference internal" href="skool-macros.html#audio"><span class="std std-ref">#AUDIO</span></a> and <a class="reference internal" href="skool-macros.html#tstates"><span class="std std-ref">#TSTATES</span></a> macros when
 they execute instructions in a simulator</p></li>
 <li><p>Removed the <code class="docutils literal notranslate"><span class="pre">MaxAmplitude</span></code> parameter from the <a class="reference internal" href="ref-files.html#ref-audiowriter"><span class="std std-ref">[AudioWriter]</span></a>
 section</p></li>
 </ul>
 </div>
-<div class="section" id="id2">
-<h2>8.7 (2022-10-08)<a class="headerlink" href="#id2" title="Permalink to this headline">¶</a></h2>
+<div class="section" id="id3">
+<h2>8.7 (2022-10-08)<a class="headerlink" href="#id3" title="Permalink to this headline">¶</a></h2>
 <ul class="simple">
 <li><p>Dropped support for Python 3.6</p></li>
 <li><p>Added the <a class="reference internal" href="skool-macros.html#sim"><span class="std std-ref">#SIM</span></a> macro (for simulating the execution of machine code in
 the internal memory snapshot constructed from the contents of the skool file)</p></li>
 <li><p>Added the <a class="reference internal" href="skool-macros.html#audio"><span class="std std-ref">#AUDIO</span></a> macro (for creating HTML5 <code class="docutils literal notranslate"><span class="pre">&lt;audio&gt;</span></code> elements, and
 optionally creating audio files in WAV format)</p></li>
 <li><p>Added the <a class="reference internal" href="skool-macros.html#tstates"><span class="std std-ref">#TSTATES</span></a> macro (which expands to the time taken, in T-states,
@@ -106,16 +149,16 @@
 register names</p></li>
 <li><p>Fixed the bug where the <code class="docutils literal notranslate"><span class="pre">stop</span></code> value of the <a class="reference internal" href="skool-macros.html#for"><span class="std std-ref">#FOR</span></a> macro is used even
 when it does not differ from <code class="docutils literal notranslate"><span class="pre">start</span></code> by a multiple of <code class="docutils literal notranslate"><span class="pre">step</span></code></p></li>
 <li><p>Fixed the bug where an <a class="reference internal" href="control-files.html#mdirective"><span class="std std-ref">M directive</span></a> with an explicit length overrides
 the sublengths of an earlier sub-block directive at the same address</p></li>
 </ul>
 </div>
-<div class="section" id="id3">
-<h2>8.6 (2021-11-06)<a class="headerlink" href="#id3" title="Permalink to this headline">¶</a></h2>
+<div class="section" id="id4">
+<h2>8.6 (2021-11-06)<a class="headerlink" href="#id4" title="Permalink to this headline">¶</a></h2>
 <ul class="simple">
 <li><p>Added the <a class="reference internal" href="skool-macros.html#str"><span class="std std-ref">#STR</span></a> macro (for retrieving the text string at a given address
 in the memory snapshot)</p></li>
 <li><p>Added the <a class="reference internal" href="skool-macros.html#while"><span class="std std-ref">#WHILE</span></a> macro (for repeatedly expanding macros until a
 conditional expression becomes false)</p></li>
 <li><p>Added the <a class="reference internal" href="skool-macros.html#udgs"><span class="std std-ref">#UDGS</span></a> macro (as an alternative to the <a class="reference internal" href="skool-macros.html#udgarray"><span class="std std-ref">#UDGARRAY</span></a> macro
 for creating an image of a rectangular array of UDGs)</p></li>
@@ -135,16 +178,16 @@
 multiple ref file sections</p></li>
 <li><p>Added the <code class="docutils literal notranslate"><span class="pre">tindex</span></code> and <code class="docutils literal notranslate"><span class="pre">alpha</span></code> parameters to the <a class="reference internal" href="skool-macros.html#copy"><span class="std std-ref">#COPY</span></a> macro (for
 specifying the transparent colour and its alpha value in the new frame)</p></li>
 <li><p>Fixed the bug where macros inside a <a class="reference internal" href="skool-macros.html#list"><span class="std std-ref">#LIST</span></a> or <a class="reference internal" href="skool-macros.html#table"><span class="std std-ref">#TABLE</span></a> macro are
 expanded twice in HTML mode (which makes <a class="reference internal" href="skool-macros.html#raw"><span class="std std-ref">#RAW</span></a> ineffective)</p></li>
 </ul>
 </div>
-<div class="section" id="id4">
-<h2>8.5 (2021-07-03)<a class="headerlink" href="#id4" title="Permalink to this headline">¶</a></h2>
+<div class="section" id="id5">
+<h2>8.5 (2021-07-03)<a class="headerlink" href="#id5" title="Permalink to this headline">¶</a></h2>
 <ul class="simple">
 <li><p>Dropped support for Python 3.5</p></li>
 <li><p>Added the <a class="reference internal" href="skool-macros.html#over"><span class="std std-ref">#OVER</span></a> macro (for superimposing one frame on another)</p></li>
 <li><p>Added the <a class="reference internal" href="skool-macros.html#copy"><span class="std std-ref">#COPY</span></a> macro (for copying all or part of an existing frame
 into a new frame)</p></li>
 <li><p>Added the <a class="reference internal" href="skool-macros.html#def"><span class="std std-ref">#DEF</span></a> macro (as a more powerful alternative to the
 <a class="reference internal" href="skool-macros.html#define"><span class="std std-ref">#DEFINE</span></a> macro, which is now deprecated)</p></li>
@@ -179,16 +222,16 @@
 imported)</p></li>
 <li><p>Fixed the bug where a frame whose pixels are modified by the <a class="reference internal" href="skool-macros.html#plot"><span class="std std-ref">#PLOT</span></a>
 macro may have incorrect colours when converted to an image</p></li>
 <li><p>Fixed the bug where an <code class="docutils literal notranslate"><span class="pre">M</span></code> directive in a control file is ignored when it
 is followed by a sub-block that has sublengths</p></li>
 </ul>
 </div>
-<div class="section" id="id5">
-<h2>8.4 (2021-03-06)<a class="headerlink" href="#id5" title="Permalink to this headline">¶</a></h2>
+<div class="section" id="id6">
+<h2>8.4 (2021-03-06)<a class="headerlink" href="#id6" title="Permalink to this headline">¶</a></h2>
 <ul class="simple">
 <li><p>Made the <a class="reference internal" href="components.html#imagewriter"><span class="std std-ref">image writer component</span></a> pluggable</p></li>
 <li><p>Added support for defining groups of entries (via the <a class="reference internal" href="ref-files.html#entrygroups"><span class="std std-ref">[EntryGroups]</span></a>
 section of the ref file) whose disassembly pages can be given custom titles
 and headers</p></li>
 <li><p>Added the <code class="docutils literal notranslate"><span class="pre">Address</span></code> parameter to the <a class="reference internal" href="ref-files.html#ref-game"><span class="std std-ref">[Game]</span></a> section (for
 specifying the format of address fields on disassembly pages and memory map
@@ -210,16 +253,16 @@
 configuration parameter</p></li>
 <li><p>Fixed the bug that prevents instruction comments from being repeated in a
 <a class="reference internal" href="control-files.html#ctlloops"><span class="std std-ref">control file loop</span></a></p></li>
 <li><p>Fixed the bug that makes <a class="reference internal" href="commands.html#sna2skool-py"><span class="std std-ref">sna2skool.py</span></a> ignore a given start address
 below 16384 when converting a snapshot</p></li>
 </ul>
 </div>
-<div class="section" id="id6">
-<h2>8.3 (2020-11-08)<a class="headerlink" href="#id6" title="Permalink to this headline">¶</a></h2>
+<div class="section" id="id7">
+<h2>8.3 (2020-11-08)<a class="headerlink" href="#id7" title="Permalink to this headline">¶</a></h2>
 <ul class="simple">
 <li><p>Added the <a class="reference internal" href="skool-macros.html#plot"><span class="std std-ref">#PLOT</span></a> macro (for setting, resetting or flipping a pixel in a
 frame already created by an image macro)</p></li>
 <li><p>Added the <code class="docutils literal notranslate"><span class="pre">--begin</span></code> option to <a class="reference internal" href="commands.html#bin2tap-py"><span class="std std-ref">bin2tap.py</span></a> (for specifying the address
 at which to begin conversion)</p></li>
 <li><p>The <code class="docutils literal notranslate"><span class="pre">--end</span></code> option of <a class="reference internal" href="commands.html#bin2tap-py"><span class="std std-ref">bin2tap.py</span></a> now applies to raw memory files as
 well as SNA, SZX and Z80 snapshots</p></li>
@@ -235,16 +278,16 @@
 <a class="reference internal" href="skool-macros.html#include"><span class="std std-ref">#INCLUDE</span></a>, <a class="reference internal" href="skool-macros.html#n"><span class="std std-ref">#N</span></a>, <a class="reference internal" href="skool-macros.html#pokes"><span class="std std-ref">#POKES</span></a>, <a class="reference internal" href="skool-macros.html#r"><span class="std std-ref">#R</span></a> and <a class="reference internal" href="skool-macros.html#space"><span class="std std-ref">#SPACE</span></a> macros, and
 in the integer parameters and cropping specification of the <a class="reference internal" href="skool-macros.html#font"><span class="std std-ref">#FONT</span></a>,
 <a class="reference internal" href="skool-macros.html#scr"><span class="std std-ref">#SCR</span></a>, <a class="reference internal" href="skool-macros.html#udg"><span class="std std-ref">#UDG</span></a> and <a class="reference internal" href="skool-macros.html#udgarray"><span class="std std-ref">#UDGARRAY</span></a> macros</p></li>
 <li><p>Fixed the bug that causes ‘e+1’ to be interpreted as a floating point number
 when it appears in a BASIC program</p></li>
 </ul>
 </div>
-<div class="section" id="id7">
-<h2>8.2 (2020-07-19)<a class="headerlink" href="#id7" title="Permalink to this headline">¶</a></h2>
+<div class="section" id="id8">
+<h2>8.2 (2020-07-19)<a class="headerlink" href="#id8" title="Permalink to this headline">¶</a></h2>
 <ul class="simple">
 <li><p>Added the <code class="docutils literal notranslate"><span class="pre">--call-graph</span></code> option to <a class="reference internal" href="commands.html#snapinfo-call-graph"><span class="std std-ref">snapinfo.py</span></a>
 (for generating a call graph in DOT format)</p></li>
 <li><p>Added the <code class="docutils literal notranslate"><span class="pre">--ctl</span></code> option to <a class="reference internal" href="commands.html#snapinfo-py"><span class="std std-ref">snapinfo.py</span></a> (for specifying a control
 file to use when generating a call graph)</p></li>
 <li><p>Added the <code class="docutils literal notranslate"><span class="pre">--org</span></code> option to <a class="reference internal" href="commands.html#snapinfo-py"><span class="std std-ref">snapinfo.py</span></a> along with the ability to
 read binary (raw memory) files</p></li>
@@ -270,16 +313,16 @@
 jump to or call an entry point)</p></li>
 <li><p>Added support for replacement fields in the integer parameters of the
 <a class="reference internal" href="skool-macros.html#for"><span class="std std-ref">#FOR</span></a> and <a class="reference internal" href="skool-macros.html#peek"><span class="std std-ref">#PEEK</span></a> macros</p></li>
 <li><p>Added the <code class="docutils literal notranslate"><span class="pre">--page</span></code> option to <a class="reference internal" href="commands.html#snapinfo-py"><span class="std std-ref">snapinfo.py</span></a> (for specifying the page of
 a 128K snapshot to map to 49152-65535)</p></li>
 </ul>
 </div>
-<div class="section" id="id8">
-<h2>8.1 (2020-03-29)<a class="headerlink" href="#id8" title="Permalink to this headline">¶</a></h2>
+<div class="section" id="id9">
+<h2>8.1 (2020-03-29)<a class="headerlink" href="#id9" title="Permalink to this headline">¶</a></h2>
 <ul class="simple">
 <li><p>Added the <code class="docutils literal notranslate"><span class="pre">--rsub</span></code> and <code class="docutils literal notranslate"><span class="pre">--rfix</span></code> options to <a class="reference internal" href="commands.html#skool2bin-py"><span class="std std-ref">skool2bin.py</span></a> (for
 parsing the skool file in <a class="reference internal" href="asm.html#rsubmode"><span class="std std-ref">&#64;rsub mode</span></a> and <a class="reference internal" href="asm.html#rfixmode"><span class="std std-ref">&#64;rfix mode</span></a>)</p></li>
 <li><p>Added the <code class="docutils literal notranslate"><span class="pre">--data</span></code> option to <a class="reference internal" href="commands.html#skool2bin-py"><span class="std std-ref">skool2bin.py</span></a> (for processing
 <a class="reference internal" href="asm.html#defb"><span class="std std-ref">&#64;defb</span></a>, <a class="reference internal" href="asm.html#defs"><span class="std std-ref">&#64;defs</span></a> and <a class="reference internal" href="asm.html#defw"><span class="std std-ref">&#64;defw</span></a> directives)</p></li>
 <li><p>Added the <code class="docutils literal notranslate"><span class="pre">--verbose</span></code> option to <a class="reference internal" href="commands.html#skool2bin-py"><span class="std std-ref">skool2bin.py</span></a> (for showing
 information on each converted instruction)</p></li>
@@ -307,16 +350,16 @@
 addresses for which to suppress warnings</p></li>
 <li><p>Added support to <a class="reference internal" href="commands.html#sna2skool-py"><span class="std std-ref">sna2skool.py</span></a> for ignoring default control files (by
 specifying <code class="docutils literal notranslate"><span class="pre">--ctl</span> <span class="pre">0</span></code>)</p></li>
 <li><p>Fixed how <a class="reference internal" href="commands.html#sna2skool-py"><span class="std std-ref">sna2skool.py</span></a> works with dot directives in a control file
 when an end address is specified</p></li>
 </ul>
 </div>
-<div class="section" id="id9">
-<h2>8.0 (2019-11-09)<a class="headerlink" href="#id9" title="Permalink to this headline">¶</a></h2>
+<div class="section" id="id10">
+<h2>8.0 (2019-11-09)<a class="headerlink" href="#id10" title="Permalink to this headline">¶</a></h2>
 <ul class="simple">
 <li><p>Dropped support for Python 3.4</p></li>
 <li><p>Made several <a class="reference internal" href="components.html#components"><span class="std std-ref">SkoolKit components</span></a> pluggable</p></li>
 <li><p>Added support for the <a class="reference internal" href="html-templates.html#td-foreach"><span class="std std-ref">foreach</span></a>, <a class="reference internal" href="html-templates.html#td-if"><span class="std std-ref">if</span></a> and <a class="reference internal" href="html-templates.html#td-include"><span class="std std-ref">include</span></a>
 directives in HTML templates</p></li>
 <li><p>Added the <a class="reference internal" href="skool-macros.html#pc"><span class="std std-ref">#PC</span></a> macro (which expands to the address of the closest
 instruction in the current entry)</p></li>
@@ -368,23 +411,24 @@
         </div>
       </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
   <h3><a href="index.html">Table of Contents</a></h3>
   <ul>
 <li><a class="reference internal" href="#">Changelog</a><ul>
-<li><a class="reference internal" href="#id1">8.8 (2022-11-19)</a></li>
-<li><a class="reference internal" href="#id2">8.7 (2022-10-08)</a></li>
-<li><a class="reference internal" href="#id3">8.6 (2021-11-06)</a></li>
-<li><a class="reference internal" href="#id4">8.5 (2021-07-03)</a></li>
-<li><a class="reference internal" href="#id5">8.4 (2021-03-06)</a></li>
-<li><a class="reference internal" href="#id6">8.3 (2020-11-08)</a></li>
-<li><a class="reference internal" href="#id7">8.2 (2020-07-19)</a></li>
-<li><a class="reference internal" href="#id8">8.1 (2020-03-29)</a></li>
-<li><a class="reference internal" href="#id9">8.0 (2019-11-09)</a></li>
+<li><a class="reference internal" href="#id1">8.9 (2023-02-19)</a></li>
+<li><a class="reference internal" href="#id2">8.8 (2022-11-19)</a></li>
+<li><a class="reference internal" href="#id3">8.7 (2022-10-08)</a></li>
+<li><a class="reference internal" href="#id4">8.6 (2021-11-06)</a></li>
+<li><a class="reference internal" href="#id5">8.5 (2021-07-03)</a></li>
+<li><a class="reference internal" href="#id6">8.4 (2021-03-06)</a></li>
+<li><a class="reference internal" href="#id7">8.3 (2020-11-08)</a></li>
+<li><a class="reference internal" href="#id8">8.2 (2020-07-19)</a></li>
+<li><a class="reference internal" href="#id9">8.1 (2020-03-29)</a></li>
+<li><a class="reference internal" href="#id10">8.0 (2019-11-09)</a></li>
 <li><a class="reference internal" href="#older-versions">Older versions</a></li>
 </ul>
 </li>
 </ul>
 
   <h4>Previous topic</h4>
   <p class="topless"><a href="migration.html"
@@ -424,17 +468,17 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="changelog7.html" title="SkoolKit 7.x changelog"
              >next</a> |</li>
         <li class="right" >
           <a href="migration.html" title="Migrating from SkoolKit 7"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Changelog</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,17 +7,55 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Changelog
 ****** ChangelogÂ¶ ******
+***** 8.9 (2023-02-19)Â¶ *****
+    * Added support to tap2sna.py for TZX loops (block types 0x24 and 0x25),
+      pauses (block types 0x10, 0x11, 0x14 and 0x20), and unused bits in data
+      blocks (block types 0x11 and 0x14)
+    * tap2sna.py now accelerates the simulation of tape-sampling loops in
+      loading routines, and also simulates the execution of interrupt routines
+      when interrupts are enabled
+    * Added the --sim-load-config option to tap2sna.py (to set the value of a -
+      -sim-load configuration parameter: accelerator, fast-load, first-edge,
+      pause, timeout, trace)
+    * Added the --tape-name option to tap2sna.py (to specify the name of a TAP/
+      TZX file in a zip archive, in case there is more than one)
+    * Added the --tape-start and --tape-stop options to tap2sna.py (to start or
+      stop the tape at a specific block number)
+    * Added the --tape-sum option to tap2sna.py (to specify the MD5 checksum of
+      the TAP/TZX file)
+    * Added support to tap2sna.py for quoted arguments in an arguments file
+    * Added the --interrupts option to trace.py (to enable the execution of
+      interrupt routines)
+    * trace.py now reads and writes the T-states counter in Z80 snapshots and
+      reads the T-states counter in SZX snapshots
+    * Added support to bin2sna.py, snapmod.py and tap2sna.py for setting the
+      tstates hardware attribute (i.e. the T-states counter in Z80 snapshots)
+    * tapinfo.py now shows full info for TZX block types 0x10 (standard speed
+      data) and 0x11 (turbo speed data)
+    * Fixed how the Z80 instruction set simulator updates the A and R registers
+      in the âLD A,Râ and âLD R,Aâ instructions
+    * Fixed how the Z80 instruction set simulator handles a CALL instruction
+      that overwrites its own address operand
+    * Fixed how a Z80 snapshot memory block that ends with a single 0xED byte
+      is decompressed
+    * Fixed how the --sim-load option of tap2sna.py transitions from a tape
+      block that ends with data to the next block when there is no pause
+      between them
+    * Fixed the bug that prevents the --find option of snapinfo.py from finding
+      byte sequences below address 16384
+    * Fixed the bug that prevents the --find-text option of snapinfo.py from
+      finding text strings below address 16384
 ***** 8.8 (2022-11-19)Â¶ *****
     * Added the trace.py command (for tracing the execution of machine code in
       a 48K memory snapshot)
     * The --sim-load option of tap2sna.py now performs any call, move, poke and
       sysvars operations specified by the --ram option
     * Improved the performance of the --sim-load option of tap2sna.py
     * Improved the performance of the #SIM macro
@@ -265,14 +303,15 @@
     * SkoolKit_5.x_changelog
     * SkoolKit_4.x_changelog
     * SkoolKit_3.x_changelog
     * SkoolKit_2.x_changelog
     * SkoolKit_1.x_changelog
 **** Table_of_Contents ****
     * Changelog
+          o 8.9_(2023-02-19)
           o 8.8_(2022-11-19)
           o 8.7_(2022-10-08)
           o 8.6_(2021-11-06)
           o 8.5_(2021-07-03)
           o 8.4_(2021-03-06)
           o 8.3_(2020-11-08)
           o 8.2_(2020-07-19)
@@ -288,10 +327,10 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Changelog
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/changelog1.html` & `skoolkit-8.9/docs/changelog1.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>SkoolKit 1.x changelog &#8212; SkoolKit 8.8 documentation</title>
+    <title>SkoolKit 1.x changelog &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
@@ -31,15 +31,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="parsing.html" title="Parsing, rendering, and modes"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="changelog2.html" title="SkoolKit 2.x changelog"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="changelog.html" accesskey="U">Changelog</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">SkoolKit 1.x changelog</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -230,18 +230,18 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="parsing.html" title="Parsing, rendering, and modes"
              >next</a> |</li>
         <li class="right" >
           <a href="changelog2.html" title="SkoolKit 2.x changelog"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="changelog.html" >Changelog</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">SkoolKit 1.x changelog</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Changelog »
     * SkoolKit 1.x changelog
 ****** SkoolKit 1.x changelogÂ¶ ******
 ***** 1.4 (2010-11-11)Â¶ *****
     * Updated the Skool Daze disassembly
     * Updated the Back to Skool disassembly
     * Updated the incomplete Contact Sam Cruise disassembly
@@ -106,11 +106,11 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Changelog »
     * SkoolKit 1.x changelog
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/changelog2.html` & `skoolkit-8.9/docs/changelog2.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>SkoolKit 2.x changelog &#8212; SkoolKit 8.8 documentation</title>
+    <title>SkoolKit 2.x changelog &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
@@ -31,15 +31,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="changelog1.html" title="SkoolKit 1.x changelog"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="changelog3.html" title="SkoolKit 3.x changelog"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="changelog.html" accesskey="U">Changelog</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">SkoolKit 2.x changelog</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -402,18 +402,18 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="changelog1.html" title="SkoolKit 1.x changelog"
              >next</a> |</li>
         <li class="right" >
           <a href="changelog3.html" title="SkoolKit 3.x changelog"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="changelog.html" >Changelog</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">SkoolKit 2.x changelog</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Changelog »
     * SkoolKit 2.x changelog
 ****** SkoolKit 2.x changelogÂ¶ ******
 ***** 2.5 (2012-02-22)Â¶ *****
     * Added support for [MemoryMap:*] sections in ref files (for defining the
       properties of memory map pages); removed support for the [MapDetails]
       section accordingly
@@ -235,11 +235,11 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Changelog »
     * SkoolKit 2.x changelog
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/changelog3.html` & `skoolkit-8.9/docs/changelog3.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>SkoolKit 3.x changelog &#8212; SkoolKit 8.8 documentation</title>
+    <title>SkoolKit 3.x changelog &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
@@ -31,15 +31,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="changelog2.html" title="SkoolKit 2.x changelog"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="changelog4.html" title="SkoolKit 4.x changelog"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="changelog.html" accesskey="U">Changelog</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">SkoolKit 3.x changelog</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -386,18 +386,18 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="changelog2.html" title="SkoolKit 2.x changelog"
              >next</a> |</li>
         <li class="right" >
           <a href="changelog4.html" title="SkoolKit 4.x changelog"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="changelog.html" >Changelog</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">SkoolKit 3.x changelog</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Changelog »
     * SkoolKit 3.x changelog
 ****** SkoolKit 3.x changelogÂ¶ ******
 ***** 3.7 (2014-03-08)Â¶ *****
     * Added support for numbers in binary notation (e.g. %10101010)
     * Added the s and S control directives for encoding DEFS statements (with
       optional non-zero byte values); the z and Z directives are now deprecated
@@ -238,11 +238,11 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Changelog »
     * SkoolKit 3.x changelog
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/changelog4.html` & `skoolkit-8.9/docs/changelog4.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>SkoolKit 4.x changelog &#8212; SkoolKit 8.8 documentation</title>
+    <title>SkoolKit 4.x changelog &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
@@ -31,15 +31,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="changelog3.html" title="SkoolKit 3.x changelog"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="changelog5.html" title="SkoolKit 5.x changelog"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="changelog.html" accesskey="U">Changelog</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">SkoolKit 4.x changelog</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -257,18 +257,18 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="changelog3.html" title="SkoolKit 3.x changelog"
              >next</a> |</li>
         <li class="right" >
           <a href="changelog5.html" title="SkoolKit 5.x changelog"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="changelog.html" >Changelog</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">SkoolKit 4.x changelog</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Changelog »
     * SkoolKit 4.x changelog
 ****** SkoolKit 4.x changelogÂ¶ ******
 ***** 4.5 (2015-07-04)Â¶ *****
     * Added support to tap2sna.py for TZX block type 0x14 (pure data), for
       loading the first and last bytes of a tape block (which are usually, but
       not always, the flag and parity bytes), and for modifying memory with XOR
@@ -154,11 +154,11 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Changelog »
     * SkoolKit 4.x changelog
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/changelog5.html` & `skoolkit-8.9/docs/changelog5.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>SkoolKit 5.x changelog &#8212; SkoolKit 8.8 documentation</title>
+    <title>SkoolKit 5.x changelog &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
@@ -31,15 +31,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="changelog4.html" title="SkoolKit 4.x changelog"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="changelog6.html" title="SkoolKit 6.x changelog"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="changelog.html" accesskey="U">Changelog</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">SkoolKit 5.x changelog</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -233,18 +233,18 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="changelog4.html" title="SkoolKit 4.x changelog"
              >next</a> |</li>
         <li class="right" >
           <a href="changelog6.html" title="SkoolKit 6.x changelog"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="changelog.html" >Changelog</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">SkoolKit 5.x changelog</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Changelog »
     * SkoolKit 5.x changelog
 ****** SkoolKit 5.x changelogÂ¶ ******
 ***** 5.4 (2017-01-08)Â¶ *****
     * Added the sna2img.py command (for converting the screenshot in a SCR file
       or SNA/SZX/Z80 snapshot into a PNG or GIF file)
     * Added the @equ ASM directive (which produces an EQU directive in the ASM
@@ -133,11 +133,11 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Changelog »
     * SkoolKit 5.x changelog
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/changelog6.html` & `skoolkit-8.9/docs/changelog6.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>SkoolKit 6.x changelog &#8212; SkoolKit 8.8 documentation</title>
+    <title>SkoolKit 6.x changelog &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
@@ -31,15 +31,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="changelog5.html" title="SkoolKit 5.x changelog"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="changelog7.html" title="SkoolKit 7.x changelog"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="changelog.html" accesskey="U">Changelog</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">SkoolKit 6.x changelog</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -278,18 +278,18 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="changelog5.html" title="SkoolKit 5.x changelog"
              >next</a> |</li>
         <li class="right" >
           <a href="changelog7.html" title="SkoolKit 7.x changelog"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="changelog.html" >Changelog</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">SkoolKit 6.x changelog</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Changelog »
     * SkoolKit 6.x changelog
 ****** SkoolKit 6.x changelogÂ¶ ******
 ***** 6.4 (2018-03-31)Â¶ *****
     * Added the @if directive (for conditionally processing other ASM
       directives)
     * Added the #RAW macro (which prevents any macros or macro-like tokens in
@@ -181,11 +181,11 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Changelog »
     * SkoolKit 6.x changelog
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/changelog7.html` & `skoolkit-8.9/docs/changelog7.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>SkoolKit 7.x changelog &#8212; SkoolKit 8.8 documentation</title>
+    <title>SkoolKit 7.x changelog &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
@@ -31,15 +31,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="changelog6.html" title="SkoolKit 6.x changelog"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="changelog.html" title="Changelog"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="changelog.html" accesskey="U">Changelog</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">SkoolKit 7.x changelog</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -221,18 +221,18 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="changelog6.html" title="SkoolKit 6.x changelog"
              >next</a> |</li>
         <li class="right" >
           <a href="changelog.html" title="Changelog"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="changelog.html" >Changelog</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">SkoolKit 7.x changelog</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Changelog »
     * SkoolKit 7.x changelog
 ****** SkoolKit 7.x changelogÂ¶ ******
 ***** 7.2 (2019-06-02)Â¶ *****
     * Added support to control files for specifying comments over multiple
       lines (by using the dot_and_colon_directives)
     * Added support to skool2ctl.py for reading configuration fromskoolkit.ini
@@ -127,11 +127,11 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Changelog »
     * SkoolKit 7.x changelog
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/commands.html` & `skoolkit-8.9/docs/commands.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Commands &#8212; SkoolKit 8.8 documentation</title>
+    <title>Commands &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
@@ -31,15 +31,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="assemblers.html" title="Supported assemblers"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="diy.html" title="Disassembly DIY"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Commands</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -94,23 +94,26 @@
 <table class="docutils colwidths-auto align-default">
 <thead>
 <tr class="row-odd"><th class="head"><p>Version</p></th>
 <th class="head"><p>Changes</p></th>
 </tr>
 </thead>
 <tbody>
-<tr class="row-even"><td><p>6.3</p></td>
+<tr class="row-even"><td><p>8.9</p></td>
+<td><p>Added the <code class="docutils literal notranslate"><span class="pre">tstates</span></code> hardware state attribute</p></td>
+</tr>
+<tr class="row-odd"><td><p>6.3</p></td>
 <td><p>Added the <code class="docutils literal notranslate"><span class="pre">--poke</span></code> option</p></td>
 </tr>
-<tr class="row-odd"><td><p>6.2</p></td>
+<tr class="row-even"><td><p>6.2</p></td>
 <td><p>Added the <code class="docutils literal notranslate"><span class="pre">--reg</span></code> and <code class="docutils literal notranslate"><span class="pre">--state</span></code> options; the <code class="docutils literal notranslate"><span class="pre">--org</span></code>,
 <code class="docutils literal notranslate"><span class="pre">--stack</span></code> and <code class="docutils literal notranslate"><span class="pre">--start</span></code> options accept a hexadecimal integer
 prefixed by ‘0x’</p></td>
 </tr>
-<tr class="row-even"><td><p>5.2</p></td>
+<tr class="row-odd"><td><p>5.2</p></td>
 <td><p>New</p></td>
 </tr>
 </tbody>
 </table>
 </div>
 <div class="section" id="bin2tap-py">
 <span id="id3"></span><h2>bin2tap.py<a class="headerlink" href="#bin2tap-py" title="Permalink to this headline">¶</a></h2>
@@ -1391,19 +1394,22 @@
 <table class="docutils colwidths-auto align-default">
 <thead>
 <tr class="row-odd"><th class="head"><p>Version</p></th>
 <th class="head"><p>Changes</p></th>
 </tr>
 </thead>
 <tbody>
-<tr class="row-even"><td><p>6.2</p></td>
+<tr class="row-even"><td><p>8.9</p></td>
+<td><p>Added the <code class="docutils literal notranslate"><span class="pre">tstates</span></code> hardware state attribute</p></td>
+</tr>
+<tr class="row-odd"><td><p>6.2</p></td>
 <td><p>The <code class="docutils literal notranslate"><span class="pre">--move</span></code>, <code class="docutils literal notranslate"><span class="pre">--poke</span></code> and <code class="docutils literal notranslate"><span class="pre">--reg</span></code> options accept
 hexadecimal integers prefixed by ‘0x’</p></td>
 </tr>
-<tr class="row-odd"><td><p>5.3</p></td>
+<tr class="row-even"><td><p>5.3</p></td>
 <td><p>New</p></td>
 </tr>
 </tbody>
 </table>
 </div>
 <div class="section" id="tap2sna-py">
 <span id="id18"></span><h2>tap2sna.py<a class="headerlink" href="#tap2sna-py" title="Permalink to this headline">¶</a></h2>
@@ -1419,14 +1425,18 @@
 
 Convert a TAP or TZX file (which may be inside a zip archive) into a Z80
 snapshot. INPUT may be the full URL to a remote zip archive or TAP/TZX file,
 or the path to a local file. Arguments may be read from FILE instead of (or as
 well as) being given on the command line.
 
 Options:
+  -c name=value, --sim-load-config name=value
+                        Set the value of a --sim-load configuration parameter.
+                        Do &#39;-c help&#39; for more information. This option may be
+                        used multiple times.
   -d DIR, --output-dir DIR
                         Write the snapshot file in this directory.
   -f, --force           Overwrite an existing snapshot.
   -p STACK, --stack STACK
                         Set the stack pointer.
   --ram OPERATION       Perform a load operation or otherwise modify the
                         memory snapshot being built. Do &#39;--ram help&#39; for more
@@ -1435,50 +1445,37 @@
                         information. This option may be used multiple times.
   -s START, --start START
                         Set the start address to JP to.
   --sim-load            Simulate a 48K ZX Spectrum running LOAD &quot;&quot;.
   --state name=value    Set a hardware state attribute. Do &#39;--state help&#39; for
                         more information. This option may be used multiple
                         times.
+  --tape-name NAME      Specify the name of a TAP/TZX file in a zip archive.
+  --tape-start BLOCK    Start the tape at this block number.
+  --tape-stop BLOCK     Stop the tape at this block number.
+  --tape-sum MD5SUM     Specify the MD5 checksum of the TAP/TZX file.
   -u AGENT, --user-agent AGENT
                         Set the User-Agent header.
   -V, --version         Show SkoolKit version number and exit.
 </pre></div>
 </div>
-<p>Note that support for TZX files is limited to block types 0x10 (standard speed
-data), 0x11 (turbo speed data) and 0x14 (pure data).</p>
+<p>Note that <cite>tap2sna.py</cite> can read data from TZX block types 0x10 (standard speed
+data), 0x11 (turbo speed data) and 0x14 (pure data), but not block types 0x15
+(direct recording), 0x18 (CSW recording) or 0x19 (generalized data block).</p>
 <p>By default, <cite>tap2sna.py</cite> loads bytes from every data block on the tape, using
 the start address given in the corresponding header. For tapes that contain
 headerless data blocks, headers with incorrect start addresses, or irrelevant
 blocks, the <code class="docutils literal notranslate"><span class="pre">--ram</span></code> option can be used to load bytes from specific blocks at
 the appropriate addresses. For example:</p>
 <div class="highlight-none notranslate"><div class="highlight"><pre><span></span>$ tap2sna.py --ram load=3,30000 game.tzx game.z80
 </pre></div>
 </div>
 <p>loads the third block on the tape at address 30000, and ignores all other
 blocks. (To see information on the blocks in a TAP or TZX file, use the
 <a class="reference internal" href="#tapinfo-py"><span class="std std-ref">tapinfo.py</span></a> command.)</p>
-<p>An alternative to the <code class="docutils literal notranslate"><span class="pre">--ram</span> <span class="pre">load</span></code> approach is the <code class="docutils literal notranslate"><span class="pre">--sim-load</span></code> option. It
-simulates a freshly booted 48K ZX Spectrum running LOAD “” (or LOAD “”CODE, if
-the first block on the tape is a ‘Bytes’ header). Whenever the Spectrum ROM’s
-load routine at $0556 is called, a shortcut is taken by fast loading the next
-block on the tape. All other code (including any custom loader) is fully
-simulated. Simulation continues until the program counter hits the start
-address given by the <code class="docutils literal notranslate"><span class="pre">--start</span></code> option, or 10 minutes of simulated Z80 CPU
-time has elapsed, or the end of the tape is reached and one of the following
-conditions is satisfied:</p>
-<ul class="simple">
-<li><p>a custom loader was detected</p></li>
-<li><p>the program counter hits an address outside the ROM</p></li>
-<li><p>more than one second of simulated Z80 CPU time has elapsed since the end of
-the tape was reached</p></li>
-</ul>
-<p>The simulation can also be aborted by pressing Ctrl-C. When a simulated LOAD
-has completed or been aborted, the values of the registers (including the
-program counter) in the simulator are used to populate the Z80 snapshot.</p>
 <p>In addition to loading specific blocks, the <code class="docutils literal notranslate"><span class="pre">--ram</span></code> option can also be used
 to move blocks of bytes from one location to another, POKE values into
 individual addresses or address ranges, modify memory with XOR and ADD
 operations, initialise the system variables, or call a Python function to
 modify the memory snapshot in an arbitrary way before it is saved. For more
 information on these operations, run:</p>
 <div class="highlight-none notranslate"><div class="highlight"><pre><span></span>$ tap2sna.py --ram help
@@ -1503,58 +1500,138 @@
 </div>
 <p>then:</p>
 <div class="highlight-none notranslate"><div class="highlight"><pre><span></span>$ tap2sna.py @game.t2s
 </pre></div>
 </div>
 <p>will create <cite>game.z80</cite> as if the arguments specified in <cite>game.t2s</cite> had been
 given on the command line.</p>
+<div class="section" id="simulated-load">
+<h3>Simulated LOAD<a class="headerlink" href="#simulated-load" title="Permalink to this headline">¶</a></h3>
+<p>An alternative to the <code class="docutils literal notranslate"><span class="pre">--ram</span> <span class="pre">load</span></code> approach is the <code class="docutils literal notranslate"><span class="pre">--sim-load</span></code> option. It
+simulates a freshly booted 48K ZX Spectrum running LOAD “” (or LOAD “”CODE, if
+the first block on the tape is a ‘Bytes’ header). Whenever the Spectrum ROM’s
+load routine at $0556 is called, a shortcut is taken by “fast loading” the next
+block on the tape. All other code (including any custom loader) is fully
+simulated. Simulation continues until the program counter hits the start
+address given by the <code class="docutils literal notranslate"><span class="pre">--start</span></code> option, or 15 minutes of simulated Z80 CPU
+time has elapsed, or the end of the tape is reached and one of the following
+conditions is satisfied:</p>
+<ul class="simple">
+<li><p>a custom loader was detected</p></li>
+<li><p>the program counter hits an address outside the ROM</p></li>
+<li><p>more than one second of simulated Z80 CPU time has elapsed since the end of
+the tape was reached</p></li>
+</ul>
+<p>A simulated LOAD can also be aborted by pressing Ctrl-C. When a simulated LOAD
+has completed or been aborted, the values of the registers (including the
+program counter) in the simulator are used to populate the Z80 snapshot.</p>
+<p>A simulated LOAD can be configured via parameters that are set by the
+<code class="docutils literal notranslate"><span class="pre">--sim-load-config</span></code> (or <code class="docutils literal notranslate"><span class="pre">-c</span></code>) option. The recognised configuration
+parameters are:</p>
+<ul class="simple">
+<li><p><code class="docutils literal notranslate"><span class="pre">accelerator</span></code> - the tape-sampling loop accelerator to use (default:
+automatically selected - see below); use this to specify a particular
+accelerator (which may produce a faster simulated LOAD), or to disable
+acceleration entirely (<code class="docutils literal notranslate"><span class="pre">accelerator=none</span></code>)</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">fast-load</span></code> - enable fast loading (<code class="docutils literal notranslate"><span class="pre">1</span></code>, the default), or disable it
+(<code class="docutils literal notranslate"><span class="pre">0</span></code>); fast loading significantly reduces the load time for many tapes, but
+can also cause some loaders to fail</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">first-edge</span></code> - the time (in T-states) from the start of the tape at which
+to place the leading edge of the first pulse (default: <code class="docutils literal notranslate"><span class="pre">-2168</span></code>); the
+default value places the trailing edge of the first pulse at time 0, but some
+loaders (e.g. polarity-sensitive loaders) require <code class="docutils literal notranslate"><span class="pre">first-edge=0</span></code></p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">pause</span></code> - pause the tape between blocks and resume playback when port 254
+is read (<code class="docutils literal notranslate"><span class="pre">1</span></code>, the default), or run the tape continuously (<code class="docutils literal notranslate"><span class="pre">0</span></code>); pausing
+can help with tapes that require (but do not actually contain) long pauses
+between blocks, but can cause some loaders to fail</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">timeout</span></code> - the number of seconds of Z80 CPU time after which to abort the
+simulated LOAD if it’s still in progress (default: 900)</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">trace</span></code> - the file to which to log all instructions executed during the
+simulated LOAD (default: none)</p></li>
+</ul>
+<p>The names of the available tape-sampling loop accelerators are:</p>
+<ul class="simple">
+<li><p><code class="docutils literal notranslate"><span class="pre">alkatraz</span></code> (Alkatraz)</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">alkatraz2</span></code> (Alkatraz 2)</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">bleepload</span></code> (Firebird BleepLoad)</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">cyberlode</span></code> (Cyberlode 1.1)</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">digital-integration</span></code> (Digital Integration)</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">dinaload</span></code> (Dinaload)</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">edge</span></code> (Edge)</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">elite-uni-loader</span></code> (Elite Uni-Loader)</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">excelerator</span></code> (The Excelerator Loader)</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">flash-loader</span></code> (Flash Loader)</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">ftl</span></code> (FTL)</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">gargoyle</span></code> (Gargoyle)</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">gremlin</span></code> (various games published by Gremlin Graphics)</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">hewson-slowload</span></code> (Hewson Slowload)</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">injectaload</span></code> (Injectaload)</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">microsphere</span></code> (Back to Skool, Skool Daze, Sky Ranger)</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">none</span></code> (no accelerator)</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">paul-owens</span></code> (Paul Owens Protection System)</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">poliload</span></code> (Poliload)</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">power-load</span></code> (Power-Load)</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">rom</span></code> (any loader whose sampling loop is the same as the ROM’s)</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">search-loader</span></code> (Search Loader)</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">softlock</span></code> (SoftLock)</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">speedlock</span></code> (Speedlock - all versions)</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">zydroload</span></code> (Zydroload)</p></li>
+</ul>
 <table class="docutils colwidths-auto align-default">
 <thead>
 <tr class="row-odd"><th class="head"><p>Version</p></th>
 <th class="head"><p>Changes</p></th>
 </tr>
 </thead>
 <tbody>
-<tr class="row-even"><td><p>8.8</p></td>
+<tr class="row-even"><td><p>8.9</p></td>
+<td><p>Added the <code class="docutils literal notranslate"><span class="pre">--sim-load-config</span></code>, <code class="docutils literal notranslate"><span class="pre">--tape-name</span></code>,
+<code class="docutils literal notranslate"><span class="pre">--tape-start</span></code>, <code class="docutils literal notranslate"><span class="pre">--tape-stop</span></code> and <code class="docutils literal notranslate"><span class="pre">--tape-sum</span></code> options;
+added support for TZX loops, pauses, and unused bits in data
+blocks; added support for quoted arguments in an arguments file;
+added the <code class="docutils literal notranslate"><span class="pre">tstates</span></code> hardware state attribute</p></td>
+</tr>
+<tr class="row-odd"><td><p>8.8</p></td>
 <td><p>The <code class="docutils literal notranslate"><span class="pre">--sim-load</span></code> option performs any <code class="docutils literal notranslate"><span class="pre">call/move/poke/sysvars</span></code>
 operations specified by <code class="docutils literal notranslate"><span class="pre">--ram</span></code></p></td>
 </tr>
-<tr class="row-odd"><td><p>8.7</p></td>
+<tr class="row-even"><td><p>8.7</p></td>
 <td><p>Added the <code class="docutils literal notranslate"><span class="pre">--sim-load</span></code> option; when a headerless block is
 ignored because no <code class="docutils literal notranslate"><span class="pre">--ram</span> <span class="pre">load</span></code> options have been specified, a
 warning is printed</p></td>
 </tr>
-<tr class="row-even"><td><p>8.6</p></td>
+<tr class="row-odd"><td><p>8.6</p></td>
 <td><p>Added support to the <code class="docutils literal notranslate"><span class="pre">--ram</span></code> option for the <code class="docutils literal notranslate"><span class="pre">call</span></code> operation</p></td>
 </tr>
-<tr class="row-odd"><td><p>8.4</p></td>
+<tr class="row-even"><td><p>8.4</p></td>
 <td><p>Added support to the <code class="docutils literal notranslate"><span class="pre">--ram</span></code> option for the <code class="docutils literal notranslate"><span class="pre">sysvars</span></code>
 operation</p></td>
 </tr>
-<tr class="row-even"><td><p>6.3</p></td>
+<tr class="row-odd"><td><p>6.3</p></td>
 <td><p>Added the <code class="docutils literal notranslate"><span class="pre">--user-agent</span></code> option</p></td>
 </tr>
-<tr class="row-odd"><td><p>6.2</p></td>
+<tr class="row-even"><td><p>6.2</p></td>
 <td><p>The <code class="docutils literal notranslate"><span class="pre">--ram</span></code>, <code class="docutils literal notranslate"><span class="pre">--reg</span></code>, <code class="docutils literal notranslate"><span class="pre">--stack</span></code> and <code class="docutils literal notranslate"><span class="pre">--start</span></code> options
 accept hexadecimal integers prefixed by ‘0x’</p></td>
 </tr>
-<tr class="row-even"><td><p>5.3</p></td>
+<tr class="row-odd"><td><p>5.3</p></td>
 <td><p>Added the <code class="docutils literal notranslate"><span class="pre">--stack</span></code> and <code class="docutils literal notranslate"><span class="pre">--start</span></code> options</p></td>
 </tr>
-<tr class="row-odd"><td><p>4.5</p></td>
+<tr class="row-even"><td><p>4.5</p></td>
 <td><p>Added support for TZX block type 0x14 (pure data), for loading
 the first and last bytes of a tape block, and for modifying
 memory with XOR and ADD operations</p></td>
 </tr>
-<tr class="row-even"><td><p>3.5</p></td>
+<tr class="row-odd"><td><p>3.5</p></td>
 <td><p>New</p></td>
 </tr>
 </tbody>
 </table>
 </div>
+</div>
 <div class="section" id="tapinfo-py">
 <span id="id19"></span><h2>tapinfo.py<a class="headerlink" href="#tapinfo-py" title="Permalink to this headline">¶</a></h2>
 <p><cite>tapinfo.py</cite> shows information on the blocks in a TAP or TZX file. For
 example:</p>
 <div class="highlight-none notranslate"><div class="highlight"><pre><span></span>$ tapinfo.py game.tzx
 </pre></div>
 </div>
@@ -1578,33 +1655,36 @@
 <table class="docutils colwidths-auto align-default">
 <thead>
 <tr class="row-odd"><th class="head"><p>Version</p></th>
 <th class="head"><p>Changes</p></th>
 </tr>
 </thead>
 <tbody>
-<tr class="row-even"><td><p>8.3</p></td>
+<tr class="row-even"><td><p>8.9</p></td>
+<td><p>Shows full info for TZX block types 0x10 and 0x11</p></td>
+</tr>
+<tr class="row-odd"><td><p>8.3</p></td>
 <td><p>Added the <code class="docutils literal notranslate"><span class="pre">--data</span></code> option</p></td>
 </tr>
-<tr class="row-odd"><td><p>8.1</p></td>
+<tr class="row-even"><td><p>8.1</p></td>
 <td><p>Shows contents of TZX block types 0x33 (hardware type) and 0x35
 (custom info)</p></td>
 </tr>
-<tr class="row-even"><td><p>7.1</p></td>
+<tr class="row-odd"><td><p>7.1</p></td>
 <td><p>Shows pulse lengths in TZX block type 0x13 and full info for TZX
 block type 0x14</p></td>
 </tr>
-<tr class="row-odd"><td><p>6.2</p></td>
+<tr class="row-even"><td><p>6.2</p></td>
 <td><p>The <code class="docutils literal notranslate"><span class="pre">--basic</span></code> option accepts a hexadecimal address prefixed by
 ‘0x’</p></td>
 </tr>
-<tr class="row-even"><td><p>6.0</p></td>
+<tr class="row-odd"><td><p>6.0</p></td>
 <td><p>Added the <code class="docutils literal notranslate"><span class="pre">--basic</span></code> option</p></td>
 </tr>
-<tr class="row-odd"><td><p>5.0</p></td>
+<tr class="row-even"><td><p>5.0</p></td>
 <td><p>New</p></td>
 </tr>
 </tbody>
 </table>
 </div>
 <div class="section" id="trace-py">
 <span id="id20"></span><h2>trace.py<a class="headerlink" href="#trace-py" title="Permalink to this headline">¶</a></h2>
@@ -1620,14 +1700,15 @@
 SNA, SZX or Z80 snapshot, or &#39;.&#39; for no snapshot.
 
 Options:
   --audio               Show audio delays.
   --depth DEPTH         Simplify audio delays to this depth (default: 2).
   -D, --decimal         Show decimal values in verbose mode.
   --dump FILE           Dump a Z80 snapshot to this file after execution.
+  -i, --interrupts      Execute interrupt routines.
   --max-operations MAX  Maximum number of instructions to execute.
   --max-tstates MAX     Maximum number of T-states to run for.
   -o ADDR, --org ADDR   Specify the origin address of a binary (raw memory)
                         file (default: 65536 - length).
   -p a[-b[-c]],[^+]v, --poke a[-b[-c]],[^+]v
                         POKE N,v for N in {a, a+c, a+2c..., b}. Prefix &#39;v&#39;
                         with &#39;^&#39; to perform an XOR operation, or &#39;+&#39; to
@@ -1646,30 +1727,36 @@
                         register values too.
   -V, --version         Show SkoolKit version number and exit.
 </pre></div>
 </div>
 <p>By default, <cite>trace.py</cite> silently simulates code execution beginning with the
 instruction at the address specified by the <code class="docutils literal notranslate"><span class="pre">--start</span></code> option (or the program
 counter in the snapshot) and ending when the instruction at the address
-specified by <code class="docutils literal notranslate"><span class="pre">--stop</span></code> (if any) is reached. Use the <code class="docutils literal notranslate"><span class="pre">--verbose</span></code> option to
-show each instruction executed. Repeat the <code class="docutils literal notranslate"><span class="pre">--verbose</span></code> option (<code class="docutils literal notranslate"><span class="pre">-vv</span></code>) to
-show register values too.</p>
+specified by <code class="docutils literal notranslate"><span class="pre">--stop</span></code> (if any) is reached, and does not execute interrupt
+routines. Use the <code class="docutils literal notranslate"><span class="pre">--verbose</span></code> option to show each instruction executed.
+Repeat the <code class="docutils literal notranslate"><span class="pre">--verbose</span></code> option (<code class="docutils literal notranslate"><span class="pre">-vv</span></code>) to show register values too. Use the
+<code class="docutils literal notranslate"><span class="pre">--interrupts</span></code> option to enable the execution of interrupt routines.</p>
 <p>When the <code class="docutils literal notranslate"><span class="pre">--audio</span></code> option is given, <cite>trace.py</cite> tracks changes in the state
 of the ZX Spectrum speaker, and then prints a list of the delays (in T-states)
 between those changes. This list can be supplied to the <a class="reference internal" href="skool-macros.html#audio"><span class="std std-ref">#AUDIO</span></a> macro to
 produce a WAV file for the sound effect that would be produced by the same code
 running on a real ZX Spectrum.</p>
 <table class="docutils colwidths-auto align-default">
 <thead>
 <tr class="row-odd"><th class="head"><p>Version</p></th>
 <th class="head"><p>Changes</p></th>
 </tr>
 </thead>
 <tbody>
-<tr class="row-even"><td><p>8.8</p></td>
+<tr class="row-even"><td><p>8.9</p></td>
+<td><p>Added the <code class="docutils literal notranslate"><span class="pre">--interrupts</span></code> option; reads and writes the T-states
+counter in Z80 snapshots and reads the T-states counter in SZX
+snapshots</p></td>
+</tr>
+<tr class="row-odd"><td><p>8.8</p></td>
 <td><p>New</p></td>
 </tr>
 </tbody>
 </table>
 </div>
 </div>
 
@@ -1709,15 +1796,18 @@
 </li>
 <li><a class="reference internal" href="#snapinfo-py">snapinfo.py</a><ul>
 <li><a class="reference internal" href="#call-graphs">Call graphs</a></li>
 <li><a class="reference internal" href="#snapinfo-conf">Configuration</a></li>
 </ul>
 </li>
 <li><a class="reference internal" href="#snapmod-py">snapmod.py</a></li>
-<li><a class="reference internal" href="#tap2sna-py">tap2sna.py</a></li>
+<li><a class="reference internal" href="#tap2sna-py">tap2sna.py</a><ul>
+<li><a class="reference internal" href="#simulated-load">Simulated LOAD</a></li>
+</ul>
+</li>
 <li><a class="reference internal" href="#tapinfo-py">tapinfo.py</a></li>
 <li><a class="reference internal" href="#trace-py">trace.py</a></li>
 </ul>
 </li>
 </ul>
 
   <h4>Previous topic</h4>
@@ -1758,17 +1848,17 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="assemblers.html" title="Supported assemblers"
              >next</a> |</li>
         <li class="right" >
           <a href="diy.html" title="Disassembly DIY"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Commands</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Commands
 ****** CommandsÂ¶ ******
 ***** bin2sna.pyÂ¶ *****
 bin2sna.pyconverts a binary (raw memory) file into a Z80 snapshot. For example:
 $ bin2sna.py game.bin
 will create a file namedgame.z80. By default, the origin address (the address
 of the first byte of code or data), the start address (the first byte of code
@@ -49,14 +49,15 @@
                         ORG).
   -S name=value, --state name=value
                         Set a hardware state attribute. Do '--state help' for
                         more information. This option may be used multiple
                         times.
   -V, --version         Show SkoolKit version number and exit.
 Version Changes
+8.9     Added the tstates hardware state attribute
 6.3     Added the --poke option
 6.2     Added the --reg and --state options; the --org, --stack and --start
         options accept a hexadecimal integer prefixed by â0xâ
 5.2     New
 ***** bin2tap.pyÂ¶ *****
 bin2tap.pyconverts a binary (raw memory) file or a SNA, SZX or Z80 snapshot
 into a TAP file. For example:
@@ -910,14 +911,15 @@
                         information. This option may be used multiple times.
   -s name=value, --state name=value
                         Set a hardware state attribute. Do '--state help' for
                         more information. This option may be used multiple
                         times.
   -V, --version         Show SkoolKit version number and exit.
 Version Changes
+8.9     Added the tstates hardware state attribute
 6.2     The --move, --poke and --reg options accept hexadecimal integers
         prefixed by â0xâ
 5.3     New
 ***** tap2sna.pyÂ¶ *****
 tap2sna.pyconverts a TAP or TZX file (which may be inside a zip archive) into a
 Z80 snapshot. For example:
 $ tap2sna.py game.tap game.z80
@@ -928,14 +930,18 @@
 
 Convert a TAP or TZX file (which may be inside a zip archive) into a Z80
 snapshot. INPUT may be the full URL to a remote zip archive or TAP/TZX file,
 or the path to a local file. Arguments may be read from FILE instead of (or as
 well as) being given on the command line.
 
 Options:
+  -c name=value, --sim-load-config name=value
+                        Set the value of a --sim-load configuration parameter.
+                        Do '-c help' for more information. This option may be
+                        used multiple times.
   -d DIR, --output-dir DIR
                         Write the snapshot file in this directory.
   -f, --force           Overwrite an existing snapshot.
   -p STACK, --stack STACK
                         Set the stack pointer.
   --ram OPERATION       Perform a load operation or otherwise modify the
                         memory snapshot being built. Do '--ram help' for more
@@ -944,44 +950,33 @@
                         information. This option may be used multiple times.
   -s START, --start START
                         Set the start address to JP to.
   --sim-load            Simulate a 48K ZX Spectrum running LOAD "".
   --state name=value    Set a hardware state attribute. Do '--state help' for
                         more information. This option may be used multiple
                         times.
+  --tape-name NAME      Specify the name of a TAP/TZX file in a zip archive.
+  --tape-start BLOCK    Start the tape at this block number.
+  --tape-stop BLOCK     Stop the tape at this block number.
+  --tape-sum MD5SUM     Specify the MD5 checksum of the TAP/TZX file.
   -u AGENT, --user-agent AGENT
                         Set the User-Agent header.
   -V, --version         Show SkoolKit version number and exit.
-Note that support for TZX files is limited to block types 0x10 (standard speed
-data), 0x11 (turbo speed data) and 0x14 (pure data).
+Note thattap2sna.pycan read data from TZX block types 0x10 (standard speed
+data), 0x11 (turbo speed data) and 0x14 (pure data), but not block types 0x15
+(direct recording), 0x18 (CSW recording) or 0x19 (generalized data block).
 By default,tap2sna.pyloads bytes from every data block on the tape, using the
 start address given in the corresponding header. For tapes that contain
 headerless data blocks, headers with incorrect start addresses, or irrelevant
 blocks, the --ram option can be used to load bytes from specific blocks at the
 appropriate addresses. For example:
 $ tap2sna.py --ram load=3,30000 game.tzx game.z80
 loads the third block on the tape at address 30000, and ignores all other
 blocks. (To see information on the blocks in a TAP or TZX file, use the
 tapinfo.py command.)
-An alternative to the --ram load approach is the --sim-load option. It
-simulates a freshly booted 48K ZX Spectrum running LOAD ââ (or LOAD
-ââCODE, if the first block on the tape is a âBytesâ header). Whenever
-the Spectrum ROMâs load routine at $0556 is called, a shortcut is taken by
-fast loading the next block on the tape. All other code (including any custom
-loader) is fully simulated. Simulation continues until the program counter hits
-the start address given by the --start option, or 10 minutes of simulated Z80
-CPU time has elapsed, or the end of the tape is reached and one of the
-following conditions is satisfied:
-    * a custom loader was detected
-    * the program counter hits an address outside the ROM
-    * more than one second of simulated Z80 CPU time has elapsed since the end
-      of the tape was reached
-The simulation can also be aborted by pressing Ctrl-C. When a simulated LOAD
-has completed or been aborted, the values of the registers (including the
-program counter) in the simulator are used to populate the Z80 snapshot.
 In addition to loading specific blocks, the --ram option can also be used to
 move blocks of bytes from one location to another, POKE values into individual
 addresses or address ranges, modify memory with XOR and ADD operations,
 initialise the system variables, or call a Python function to modify the memory
 snapshot in an arbitrary way before it is saved. For more information on these
 operations, run:
 $ tap2sna.py --ram help
@@ -1000,15 +995,83 @@
 --state iff=0              # Disable interrupts
 --stack 32768              # Stack at 32768
 --start 34816              # Start at 34816
 then:
 $ tap2sna.py @game.t2s
 will creategame.z80as if the arguments specified ingame.t2shad been given on
 the command line.
+**** Simulated LOADÂ¶ ****
+An alternative to the --ram load approach is the --sim-load option. It
+simulates a freshly booted 48K ZX Spectrum running LOAD ââ (or LOAD
+ââCODE, if the first block on the tape is a âBytesâ header). Whenever
+the Spectrum ROMâs load routine at $0556 is called, a shortcut is taken by
+âfast loadingâ the next block on the tape. All other code (including any
+custom loader) is fully simulated. Simulation continues until the program
+counter hits the start address given by the --start option, or 15 minutes of
+simulated Z80 CPU time has elapsed, or the end of the tape is reached and one
+of the following conditions is satisfied:
+    * a custom loader was detected
+    * the program counter hits an address outside the ROM
+    * more than one second of simulated Z80 CPU time has elapsed since the end
+      of the tape was reached
+A simulated LOAD can also be aborted by pressing Ctrl-C. When a simulated LOAD
+has completed or been aborted, the values of the registers (including the
+program counter) in the simulator are used to populate the Z80 snapshot.
+A simulated LOAD can be configured via parameters that are set by the --sim-
+load-config (or -c) option. The recognised configuration parameters are:
+    * accelerator - the tape-sampling loop accelerator to use (default:
+      automatically selected - see below); use this to specify a particular
+      accelerator (which may produce a faster simulated LOAD), or to disable
+      acceleration entirely (accelerator=none)
+    * fast-load - enable fast loading (1, the default), or disable it (0); fast
+      loading significantly reduces the load time for many tapes, but can also
+      cause some loaders to fail
+    * first-edge - the time (in T-states) from the start of the tape at which
+      to place the leading edge of the first pulse (default: -2168); the
+      default value places the trailing edge of the first pulse at time 0, but
+      some loaders (e.g. polarity-sensitive loaders) require first-edge=0
+    * pause - pause the tape between blocks and resume playback when port 254
+      is read (1, the default), or run the tape continuously (0); pausing can
+      help with tapes that require (but do not actually contain) long pauses
+      between blocks, but can cause some loaders to fail
+    * timeout - the number of seconds of Z80 CPU time after which to abort the
+      simulated LOAD if itâs still in progress (default: 900)
+    * trace - the file to which to log all instructions executed during the
+      simulated LOAD (default: none)
+The names of the available tape-sampling loop accelerators are:
+    * alkatraz (Alkatraz)
+    * alkatraz2 (Alkatraz 2)
+    * bleepload (Firebird BleepLoad)
+    * cyberlode (Cyberlode 1.1)
+    * digital-integration (Digital Integration)
+    * dinaload (Dinaload)
+    * edge (Edge)
+    * elite-uni-loader (Elite Uni-Loader)
+    * excelerator (The Excelerator Loader)
+    * flash-loader (Flash Loader)
+    * ftl (FTL)
+    * gargoyle (Gargoyle)
+    * gremlin (various games published by Gremlin Graphics)
+    * hewson-slowload (Hewson Slowload)
+    * injectaload (Injectaload)
+    * microsphere (Back to Skool, Skool Daze, Sky Ranger)
+    * none (no accelerator)
+    * paul-owens (Paul Owens Protection System)
+    * poliload (Poliload)
+    * power-load (Power-Load)
+    * rom (any loader whose sampling loop is the same as the ROMâs)
+    * search-loader (Search Loader)
+    * softlock (SoftLock)
+    * speedlock (Speedlock - all versions)
+    * zydroload (Zydroload)
 Version Changes
+        Added the --sim-load-config, --tape-name, --tape-start, --tape-stop and
+8.9     --tape-sum options; added support for TZX loops, pauses, and unused
+        bits in data blocks; added support for quoted arguments in an arguments
+        file; added the tstates hardware state attribute
 8.8     The --sim-load option performs any call/move/poke/sysvars operations
         specified by --ram
 8.7     Added the --sim-load option; when a headerless block is ignored because
         no --ram load options have been specified, a warning is printed
 8.6     Added support to the --ram option for the call operation
 8.4     Added support to the --ram option for the sysvars operation
 6.3     Added the --user-agent option
@@ -1034,14 +1097,15 @@
                         10,11,2a.
   -B N[,A], --basic N[,A]
                         List the BASIC program in block N loaded at address A
                         (default 23755).
   -d, --data            Show the entire contents of header and data blocks.
   -V, --version         Show SkoolKit version number and exit.
 Version Changes
+8.9     Shows full info for TZX block types 0x10 and 0x11
 8.3     Added the --data option
 8.1     Shows contents of TZX block types 0x33 (hardware type) and 0x35 (custom
         info)
 7.1     Shows pulse lengths in TZX block type 0x13 and full info for TZX block
         type 0x14
 6.2     The --basic option accepts a hexadecimal address prefixed by â0xâ
 6.0     Added the --basic option
@@ -1057,14 +1121,15 @@
 SNA, SZX or Z80 snapshot, or '.' for no snapshot.
 
 Options:
   --audio               Show audio delays.
   --depth DEPTH         Simplify audio delays to this depth (default: 2).
   -D, --decimal         Show decimal values in verbose mode.
   --dump FILE           Dump a Z80 snapshot to this file after execution.
+  -i, --interrupts      Execute interrupt routines.
   --max-operations MAX  Maximum number of instructions to execute.
   --max-tstates MAX     Maximum number of T-states to run for.
   -o ADDR, --org ADDR   Specify the origin address of a binary (raw memory)
                         file (default: 65536 - length).
   -p a[-b[-c]],[^+]v, --poke a[-b[-c]],[^+]v
                         POKE N,v for N in {a, a+c, a+2c..., b}. Prefix 'v'
                         with '^' to perform an XOR operation, or '+' to
@@ -1081,23 +1146,26 @@
   --stats               Show stats after execution.
   -v, --verbose         Show executed instructions. Repeat this option to show
                         register values too.
   -V, --version         Show SkoolKit version number and exit.
 By default,trace.pysilently simulates code execution beginning with the
 instruction at the address specified by the --start option (or the program
 counter in the snapshot) and ending when the instruction at the address
-specified by --stop (if any) is reached. Use the --verbose option to show each
-instruction executed. Repeat the --verbose option (-vv) to show register values
-too.
+specified by --stop (if any) is reached, and does not execute interrupt
+routines. Use the --verbose option to show each instruction executed. Repeat
+the --verbose option (-vv) to show register values too. Use the --interrupts
+option to enable the execution of interrupt routines.
 When the --audio option is given,trace.pytracks changes in the state of the ZX
 Spectrum speaker, and then prints a list of the delays (in T-states) between
 those changes. This list can be supplied to the #AUDIO macro to produce a WAV
 file for the sound effect that would be produced by the same code running on a
 real ZX Spectrum.
 Version Changes
+8.9     Added the --interrupts option; reads and writes the T-states counter in
+        Z80 snapshots and reads the T-states counter in SZX snapshots
 8.8     New
 **** Table_of_Contents ****
     * Commands
           o bin2sna.py
           o bin2tap.py
           o skool2asm.py
                 # Configuration
@@ -1112,14 +1180,15 @@
           o sna2skool.py
                 # Configuration
           o snapinfo.py
                 # Call_graphs
                 # Configuration
           o snapmod.py
           o tap2sna.py
+                # Simulated_LOAD
           o tapinfo.py
           o trace.py
 *** Previous topic ***
 Disassembly_DIY
 *** Next topic ***
 Supported_assemblers
 **** This Page ****
@@ -1127,10 +1196,10 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Commands
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/components.html` & `skoolkit-8.9/docs/components.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>SkoolKit components &#8212; SkoolKit 8.8 documentation</title>
+    <title>SkoolKit components &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
@@ -27,15 +27,15 @@
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="extending.html" title="Extending SkoolKit"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">SkoolKit components</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -986,17 +986,17 @@
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="extending.html" title="Extending SkoolKit"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">SkoolKit components</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 **** Navigation ****
     * index
     * modules |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * SkoolKit components
 ****** SkoolKit componentsÂ¶ ******
 SkoolKit relies on several components in order to function:
     * Assembler
     * Control_directive_composer
     * Control_file_generator
     * Disassembler
@@ -481,10 +481,10 @@
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * SkoolKit components
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/control-files.html` & `skoolkit-8.9/docs/control-files.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Control files &#8212; SkoolKit 8.8 documentation</title>
+    <title>Control files &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
@@ -31,15 +31,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="skool-files.html" title="Skool files"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="parsing.html" title="Parsing, rendering, and modes"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Control files</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -1113,17 +1113,17 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="skool-files.html" title="Skool files"
              >next</a> |</li>
         <li class="right" >
           <a href="parsing.html" title="Parsing, rendering, and modes"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Control files</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Control files
 ****** Control filesÂ¶ ******
 A control file contains a list of start addresses of code and data blocks. This
 information can be used by sna2skool.py to organise a skool file into
 corresponding code and data blocks.
 Each block address in a control file is marked with a âcontrol directiveâ,
 which is a single letter that indicates what the block contains:
@@ -689,10 +689,10 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Control files
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/diy.html` & `skoolkit-8.9/docs/diy.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Disassembly DIY &#8212; SkoolKit 8.8 documentation</title>
+    <title>Disassembly DIY &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
@@ -31,15 +31,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="commands.html" title="Commands"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="usage.html" title="Installing and using SkoolKit"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Disassembly DIY</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -382,17 +382,17 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="commands.html" title="Commands"
              >next</a> |</li>
         <li class="right" >
           <a href="usage.html" title="Installing and using SkoolKit"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Disassembly DIY</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Disassembly DIY
 ****** Disassembly DIYÂ¶ ******
 The following sections describe how to use SkoolKit to get started on your own
 Spectrum game disassembly.
 ***** Getting startedÂ¶ *****
 The first thing to do is select a Spectrum game to disassemble. For the purpose
 of this discussion, weâll use Hungry_Horace. To build a pristine snapshot of
@@ -249,10 +249,10 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Disassembly DIY
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/extending.html` & `skoolkit-8.9/docs/extending.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Extending SkoolKit &#8212; SkoolKit 8.8 documentation</title>
+    <title>Extending SkoolKit &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
@@ -31,15 +31,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="components.html" title="SkoolKit components"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="html-templates.html" title="HTML templates"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Extending SkoolKit</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -987,17 +987,17 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="components.html" title="SkoolKit components"
              >next</a> |</li>
         <li class="right" >
           <a href="html-templates.html" title="HTML templates"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Extending SkoolKit</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

### Comparing `skoolkit-8.8/docs/genindex.html` & `skoolkit-8.9/docs/genindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Index &#8212; SkoolKit 8.8 documentation</title>
+    <title>Index &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
@@ -23,15 +23,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="#" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Index</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -371,17 +371,17 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="#" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Index</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Index
 ****** Index ******
 A | C | D | E | F | G | H | I | M | O | P | R | S | T | U | W
 ***** A *****
     * assemble()_                         * Assembler_(class_in_skoolkit.z80)
       (skoolkit.z80.Assembler_method)
 ***** C *****
@@ -110,10 +110,10 @@
 ***** W *****
     * write_image()_(skoolkit.image.ImageWriter_method)
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Index
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/html-templates.html` & `skoolkit-8.9/docs/html-templates.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>HTML templates &#8212; SkoolKit 8.8 documentation</title>
+    <title>HTML templates &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
@@ -31,15 +31,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="extending.html" title="Extending SkoolKit"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="asm-templates.html" title="ASM templates"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">HTML templates</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -864,17 +864,17 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="extending.html" title="Extending SkoolKit"
              >next</a> |</li>
         <li class="right" >
           <a href="asm-templates.html" title="ASM templates"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">HTML templates</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * HTML templates
 ****** HTML templatesÂ¶ ******
 Every page in an HTML disassembly is built from the Layout template and zero or
 more subtemplates defined by [Template:*] sections in the ref file.
 A template may contain âreplacement fieldsâ - identifiers enclosed by
 braces ({ and }) - that are replaced by appropriate content (typically derived
 from the skool file or a ref file section) when the template is formatted. The
@@ -472,10 +472,10 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * HTML templates
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/index.html` & `skoolkit-8.9/docs/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>SkoolKit manual &#8212; SkoolKit 8.8 documentation</title>
+    <title>SkoolKit manual &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
@@ -27,15 +27,15 @@
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="whatis.html" title="What is SkoolKit?"
              accesskey="N">next</a> |</li>
-        <li class="nav-item nav-item-0"><a href="#">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="#">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">SkoolKit manual</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -126,17 +126,17 @@
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="whatis.html" title="What is SkoolKit?"
              >next</a> |</li>
-        <li class="nav-item nav-item-0"><a href="#">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="#">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">SkoolKit manual</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * SkoolKit manual
 ****** SkoolKit manualÂ¶ ******
     * What_is_SkoolKit?
     * Installing_and_using_SkoolKit
     * Disassembly_DIY
     * Commands
     * Supported_assemblers
@@ -41,10 +41,10 @@
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * SkoolKit manual
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/man/bin2sna.py.html` & `skoolkit-8.9/docs/man/bin2sna.py.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>bin2sna.py &#8212; SkoolKit 8.8 documentation</title>
+    <title>bin2sna.py &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="../_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="../_static/custom.css" />
     
     <script id="documentation_options" data-url_root="../" src="../_static/documentation_options.js"></script>
     <script src="../_static/jquery.js"></script>
     <script src="../_static/underscore.js"></script>
@@ -23,15 +23,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">bin2sna.py</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -127,23 +127,24 @@
 <p>The <code class="docutils literal notranslate"><span class="pre">--state</span></code> option sets a hardware state attribute.</p>
 <div class="line-block">
 <div class="line"><br /></div>
 <div class="line-block">
 <div class="line"><code class="docutils literal notranslate"><span class="pre">--state</span> <span class="pre">name=value</span></code></div>
 </div>
 </div>
-<p>Recognised attribute names are:</p>
-<dl class="simple">
-<dt><code class="docutils literal notranslate"><span class="pre">border</span></code></dt><dd><p>border colour</p>
-</dd>
-<dt><code class="docutils literal notranslate"><span class="pre">iff</span></code></dt><dd><p>interrupt flip-flop: 0=disabled, 1=enabled</p>
-</dd>
-<dt><code class="docutils literal notranslate"><span class="pre">im</span></code></dt><dd><p>interrupt mode</p>
-</dd>
-</dl>
+<p>Recognised attribute names and their default values are:</p>
+<div class="line-block">
+<div class="line"><br /></div>
+<div class="line-block">
+<div class="line"><code class="docutils literal notranslate"><span class="pre">border</span></code>  - border colour (default=0)</div>
+<div class="line"><code class="docutils literal notranslate"><span class="pre">iff</span></code>     - interrupt flip-flop: 0=disabled, 1=enabled (default=1)</div>
+<div class="line"><code class="docutils literal notranslate"><span class="pre">im</span></code>      - interrupt mode (default=1)</div>
+<div class="line"><code class="docutils literal notranslate"><span class="pre">tstates</span></code> - T-states elapsed since start of frame (default=0)</div>
+</div>
+</div>
 </div>
 <div class="section" id="examples">
 <h2>EXAMPLES<a class="headerlink" href="#examples" title="Permalink to this headline">¶</a></h2>
 <ol class="arabic">
 <li><p>Convert <code class="docutils literal notranslate"><span class="pre">game.bin</span></code> into a Z80 snapshot named <code class="docutils literal notranslate"><span class="pre">game.z80</span></code>:</p>
 <div class="line-block">
 <div class="line"><br /></div>
@@ -211,17 +212,17 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">bin2sna.py</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * bin2sna.py
 ****** bin2sna.pyÂ¶ ******
 ***** SYNOPSISÂ¶ *****
 bin2sna.py [options] file.bin [file.z80]
 ***** DESCRIPTIONÂ¶ *****
 bin2sna.py converts a binary (raw memory) file into a Z80 snapshot.
 âfile.binâ may be a regular file, or â-â for standard input. If
@@ -66,21 +66,20 @@
 ^a, ^b, ^bc, ^c, ^d, ^de, ^e, ^f, ^h, ^hl, ^l,
 a, b, bc, c, d, de, e, f, h, hl, l,
 i, ix, iy, pc, r, sp
 ***** HARDWARE STATEÂ¶ *****
 The --state option sets a hardware state attribute.
 
 --state name=value
-Recognised attribute names are:
-  border
-      border colour
-  iff
-      interrupt flip-flop: 0=disabled, 1=enabled
-  im
-      interrupt mode
+Recognised attribute names and their default values are:
+
+border - border colour (default=0)
+iff - interrupt flip-flop: 0=disabled, 1=enabled (default=1)
+im - interrupt mode (default=1)
+tstates - T-states elapsed since start of frame (default=0)
 ***** EXAMPLESÂ¶ *****
    1. Convert game.bin into a Z80 snapshot named game.z80:
 
       bin2sna.py game.bin
    2. Convert ram.bin into a Z80 snapshot named game.z80 that starts execution
       at 32768:
 
@@ -96,10 +95,10 @@
 **** This Page ****
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * bin2sna.py
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/man/bin2tap.py.html` & `skoolkit-8.9/docs/man/bin2tap.py.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>bin2tap.py &#8212; SkoolKit 8.8 documentation</title>
+    <title>bin2tap.py &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="../_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="../_static/custom.css" />
     
     <script id="documentation_options" data-url_root="../" src="../_static/documentation_options.js"></script>
     <script src="../_static/jquery.js"></script>
     <script src="../_static/underscore.js"></script>
@@ -23,15 +23,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">bin2tap.py</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -170,17 +170,17 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">bin2tap.py</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * bin2tap.py
 ****** bin2tap.pyÂ¶ ******
 ***** SYNOPSISÂ¶ *****
 bin2tap.py [options] FILE [file.tap]
 ***** DESCRIPTIONÂ¶ *****
 bin2tap.py converts a binary (raw memory) file or a SNA, SZX or Z80 snapshot
 into a TAP file. FILE may be a regular file, or â-â to read a binary file
@@ -77,10 +77,10 @@
 **** This Page ****
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * bin2tap.py
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/man/skool2asm.py.html` & `skoolkit-8.9/docs/man/skool2asm.py.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>skool2asm.py &#8212; SkoolKit 8.8 documentation</title>
+    <title>skool2asm.py &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="../_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="../_static/custom.css" />
     
     <script id="documentation_options" data-url_root="../" src="../_static/documentation_options.js"></script>
     <script src="../_static/jquery.js"></script>
     <script src="../_static/underscore.js"></script>
@@ -23,15 +23,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">skool2asm.py</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -387,17 +387,17 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">skool2asm.py</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * skool2asm.py
 ****** skool2asm.pyÂ¶ ******
 ***** SYNOPSISÂ¶ *****
 skool2asm.py [options] FILE
 ***** DESCRIPTIONÂ¶ *****
 skool2asm.py converts a skool file into an ASM file that can be used by a Z80
 assembler. The ASM file is written to standard output. When FILE is â-â,
@@ -204,10 +204,10 @@
 **** This Page ****
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * skool2asm.py
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/man/skool2bin.py.html` & `skoolkit-8.9/docs/man/skool2bin.py.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>skool2bin.py &#8212; SkoolKit 8.8 documentation</title>
+    <title>skool2bin.py &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="../_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="../_static/custom.css" />
     
     <script id="documentation_options" data-url_root="../" src="../_static/documentation_options.js"></script>
     <script src="../_static/jquery.js"></script>
     <script src="../_static/underscore.js"></script>
@@ -23,15 +23,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">skool2bin.py</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -167,17 +167,17 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">skool2bin.py</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * skool2bin.py
 ****** skool2bin.pyÂ¶ ******
 ***** SYNOPSISÂ¶ *****
 skool2bin.py [options] file.skool [file.bin]
 ***** DESCRIPTIONÂ¶ *****
 skool2bin.py converts a skool file into a binary (raw memory) file.
 âfile.skoolâ may be a regular file, or â-â for standard input. If
@@ -62,10 +62,10 @@
 **** This Page ****
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * skool2bin.py
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/man/skool2ctl.py.html` & `skoolkit-8.9/docs/man/skool2ctl.py.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>skool2ctl.py &#8212; SkoolKit 8.8 documentation</title>
+    <title>skool2ctl.py &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="../_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="../_static/custom.css" />
     
     <script id="documentation_options" data-url_root="../" src="../_static/documentation_options.js"></script>
     <script src="../_static/jquery.js"></script>
     <script src="../_static/underscore.js"></script>
@@ -23,15 +23,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">skool2ctl.py</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -217,17 +217,17 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">skool2ctl.py</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * skool2ctl.py
 ****** skool2ctl.pyÂ¶ ******
 ***** SYNOPSISÂ¶ *****
 skool2ctl.py [options] FILE
 ***** DESCRIPTIONÂ¶ *****
 skool2ctl.py converts a skool file into a control file. The control file is
 written to stdout. When FILE is â-â, skool2ctl.py reads from standard
@@ -93,10 +93,10 @@
 **** This Page ****
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * skool2ctl.py
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/man/skool2html.py.html` & `skoolkit-8.9/docs/man/skool2html.py.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>skool2html.py &#8212; SkoolKit 8.8 documentation</title>
+    <title>skool2html.py &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="../_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="../_static/custom.css" />
     
     <script id="documentation_options" data-url_root="../" src="../_static/documentation_options.js"></script>
     <script src="../_static/jquery.js"></script>
     <script src="../_static/underscore.js"></script>
@@ -23,15 +23,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">skool2html.py</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -416,17 +416,17 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">skool2html.py</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * skool2html.py
 ****** skool2html.pyÂ¶ ******
 ***** SYNOPSISÂ¶ *****
 skool2html.py [options] SKOOLFILE [REFFILEâ¦]
 ***** DESCRIPTIONÂ¶ *****
 skool2html.py converts a skool file and ref files to HTML. When SKOOLFILE is
 â-â, skool2html.py reads from standard input.
@@ -213,10 +213,10 @@
 **** This Page ****
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * skool2html.py
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/man/sna2ctl.py.html` & `skoolkit-8.9/docs/man/sna2ctl.py.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>sna2ctl.py &#8212; SkoolKit 8.8 documentation</title>
+    <title>sna2ctl.py &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="../_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="../_static/custom.css" />
     
     <script id="documentation_options" data-url_root="../" src="../_static/documentation_options.js"></script>
     <script src="../_static/jquery.js"></script>
     <script src="../_static/underscore.js"></script>
@@ -23,15 +23,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">sna2ctl.py</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -212,17 +212,17 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">sna2ctl.py</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * sna2ctl.py
 ****** sna2ctl.pyÂ¶ ******
 ***** SYNOPSISÂ¶ *****
 sna2ctl.py [options] FILE
 ***** DESCRIPTIONÂ¶ *****
 sna2ctl.py generates a control file for a binary (raw memory) file or a SNA,
 SZX or Z80 snapshot. The control file is written to standard output. When FILE
@@ -93,10 +93,10 @@
 **** This Page ****
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * sna2ctl.py
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/man/sna2img.py.html` & `skoolkit-8.9/docs/man/sna2img.py.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>sna2img.py &#8212; SkoolKit 8.8 documentation</title>
+    <title>sna2img.py &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="../_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="../_static/custom.css" />
     
     <script id="documentation_options" data-url_root="../" src="../_static/documentation_options.js"></script>
     <script src="../_static/jquery.js"></script>
     <script src="../_static/underscore.js"></script>
@@ -23,15 +23,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">sna2img.py</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -183,17 +183,17 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">sna2img.py</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * sna2img.py
 ****** sna2img.pyÂ¶ ******
 ***** SYNOPSISÂ¶ *****
 sna2img.py [options] INPUT [OUTPUT]
 ***** DESCRIPTIONÂ¶ *****
 sna2img.py converts a Spectrum screenshot or other graphic data into a PNG
 file. INPUT may be a binary (raw memory) file, a SCR file, a skool file, or a
@@ -75,10 +75,10 @@
 **** This Page ****
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * sna2img.py
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/man/sna2skool.py.html` & `skoolkit-8.9/docs/man/sna2skool.py.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>sna2skool.py &#8212; SkoolKit 8.8 documentation</title>
+    <title>sna2skool.py &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="../_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="../_static/custom.css" />
     
     <script id="documentation_options" data-url_root="../" src="../_static/documentation_options.js"></script>
     <script src="../_static/jquery.js"></script>
     <script src="../_static/underscore.js"></script>
@@ -23,15 +23,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">sna2skool.py</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -316,17 +316,17 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">sna2skool.py</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * sna2skool.py
 ****** sna2skool.pyÂ¶ ******
 ***** SYNOPSISÂ¶ *****
 sna2kool.py [options] FILE
 ***** DESCRIPTIONÂ¶ *****
 sna2skool.py converts a binary (raw memory) file or a SNA, SZX or Z80 snapshot
 into a skool file. The skool file is written to standard output. When FILE is
@@ -170,10 +170,10 @@
 **** This Page ****
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * sna2skool.py
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/man/snapinfo.py.html` & `skoolkit-8.9/docs/man/snapinfo.py.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>snapinfo.py &#8212; SkoolKit 8.8 documentation</title>
+    <title>snapinfo.py &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="../_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="../_static/custom.css" />
     
     <script id="documentation_options" data-url_root="../" src="../_static/documentation_options.js"></script>
     <script src="../_static/jquery.js"></script>
     <script src="../_static/underscore.js"></script>
@@ -23,15 +23,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">snapinfo.py</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -235,17 +235,17 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">snapinfo.py</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * snapinfo.py
 ****** snapinfo.pyÂ¶ ******
 ***** SYNOPSISÂ¶ *****
 snapinfo.py [options] FILE
 ***** DESCRIPTIONÂ¶ *****
 snapinfo.py shows information on the registers or RAM in a binary (raw memory)
 file or a SNA, SZX or Z80 snapshot.
@@ -115,10 +115,10 @@
 **** This Page ****
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * snapinfo.py
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/man/snapmod.py.html` & `skoolkit-8.9/docs/man/snapmod.py.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>snapmod.py &#8212; SkoolKit 8.8 documentation</title>
+    <title>snapmod.py &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="../_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="../_static/custom.css" />
     
     <script id="documentation_options" data-url_root="../" src="../_static/documentation_options.js"></script>
     <script src="../_static/jquery.js"></script>
     <script src="../_static/underscore.js"></script>
@@ -23,15 +23,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">snapmod.py</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -117,37 +117,38 @@
 <p>The <code class="docutils literal notranslate"><span class="pre">--state</span></code> option sets a hardware state attribute.</p>
 <div class="line-block">
 <div class="line"><br /></div>
 <div class="line-block">
 <div class="line"><code class="docutils literal notranslate"><span class="pre">--state</span> <span class="pre">name=value</span></code></div>
 </div>
 </div>
-<p>Recognised attribute names are:</p>
-<dl class="simple">
-<dt><code class="docutils literal notranslate"><span class="pre">border</span></code></dt><dd><p>border colour</p>
-</dd>
-<dt><code class="docutils literal notranslate"><span class="pre">iff</span></code></dt><dd><p>interrupt flip-flop: 0=disabled, 1=enabled</p>
-</dd>
-<dt><code class="docutils literal notranslate"><span class="pre">im</span></code></dt><dd><p>interrupt mode</p>
-</dd>
-</dl>
+<p>Recognised attribute names and their default values are:</p>
+<div class="line-block">
+<div class="line"><br /></div>
+<div class="line-block">
+<div class="line"><code class="docutils literal notranslate"><span class="pre">border</span></code>  - border colour (default=0)</div>
+<div class="line"><code class="docutils literal notranslate"><span class="pre">iff</span></code>     - interrupt flip-flop: 0=disabled, 1=enabled (default=1)</div>
+<div class="line"><code class="docutils literal notranslate"><span class="pre">im</span></code>      - interrupt mode (default=1)</div>
+<div class="line"><code class="docutils literal notranslate"><span class="pre">tstates</span></code> - T-states elapsed since start of frame (default=0)</div>
+</div>
+</div>
 </div>
 <div class="section" id="examples">
 <h2>EXAMPLES<a class="headerlink" href="#examples" title="Permalink to this headline">¶</a></h2>
 <ol class="arabic">
-<li><p>Set the value of the HL register pair to 0 in game.z80:</p>
+<li><p>Set the value of the HL register pair to 0 in <code class="docutils literal notranslate"><span class="pre">game.z80</span></code>:</p>
 <div class="line-block">
 <div class="line"><br /></div>
 <div class="line-block">
 <div class="line"><code class="docutils literal notranslate"><span class="pre">snapmod.py</span> <span class="pre">-f</span> <span class="pre">-r</span> <span class="pre">hl=0</span> <span class="pre">game.z80</span></code></div>
 </div>
 </div>
 </li>
-<li><p>POKE the value 23 into address 32768 in game.z80, and write the resultant
-snapshot to poked.z80:</p>
+<li><p>POKE the value 23 into address 32768 in <code class="docutils literal notranslate"><span class="pre">game.z80</span></code>, and write the
+resultant snapshot to <code class="docutils literal notranslate"><span class="pre">poked.z80</span></code>:</p>
 <div class="line-block">
 <div class="line"><br /></div>
 <div class="line-block">
 <div class="line"><code class="docutils literal notranslate"><span class="pre">snapmod.py</span> <span class="pre">-p</span> <span class="pre">32768,23</span> <span class="pre">game.z80</span> <span class="pre">poked.z80</span></code></div>
 </div>
 </div>
 </li>
@@ -201,17 +202,17 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">snapmod.py</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * snapmod.py
 ****** snapmod.pyÂ¶ ******
 ***** SYNOPSISÂ¶ *****
 snapmod.py [options] in.z80 [out.z80]
 ***** DESCRIPTIONÂ¶ *****
 snapmod.py modifies the registers and RAM in a 48K Z80 snapshot.
 ***** OPTIONSÂ¶ *****
@@ -53,21 +53,20 @@
 ^a, ^b, ^bc, ^c, ^d, ^de, ^e, ^f, ^h, ^hl, ^l,
 a, b, bc, c, d, de, e, f, h, hl, l,
 i, ix, iy, pc, r, sp
 ***** HARDWARE STATEÂ¶ *****
 The --state option sets a hardware state attribute.
 
 --state name=value
-Recognised attribute names are:
-  border
-      border colour
-  iff
-      interrupt flip-flop: 0=disabled, 1=enabled
-  im
-      interrupt mode
+Recognised attribute names and their default values are:
+
+border - border colour (default=0)
+iff - interrupt flip-flop: 0=disabled, 1=enabled (default=1)
+im - interrupt mode (default=1)
+tstates - T-states elapsed since start of frame (default=0)
 ***** EXAMPLESÂ¶ *****
    1. Set the value of the HL register pair to 0 in game.z80:
 
       snapmod.py -f -r hl=0 game.z80
    2. POKE the value 23 into address 32768 in game.z80, and write the resultant
       snapshot to poked.z80:
 
@@ -83,10 +82,10 @@
 **** This Page ****
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * snapmod.py
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/man/tap2sna.py.html` & `skoolkit-8.9/docs/man/tap2sna.py.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>tap2sna.py &#8212; SkoolKit 8.8 documentation</title>
+    <title>tap2sna.py &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="../_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="../_static/custom.css" />
     
     <script id="documentation_options" data-url_root="../" src="../_static/documentation_options.js"></script>
     <script src="../_static/jquery.js"></script>
     <script src="../_static/underscore.js"></script>
@@ -23,15 +23,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">tap2sna.py</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -52,14 +52,18 @@
 into a Z80 snapshot. INPUT may be the full URL to a remote zip archive or
 TAP/TZX file, or the path to a local file. Arguments may be read from FILE
 instead of (or as well as) being given on the command line.</p>
 </div>
 <div class="section" id="options">
 <h2>OPTIONS<a class="headerlink" href="#options" title="Permalink to this headline">¶</a></h2>
 <dl class="simple">
+<dt>-c, –sim-load-config name=value</dt><dd><p>Set the value of a <code class="docutils literal notranslate"><span class="pre">--sim-load</span></code> configuration parameter. Do <code class="docutils literal notranslate"><span class="pre">-c</span> <span class="pre">help</span></code> for
+more information, and see the section on <code class="docutils literal notranslate"><span class="pre">SIMULATED</span> <span class="pre">LOAD</span></code> below. This
+option may be used multiple times.</p>
+</dd>
 <dt>-d, –output-dir <cite>DIR</cite></dt><dd><p>Write the snapshot file in this directory.</p>
 </dd>
 </dl>
 <dl class="option-list">
 <dt><kbd><span class="option">-f</span>, <span class="option">--force</span></kbd></dt>
 <dd><p>Overwrite an existing snapshot.</p>
 </dd>
@@ -93,42 +97,123 @@
 </dd>
 </dl>
 <dl class="simple">
 <dt>–state name=value</dt><dd><p>Set a hardware state attribute. Do <code class="docutils literal notranslate"><span class="pre">--state</span> <span class="pre">help</span></code> for more information, or
 see the section on <code class="docutils literal notranslate"><span class="pre">HARDWARE</span> <span class="pre">STATE</span></code> below. This option may be used multiple
 times.</p>
 </dd>
+</dl>
+<dl class="option-list">
+<dt><kbd><span class="option">--tape-name <var>NAME</var></span></kbd></dt>
+<dd><p>Specify the name of a TAP/TZX file in a zip archive. By default, the first
+TAP/TZX file found in the zip archive is selected.</p>
+</dd>
+<dt><kbd><span class="option">--tape-start <var>BLOCK</var></span></kbd></dt>
+<dd><p>Start the tape at this block number. In a TAP/TZX file, the first block is
+number 1, the second is 2, etc.</p>
+</dd>
+<dt><kbd><span class="option">--tape-stop <var>BLOCK</var></span></kbd></dt>
+<dd><p>Stop the tape at this block number. In a TAP/TZX file, the first block is
+number 1, the second is 2, etc.</p>
+</dd>
+<dt><kbd><span class="option">--tape-sum <var>MD5SUM</var></span></kbd></dt>
+<dd><p>Specify the MD5 checksum of the TAP/TZX file. <code class="docutils literal notranslate"><span class="pre">tap2sna.py</span></code> will abort if
+there is a checksum mismatch.</p>
+</dd>
+</dl>
+<dl class="simple">
 <dt>-u, –user-agent <cite>AGENT</cite></dt><dd><p>Set the User-Agent header used in an HTTP(S) request.</p>
 </dd>
 </dl>
 <dl class="option-list">
 <dt><kbd><span class="option">-V</span>, <span class="option">--version</span></kbd></dt>
 <dd><p>Show the SkoolKit version number and exit.</p>
 </dd>
 </dl>
 </div>
+<div class="section" id="tzx-support">
+<h2>TZX SUPPORT<a class="headerlink" href="#tzx-support" title="Permalink to this headline">¶</a></h2>
+<p><code class="docutils literal notranslate"><span class="pre">tap2sna.py</span></code> can read data from TZX block types 0x10 (standard speed data),
+0x11 (turbo speed data) and 0x14 (pure data), but not block types 0x15 (direct
+recording), 0x18 (CSW recording) or 0x19 (generalized data block).</p>
+</div>
 <div class="section" id="simulated-load">
 <h2>SIMULATED LOAD<a class="headerlink" href="#simulated-load" title="Permalink to this headline">¶</a></h2>
 <p>The <code class="docutils literal notranslate"><span class="pre">--sim-load</span></code> option simulates a freshly booted 48K ZX Spectrum running
 LOAD “” (or LOAD “”CODE, if the first block on the tape is a ‘Bytes’ header).
 Whenever the Spectrum ROM’s load routine at $0556 is called, a shortcut is
-taken by fast loading the next block on the tape. All other code (including any
-custom loader) is fully simulated. Simulation continues until the program
+taken by “fast loading” the next block on the tape. All other code (including
+any custom loader) is fully simulated. Simulation continues until the program
 counter hits the start address given by the <code class="docutils literal notranslate"><span class="pre">--start</span></code> option, or 10 minutes
 of simulated Z80 CPU time has elapsed, or the end of the tape is reached and
 one of the following conditions is satisfied:</p>
 <ul class="simple">
 <li><p>a custom loader was detected</p></li>
 <li><p>the program counter hits an address outside the ROM</p></li>
 <li><p>more than one second of simulated Z80 CPU time has elapsed since the end of
 the tape was reached</p></li>
 </ul>
-<p>The simulation can also be aborted by pressing Ctrl-C. When a simulated LOAD
+<p>A simulated LOAD can also be aborted by pressing Ctrl-C. When a simulated LOAD
 has completed or been aborted, the values of the registers (including the
 program counter) in the simulator are used to populate the Z80 snapshot.</p>
+<p>A simulated LOAD can be configured via parameters that are set by the
+by the <code class="docutils literal notranslate"><span class="pre">--sim-load-config</span></code> (or <code class="docutils literal notranslate"><span class="pre">-c</span></code>) option. The recognised configuration
+parameters are:</p>
+<ul class="simple">
+<li><p><code class="docutils literal notranslate"><span class="pre">accelerator</span></code> - the tape-sampling loop accelerator to use (default:
+automatically selected - see below); use this to specify a particular
+accelerator (which may produce a faster simulated LOAD), or to disable
+acceleration entirely (<code class="docutils literal notranslate"><span class="pre">accelerator=none</span></code>)</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">fast-load</span></code> - enable fast loading (<code class="docutils literal notranslate"><span class="pre">1</span></code>, the default), or disable it
+(<code class="docutils literal notranslate"><span class="pre">0</span></code>); fast loading significantly reduces the load time for many tapes, but
+can also cause some loaders to fail</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">first-edge</span></code> - the time (in T-states) from the start of the tape at which
+to place the leading edge of the first pulse (default: <code class="docutils literal notranslate"><span class="pre">-2168</span></code>); the
+default value places the trailing edge of the first pulse at time 0, but some
+loaders (e.g. polarity-sensitive loaders) require <code class="docutils literal notranslate"><span class="pre">first-edge=0</span></code></p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">pause</span></code> - pause the tape between blocks and resume playback when port 254
+is read (<code class="docutils literal notranslate"><span class="pre">1</span></code>, the default), or run the tape continuously (<code class="docutils literal notranslate"><span class="pre">0</span></code>); pausing
+can help with tapes that require (but do not actually contain) long pauses
+between blocks, but can cause some loaders to fail</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">timeout</span></code> - the number of seconds of Z80 CPU time after which to abort the
+simulated LOAD if it’s still in progress (default: 900)</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">trace</span></code> - the file to which to log all instructions executed during the
+simulated LOAD (default: none)</p></li>
+</ul>
+<p>The names of the available tape-sampling loop accelerators are:</p>
+<div class="line-block">
+<div class="line"><br /></div>
+<div class="line-block">
+<div class="line"><code class="docutils literal notranslate"><span class="pre">alkatraz</span></code> - Alkatraz</div>
+<div class="line"><code class="docutils literal notranslate"><span class="pre">alkatraz2</span></code> - Alkatraz 2</div>
+<div class="line"><code class="docutils literal notranslate"><span class="pre">bleepload</span></code> - Firebird BleepLoad</div>
+<div class="line"><code class="docutils literal notranslate"><span class="pre">cyberlode</span></code> - Cyberlode 1.1</div>
+<div class="line"><code class="docutils literal notranslate"><span class="pre">digital-integration</span></code> - Digital Integration</div>
+<div class="line"><code class="docutils literal notranslate"><span class="pre">dinaload</span></code> - Dinaload</div>
+<div class="line"><code class="docutils literal notranslate"><span class="pre">edge</span></code> - Edge</div>
+<div class="line"><code class="docutils literal notranslate"><span class="pre">elite-uni-loader</span></code> - Elite Uni-Loader</div>
+<div class="line"><code class="docutils literal notranslate"><span class="pre">excelerator</span></code> - The Excelerator Loader</div>
+<div class="line"><code class="docutils literal notranslate"><span class="pre">flash-loader</span></code> - Flash Loader</div>
+<div class="line"><code class="docutils literal notranslate"><span class="pre">ftl</span></code> - FTL</div>
+<div class="line"><code class="docutils literal notranslate"><span class="pre">gargoyle</span></code> - Gargoyle</div>
+<div class="line"><code class="docutils literal notranslate"><span class="pre">gremlin</span></code> - various games published by Gremlin Graphics</div>
+<div class="line"><code class="docutils literal notranslate"><span class="pre">hewson-slowload</span></code> - Hewson Slowload</div>
+<div class="line"><code class="docutils literal notranslate"><span class="pre">injectaload</span></code> - Injectaload</div>
+<div class="line"><code class="docutils literal notranslate"><span class="pre">microsphere</span></code> - Back to Skool, Skool Daze, Sky Ranger</div>
+<div class="line"><code class="docutils literal notranslate"><span class="pre">none</span></code> - no accelerator</div>
+<div class="line"><code class="docutils literal notranslate"><span class="pre">paul-owens</span></code> - Paul Owens Protection System</div>
+<div class="line"><code class="docutils literal notranslate"><span class="pre">poliload</span></code> - Poliload</div>
+<div class="line"><code class="docutils literal notranslate"><span class="pre">power-load</span></code> - Power-Load</div>
+<div class="line"><code class="docutils literal notranslate"><span class="pre">rom</span></code> - any loader whose sampling loop is the same as the ROM’s</div>
+<div class="line"><code class="docutils literal notranslate"><span class="pre">search-loader</span></code> - Search Loader</div>
+<div class="line"><code class="docutils literal notranslate"><span class="pre">softlock</span></code> - SoftLock</div>
+<div class="line"><code class="docutils literal notranslate"><span class="pre">speedlock</span></code> - Speedlock (all versions)</div>
+<div class="line"><code class="docutils literal notranslate"><span class="pre">zydroload</span></code> - Zydroload</div>
+</div>
+</div>
 </div>
 <div class="section" id="call-operations">
 <h2>CALL OPERATIONS<a class="headerlink" href="#call-operations" title="Permalink to this headline">¶</a></h2>
 <p>The <code class="docutils literal notranslate"><span class="pre">--ram</span></code> option can be used to call a Python function to perform arbitrary
 modification of the memory snapshot.</p>
 <div class="line-block">
 <div class="line"><br /></div>
@@ -297,22 +382,23 @@
 <div class="line-block">
 <div class="line"><br /></div>
 <div class="line-block">
 <div class="line"><code class="docutils literal notranslate"><span class="pre">--state</span> <span class="pre">name=value</span></code></div>
 </div>
 </div>
 <p>Recognised attribute names and their default values are:</p>
-<dl class="simple">
-<dt><code class="docutils literal notranslate"><span class="pre">border</span></code></dt><dd><p>border colour (default=0)</p>
-</dd>
-<dt><code class="docutils literal notranslate"><span class="pre">iff</span></code></dt><dd><p>interrupt flip-flop: 0=disabled, 1=enabled (default=1)</p>
-</dd>
-<dt><code class="docutils literal notranslate"><span class="pre">im</span></code></dt><dd><p>interrupt mode (default=1)</p>
-</dd>
-</dl>
+<div class="line-block">
+<div class="line"><br /></div>
+<div class="line-block">
+<div class="line"><code class="docutils literal notranslate"><span class="pre">border</span></code>  - border colour (default=0)</div>
+<div class="line"><code class="docutils literal notranslate"><span class="pre">iff</span></code>     - interrupt flip-flop: 0=disabled, 1=enabled (default=1)</div>
+<div class="line"><code class="docutils literal notranslate"><span class="pre">im</span></code>      - interrupt mode (default=1)</div>
+<div class="line"><code class="docutils literal notranslate"><span class="pre">tstates</span></code> - T-states elapsed since start of frame (default=0)</div>
+</div>
+</div>
 </div>
 <div class="section" id="reading-arguments-from-a-file">
 <h2>READING ARGUMENTS FROM A FILE<a class="headerlink" href="#reading-arguments-from-a-file" title="Permalink to this headline">¶</a></h2>
 <p>For complex snapshots that require many <code class="docutils literal notranslate"><span class="pre">--ram</span></code>, <code class="docutils literal notranslate"><span class="pre">--reg</span></code> or <code class="docutils literal notranslate"><span class="pre">--state</span></code>
 options to build, it may be more convenient to store the arguments to
 <code class="docutils literal notranslate"><span class="pre">tap2sna.py</span></code> in a file. For example, if the file <code class="docutils literal notranslate"><span class="pre">game.t2s</span></code> has the
 following contents:</p>
@@ -339,19 +425,14 @@
 <div class="line-block">
 <div class="line"><code class="docutils literal notranslate"><span class="pre">tap2sna.py</span> <span class="pre">&#64;game.t2s</span></code></div>
 </div>
 </div>
 <p>will create <code class="docutils literal notranslate"><span class="pre">game.z80</span></code> as if the arguments specified in <code class="docutils literal notranslate"><span class="pre">game.t2s</span></code> had been
 given on the command line.</p>
 </div>
-<div class="section" id="tzx-support">
-<h2>TZX SUPPORT<a class="headerlink" href="#tzx-support" title="Permalink to this headline">¶</a></h2>
-<p>Support for TZX files is limited to block types 0x10 (standard speed data),
-0x11 (turbo speed data) and 0x14 (pure data).</p>
-</div>
 <div class="section" id="examples">
 <h2>EXAMPLES<a class="headerlink" href="#examples" title="Permalink to this headline">¶</a></h2>
 <ol class="arabic">
 <li><p>Extract the TAP or TZX file from a remote zip archive and convert it into a
 Z80 snapshot:</p>
 <div class="line-block">
 <div class="line"><br /></div>
@@ -400,24 +481,24 @@
         <div class="sphinxsidebarwrapper">
   <h3><a href="../index.html">Table of Contents</a></h3>
   <ul>
 <li><a class="reference internal" href="#">tap2sna.py</a><ul>
 <li><a class="reference internal" href="#synopsis">SYNOPSIS</a></li>
 <li><a class="reference internal" href="#description">DESCRIPTION</a></li>
 <li><a class="reference internal" href="#options">OPTIONS</a></li>
+<li><a class="reference internal" href="#tzx-support">TZX SUPPORT</a></li>
 <li><a class="reference internal" href="#simulated-load">SIMULATED LOAD</a></li>
 <li><a class="reference internal" href="#call-operations">CALL OPERATIONS</a></li>
 <li><a class="reference internal" href="#load-operations">LOAD OPERATIONS</a></li>
 <li><a class="reference internal" href="#move-operations">MOVE OPERATIONS</a></li>
 <li><a class="reference internal" href="#poke-operations">POKE OPERATIONS</a></li>
 <li><a class="reference internal" href="#sysvars-operation">SYSVARS OPERATION</a></li>
 <li><a class="reference internal" href="#registers">REGISTERS</a></li>
 <li><a class="reference internal" href="#hardware-state">HARDWARE STATE</a></li>
 <li><a class="reference internal" href="#reading-arguments-from-a-file">READING ARGUMENTS FROM A FILE</a></li>
-<li><a class="reference internal" href="#tzx-support">TZX SUPPORT</a></li>
 <li><a class="reference internal" href="#examples">EXAMPLES</a></li>
 </ul>
 </li>
 </ul>
 
   <div role="note" aria-label="source link">
     <h3>This Page</h3>
@@ -445,17 +526,17 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">tap2sna.py</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,26 +3,30 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * tap2sna.py
 ****** tap2sna.pyÂ¶ ******
 ***** SYNOPSISÂ¶ *****
 tap2sna.py [options] INPUT snapshot.z80
 tap2sna.py @FILE [args]
 ***** DESCRIPTIONÂ¶ *****
 tap2sna.py converts a TAP or TZX file (which may be inside a zip archive) into
 a Z80 snapshot. INPUT may be the full URL to a remote zip archive or TAP/TZX
 file, or the path to a local file. Arguments may be read from FILE instead of
 (or as well as) being given on the command line.
 ***** OPTIONSÂ¶ *****
+  -c, âsim-load-config name=value
+      Set the value of a --sim-load configuration parameter. Do -c help for
+      more information, and see the section on SIMULATED LOAD below. This
+      option may be used multiple times.
   -d, âoutput-dirDIR
       Write the snapshot file in this directory.
   -f, --force
       Overwrite an existing snapshot.
   -p, âstackSTACK
       Set the stack pointer. This option is equivalent to --reg
       sp=STACK.STACKmust be a decimal number, or a hexadecimal number prefixed
@@ -42,34 +46,98 @@
   --sim-load
       Simulate a 48K ZX Spectrum running LOAD ââ. See the section on
       SIMULATED LOAD below.
   âstate name=value
       Set a hardware state attribute. Do --state help for more information, or
       see the section on HARDWARE STATE below. This option may be used multiple
       times.
+  --tape-name NAME
+      Specify the name of a TAP/TZX file in a zip archive. By default, the
+      first TAP/TZX file found in the zip archive is selected.
+  --tape-start BLOCK
+      Start the tape at this block number. In a TAP/TZX file, the first block
+      is number 1, the second is 2, etc.
+  --tape-stop BLOCK
+      Stop the tape at this block number. In a TAP/TZX file, the first block is
+      number 1, the second is 2, etc.
+  --tape-sum MD5SUM
+      Specify the MD5 checksum of the TAP/TZX file. tap2sna.py will abort if
+      there is a checksum mismatch.
   -u, âuser-agentAGENT
       Set the User-Agent header used in an HTTP(S) request.
   -V, --version
       Show the SkoolKit version number and exit.
+***** TZX SUPPORTÂ¶ *****
+tap2sna.py can read data from TZX block types 0x10 (standard speed data), 0x11
+(turbo speed data) and 0x14 (pure data), but not block types 0x15 (direct
+recording), 0x18 (CSW recording) or 0x19 (generalized data block).
 ***** SIMULATED LOADÂ¶ *****
 The --sim-load option simulates a freshly booted 48K ZX Spectrum running LOAD
 ââ (or LOAD ââCODE, if the first block on the tape is a âBytesâ
 header). Whenever the Spectrum ROMâs load routine at $0556 is called, a
-shortcut is taken by fast loading the next block on the tape. All other code
-(including any custom loader) is fully simulated. Simulation continues until
-the program counter hits the start address given by the --start option, or 10
-minutes of simulated Z80 CPU time has elapsed, or the end of the tape is
+shortcut is taken by âfast loadingâ the next block on the tape. All other
+code (including any custom loader) is fully simulated. Simulation continues
+until the program counter hits the start address given by the --start option,
+or 10 minutes of simulated Z80 CPU time has elapsed, or the end of the tape is
 reached and one of the following conditions is satisfied:
     * a custom loader was detected
     * the program counter hits an address outside the ROM
     * more than one second of simulated Z80 CPU time has elapsed since the end
       of the tape was reached
-The simulation can also be aborted by pressing Ctrl-C. When a simulated LOAD
+A simulated LOAD can also be aborted by pressing Ctrl-C. When a simulated LOAD
 has completed or been aborted, the values of the registers (including the
 program counter) in the simulator are used to populate the Z80 snapshot.
+A simulated LOAD can be configured via parameters that are set by the by the --
+sim-load-config (or -c) option. The recognised configuration parameters are:
+    * accelerator - the tape-sampling loop accelerator to use (default:
+      automatically selected - see below); use this to specify a particular
+      accelerator (which may produce a faster simulated LOAD), or to disable
+      acceleration entirely (accelerator=none)
+    * fast-load - enable fast loading (1, the default), or disable it (0); fast
+      loading significantly reduces the load time for many tapes, but can also
+      cause some loaders to fail
+    * first-edge - the time (in T-states) from the start of the tape at which
+      to place the leading edge of the first pulse (default: -2168); the
+      default value places the trailing edge of the first pulse at time 0, but
+      some loaders (e.g. polarity-sensitive loaders) require first-edge=0
+    * pause - pause the tape between blocks and resume playback when port 254
+      is read (1, the default), or run the tape continuously (0); pausing can
+      help with tapes that require (but do not actually contain) long pauses
+      between blocks, but can cause some loaders to fail
+    * timeout - the number of seconds of Z80 CPU time after which to abort the
+      simulated LOAD if itâs still in progress (default: 900)
+    * trace - the file to which to log all instructions executed during the
+      simulated LOAD (default: none)
+The names of the available tape-sampling loop accelerators are:
+
+alkatraz - Alkatraz
+alkatraz2 - Alkatraz 2
+bleepload - Firebird BleepLoad
+cyberlode - Cyberlode 1.1
+digital-integration - Digital Integration
+dinaload - Dinaload
+edge - Edge
+elite-uni-loader - Elite Uni-Loader
+excelerator - The Excelerator Loader
+flash-loader - Flash Loader
+ftl - FTL
+gargoyle - Gargoyle
+gremlin - various games published by Gremlin Graphics
+hewson-slowload - Hewson Slowload
+injectaload - Injectaload
+microsphere - Back to Skool, Skool Daze, Sky Ranger
+none - no accelerator
+paul-owens - Paul Owens Protection System
+poliload - Poliload
+power-load - Power-Load
+rom - any loader whose sampling loop is the same as the ROMâs
+search-loader - Search Loader
+softlock - SoftLock
+speedlock - Speedlock (all versions)
+zydroload - Zydroload
 ***** CALL OPERATIONSÂ¶ *****
 The --ram option can be used to call a Python function to perform arbitrary
 modification of the memory snapshot.
 
 --ram call=[/path/to/moduledir:]module.function
 The function is called with the memory snapshot (a list of 65536 byte values)
 as the sole positional argument. The function must modify the snapshot in
@@ -163,20 +231,19 @@
 i=63
 iy=23610
 ***** HARDWARE STATEÂ¶ *****
 The --state option sets a hardware state attribute.
 
 --state name=value
 Recognised attribute names and their default values are:
-  border
-      border colour (default=0)
-  iff
-      interrupt flip-flop: 0=disabled, 1=enabled (default=1)
-  im
-      interrupt mode (default=1)
+
+border - border colour (default=0)
+iff - interrupt flip-flop: 0=disabled, 1=enabled (default=1)
+im - interrupt mode (default=1)
+tstates - T-states elapsed since start of frame (default=0)
 ***** READING ARGUMENTS FROM A FILEÂ¶ *****
 For complex snapshots that require many --ram, --reg or --state options to
 build, it may be more convenient to store the arguments to tap2sna.py in a
 file. For example, if the file game.t2s has the following contents:
 
 ;
 ; tap2sna.py file for GAME
@@ -191,17 +258,14 @@
 âstack 32768 # Stack at 32768
 âstart 34816 # Start at 34816
 then:
 
 tap2sna.py @game.t2s
 will create game.z80 as if the arguments specified in game.t2s had been given
 on the command line.
-***** TZX SUPPORTÂ¶ *****
-Support for TZX files is limited to block types 0x10 (standard speed data),
-0x11 (turbo speed data) and 0x14 (pure data).
 ***** EXAMPLESÂ¶ *****
    1. Extract the TAP or TZX file from a remote zip archive and convert it into
       a Z80 snapshot:
 
       tap2sna.py ftp://example.com/game.zip game.z80
    2. Extract the TAP or TZX file from a zip archive, and convert it into a Z80
       snapshot with the program counter set to 32768:
@@ -216,28 +280,28 @@
 
       tap2sna.py @game.t2s game.tzx game.z80
 **** Table_of_Contents ****
     * tap2sna.py
           o SYNOPSIS
           o DESCRIPTION
           o OPTIONS
+          o TZX_SUPPORT
           o SIMULATED_LOAD
           o CALL_OPERATIONS
           o LOAD_OPERATIONS
           o MOVE_OPERATIONS
           o POKE_OPERATIONS
           o SYSVARS_OPERATION
           o REGISTERS
           o HARDWARE_STATE
           o READING_ARGUMENTS_FROM_A_FILE
-          o TZX_SUPPORT
           o EXAMPLES
 **** This Page ****
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * tap2sna.py
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/man/tapinfo.py.html` & `skoolkit-8.9/docs/man/tapinfo.py.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>tapinfo.py &#8212; SkoolKit 8.8 documentation</title>
+    <title>tapinfo.py &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="../_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="../_static/custom.css" />
     
     <script id="documentation_options" data-url_root="../" src="../_static/documentation_options.js"></script>
     <script src="../_static/jquery.js"></script>
     <script src="../_static/underscore.js"></script>
@@ -23,15 +23,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">tapinfo.py</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -135,17 +135,17 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">tapinfo.py</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * tapinfo.py
 ****** tapinfo.pyÂ¶ ******
 ***** SYNOPSISÂ¶ *****
 tapinfo.py [options] FILE
 ***** DESCRIPTIONÂ¶ *****
 tapinfo.py shows information on the blocks in a TAP or TZX file.
 ***** OPTIONSÂ¶ *****
@@ -43,10 +43,10 @@
 **** This Page ****
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * tapinfo.py
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/man/trace.py.html` & `skoolkit-8.9/docs/man/trace.py.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>trace.py &#8212; SkoolKit 8.8 documentation</title>
+    <title>trace.py &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="../_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="../_static/custom.css" />
     
     <script id="documentation_options" data-url_root="../" src="../_static/documentation_options.js"></script>
     <script src="../_static/jquery.js"></script>
     <script src="../_static/underscore.js"></script>
@@ -23,15 +23,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">trace.py</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -68,14 +68,21 @@
 <dt><kbd><span class="option">-D</span>, <span class="option">--decimal</span></kbd></dt>
 <dd><p>Show decimal values in verbose (<code class="docutils literal notranslate"><span class="pre">-v</span></code>, <code class="docutils literal notranslate"><span class="pre">-vv</span></code>) mode.</p>
 </dd>
 </dl>
 <dl class="simple">
 <dt>–dump <cite>FILE</cite></dt><dd><p>Dump a Z80 snapshot to this file after execution.</p>
 </dd>
+</dl>
+<dl class="option-list">
+<dt><kbd><span class="option">-i</span>, <span class="option">--interrupts</span></kbd></dt>
+<dd><p>Execute interrupt routines.</p>
+</dd>
+</dl>
+<dl class="simple">
 <dt>–max-operations <cite>MAX</cite></dt><dd><p>Maximum number of instructions to execute. Overrides the <cite>STOP</cite> address (if
 given).</p>
 </dd>
 <dt>–max-tstates <cite>MAX</cite></dt><dd><p>Maximum number of (simulated) T-states to run for. Overrides the <cite>STOP</cite>
 address (if given).</p>
 </dd>
 <dt>-o, –org <cite>ORG</cite></dt><dd><p>Specify the origin address of a binary (raw memory) file. The default origin
@@ -219,17 +226,17 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">trace.py</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * trace.py
 ****** trace.pyÂ¶ ******
 ***** SYNOPSISÂ¶ *****
 trace.py [options] FILE
 ***** DESCRIPTIONÂ¶ *****
 trace.py simulates the execution of machine code in a 48K binary (raw memory)
 file or a SNA, SZX or Z80 snapshot. If FILE is â.â, no snapshot is loaded,
@@ -25,14 +25,16 @@
       given, any sequence of delays up to lengthNthat repeats is shown in a
       simplified form. For example, ifNis 3, the run of delay values [1, 2, 3,
       1, 2, 3] is reduced to [1, 2, 3]*2.
   -D, --decimal
       Show decimal values in verbose (-v, -vv) mode.
   âdumpFILE
       Dump a Z80 snapshot to this file after execution.
+  -i, --interrupts
+      Execute interrupt routines.
   âmax-operationsMAX
       Maximum number of instructions to execute. Overrides theSTOPaddress (if
       given).
   âmax-tstatesMAX
       Maximum number of (simulated) T-states to run for. Overrides
       theSTOPaddress (if given).
   -o, âorgORG
@@ -102,10 +104,10 @@
 **** This Page ****
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * trace.py
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/migration.html` & `skoolkit-8.9/docs/migration.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Migrating from SkoolKit 7 &#8212; SkoolKit 8.8 documentation</title>
+    <title>Migrating from SkoolKit 7 &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
@@ -31,15 +31,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="changelog.html" title="Changelog"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="assemblers.html" title="Supported assemblers"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Migrating from SkoolKit 7</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -339,17 +339,17 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="changelog.html" title="Changelog"
              >next</a> |</li>
         <li class="right" >
           <a href="assemblers.html" title="Supported assemblers"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Migrating from SkoolKit 7</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Migrating from SkoolKit 7
 ****** Migrating from SkoolKit 7Â¶ ******
 SkoolKit 8 includes some changes that make it incompatible with SkoolKit 7. If
 you have developed a disassembly using SkoolKit 7 and find that the SkoolKit
 commands no longer work with your source files, or produce broken output, look
 through the following sections for tips on how to migrate your disassembly to
 SkoolKit 8.
@@ -155,10 +155,10 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Migrating from SkoolKit 7
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/parsing.html` & `skoolkit-8.9/docs/parsing.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Parsing, rendering, and modes &#8212; SkoolKit 8.8 documentation</title>
+    <title>Parsing, rendering, and modes &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
@@ -31,15 +31,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="control-files.html" title="Control files"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="changelog1.html" title="SkoolKit 1.x changelog"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Parsing, rendering, and modes</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -197,17 +197,17 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="control-files.html" title="Control files"
              >next</a> |</li>
         <li class="right" >
           <a href="changelog1.html" title="SkoolKit 1.x changelog"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Parsing, rendering, and modes</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Parsing, rendering, and modes
 ****** Parsing, rendering, and modesÂ¶ ******
 The following subsections explain at a high level the two phases involved in
 transforming a skool file (and its related ref files, if any exist) into HTML
 or ASM format by using skool2html.py or skool2asm.py: parsing and rendering.
 ***** ParsingÂ¶ *****
 In the first phase, the skool file is parsed. Parsing a skool file entails
@@ -98,10 +98,10 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Parsing, rendering, and modes
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/py-modindex.html` & `skoolkit-8.9/docs/py-modindex.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Python Module Index &#8212; SkoolKit 8.8 documentation</title>
+    <title>Python Module Index &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
@@ -26,15 +26,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="#" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Python Module Index</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -105,17 +105,17 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="#" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Python Module Index</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Python Module Index
 ****** Python Module Index ******
 s
      
     s
 [-] skoolkit
         skoolkit.components
@@ -19,10 +19,10 @@
         skoolkit.snapshot
         skoolkit.snaskool
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Python Module Index
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/ref-files.html` & `skoolkit-8.9/docs/ref-files.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Ref files &#8212; SkoolKit 8.8 documentation</title>
+    <title>Ref files &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
@@ -31,15 +31,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="asm.html" title="ASM modes and directives"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="skool-macros.html" title="Skool macros"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Ref files</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -1390,17 +1390,17 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="asm.html" title="ASM modes and directives"
              >next</a> |</li>
         <li class="right" >
           <a href="skool-macros.html" title="Skool macros"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Ref files</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Ref files
 ****** Ref filesÂ¶ ******
 If you want to configure or augment an HTML disassembly, you will need one or
 more ref files. A ref file can be used to (for example):
     * add a âBugsâ page on which bugs are documented
     * add a âTriviaâ page on which interesting facts are documented
     * add a âPokesâ page on which useful POKEs are listed
@@ -831,10 +831,10 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Ref files
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/search.html` & `skoolkit-8.9/docs/search.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Search &#8212; SkoolKit 8.8 documentation</title>
+    <title>Search &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
@@ -29,15 +29,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Search</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -80,17 +80,17 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Search</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,19 +3,19 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Search
 ****** Search ******
 Please activate JavaScript to enable the search functionality.
 Searching for multiple words only shows matches that contain all words.
 [q                   ] [search]
 **** Navigation ****
     * index
     * modules |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Search
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/searchindex.js` & `skoolkit-8.9/docs/searchindex.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -155,29 +155,36 @@
         "0123456789": 36,
         "02x": [11, 16, 27],
         "04x": [10, 11, 27, 34, 36],
         "0556": [11, 29],
         "08b": [11, 27],
         "0x000f": 36,
         "0x0556": [11, 19],
-        "0x10": [11, 29, 30],
+        "0x10": [3, 11, 29, 30],
         "0x100": 29,
-        "0x11": [11, 29, 30],
+        "0x11": [3, 11, 29, 30],
         "0x13": [10, 11],
-        "0x14": [7, 10, 11, 29],
+        "0x14": [3, 7, 10, 11, 29],
+        "0x15": [11, 29],
+        "0x18": [11, 29],
+        "0x19": [11, 29],
         "0x1f": [18, 28, 29, 31],
+        "0x20": 3,
+        "0x24": 3,
+        "0x25": 3,
         "0x33": [3, 11],
         "0x35": [3, 11],
         "0x3d00": 0,
         "0x400e": [11, 19],
         "0x5d90": [11, 19],
         "0x6000": 29,
         "0x9c00": 29,
         "0x9d00": 29,
         "0xc000": 29,
+        "0xed": 3,
         "100": [9, 13, 14, 36],
         "1000": 36,
         "10000": 6,
         "10000001": 13,
         "10001111": 13,
         "10072": [18, 28, 29, 31],
         "100th": [15, 36],
@@ -213,14 +220,15 @@
         "194": 0,
         "197": 34,
         "198": 34,
         "200": [0, 36],
         "2018": [13, 35],
         "2048": 29,
         "205": 34,
+        "2168": [11, 29],
         "22528": [0, 15, 36],
         "23296": 14,
         "23552": [29, 36],
         "23610": [29, 36],
         "237": 9,
         "23754": 29,
         "23755": [11, 30],
@@ -246,15 +254,15 @@
         "25000": 29,
         "25087": 13,
         "25088": 13,
         "25167": 14,
         "25343": 13,
         "25344": 13,
         "25396": 0,
-        "254": [34, 36],
+        "254": [11, 29, 34, 36],
         "25404": 0,
         "255": [0, 15, 34, 36],
         "25560": 0,
         "256": [0, 9, 29, 36],
         "25820": 36,
         "26429": 14,
         "26572": 36,
@@ -429,33 +437,33 @@
         "6912": [11, 19],
         "69888": 34,
         "800": 36,
         "8000": 9,
         "8192": 11,
         "8593": 36,
         "8x8": [5, 15, 36],
-        "900": 36,
+        "900": [11, 29, 36],
         "942": 34,
         "9c40": 11,
         "9c41": 11,
         "9c43": 11,
         "9c44": 11,
         "9c46": 11,
         "boolean": 36,
         "break": [10, 11, 13, 14, 22],
         "byte": [0, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 15, 16, 19, 25, 26, 27, 28, 29, 32, 34, 35, 36, 38],
         "case": [0, 1, 2, 3, 5, 6, 7, 9, 10, 11, 12, 13, 16, 20, 22, 23, 24, 26, 33, 34, 36],
         "char": [11, 27, 36],
         "class": [0, 3, 6, 7, 11, 12, 15, 16, 20, 23, 32, 34, 36],
-        "default": [0, 1, 2, 3, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 29, 30, 31, 32, 34, 35, 36],
+        "default": [0, 1, 2, 3, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 34, 35, 36],
         "final": [5, 9, 13, 32, 34, 35, 36],
         "float": 3,
         "function": [3, 11, 12, 15, 29],
         "import": [3, 13, 15, 34, 35],
-        "long": [0, 6, 11, 13, 15, 34, 35, 36],
+        "long": [0, 6, 11, 13, 15, 29, 34, 35, 36],
         "new": [0, 3, 7, 10, 11, 14, 15, 16, 32, 34, 36],
         "public": [4, 38],
         "return": [11, 12, 14, 15, 19, 36],
         "short": [11, 34],
         "static": [4, 14, 24, 38],
         "switch": [0, 36],
         "true": [0, 11, 12, 15, 16, 36],
@@ -487,28 +495,29 @@
         a001: 0,
         abbrevi: 13,
         abcd: 34,
         abil: [0, 3, 5, 7, 8, 9, 10, 11, 12, 34, 35, 36],
         abort: [11, 29],
         about: [0, 7, 20, 36],
         abov: [0, 4, 11, 13, 34, 35, 36, 37],
+        acceler: [3, 11, 29],
         accept: [0, 3, 6, 8, 9, 11, 12, 15, 36],
         access: [0, 12, 16, 36],
         accid: 14,
         accompani: [14, 35],
         accord: [4, 11, 13, 15, 16, 26, 36],
         accordingli: [5, 6, 14, 32],
         accumul: [0, 13, 36],
         accur: [6, 14, 36],
         accuraci: 10,
         achiev: [13, 32],
         across: 4,
         act: 9,
         action: [0, 15],
-        actual: [0, 12, 16, 36],
+        actual: [0, 11, 12, 16, 29, 36],
         adc: 4,
         add: [0, 4, 6, 7, 10, 11, 13, 14, 15, 18, 19, 20, 22, 23, 24, 25, 26, 27, 28, 29, 31, 34, 36, 38],
         added: [0, 11, 13, 14, 15, 29, 34, 35, 36, 37],
         adding: [6, 8, 10, 13, 14, 15, 34],
         addit: [0, 4, 5, 9, 11, 13, 14, 15, 16, 32, 34, 35, 36],
         addition: 12,
         addr1: [0, 13, 34],
@@ -526,25 +535,27 @@
         affix: [3, 36],
         after: [0, 2, 5, 7, 10, 11, 12, 13, 15, 20, 29, 31, 33, 34, 35, 36],
         again: 14,
         agent: [9, 11, 29],
         algorithm: 10,
         alic: 16,
         align: [1, 9, 16, 36],
+        alkatraz2: [11, 29],
+        alkatraz: [11, 29],
         all: [0, 1, 3, 5, 8, 10, 11, 13, 14, 15, 22, 23, 29, 31, 33, 34, 35, 36],
         allevi: 36,
         allow: [10, 11, 12, 24, 36],
         alon: [7, 11, 19, 23, 34, 36],
         along: [3, 5, 10, 11, 12, 32, 33, 34, 38],
         alongsid: [6, 11, 13, 14, 16, 23, 34],
         alpha: [3, 15, 34, 36],
         alphabet: 12,
         alphanumer: [11, 24, 36],
         alreadi: [3, 14, 29, 34, 36, 37],
-        also: [0, 1, 11, 12, 13, 14, 15, 16, 20, 22, 23, 24, 26, 27, 29, 32, 34, 35, 36, 38],
+        also: [0, 1, 3, 11, 12, 13, 14, 15, 16, 20, 22, 23, 24, 26, 27, 29, 32, 34, 35, 36, 38],
         alt: [7, 15, 16, 36],
         altern: [0, 3, 10, 11, 12, 13, 14, 15, 16, 18, 28, 29, 31, 34, 36],
         although: 0,
         alwai: [6, 7, 11, 13, 26, 32, 33, 36, 38],
         amen: 0,
         amend: 3,
         amount: 36,
@@ -569,15 +580,15 @@
         append: [0, 8, 10, 11, 13, 15, 20, 35, 36],
         appli: [0, 3, 6, 7, 9, 11, 12, 13, 15, 16, 20, 21, 35, 36],
         applic: 0,
         approach: [11, 14],
         appropri: [1, 11, 12, 14, 15, 16, 19, 29, 32, 33, 36],
         approxim: 36,
         arbitrari: [0, 3, 6, 8, 11, 15, 16, 29, 34, 35, 36, 38],
-        archiv: [11, 14, 29, 37],
+        archiv: [3, 11, 14, 29, 37],
         area: [8, 27],
         arg: [3, 12, 29, 36],
         argument: [3, 5, 7, 9, 10, 11, 12, 13, 15, 36, 37],
         arithmet: [0, 8, 9, 11, 15, 36],
         around: [0, 3, 11, 12, 26, 36],
         arrai: [3, 7, 8, 15, 36],
         arrang: 36,
@@ -614,23 +625,23 @@
         attrs2: 36,
         audio4: 36,
         audio: [0, 3, 11, 23, 31, 34, 38],
         audioformat: [3, 34, 36],
         audiopath: [3, 34, 36],
         audiowrit: [3, 36],
         augment: 34,
-        automat: [0, 5, 9, 10, 15, 34],
-        avail: [0, 1, 3, 5, 9, 11, 12, 16, 32, 34, 36, 37],
+        automat: [0, 5, 9, 10, 11, 15, 29, 34],
+        avail: [0, 1, 3, 5, 9, 11, 12, 16, 29, 32, 34, 36, 37],
         avoid: 36,
         awar: 15,
         b31995: 13,
         b50000: 35,
         b50002: 35,
         b50003: 35,
-        back: [4, 5, 11, 14, 38],
+        back: [4, 5, 11, 14, 29, 38],
         background: [11, 15, 27, 34, 36],
         backslash: [6, 35],
         bar31: 0,
         bar: 0,
         bare: [11, 12, 19],
         base: [0, 3, 6, 7, 9, 10, 11, 12, 20, 22, 23, 26, 32, 34, 36],
         base_sprit: 36,
@@ -652,26 +663,27 @@
         being: [0, 3, 6, 7, 8, 9, 11, 12, 15, 16, 20, 24, 29, 33, 34, 35, 36, 37],
         belong: [13, 34],
         below: [0, 2, 3, 6, 11, 15, 16, 18, 23, 28, 29, 31, 34, 36, 37],
         benefit: 14,
         besid: [13, 14],
         best: 14,
         better: [14, 15, 36, 38],
-        between: [0, 1, 9, 11, 13, 15, 16, 27, 31, 33, 34, 35, 36, 38],
+        between: [0, 1, 3, 9, 11, 13, 15, 16, 27, 29, 31, 33, 34, 35, 36, 38],
         bfix: [5, 8, 9, 10, 11, 13, 20, 21, 25, 33, 36],
         bfmt: 16,
         bgcolor: [11, 27],
-        bin2sna: [2, 8, 9, 38],
+        bin2sna: [2, 3, 8, 9, 38],
         bin2tap: [2, 3, 4, 5, 7, 8, 38],
         bin: [2, 11, 18, 19, 21, 26, 27, 37],
         binari: [2, 3, 5, 6, 8, 9, 11, 12, 13, 18, 19, 21, 22, 24, 25, 26, 27, 31, 35, 36],
-        bit: [0, 7, 10, 13, 25, 36],
+        bit: [0, 3, 7, 10, 11, 13, 25, 36],
         bitwis: 36,
         black: [34, 36],
         blank: [0, 5, 6, 8, 9, 11, 13, 15, 16, 20, 31, 34, 35, 36],
+        bleepload: [11, 29],
         block: [1, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 14, 16, 19, 20, 22, 23, 24, 25, 26, 28, 29, 30, 32, 33, 34, 36, 38],
         block_com: 16,
         blue: [34, 36],
         bmask: 0,
         bob: 16,
         bodi: [13, 34, 36],
         bold: 35,
@@ -730,26 +742,27 @@
         candid: 36,
         cannot: [0, 12, 13, 32, 33, 34, 36],
         capabl: [6, 36, 38],
         capit: 36,
         care: [13, 14, 16, 35, 36],
         carefulli: 14,
         carol: 16,
-        caus: [3, 4, 14, 34],
+        caus: [3, 4, 11, 14, 29, 34],
         cdc6cd: 34,
         cell: [0, 3, 5, 6, 9, 10, 11, 13, 16, 20, 25, 34, 36],
         cent: 13,
         centr: 36,
         central: 36,
         certain: [15, 32, 34, 35, 36],
         chain: 0,
         chang: [0, 1, 3, 4, 5, 11, 12, 13, 15, 16, 31, 32, 34, 35, 36, 37],
         changelog: [14, 16, 17, 34],
         charact: [0, 2, 3, 6, 7, 9, 10, 11, 12, 13, 15, 16, 20, 22, 24, 26, 34, 36],
         check: [0, 13],
+        checksum: [3, 11, 29],
         choic: 14,
         choke: 5,
         choos: 37,
         chosen: [2, 14, 36],
         chr127: 36,
         chr169: 36,
         chr: [0, 3, 6],
@@ -800,16 +813,16 @@
         compress: [7, 8, 34, 36],
         compris: 16,
         comput: [10, 12, 15, 36],
         concaten: [6, 11, 23, 36],
         concern: 0,
         condit: [3, 11, 29, 36],
         condition: [0, 9, 16],
-        config: [0, 3, 6, 8, 9, 10, 11, 12, 14, 15, 20, 22, 23, 24, 26, 27, 36],
-        configur: [0, 1, 3, 6, 9, 10, 12, 14, 32, 34, 36],
+        config: [0, 3, 6, 8, 9, 10, 11, 12, 14, 15, 20, 22, 23, 24, 26, 27, 29, 36],
+        configur: [0, 1, 3, 6, 9, 10, 12, 14, 29, 32, 34, 36],
         connect: [5, 11],
         consid: [13, 36],
         consist: [0, 12, 13, 34, 36],
         constant: 2,
         constitut: 36,
         construct: [0, 3, 12, 36],
         constructor: 12,
@@ -844,56 +857,59 @@
         correct: [0, 4, 11, 19, 35, 36],
         correctli: [5, 6, 9, 13, 35],
         correspond: [5, 10, 11, 12, 13, 14, 15, 16, 29, 33, 36],
         correspondingli: 5,
         corrupt: 6,
         could: [10, 13, 14, 15, 16, 32, 36],
         count: [13, 36],
-        counter: [11, 29, 31, 36],
+        counter: [3, 11, 29, 31, 36],
         cover: [0, 9, 10, 13],
         cpu: [4, 11, 29],
         craft: 35,
         crash: [6, 11, 19],
         creat: [0, 3, 5, 6, 7, 8, 9, 11, 14, 15, 16, 20, 23, 29, 32, 33, 34, 36, 38],
         createlabel: [11, 20, 23],
         creation: [6, 8, 34, 36],
         crlf: [0, 20],
         crop: [3, 6, 9, 11, 25],
         crop_rect: 15,
         cross: [3, 4],
         cruis: [4, 5, 38],
         csc: [4, 5],
         css: [6, 11, 14, 16, 23, 34, 36],
+        csw: [11, 29],
         ctl: [3, 4, 6, 7, 10, 11, 12, 14, 22, 24, 26, 27],
         ctrl: [11, 29],
         cumbersom: 36,
         current: [0, 3, 9, 10, 11, 12, 15, 16, 20, 22, 23, 24, 26, 27, 36, 37],
         custom: [1, 3, 5, 8, 10, 11, 14, 15, 16, 20, 29, 34],
         customis: [14, 15],
         cwd: 15,
         cyan: [11, 27, 34, 36],
+        cyberlod: [11, 29],
         cycl: 34,
         d27126: 36,
         daddr: 36,
         danger: 14,
         dangl: 9,
         dark: [6, 11, 14, 23],
         dash: 36,
         data: [0, 3, 4, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 19, 20, 21, 23, 24, 25, 26, 27, 29, 30, 33, 34, 35, 36, 38],
         datamap: 34,
         datat: 6,
-        daze: [4, 5, 11, 38],
+        daze: [4, 5, 11, 29, 38],
         ddcb: 4,
         deal: [0, 12],
         death: 14,
         dec: [0, 14, 36],
         decent: 14,
         decid: [0, 12],
         decim: [0, 5, 6, 7, 8, 9, 11, 12, 13, 14, 15, 16, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 34, 36],
         declar: [0, 5, 7, 11, 12, 13, 14, 34, 35, 36],
+        decompress: 3,
         decreas: 5,
         decrement: 14,
         deep: 15,
         def1: 36,
         def2: 36,
         def: [3, 5, 6, 7, 9, 10, 11, 12, 13, 15, 16, 21, 22, 33],
         defaultanimationformat: [8, 32],
@@ -942,19 +958,20 @@
         devic: 2,
         df_addr: 15,
         dict: 15,
         dictionari: [3, 9, 10, 11, 12, 15, 16, 24, 34, 36],
         did: [6, 32],
         differ: [3, 5, 13, 15, 33, 36],
         difficult: 14,
-        digit: [11, 16, 24, 34, 35, 36],
+        digit: [11, 16, 24, 29, 34, 35, 36],
         dii: 17,
         dimension: 15,
+        dinaload: [11, 29],
         dir: [6, 11, 20, 23, 29],
-        direct: [1, 3, 5, 6, 7, 8, 9, 10, 11, 14, 15, 17, 20, 21, 22, 23, 33, 34, 36],
+        direct: [1, 3, 5, 6, 7, 8, 9, 10, 11, 14, 15, 17, 20, 21, 22, 23, 29, 33, 34, 36],
         directli: [0, 36],
         directori: [3, 5, 6, 7, 9, 11, 12, 14, 15, 20, 22, 23, 24, 26, 27, 29, 34, 36, 37],
         disabl: [11, 18, 28, 29, 36],
         disassembl: [0, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 13, 15, 16, 17, 20, 23, 26, 32, 33, 34, 35, 36, 38],
         disassemblytablenumcol: [10, 34],
         discard: 33,
         discov: 38,
@@ -980,35 +997,36 @@
         down: 36,
         download: 5,
         draw: 14,
         drawn: 36,
         drop: [3, 6, 8, 9],
         dump: [11, 31],
         durat: 36,
-        dure: [0, 3, 33, 36],
+        dure: [0, 3, 11, 29, 33, 36],
         dwidth: 36,
         dymond: 38,
         each: [0, 1, 2, 3, 4, 5, 7, 10, 11, 12, 13, 14, 15, 16, 18, 20, 21, 25, 27, 28, 29, 31, 33, 34, 35, 36, 38],
         earlier: 3,
         easier: [8, 9, 13, 14, 36],
         easili: [14, 15, 34],
         ed0101010101: 7,
         ed63: 4,
         ed6b: 4,
         ed72: 4,
         ed7a: 4,
-        edg: [0, 11, 27, 36],
+        edg: [0, 3, 11, 27, 29, 36],
         edgeattribut: [11, 27],
         edit: 14,
         effect: [0, 7, 11, 14, 16, 31, 32, 33, 34, 36, 38],
         eight: [0, 36],
         either: [0, 1, 9, 12, 13, 14, 15, 31, 33, 34, 35, 36, 38],
-        elaps: [4, 11, 29, 36],
+        elaps: [4, 11, 18, 28, 29, 36],
         element: [3, 7, 8, 11, 12, 13, 15, 16, 22, 32, 34, 36],
         elig: [11, 12, 24],
+        elit: [11, 29],
         els: [0, 13, 14, 15, 16, 33],
         elsewher: [34, 36],
         empti: [0, 1, 3, 6, 9, 12, 13, 15, 16, 20, 34, 35, 36],
         emul: [2, 6, 11, 14, 24, 38],
         enabl: [0, 3, 6, 8, 11, 18, 19, 28, 29, 34, 36, 38],
         enclos: [1, 12, 15, 16, 36],
         encod: [3, 6, 13, 36],
@@ -1018,15 +1036,15 @@
         endfor: 16,
         endgam: 0,
         endif: 16,
         enhanc: [5, 6],
         ensur: [0, 14, 16, 34, 35],
         entail: 33,
         enter: 37,
-        entir: [0, 3, 7, 10, 11, 13, 15, 16, 20, 23, 30, 36],
+        entir: [0, 3, 7, 10, 11, 13, 15, 16, 20, 23, 29, 30, 36],
         entireti: 0,
         entri: [0, 1, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 14, 15, 16, 26, 32, 34, 36],
         entrydescript: [7, 34],
         entrygroup: 3,
         entrylabel: [3, 11, 20, 23],
         entrypointlabel: [3, 11, 20, 23],
         entrypointref: [11, 26],
@@ -1054,18 +1072,19 @@
         ever: 14,
         everi: [0, 6, 7, 9, 10, 11, 12, 13, 16, 29, 34, 36],
         everyth: [0, 13, 14, 16, 34],
         exact: [9, 36],
         exactli: [0, 11, 20, 26, 34, 36, 37],
         examin: 14,
         exampl: [0, 1, 2, 4, 6, 7, 11, 12, 13, 14, 15, 16, 32, 33, 34, 35, 36],
+        exceler: [11, 29],
         except: [13, 14, 29, 34, 36],
         exclud: 16,
         exclus: 34,
-        execut: [0, 3, 6, 8, 11, 14, 15, 18, 19, 24, 31, 36, 38],
+        execut: [0, 3, 6, 8, 11, 14, 15, 18, 19, 24, 29, 31, 36, 38],
         exercis: 14,
         exist: [0, 3, 5, 10, 11, 14, 15, 16, 23, 28, 29, 32, 33, 34, 36],
         exit: [0, 11, 13, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31],
         expand: [3, 8, 9, 10, 11, 20, 25, 33, 34, 35, 36],
         expand_invers: 15,
         expand_macronam: 15,
         expand_sprit: 15,
@@ -1085,20 +1104,21 @@
         extract: [15, 29],
         extran: 7,
         extrem: 14,
         face: 6,
         facilit: 12,
         fact: [5, 13, 14, 34, 38],
         factor: 36,
-        fail: [6, 14],
+        fail: [6, 11, 14, 29],
         fall: 36,
         fals: [0, 3, 12, 15, 16, 36],
         familiar: 14,
         far: [11, 13, 14],
-        fast: [11, 29],
+        fast: [3, 11, 29],
+        faster: [11, 29],
         faulti: 0,
         fdcb: 4,
         fed: 11,
         fedora: 37,
         ff0000: 34,
         ff00: 34,
         ff00ff: 34,
@@ -1106,23 +1126,24 @@
         ffff: 12,
         ffffff: 34,
         field: [0, 1, 3, 4, 5, 9, 10, 11, 12, 14, 16, 20, 23, 26, 27, 32, 34, 35],
         figur: 14,
         file: [0, 1, 3, 4, 5, 6, 7, 8, 9, 10, 11, 16, 17, 18, 19, 20, 21, 22, 24, 25, 26, 27, 30, 31, 33, 36, 38],
         filenam: [7, 8, 11, 12, 15, 16, 25, 34],
         fill: 36,
-        find: [9, 11, 14, 15, 27, 32, 34, 38],
+        find: [3, 9, 11, 14, 15, 27, 32, 34, 38],
         finish: [14, 38],
-        first: [0, 2, 5, 7, 8, 10, 11, 12, 13, 14, 15, 16, 20, 23, 27, 29, 33, 34, 35, 36],
+        firebird: [11, 29],
+        first: [0, 2, 3, 5, 7, 8, 10, 11, 12, 13, 14, 15, 16, 20, 23, 27, 29, 33, 34, 35, 36],
         fit: [14, 35],
         five: [0, 7, 13],
         fix: [0, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 20, 36],
         flac: [34, 36],
         flag: [3, 7, 10, 29, 36],
-        flash: [8, 9, 11, 25, 34],
+        flash: [8, 9, 11, 25, 29, 34],
         flatten: 36,
         flexibl: [0, 15],
         flip: [0, 3, 5, 11, 15, 18, 25, 28, 29, 36],
         flip_udg: [7, 15],
         flop: [18, 28, 29],
         fmt: [3, 16],
         fname: [9, 12, 15, 34, 36],
@@ -1145,43 +1166,45 @@
         form: [0, 2, 12, 13, 14, 15, 16, 31, 34, 36],
         format0: 36,
         format: [1, 2, 3, 6, 7, 8, 9, 10, 11, 12, 13, 14, 16, 20, 22, 23, 26, 27, 33, 34, 38],
         format_byt: 12,
         format_templ: [12, 15, 32],
         format_word: 12,
         forstart: 36,
-        found: [11, 14, 15, 20, 22, 23, 24, 26, 27, 33, 34, 36, 38],
+        found: [11, 14, 15, 20, 22, 23, 24, 26, 27, 29, 33, 34, 36, 38],
         foundat: 38,
         four: [11, 13, 19, 35, 36],
         fourth: [11, 29],
         frame1: 36,
         frame2: 36,
-        frame: [3, 6, 7, 12, 15, 34, 36],
+        frame: [3, 6, 7, 12, 15, 18, 28, 29, 34, 36],
         framedur: 34,
         free: 38,
         freshli: [11, 29],
         friendli: 38,
         from: [0, 1, 3, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 22, 23, 24, 25, 26, 27, 28, 31, 34, 35, 36, 37, 38],
         fsep: 36,
+        ftl: [11, 29],
         ftp: 29,
-        full: [0, 10, 11, 14, 16, 29, 36, 38],
+        full: [0, 3, 10, 11, 14, 16, 29, 36, 38],
         fulli: [11, 14, 29, 34],
         further: 11,
         fuse: [6, 11, 14, 24],
         gain: 0,
         game8: 32,
         game: [0, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 13, 14, 15, 16, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 35, 36, 38],
         gameasmwrit: 15,
         gamedir: [14, 34],
         gamehtmlwrit: 15,
         gameindex: [3, 16, 32, 34],
         gamestatusbuff: [34, 36],
         gap: 36,
+        gargoyl: [11, 29],
         gbuffer: 34,
-        gener: [0, 2, 3, 4, 5, 6, 7, 9, 10, 11, 15, 24, 26, 27, 34, 35, 38],
+        gener: [0, 2, 3, 4, 5, 6, 7, 9, 10, 11, 15, 24, 26, 27, 29, 34, 35, 38],
         generate_ctl: 12,
         get: [15, 35, 36, 37],
         get_compon: 12,
         get_dictionari: 15,
         get_sect: 15,
         get_siz: 12,
         get_snapshot: 12,
@@ -1200,20 +1223,21 @@
         gnu: 38,
         goe: 14,
         going: [14, 15],
         good: [14, 16],
         grab: 14,
         graph: [0, 3, 12, 27, 38],
         graphattribut: [11, 27],
-        graphic: [5, 6, 9, 11, 25, 27, 34, 36, 38],
+        graphic: [5, 6, 9, 11, 25, 27, 29, 34, 36, 38],
         graphicglitch: 34,
         graphviz: 11,
         great: 13,
         greater: [35, 36],
         green: [6, 14, 34, 36],
+        gremlin: [11, 29],
         grid: 35,
         group: [0, 3, 5, 6, 13, 16, 32, 34, 36],
         groupid: 34,
         had: [11, 14, 29],
         half: 2,
         handi: 14,
         handl: [0, 1, 3, 5, 6, 7, 8, 9, 10, 20],
@@ -1233,14 +1257,15 @@
         height: [11, 15, 25, 36],
         held: 38,
         hell: 13,
         hello: [0, 36],
         hello_there_peep: 36,
         help: [11, 18, 28, 29, 31],
         here: [0, 7, 8, 13, 14, 16, 34, 36, 37],
+        hewson: [11, 29],
         hex: [6, 7, 8, 9, 11, 14, 15, 20, 22, 23, 24, 26, 34, 36],
         hexadecim: [0, 2, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 34, 35, 36],
         high: [2, 33],
         highest: 34,
         highli: 14,
         hit: [11, 29],
         hlh: [8, 36],
@@ -1317,36 +1342,38 @@
         inform: [0, 3, 4, 8, 11, 13, 14, 18, 20, 27, 28, 29, 30, 31, 34, 35, 36],
         ini: [3, 9, 10, 11, 12, 20, 22, 23, 24, 26, 27],
         init: 15,
         init_pag: 15,
         initi: [4, 36],
         initialis: [0, 3, 11, 12, 29, 36],
         initmodul: [3, 14, 34],
+        injectaload: [11, 29],
         ink: [8, 36],
         inner: 36,
         input: [5, 6, 8, 11, 13, 16, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 29, 32, 34, 35, 36],
         input_regist: 16,
         inputregistertablehead: [6, 34],
         insert: [0, 3, 4, 9, 10, 11, 12, 15, 16, 36],
         insid: [3, 10, 11, 13, 29, 32, 34, 36],
         inspect: 15,
         instal: [0, 5, 6, 11, 17, 23, 34],
         instanc: [0, 5, 15, 33, 36],
         instead: [0, 3, 4, 5, 6, 8, 11, 13, 14, 15, 26, 29, 32, 34, 36],
-        instruct: [0, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 14, 16, 20, 21, 22, 23, 26, 27, 31, 34, 35, 36, 37, 38],
+        instruct: [0, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 14, 16, 20, 21, 22, 23, 26, 27, 29, 31, 34, 35, 36, 37, 38],
         instructionutil: 12,
         instructionwidth: [10, 11, 26],
         intact: 14,
         integ: [0, 3, 8, 9, 11, 12, 15, 20, 23, 36],
+        integr: [11, 29],
         intend: [0, 23, 34, 36],
         interest: [13, 34],
         intern: [0, 3, 20, 36],
         internet: 5,
         interpret: [3, 10, 14, 36],
-        interrupt: [11, 18, 28, 29, 34, 36],
+        interrupt: [3, 11, 18, 28, 29, 31, 34, 36],
         interruptdelai: [34, 36],
         interv: 36,
         intro: [7, 16, 34, 36],
         invalid: 5,
         invers: 15,
         inverseaddress: 15,
         invert: [10, 11, 13, 25],
@@ -1390,15 +1417,15 @@
         languag: [0, 12, 13, 14, 16, 36, 38],
         larg: 15,
         larger: 36,
         last: [0, 4, 5, 7, 11, 13, 15, 19, 29, 35, 36],
         later: [0, 9, 15, 33, 38],
         latest: [37, 38],
         layout: [5, 14, 15, 34],
-        lead: [3, 4, 15, 36],
+        lead: [3, 4, 11, 15, 29, 36],
         least: [11, 12, 13, 14, 16, 19, 24, 35, 36],
         leav: [0, 7, 11, 12, 13, 19, 20, 23, 34, 36],
         left: [0, 5, 6, 8, 9, 11, 13, 14, 15, 25, 31, 34, 36],
         leftmost: 36,
         length: [0, 1, 2, 3, 5, 6, 7, 9, 10, 11, 12, 16, 18, 19, 24, 25, 26, 27, 29, 31, 32, 34, 36],
         lengthcolumn: [7, 34],
         less: [11, 19, 36],
@@ -1407,39 +1434,39 @@
         level: [0, 5, 6, 7, 9, 11, 14, 16, 22, 33, 34, 35, 36],
         lib: 15,
         librari: [5, 6, 34],
         licens: 38,
         lies: 13,
         like: [0, 9, 13, 14, 15, 34, 36, 37],
         likewis: 35,
-        limit: [9, 11, 29, 32, 34, 36],
+        limit: [9, 32, 34, 36],
         line: [0, 1, 3, 5, 6, 7, 9, 10, 11, 13, 14, 15, 16, 20, 22, 23, 24, 26, 27, 29, 33, 34, 36],
         linewidth: [3, 11, 26],
         link: [3, 5, 6, 7, 8, 9, 10, 11, 12, 14, 20],
         link_text: [16, 36],
         linkinternaloperand: [7, 34],
         linkoperand: [6, 34],
         linux: 4,
         list: [0, 2, 3, 4, 5, 6, 7, 9, 10, 11, 12, 13, 14, 15, 20, 23, 24, 26, 27, 29, 30, 31, 32, 34, 35, 38],
         list_entri: 32,
         list_item: [7, 32],
         listitem: [3, 16, 34],
         listref: [0, 11, 26],
         liter: 36,
         live: [0, 14, 34, 36],
-        load: [2, 3, 5, 7, 8, 11, 14, 18, 19, 30, 31, 36],
+        load: [2, 3, 5, 7, 8, 14, 18, 19, 30, 31, 36],
         loader: [7, 11, 19, 29],
         local: [6, 11, 29, 37],
         locat: [6, 7, 9, 11, 13, 15, 16, 20, 23, 29, 34, 36, 37],
-        log: 11,
+        log: [11, 29],
         logo: [6, 14, 16, 34],
         logoimag: [6, 34],
         longer: [5, 6, 9, 11, 32, 36],
         look: [3, 11, 14, 15, 32, 34, 36, 38],
-        loop: [0, 3, 7, 16, 36],
+        loop: [0, 3, 7, 11, 16, 29, 36],
         lose: 14,
         low: [2, 5],
         lower: [0, 2, 3, 5, 6, 7, 9, 10, 11, 12, 15, 20, 22, 23, 24, 26, 34, 36],
         lowest: [11, 19, 34],
         lsb: [0, 16],
         m_list_item: 16,
         m_table_row: 16,
@@ -1470,34 +1497,38 @@
         mask: [0, 5, 7, 9, 15],
         match: [0, 3, 8, 11, 12, 13, 15, 16, 34, 35, 36],
         materi: 6,
         max: [0, 11, 31, 36],
         max_reg_len: [1, 3],
         maxamplitud: [3, 34],
         maximum: [0, 1, 3, 7, 11, 12, 15, 20, 26, 31],
+        md5: [3, 11, 29],
+        md5sum: [11, 29],
         mean: [11, 16, 19, 29, 34, 35, 36, 37],
         meaning: 14,
         meant: 0,
         meet: 36,
         memori: [0, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 16, 18, 19, 21, 23, 24, 25, 26, 27, 29, 31, 34, 36, 38],
         memorymap: [3, 5, 7, 9, 16, 32, 36],
         mere: 14,
         messag: [0, 11, 12, 13, 20, 26, 34, 36],
         messagesmap: 34,
         method: [7, 12, 13, 32, 36],
         methodnam: 36,
+        microspher: [11, 29],
         mid: [0, 1, 5, 11, 16, 22, 35, 36],
         might: [0, 14, 15, 32, 34, 36],
         migrat: 17,
         min: [0, 6, 20, 36],
         miner: [7, 38],
         minim: 15,
         minimum: [0, 10, 11, 12, 20, 24, 26, 36],
         minu: [11, 13, 18, 19, 24, 25, 26, 27, 31],
         minut: [11, 29],
+        mismatch: 29,
         miss: [5, 11, 12],
         mistak: 0,
         mnemon: 4,
         mode: [3, 5, 6, 8, 9, 10, 11, 12, 13, 15, 17, 18, 25, 28, 29, 31, 34, 35, 36],
         modif: [29, 34],
         modifi: [3, 4, 7, 8, 11, 13, 14, 28, 29, 34, 36, 38],
         modul: [0, 3, 6, 29, 34],
@@ -1528,25 +1559,25 @@
         needless: 14,
         neg: [10, 12, 13, 36],
         neither: [12, 15, 36],
         nervou: 14,
         nest: [5, 9, 36],
         never: [11, 14, 26],
         newlin: [5, 36],
-        next: [0, 9, 10, 11, 13, 14, 15, 16, 29, 32, 36],
+        next: [0, 3, 9, 10, 11, 13, 14, 15, 16, 29, 32, 36],
         next_entri: 16,
         nicer: 14,
         nine: 36,
         node: [0, 11, 27],
         nodeattribut: [11, 27],
         nodeid: [11, 27],
         nodelabel: [11, 27],
         nolabel: 9,
         non: [0, 3, 4, 6, 10, 11, 12, 16, 20, 24, 34, 36],
-        none: [0, 9, 11, 12, 13, 15, 16, 20, 27, 34],
+        none: [0, 9, 11, 12, 13, 15, 16, 20, 27, 29, 34],
         nonsens: 4,
         nop: 0,
         nor: [15, 36],
         normal: 13,
         notat: [0, 2, 5, 6, 13, 14, 16, 23, 35, 36],
         note: [0, 11, 12, 13, 14, 15, 16, 32, 34, 35, 36, 37],
         noth: 15,
@@ -1613,15 +1644,16 @@
         overlap: [0, 11, 19],
         overlay_udg: 15,
         overrid: [0, 3, 11, 15, 19, 20, 22, 23, 24, 26, 27, 31],
         overridden: [1, 34],
         overwrit: [0, 3, 5, 10, 11, 19, 23, 28, 29],
         overwrot: 11,
         overx: 36,
-        own: [0, 1, 5, 6, 14, 16, 34, 35, 36],
+        owen: [11, 29],
+        own: [0, 1, 3, 5, 6, 14, 16, 34, 35, 36],
         packag: [0, 5, 6, 11, 15, 20, 23, 34, 37],
         package_dir: [11, 23],
         pad: [8, 9, 36],
         page1id: 34,
         page2id: 34,
         page: [0, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 14, 23, 24, 26, 27, 32, 36, 38],
         page_head: 16,
@@ -1642,23 +1674,25 @@
         pars: [0, 3, 5, 6, 7, 8, 9, 11, 12, 17, 20, 25, 34, 35],
         parse_bracket: 15,
         parse_image_macro: 15,
         parse_int: 15,
         parse_str: 15,
         parser: 0,
         part: [0, 3, 6, 9, 13, 15, 34, 36],
-        particular: [14, 33, 37],
+        particular: [11, 14, 29, 33, 37],
         particularli: [14, 34],
         pass: [0, 11, 12, 13, 15, 16, 36],
         past: 29,
         patch: [11, 31],
         path: [0, 3, 5, 6, 7, 9, 10, 11, 15, 16, 20, 23, 26, 27, 29, 36, 37],
         path_id: 15,
         pathnam: 34,
         pattern: [0, 3, 12, 13, 34, 36],
+        paul: [11, 29],
+        paus: [3, 11, 29],
         peek29435: 36,
         peek32768: 36,
         peek33879: 36,
         peek37159: 36,
         peek37168: 36,
         peek40960: 0,
         peek47134: 36,
@@ -1681,19 +1715,20 @@
         philip: 38,
         pick: [0, 36],
         piec: [0, 3, 14, 36, 38],
         pil: 6,
         pip: 37,
         pipe: [8, 36],
         pixel: [3, 15, 36],
-        place: [0, 6, 7, 9, 13, 14, 15, 29, 34, 35, 36, 38],
+        place: [0, 6, 7, 9, 11, 13, 14, 15, 29, 34, 35, 36, 38],
         placehold: 36,
         plai: 14,
         plain: [13, 33, 34, 36],
         plan: 14,
+        playback: [11, 29],
         plot1: 36,
         plot: 3,
         plotx: 36,
         plu: 36,
         pluggabl: [3, 12],
         plum: [6, 14],
         png: [6, 8, 11, 15, 25, 32, 34, 36, 38],
@@ -1702,23 +1737,26 @@
         pngenableanim: 34,
         point: [0, 3, 4, 5, 6, 10, 11, 12, 16, 26, 35, 36],
         pointer: [5, 7, 11, 18, 29, 36],
         poke: [3, 4, 5, 6, 9, 11, 18, 23, 25, 28, 31, 34, 38],
         pokes30000: 8,
         pokes32772: 36,
         pokesaddr: 36,
+        polar: [11, 29],
+        poliload: [11, 29],
         pop: 6,
         pop_snapshot: 15,
         popul: [0, 9, 11, 15, 29, 36],
+        port: [11, 29],
         portion: [5, 36],
         posit: [5, 10, 11, 29, 36],
         possibl: [14, 15, 34, 35, 36],
         post: 15,
         potenti: 14,
-        power: [3, 36],
+        power: [3, 11, 29, 36],
         ppa: 37,
         pre: [34, 36],
         preced: [0, 6, 12, 34, 35, 36],
         prefer: [14, 15, 16, 34, 35],
         prefix: [1, 3, 4, 6, 8, 9, 10, 11, 13, 14, 15, 16, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 34, 35, 36, 37],
         prefix_len: 1,
         preformat: 16,
@@ -1735,51 +1773,54 @@
         previous: [0, 15, 36],
         print: [0, 3, 5, 11, 20, 36],
         pristin: [6, 14, 38],
         probabl: [14, 37],
         problem: [13, 15, 36],
         process: [0, 3, 6, 9, 10, 11, 16, 20, 21, 33, 35],
         prod: 36,
-        produc: [0, 1, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 14, 16, 20, 24, 27, 31, 32, 34, 36, 38],
+        produc: [0, 1, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 14, 16, 20, 24, 27, 29, 31, 32, 34, 36, 38],
         product: 36,
         profil: [11, 14, 24],
         program: [2, 3, 8, 9, 11, 18, 19, 27, 29, 30, 31, 35, 36, 38],
         programmat: [8, 36],
+        progress: [11, 29],
         prompt: 37,
         properti: [0, 1, 3, 5, 6, 8, 11, 12, 34, 36],
+        protect: [11, 29],
         provid: [3, 10, 11, 12, 13, 15, 34, 36],
         pub: [11, 29],
-        publish: 38,
-        puls: [10, 11],
+        publish: [11, 29, 38],
+        puls: [10, 11, 29],
         pure: [0, 7, 10, 11, 29, 36],
         purpl: 14,
         purpos: [0, 6, 9, 12, 14, 33, 36, 38],
         push: [0, 6],
         push_snapshot: 15,
         pypi: 37,
         python39: 37,
         python3: [15, 37],
         python: [0, 3, 5, 6, 8, 9, 11, 14, 16, 20, 23, 27, 29, 34, 36, 37],
         qualifi: 35,
         quiet: [11, 20, 23],
         quit: 35,
-        quot: [6, 12, 35],
+        quot: [3, 6, 11, 12, 35],
         r25404: 0,
         r25820: 36,
         r27126: 36,
         r27634: 0,
         r29015: 0,
         r32768: 35,
         r40000: 36,
         raddr1: 0,
         raddr2: 0,
         raddr: 36,
         rais: 12,
         ram: [3, 7, 8, 9, 11, 18, 27, 28, 29, 31, 34],
         rang: [0, 3, 6, 9, 11, 12, 13, 14, 19, 27, 34, 36],
+        ranger: [11, 29],
         rare: 13,
         rate: 34,
         rather: 14,
         rattr: 15,
         raw: [2, 3, 5, 9, 10, 11, 18, 19, 21, 24, 25, 26, 27, 31, 38],
         rbyte: 15,
         rc7: 2,
@@ -1794,23 +1835,23 @@
         rebuild: [3, 11, 23],
         rebuildaudio: [3, 11, 23],
         rebuildimag: [11, 23],
         recast: 13,
         recent: 15,
         recognis: [0, 2, 4, 11, 12, 18, 20, 22, 23, 24, 26, 27, 28, 29, 31, 32, 34, 36],
         recommend: [14, 36],
-        record: [11, 14, 27],
+        record: [11, 14, 27, 29],
         recov: 12,
         rectangl: 9,
         rectangular: [3, 5, 36],
         recurs: 16,
         red: [34, 36],
         redefin: 36,
         redistribut: 38,
-        reduc: [13, 31, 36],
+        reduc: [11, 13, 29, 31, 36],
         redund: [0, 5, 6],
         ref: [3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 14, 16, 17, 23, 26, 32, 33, 36, 38],
         ref_instruct: 12,
         refaddr: 36,
         refer: [0, 3, 5, 6, 7, 14, 32, 34, 36, 38],
         reference_entri: 32,
         referr: [0, 3, 4, 6, 11, 12, 26],
@@ -1865,14 +1906,15 @@
         resolv: [6, 36],
         resourc: [3, 6, 7, 9, 11, 23, 36, 38],
         respect: 36,
         respons: 12,
         restor: [6, 7, 8, 10, 13, 15],
         restrict: 15,
         result: [0, 2, 13, 14, 15, 28, 29, 32, 35, 36],
+        resum: [11, 29],
         ret: [0, 5, 11, 13, 36],
         retain: [9, 35, 36, 38],
         retriev: [3, 15, 36],
         revers: 0,
         rewritten: [32, 36],
         rfix: [3, 8, 9, 10, 11, 13, 20, 21, 33, 36],
         rgb: [12, 34, 36],
@@ -1904,16 +1946,16 @@
         rule: [6, 15, 16, 35],
         run: [0, 2, 3, 4, 5, 11, 14, 15, 16, 23, 29, 31, 33, 34, 35, 36, 37],
         rzx: 14,
         safe: [11, 20, 36],
         safe_kei: 36,
         sai: [14, 15],
         sam: [4, 5, 38],
-        same: [0, 3, 4, 6, 7, 8, 11, 12, 13, 14, 16, 32, 34, 35, 36],
-        sampl: 34,
+        same: [0, 3, 4, 6, 7, 8, 11, 12, 13, 14, 16, 29, 32, 34, 35, 36],
+        sampl: [3, 11, 29, 34],
         sampler: 34,
         satisfi: [11, 29],
         save: [0, 5, 11, 14, 15, 29, 36],
         savebin: 2,
         sbc: 4,
         scale: [11, 15, 25, 34, 36],
         scan: 8,
@@ -1933,23 +1975,24 @@
         section_nam: 15,
         section_typ: 15,
         sectionnam: 34,
         sectionprefix: [8, 34],
         sectiontyp: [3, 8, 9, 16, 34],
         see: [0, 11, 13, 14, 15, 16, 18, 20, 22, 23, 24, 26, 27, 28, 29, 31, 32, 34, 35, 36, 37, 38],
         seen: [33, 35],
-        select: 14,
+        select: [11, 14, 29],
         self: [15, 36],
         semicolon: [0, 5, 7, 9, 10, 11, 13, 26, 34, 36],
         sens: 13,
+        sensit: [11, 29],
         sentenc: 5,
         sep: [1, 16, 36],
         separ: [0, 1, 3, 5, 7, 8, 9, 11, 12, 13, 15, 16, 20, 23, 30, 34, 35, 36, 38],
         seq: 34,
-        sequenc: [0, 5, 6, 9, 10, 11, 12, 13, 15, 27, 31, 34, 35, 36, 38],
+        sequenc: [0, 3, 5, 6, 9, 10, 11, 12, 13, 15, 27, 31, 34, 35, 36, 38],
         seri: 36,
         serv: 34,
         set: [1, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 18, 19, 20, 22, 23, 24, 25, 26, 27, 28, 29, 31, 34, 36, 38],
         set_byte_valu: 12,
         setup: [5, 6],
         sever: [3, 11, 12, 36],
         sft: 32,
@@ -1963,72 +2006,76 @@
         should: [0, 3, 11, 12, 13, 14, 15, 16, 19, 32, 33, 36],
         show: [3, 4, 6, 7, 8, 9, 10, 11, 13, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 34, 36, 38],
         show_byt: [10, 16],
         shown: [3, 11, 13, 23, 31, 34, 35, 36, 37],
         side: 36,
         sign: [13, 36, 37],
         signatur: [12, 32, 36],
+        significantli: [11, 29],
         silent: 11,
         sim: [0, 3, 11, 29],
         similar: 34,
         simpl: [14, 15, 34, 36],
         simpler: [13, 14, 15],
         simpli: [35, 36],
         simplifi: [5, 11, 31],
         simstop: 36,
-        simul: [0, 3, 6, 11, 31, 36],
-        sinc: [0, 11, 29, 36],
-        singl: [0, 6, 7, 8, 10, 11, 13, 14, 15, 16, 23, 29, 33, 34, 35, 36],
+        simul: [0, 3, 6, 31, 36],
+        sinc: [0, 11, 18, 28, 29, 36],
+        singl: [0, 3, 6, 7, 8, 10, 11, 13, 14, 15, 16, 23, 29, 33, 34, 35, 36],
         size: [3, 11, 12, 13, 16, 25, 26, 28, 34, 36],
         sjasm: 2,
         sjasmplu: 9,
         skim: 14,
         skool2asm: [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 14, 15, 33, 35, 36, 38],
         skool2bin: [0, 3, 8, 10, 38],
         skool2ctl: [4, 5, 6, 7, 8, 9, 10, 13, 14, 32, 35, 38],
         skool2html: [0, 3, 4, 5, 6, 7, 8, 9, 10, 14, 15, 16, 33, 34, 35, 36, 38],
         skool2htmltest: 5,
         skool2sft: [5, 6, 7, 8, 10, 32],
-        skool: [0, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 16, 17, 20, 21, 22, 23, 25, 26, 33, 34, 38],
+        skool: [0, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 16, 17, 20, 21, 22, 23, 25, 26, 29, 33, 34, 38],
         skoolasm: [0, 15],
         skoolctl: 12,
         skoolfil: [11, 23],
         skoolhtml: [12, 15, 34],
         skoolkit: [0, 2, 3, 11, 14, 16, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 34, 35, 36],
         skoolmacro: 15,
         skoolpars: 12,
         skoolparsingerror: 12,
         sks: 14,
+        sky: [11, 29],
         slash: 37,
         slot: 36,
         slowdown: 34,
+        slowload: [11, 29],
         small: 34,
         smaller: 36,
         smith: [13, 35],
         smpl: [0, 11, 34],
         sna2ctl: [10, 12, 14, 38],
         sna2img: [8, 9, 38],
         sna2kool: 26,
         sna2skool: [0, 3, 4, 5, 6, 7, 8, 9, 10, 12, 13, 14, 36, 38],
         sna: [3, 6, 7, 8, 11, 19, 24, 25, 26, 27, 31, 38],
         snactl: 12,
         snapinfo: [0, 3, 8, 9, 12, 38],
-        snapmod: [8, 38],
+        snapmod: [3, 8, 38],
         snapshot: [0, 3, 5, 6, 7, 8, 9, 11, 14, 18, 19, 24, 25, 26, 27, 28, 29, 31, 38],
         snapshoterror: 12,
         snapshotread: 12,
         snapshotreferencecalcul: 12,
         snapshotreferenceoper: [3, 12],
         snaskool: 12,
         snippet: 13,
+        softlock: [11, 29],
         softwar: [34, 38],
         sole: [9, 29, 36],
         solut: 13,
         solv: [13, 15],
-        some: [0, 5, 6, 11, 13, 14, 15, 32, 33, 34, 35, 36, 37],
+        some: [0, 5, 6, 11, 13, 14, 15, 29, 32, 33, 34, 35, 36, 37],
         someth: [11, 13, 14, 15, 19, 33, 35],
         sometim: 13,
         somewher: [0, 15],
         soon: 36,
         sound: [11, 14, 31, 36, 38],
         sourc: [2, 4, 5, 6, 14, 32, 34, 38],
         space8: 36,
@@ -2039,15 +2086,16 @@
         spec1: 36,
         spec2: 36,
         specemu: [6, 8, 11, 14, 24],
         special: [0, 8, 11, 12, 13, 34, 36],
         specif: [3, 7, 8, 9, 11, 13, 15, 29, 34, 36],
         specifi: [0, 1, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 20, 23, 24, 26, 27, 29, 31, 34, 35, 36],
         spectrum: [0, 3, 6, 8, 11, 14, 15, 19, 24, 25, 29, 31, 36],
-        speed: [6, 11, 29, 30, 34],
+        speed: [3, 6, 11, 29, 30, 34],
+        speedlock: [11, 29],
         split: [0, 5, 7, 9, 11, 12, 13, 14, 34, 35, 36],
         split_operand: 12,
         sport: 14,
         sprite3: 15,
         sprite: [13, 15, 34, 36],
         sprite_id: 15,
         spriteid: 15,
@@ -2057,27 +2105,27 @@
         src: [4, 11, 16, 25, 28, 29],
         ssub: [5, 7, 8, 9, 10, 11, 12, 13, 20, 21, 33, 36],
         stabl: [37, 38],
         stack: [5, 6, 7, 8, 11, 18, 29, 36],
         stage: 29,
         stand: 36,
         standalon: [0, 6, 15, 34],
-        standard: [5, 8, 11, 18, 19, 20, 21, 22, 23, 24, 26, 27, 29, 30, 34, 36],
-        start: [1, 3, 4, 5, 6, 7, 8, 10, 11, 12, 15, 16, 18, 19, 20, 21, 22, 23, 24, 26, 27, 29, 31, 34, 35, 36, 38],
+        standard: [3, 5, 8, 11, 18, 19, 20, 21, 22, 23, 24, 26, 27, 29, 30, 34, 36],
+        start: [1, 3, 4, 5, 6, 7, 8, 10, 11, 12, 15, 16, 18, 19, 20, 21, 22, 23, 24, 26, 27, 28, 29, 31, 34, 35, 36, 38],
         stat: [11, 31],
         state: [3, 9, 11, 12, 13, 31, 34, 36],
         statement: [0, 3, 4, 5, 6, 7, 9, 10, 11, 12, 13, 16, 22, 26, 36],
         statist: 31,
         statu: [4, 11, 13, 16, 26, 34, 35],
         stdout: 22,
         step: [3, 6, 9, 11, 14, 15, 27, 29, 36],
         stick: 14,
-        still: [13, 15, 38],
+        still: [11, 13, 15, 29, 38],
         stock: [16, 34],
-        stop: [0, 3, 7, 11, 20, 21, 22, 24, 26, 31, 36],
+        stop: [0, 3, 7, 11, 20, 21, 22, 24, 26, 29, 31, 36],
         store: [0, 11, 13, 19, 29],
         str47154: 36,
         str47158: 36,
         str47161: 36,
         str: 3,
         straddr: 36,
         strftime: 15,
@@ -2104,15 +2152,15 @@
         subtitut: 35,
         subtract: 29,
         success: 36,
         succinctli: 13,
         suffix: [1, 3, 10, 11, 13, 14, 15, 16, 26, 27, 29, 34, 36],
         suit: 15,
         suitabl: [0, 29, 33, 34, 36, 37],
-        sum: 36,
+        sum: [3, 11, 29, 36],
         summari: 15,
         superimpos: [3, 15, 36],
         supplementari: 16,
         suppli: [0, 4, 10, 11, 12, 14, 34, 35, 36],
         support: [0, 3, 4, 5, 6, 7, 8, 9, 10, 11, 13, 14, 15, 17, 24, 32, 34, 35, 36],
         suppos: 36,
         suppress: [0, 3, 5, 7, 11, 20, 21],
@@ -2133,16 +2181,16 @@
         tabl: [0, 3, 5, 6, 7, 9, 10, 13, 15, 20, 32, 34, 35],
         table_cel: [7, 32],
         table_header_cel: [7, 32],
         table_row: [7, 32],
         take: [5, 6, 7, 13, 14, 16, 34, 36, 38],
         taken: [3, 11, 13, 14, 16, 29, 35, 36],
         tap2sna: [3, 6, 7, 8, 9, 14, 38],
-        tap: [5, 6, 8, 11, 19, 29, 30, 38],
-        tape: [2, 7, 9, 11, 19, 29],
+        tap: [3, 5, 6, 8, 11, 19, 29, 30, 38],
+        tape: [2, 3, 7, 9, 11, 19, 29],
         tapinfo: [3, 8, 9, 10, 38],
         tarbal: 37,
         target: [11, 15, 20, 33, 34],
         task: 15,
         tediou: 15,
         tell: [11, 14],
         templat: [3, 5, 6, 7, 8, 9, 10, 11, 17, 20, 26, 36],
@@ -2179,47 +2227,49 @@
         throughout: 37,
         thu: [0, 2, 5, 11, 13, 14, 15, 23, 34, 35, 36],
         tile32768: 36,
         tile: [8, 9, 11, 15, 25, 27, 38],
         tilen: 36,
         tiles32768: 36,
         time: [2, 3, 4, 10, 11, 13, 14, 15, 18, 20, 22, 23, 24, 25, 26, 27, 28, 29, 31, 34, 36],
+        timeout: [3, 11, 29],
         timestamp: 15,
         tindex: [3, 15, 36],
         tip: 32,
         titl: [0, 1, 3, 4, 5, 8, 9, 10, 11, 13, 14, 16, 22, 26, 35, 36],
         titleprefix: 32,
         titlesuffix: 32,
         togeth: [11, 19],
         token: [9, 11, 36],
         too: [11, 13, 14, 15, 29, 31, 35],
         top: [11, 13, 15, 16, 25, 34, 36],
         topmost: 36,
         total: 35,
         tpng: 11,
-        trace: [3, 14],
+        trace: [3, 14, 29],
         tracer: 14,
         track: [11, 15, 36],
         tradit: 14,
-        trail: [3, 36],
+        trail: [3, 11, 29, 36],
         transform: 33,
+        transit: 3,
         transpar: [3, 6, 15, 34, 36],
         treat: 14,
         trim: 15,
         triplet: [6, 12, 34],
         trivia: [4, 5, 6, 34, 38],
         truth: [16, 36],
-        tstate: [3, 11, 13, 31],
+        tstate: [3, 11, 13, 18, 28, 29, 31],
         tstates30000: 36,
         tstates40000: 36,
         tstates50002: 36,
         tstatesstart: 36,
         tune: 38,
         tupl: [12, 15, 36],
-        turbo: [11, 29, 30],
+        turbo: [3, 11, 29, 30],
         turn: 36,
         tutori: 14,
         twice: 3,
         two: [0, 4, 5, 6, 9, 10, 11, 12, 13, 15, 16, 20, 23, 26, 29, 33, 34, 35, 36],
         type: [3, 4, 5, 7, 10, 11, 12, 13, 15, 16, 22, 26, 29, 34, 35, 36],
         typic: [0, 13, 15, 16, 34, 35],
         tzx: [3, 6, 7, 8, 10, 11, 30, 38],
@@ -2261,14 +2311,15 @@
         unconvert: [0, 7],
         uncrop: 8,
         undefin: 36,
         under: [34, 38],
         underscor: 34,
         understand: 14,
         unexpand: 36,
+        uni: [11, 29],
         unicod: [6, 36],
         unind: 9,
         uniqu: 34,
         unit: 5,
         univers: 16,
         unlabel: [6, 11, 20, 23],
         unless: [9, 14, 36],
@@ -2276,18 +2327,18 @@
         unmatch: [15, 35],
         unpack: [14, 37],
         unprint: 10,
         unstyl: 32,
         unsupport: [0, 6, 20],
         until: [3, 11, 29],
         untitl: [11, 26],
-        unus: [0, 11, 13, 26, 34, 35],
+        unus: [0, 3, 11, 13, 26, 34, 35],
         unusedmap: 34,
         unwant: 16,
-        updat: [4, 5, 7, 14, 36],
+        updat: [3, 4, 5, 7, 14, 36],
         upon: [11, 13, 19],
         upper: [3, 5, 6, 10, 11, 12, 13, 15, 16, 20, 22, 23, 24, 26, 34, 36],
         url: [11, 29],
         usabl: [11, 19],
         usag: 11,
         use: [0, 2, 3, 5, 6, 7, 8, 9, 11, 12, 13, 14, 15, 16, 18, 19, 20, 22, 23, 24, 26, 27, 28, 29, 31, 32, 34, 35, 36, 37, 38],
         use_label: 12,
@@ -2305,22 +2356,22 @@
         val: 16,
         valid: [0, 12, 13, 16, 36],
         valu: [0, 1, 3, 6, 7, 8, 9, 10, 11, 12, 15, 16, 18, 19, 20, 22, 23, 24, 26, 27, 28, 29, 31, 34, 35, 36, 38],
         value1: [0, 15],
         value2: [0, 15],
         valueerror: 12,
         variabl: [0, 3, 8, 9, 11, 12, 15, 16, 20, 23, 27, 29, 34, 36, 37],
-        variou: [12, 34, 36, 37],
+        variou: [11, 12, 29, 34, 36, 37],
         verbatim: [8, 11, 13, 35, 36],
         verbos: [3, 11, 20, 21, 23, 31],
         veri: [9, 14, 35],
         versa: [0, 14],
         version: [0, 1, 2, 5, 7, 9, 11, 12, 13, 14, 15, 16, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 33, 34, 35, 38],
         vertic: [0, 3, 5, 6, 11, 15, 20, 25, 36],
-        via: [0, 3, 6, 8, 11, 12, 34, 36],
+        via: [0, 3, 6, 8, 11, 12, 29, 34, 36],
         vice: [0, 14],
         video: [11, 25],
         virtu: 34,
         wai: [0, 6, 8, 11, 13, 14, 15, 20, 22, 23, 24, 26, 27, 33, 34, 35, 36, 37],
         want: [0, 2, 13, 14, 15, 34, 36],
         warn: [0, 3, 5, 6, 7, 11, 12, 20, 21],
         wav: [0, 3, 11, 34, 36, 38],
@@ -2337,15 +2388,15 @@
         whether: [0, 3, 7, 11, 12, 15, 33, 36],
         which: [0, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 18, 20, 23, 26, 27, 29, 32, 33, 34, 35, 36, 37],
         whichev: 13,
         white: [18, 34, 36],
         whitespac: [3, 7, 15, 34, 35, 36],
         who: 38,
         whole: [13, 36],
-        whose: [0, 3, 9, 11, 12, 13, 14, 15, 16, 23, 26, 27, 34, 36],
+        whose: [0, 3, 9, 11, 12, 13, 14, 15, 16, 23, 26, 27, 29, 34, 36],
         why: [0, 14],
         wide: [5, 6, 11, 14, 23, 36],
         widest: 9,
         width: [0, 1, 3, 5, 6, 7, 10, 11, 13, 15, 16, 20, 25, 26, 36],
         wildcard: [9, 34],
         willi: [7, 38],
         within: [35, 36],
@@ -2355,15 +2406,15 @@
         work: [0, 2, 3, 5, 6, 7, 10, 11, 12, 13, 14, 15, 20, 22, 23, 24, 26, 27, 32, 36, 37],
         workaround: 2,
         would: [0, 11, 12, 13, 14, 15, 16, 36, 37],
         wouldn: 0,
         wrap: [0, 3, 6, 11, 12, 20, 26, 36],
         wrapalign: [10, 36],
         wrappabl: [0, 20],
-        write: [0, 2, 4, 5, 6, 7, 8, 10, 11, 12, 13, 14, 15, 20, 22, 23, 24, 25, 26, 28, 29, 34, 35, 36],
+        write: [0, 2, 3, 4, 5, 6, 7, 8, 10, 11, 12, 13, 14, 15, 20, 22, 23, 24, 25, 26, 28, 29, 34, 35, 36],
         write_imag: 12,
         writer: [3, 6, 7, 8, 11, 23, 34, 36],
         written: [10, 11, 13, 15, 20, 22, 24, 26, 34, 36, 38],
         wxh: [11, 25],
         x_offset: 15,
         xbc: 36,
         xde: 36,
@@ -2378,16 +2429,17 @@
         yield: 36,
         yoffset: 36,
         yor: 4,
         you: [0, 2, 11, 13, 14, 15, 16, 19, 23, 32, 34, 35, 36, 37, 38],
         your: [0, 2, 13, 14, 15, 32, 34, 37, 38],
         z80: [3, 5, 6, 7, 8, 11, 12, 14, 18, 19, 20, 24, 25, 26, 27, 28, 29, 31, 34, 35, 38],
         zero: [0, 3, 5, 6, 10, 11, 13, 14, 16, 24, 31, 34, 35, 36],
-        zip: [11, 29, 37],
-        zxspectrum48: 2
+        zip: [3, 11, 29, 37],
+        zxspectrum48: 2,
+        zydroload: [11, 29]
     },
     titles: ["ASM modes and directives", "ASM templates", "Supported assemblers", "Changelog", "SkoolKit 1.x changelog", "SkoolKit 2.x changelog", "SkoolKit 3.x changelog", "SkoolKit 4.x changelog", "SkoolKit 5.x changelog", "SkoolKit 6.x changelog", "SkoolKit 7.x changelog", "Commands", "SkoolKit components", "Control files", "Disassembly DIY", "Extending SkoolKit", "HTML templates", "SkoolKit manual", "bin2sna.py", "bin2tap.py", "skool2asm.py", "skool2bin.py", "skool2ctl.py", "skool2html.py", "sna2ctl.py", "sna2img.py", "sna2skool.py", "snapinfo.py", "snapmod.py", "tap2sna.py", "tapinfo.py", "trace.py", "Migrating from SkoolKit 7", "Parsing, rendering, and modes", "Ref files", "Skool files", "Skool macros", "Installing and using SkoolKit", "What is SkoolKit?"],
     titleterms: {
         "2010": [4, 5],
         "2011": 5,
         "2012": [5, 6],
         "2013": 6,
@@ -2396,14 +2448,15 @@
         "2016": 8,
         "2017": [8, 9],
         "2018": [9, 10],
         "2019": [3, 10],
         "2020": 3,
         "2021": 3,
         "2022": 3,
+        "2023": 3,
         "48k": 38,
         "case": 15,
         "switch": 14,
         "while": 36,
         Adding: 14,
         FOR: 36,
         The: [13, 14],
@@ -2512,15 +2565,15 @@
         level: 13,
         licenc: 38,
         limit: 13,
         line: [35, 37],
         link: [16, 34, 36],
         linux: 37,
         list: [16, 36],
-        load: 29,
+        load: [11, 29],
         loop: 13,
         macro: [15, 36],
         manual: 17,
         map: 36,
         mask: 36,
         memori: 15,
         memory_map: 16,
@@ -2576,15 +2629,15 @@
         rom: [0, 38],
         rsub: 0,
         scr: 36,
         section: 16,
         selector: 32,
         set: 0,
         sim: 36,
-        simul: 29,
+        simul: [11, 29],
         sjasmplu: 2,
         skeleton: 14,
         skool2asm: [11, 20],
         skool2bin: [11, 21],
         skool2ctl: [11, 22],
         skool2html: [11, 23],
         skool: [15, 32, 35, 36],
```

### Comparing `skoolkit-8.8/docs/skool-files.html` & `skoolkit-8.9/docs/skool-files.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Skool files &#8212; SkoolKit 8.8 documentation</title>
+    <title>Skool files &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
@@ -31,15 +31,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="skool-macros.html" title="Skool macros"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="control-files.html" title="Control files"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Skool files</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -409,17 +409,17 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="skool-macros.html" title="Skool macros"
              >next</a> |</li>
         <li class="right" >
           <a href="control-files.html" title="Control files"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Skool files</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Skool files
 ****** Skool filesÂ¶ ******
 A skool file contains the list of Z80 instructions that make up the routines
 and data blocks of the program being disassembled, with accompanying comments
 (if any).
 ***** Skool file formatÂ¶ *****
 A skool file must be in a certain format to ensure that it is processed
@@ -234,10 +234,10 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Skool files
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/skool-macros.html` & `skoolkit-8.9/docs/skool-macros.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Skool macros &#8212; SkoolKit 8.8 documentation</title>
+    <title>Skool macros &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
@@ -31,15 +31,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="ref-files.html" title="Ref files"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="skool-files.html" title="Skool files"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Skool macros</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -3223,17 +3223,17 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="ref-files.html" title="Ref files"
              >next</a> |</li>
         <li class="right" >
           <a href="skool-files.html" title="Skool files"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Skool macros</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Skool macros
 ****** Skool macrosÂ¶ ******
 Skool files and ref files may contain skool macros that are âexpandedâ to
 an appropriate piece of HTML markup (when rendering in HTML mode), or to an
 appropriate piece of plain text (when rendering in ASM mode).
 ***** SyntaxÂ¶ *****
 Skool macros have the following general form:
@@ -1881,10 +1881,10 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Skool macros
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/usage.html` & `skoolkit-8.9/docs/usage.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Installing and using SkoolKit &#8212; SkoolKit 8.8 documentation</title>
+    <title>Installing and using SkoolKit &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
@@ -31,15 +31,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="diy.html" title="Disassembly DIY"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="whatis.html" title="What is SkoolKit?"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Installing and using SkoolKit</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -166,17 +166,17 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="diy.html" title="Disassembly DIY"
              >next</a> |</li>
         <li class="right" >
           <a href="whatis.html" title="What is SkoolKit?"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Installing and using SkoolKit</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Installing and using SkoolKit
 ****** Installing and using SkoolKitÂ¶ ******
 ***** RequirementsÂ¶ *****
 SkoolKit requires Python 3.7+. If youâre running Linux or one of the BSDs,
 you probably already have Python installed. If youâre running Windows, you
 can get Python here.
 ***** InstallationÂ¶ *****
@@ -69,10 +69,10 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * Installing and using SkoolKit
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/docs/whatis.html` & `skoolkit-8.9/docs/whatis.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>What is SkoolKit? &#8212; SkoolKit 8.8 documentation</title>
+    <title>What is SkoolKit? &#8212; SkoolKit 8.9 documentation</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/classic.css" type="text/css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
@@ -31,15 +31,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="usage.html" title="Installing and using SkoolKit"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="index.html" title="SkoolKit manual"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">What is SkoolKit?</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -190,17 +190,17 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="usage.html" title="Installing and using SkoolKit"
              >next</a> |</li>
         <li class="right" >
           <a href="index.html" title="SkoolKit manual"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">SkoolKit 8.9 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">What is SkoolKit?</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2022, Richard Dymond.
+        &#169; Copyright 2023, Richard Dymond.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * What is SkoolKit?
 ****** What is SkoolKit?Â¶ ******
 SkoolKit is a collection of utilities that can be used to disassemble a
 Spectrum game (or indeed any piece of Spectrum software written in machine
 code) into a format known as a skool file. Then, from this skool file, you can
 use SkoolKit to create a browsable disassembly in HTML format, or a re-
 assemblable disassembly in assembly language. So the skool file is - from start
@@ -100,10 +100,10 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * SkoolKit_8.8_documentation »
+    * SkoolKit_8.9_documentation »
     * What is SkoolKit?
-© Copyright 2022, Richard Dymond. Created using Sphinx 3.4.3.
+© Copyright 2023, Richard Dymond. Created using Sphinx 3.4.3.
```

### Comparing `skoolkit-8.8/examples/hungry_horace.ctl` & `skoolkit-8.9/examples/hungry_horace.ctl`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/examples/hungry_horace.ref` & `skoolkit-8.9/examples/hungry_horace.ref`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/man/man1/bin2sna.py.1` & `skoolkit-8.9/man/man1/bin2sna.py.1`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "BIN2SNA.PY" "1" "Nov 19, 2022" "8.8" "SkoolKit"
+.TH "BIN2SNA.PY" "1" "Feb 19, 2023" "8.9" "SkoolKit"
 .SH NAME
 bin2sna.py \- convert a binary file into a Z80 snapshot
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -129,26 +129,25 @@
 
 .in +2
 \fB\-\-state name=value\fP
 .in -2
 .fi
 .sp
 .sp
-Recognised attribute names are:
-.INDENT 0.0
-.TP
-.B \fBborder\fP
-border colour
-.TP
-.B \fBiff\fP
-interrupt flip\-flop: 0=disabled, 1=enabled
-.TP
-.B \fBim\fP
-interrupt mode
-.UNINDENT
+Recognised attribute names and their default values are:
+.nf
+
+.in +2
+\fBborder\fP  \- border colour (default=0)
+\fBiff\fP     \- interrupt flip\-flop: 0=disabled, 1=enabled (default=1)
+\fBim\fP      \- interrupt mode (default=1)
+\fBtstates\fP \- T\-states elapsed since start of frame (default=0)
+.in -2
+.fi
+.sp
 .SH EXAMPLES
 .INDENT 0.0
 .IP 1. 3
 Convert \fBgame.bin\fP into a Z80 snapshot named \fBgame.z80\fP:
 .nf
 
 .in +2
@@ -166,10 +165,10 @@
 .in -2
 .fi
 .sp
 .UNINDENT
 .SH AUTHOR
 Richard Dymond
 .SH COPYRIGHT
-2022, Richard Dymond
+2023, Richard Dymond
 .\" Generated by docutils manpage writer.
 .
```

### Comparing `skoolkit-8.8/man/man1/bin2tap.py.1` & `skoolkit-8.9/man/man1/bin2tap.py.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "BIN2TAP.PY" "1" "Nov 19, 2022" "8.8" "SkoolKit"
+.TH "BIN2TAP.PY" "1" "Feb 19, 2023" "8.9" "SkoolKit"
 .SH NAME
 bin2tap.py \- convert a binary file or snapshot into a TAP file
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -116,10 +116,10 @@
 .in -2
 .fi
 .sp
 .UNINDENT
 .SH AUTHOR
 Richard Dymond
 .SH COPYRIGHT
-2022, Richard Dymond
+2023, Richard Dymond
 .\" Generated by docutils manpage writer.
 .
```

### Comparing `skoolkit-8.8/man/man1/skool2asm.py.1` & `skoolkit-8.9/man/man1/skool2asm.py.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "SKOOL2ASM.PY" "1" "Nov 19, 2022" "8.8" "SkoolKit"
+.TH "SKOOL2ASM.PY" "1" "Feb 19, 2023" "8.9" "SkoolKit"
 .SH NAME
 skool2asm.py \- convert a skool file to ASM format
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -351,10 +351,10 @@
 .in -2
 .fi
 .sp
 .UNINDENT
 .SH AUTHOR
 Richard Dymond
 .SH COPYRIGHT
-2022, Richard Dymond
+2023, Richard Dymond
 .\" Generated by docutils manpage writer.
 .
```

### Comparing `skoolkit-8.8/man/man1/skool2bin.py.1` & `skoolkit-8.9/man/man1/skool2bin.py.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "SKOOL2BIN.PY" "1" "Nov 19, 2022" "8.8" "SkoolKit"
+.TH "SKOOL2BIN.PY" "1" "Feb 19, 2023" "8.9" "SkoolKit"
 .SH NAME
 skool2bin.py \- convert a skool file into a binary (raw memory) file
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -109,10 +109,10 @@
 .in -2
 .fi
 .sp
 .UNINDENT
 .SH AUTHOR
 Richard Dymond
 .SH COPYRIGHT
-2022, Richard Dymond
+2023, Richard Dymond
 .\" Generated by docutils manpage writer.
 .
```

### Comparing `skoolkit-8.8/man/man1/skool2ctl.py.1` & `skoolkit-8.9/man/man1/skool2ctl.py.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "SKOOL2CTL.PY" "1" "Nov 19, 2022" "8.8" "SkoolKit"
+.TH "SKOOL2CTL.PY" "1" "Feb 19, 2023" "8.9" "SkoolKit"
 .SH NAME
 skool2ctl.py \- convert a skool file into a control file
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -172,10 +172,10 @@
 .in -2
 .fi
 .sp
 .UNINDENT
 .SH AUTHOR
 Richard Dymond
 .SH COPYRIGHT
-2022, Richard Dymond
+2023, Richard Dymond
 .\" Generated by docutils manpage writer.
 .
```

### Comparing `skoolkit-8.8/man/man1/skool2html.py.1` & `skoolkit-8.9/man/man1/skool2html.py.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "SKOOL2HTML.PY" "1" "Nov 19, 2022" "8.8" "SkoolKit"
+.TH "SKOOL2HTML.PY" "1" "Feb 19, 2023" "8.9" "SkoolKit"
 .SH NAME
 skool2html.py \- convert a skool file and ref files to HTML
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -387,10 +387,10 @@
 .in -2
 .fi
 .sp
 .UNINDENT
 .SH AUTHOR
 Richard Dymond
 .SH COPYRIGHT
-2022, Richard Dymond
+2023, Richard Dymond
 .\" Generated by docutils manpage writer.
 .
```

### Comparing `skoolkit-8.8/man/man1/sna2ctl.py.1` & `skoolkit-8.9/man/man1/sna2ctl.py.1`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "SNA2CTL.PY" "1" "Nov 19, 2022" "8.8" "SkoolKit"
+.TH "SNA2CTL.PY" "1" "Feb 19, 2023" "8.9" "SkoolKit"
 .SH NAME
 sna2ctl.py \- generate a control file for a binary file or a snapshot
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -167,10 +167,10 @@
 .in -2
 .fi
 .sp
 .UNINDENT
 .SH AUTHOR
 Richard Dymond
 .SH COPYRIGHT
-2022, Richard Dymond
+2023, Richard Dymond
 .\" Generated by docutils manpage writer.
 .
```

### Comparing `skoolkit-8.8/man/man1/sna2img.py.1` & `skoolkit-8.9/man/man1/sna2img.py.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "SNA2IMG.PY" "1" "Nov 19, 2022" "8.8" "SkoolKit"
+.TH "SNA2IMG.PY" "1" "Feb 19, 2023" "8.9" "SkoolKit"
 .SH NAME
 sna2img.py \- convert a binary file or a SCR/SKOOL/SNA/SZX/Z80 file into a PNG file
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -133,10 +133,10 @@
 .in -2
 .fi
 .sp
 .UNINDENT
 .SH AUTHOR
 Richard Dymond
 .SH COPYRIGHT
-2022, Richard Dymond
+2023, Richard Dymond
 .\" Generated by docutils manpage writer.
 .
```

### Comparing `skoolkit-8.8/man/man1/sna2skool.py.1` & `skoolkit-8.9/man/man1/sna2skool.py.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "SNA2SKOOL.PY" "1" "Nov 19, 2022" "8.8" "SkoolKit"
+.TH "SNA2SKOOL.PY" "1" "Feb 19, 2023" "8.9" "SkoolKit"
 .SH NAME
 sna2skool.py \- convert a binary file or a snapshot into a skool file
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -274,10 +274,10 @@
 .in -2
 .fi
 .sp
 .UNINDENT
 .SH AUTHOR
 Richard Dymond
 .SH COPYRIGHT
-2022, Richard Dymond
+2023, Richard Dymond
 .\" Generated by docutils manpage writer.
 .
```

### Comparing `skoolkit-8.8/man/man1/snapinfo.py.1` & `skoolkit-8.9/man/man1/snapinfo.py.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "SNAPINFO.PY" "1" "Nov 19, 2022" "8.8" "SkoolKit"
+.TH "SNAPINFO.PY" "1" "Feb 19, 2023" "8.9" "SkoolKit"
 .SH NAME
 snapinfo.py \- show information on the registers and RAM in a snapshot file
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -196,10 +196,10 @@
 \fBsnapinfo.py \-T 2,3\-1\-2 game.z80\fP
 .in -2
 .fi
 .sp
 .SH AUTHOR
 Richard Dymond
 .SH COPYRIGHT
-2022, Richard Dymond
+2023, Richard Dymond
 .\" Generated by docutils manpage writer.
 .
```

### Comparing `skoolkit-8.8/man/man1/snapmod.py.1` & `skoolkit-8.9/man/man1/snapmod.py.1`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "SNAPMOD.PY" "1" "Nov 19, 2022" "8.8" "SkoolKit"
+.TH "SNAPMOD.PY" "1" "Feb 19, 2023" "8.9" "SkoolKit"
 .SH NAME
 snapmod.py \- modify a 48K Z80 snapshot
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -116,47 +116,46 @@
 
 .in +2
 \fB\-\-state name=value\fP
 .in -2
 .fi
 .sp
 .sp
-Recognised attribute names are:
-.INDENT 0.0
-.TP
-.B \fBborder\fP
-border colour
-.TP
-.B \fBiff\fP
-interrupt flip\-flop: 0=disabled, 1=enabled
-.TP
-.B \fBim\fP
-interrupt mode
-.UNINDENT
+Recognised attribute names and their default values are:
+.nf
+
+.in +2
+\fBborder\fP  \- border colour (default=0)
+\fBiff\fP     \- interrupt flip\-flop: 0=disabled, 1=enabled (default=1)
+\fBim\fP      \- interrupt mode (default=1)
+\fBtstates\fP \- T\-states elapsed since start of frame (default=0)
+.in -2
+.fi
+.sp
 .SH EXAMPLES
 .INDENT 0.0
 .IP 1. 3
-Set the value of the HL register pair to 0 in game.z80:
+Set the value of the HL register pair to 0 in \fBgame.z80\fP:
 .nf
 
 .in +2
 \fBsnapmod.py \-f \-r hl=0 game.z80\fP
 .in -2
 .fi
 .sp
 .IP 2. 3
-POKE the value 23 into address 32768 in game.z80, and write the resultant
-snapshot to poked.z80:
+POKE the value 23 into address 32768 in \fBgame.z80\fP, and write the
+resultant snapshot to \fBpoked.z80\fP:
 .nf
 
 .in +2
 \fBsnapmod.py \-p 32768,23 game.z80 poked.z80\fP
 .in -2
 .fi
 .sp
 .UNINDENT
 .SH AUTHOR
 Richard Dymond
 .SH COPYRIGHT
-2022, Richard Dymond
+2023, Richard Dymond
 .\" Generated by docutils manpage writer.
 .
```

### Comparing `skoolkit-8.8/man/man1/tap2sna.py.1` & `skoolkit-8.9/man/man1/tap2sna.py.1`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "TAP2SNA.PY" "1" "Nov 19, 2022" "8.8" "SkoolKit"
+.TH "TAP2SNA.PY" "1" "Feb 19, 2023" "8.9" "SkoolKit"
 .SH NAME
 tap2sna.py \- convert a TAP or TZX file into a snapshot file
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -41,14 +41,19 @@
 \fBtap2sna.py\fP converts a TAP or TZX file (which may be inside a zip archive)
 into a Z80 snapshot. INPUT may be the full URL to a remote zip archive or
 TAP/TZX file, or the path to a local file. Arguments may be read from FILE
 instead of (or as well as) being given on the command line.
 .SH OPTIONS
 .INDENT 0.0
 .TP
+.B \-c, \-\-sim\-load\-config name=value
+Set the value of a \fB\-\-sim\-load\fP configuration parameter. Do \fB\-c help\fP for
+more information, and see the section on \fBSIMULATED LOAD\fP below. This
+option may be used multiple times.
+.TP
 .B \-d, \-\-output\-dir \fIDIR\fP
 Write the snapshot file in this directory.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-f\fP,\fB  \-\-force
 Overwrite an existing snapshot.
@@ -86,46 +91,135 @@
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-\-state name=value
 Set a hardware state attribute. Do \fB\-\-state help\fP for more information, or
 see the section on \fBHARDWARE STATE\fP below. This option may be used multiple
 times.
+.UNINDENT
+.INDENT 0.0
+.TP
+.BI \-\-tape\-name \ NAME
+Specify the name of a TAP/TZX file in a zip archive. By default, the first
+TAP/TZX file found in the zip archive is selected.
+.TP
+.BI \-\-tape\-start \ BLOCK
+Start the tape at this block number. In a TAP/TZX file, the first block is
+number 1, the second is 2, etc.
+.TP
+.BI \-\-tape\-stop \ BLOCK
+Stop the tape at this block number. In a TAP/TZX file, the first block is
+number 1, the second is 2, etc.
+.TP
+.BI \-\-tape\-sum \ MD5SUM
+Specify the MD5 checksum of the TAP/TZX file. \fBtap2sna.py\fP will abort if
+there is a checksum mismatch.
+.UNINDENT
+.INDENT 0.0
 .TP
 .B \-u, \-\-user\-agent \fIAGENT\fP
 Set the User\-Agent header used in an HTTP(S) request.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-V\fP,\fB  \-\-version
 Show the SkoolKit version number and exit.
 .UNINDENT
+.SH TZX SUPPORT
+.sp
+\fBtap2sna.py\fP can read data from TZX block types 0x10 (standard speed data),
+0x11 (turbo speed data) and 0x14 (pure data), but not block types 0x15 (direct
+recording), 0x18 (CSW recording) or 0x19 (generalized data block).
 .SH SIMULATED LOAD
 .sp
 The \fB\-\-sim\-load\fP option simulates a freshly booted 48K ZX Spectrum running
 LOAD "" (or LOAD ""CODE, if the first block on the tape is a \(aqBytes\(aq header).
 Whenever the Spectrum ROM\(aqs load routine at $0556 is called, a shortcut is
-taken by fast loading the next block on the tape. All other code (including any
-custom loader) is fully simulated. Simulation continues until the program
+taken by "fast loading" the next block on the tape. All other code (including
+any custom loader) is fully simulated. Simulation continues until the program
 counter hits the start address given by the \fB\-\-start\fP option, or 10 minutes
 of simulated Z80 CPU time has elapsed, or the end of the tape is reached and
 one of the following conditions is satisfied:
 .INDENT 0.0
 .IP \(bu 2
 a custom loader was detected
 .IP \(bu 2
 the program counter hits an address outside the ROM
 .IP \(bu 2
 more than one second of simulated Z80 CPU time has elapsed since the end of
 the tape was reached
 .UNINDENT
 .sp
-The simulation can also be aborted by pressing Ctrl\-C. When a simulated LOAD
+A simulated LOAD can also be aborted by pressing Ctrl\-C. When a simulated LOAD
 has completed or been aborted, the values of the registers (including the
 program counter) in the simulator are used to populate the Z80 snapshot.
+.sp
+A simulated LOAD can be configured via parameters that are set by the
+by the \fB\-\-sim\-load\-config\fP (or \fB\-c\fP) option. The recognised configuration
+parameters are:
+.INDENT 0.0
+.IP \(bu 2
+\fBaccelerator\fP \- the tape\-sampling loop accelerator to use (default:
+automatically selected \- see below); use this to specify a particular
+accelerator (which may produce a faster simulated LOAD), or to disable
+acceleration entirely (\fBaccelerator=none\fP)
+.IP \(bu 2
+\fBfast\-load\fP \- enable fast loading (\fB1\fP, the default), or disable it
+(\fB0\fP); fast loading significantly reduces the load time for many tapes, but
+can also cause some loaders to fail
+.IP \(bu 2
+\fBfirst\-edge\fP \- the time (in T\-states) from the start of the tape at which
+to place the leading edge of the first pulse (default: \fB\-2168\fP); the
+default value places the trailing edge of the first pulse at time 0, but some
+loaders (e.g. polarity\-sensitive loaders) require \fBfirst\-edge=0\fP
+.IP \(bu 2
+\fBpause\fP \- pause the tape between blocks and resume playback when port 254
+is read (\fB1\fP, the default), or run the tape continuously (\fB0\fP); pausing
+can help with tapes that require (but do not actually contain) long pauses
+between blocks, but can cause some loaders to fail
+.IP \(bu 2
+\fBtimeout\fP \- the number of seconds of Z80 CPU time after which to abort the
+simulated LOAD if it\(aqs still in progress (default: 900)
+.IP \(bu 2
+\fBtrace\fP \- the file to which to log all instructions executed during the
+simulated LOAD (default: none)
+.UNINDENT
+.sp
+The names of the available tape\-sampling loop accelerators are:
+.nf
+
+.in +2
+\fBalkatraz\fP \- Alkatraz
+\fBalkatraz2\fP \- Alkatraz 2
+\fBbleepload\fP \- Firebird BleepLoad
+\fBcyberlode\fP \- Cyberlode 1.1
+\fBdigital\-integration\fP \- Digital Integration
+\fBdinaload\fP \- Dinaload
+\fBedge\fP \- Edge
+\fBelite\-uni\-loader\fP \- Elite Uni\-Loader
+\fBexcelerator\fP \- The Excelerator Loader
+\fBflash\-loader\fP \- Flash Loader
+\fBftl\fP \- FTL
+\fBgargoyle\fP \- Gargoyle
+\fBgremlin\fP \- various games published by Gremlin Graphics
+\fBhewson\-slowload\fP \- Hewson Slowload
+\fBinjectaload\fP \- Injectaload
+\fBmicrosphere\fP \- Back to Skool, Skool Daze, Sky Ranger
+\fBnone\fP \- no accelerator
+\fBpaul\-owens\fP \- Paul Owens Protection System
+\fBpoliload\fP \- Poliload
+\fBpower\-load\fP \- Power\-Load
+\fBrom\fP \- any loader whose sampling loop is the same as the ROM\(aqs
+\fBsearch\-loader\fP \- Search Loader
+\fBsoftlock\fP \- SoftLock
+\fBspeedlock\fP \- Speedlock (all versions)
+\fBzydroload\fP \- Zydroload
+.in -2
+.fi
+.sp
 .SH CALL OPERATIONS
 .sp
 The \fB\-\-ram\fP option can be used to call a Python function to perform arbitrary
 modification of the memory snapshot.
 .nf
 
 .in +2
@@ -324,25 +418,24 @@
 .in +2
 \fB\-\-state name=value\fP
 .in -2
 .fi
 .sp
 .sp
 Recognised attribute names and their default values are:
-.INDENT 0.0
-.TP
-.B \fBborder\fP
-border colour (default=0)
-.TP
-.B \fBiff\fP
-interrupt flip\-flop: 0=disabled, 1=enabled (default=1)
-.TP
-.B \fBim\fP
-interrupt mode (default=1)
-.UNINDENT
+.nf
+
+.in +2
+\fBborder\fP  \- border colour (default=0)
+\fBiff\fP     \- interrupt flip\-flop: 0=disabled, 1=enabled (default=1)
+\fBim\fP      \- interrupt mode (default=1)
+\fBtstates\fP \- T\-states elapsed since start of frame (default=0)
+.in -2
+.fi
+.sp
 .SH READING ARGUMENTS FROM A FILE
 .sp
 For complex snapshots that require many \fB\-\-ram\fP, \fB\-\-reg\fP or \fB\-\-state\fP
 options to build, it may be more convenient to store the arguments to
 \fBtap2sna.py\fP in a file. For example, if the file \fBgame.t2s\fP has the
 following contents:
 .nf
@@ -371,18 +464,14 @@
 \fBtap2sna.py @game.t2s\fP
 .in -2
 .fi
 .sp
 .sp
 will create \fBgame.z80\fP as if the arguments specified in \fBgame.t2s\fP had been
 given on the command line.
-.SH TZX SUPPORT
-.sp
-Support for TZX files is limited to block types 0x10 (standard speed data),
-0x11 (turbo speed data) and 0x14 (pure data).
 .SH EXAMPLES
 .INDENT 0.0
 .IP 1. 3
 Extract the TAP or TZX file from a remote zip archive and convert it into a
 Z80 snapshot:
 .nf
 
@@ -421,10 +510,10 @@
 .in -2
 .fi
 .sp
 .UNINDENT
 .SH AUTHOR
 Richard Dymond
 .SH COPYRIGHT
-2022, Richard Dymond
+2023, Richard Dymond
 .\" Generated by docutils manpage writer.
 .
```

### Comparing `skoolkit-8.8/man/man1/tapinfo.py.1` & `skoolkit-8.9/man/man1/tapinfo.py.1`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "TAPINFO.PY" "1" "Nov 19, 2022" "8.8" "SkoolKit"
+.TH "TAPINFO.PY" "1" "Feb 19, 2023" "8.9" "SkoolKit"
 .SH NAME
 tapinfo.py \- show the blocks in a TAP or TZX file
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -79,10 +79,10 @@
 \fBtapinfo.py \-B 2 game.tap\fP
 .in -2
 .fi
 .sp
 .SH AUTHOR
 Richard Dymond
 .SH COPYRIGHT
-2022, Richard Dymond
+2023, Richard Dymond
 .\" Generated by docutils manpage writer.
 .
```

### Comparing `skoolkit-8.8/man/man1/trace.py.1` & `skoolkit-8.9/man/man1/trace.py.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "TRACE.PY" "1" "Nov 19, 2022" "8.8" "SkoolKit"
+.TH "TRACE.PY" "1" "Feb 19, 2023" "8.9" "SkoolKit"
 .SH NAME
 trace.py \- simulate code execution in a 48K memory snapshot
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -58,14 +58,21 @@
 .B \-D\fP,\fB  \-\-decimal
 Show decimal values in verbose (\fB\-v\fP, \fB\-vv\fP) mode.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-\-dump \fIFILE\fP
 Dump a Z80 snapshot to this file after execution.
+.UNINDENT
+.INDENT 0.0
+.TP
+.B \-i\fP,\fB  \-\-interrupts
+Execute interrupt routines.
+.UNINDENT
+.INDENT 0.0
 .TP
 .B \-\-max\-operations \fIMAX\fP
 Maximum number of instructions to execute. Overrides the \fISTOP\fP address (if
 given).
 .TP
 .B \-\-max\-tstates \fIMAX\fP
 Maximum number of (simulated) T\-states to run for. Overrides the \fISTOP\fP
@@ -176,10 +183,10 @@
 \fBtrace.py \-\-audio \-s 49152 \-S 49193 game.z80\fP
 .in -2
 .fi
 .sp
 .SH AUTHOR
 Richard Dymond
 .SH COPYRIGHT
-2022, Richard Dymond
+2023, Richard Dymond
 .\" Generated by docutils manpage writer.
 .
```

### Comparing `skoolkit-8.8/setup.cfg` & `skoolkit-8.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skool2asm.py` & `skoolkit-8.9/skool2asm.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skool2bin.py` & `skoolkit-8.9/skool2bin.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skool2ctl.py` & `skoolkit-8.9/skool2ctl.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skool2html.py` & `skoolkit-8.9/skool2html.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/__init__.py` & `skoolkit-8.9/skoolkit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2011-2022 Richard Dymond (rjdymond@gmail.com)
+# Copyright 2011-2023 Richard Dymond (rjdymond@gmail.com)
 #
 # This file is part of SkoolKit.
 #
 # SkoolKit is free software: you can redistribute it and/or modify it under the
 # terms of the GNU General Public License as published by the Free Software
 # Foundation, either version 3 of the License, or (at your option) any later
 # version.
@@ -18,15 +18,15 @@
 import html
 import sys
 import os
 import posixpath
 import textwrap
 import importlib
 
-VERSION = '8.8'
+VERSION = '8.9'
 PACKAGE_DIR = os.path.dirname(__file__)
 
 BASE_10 = 10
 BASE_16 = 16
 
 CASE_LOWER = 1
 CASE_UPPER = 2
```

### Comparing `skoolkit-8.8/skoolkit/audio.py` & `skoolkit-8.9/skoolkit/audio.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/basic.py` & `skoolkit-8.9/skoolkit/basic.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/bin2sna.py` & `skoolkit-8.9/skoolkit/bin2sna.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/bin2tap.py` & `skoolkit-8.9/skoolkit/bin2tap.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/components.py` & `skoolkit-8.9/skoolkit/components.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/config.py` & `skoolkit-8.9/skoolkit/config.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/ctlparser.py` & `skoolkit-8.9/skoolkit/ctlparser.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/defaults.py` & `skoolkit-8.9/skoolkit/defaults.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/disassembler.py` & `skoolkit-8.9/skoolkit/disassembler.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/graphics.py` & `skoolkit-8.9/skoolkit/graphics.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/image.py` & `skoolkit-8.9/skoolkit/image.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/opcodes.py` & `skoolkit-8.9/skoolkit/opcodes.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/pngwriter.py` & `skoolkit-8.9/skoolkit/pngwriter.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/refparser.py` & `skoolkit-8.9/skoolkit/refparser.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/resources/48.rom` & `skoolkit-8.9/skoolkit/resources/48.rom`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/resources/skoolkit-dark.css` & `skoolkit-8.9/skoolkit/resources/skoolkit-dark.css`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/resources/skoolkit-green.css` & `skoolkit-8.9/skoolkit/resources/skoolkit-green.css`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/resources/skoolkit-plum.css` & `skoolkit-8.9/skoolkit/resources/skoolkit-plum.css`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/resources/skoolkit.css` & `skoolkit-8.9/skoolkit/resources/skoolkit.css`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/simtables.py` & `skoolkit-8.9/skoolkit/simtables.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/simulator.py` & `skoolkit-8.9/skoolkit/simulator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Richard Dymond (rjdymond@gmail.com)
+# Copyright 2022, 2023 Richard Dymond (rjdymond@gmail.com)
 #
 # This file is part of SkoolKit.
 #
 # SkoolKit is free software: you can redistribute it and/or modify it under the
 # terms of the GNU General Public License as published by the Free Software
 # Foundation, either version 3 of the License, or (at your option) any later
 # version.
@@ -118,15 +118,15 @@
             0      # T (T-states)
         ]
         if registers:
             self.set_registers(registers)
         if state is None:
             state = {}
         self.imode = state.get('im', 1)
-        self.iff2 = state.get('iff', 0)
+        self.iff = state.get('iff', 0)
         self.registers[25] = state.get('tstates', 0)
         cfg = CONFIG.copy()
         if config:
             cfg.update(config)
         self.create_opcodes()
         if cfg['fast_djnz']:
             self.opcodes[0x10] = partial(self.djnz_fast, self.registers, self.memory)
@@ -147,15 +147,15 @@
             self.out_tracer = None
 
     def run(self, start=None, stop=None):
         opcodes = self.opcodes
         memory = self.memory
         registers = self.registers
         if start is not None:
-            registers[24] = start
+            registers[24] = start # PC
         pc = registers[24]
 
         if stop is None:
             opcodes[memory[pc]]()
         else:
             while True:
                 opcodes[memory[pc]]()
@@ -176,141 +176,165 @@
                 self.registers[rh] = value // 256
                 self.registers[rh + 1] = value % 256
             elif len(reg) == 2:
                 rh = REGISTERS[reg[0]]
                 self.registers[rh] = value // 256
                 self.registers[rh + 1] = value % 256
 
+    def accept_interrupt(self, registers, memory, prev_pc):
+        opcode = memory[prev_pc]
+        pc = registers[24]
+        if opcode == 0xFB or (opcode in (0xDD, 0xFD) and prev_pc == (pc - 1) % 65536):
+            return True
+        if self.imode == 2:
+            vaddr = 255 + 256 * registers[14]
+            iaddr = memory[vaddr] + 256 * memory[(vaddr + 1) % 65536]
+            registers[25] += 19 # T-states
+        else:
+            iaddr = 56
+            registers[25] += 13 # T-states
+        sp = (registers[12] - 2) % 65536
+        registers[12] = sp
+        if sp > 0x3FFF:
+            memory[sp] = pc % 256
+        sp = (sp + 1) % 65536
+        if sp > 0x3FFF:
+            memory[sp] = pc // 256
+        registers[15] = R1[registers[15]] # R
+        registers[24] = iaddr # PC
+        self.iff = 0
+        return False
+
     def prefix(self, opcodes, registers, memory):
         opcodes[memory[(registers[24] + 1) % 65536]]()
 
     def prefix2(self, opcodes, registers, memory):
         opcodes[memory[(registers[24] + 3) % 65536]]()
 
     def af_hl(self, registers, memory, af):
         # ADD A,(HL) / AND (HL) / CP (HL) / OR (HL) / SUB (HL) / XOR (HL)
         registers[:2] = af[registers[0]][memory[registers[7] + 256 * registers[6]]]
-        registers[15] = R1[registers[15]]
-        registers[25] += 7
-        registers[24] = (registers[24] + 1) % 65536
+        registers[15] = R1[registers[15]] # R
+        registers[25] += 7 # T-states
+        registers[24] = (registers[24] + 1) % 65536 # PC
 
     def af_n(self, registers, memory, af):
         # ADD A,n / AND n / CP n / OR n / SUB n / XOR n
         pcn = registers[24] + 1
         registers[:2] = af[registers[0]][memory[pcn % 65536]]
-        registers[15] = R1[registers[15]]
-        registers[25] += 7
-        registers[24] = (pcn + 1) % 65536
+        registers[15] = R1[registers[15]] # R
+        registers[25] += 7 # T-states
+        registers[24] = (pcn + 1) % 65536 # PC
 
     def af_r(self, registers, r_inc, timing, size, af, r):
-        # ADC A,A / ADD A,r / AND r / CP r / OR r / SBC A,A / SUB r / XOR r
-        # DAA / RLA / RLCA / RRA / RRCA
+        # ADD A,r / AND r / CP r / OR r / SUB r / XOR r
+        # CPL / DAA / RLA / RLCA / RRA / RRCA
         registers[:2] = af[registers[0]][registers[r]]
-        registers[15] = r_inc[registers[15]]
-        registers[25] += timing
-        registers[24] = (registers[24] + size) % 65536
+        registers[15] = r_inc[registers[15]] # R
+        registers[25] += timing # T-states
+        registers[24] = (registers[24] + size) % 65536 # PC
 
     def af_xy(self, registers, memory, af, xyh, xyl):
-        # ADD A,(IX/Y+d) / AND (IX/Y+d) / CP (IX/Y+d) / # OR (IX/Y+d)
+        # ADD A,(IX/Y+d) / AND (IX/Y+d) / CP (IX/Y+d) / OR (IX/Y+d)
         # SUB (IX/Y+d) / XOR (IX/Y+d)
         pcn = registers[24] + 3
         registers[:2] = af[registers[0]][memory[(registers[xyl] + 256 * registers[xyh] + OFFSETS[memory[(pcn - 1) % 65536]]) % 65536]]
-        registers[15] = R2[registers[15]]
-        registers[25] += 19
-        registers[24] = pcn % 65536
+        registers[15] = R2[registers[15]] # R
+        registers[25] += 19 # T-states
+        registers[24] = pcn % 65536 # PC
 
     def afc_hl(self, registers, memory, afc):
         # ADC/SBC A,(HL)
         registers[:2] = afc[registers[1] % 2][registers[0]][memory[registers[7] + 256 * registers[6]]]
-        registers[15] = R1[registers[15]]
-        registers[25] += 7
-        registers[24] = (registers[24] + 1) % 65536
+        registers[15] = R1[registers[15]] # R
+        registers[25] += 7 # T-states
+        registers[24] = (registers[24] + 1) % 65536 # PC
 
     def afc_n(self, registers, memory, afc):
         # ADC/SBC A,n
         pcn = registers[24] + 1
         registers[:2] = afc[registers[1] % 2][registers[0]][memory[pcn % 65536]]
-        registers[15] = R1[registers[15]]
-        registers[25] += 7
-        registers[24] = (pcn + 1) % 65536
+        registers[15] = R1[registers[15]] # R
+        registers[25] += 7 # T-states
+        registers[24] = (pcn + 1) % 65536 # PC
 
     def afc_r(self, registers, r_inc, timing, size, afc, r):
         # ADC/SBC A,r (r != A)
         registers[:2] = afc[registers[1] % 2][registers[0]][registers[r]]
-        registers[15] = r_inc[registers[15]]
-        registers[25] += timing
-        registers[24] = (registers[24] + size) % 65536
+        registers[15] = r_inc[registers[15]] # R
+        registers[25] += timing # T-states
+        registers[24] = (registers[24] + size) % 65536 # PC
 
     def afc_xy(self, registers, memory, afc, xyh, xyl):
         # ADC/SBC A,(IX/Y+d)
         pcn = registers[24] + 3
         registers[:2] = afc[registers[1] % 2][registers[0]][memory[(registers[xyl] + 256 * registers[xyh] + OFFSETS[memory[(pcn - 1) % 65536]]) % 65536]]
-        registers[15] = R2[registers[15]]
-        registers[25] += 19
-        registers[24] = pcn % 65536
+        registers[15] = R2[registers[15]] # R
+        registers[25] += 19 # T-states
+        registers[24] = pcn % 65536 # PC
 
     def f_hl(self, registers, memory, f):
         # RLC/RRC/SLA/SLL/SRA/SRL (HL)
         hl = registers[7] + 256 * registers[6]
         value, registers[1] = f[memory[hl]]
         if hl > 0x3FFF:
             memory[hl] = value
-        registers[15] = R2[registers[15]]
-        registers[25] += 15
-        registers[24] = (registers[24] + 2) % 65536
+        registers[15] = R2[registers[15]] # R
+        registers[25] += 15 # T-states
+        registers[24] = (registers[24] + 2) % 65536 # PC
 
     def f_r(self, registers, f, r):
         # RLC/RRC/SLA/SLL/SRA/SRL r
         registers[r], registers[1] = f[registers[r]]
-        registers[15] = R2[registers[15]]
-        registers[25] += 8
-        registers[24] = (registers[24] + 2) % 65536
+        registers[15] = R2[registers[15]] # R
+        registers[25] += 8 # T-states
+        registers[24] = (registers[24] + 2) % 65536 # PC
 
     def f_xy(self, registers, memory, f, xyh, xyl, dest=-1):
         # RLC/RRC/SLA/SLL/SRA/SRL (IX/Y+d)[,r]
         pcn = registers[24] + 4
         addr = (registers[xyl] + 256 * registers[xyh] + OFFSETS[memory[(pcn - 2) % 65536]]) % 65536
         value, registers[1] = f[memory[addr]]
         if addr > 0x3FFF:
             memory[addr] = value
         if dest >= 0:
             registers[dest] = value
-        registers[15] = R2[registers[15]]
-        registers[25] += 23
-        registers[24] = pcn % 65536
+        registers[15] = R2[registers[15]] # R
+        registers[25] += 23 # T-states
+        registers[24] = pcn % 65536 # PC
 
     def fc_hl(self, registers, memory, r_inc, timing, size, fc):
         # DEC/INC/RL/RR (HL)
         hl = registers[7] + 256 * registers[6]
         value, registers[1] = fc[registers[1] % 2][memory[hl]]
         if hl > 0x3FFF:
             memory[hl] = value
-        registers[15] = r_inc[registers[15]]
-        registers[25] += timing
-        registers[24] = (registers[24] + size) % 65536
+        registers[15] = r_inc[registers[15]] # R
+        registers[25] += timing # T-states
+        registers[24] = (registers[24] + size) % 65536 # PC
 
     def fc_r(self, registers, r_inc, timing, size, fc, r):
-        # DEC/INC/RL/RR r
+        # DEC/INC/RL/RR r / ADC A,A / SBC A,A
         registers[r], registers[1] = fc[registers[1] % 2][registers[r]]
-        registers[15] = r_inc[registers[15]]
-        registers[25] += timing
-        registers[24] = (registers[24] + size) % 65536
+        registers[15] = r_inc[registers[15]] # R
+        registers[25] += timing # T-states
+        registers[24] = (registers[24] + size) % 65536 # PC
 
     def fc_xy(self, registers, memory, size, fc, xyh, xyl, dest=-1):
         # DEC/INC/RL/RR (IX/Y+d)[,r]
         pc = registers[24]
         addr = (registers[xyl] + 256 * registers[xyh] + OFFSETS[memory[(pc + 2) % 65536]]) % 65536
         value, registers[1] = fc[registers[1] % 2][memory[addr]]
         if addr > 0x3FFF:
             memory[addr] = value
         if dest >= 0:
             registers[dest] = value
-        registers[15] = R2[registers[15]]
-        registers[25] += 23
-        registers[24] = (pc + size) % 65536
+        registers[15] = R2[registers[15]] # R
+        registers[25] += 23 # T-states
+        registers[24] = (pc + size) % 65536 # PC
 
     def adc_hl(self, registers, rh, rl):
         # ADC HL,BC/DE/HL/SP
         rr = registers[rl] + 256 * registers[rh]
         hl = registers[7] + 256 * registers[6]
         rr_c = rr + registers[1] % 2
         result = hl + rr_c
@@ -329,17 +353,17 @@
             # differs from the sign of the result
             f += 0x04 # .....P..
 
         h = result // 256
         registers[1] = f + (h & 0xA8)
         registers[7] = result % 256
         registers[6] = h
-        registers[15] = R2[registers[15]]
-        registers[25] += 15
-        registers[24] = (registers[24] + 2) % 65536
+        registers[15] = R2[registers[15]] # R
+        registers[25] += 15 # T-states
+        registers[24] = (registers[24] + 2) % 65536 # PC
 
     def add_rr(self, registers, r_inc, timing, size, ah, al, rh, rl):
         # ADD HL/IX/IY,BC/DE/HL/SP/IX/IY
         addend_v = registers[rl] + 256 * registers[rh]
         augend_v = registers[al] + 256 * registers[ah]
         result = augend_v + addend_v
 
@@ -351,66 +375,68 @@
         if (augend_v % 4096) + (addend_v % 4096) > 0x0FFF:
             f += 0x10 # ...H....
 
         result_hi = result // 256
         registers[1] = f + (result_hi & 0x28)
         registers[al] = result % 256
         registers[ah] = result_hi
-        registers[15] = r_inc[registers[15]]
-        registers[25] += timing
-        registers[24] = (registers[24] + size) % 65536
+        registers[15] = r_inc[registers[15]] # R
+        registers[25] += timing # T-states
+        registers[24] = (registers[24] + size) % 65536 # PC
 
     def bit_hl(self, registers, memory, bit, b):
         # BIT n,(HL)
         registers[1] = bit[registers[1] % 2][b][memory[registers[7] + 256 * registers[6]]]
-        registers[15] = R2[registers[15]]
-        registers[25] += 12
-        registers[24] = (registers[24] + 2) % 65536
+        registers[15] = R2[registers[15]] # R
+        registers[25] += 12 # T-states
+        registers[24] = (registers[24] + 2) % 65536 # PC
 
     def bit_r(self, registers, bit, b, reg):
         # BIT n,r
         registers[1] = bit[registers[1] % 2][b][registers[reg]]
-        registers[15] = R2[registers[15]]
-        registers[25] += 8
-        registers[24] = (registers[24] + 2) % 65536
+        registers[15] = R2[registers[15]] # R
+        registers[25] += 8 # T-states
+        registers[24] = (registers[24] + 2) % 65536 # PC
 
     def bit_xy(self, registers, memory, bit, b, xyh, xyl):
         # BIT n,(IX/Y+d)
         xy = (registers[xyl] + 256 * registers[xyh] + OFFSETS[memory[(registers[24] + 2) % 65536]]) % 65536
         registers[1] = (bit[registers[1] % 2][b][memory[xy]] & 0xD7) + ((xy // 256) & 0x28)
-        registers[15] = R2[registers[15]]
-        registers[25] += 20
-        registers[24] = (registers[24] + 4) % 65536
+        registers[15] = R2[registers[15]] # R
+        registers[25] += 20 # T-states
+        registers[24] = (registers[24] + 4) % 65536 # PC
 
     def call(self, registers, memory, c_and, c_val):
+        # CALL nn / CALL cc,nn
         if c_and and registers[1] & c_and == c_val:
-            registers[25] += 10
-            registers[24] = (registers[24] + 3) % 65536
+            registers[25] += 10 # T-states
+            registers[24] = (registers[24] + 3) % 65536 # PC
         else:
             pc = registers[24]
+            registers[24] = memory[(pc + 1) % 65536] + 256 * memory[(pc + 2) % 65536] # PC
             ret_addr = (pc + 3) % 65536
             sp = (registers[12] - 2) % 65536
             registers[12] = sp
             if sp > 0x3FFF:
                 memory[sp] = ret_addr % 256
             sp = (sp + 1) % 65536
             if sp > 0x3FFF:
                 memory[sp] = ret_addr // 256
-            registers[25] += 17
-            registers[24] = memory[(pc + 1) % 65536] + 256 * memory[(pc + 2) % 65536]
-        registers[15] = R1[registers[15]]
+            registers[25] += 17 # T-states
+        registers[15] = R1[registers[15]] # R
 
     def cf(self, registers, cf):
+        # CCF / SCF
         registers[1] = cf[registers[1]][registers[0]]
-        registers[15] = R1[registers[15]]
-        registers[25] += 4
-        registers[24] = (registers[24] + 1) % 65536
+        registers[15] = R1[registers[15]] # R
+        registers[25] += 4 # T-states
+        registers[24] = (registers[24] + 1) % 65536 # PC
 
     def cpi(self, registers, memory, inc, repeat):
-        # CPI, CPD, CPIR, CPDR
+        # CPI / CPD / CPIR / CPDR
         hl = registers[7] + 256 * registers[6]
         bc = registers[3] + 256 * registers[2]
         a = registers[0]
         value = memory[hl]
         hl = (hl + inc) % 65536
         bc = (bc - 1) % 65536
         registers[7] = hl % 256
@@ -419,137 +445,146 @@
         registers[2] = bc // 256
 
         cp = a - value
         hf = a % 16 < value % 16
         f = (cp & 0x80) + hf * 0x10 + 0x02 + (registers[1] % 2) # S..H..NC
         if repeat and cp and bc:
             registers[1] = f + ((registers[24] // 256) & 0x28) + 0x04 # .Z5.3P..
-            registers[25] += 21
+            registers[25] += 21 # T-states
         else:
             n = cp - hf
             registers[1] = f + (cp == 0) * 0x40 + (n & 0x02) * 16 + (n & 0x08) + (bc > 0) * 0x04 # .Z5.3P..
-            registers[25] += 16
-            registers[24] = (registers[24] + 2) % 65536
-        registers[15] = R2[registers[15]]
-
-    def di_ei(self, registers, iff2):
-        self.iff2 = iff2
-        registers[15] = R1[registers[15]]
-        registers[25] += 4
-        registers[24] = (registers[24] + 1) % 65536
+            registers[25] += 16 # T-states
+            registers[24] = (registers[24] + 2) % 65536 # PC
+        registers[15] = R2[registers[15]] # R
+
+    def di_ei(self, registers, iff):
+        # DI / EI
+        self.iff = iff
+        registers[15] = R1[registers[15]] # R
+        registers[25] += 4 # T-states
+        registers[24] = (registers[24] + 1) % 65536 # PC
 
     def djnz(self, registers, memory):
+        # DJNZ nn
         b = (registers[2] - 1) % 256
         registers[2] = b
         if b:
-            registers[25] += 13
+            registers[25] += 13 # T-states
             pc = registers[24]
-            registers[24] = (pc + JR_OFFSETS[memory[(pc + 1) % 65536]]) % 65536
+            registers[24] = (pc + JR_OFFSETS[memory[(pc + 1) % 65536]]) % 65536 # PC
         else:
-            registers[25] += 8
-            registers[24] = (registers[24] + 2) % 65536
-        registers[15] = R1[registers[15]]
+            registers[25] += 8 # T-states
+            registers[24] = (registers[24] + 2) % 65536 # PC
+        registers[15] = R1[registers[15]] # R
 
     def djnz_fast(self, registers, memory):
         if memory[(registers[24] + 1) % 65536] == 0xFE:
             b = (registers[2] - 1) % 256
             registers[2] = 0
             r = registers[15]
-            registers[15] = (r & 0x80) + ((r + b + 1) % 128)
-            registers[25] += b * 13 + 8
-            registers[24] = (registers[24] + 2) % 65536
+            registers[15] = (r & 0x80) + ((r + b + 1) % 128) # R
+            registers[25] += b * 13 + 8 # T-states
+            registers[24] = (registers[24] + 2) % 65536 # PC
         else:
             self.djnz(registers, memory)
 
     def ex_af(self, registers):
+        # EX AF,AF'
         registers[0], registers[16] = registers[16], registers[0]
         registers[1], registers[17] = registers[17], registers[1]
-        registers[15] = R1[registers[15]]
-        registers[25] += 4
-        registers[24] = (registers[24] + 1) % 65536
+        registers[15] = R1[registers[15]] # R
+        registers[25] += 4 # T-states
+        registers[24] = (registers[24] + 1) % 65536 # PC
 
     def ex_de_hl(self, registers):
+        # EX DE,HL
         registers[4], registers[6] = registers[6], registers[4]
         registers[5], registers[7] = registers[7], registers[5]
-        registers[15] = R1[registers[15]]
-        registers[25] += 4
-        registers[24] = (registers[24] + 1) % 65536
+        registers[15] = R1[registers[15]] # R
+        registers[25] += 4 # T-states
+        registers[24] = (registers[24] + 1) % 65536 # PC
 
     def ex_sp(self, registers, memory, r_inc, timing, size, rh, rl):
         # EX (SP),HL/IX/IY
         sp = registers[12]
         sp1 = memory[sp]
         if sp > 0x3FFF:
             memory[sp] = registers[rl]
         sp = (sp + 1) % 65536
         sp2 = memory[sp]
         if sp > 0x3FFF:
             memory[sp] = registers[rh]
         registers[rl] = sp1
         registers[rh] = sp2
-        registers[15] = r_inc[registers[15]]
-        registers[25] += timing
-        registers[24] = (registers[24] + size) % 65536
+        registers[15] = r_inc[registers[15]] # R
+        registers[25] += timing # T-states
+        registers[24] = (registers[24] + size) % 65536 # PC
 
     def exx(self, registers):
+        # EXX
         registers[2:8], registers[18:24] = registers[18:24], registers[2:8]
-        registers[15] = R1[registers[15]]
-        registers[25] += 4
-        registers[24] = (registers[24] + 1) % 65536
+        registers[15] = R1[registers[15]] # R
+        registers[25] += 4 # T-states
+        registers[24] = (registers[24] + 1) % 65536 # PC
 
     def halt(self, registers):
-        if self.iff2:
+        # HALT
+        if self.iff:
             t = registers[25]
-            if (t + 4) % FRAME_DURATION < t % FRAME_DURATION:
-                registers[24] = (registers[24] + 1) % 65536
-        registers[15] = R1[registers[15]]
-        registers[25] += 4
+            if (t + 4) // FRAME_DURATION > t // FRAME_DURATION:
+                registers[24] = (registers[24] + 1) % 65536 # PC
+        registers[15] = R1[registers[15]] # R
+        registers[25] += 4 # T-states
 
     def im(self, registers, mode):
+        # IM 0/1/2
         self.imode = mode
-        registers[15] = R2[registers[15]]
-        registers[25] += 8
-        registers[24] = (registers[24] + 2) % 65536
+        registers[15] = R2[registers[15]] # R
+        registers[25] += 8 # T-states
+        registers[24] = (registers[24] + 2) % 65536 # PC
 
     def in_a(self, registers, memory):
+        # IN A,(n)
         pcn = registers[24] + 1
         if self.in_tracer:
             registers[0] = self.in_tracer(memory[pcn % 65536] + 256 * registers[0])
         else:
-            registers[0] = 191
-        registers[15] = R1[registers[15]]
-        registers[25] += 11
-        registers[24] = (pcn + 1) % 65536
+            registers[0] = 255
+        registers[15] = R1[registers[15]] # R
+        registers[25] += 11 # T-states
+        registers[24] = (pcn + 1) % 65536 # PC
 
     def in_c(self, registers, reg, sz53p):
+        # IN r,(C)
         if self.in_tracer:
             value = self.in_tracer(registers[3] + 256 * registers[2])
         else:
-            value = 191
+            value = 255
         if reg != 1:
             registers[reg] = value
         registers[1] = sz53p[value] + (registers[1] % 2)
-        registers[15] = R2[registers[15]]
-        registers[25] += 12
-        registers[24] = (registers[24] + 2) % 65536
+        registers[15] = R2[registers[15]] # R
+        registers[25] += 12 # T-states
+        registers[24] = (registers[24] + 2) % 65536 # PC
 
     def inc_dec_rr(self, registers, r_inc, timing, size, inc, rh, rl):
         # INC/DEC BC/DE/HL/SP/IX/IY
         if rl == 12:
             registers[12] = (registers[12] + inc) % 65536
         else:
             value = (registers[rl] + 256 * registers[rh] + inc) % 65536
             registers[rh] = value // 256
             registers[rl] = value % 256
-        registers[15] = r_inc[registers[15]]
-        registers[25] += timing
-        registers[24] = (registers[24] + size) % 65536
+        registers[15] = r_inc[registers[15]] # R
+        registers[25] += timing # T-states
+        registers[24] = (registers[24] + size) % 65536 # PC
 
     def ini(self, registers, memory, inc, repeat, parity):
-        # INI, IND, INIR, INDR
+        # INI / IND / INIR / INDR
         hl = registers[7] + 256 * registers[6]
         b = registers[2]
         c = registers[3]
 
         if self.in_tracer:
             value = self.in_tracer(c + 256 * b)
         else:
@@ -573,163 +608,167 @@
                 else:
                     h = (b % 16 == 15) * 0x10
                     p = parity[(j % 8) ^ b ^ ((b + 1) % 8)]
             else:
                 h = 0
                 p = parity[(j % 8) ^ b ^ (b % 8)]
             registers[1] = (b & 0x80) + ((registers[24] // 256) & 0x28) + h + p + n + c
-            registers[25] += 21
+            registers[25] += 21 # T-states
         else:
             registers[1] = (b & 0xA8) + (b == 0) * 0x40 + c * 0x11 + parity[(j % 8) ^ b] + n
-            registers[24] = (registers[24] + 2) % 65536
-            registers[25] += 16
-        registers[15] = R2[registers[15]]
+            registers[24] = (registers[24] + 2) % 65536 # PC
+            registers[25] += 16 # T-states
+        registers[15] = R2[registers[15]] # R
 
     def jp(self, registers, memory, c_and, c_val):
+        # JP nn / JP cc,nn
         if registers[1] & c_and == c_val:
-            registers[24] = memory[(registers[24] + 1) % 65536] + 256 * memory[(registers[24] + 2) % 65536]
+            registers[24] = memory[(registers[24] + 1) % 65536] + 256 * memory[(registers[24] + 2) % 65536] # PC
         else:
-            registers[24] = (registers[24] + 3) % 65536
-        registers[15] = R1[registers[15]]
-        registers[25] += 10
+            registers[24] = (registers[24] + 3) % 65536 # PC
+        registers[15] = R1[registers[15]] # R
+        registers[25] += 10 # T-states
 
     def jp_rr(self, registers, r_inc, timing, rh, rl):
         # JP (HL/IX/IY)
-        registers[15] = r_inc[registers[15]]
-        registers[25] += timing
-        registers[24] = registers[rl] + 256 * registers[rh]
+        registers[15] = r_inc[registers[15]] # R
+        registers[25] += timing # T-states
+        registers[24] = registers[rl] + 256 * registers[rh] # PC
 
     def jr(self, registers, memory, c_and, c_val):
+        # JR nn / JR cc,nn
         if registers[1] & c_and == c_val:
-            registers[25] += 12
+            registers[25] += 12 # T-states
             pc = registers[24]
-            registers[24] = (pc + JR_OFFSETS[memory[(pc + 1) % 65536]]) % 65536
+            registers[24] = (pc + JR_OFFSETS[memory[(pc + 1) % 65536]]) % 65536 # PC
         else:
-            registers[25] += 7
-            registers[24] = (registers[24] + 2) % 65536
-        registers[15] = R1[registers[15]]
+            registers[25] += 7 # T-states
+            registers[24] = (registers[24] + 2) % 65536 # PC
+        registers[15] = R1[registers[15]] # R
 
     def ld_a_ir(self, registers, r):
         # LD A,I/R
+        registers[15] = R2[registers[15]] # R
         a = registers[r]
         registers[0] = a
-        registers[1] = (a & 0xA8) + (a == 0) * 0x40 + self.iff2 * 0x04 + (registers[1] % 2)
-        registers[15] = R2[registers[15]]
-        registers[25] += 9
-        registers[24] = (registers[24] + 2) % 65536
+        registers[1] = (a & 0xA8) + (a == 0) * 0x40 + self.iff * 0x04 + (registers[1] % 2)
+        registers[25] += 9 # T-states
+        registers[24] = (registers[24] + 2) % 65536 # PC
 
     def ld_hl_n(self, registers, memory):
         # LD (HL),n
         pcn = registers[24] + 1
         addr = registers[7] + 256 * registers[6]
         if addr > 0x3FFF:
             memory[addr] = memory[pcn % 65536]
-        registers[15] = R1[registers[15]]
-        registers[25] += 10
-        registers[24] = (pcn + 1) % 65536
+        registers[15] = R1[registers[15]] # R
+        registers[25] += 10 # T-states
+        registers[24] = (pcn + 1) % 65536 # PC
 
     def ld_r_n(self, registers, memory, r_inc, timing, size, r):
+        # LD r,n
         end = registers[24] + size
         registers[r] = memory[(end - 1) % 65536]
-        registers[15] = r_inc[registers[15]]
-        registers[25] += timing
-        registers[24] = end % 65536
+        registers[15] = r_inc[registers[15]] # R
+        registers[25] += timing # T-states
+        registers[24] = end % 65536 # PC
 
     def ld_r_r(self, registers, r_inc, timing, size, r1, r2):
+        # LD r,r
+        registers[15] = r_inc[registers[15]] # R
         registers[r1] = registers[r2]
-        registers[15] = r_inc[registers[15]]
-        registers[25] += timing
-        registers[24] = (registers[24] + size) % 65536
+        registers[25] += timing # T-states
+        registers[24] = (registers[24] + size) % 65536 # PC
 
     def ld_r_rr(self, registers, memory, r, rh, rl):
         # LD r,(HL/DE/BC)
         registers[r] = memory[registers[rl] + 256 * registers[rh]]
-        registers[15] = R1[registers[15]]
-        registers[25] += 7
-        registers[24] = (registers[24] + 1) % 65536
+        registers[15] = R1[registers[15]] # R
+        registers[25] += 7 # T-states
+        registers[24] = (registers[24] + 1) % 65536 # PC
 
     def ld_rr_r(self, registers, memory, rh, rl, r):
         # LD (HL/DE/BC),r
         addr = registers[rl] + 256 * registers[rh]
         if addr > 0x3FFF:
             memory[addr] = registers[r]
-        registers[15] = R1[registers[15]]
-        registers[25] += 7
-        registers[24] = (registers[24] + 1) % 65536
+        registers[15] = R1[registers[15]] # R
+        registers[25] += 7 # T-states
+        registers[24] = (registers[24] + 1) % 65536 # PC
 
     def ld_r_xy(self, registers, memory, r, xyh, xyl):
         # LD r,(IX/Y+d)
         pcn = registers[24] + 3
         registers[r] = memory[(registers[xyl] + 256 * registers[xyh] + OFFSETS[memory[(pcn - 1) % 65536]]) % 65536]
-        registers[15] = R2[registers[15]]
-        registers[25] += 19
-        registers[24] = pcn % 65536
+        registers[15] = R2[registers[15]] # R
+        registers[25] += 19 # T-states
+        registers[24] = pcn % 65536 # PC
 
     def ld_xy_n(self, registers, memory, xyh, xyl):
         # LD (IX/Y+d),n
         pcn = registers[24] + 4
         addr = (registers[xyl] + 256 * registers[xyh] + OFFSETS[memory[(pcn - 2) % 65536]]) % 65536
         if addr > 0x3FFF:
             memory[addr] = memory[(pcn - 1) % 65536]
-        registers[15] = R2[registers[15]]
-        registers[25] += 19
-        registers[24] = pcn % 65536
+        registers[15] = R2[registers[15]] # R
+        registers[25] += 19 # T-states
+        registers[24] = pcn % 65536 # PC
 
     def ld_xy_r(self, registers, memory, xyh, xyl, r):
         # LD (IX/Y+d),r
         pcn = registers[24] + 3
         addr = (registers[xyl] + 256 * registers[xyh] + OFFSETS[memory[(pcn - 1) % 65536]]) % 65536
         if addr > 0x3FFF:
             memory[addr] = registers[r]
-        registers[15] = R2[registers[15]]
-        registers[25] += 19
-        registers[24] = pcn % 65536
+        registers[15] = R2[registers[15]] # R
+        registers[25] += 19 # T-states
+        registers[24] = pcn % 65536 # PC
 
     def ld_rr_nn(self, registers, memory, r_inc, timing, size, rh, rl):
         # LD BC/DE/HL/SP/IX/IY,nn
         end = registers[24] + size
         if rl == 12:
             registers[12] = memory[(end - 2) % 65536] + 256 * memory[(end - 1) % 65536]
         else:
             registers[rl] = memory[(end - 2) % 65536]
             registers[rh] = memory[(end - 1) % 65536]
-        registers[15] = r_inc[registers[15]]
-        registers[25] += timing
-        registers[24] = end % 65536
+        registers[15] = r_inc[registers[15]] # R
+        registers[25] += timing # T-states
+        registers[24] = end % 65536 # PC
 
     def ld_a_m(self, registers, memory):
         # LD A,(nn)
         pcn = registers[24] + 1
         registers[0] = memory[memory[pcn % 65536] + 256 * memory[(pcn + 1) % 65536]]
-        registers[15] = R1[registers[15]]
-        registers[25] += 13
-        registers[24] = (pcn + 2) % 65536
+        registers[15] = R1[registers[15]] # R
+        registers[25] += 13 # T-states
+        registers[24] = (pcn + 2) % 65536 # PC
 
     def ld_m_a(self, registers, memory):
         # LD (nn),A
         pcn = registers[24] + 1
         addr = memory[pcn % 65536] + 256 * memory[(pcn + 1) % 65536]
         if addr > 0x3FFF:
             memory[addr] = registers[0]
-        registers[15] = R1[registers[15]]
-        registers[25] += 13
-        registers[24] = (pcn + 2) % 65536
+        registers[15] = R1[registers[15]] # R
+        registers[25] += 13 # T-states
+        registers[24] = (pcn + 2) % 65536 # PC
 
     def ld_rr_mm(self, registers, memory, r_inc, timing, size, rh, rl):
         # LD BC/DE/HL/SP/IX/IY,(nn)
         end = registers[24] + size
         addr = memory[(end - 2) % 65536] + 256 * memory[(end - 1) % 65536]
         if rl == 12:
             registers[12] = memory[addr] + 256 * memory[(addr + 1) % 65536]
         else:
             registers[rl] = memory[addr]
             registers[rh] = memory[(addr + 1) % 65536]
-        registers[15] = r_inc[registers[15]]
-        registers[25] += timing
-        registers[24] = end % 65536
+        registers[15] = r_inc[registers[15]] # R
+        registers[25] += timing # T-states
+        registers[24] = end % 65536 # PC
 
     def ld_mm_rr(self, registers, memory, r_inc, timing, size, rh, rl):
         # LD (nn),BC/DE/HL/SP/IX/IY
         end = registers[24] + size
         addr = memory[(end - 2) % 65536] + 256 * memory[(end - 1) % 65536]
         if rl == 12:
             sp = registers[12]
@@ -740,20 +779,20 @@
                 memory[addr] = sp // 256
         else:
             if addr > 0x3FFF:
                 memory[addr] = registers[rl]
             addr = (addr + 1) % 65536
             if addr > 0x3FFF:
                 memory[addr] = registers[rh]
-        registers[15] = r_inc[registers[15]]
-        registers[25] += timing
-        registers[24] = end % 65536
+        registers[15] = r_inc[registers[15]] # R
+        registers[25] += timing # T-states
+        registers[24] = end % 65536 # PC
 
     def ldi(self, registers, memory, inc, repeat):
-        # LDI, LDD, LDIR, LDDR
+        # LDI / LDD / LDIR / LDDR
         hl = registers[7] + 256 * registers[6]
         de = registers[5] + 256 * registers[4]
         bc = registers[3] + 256 * registers[2]
 
         at_hl = memory[hl]
         if de > 0x3FFF:
             memory[de] = at_hl
@@ -766,21 +805,21 @@
         registers[5] = de % 256
         registers[4] = de // 256
         registers[3] = bc % 256
         registers[2] = bc // 256
 
         if repeat and bc:
             registers[1] = (registers[1] & 0xC1) + ((registers[24] // 256) & 0x28) + 0x04
-            registers[25] += 21
+            registers[25] += 21 # T-states
         else:
             n = registers[0] + at_hl
             registers[1] = (registers[1] & 0xC1) + (n & 0x02) * 16 + (n & 0x08) + (bc > 0) * 0x04
-            registers[25] += 16
-            registers[24] = (registers[24] + 2) % 65536
-        registers[15] = R2[registers[15]]
+            registers[25] += 16 # T-states
+            registers[24] = (registers[24] + 2) % 65536 # PC
+        registers[15] = R2[registers[15]] # R
 
     def ldir_fast(self, registers, memory, inc):
         de = registers[5] + 256 * registers[4]
         bc = registers[3] + 256 * registers[2]
         hl = registers[7] + 256 * registers[6]
         count = 0
         repeat = True
@@ -793,62 +832,66 @@
             de = (de + inc) % 65536
             hl = (hl + inc) % 65536
             count += 1
         registers[3], registers[2] = bc % 256, bc // 256
         registers[5], registers[4] = de % 256, de // 256
         registers[7], registers[6] = hl % 256, hl // 256
         r = registers[15]
-        registers[15] = (r & 0x80) + ((r + 2 * count) % 128)
+        registers[15] = (r & 0x80) + ((r + 2 * count) % 128) # R
         if bc:
             registers[1] = (registers[1] & 0xC1) + ((registers[24] // 256) & 0x28) + 0x04
         else:
             n = registers[0] + memory[(hl - inc) % 65536]
             registers[1] = (registers[1] & 0xC1) + (n & 0x02) * 16 + (n & 0x08)
-            registers[24] = (registers[24] + 2) % 65536
-        registers[25] += 21 * count - 5
+            registers[24] = (registers[24] + 2) % 65536 # PC
+        registers[25] += 21 * count - 5 # T-states
 
     def ld_sp_rr(self, registers, r_inc, timing, size, rh, rl):
         # LD SP,HL/IX/IY
         registers[12] = registers[rl] + 256 * registers[rh]
-        registers[15] = r_inc[registers[15]]
-        registers[25] += timing
-        registers[24] = (registers[24] + size) % 65536
+        registers[15] = r_inc[registers[15]] # R
+        registers[25] += timing # T-states
+        registers[24] = (registers[24] + size) % 65536 # PC
 
     def neg(self, registers, neg):
+        # NEG
         registers[:2] = neg[registers[0]]
-        registers[15] = R2[registers[15]]
-        registers[25] += 8
-        registers[24] = (registers[24] + 2) % 65536
+        registers[15] = R2[registers[15]] # R
+        registers[25] += 8 # T-states
+        registers[24] = (registers[24] + 2) % 65536 # PC
 
     def nop(self, registers, r_inc, timing, size):
-        registers[15] = r_inc[registers[15]]
-        registers[25] += timing
-        registers[24] = (registers[24] + size) % 65536
+        # NOP and equivalents
+        registers[15] = r_inc[registers[15]] # R
+        registers[25] += timing # T-states
+        registers[24] = (registers[24] + size) % 65536 # PC
 
     def out_a(self, registers, memory):
+        # OUT (n),A
         pcn = registers[24] + 1
         if self.out_tracer:
             a = registers[0]
             self.out_tracer(memory[pcn % 65536] + 256 * a, a)
-        registers[15] = R1[registers[15]]
-        registers[25] += 11
-        registers[24] = (pcn + 1) % 65536
+        registers[15] = R1[registers[15]] # R
+        registers[25] += 11 # T-states
+        registers[24] = (pcn + 1) % 65536 # PC
 
     def out_c(self, registers, reg):
+        # OUT (C),r/0
         if self.out_tracer:
             if reg >= 0:
                 self.out_tracer(registers[3] + 256 * registers[2], registers[reg])
             else:
                 self.out_tracer(registers[3] + 256 * registers[2], 0)
-        registers[15] = R2[registers[15]]
-        registers[25] += 12
-        registers[24] = (registers[24] + 2) % 65536
+        registers[15] = R2[registers[15]] # R
+        registers[25] += 12 # T-states
+        registers[24] = (registers[24] + 2) % 65536 # PC
 
     def outi(self, registers, memory, inc, repeat, parity):
-        # OUTI, OUTD, OTIR, OTDR
+        # OUTI / OUTD / OTIR / OTDR
         hl = registers[7] + 256 * registers[6]
         b = (registers[2] - 1) % 256
 
         value = memory[hl]
         if self.out_tracer:
             self.out_tracer(registers[3] + 256 * b, value)
         hl = (hl + inc) % 65536
@@ -868,132 +911,137 @@
                 else:
                     h = (b % 16 == 15) * 0x10
                     p = parity[(j % 8) ^ b ^ ((b + 1) % 8)]
             else:
                 h = 0
                 p = parity[(j % 8) ^ b ^ (b % 8)]
             registers[1] = (b & 0x80) + ((registers[24] // 256) & 0x28) + h + p + n + c
-            registers[25] += 21
+            registers[25] += 21 # T-states
         else:
             registers[1] = (b & 0xA8) + (b == 0) * 0x40 + c * 0x11 + parity[(j % 8) ^ b] + n
-            registers[24] = (registers[24] + 2) % 65536
-            registers[25] += 16
-        registers[15] = R2[registers[15]]
+            registers[24] = (registers[24] + 2) % 65536 # PC
+            registers[25] += 16 # T-states
+        registers[15] = R2[registers[15]] # R
 
     def pop(self, registers, memory, r_inc, timing, size, rh, rl):
         # POP AF/BC/DE/HL/IX/IY
         sp = registers[12]
         registers[12] = (sp + 2) % 65536
         registers[rl] = memory[sp]
         registers[rh] = memory[(sp + 1) % 65536]
-        registers[15] = r_inc[registers[15]]
-        registers[25] += timing
-        registers[24] = (registers[24] + size) % 65536
+        registers[15] = r_inc[registers[15]] # R
+        registers[25] += timing # T-states
+        registers[24] = (registers[24] + size) % 65536 # PC
 
     def push(self, registers, memory, r_inc, timing, size, rh, rl):
         # PUSH AF/BC/DE/HL/IX/IY
         sp = (registers[12] - 2) % 65536
         registers[12] = sp
         if sp > 0x3FFF:
             memory[sp] = registers[rl]
         sp = (sp + 1) % 65536
         if sp > 0x3FFF:
             memory[sp] = registers[rh]
-        registers[15] = r_inc[registers[15]]
-        registers[25] += timing
-        registers[24] = (registers[24] + size) % 65536
+        registers[15] = r_inc[registers[15]] # R
+        registers[25] += timing # T-states
+        registers[24] = (registers[24] + size) % 65536 # PC
 
     def res_hl(self, registers, memory, bit):
         # RES n,(HL)
         addr = registers[7] + 256 * registers[6]
         if addr > 0x3FFF:
             memory[addr] &= bit
-        registers[15] = R2[registers[15]]
-        registers[25] += 15
-        registers[24] = (registers[24] + 2) % 65536
+        registers[15] = R2[registers[15]] # R
+        registers[25] += 15 # T-states
+        registers[24] = (registers[24] + 2) % 65536 # PC
 
     def res_r(self, registers, bit, reg):
         # RES n,r
         registers[reg] &= bit
-        registers[15] = R2[registers[15]]
-        registers[25] += 8
-        registers[24] = (registers[24] + 2) % 65536
+        registers[15] = R2[registers[15]] # R
+        registers[25] += 8 # T-states
+        registers[24] = (registers[24] + 2) % 65536 # PC
 
     def res_xy(self, registers, memory, bit, xyh, xyl, dest=-1):
         # RES n,(IX/Y+d)
         addr = (registers[xyl] + 256 * registers[xyh] + OFFSETS[memory[(registers[24] + 2) % 65536]]) % 65536
         value = memory[addr] & bit
         if addr > 0x3FFF:
             memory[addr] = value
         if dest >= 0:
             registers[dest] = value
-        registers[15] = R2[registers[15]]
-        registers[25] += 23
-        registers[24] = (registers[24] + 4) % 65536
+        registers[15] = R2[registers[15]] # R
+        registers[25] += 23 # T-states
+        registers[24] = (registers[24] + 4) % 65536 # PC
 
     def ret(self, registers, memory, c_and, c_val):
+        # RET / RET cc
         if c_and:
             if registers[1] & c_and == c_val:
-                registers[25] += 5
-                registers[24] = (registers[24] + 1) % 65536
+                registers[25] += 5 # T-states
+                registers[24] = (registers[24] + 1) % 65536 # PC
             else:
-                registers[25] += 11
+                registers[25] += 11 # T-states
                 sp = registers[12]
                 registers[12] = (sp + 2) % 65536
-                registers[24] = memory[sp] + 256 * memory[(sp + 1) % 65536]
+                registers[24] = memory[sp] + 256 * memory[(sp + 1) % 65536] # PC
         else:
-            registers[25] += 10
+            registers[25] += 10 # T-states
             sp = registers[12]
             registers[12] = (sp + 2) % 65536
-            registers[24] = memory[sp] + 256 * memory[(sp + 1) % 65536]
-        registers[15] = R1[registers[15]]
+            registers[24] = memory[sp] + 256 * memory[(sp + 1) % 65536] # PC
+        registers[15] = R1[registers[15]] # R
 
     def reti(self, registers, memory):
-        registers[15] = R2[registers[15]]
-        registers[25] += 14
+        # RETI / RETN
+        registers[15] = R2[registers[15]] # R
+        registers[25] += 14 # T-states
         sp = registers[12]
         registers[12] = (sp + 2) % 65536
-        registers[24] = memory[sp] + 256 * memory[(sp + 1) % 65536]
+        registers[24] = memory[sp] + 256 * memory[(sp + 1) % 65536] # PC
 
     def rld(self, registers, memory, sz53p):
+        # RLD
         hl = registers[7] + 256 * registers[6]
         a = registers[0]
         at_hl = memory[hl]
         if hl > 0x3FFF:
             memory[hl] = ((at_hl * 16) % 256) + (a % 16)
         a_out = registers[0] = (a & 240) + at_hl // 16
         registers[1] = sz53p[a_out] + (registers[1] % 2)
-        registers[15] = R2[registers[15]]
-        registers[25] += 18
-        registers[24] = (registers[24] + 2) % 65536
+        registers[15] = R2[registers[15]] # R
+        registers[25] += 18 # T-states
+        registers[24] = (registers[24] + 2) % 65536 # PC
 
     def rrd(self, registers, memory, sz53p):
+        # RRD
         hl = registers[7] + 256 * registers[6]
         a = registers[0]
         at_hl = memory[hl]
         if hl > 0x3FFF:
             memory[hl] = ((a * 16) % 256) + (at_hl // 16)
         a_out = registers[0] = (a & 240) + (at_hl % 16)
         registers[1] = sz53p[a_out] + (registers[1] % 2)
-        registers[15] = R2[registers[15]]
-        registers[25] += 18
-        registers[24] = (registers[24] + 2) % 65536
+        registers[15] = R2[registers[15]] # R
+        registers[25] += 18 # T-states
+        registers[24] = (registers[24] + 2) % 65536 # PC
 
     def rst(self, registers, memory, addr):
+        # RST n
         sp = (registers[12] - 2) % 65536
         registers[12] = sp
         ret_addr = (registers[24] + 1) % 65536
         if sp > 0x3FFF:
             memory[sp] = ret_addr % 256
         sp = (sp + 1) % 65536
         if sp > 0x3FFF:
             memory[sp] = ret_addr // 256
-        registers[15] = R1[registers[15]]
-        registers[25] += 11
-        registers[24] = addr
+        registers[15] = R1[registers[15]] # R
+        registers[25] += 11 # T-states
+        registers[24] = addr # PC
 
     def sbc_hl(self, registers, rh, rl):
         # SBC HL,BC/DE/HL/SP
         rr = registers[rl] + 256 * registers[rh]
         hl = registers[7] + 256 * registers[6]
         rr_c = rr + (registers[1] % 2)
         result = (hl - rr_c) % 65536
@@ -1011,45 +1059,45 @@
             # minuend's sign differs from the sign of the result
             f += 0x04 # .....P..
 
         h = result // 256
         registers[1] = f + (h & 0xA8)
         registers[7] = result % 256
         registers[6] = h
-        registers[15] = R2[registers[15]]
-        registers[25] += 15
-        registers[24] = (registers[24] + 2) % 65536
+        registers[15] = R2[registers[15]] # R
+        registers[25] += 15 # T-states
+        registers[24] = (registers[24] + 2) % 65536 # PC
 
     def set_hl(self, registers, memory, bit):
         # SET n,(HL)
         addr = registers[7] + 256 * registers[6]
         if addr > 0x3FFF:
             memory[addr] |= bit
-        registers[15] = R2[registers[15]]
-        registers[25] += 15
-        registers[24] = (registers[24] + 2) % 65536
+        registers[15] = R2[registers[15]] # R
+        registers[25] += 15 # T-states
+        registers[24] = (registers[24] + 2) % 65536 # PC
 
     def set_r(self, registers, bit, reg):
         # SET n,r
         registers[reg] |= bit
-        registers[15] = R2[registers[15]]
-        registers[25] += 8
-        registers[24] = (registers[24] + 2) % 65536
+        registers[15] = R2[registers[15]] # R
+        registers[25] += 8 # T-states
+        registers[24] = (registers[24] + 2) % 65536 # PC
 
     def set_xy(self, registers, memory, bit, xyh, xyl, dest=-1):
         # SET n,(IX/Y+d)
         addr = (registers[xyl] + 256 * registers[xyh] + OFFSETS[memory[(registers[24] + 2) % 65536]]) % 65536
         value = memory[addr] | bit
         if addr > 0x3FFF:
             memory[addr] = value
         if dest >= 0:
             registers[dest] = value
-        registers[15] = R2[registers[15]]
-        registers[25] += 23
-        registers[24] = (registers[24] + 4) % 65536
+        registers[15] = R2[registers[15]] # R
+        registers[25] += 23 # T-states
+        registers[24] = (registers[24] + 4) % 65536 # PC
 
     def create_opcodes(self):
         from skoolkit.simtables import (
             ADC, ADC_A_A, ADD, AND, BIT, CCF, CP, CPL, DAA, DEC, INC, NEG, OR,
             PARITY, RL, RLC, RR, RRC, RLA, RLCA, RRA, RRCA, SBC, SBC_A_A, SCF,
             SLA, SLL, SRA, SRL, SUB, SZ53P, XOR
         )
```

### Comparing `skoolkit-8.8/skoolkit/skool2asm.py` & `skoolkit-8.9/skoolkit/skool2asm.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/skool2bin.py` & `skoolkit-8.9/skoolkit/skool2bin.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/skool2ctl.py` & `skoolkit-8.9/skoolkit/skool2ctl.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/skool2html.py` & `skoolkit-8.9/skoolkit/skool2html.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/skoolasm.py` & `skoolkit-8.9/skoolkit/skoolasm.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/skoolctl.py` & `skoolkit-8.9/skoolkit/skoolctl.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/skoolhtml.py` & `skoolkit-8.9/skoolkit/skoolhtml.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/skoolmacro.py` & `skoolkit-8.9/skoolkit/skoolmacro.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/skoolparser.py` & `skoolkit-8.9/skoolkit/skoolparser.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/sna2ctl.py` & `skoolkit-8.9/skoolkit/sna2ctl.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/sna2img.py` & `skoolkit-8.9/skoolkit/sna2img.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/sna2skool.py` & `skoolkit-8.9/skoolkit/sna2skool.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/snactl.py` & `skoolkit-8.9/skoolkit/snactl.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/snapinfo.py` & `skoolkit-8.9/skoolkit/snapinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2013-2017, 2019-2022 Richard Dymond (rjdymond@gmail.com)
+# Copyright 2013-2017, 2019-2023 Richard Dymond (rjdymond@gmail.com)
 #
 # This file is part of SkoolKit.
 #
 # SkoolKit is free software: you can redistribute it and/or modify it under the
 # terms of the GNU General Public License as published by the Free Software
 # Foundation, either version 3 of the License, or (at your option) any later
 # version.
@@ -16,15 +16,15 @@
 
 import argparse
 
 from skoolkit import SkoolKitError, get_dword, get_int_param, get_word, integer, read_bin_file, VERSION
 from skoolkit.basic import BasicLister, VariableLister, get_char
 from skoolkit.config import get_config, show_config, update_options
 from skoolkit.opcodes import END, decode
-from skoolkit.snapshot import make_snapshot
+from skoolkit.snapshot import FRAME_DURATION, QFRAME_DURATION, make_snapshot
 from skoolkit.sna2skool import get_ctl_parser
 from skoolkit.snaskool import Disassembly
 
 class Registers:
     reg_map = {
         'b': 'bc', 'c': 'bc', 'b2': 'bc2', 'c2': 'bc2',
         'd': 'de', 'e': 'de', 'd2': 'de2', 'e2': 'de2',
@@ -155,14 +155,20 @@
     reg.a2 = header[21]
     reg.f2 = header[22]
     reg.iy = get_word(header, 23)
     reg.ix = get_word(header, 25)
     reg.border = (header[12] // 2) % 8
     reg.iff2 = header[28]
     reg.im = header[29] & 3
+    if version == 3:
+        t1 = (header[55] + 256 * header[56]) % QFRAME_DURATION
+        t2 = (2 - header[57]) % 4
+        reg.tstates = FRAME_DURATION - 1 - t2 * QFRAME_DURATION - t1
+    else:
+        reg.tstates = 0
 
     return header, reg, ram_blocks
 
 def _analyse_z80(z80file, header, reg, ram_blocks):
     if get_word(header, 6) > 0:
         version = 1
     else:
@@ -270,14 +276,15 @@
             reg.iy = get_word(block, 18)
             reg.sp = get_word(block, 20)
             reg.pc = get_word(block, 22)
             reg.i = block[24]
             reg.r = block[25]
             reg.iff2 = block[27]
             reg.im = block[28]
+            reg.tstates = get_dword(block, 29)
         elif block_id == 'SPCR':
             reg.border = block[0]
 
     return header, reg, blocks
 
 def _get_block_id(data, index):
     return ''.join([chr(b) for b in data[index:index+ 4]])
@@ -368,14 +375,15 @@
     if len(sna) > 49179:
         reg.pc = get_word(sna, 49179)
     else:
         reg.pc = get_word(sna, reg.sp - 16357)
     reg.border = sna[26]
     reg.iff2 = (sna[19] & 4) // 4
     reg.im = sna[25]
+    reg.tstates = 0
 
     return sna[:27], reg, sna[27:]
 
 def _print_ram_banks(sna):
     bank = sna[49154] & 7
     print('RAM bank 5 (16384 bytes: 16384-32767 4000-7FFF)')
     print('RAM bank 2 (16384 bytes: 32768-49151 8000-BFFF)')
@@ -450,15 +458,15 @@
         node_id = config['NodeId'].format(**props)
         print('{} [label={}]'.format(node_id, config['NodeLabel'].format(**props)))
         if children:
             ref_ids = [config['NodeId'].format(address=a, label=entries[a][0].instructions[0].label or '') for a in children]
             print('{} -> {{{}}}'.format(node_id, ' '.join(ref_ids)))
     print('}')
 
-def _find(snapshot, byte_seq, base_addr=16384):
+def _find(snapshot, byte_seq, base_addr):
     steps = '1'
     if '-' in byte_seq:
         byte_seq, steps = byte_seq.split('-', 1)
     try:
         byte_values = [get_int_param(i, True) for i in byte_seq.split(',')]
     except ValueError:
         raise SkoolKitError('Invalid byte sequence: {}'.format(byte_seq))
@@ -488,18 +496,18 @@
         raise SkoolKitError('Invalid tile coordinates: {}'.format(coords))
     df_addr = 16384 + 2048 * (y // 8) + 32 * (y & 7) + x
     byte_seq = snapshot[df_addr:df_addr + 2048:256]
     for b in byte_seq:
         print('|{:08b}|'.format(b).replace('0', ' ').replace('1', '*'))
     _find(snapshot, '{}-{}'.format(','.join([str(b) for b in byte_seq]), steps), 23296)
 
-def _find_text(snapshot, text):
+def _find_text(snapshot, text, base_addr):
     size = len(text)
     byte_values = [ord(c) for c in text]
-    for a in range(16384, 65536 - size + 1):
+    for a in range(base_addr, 65536 - size + 1):
         if snapshot[a:a + size] == byte_values:
             print("{0}-{1} {0:04X}-{1:04X}: {2}".format(a, a + size - 1, text))
 
 def _peek(snapshot, specs, fmt):
     for addr1, addr2, step in _get_address_ranges(specs):
         for a in range(addr1, addr2 + 1, step):
             value = snapshot[a]
@@ -513,19 +521,19 @@
             print(fmt.format(address=a, value=value))
 
 def run(infile, options, config):
     if any((options.find, options.tile, options.text, options.call_graph, options.peek,
             options.word, options.basic, options.variables)):
         snapshot, start, end = make_snapshot(infile, options.org, page=options.page)
         if options.find:
-            _find(snapshot, options.find)
+            _find(snapshot, options.find, start)
         elif options.tile:
             _find_tile(snapshot, options.tile)
         elif options.text:
-            _find_text(snapshot, options.text)
+            _find_text(snapshot, options.text, start)
         elif options.call_graph:
             _call_graph(snapshot, options.ctlfiles, infile, start, end, config)
         elif options.peek:
             _peek(snapshot, options.peek, config['Peek'])
         elif options.word:
             _word(snapshot, options.word, config['Word'])
         else:
```

### Comparing `skoolkit-8.8/skoolkit/snapmod.py` & `skoolkit-8.9/skoolkit/snapmod.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/snapshot.py` & `skoolkit-8.9/skoolkit/snapshot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2009-2013, 2015-2022 Richard Dymond (rjdymond@gmail.com)
+# Copyright 2009-2013, 2015-2023 Richard Dymond (rjdymond@gmail.com)
 #
 # This file is part of SkoolKit.
 #
 # SkoolKit is free software: you can redistribute it and/or modify it under the
 # terms of the GNU General Public License as published by the Free Software
 # Foundation, either version 3 of the License, or (at your option) any later
 # version.
@@ -16,14 +16,17 @@
 
 import textwrap
 import zlib
 
 from skoolkit import SkoolKitError, get_int_param, parse_int, read_bin_file
 from skoolkit.components import get_snapshot_reader, get_value
 
+FRAME_DURATION = 69888
+QFRAME_DURATION = FRAME_DURATION // 4
+
 # https://worldofspectrum.net/faq/reference/z80format.htm
 Z80_REGISTERS = {
     'a': 0,
     'f': 1,
     'bc': 2,
     'c': 2,
     'b': 3,
@@ -157,31 +160,36 @@
                 z80[27] = z80[28] = get_int_param(val) & 255
             elif name == 'im':
                 z80[29] &= 252 # Clear bits 0 and 1
                 z80[29] |= get_int_param(val) & 3
             elif name == 'border':
                 z80[12] &= 241 # Clear bits 1-3
                 z80[12] |= (get_int_param(val) & 7) * 2 # Border colour
+            elif name == 'tstates':
+                t = FRAME_DURATION - 1 - (get_int_param(val) % FRAME_DURATION)
+                t1, t2 = t % QFRAME_DURATION, t // QFRAME_DURATION
+                z80[55:58] = (t1 % 256, t1 // 256, (2 - t2) % 4)
             else:
                 raise SkoolKitError("Invalid parameter: {}".format(spec))
         except ValueError:
             raise SkoolKitError("Cannot parse integer: {}".format(spec))
 
 def print_state_help(short_option=None):
     options = ['--state name=value']
     if short_option:
         options.insert(0, '-{} name=value'.format(short_option))
     print("""
 Usage: {}
 
 Set a hardware state attribute. Recognised names and their default values are:
 
-  border - border colour (default=0)
-  iff    - interrupt flip-flop: 0=disabled, 1=enabled (default=1)
-  im     - interrupt mode (default=1)
+  border  - border colour (default=0)
+  iff     - interrupt flip-flop: 0=disabled, 1=enabled (default=1)
+  im      - interrupt mode (default=1)
+  tstates - T-states elapsed since start of frame (default=0)
 """.format(', '.join(options)).strip())
 
 def make_z80_ram_block(data, page):
     block = []
     prev_b = None
     count = 0
     for b in data:
@@ -375,15 +383,15 @@
 
 def _decompress_block(ramz):
     block = []
     i = 0
     while i < len(ramz):
         b = ramz[i]
         i += 1
-        if b == 237:
+        if b == 237 and i < len(ramz):
             c = ramz[i]
             i += 1
             if c == 237:
                 length, byte = ramz[i], ramz[i + 1]
                 if length == 0:
                     raise SnapshotError("Found ED ED 00 {0:02X}".format(byte))
                 block += [byte] * length
```

### Comparing `skoolkit-8.8/skoolkit/snaskool.py` & `skoolkit-8.9/skoolkit/snaskool.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/tap2sna.py` & `skoolkit-8.9/skoolkit/tap2sna.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2013, 2015-2018, 2020-2022 Richard Dymond (rjdymond@gmail.com)
+# Copyright 2013, 2015-2018, 2020-2023 Richard Dymond (rjdymond@gmail.com)
 #
 # This file is part of SkoolKit.
 #
 # SkoolKit is free software: you can redistribute it and/or modify it under the
 # terms of the GNU General Public License as published by the Free Software
 # Foundation, either version 3 of the License, or (at your option) any later
 # version.
@@ -13,22 +13,24 @@
 #
 # You should have received a copy of the GNU General Public License along with
 # SkoolKit. If not, see <http://www.gnu.org/licenses/>.
 
 import sys
 import os
 import argparse
+import hashlib
 import tempfile
 import zipfile
 from urllib.request import Request, urlopen
 from urllib.parse import urlparse
 
 from skoolkit import (SkoolKitError, get_dword, get_int_param, get_object,
-                      get_word, get_word3, integer, open_file, read_bin_file,
-                      warn, write_line, ROM48, VERSION)
+                      get_word, get_word3, integer, open_file, parse_int,
+                      read_bin_file, warn, write_line, ROM48, VERSION)
+from skoolkit.loadsample import ACCELERATORS
 from skoolkit.loadtracer import LoadTracer
 from skoolkit.simulator import (Simulator, A, F, B, C, D, E, H, L, IXh, IXl, IYh, IYl,
                                 SP, I, R, xA, xF, xB, xC, xD, xE, xH, xL, PC)
 from skoolkit.snapshot import move, poke, print_reg_help, print_state_help, write_z80v3
 
 SYSVARS = (
     255, 0, 0, 0,         # 23552 - KSTATE0
@@ -149,53 +151,109 @@
     0x5C86: 0xE0,   # DF-CCL
     0x5C8A: 0x21,   # S-POSNL
     0x5CCB: 0x80,   # First byte of program area
     0x5CCC: 0xEF,   # LOAD
     0x5CCD: 0x2222, # ""
     0x5CCF: 0x0D,   # ENTER
     0x5CD0: 0x80,   # End of program area
+    0xFF18: 0x0DF3, # Stack...
+    0xFF1A: 0x0BCE,
+    0xFF1C: 0x50E3,
+    0xFF1E: 0x0BCE,
+    0xFF20: 0x50E4,
+    0xFF22: 0x171D,
+    0xFF24: 0x0ADC,
+    0xFF26: 0x0BCE,
+    0xFF28: 0x50E7,
+    0xFF2A: 0x171A,
+    0xFF2C: 0x0ADC,
+    0xFF2E: 0x18D7,
+    0xFF30: 0x0038,
+    0xFF32: 0x0038,
+    0xFF34: 0x190D,
+    0xFF36: 0x5CCF,
+    0xFF38: 0x0306,
+    0xFF3A: 0x5C07,
+    0xFF3C: 0x004D,
+    0xFF3E: 0x33B1,
+    0xFF40: 0x5C92,
+    0xFF42: 0x0005,
+    0xFF44: 0x32C8,
+    0xFF46: 0x3429,
+    0xFF48: 0x369B,
+    0xFF4A: 0x001F,
+    0xFF4C: 0x1B6D,
+    0xFF4E: 0x1CDB,
     0xFF50: 0x1B52, # Address of SCAN-LOOP
     0xFF52: 0x1B76, # Address of STMT-RET
     0xFF54: 0x12B7, # Address of entry point in 'MAIN EXECUTION' loop at 0x12A2
     0xFF56: 0x3E00  # RAMTOP marker
 }
 
 SIM_LOAD_CODE_PATCH = {
     0x5C5B: 0x5CD0, # K-CUR
     0x5C61: 0x5CD2, # WORKSP
     0x5C63: 0x5CD2, # STKBOT
     0x5C65: 0x5CD2, # STKEND
     0x5C82: 0x14,   # ECHO-E
     0x5CCF: 0xAF,   # CODE
     0x5CD0: 0x0D,   # ENTER
-    0x5CD1: 0x80    # End of program area
+    0x5CD1: 0x80,   # End of program area
+    0xFF1C: 0x50EA, # Stack...
+    0xFF20: 0x50EB,
+    0xFF22: 0x1716,
+    0xFF28: 0x50EC,
+    0xFF2A: 0x1715,
+    0xFF30: 0x000A,
+    0xFF36: 0x5CD0
 }
 
 class SkoolKitArgumentParser(argparse.ArgumentParser):
     def convert_arg_line_to_args(self, arg_line):
-        for arg in arg_line.split():
-            if arg in (';', '#'):
+        args = []
+        arg = ''
+        q = None
+        for c in arg_line:
+            if c == q:
+                args.append(arg)
+                arg = ''
+                q = None
+            elif c in '\'"' and q is None:
+                q = c
+            elif c.isspace() and q is None:
+                if arg:
+                    args.append(arg)
+                    arg = ''
+            elif c in ';#' and q is None:
                 break
-            yield arg
+            else:
+                arg += c
+        if arg:
+            args.append(arg)
+        return args
 
 class TapeError(Exception):
     pass
 
 class TapeBlockTimings:
-    def __init__(self, pilot_len=0, pilot=0, sync=(), zero=0, one=0, pause=0):
+    def __init__(self, pilot_len=0, pilot=0, sync=(), zero=0, one=0, pause=0, used_bits=8):
         self.pilot_len = pilot_len
         self.pilot = pilot
         self.sync = sync
         self.zero = zero
         self.one = one
         self.pause = pause
+        self.used_bits = used_bits
 
-TAP_TIMINGS_HEADER = TapeBlockTimings(8063, 2168, (667, 735), 855, 1710, 3500000)
-
-TAP_TIMINGS_DATA = TapeBlockTimings(3223, 2168, (667, 735), 855, 1710, 3500000)
+def get_tape_block_timings(first_byte, pause=3500000):
+    if first_byte == 0:
+        # Header block
+        return TapeBlockTimings(8063, 2168, (667, 735), 855, 1710, pause)
+    # Data block
+    return TapeBlockTimings(3223, 2168, (667, 735), 855, 1710, pause)
 
 def _write_z80(ram, options, fname):
     parent_dir = os.path.dirname(fname)
     if parent_dir and not os.path.isdir(parent_dir):
         os.makedirs(parent_dir)
     write_line('Writing {0}'.format(fname))
     write_z80v3(fname, ram, options.reg, options.state)
@@ -214,36 +272,69 @@
         elif op_type == 'poke':
             poke(snapshot, param_str)
         elif op_type == 'sysvars':
             snapshot[23552:23755] = SYSVARS
         else:
             raise SkoolKitError(f'Invalid operation: {spec}')
 
+def _set_sim_load_config(options):
+    options.accelerator = None
+    options.fast_load = True
+    options.first_edge = -2168
+    options.pause = True
+    options.timeout = 900
+    options.trace = None
+    for spec in options.sim_load_config:
+        name, sep, value = spec.lower().partition('=')
+        if sep:
+            if name == 'accelerator':
+                options.accelerator = value
+            elif name == 'fast-load': # pragma: no cover
+                options.fast_load = parse_int(value, options.fast_load)
+            elif name == 'first-edge': # pragma: no cover
+                options.first_edge = parse_int(value, options.first_edge)
+            elif name == 'pause': # pragma: no cover
+                options.pause = parse_int(value, options.pause)
+            elif name == 'timeout': # pragma: no cover
+                options.timeout = parse_int(value, options.timeout)
+            elif name == 'trace':
+                options.trace = value
+            else:
+                raise SkoolKitError(f'Invalid sim-load configuration parameter: {name}')
+
 def sim_load(blocks, options):
+    _set_sim_load_config(options)
+    if options.accelerator:
+        accelerator = ACCELERATORS.get(options.accelerator)
+        if options.accelerator != 'none' and accelerator is None:
+            raise SkoolKitError(f'Unrecognised accelerator: {options.accelerator}')
+    else:
+        accelerator = set(ACCELERATORS.values())
     snapshot = [0] * 65536
     rom = read_bin_file(ROM48, 16384)
     snapshot[:len(rom)] = rom
+    snapshot[0x5800:0x5B00] = [56] * 768 # PAPER 7: INK 0
     snapshot[0x5C00:0x5C00 + len(SYSVARS)] = SYSVARS
     for a, b in SIM_LOAD_PATCH.items():
         snapshot[a] = b % 256
         if b > 0xFF:
             snapshot[a + 1] = b // 256
     block1_data = blocks[0][1]
     if len(block1_data) >= 19 and tuple(block1_data[0:2]) == (0, 3):
         for a, b in SIM_LOAD_CODE_PATCH.items():
             snapshot[a] = b % 256
             if b > 0xFF:
                 snapshot[a + 1] = b // 256
     snapshot[0xFF58:] = snapshot[0x3E08:0x3EB0] # UDGs
-    config = {'fast_djnz': True, 'fast_ldir': True}
-    simulator = Simulator(snapshot, {'SP': 0xFF50}, config=config)
-    tracer = LoadTracer(blocks)
+    simulator = Simulator(snapshot, {'SP': 0xFF50})
+    tracer = LoadTracer(simulator, blocks, accelerator, options.pause, options.first_edge)
     simulator.set_tracer(tracer)
     try:
-        tracer.run(simulator, 0x0605, options.start) # SAVE-ETC
+        # Begin execution at 0x0605 (SAVE-ETC)
+        tracer.run(0x0605, options.start, options.fast_load, options.trace, options.timeout * 3500000)
         _ram_operations(snapshot, options.ram_ops)
     except KeyboardInterrupt: # pragma: no cover
         write_line(f'Simulation stopped (interrupted): PC={simulator.registers[PC]}')
     sim_registers = simulator.registers
     registers = {
         'A': sim_registers[A],
         'F': sim_registers[F],
@@ -265,15 +356,15 @@
         '^D': sim_registers[xD],
         '^E': sim_registers[xE],
         '^H': sim_registers[xH],
         '^L': sim_registers[xL],
         'PC': sim_registers[PC]
     }
     options.reg = [f'{r}={v}' for r, v in registers.items()] + options.reg
-    state = [f'im={simulator.imode}', f'iff={simulator.iff2}', f'border={tracer.border}']
+    state = [f'im={simulator.imode}', f'iff={simulator.iff}', f'border={tracer.border}']
     options.state = state + options.state
     return simulator.memory[0x4000:]
 
 def _get_load_params(param_str):
     params = []
     for index, n in enumerate(param_str.split(',')):
         if index == 0:
@@ -373,34 +464,33 @@
     # https://worldofspectrum.net/features/TZXformat.html
     block_id = data[i]
     tape_data = None
     timings = None
     i += 1
     if block_id == 16:
         # Standard speed data block
+        pause = get_word(data, i) * 3500
         length = get_word(data, i + 2)
         tape_data = data[i + 4:i + 4 + length]
         if tape_data:
-            if tape_data[0] == 0:
-                timings = TAP_TIMINGS_HEADER
-            else:
-                timings = TAP_TIMINGS_DATA
+            timings = get_tape_block_timings(tape_data[0], pause)
         i += 4 + length
     elif block_id == 17:
         # Turbo speed data block
         length = get_word3(data, i + 15)
         tape_data = data[i + 18:i + 18 + length]
         pilot = get_word(data, i)
         sync1 = get_word(data, i + 2)
         sync2 = get_word(data, i + 4)
         zero = get_word(data, i + 6)
         one = get_word(data, i + 8)
         pilot_len = get_word(data, i + 10)
+        used_bits = data[i + 12]
         pause = get_word(data, i + 13) * 3500
-        timings = TapeBlockTimings(pilot_len, pilot, (sync1, sync2), zero, one, pause)
+        timings = TapeBlockTimings(pilot_len, pilot, (sync1, sync2), zero, one, pause, used_bits)
         i += 18 + length
     elif block_id == 18:
         # Pure tone
         if sim: # pragma: no cover
             tape_data = []
             pilot = get_word(data, i)
             pilot_len = get_word(data, i + 2)
@@ -417,16 +507,17 @@
     elif block_id == 20:
         # Pure data block
         length = get_word3(data, i + 7)
         tape_data = data[i + 10:i + 10 + length]
         if sim: # pragma: no cover
             zero = get_word(data, i)
             one = get_word(data, i + 2)
+            used_bits = data[i + 4]
             pause = get_word(data, i + 5) * 3500
-            timings = TapeBlockTimings(zero=zero, one=one, pause=pause)
+            timings = TapeBlockTimings(zero=zero, one=one, pause=pause, used_bits=used_bits)
         i += 10 + length
     elif block_id == 21:
         # Direct recording block
         if sim:
             raise TapeError("TZX Direct Recording (0x15) not supported")
         i += get_word3(data, i + 5) + 8
     elif block_id == 24:
@@ -437,14 +528,17 @@
     elif block_id == 25:
         # Generalized data block
         if sim:
             raise TapeError("TZX Generalized Data Block (0x19) not supported")
         i += get_dword(data, i) + 4
     elif block_id == 32:
         # Pause (silence) or 'Stop the tape' command
+        if sim: # pragma: no cover
+            pause = get_word(data, i) * 3500
+            timings = TapeBlockTimings(pause=pause)
         i += 2
     elif block_id == 33:
         # Group start
         i += data[i] + 1
     elif block_id == 34:
         # Group end
         pass
@@ -465,16 +559,14 @@
         pass
     elif block_id == 40:
         # Select block
         i += get_word(data, i) + 2
     elif block_id == 42:
         # Stop the tape if in 48K mode
         i += 4
-        if sim: # pragma: no cover
-            i = len(data)
     elif block_id == 43:
         # Set signal level
         i += 5
     elif block_id == 48:
         # Text description
         i += data[i] + 1
     elif block_id == 49:
@@ -490,49 +582,73 @@
         # Custom info block
         i += get_dword(data, i + 16) + 20
     elif block_id == 90:
         # "Glue" block
         i += 9
     else:
         raise TapeError('Unknown TZX block ID: 0x{:X}'.format(block_id))
-    return i, timings, tape_data
+    return i, block_id, timings, tape_data
 
-def _get_tzx_blocks(data, sim):
+def _get_tzx_blocks(data, sim, start, stop):
     signature = ''.join(chr(b) for b in data[:7])
     if signature != 'ZXTape!':
         raise TapeError("Not a TZX file")
     i = 10
     blocks = []
+    block_num = 1
+    loop = None
     while i < len(data):
-        i, timings, tape_data = _get_tzx_block(data, i, sim)
-        blocks.append((timings, tape_data))
+        if block_num >= stop > 0:
+            break
+        i, block_id, timings, tape_data = _get_tzx_block(data, i, sim)
+        if block_num >= start:
+            if sim: # pragma: no cover
+                if block_id == 0x20:
+                    if stop == 0 and timings.pause == 0:
+                        break
+                elif block_id == 0x24:
+                    loop = []
+                    repetitions = get_word(data, i - 2)
+                elif block_id == 0x2A and stop == 0:
+                    # Stop the tape if in 48K mode
+                    break
+            if loop is None:
+                blocks.append((timings, tape_data))
+            else: # pragma: no cover
+                loop.append((timings, tape_data))
+            if block_id == 0x25 and loop is not None: # pragma: no cover
+                blocks.extend(loop * repetitions)
+                loop = None
+        block_num += 1
     return blocks
 
-def get_tap_blocks(tap, sim=False):
+def get_tap_blocks(tap, start=1, stop=0):
     blocks = []
+    block_num = 1
     i = 0
     while i + 1 < len(tap):
+        if block_num >= stop > 0:
+            break # pragma: no cover (tested but missed by coverage)
         block_len = tap[i] + 256 * tap[i + 1]
         i += 2
-        data = tap[i:i + block_len]
-        if data:
-            if data[0] == 0:
-                timings = TAP_TIMINGS_HEADER
-            else:
-                timings = TAP_TIMINGS_DATA
-            blocks.append((timings, data))
+        if block_num >= start:
+            data = tap[i:i + block_len]
+            if data:
+                timings = get_tape_block_timings(data[0])
+                blocks.append((timings, data))
         i += block_len
+        block_num += 1
     return blocks
 
-def _get_tape_blocks(tape_type, tape, sim):
+def _get_tape_blocks(tape_type, tape, sim, start, stop):
     if tape_type.lower() == 'tzx':
-        return _get_tzx_blocks(tape, sim)
-    return get_tap_blocks(tape, sim)
+        return _get_tzx_blocks(tape, sim, start, stop)
+    return get_tap_blocks(tape, start, stop)
 
-def _get_tape(urlstring, user_agent, member=None):
+def _get_tape(urlstring, user_agent, member):
     url = urlparse(urlstring)
     if url.scheme:
         write_line('Downloading {0}'.format(urlstring))
         r = Request(urlstring, headers={'User-Agent': user_agent})
         u = urlopen(r, timeout=30)
         f = tempfile.NamedTemporaryFile(prefix='tap2sna-')
         while 1:
@@ -550,15 +666,18 @@
                 if name.lower().endswith(('.tap', '.tzx')):
                     member = name
                     break
             else:
                 f.close()
                 raise TapeError('No TAP or TZX file found')
         write_line('Extracting {0}'.format(member))
-        tape = z.open(member)
+        try:
+            tape = z.open(member)
+        except KeyError:
+            raise TapeError(f'No file named "{member}" in the archive')
         data = bytearray(tape.read())
         tape_type = member[-3:]
     else:
         tape_type = urlstring[-3:]
         f.seek(0)
         data = bytearray(f.read())
 
@@ -648,17 +767,81 @@
 
 --ram sysvars
 
   Initialise the system variables at 23552-23754 (5C00-5CCA) with values
   suitable for a 48K ZX Spectrum.
 """.lstrip())
 
+def _print_sim_load_config_help():
+    width = max(len(n) for n in ACCELERATORS) + 2
+    names = [n.ljust(width) for n in sorted(ACCELERATORS)]
+    num_cols = 3
+    names += [''] * (-len(names) % num_cols)
+    cl = len(names) // num_cols
+    columns = [names[i:i + cl] for i in range(0, len(names), cl)]
+    accelerators = '\n  '.join(''.join(n) for n in zip(*columns))
+    print(f"""
+Usage: --sim-load-config accelerator=NAME
+       --sim-load-config fast-load=0/1
+       --sim-load-config first-edge=N
+       --sim-load-config pause=0/1
+       --sim-load-config timeout=N
+       --sim-load-config trace=FILE
+
+Use a specific tape-sampling loop accelerator, disable fast loading, set the
+location of the leading edge of the first pulse on the tape, disable pausing
+between tape blocks, set the timeout, or log executed instructions to a file.
+
+--sim-load-config accelerator=NAME
+
+  Use a specific accelerator to speed up the simulation of the tape-sampling
+  loop in a loading routine, or disable acceleration entirely. (By default, an
+  appropriate accelerator is automatically selected, if available.) Recognised
+  accelerator names are:
+
+  {accelerators}
+
+--sim-load-config fast-load=0/1
+
+  By default, whenever the Spectrum ROM's load routine is called, a shortcut is
+  taken by "fast loading" the next block on the tape. This significantly
+  reduces the load time for many tapes, but can also cause some loaders to
+  fail. Set fast-load=0 to disable fast loading.
+
+--sim-load-config first-edge=N
+
+  Set the time (in T-states) from the start of the tape at which to place the
+  leading edge of the first pulse (default: -2168). The default value places
+  the trailing edge of the first pulse at time 0, but some loaders (e.g.
+  polarity-sensitive loaders) require first-edge=0.
+
+--sim-load-config pause=0/1
+
+  By default, the tape is paused between blocks, and resumed whenever port 254
+  is read. While this can help with tapes that require (but do not actually
+  contain) long pauses between blocks, it can cause some loaders to fail. Set
+  pause=0 to disable this behaviour and run the tape continuously.
+
+--sim-load-config timeout=N
+
+  Set the timeout to N seconds (default: 900). A simulated LOAD still in
+  progress after this period of Z80 CPU time will automatically abort.
+
+--sim-load-config trace=FILE
+
+  Log to FILE all instructions executed during the simulated LOAD.
+""".strip())
+
 def make_z80(url, options, z80):
-    tape_type, tape = _get_tape(url, options.user_agent)
-    tape_blocks = _get_tape_blocks(tape_type, tape, options.sim_load)
+    tape_type, tape = _get_tape(url, options.user_agent, options.tape_name)
+    if options.tape_sum:
+        md5sum = hashlib.md5(tape).hexdigest()
+        if md5sum != options.tape_sum:
+            raise TapeError(f'Checksum mismatch: Expected {options.tape_sum}, actually {md5sum}')
+    tape_blocks = _get_tape_blocks(tape_type, tape, options.sim_load, options.tape_start, options.tape_stop)
     if options.sim_load:
         blocks = [b for b in tape_blocks if b[0]]
         ram = sim_load(blocks, options)
     else:
         blocks = [b[1] for b in tape_blocks]
         ram = _get_ram(blocks, options)
     _write_z80(ram, options, z80)
@@ -670,14 +853,17 @@
                     "INPUT may be the full URL to a remote zip archive or TAP/TZX file, or the path to a local file. "
                     "Arguments may be read from FILE instead of (or as well as) being given on the command line.",
         fromfile_prefix_chars='@',
         add_help=False
     )
     parser.add_argument('args', help=argparse.SUPPRESS, nargs='*')
     group = parser.add_argument_group('Options')
+    group.add_argument('-c', '--sim-load-config', metavar='name=value', action='append', default=[],
+                       help="Set the value of a --sim-load configuration parameter. "
+                            "Do '-c help' for more information. This option may be used multiple times.")
     group.add_argument('-d', '--output-dir', dest='output_dir', metavar='DIR',
                        help="Write the snapshot file in this directory.")
     group.add_argument('-f', '--force', action='store_true',
                        help="Overwrite an existing snapshot.")
     group.add_argument('-p', '--stack', dest='stack', metavar='STACK', type=integer,
                        help="Set the stack pointer.")
     group.add_argument('--ram', dest='ram_ops', metavar='OPERATION', action='append', default=[],
@@ -689,19 +875,30 @@
     group.add_argument('-s', '--start', dest='start', metavar='START', type=integer,
                        help="Set the start address to JP to.")
     group.add_argument('--sim-load', action='store_true',
                        help='Simulate a 48K ZX Spectrum running LOAD "".')
     group.add_argument('--state', dest='state', metavar='name=value', action='append', default=[],
                        help="Set a hardware state attribute. Do '--state help' for more information. "
                             "This option may be used multiple times.")
+    group.add_argument('--tape-name', metavar='NAME',
+                       help="Specify the name of a TAP/TZX file in a zip archive.")
+    group.add_argument('--tape-start', metavar='BLOCK', type=int, default=1,
+                       help="Start the tape at this block number.")
+    group.add_argument('--tape-stop', metavar='BLOCK', type=int, default=0,
+                       help="Stop the tape at this block number.")
+    group.add_argument('--tape-sum', metavar='MD5SUM',
+                       help="Specify the MD5 checksum of the TAP/TZX file.")
     group.add_argument('-u', '--user-agent', dest='user_agent', metavar='AGENT', default='',
                        help="Set the User-Agent header.")
     group.add_argument('-V', '--version', action='version', version='SkoolKit {}'.format(VERSION),
                        help='Show SkoolKit version number and exit.')
     namespace, unknown_args = parser.parse_known_args(args)
+    if 'help' in namespace.sim_load_config:
+        _print_sim_load_config_help()
+        return
     if 'help' in namespace.ram_ops:
         _print_ram_help()
         return
     if 'help' in namespace.reg:
         print_reg_help()
         return
     if 'help' in namespace.state:
```

### Comparing `skoolkit-8.8/skoolkit/tapinfo.py` & `skoolkit-8.9/skoolkit/tapinfo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2013, 2015, 2017, 2020 Richard Dymond (rjdymond@gmail.com)
+# Copyright 2013, 2015, 2017, 2020, 2022 Richard Dymond (rjdymond@gmail.com)
 #
 # This file is part of SkoolKit.
 #
 # SkoolKit is free software: you can redistribute it and/or modify it under the
 # terms of the GNU General Public License as published by the Free Software
 # Foundation, either version 3 of the License, or (at your option) any later
 # version.
@@ -12,15 +12,15 @@
 # A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # SkoolKit. If not, see <http://www.gnu.org/licenses/>.
 
 import argparse
 
-from skoolkit import SkoolKitError, get_word, get_word3, get_dword, get_int_param, VERSION
+from skoolkit import SkoolKitError, get_word, get_word3, get_dword, get_int_param, warn, VERSION
 from skoolkit.basic import BasicLister, get_char
 
 ARCHIVE_INFO = {
     0: "Full title",
     1: "Software house/publisher",
     2: "Author(s)",
     3: "Year of publication",
@@ -260,19 +260,28 @@
     # https://worldofspectrum.net/features/TZXformat.html
     block_id = data[i]
     info = []
     tape_data = []
     i += 1
     if block_id == 16:
         header = 'Standard speed data'
+        info.append('Pause: {}ms'.format(get_word(data, i)))
         length = get_word(data, i + 2)
         tape_data = data[i + 4:i + 4 + length]
         i += 4 + length
     elif block_id == 17:
         header = 'Turbo speed data'
+        info.append('Pilot pulse: {}'.format(get_word(data, i)))
+        info.append('Sync pulse 1: {}'.format(get_word(data, i + 2)))
+        info.append('Sync pulse 2: {}'.format(get_word(data, i + 4)))
+        info.append('0-pulse: {}'.format(get_word(data, i + 6)))
+        info.append('1-pulse: {}'.format(get_word(data, i + 8)))
+        info.append('Pilot length: {} pulses'.format(get_word(data, i + 10)))
+        info.append('Used bits in last byte: {}'.format(data[i + 12]))
+        info.append('Pause: {}ms'.format(get_word(data, i + 13)))
         length = get_word3(data, i + 15)
         tape_data = data[i + 18:i + 18 + length]
         i += 18 + length
     elif block_id == 18:
         header = 'Pure tone'
         info.append('Pulse length: {} T-states'.format(get_word(data, i)))
         info.append('Pulses: {}'.format(get_word(data, i + 2)))
@@ -488,24 +497,29 @@
         elif not block_ids or block_id in block_ids:
             _print_block(block_num, tape_data, options.data, info, block_id, header)
         block_num += 1
 
 def _analyse_tap(tap, basic_block, show_data):
     i = 0
     block_num = 1
-    while i < len(tap):
+    while i + 1 < len(tap):
         block_len = get_word(tap, i)
         data = tap[i + 2:i + 2 + block_len]
         if basic_block:
             _list_basic(block_num, data, *basic_block)
         else:
             _print_block(block_num, data, show_data)
         i += block_len + 2
         block_num += 1
 
+    if i < len(tap):
+        warn('Extraneous byte at end of file')
+    elif i > len(tap):
+        warn(f'Missing {i - len(tap)} data byte(s) at end of file')
+
 def main(args):
     parser = argparse.ArgumentParser(
         usage="tapinfo.py FILE",
         description="Show the blocks in a TAP or TZX file.",
         add_help=False
     )
     parser.add_argument('infile', help=argparse.SUPPRESS, nargs='?')
```

### Comparing `skoolkit-8.8/skoolkit/textutils.py` & `skoolkit-8.9/skoolkit/textutils.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/trace.py` & `skoolkit-8.9/skoolkit/trace.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Richard Dymond (rjdymond@gmail.com)
+# Copyright 2022, 2023 Richard Dymond (rjdymond@gmail.com)
 #
 # This file is part of SkoolKit.
 #
 # SkoolKit is free software: you can redistribute it and/or modify it under the
 # terms of the GNU General Public License as published by the Free Software
 # Foundation, either version 3 of the License, or (at your option) any later
 # version.
@@ -16,15 +16,15 @@
 
 import argparse
 import time
 
 from skoolkit import ROM48, VERSION, SkoolKitError, get_int_param, integer, read_bin_file
 from skoolkit.snapshot import make_snapshot, poke, print_reg_help, write_z80v3
 from skoolkit.simulator import (Simulator, A, F, B, C, D, E, H, L, IXh, IXl, IYh, IYl,
-                                SP, I, R, xA, xF, xB, xC, xD, xE, xH, xL, PC, T)
+                                SP, I, R, xA, xF, xB, xC, xD, xE, xH, xL, PC, T, FRAME_DURATION)
 from skoolkit.snapinfo import parse_snapshot
 from skoolkit.traceutils import disassemble
 
 TRACE1H = "${address:04X} {data:<8} {i}"
 TRACE1D = "{address:05} {data:<8} {i}"
 TRACE2H = """
 ${address:04X} {data:<8} {i:<15}  A={A:02X} F={F:08b} BC={BC:04X} DE={DE:04X} HL={HL:04X} IX={IX:04X} IY={IY:04X} IR={IR:04X}
@@ -38,20 +38,22 @@
 class Tracer:
     def __init__(self, border):
         self.operations = 0
         self.border = border
         self.spkr = None
         self.out_times = []
 
-    def run(self, simulator, start, stop, verbose, max_operations, max_tstates, decimal):
+    def run(self, simulator, start, stop, verbose, max_operations, max_tstates, decimal, interrupts):
         opcodes = simulator.opcodes
         memory = simulator.memory
         registers = simulator.registers
         pc = registers[PC] = start
         operations = 0
+        tstates = 0
+        accept_int = False
 
         if decimal:
             p = b = w = ''
             if verbose > 1:
                 fmt = TRACE2D
             else:
                 fmt = TRACE1D
@@ -66,15 +68,24 @@
             values = {
                 'address': pc,
                 'data': ''.join(f'{memory[a % 65536]:02X}' for a in range(pc, pc + size)),
                 'i': instruction
             }
 
         while True:
+            t0 = tstates
             opcodes[memory[pc]]()
+            tstates = registers[25]
+
+            if interrupts and simulator.iff:
+                if tstates // FRAME_DURATION > t0 // FRAME_DURATION:
+                    accept_int = True
+                if accept_int:
+                    accept_int = simulator.accept_interrupt(registers, memory, pc)
+
             pc = registers[24]
 
             if verbose:
                 values.update({
                     "A": registers[A],
                     "F": registers[F],
                     "BC": registers[C] + 256 * registers[B],
@@ -209,34 +220,36 @@
     memory[:len(rom)] = rom
     for spec in options.pokes:
         poke(memory, spec)
     if reg:
         im = reg.im
         iff = reg.iff2
         border = reg.border
+        tstates = reg.tstates
     else:
         im = 1
         iff = 1
         border = 7
-    state = {'im': im, 'iff': iff}
-    config = {
-        'fast_djnz': options.verbose == 0,
-        'fast_ldir': options.verbose == 0
-    }
+        tstates = 0
+    state = {'im': im, 'iff': iff, 'tstates': tstates}
+    fast = options.verbose == 0 and not options.interrupts
+    config = {'fast_djnz': fast, 'fast_ldir': fast}
     simulator = Simulator(memory, get_registers(reg, options.reg), state, config)
     tracer = Tracer(border)
     simulator.set_tracer(tracer)
     begin = time.time()
     tracer.run(simulator, start, options.stop, options.verbose,
-               options.max_operations, options.max_tstates, options.decimal)
+               options.max_operations, options.max_tstates, options.decimal,
+               options.interrupts)
     rt = time.time() - begin
     if options.stats:
-        z80t = simulator.registers[T] / 3500000
-        speed = z80t / (rt or 0.001) # Avoid division by zero
-        print(f'Z80 execution time: {simulator.registers[T]} T-states ({z80t:.03f}s)')
+        z80t = simulator.registers[T] - tstates
+        z80s = z80t / 3500000
+        speed = z80s / (rt or 0.001) # Avoid division by zero
+        print(f'Z80 execution time: {z80t} T-states ({z80s:.03f}s)')
         print(f'Instructions executed: {tracer.operations}')
         print(f'Simulation time: {rt:.03f}s (x{speed:.02f})')
     if options.audio:
         delays = []
         for i, t in enumerate(tracer.out_times[1:]):
             delays.append(t - tracer.out_times[i])
         duration = sum(delays)
@@ -261,16 +274,17 @@
             f'^bc={r[xC] + 256 * r[xB]}',
             f'^de={r[xE] + 256 * r[xD]}',
             f'^hl={r[xL] + 256 * r[xH]}',
             f'pc={r[PC]}'
         )
         state = (
             f'border={tracer.border}',
-            f'iff={simulator.iff2}',
-            f'im={simulator.imode}'
+            f'iff={simulator.iff}',
+            f'im={simulator.imode}',
+            f'tstates={r[T]}'
         )
         write_z80v3(options.dump, ram, registers, state)
         print(f'Z80 snapshot dumped to {options.dump}')
 
 def main(args):
     parser = argparse.ArgumentParser(
         usage='trace.py [options] FILE',
@@ -284,14 +298,16 @@
                        help="Show audio delays.")
     group.add_argument('-D', '--decimal', action='store_true',
                        help="Show decimal values in verbose mode.")
     group.add_argument('--depth', type=int, default=2,
                        help='Simplify audio delays to this depth (default: 2).')
     group.add_argument('--dump', metavar='FILE',
                        help='Dump a Z80 snapshot to this file after execution.')
+    group.add_argument('-i', '--interrupts', action='store_true',
+                       help='Execute interrupt routines.')
     group.add_argument('--max-operations', metavar='MAX', type=int, default=0,
                        help='Maximum number of instructions to execute.')
     group.add_argument('--max-tstates', metavar='MAX', type=int, default=0,
                        help='Maximum number of T-states to run for.')
     group.add_argument('-o', '--org', metavar='ADDR', type=integer,
                        help='Specify the origin address of a binary (raw memory) file (default: 65536 - length).')
     group.add_argument('-p', '--poke', dest='pokes', metavar='a[-b[-c]],[^+]v', action='append', default=[],
```

### Comparing `skoolkit-8.8/skoolkit/traceutils.py` & `skoolkit-8.9/skoolkit/traceutils.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit/z80.py` & `skoolkit-8.9/skoolkit/z80.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/skoolkit.egg-info/PKG-INFO` & `skoolkit-8.9/skoolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skoolkit
-Version: 8.8
+Version: 8.9
 Summary: A suite of tools for creating disassemblies of ZX Spectrum games
 Home-page: https://skoolkit.ca
 Author: Richard Dymond
 Author-email: rjdymond@gmail.com
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `skoolkit-8.8/skoolkit.egg-info/SOURCES.txt` & `skoolkit-8.9/skoolkit.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 COPYING
 MANIFEST.in
 bin2sna.py
 bin2tap.py
+long_description.rst
 pyproject.toml
 setup.cfg
 skool2asm.py
 skool2bin.py
 skool2ctl.py
 skool2html.py
 sna2ctl.py
@@ -137,14 +138,15 @@
 skoolkit/components.py
 skoolkit/config.py
 skoolkit/ctlparser.py
 skoolkit/defaults.py
 skoolkit/disassembler.py
 skoolkit/graphics.py
 skoolkit/image.py
+skoolkit/loadsample.py
 skoolkit/loadtracer.py
 skoolkit/opcodes.py
 skoolkit/pngwriter.py
 skoolkit/refparser.py
 skoolkit/simtables.py
 skoolkit/simulator.py
 skoolkit/skool2asm.py
```

### Comparing `skoolkit-8.8/sna2ctl.py` & `skoolkit-8.9/sna2ctl.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/sna2img.py` & `skoolkit-8.9/sna2img.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/sna2skool.py` & `skoolkit-8.9/sna2skool.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/snapinfo.py` & `skoolkit-8.9/snapinfo.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/snapmod.py` & `skoolkit-8.9/snapmod.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/tap2sna.py` & `skoolkit-8.9/tap2sna.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/tapinfo.py` & `skoolkit-8.9/tapinfo.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/tests/macrotest.py` & `skoolkit-8.9/tests/macrotest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1995,23 +1995,23 @@
             "#FORMAT(A={sim[A]},F={sim[F]},BC={sim[BC]},DE={sim[DE]},HL={sim[HL]},A'={sim[^A]},"
             "F'={sim[^F]},BC'={sim[^BC]},DE'={sim[^DE]},HL'={sim[^HL]},IX={sim[IX]},IY={sim[IY]},"
             "I={sim[I]},R={sim[R]},SP={sim[SP]},PC={sim[PC]},tstates={sim[tstates]})"
         )
 
         # First run
         self.assertEqual(writer.expand('#SIM32797,32793,0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,23296'), '')
-        self.assertEqual(writer.expand(macro), "A=2,F=0,BC=260,DE=261,HL=265,A'=7,F'=1,BC'=265,DE'=266,HL'=275,IX=272,IY=272,I=2,R=5,SP=23294,PC=32797,tstates=164")
+        self.assertEqual(writer.expand(macro), "A=2,F=0,BC=260,DE=261,HL=265,A'=7,F'=1,BC'=265,DE'=266,HL'=275,IX=272,IY=272,I=2,R=3,SP=23294,PC=32797,tstates=164")
 
         # Resume
         self.assertEqual(writer.expand('#SIM32792'), '')
-        self.assertEqual(writer.expand(macro), "A=3,F=0,BC=517,DE=518,HL=782,A'=8,F'=9,BC'=522,DE'=523,HL'=797,IX=790,IY=789,I=3,R=5,SP=23294,PC=32792,tstates=300")
+        self.assertEqual(writer.expand(macro), "A=3,F=0,BC=517,DE=518,HL=782,A'=8,F'=9,BC'=522,DE'=523,HL'=797,IX=790,IY=789,I=3,R=3,SP=23294,PC=32792,tstates=300")
 
         # Clear
         self.assertEqual(writer.expand('#SIM32792,32768,1'), '')
-        self.assertEqual(writer.expand(macro), "A=1,F=0,BC=257,DE=257,HL=257,A'=1,F'=0,BC'=257,DE'=257,HL'=257,IX=257,IY=23867,I=1,R=3,SP=23552,PC=32792,tstates=126")
+        self.assertEqual(writer.expand(macro), "A=1,F=0,BC=257,DE=257,HL=257,A'=1,F'=0,BC'=257,DE'=257,HL'=257,IX=257,IY=23867,I=1,R=1,SP=23552,PC=32792,tstates=126")
 
     def test_macro_sim_modifies_internal_memory_snapshot(self):
         skool = """
             @start
             @assemble=2,2
             ; Routine
             c49152 LD (HL),A
```

### Comparing `skoolkit-8.8/tests/skoolkittest.py` & `skoolkit-8.9/tests/skoolkittest.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,26 +51,26 @@
     data_block = create_data_block(data)
     length = len(data_block)
     return [length % 256, length // 256] + data_block
 
 def create_tap_header_block(title='', start=0, length=0, data_type=3):
     return [19, 0] + create_header_block(title, start, length, data_type)
 
-def create_tzx_data_block(data):
+def create_tzx_data_block(data, pause=0):
     block = [16] # Block ID
-    block.extend((0, 0)) # Pause duration
+    block.extend((pause % 256, pause // 256))
     data_block = create_data_block(data)
     length = len(data_block)
     block.extend((length % 256, length // 256))
     block.extend(data_block)
     return block
 
-def create_tzx_header_block(title='', start=0, length=0, data_type=3):
+def create_tzx_header_block(title='', start=0, length=0, data_type=3, pause=0):
     block = [16] # Block ID
-    block.extend((0, 0)) # Pause duration
+    block.extend((pause % 256, pause // 256))
     data_block = create_header_block(title, start, length, data_type)
     length = len(data_block)
     block.extend((length % 256, length // 256))
     block.extend(data_block)
     return block
 
 class Stream:
@@ -210,15 +210,15 @@
         sys.stdin = StdIn(contents)
 
     def _get_z80_ram_block(self, data, compress, page=None):
         if compress:
             block = []
             prev_b = None
             count = 0
-            for b in data + [-1]:
+            for b in data:
                 if b == prev_b or prev_b is None:
                     prev_b = b
                     if count < 255:
                         count += 1
                         continue
                 if count > 4 or (prev_b == 237 and count > 1):
                     block += [237, 237, count, prev_b]
@@ -227,14 +227,18 @@
                     prev_b = None
                     count = 0
                     continue
                 else:
                     block += [prev_b] * count
                 prev_b = b
                 count = 1
+            if count > 4 or (count > 1 and prev_b == 237):
+                block.extend((237, 237, count, prev_b))
+            else:
+                block.extend((prev_b,) * count)
         else:
             block = data
         if page is not None:
             length = len(block) if compress else 65535
             return [length % 256, length // 256, page] + block
         if compress:
             return block + [0, 237, 237, 0]
@@ -250,14 +254,18 @@
         pc = registers.get('PC', 0)
         if version == 1:
             header[6] = pc % 256
             header[7] = pc // 256
         else:
             header[32] = pc % 256
             header[33] = pc // 256
+            if version == 3:
+                t = 69887 - (registers.get('tstates', 0) % 69888)
+                t1, t2 = t % 17472, t // 17472
+                header[55:58] = (t1 % 256, t1 // 256, (2 - t2) % 4)
         sp = registers.get('SP', 0)
         header[8] = sp % 256
         header[9] = sp // 256
         header[10] = registers.get('I', 0)
         r = registers.get('R', 0)
         header[11] = r % 0x80
         header[12] = (header[12] & 0xFE) | (r // 0x80)
```

### Comparing `skoolkit-8.8/tests/test_audio.py` & `skoolkit-8.9/tests/test_audio.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/tests/test_basic.py` & `skoolkit-8.9/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/tests/test_bin2sna.py` & `skoolkit-8.9/tests/test_bin2sna.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,17 +25,17 @@
         self.assertEqual(output, '')
         self.assertEqual(error, '')
         self.assertTrue(os.path.isfile(outfile))
         self.tempfiles.append(outfile)
         return outfile
 
     def _check_z80(self, z80file, data, org=None, sp=None, pc=None, border=7,
-                   iff=1, im=1):
+                   iff=1, im=1, tstates=34943):
         with open(z80file, 'rb') as f:
-            z80h = f.read(34)
+            z80h = f.read(58)
         if org is None:
             org = 65536 - len(data)
         if sp is None:
             sp = org
         if pc is None:
             pc = org
 
@@ -44,14 +44,17 @@
         self.assertEqual(z80h[28], iff)               # IFF2
         self.assertEqual(z80h[29] & 3, im)            # Interrupt mode
 
         self.assertEqual(z80h[8] + 256 * z80h[9], sp)      # SP
         self.assertEqual(z80h[10], 63)                     # I
         self.assertEqual(z80h[23] + 256 * z80h[24], 23610) # IY
         self.assertEqual(z80h[32] + 256 * z80h[33], pc)    # PC
+        t1 = (z80h[55] + 256 * z80h[56]) % 17472
+        t2 = (2 - z80h[57]) % 4
+        self.assertEqual(69887 - t2 * 17472 - t1, tstates)
 
         snapshot = get_snapshot(z80file)
         self.assertEqual(data, snapshot[org:org + len(data)])
 
     def _test_poke(self, option, address, exp_values):
         binfile = self.write_bin_file([0], suffix='.bin')
         z80file = self._run('{} {}'.format(option, binfile))
@@ -352,16 +355,16 @@
             self.assertEqual(error, '')
             infile, outfile, options = run_args
             self.assertEqual(values, options.state)
 
     def test_option_S(self):
         data = [0]
         binfile = self.write_bin_file(data, suffix='.bin')
-        z80file = self._run("-S border=3 --state iff=0 -S im=2 {}".format(binfile))
-        self._check_z80(z80file, data, border=3, iff=0, im=2)
+        z80file = self._run("-S border=3 --state iff=0 -S im=2 --state tstates=100 {}".format(binfile))
+        self._check_z80(z80file, data, border=3, iff=0, im=2, tstates=100)
 
     def test_option_S_invalid_values(self):
         self._test_bad_spec('-S border=k', 'Cannot parse integer: border=k')
         self._test_bad_spec('--state iff=$', 'Cannot parse integer: iff=$')
         self._test_bad_spec('-S im=?', 'Cannot parse integer: im=?')
         self._test_bad_spec('--state bar=1', 'Invalid parameter: bar=1')
 
@@ -369,17 +372,18 @@
         output, error = self.run_bin2sna('--state help')
         self.assertEqual(error, '')
         exp_output = """
             Usage: -S name=value, --state name=value
 
             Set a hardware state attribute. Recognised names and their default values are:
 
-              border - border colour (default=0)
-              iff    - interrupt flip-flop: 0=disabled, 1=enabled (default=1)
-              im     - interrupt mode (default=1)
+              border  - border colour (default=0)
+              iff     - interrupt flip-flop: 0=disabled, 1=enabled (default=1)
+              im      - interrupt mode (default=1)
+              tstates - T-states elapsed since start of frame (default=0)
         """
         self.assertEqual(textwrap.dedent(exp_output).lstrip(), output)
 
     def test_option_V(self):
         for option in ('-V', '--version'):
             output, error = self.run_bin2sna(option, catch_exit=0)
             self.assertEqual(output, 'SkoolKit {}\n'.format(VERSION))
```

### Comparing `skoolkit-8.8/tests/test_bin2tap.py` & `skoolkit-8.9/tests/test_bin2tap.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/tests/test_ctlparser.py` & `skoolkit-8.9/tests/test_ctlparser.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/tests/test_disassembler.py` & `skoolkit-8.9/tests/test_disassembler.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/tests/test_graphics.py` & `skoolkit-8.9/tests/test_graphics.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/tests/test_image.py` & `skoolkit-8.9/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/tests/test_refparser.py` & `skoolkit-8.9/tests/test_refparser.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/tests/test_simulator.py` & `skoolkit-8.9/tests/test_simulator.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         if sna_out:
             actual_memory = {a: simulator.memory[a] for a in sna_out}
             self.assertEqual(actual_memory, sna_out, f"Memory mismatch for '{inst}' ({data_hex}); input: {regvals}")
         if state_out:
             if 'im' in state_out:
                 self.assertEqual(simulator.imode, state_out['im'])
             if 'iff' in state_out:
-                self.assertEqual(simulator.iff2, state_out['iff'])
+                self.assertEqual(simulator.iff, state_out['iff'])
 
     def _test_arithmetic(self, op, opcode1, opcode2, *specs):
         simulator = Simulator([0] * 65536)
         registers = simulator.registers
         memory = simulator.memory
 
         if op in ('AND', 'CP', 'OR', 'SUB', 'XOR'):
@@ -1273,49 +1273,68 @@
                 registers[rh] = rr // 256
                 registers[rl] = rr % 256
                 reg_out = {A: r2, rh: rr // 256, rl: rr % 256}
                 memory[rr] = r1
                 sna_out = {rr: r2}
             self._test_instruction(simulator, operation, data, 7, reg_out, sna_out)
 
-    def test_ld_a_special(self):
-        # LD A,I; LD A,R
+    def test_ld_a_i(self):
+        # LD A,I
         simulator = Simulator([0] * 65536)
         registers = simulator.registers
         a = 29
+        data = (237, 87)
 
-        for opcode, reg, ri in ((87, 'I', I), (95, 'R', R)):
-            for r_in, f_in, f_out in (
-                    # I/R   SZ5H3PNC    SZ5H3PNC
-                    (128, 0b00010110, 0b10000000),
-                    (0,   0b00000100, 0b01000000),
-            ):
-                operation = f'LD A,{reg}'
-                data = (237, opcode)
-                registers[A] = a
-                registers[F] = f_in
-                registers[ri] = r_in
-                reg_out = {A: r_in, F: f_out}
-                self._test_instruction(simulator, operation, data, 9, reg_out)
+        for i_in, f_in, f_out in (
+                # I     SZ5H3PNC    SZ5H3PNC
+                (128, 0b00010110, 0b10000000),
+                (0,   0b00000100, 0b01000000),
+        ):
+            operation = 'LD A,I'
+            registers[A] = a
+            registers[F] = f_in
+            registers[I] = i_in
+            reg_out = {A: i_in, F: f_out}
+            self._test_instruction(simulator, operation, data, 9, reg_out)
+
+    def test_ld_a_r(self):
+        # LD A,R
+        simulator = Simulator([0] * 65536)
+        registers = simulator.registers
+        a = 29
+        data = (237, 95)
+
+        for r_in, r_out, f_in, f_out in (
+                #            SZ5H3PNC    SZ5H3PNC
+                (126, 0,   0b10010110, 0b01000000),
+                (128, 130, 0b00010110, 0b10000000),
+                (254, 128, 0b00000100, 0b10000000),
+        ):
+            operation = 'LD A,R'
+            registers[A] = a
+            registers[F] = f_in
+            registers[R] = r_in
+            reg_out = {A: r_out, F: f_out}
+            self._test_instruction(simulator, operation, data, 9, reg_out)
 
     def test_ld_special_a(self):
         # LD I,A; LD R,A
         simulator = Simulator([0] * 65536)
         registers = simulator.registers
         r, a = 2, 99
 
-        for opcode, reg, ri, r_out in (
-                (71, 'I', I, a),
-                (79, 'R', R, a + 2)
+        for opcode, reg, ri in (
+                (71, 'I', I),
+                (79, 'R', R)
         ):
             operation = f'LD {reg},A'
             data = (237, opcode)
             registers[ri] = r
             registers[A] = a
-            reg_out = {ri: r_out}
+            reg_out = {ri: a}
             self._test_instruction(simulator, operation, data, 9, reg_out)
 
     def test_ld_rr_nn(self):
         simulator = Simulator([0] * 65536)
         registers = simulator.registers
         lsb, msb = 3, 6
 
@@ -1576,14 +1595,27 @@
         operation = f'CALL ${addr:04X}'
         data = (205, addr % 256, addr // 256)
         registers[SP] = sp
         reg_out = {SP: sp - 2}
         sna_out = {sp - 1: (start + 3) // 256, sp - 2: (start + 3) % 256}
         self._test_instruction(simulator, operation, data, 17, reg_out, sna_out, start=start, end=addr)
 
+    def test_call_nn_overwriting_its_operand(self):
+        simulator = Simulator([0] * 65536)
+        registers = simulator.registers
+        start = 30000
+        addr = 51426
+        sp = start + 3
+        operation = f'CALL ${addr:04X}'
+        data = (205, addr % 256, addr // 256)
+        registers[SP] = sp
+        reg_out = {SP: sp - 2}
+        sna_out = {sp - 1: (start + 3) // 256, sp - 2: (start + 3) % 256}
+        self._test_instruction(simulator, operation, data, 17, reg_out, sna_out, start=start, end=addr)
+
     def test_call_conditional(self):
         simulator = Simulator([0] * 65536)
         registers = simulator.registers
         start = 40000
         addr = 45271
         sp = 23456
 
@@ -1616,14 +1648,40 @@
             else:
                 timing = 10
                 reg_out = None
                 sna_out = None
             data = (opcode, addr % 256, addr // 256)
             self._test_instruction(simulator, operation, data, timing, reg_out, sna_out, start=start, end=end)
 
+    def test_call_conditional_overwriting_its_operand(self):
+        simulator = Simulator([0] * 65536)
+        registers = simulator.registers
+        start = 40000
+        addr = 45271
+        sp = start + 3
+
+        for opcode, condition, flags in (
+                #             SZ5H3PNC
+                (196, 'NZ', 0b00000000),
+                (204, 'Z',  0b01000000),
+                (212, 'NC', 0b00000000),
+                (220, 'C',  0b00000001),
+                (228, 'PO', 0b00000000),
+                (236, 'PE', 0b00000100),
+                (244, 'P',  0b00000000),
+                (252, 'M',  0b10000000),
+        ):
+            operation = f'CALL {condition},${addr:04X}'
+            registers[F] = flags
+            registers[SP] = sp
+            reg_out = {SP: sp - 2}
+            sna_out = {sp - 1: (start + 3) // 256, sp - 2: (start + 3) % 256}
+            data = (opcode, addr % 256, addr // 256)
+            self._test_instruction(simulator, operation, data, 17, reg_out, sna_out, start=start, end=addr)
+
     def test_jp_nn(self):
         simulator = Simulator([0] * 65536)
         start = 30000
         addr = 51426
         operation = f'JP ${addr:04X}'
         data = (195, addr % 256, addr // 256)
         self._test_instruction(simulator, operation, data, 10, start=start, end=addr)
@@ -1780,15 +1838,15 @@
         self._test_instruction(simulator, operation, data, 12)
 
     def test_in_a_n(self):
         simulator = Simulator([0] * 65536)
         n = 56
         operation = f'IN A,(${n:02X})'
         data = (0xDB, n)
-        reg_out = {A: 191}
+        reg_out = {A: 255}
         self._test_instruction(simulator, operation, data, 11, reg_out)
 
     def test_in_r_c(self):
         simulator = Simulator([0] * 65536)
         registers = simulator.registers
         tracer = InTestTracer()
         simulator.set_tracer(tracer)
@@ -1810,15 +1868,15 @@
             in_value ^= 255
             self._test_instruction(simulator, operation, data, 12, reg_out)
 
     def test_in_f_c(self):
         simulator = Simulator([0] * 65536)
         operation = f'IN F,(C)'
         data = (0xED, 0x70)
-        reg_out = {F: 0b10101000}
+        reg_out = {F: 0b10101100}
         self._test_instruction(simulator, operation, data, 12, reg_out)
 
     def test_djnz(self):
         simulator = Simulator([0] * 65536)
         registers = simulator.registers
         addr = 35732
 
@@ -2738,7 +2796,96 @@
         memory = [0] * 65536
         start = 32768
         memory[start:start + 2] = (0xED, 0x57) # LD A,I
         simulator = Simulator(memory, state={'iff': 1})
         simulator.run(start)
         self.assertEqual(simulator.registers[PC], start + 2)
         self.assertEqual(simulator.registers[F], 0b00101100)
+
+    def test_accept_interrupt_mode_0(self):
+        pc = 30000
+        sp = 40000
+        simulator = Simulator([0] * 65536, {'PC': pc, 'SP': sp}, {'iff': 1, 'im': 0})
+        blocked = simulator.accept_interrupt(simulator.registers, simulator.memory, pc - 1)
+        self.assertFalse(blocked)
+        self.assertEqual(simulator.registers[T], 13)
+        self.assertEqual(simulator.registers[PC], 56)
+        self.assertEqual(simulator.registers[R], 1)
+        self.assertEqual(simulator.registers[SP], sp - 2)
+        self.assertEqual([pc % 256, pc // 256], simulator.memory[sp - 2:sp])
+        self.assertEqual(simulator.iff, 0)
+
+    def test_accept_interrupt_mode_1(self):
+        pc = 40000
+        sp = 50000
+        simulator = Simulator([0] * 65536, {'PC': pc, 'SP': sp}, {'iff': 1, 'im': 1})
+        blocked = simulator.accept_interrupt(simulator.registers, simulator.memory, pc - 1)
+        self.assertFalse(blocked)
+        self.assertEqual(simulator.registers[T], 13)
+        self.assertEqual(simulator.registers[PC], 56)
+        self.assertEqual(simulator.registers[R], 1)
+        self.assertEqual(simulator.registers[SP], sp - 2)
+        self.assertEqual([pc % 256, pc // 256], simulator.memory[sp - 2:sp])
+        self.assertEqual(simulator.iff, 0)
+
+    def test_accept_interrupt_mode_2(self):
+        memory = [0] * 65536
+        iaddr = 40000
+        i = 64
+        vaddr = 255 + 256 * i
+        memory[vaddr:vaddr + 2] = (iaddr % 256, iaddr // 256)
+        pc = 50000
+        sp = 60000
+        simulator = Simulator(memory, {'PC': pc, 'SP': sp, 'I': i}, {'iff': 1, 'im': 2})
+        blocked = simulator.accept_interrupt(simulator.registers, simulator.memory, pc - 1)
+        self.assertFalse(blocked)
+        self.assertEqual(simulator.registers[T], 19)
+        self.assertEqual(simulator.registers[PC], iaddr)
+        self.assertEqual(simulator.registers[R], 1)
+        self.assertEqual(simulator.registers[SP], sp - 2)
+        self.assertEqual([pc % 256, pc // 256], simulator.memory[sp - 2:sp])
+        self.assertEqual(simulator.iff, 0)
+
+    def test_accept_interrupt_after_ei(self):
+        memory = [0] * 65536
+        pc = 30000
+        sp = 40000
+        memory[pc - 1] = 0xFB # EI
+        simulator = Simulator(memory, {'PC': pc, 'SP': sp}, {'iff': 1, 'im': 1})
+        blocked = simulator.accept_interrupt(simulator.registers, simulator.memory, pc - 1)
+        self.assertTrue(blocked)
+        self.assertEqual(simulator.registers[T], 0)
+        self.assertEqual(simulator.registers[PC], pc)
+        self.assertEqual(simulator.registers[R], 0)
+        self.assertEqual(simulator.registers[SP], sp)
+        self.assertEqual([0, 0], simulator.memory[sp - 2:sp])
+        self.assertEqual(simulator.iff, 1)
+
+    def test_accept_interrupt_after_dd_prefix(self):
+        memory = [0] * 65536
+        pc = 30000
+        sp = 40000
+        memory[pc - 1] = 0xDD
+        simulator = Simulator(memory, {'PC': pc, 'SP': sp}, {'iff': 1, 'im': 1})
+        blocked = simulator.accept_interrupt(simulator.registers, simulator.memory, pc - 1)
+        self.assertTrue(blocked)
+        self.assertEqual(simulator.registers[T], 0)
+        self.assertEqual(simulator.registers[PC], pc)
+        self.assertEqual(simulator.registers[R], 0)
+        self.assertEqual(simulator.registers[SP], sp)
+        self.assertEqual([0, 0], simulator.memory[sp - 2:sp])
+        self.assertEqual(simulator.iff, 1)
+
+    def test_accept_interrupt_after_fd_prefix(self):
+        memory = [0] * 65536
+        pc = 30000
+        sp = 40000
+        memory[pc - 1] = 0xFD
+        simulator = Simulator(memory, {'PC': pc, 'SP': sp}, {'iff': 1, 'im': 1})
+        blocked = simulator.accept_interrupt(simulator.registers, simulator.memory, pc - 1)
+        self.assertTrue(blocked)
+        self.assertEqual(simulator.registers[T], 0)
+        self.assertEqual(simulator.registers[PC], pc)
+        self.assertEqual(simulator.registers[R], 0)
+        self.assertEqual(simulator.registers[SP], sp)
+        self.assertEqual([0, 0], simulator.memory[sp - 2:sp])
+        self.assertEqual(simulator.iff, 1)
```

### Comparing `skoolkit-8.8/tests/test_skool2asm.py` & `skoolkit-8.9/tests/test_skool2asm.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/tests/test_skool2bin.py` & `skoolkit-8.9/tests/test_skool2bin.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/tests/test_skool2ctl.py` & `skoolkit-8.9/tests/test_skool2ctl.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/tests/test_skool2html.py` & `skoolkit-8.9/tests/test_skool2html.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/tests/test_skoolasm.py` & `skoolkit-8.9/tests/test_skoolasm.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/tests/test_skoolctl.py` & `skoolkit-8.9/tests/test_skoolctl.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/tests/test_skoolhtml.py` & `skoolkit-8.9/tests/test_skoolhtml.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/tests/test_skoolkit.py` & `skoolkit-8.9/tests/test_skoolkit.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/tests/test_skoolmacro.py` & `skoolkit-8.9/tests/test_skoolmacro.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/tests/test_skoolparser.py` & `skoolkit-8.9/tests/test_skoolparser.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/tests/test_sna2ctl.py` & `skoolkit-8.9/tests/test_sna2ctl.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/tests/test_sna2img.py` & `skoolkit-8.9/tests/test_sna2img.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/tests/test_sna2skool.py` & `skoolkit-8.9/tests/test_sna2skool.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/tests/test_snapinfo.py` & `skoolkit-8.9/tests/test_snapinfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -981,14 +981,26 @@
         exp_output = """
             31783-31787-2 7C27-7C2B-2: 8,10,13
             42567-42573-3 A647-A64D-3: 8,10,13
             52172-52180-4 CBCC-CBD4-4: 8,10,13
         """
         self._test_sna(ram, exp_output, '-f {}-1-5'.format(seq_str))
 
+    def test_option_f_with_address_below_16384(self):
+        data = [0] * 256
+        address = 135
+        seq = (2, 4, 6)
+        data[address:address + len(seq)] = seq
+        seq_str = ','.join([str(b) for b in seq])
+        binfile = self.write_bin_file(data, suffix='.bin')
+        exp_output = '135-137-1 0087-0089-1: {}'.format(seq_str)
+        output, error = self.run_snapinfo(f'-f {seq_str} -o 0 {binfile}')
+        self.assertEqual(error, '')
+        self.assertEqual(output.strip(), exp_output)
+
     def test_option_f_with_hexadecimal_values(self):
         ram = [0] * 49152
         address = 47983
         seq = (0x02, 0x3f, 0x5a)
         step = 0x1a
         ram[address - 16384:address - 16384 + step * len(seq):step] = seq
         seq_str = ','.join(['${:02X}'.format(b) for b in seq])
@@ -1728,14 +1740,25 @@
         self._test_sna(ram, exp_output, '--find-text {}'.format(text))
 
     def test_option_t_with_no_occurrences(self):
         ram = [0] * 49152
         exp_output = ''
         self._test_sna(ram, exp_output, '-t nowhere')
 
+    def test_option_t_with_address_below_16384(self):
+        data = [0] * 256
+        address = 204
+        text = 'hello'
+        data[address:address + len(text)] = [ord(c) for c in text]
+        binfile = self.write_bin_file(data, suffix='.bin')
+        exp_output = f'204-208 00CC-00D0: {text}'
+        output, error = self.run_snapinfo(f'-t {text} -o 0 {binfile}')
+        self.assertEqual(error, '')
+        self.assertEqual(output.strip(), exp_output)
+
     def test_option_T(self):
         ram = [0] * 49152
         tile_addr = 54212
         tile_data = [0, 24, 12, 6, 127, 6, 12, 24]
         x, y = 3, 7
         df_addr = 16384 + 2048 * (y // 8) + 32 * (y & 7) + x
         ram[df_addr - 16384:df_addr - 14336:256] = tile_data
```

### Comparing `skoolkit-8.8/tests/test_snapmod.py` & `skoolkit-8.9/tests/test_snapmod.py`

 * *Files 1% similar despite different names*

```diff
@@ -383,15 +383,16 @@
         header = [0] * 86
         header[30] = 54 # Version 3
         exp_header = header[:]
         exp_header[12] |= 4 # BORDER 2
         exp_header[27] = 1 # IFF 1
         exp_header[28] = 1 # IFF 2
         exp_header[29] = (header[29] & 252) | 2 # IM 2
-        options = '-s border=2 -s iff=1 -s im=2'
+        exp_header[55:58] = (158, 4, 1) # T-states
+        options = '-s border=2 -s iff=1 -s im=2 -s tstates=51233'
         self._test_z80(options, header, exp_header)
 
     def test_option_s_invalid_values(self):
         infile = self.write_z80_file([1] * 30, [0] * 49152, 1)
         self._test_bad_spec('-s border=k', infile, 'Cannot parse integer: border=k')
         self._test_bad_spec('-s iff=$', infile, 'Cannot parse integer: iff=$')
         self._test_bad_spec('-s im=?', infile, 'Cannot parse integer: im=?')
@@ -401,17 +402,18 @@
         output, error = self.run_snapmod('--state help')
         self.assertEqual(error, '')
         exp_output = """
             Usage: -s name=value, --state name=value
 
             Set a hardware state attribute. Recognised names and their default values are:
 
-              border - border colour (default=0)
-              iff    - interrupt flip-flop: 0=disabled, 1=enabled (default=1)
-              im     - interrupt mode (default=1)
+              border  - border colour (default=0)
+              iff     - interrupt flip-flop: 0=disabled, 1=enabled (default=1)
+              im      - interrupt mode (default=1)
+              tstates - T-states elapsed since start of frame (default=0)
         """
         self.assertEqual(textwrap.dedent(exp_output).lstrip(), output)
 
     def test_option_V(self):
         for option in ('-V', '--version'):
             output, error = self.run_snapmod(option, catch_exit=0)
             self.assertEqual(output, 'SkoolKit {}\n'.format(VERSION))
```

### Comparing `skoolkit-8.8/tests/test_snapshot.py` & `skoolkit-8.9/tests/test_snapshot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from skoolkittest import SkoolKitTestCase
-from skoolkit.snapshot import get_snapshot, make_z80_ram_block, SnapshotError
+from skoolkit.snapshot import get_snapshot, make_z80_ram_block, set_z80_state, SnapshotError
 
 class SnapshotTest(SkoolKitTestCase):
     def _check_ram(self, ram, exp_ram, model, out_7ffd, pages, page):
         self.assertEqual(len(ram), 49152)
         if model == 0:
             # 16K
             self.assertEqual(ram[:16384], exp_ram[:16384])
@@ -142,14 +142,19 @@
         self._test_z80(exp_ram, 3, False, machine_id=4)
 
     def test_z80v3_128k_page_4(self):
         exp_ram = [(n + 37) & 255 for n in range(49152)]
         pages = {4: [(n + 249) & 255 for n in range(16384)]}
         self._test_z80(exp_ram, 3, False, machine_id=4, pages=pages, page=4)
 
+    def test_z80v3_48k_compressed_block_ending_with_ED(self):
+        exp_ram = [0] * 49152
+        exp_ram[16383] = 237
+        self._test_z80(exp_ram, 3, True)
+
     def test_bad_z80(self):
         header = [0] * 30
         header[6] = 255 # Set PC > 0 to indicate a v1 Z80 snapshot
         header[12] |= 32 # Signal that the RAM data block is compressed
         z80 = header + [255] # Good byte to start with
         z80 += [237, 237, 0, 11] # Bad block of length 0
         z80 += [0, 237, 237, 0] # Terminator
@@ -171,14 +176,51 @@
         self.assertEqual(exp_data, block)
 
     def test_block_ending_with_single_ED(self):
         data = [0, 237]
         exp_data = [2, 0, 0, 0, 237]
         self.assertEqual(exp_data, make_z80_ram_block(data, 0))
 
+class Z80StateTest(SkoolKitTestCase):
+    def test_iff(self):
+        header = [255] * 30
+        for iff in (0, 1):
+            set_z80_state(header, f'iff={iff}')
+            self.assertEqual([iff, iff], header[27:29])
+
+    def test_im(self):
+        header = [255] * 30
+        for im in (0, 1, 2):
+            set_z80_state(header, f'im={im}')
+            self.assertEqual(header[29], 252 + im)
+
+    def test_border(self):
+        header = [255] * 30
+        for border in range(8):
+            set_z80_state(header, f'border={border}')
+            self.assertEqual(header[12], 241 + border * 2)
+
+    def test_tstates(self):
+        header = [255] * 58
+        for tstates in (0, 1000, 17471, 17472, 20000, 38000, 56000, 69887, 69888):
+            set_z80_state(header, f'tstates={tstates}')
+            t_lo = header[55] + 256 * header[56]
+            t_hi = header[57]
+            t = 69887 - ((2 - t_hi) % 4) * 17472 - (t_lo % 17472)
+            self.assertEqual(t, tstates % 69888)
+
+    def test_all(self):
+        header = [255] * 58
+        set_z80_state(header, 'iff=0', 'im=2', 'border=3', 'tstates=17471')
+        self.assertEqual(header[27], 0) # IFF1
+        self.assertEqual(header[28], 0) # IFF2
+        self.assertEqual(header[29], 254) # IM (bits 0-1)
+        self.assertEqual(header[12], 247) # Border (bits 1-3)
+        self.assertEqual([0, 0, 3], header[55:58]) # T-states
+
 class SZXTest(SnapshotTest):
     def _test_szx(self, exp_ram, compress, machine_id=1, ch7ffd=0, pages={}, page=None):
         tmp_szx = self.write_szx(exp_ram, compress, machine_id, ch7ffd, pages)
         snapshot = get_snapshot(tmp_szx, page)
         self._check_ram(snapshot[16384:], exp_ram, machine_id, ch7ffd, pages, page)
 
     def test_szx_16k(self):
```

### Comparing `skoolkit-8.8/tests/test_snaskool.py` & `skoolkit-8.9/tests/test_snaskool.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/tests/test_tap2sna.py` & `skoolkit-8.9/tests/test_tap2sna.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import hashlib
 import os
 import textwrap
 import urllib
 from zipfile import ZipFile
 from io import BytesIO
 from unittest.mock import patch, Mock
 
@@ -65,18 +66,18 @@
     def _get_snapshot(self, start=16384, data=None, options='', load_options=None, blocks=None, tzx=False):
         if blocks is None:
             blocks = [create_tap_data_block(data)]
         if tzx:
             tape_file = self._write_tzx(blocks)
         else:
             tape_file = self._write_tap(blocks)
-        z80file = self.write_bin_file(suffix='.z80')
+        z80file = '{}/out.z80'.format(self.make_directory())
         if load_options is None:
             load_options = '--ram load=1,{}'.format(start)
-        output, error = self.run_tap2sna('--force {} {} {} {}'.format(load_options, options, tape_file, z80file))
+        output, error = self.run_tap2sna(f'{load_options} {options} {tape_file} {z80file}')
         self.assertEqual(output, 'Writing {}\n'.format(z80file))
         self.assertEqual(error, '')
         return get_snapshot(z80file)
 
     def _test_bad_spec(self, option, exp_error):
         odir = self.make_directory()
         tapfile = self._write_tap([create_tap_data_block([1])])
@@ -92,40 +93,75 @@
         self.assertIsNone(options.output_dir)
         self.assertFalse(options.force)
         self.assertIsNone(options.stack)
         self.assertEqual([], options.ram_ops)
         self.assertEqual([], options.reg)
         self.assertIsNone(options.start)
         self.assertFalse(options.sim_load)
+        self.assertEqual([], options.sim_load_config)
         self.assertEqual([], options.state)
+        self.assertIsNone(options.tape_name)
+        self.assertEqual(options.tape_start, 1)
+        self.assertEqual(options.tape_stop, 0)
+        self.assertIsNone(options.tape_sum)
         self.assertEqual(options.user_agent, '')
 
     def test_no_arguments(self):
         output, error = self.run_tap2sna(catch_exit=2)
         self.assertEqual(output, '')
         self.assertTrue(error.startswith('usage:'))
 
     def test_invalid_arguments(self):
         for args in ('--foo', '-k test.zip'):
             output, error = self.run_tap2sna(args, catch_exit=2)
             self.assertEqual(output, '')
             self.assertTrue(error.startswith('usage:'))
 
+    def test_accelerator_unrecognised(self):
+        blocks = [create_tap_data_block([0])]
+        tapfile = self._write_tap(blocks)
+        z80file = '{}/out.z80'.format(self.make_directory())
+        with self.assertRaises(SkoolKitError) as cm:
+            self.run_tap2sna(f'-c accelerator=nope --sim-load {tapfile} {z80file}')
+        self.assertEqual(cm.exception.args[0], 'Error while getting snapshot out.z80: Unrecognised accelerator: nope')
+        self.assertEqual(self.err.getvalue(), '')
+
+    def test_unrecognised_sim_load_configuration_parameter(self):
+        blocks = [create_tap_data_block([0])]
+        tapfile = self._write_tap(blocks)
+        z80file = '{}/out.z80'.format(self.make_directory())
+        with self.assertRaises(SkoolKitError) as cm:
+            self.run_tap2sna(f'-c foo=bar --sim-load {tapfile} {z80file}')
+        self.assertEqual(cm.exception.args[0], 'Error while getting snapshot out.z80: Invalid sim-load configuration parameter: foo')
+        self.assertEqual(self.err.getvalue(), '')
+
     def test_option_d(self):
         odir = '{}/tap2sna'.format(self.make_directory())
         tapfile = self._write_tap((
             create_tap_header_block(start=16384),
             create_tap_data_block([0])
         ))
         z80_fname = 'test.z80'
         for option in ('-d', '--output-dir'):
             output, error = self.run_tap2sna('{} {} {} {}'.format(option, odir, tapfile, z80_fname))
             self.assertEqual(len(error), 0)
             self.assertTrue(os.path.isfile(os.path.join(odir, z80_fname)))
 
+    def test_option_f(self):
+        z80file = self.write_bin_file(suffix='.z80')
+        for option, b in (('-f', 1), ('--force', 255)):
+            tapfile = self._write_tap((
+                create_tap_header_block(start=16384),
+                create_tap_data_block([b])
+            ))
+            output, error = self.run_tap2sna(f'{option} {tapfile} {z80file}')
+            self.assertEqual(len(error), 0)
+            snapshot = get_snapshot(z80file)
+            self.assertEqual(snapshot[16384], b)
+
     @patch.object(tap2sna, 'make_z80', mock_make_z80)
     def test_options_p_stack(self):
         for option, stack in (('-p', 24576), ('--stack', 49152)):
             output, error = self.run_tap2sna('{} {} in.tap {}/out.z80'.format(option, stack, self.make_directory()))
             self.assertEqual(output, '')
             self.assertEqual(error, '')
             url, options, z80 = make_z80_args
@@ -141,18 +177,17 @@
             self.assertEqual(['sp={}'.format(int(stack[2:], 16))], options.reg)
 
     def test_option_p(self):
         tapfile = self._write_tap((
             create_tap_header_block(start=16384),
             create_tap_data_block([0])
         ))
-        z80file = self.write_bin_file(suffix='.z80')
+        z80file = '{}/out.z80'.format(self.make_directory())
         stack = 32768
-
-        output, error = self.run_tap2sna('-f -p {} {} {}'.format(stack, tapfile, z80file))
+        output, error = self.run_tap2sna(f'-p {stack} {tapfile} {z80file}')
         self.assertEqual(error, '')
         with open(z80file, 'rb') as f:
             z80_header = f.read(10)
         self.assertEqual(z80_header[8] + 256 * z80_header[9], stack)
 
     @patch.object(tap2sna, 'make_z80', mock_make_z80)
     def test_options_s_start(self):
@@ -177,24 +212,147 @@
             self.assertEqual(exp_reg, options.reg)
 
     def test_option_s(self):
         tapfile = self._write_tap((
             create_tap_header_block(start=16384),
             create_tap_data_block([0])
         ))
-        z80file = self.write_bin_file(suffix='.z80')
+        z80file = '{}/out.z80'.format(self.make_directory())
         start = 40000
-
-        output, error = self.run_tap2sna('-f -s {} {} {}'.format(start, tapfile, z80file))
+        output, error = self.run_tap2sna(f'-s {start} {tapfile} {z80file}')
         self.assertEqual(error, '')
         with open(z80file, 'rb') as f:
             z80_header = f.read(34)
         self.assertEqual(z80_header[32] + 256 * z80_header[33], start)
 
     @patch.object(tap2sna, '_write_z80', mock_write_z80)
+    def test_option_tape_name(self):
+        code1 = [1, 2, 3, 4, 5]
+        code1_start = 24576
+        tap1_data = create_tap_header_block(start=code1_start) + create_tap_data_block(code1)
+        tap1_fname = 'code1.tap'
+        code2 = [6, 7, 8]
+        code2_start = 32768
+        tap2_data = create_tap_header_block(start=code2_start) + create_tap_data_block(code2)
+        tap2_fname = 'code2.tap'
+        zipfile = '{}/tapes.zip'.format(self.make_directory())
+        with ZipFile(zipfile, 'w') as archive:
+            archive.writestr(tap1_fname, bytearray(tap1_data))
+            archive.writestr(tap2_fname, bytearray(tap2_data))
+        output, error = self.run_tap2sna(f'--tape-name {tap2_fname} {zipfile} out.z80')
+        self.assertEqual(error, '')
+        self.assertEqual([0] * len(code1), snapshot[code1_start:code1_start + len(code1)])
+        self.assertEqual(code2, snapshot[code2_start:code2_start + len(code2)])
+
+    def test_option_tape_name_with_invalid_name(self):
+        tap_data = create_tap_header_block(start=32768) + create_tap_data_block([1, 2, 3])
+        zipfile = '{}/tape.zip'.format(self.make_directory())
+        with ZipFile(zipfile, 'w') as archive:
+            archive.writestr('data.tap', bytearray(tap_data))
+        with self.assertRaises(SkoolKitError) as cm:
+            self.run_tap2sna(f'--tape-name code.tap {zipfile} out.z80')
+        self.assertEqual(cm.exception.args[0], 'Error while getting snapshot out.z80: No file named "code.tap" in the archive')
+        self.assertEqual(self.err.getvalue(), '')
+
+    @patch.object(tap2sna, '_write_z80', mock_write_z80)
+    def test_option_tape_start_with_tap_file(self):
+        code1_start = 24576
+        code2_start = 32768
+        code = [4, 5, 6]
+        blocks = [
+            create_tap_header_block(start=code1_start),
+            create_tap_data_block(code),
+            create_tap_header_block(start=code2_start),
+            create_tap_data_block(code)
+        ]
+        tapfile = self._write_tap(blocks)
+        output, error = self.run_tap2sna(f'--tape-start 3 {tapfile} out.z80')
+        self.assertEqual(error, '')
+        self.assertEqual([0] * len(code), snapshot[code1_start:code1_start + len(code)])
+        self.assertEqual(code, snapshot[code2_start:code2_start + len(code)])
+
+    @patch.object(tap2sna, '_write_z80', mock_write_z80)
+    def test_option_tape_start_with_tzx_file(self):
+        code1_start = 24576
+        code2_start = 32768
+        code = [4, 5, 6]
+        blocks = [
+            create_tzx_header_block(start=code1_start),
+            create_tzx_data_block(code),
+            create_tzx_header_block(start=code2_start),
+            create_tzx_data_block(code)
+        ]
+        tzxfile = self._write_tzx(blocks)
+        output, error = self.run_tap2sna(f'--tape-start 3 {tzxfile} out.z80')
+        self.assertEqual(error, '')
+        self.assertEqual([0] * len(code), snapshot[code1_start:code1_start + len(code)])
+        self.assertEqual(code, snapshot[code2_start:code2_start + len(code)])
+
+    @patch.object(tap2sna, '_write_z80', mock_write_z80)
+    def test_option_tape_stop_with_tap_file(self):
+        code1_start = 24576
+        code2_start = 32768
+        code = [4, 5, 6]
+        blocks = [
+            create_tap_header_block(start=code1_start),
+            create_tap_data_block(code),
+            create_tap_header_block(start=code2_start),
+            create_tap_data_block(code)
+        ]
+        tapfile = self._write_tap(blocks)
+        output, error = self.run_tap2sna(f'--tape-stop 3 {tapfile} out.z80')
+        self.assertEqual(error, '')
+        self.assertEqual(code, snapshot[code1_start:code1_start + len(code)])
+        self.assertEqual([0] * len(code), snapshot[code2_start:code2_start + len(code)])
+
+    @patch.object(tap2sna, '_write_z80', mock_write_z80)
+    def test_option_tape_stop_with_tzx_file(self):
+        code1_start = 24576
+        code2_start = 32768
+        code = [4, 5, 6]
+        blocks = [
+            create_tzx_header_block(start=code1_start),
+            create_tzx_data_block(code),
+            create_tzx_header_block(start=code2_start),
+            create_tzx_data_block(code)
+        ]
+        tzxfile = self._write_tzx(blocks)
+        output, error = self.run_tap2sna(f'--tape-stop 3 {tzxfile} out.z80')
+        self.assertEqual(error, '')
+        self.assertEqual(code, snapshot[code1_start:code1_start + len(code)])
+        self.assertEqual([0] * len(code), snapshot[code2_start:code2_start + len(code)])
+
+    @patch.object(tap2sna, '_write_z80', mock_write_z80)
+    def test_option_tape_sum(self):
+        code = [1, 2, 3]
+        code_start = 49152
+        tap_data = create_tap_header_block(start=code_start) + create_tap_data_block(code)
+        md5sum = hashlib.md5(bytearray(tap_data)).hexdigest()
+        zipfile = '{}/tape.zip'.format(self.make_directory())
+        with ZipFile(zipfile, 'w') as archive:
+            archive.writestr('data.tap', bytearray(tap_data))
+        output, error = self.run_tap2sna(f'--tape-sum {md5sum} {zipfile} out.z80')
+        self.assertEqual(error, '')
+        self.assertEqual(code, snapshot[code_start:code_start + len(code)])
+
+    def test_option_tape_sum_with_incorrect_value(self):
+        code = [1, 2, 3]
+        code_start = 49152
+        tap_data = create_tap_header_block(start=code_start) + create_tap_data_block(code)
+        md5sum = hashlib.md5(bytearray(tap_data)).hexdigest()
+        zipfile = '{}/tape.zip'.format(self.make_directory())
+        wrongsum = '0' * 32
+        with ZipFile(zipfile, 'w') as archive:
+            archive.writestr('data.tap', bytearray(tap_data))
+        with self.assertRaises(SkoolKitError) as cm:
+            self.run_tap2sna(f'--tape-sum {wrongsum} {zipfile} out.z80')
+        self.assertEqual(cm.exception.args[0], f'Error while getting snapshot out.z80: Checksum mismatch: Expected {wrongsum}, actually {md5sum}')
+        self.assertEqual(self.err.getvalue(), '')
+
+    @patch.object(tap2sna, '_write_z80', mock_write_z80)
     @patch.object(tap2sna, 'urlopen')
     def test_option_u(self, mock_urlopen):
         mock_urlopen.return_value = BytesIO(bytes(create_tap_data_block([1])))
         url = 'http://example.com/test.tap'
         for option, user_agent in (('-u', 'Wget/1.18'), ('--user-agent', 'SkoolKit/6.3')):
             output, error = self.run_tap2sna('{} {} --ram load=1,23296 {} {}/test.z80'.format(option, user_agent, url, self.make_directory()))
             self.assertTrue(output.startswith('Downloading {}\n'.format(url)))
@@ -241,16 +399,16 @@
             create_tap_header_block(data_type=0),
             create_tap_data_block(basic_data),
             create_tap_header_block(start=code_start),
             create_tap_data_block(code)
         ]
 
         tapfile = self._write_tap(blocks)
-        z80file = self.write_bin_file(suffix='.z80')
-        output, error = self.run_tap2sna('--force {} {}'.format(tapfile, z80file))
+        z80file = '{}/out.z80'.format(self.make_directory())
+        output, error = self.run_tap2sna(f'{tapfile} {z80file}')
         self.assertEqual(error, '')
         snapshot = get_snapshot(z80file)
         self.assertEqual(basic_data, snapshot[23755:23755 + len(basic_data)])
         self.assertEqual(code, snapshot[code_start:code_start + len(code)])
 
     def test_standard_load_ignores_headerless_block(self):
         code_start = 16384
@@ -259,16 +417,16 @@
             create_tap_header_block(start=code_start),
             create_tap_data_block(code),
             create_tap_data_block([23]),
             create_tap_data_block([97])
         ]
 
         tapfile = self._write_tap(blocks)
-        z80file = self.write_bin_file(suffix='.z80')
-        output, error = self.run_tap2sna('--force {} {}'.format(tapfile, z80file))
+        z80file = '{}/out.z80'.format(self.make_directory())
+        output, error = self.run_tap2sna(f'{tapfile} {z80file}')
         self.assertEqual(
             error,
             'WARNING: Ignoring headerless block 3\n'
             'WARNING: Ignoring headerless block 4\n'
         )
         snapshot = get_snapshot(z80file)
         self.assertEqual(code, snapshot[code_start:code_start + len(code)])
@@ -279,31 +437,31 @@
         length = len(code)
         blocks = [
             create_tap_header_block(start=code_start)[:-1],
             create_tap_data_block(code),
         ]
 
         tapfile = self._write_tap(blocks)
-        z80file = self.write_bin_file(suffix='.z80')
-        output, error = self.run_tap2sna('--force {} {}'.format(tapfile, z80file))
+        z80file = '{}/out.z80'.format(self.make_directory())
+        output, error = self.run_tap2sna(f'{tapfile} {z80file}')
         self.assertEqual(error, '')
         snapshot = get_snapshot(z80file)
         self.assertEqual([0] * length, snapshot[code_start:code_start + length])
 
     def test_standard_load_with_unknown_block_type(self):
         block_type = 1 # Array of numbers
         blocks = [
             create_tap_header_block(data_type=block_type),
             create_tap_data_block([1])
         ]
 
         tapfile = self._write_tap(blocks)
-        z80file = self.write_bin_file(suffix='.z80')
+        z80file = 'out.z80'
         with self.assertRaises(SkoolKitError) as cm:
-            self.run_tap2sna('--force {} {}'.format(tapfile, z80file))
+            self.run_tap2sna('{} {}'.format(tapfile, z80file))
         self.assertEqual(cm.exception.args[0], 'Error while getting snapshot {}: Unknown block type ({}) in header block 1'.format(z80file, block_type))
 
     def test_standard_load_from_tzx_file(self):
         basic_data = [6, 7]
         code_start = 49152
         code = [8, 9, 10]
         blocks = [
@@ -311,16 +469,16 @@
             create_tzx_header_block(data_type=0),
             create_tzx_data_block(basic_data),
             create_tzx_header_block(start=code_start),
             create_tzx_data_block(code)
         ]
 
         tzxfile = self._write_tzx(blocks)
-        z80file = self.write_bin_file(suffix='.z80')
-        output, error = self.run_tap2sna('--force {} {}'.format(tzxfile, z80file))
+        z80file = '{}/out.z80'.format(self.make_directory())
+        output, error = self.run_tap2sna(f'{tzxfile} {z80file}')
         self.assertEqual(error, '')
         snapshot = get_snapshot(z80file)
         self.assertEqual(basic_data, snapshot[23755:23755 + len(basic_data)])
         self.assertEqual(code, snapshot[code_start:code_start + len(code)])
 
     def test_empty_standard_speed_data_block_in_tzx_file_is_ignored(self):
         basic_data = [6, 7]
@@ -336,16 +494,16 @@
             create_tzx_data_block(basic_data),
             empty_block,
             create_tzx_header_block(start=code_start),
             create_tzx_data_block(code)
         ]
 
         tzxfile = self._write_tzx(blocks)
-        z80file = self.write_bin_file(suffix='.z80')
-        output, error = self.run_tap2sna('--force {} {}'.format(tzxfile, z80file))
+        z80file = '{}/out.z80'.format(self.make_directory())
+        output, error = self.run_tap2sna(f'{tzxfile} {z80file}')
         self.assertEqual(error, '')
         snapshot = get_snapshot(z80file)
         self.assertEqual(basic_data, snapshot[23755:23755 + len(basic_data)])
         self.assertEqual(code, snapshot[code_start:code_start + len(code)])
 
     def test_ram_call(self):
         ram_module = """
@@ -547,17 +705,17 @@
         self.assertEqual(error, '')
 
     def test_tap_file_in_zip_archive(self):
         data = [1]
         block = create_tap_data_block(data)
         tap_name = 'game.tap'
         zip_fname = self._write_tap([block], zip_archive=True, tap_name=tap_name)
-        z80file = self.write_bin_file(suffix='.z80')
+        z80file = '{}/out.z80'.format(self.make_directory())
         start = 16385
-        output, error = self.run_tap2sna('--force --ram load=1,{} {} {}'.format(start, zip_fname, z80file))
+        output, error = self.run_tap2sna(f'--ram load=1,{start} {zip_fname} {z80file}')
         self.assertEqual(output, 'Extracting {}\nWriting {}\n'.format(tap_name, z80file))
         self.assertEqual(error, '')
         snapshot = get_snapshot(z80file)
         self.assertEqual(data, snapshot[start:start + len(data)])
 
     def test_invalid_tzx_file(self):
         tzxfile = self.write_bin_file([1, 2, 3], suffix='.tzx')
@@ -674,21 +832,20 @@
         with self.assertRaises(SkoolKitError) as cm:
             self.run_tap2sna('{} {}/{}'.format(tzxfile, self.make_directory(), z80file))
         self.assertEqual(cm.exception.args[0], 'Error while getting snapshot {}: Unknown TZX block ID: 0x{:X}'.format(z80file, block_id))
 
     def test_default_register_values(self):
         block = create_tap_data_block([0])
         tapfile = self._write_tap([block])
-        z80file = self.write_bin_file(suffix='.z80')
+        z80file = '{}/out.z80'.format(self.make_directory())
         exp_reg_values = {
             'a': 0, 'f': 0, 'bc': 0, 'de': 0, 'hl': 0, 'i': 63, 'r': 0,
             '^bc': 0, '^de': 0, '^hl': 0, 'ix': 0, 'iy': 23610, 'sp': 0, 'pc': 0
         }
-
-        output, error = self.run_tap2sna('--force --ram load=1,16384 {} {}'.format(tapfile, z80file))
+        output, error = self.run_tap2sna('--ram load=1,16384 {} {}'.format(tapfile, z80file))
         self.assertEqual(error, '')
         with open(z80file, 'rb') as f:
             z80_header = f.read(34)
         for reg, exp_value in exp_reg_values.items():
             offset = Z80_REGISTERS[reg]
             size = len(reg) - 1 if reg.startswith('^') else len(reg)
             if size == 1:
@@ -696,24 +853,24 @@
             else:
                 value = z80_header[offset] + 256 * z80_header[offset + 1]
             self.assertEqual(value, exp_value)
 
     def test_reg(self):
         block = create_tap_data_block([1])
         tapfile = self._write_tap([block])
-        z80file = self.write_bin_file(suffix='.z80')
         reg_dicts = (
             {'^a': 1, '^b': 2, '^c': 3, '^d': 4, '^e': 5, '^f': 6, '^h': 7, '^l': 8},
             {'a': 9, 'b': 10, 'c': 11, 'd': 12, 'e': 13, 'f': 14, 'h': 15, 'l': 16, 'r': 129},
             {'^bc': 258, '^de': 515, '^hl': 65534, 'bc': 259, 'de': 516, 'hl': 65533},
             {'i': 13, 'ix': 1027, 'iy': 1284, 'pc': 1541, 'r': 23, 'sp': 32769}
         )
         for reg_dict in reg_dicts:
             reg_options = ' '.join(['--reg {}={}'.format(r, v) for r, v in reg_dict.items()])
-            output, error = self.run_tap2sna('--force --ram load=1,16384 {} {} {}'.format(reg_options, tapfile, z80file))
+            z80file = '{}/out.z80'.format(self.make_directory())
+            output, error = self.run_tap2sna(f'--ram load=1,16384 {reg_options} {tapfile} {z80file}')
             self.assertEqual(error, '')
             with open(z80file, 'rb') as f:
                 z80_header = f.read(34)
             for reg, exp_value in reg_dict.items():
                 offset = Z80_REGISTERS[reg]
                 size = len(reg) - 1 if reg.startswith('^') else len(reg)
                 if size == 1:
@@ -764,26 +921,24 @@
         tapfile, basic_data = self._write_basic_loader(code_start, code)
         z80file = '{}/out.z80'.format(self.make_directory())
         output, error = self.run_tap2sna(f'--sim-load {tapfile} {z80file}')
         out_lines = output.strip().split('\n')
         exp_out_lines = [
             'Program: simloadbas',
             'Fast loading data block: 23755,20',
-            '',
             'Bytes: simloadbyt',
             'Fast loading data block: 32768,2',
-            '',
             'Tape finished',
             'Simulation stopped (PC in RAM): PC=32768',
         ]
         self.assertEqual(exp_out_lines, out_lines)
         self.assertEqual(error, '')
         self.assertEqual(basic_data, snapshot[23755:23755 + len(basic_data)])
         self.assertEqual(code, snapshot[code_start:code_start + len(code)])
-        exp_reg = set(('SP=65344', 'IX=32770', 'IY=23610', 'PC=32768'))
+        exp_reg = set(('^F=129', 'SP=65344', 'IX=32770', 'IY=23610', 'PC=32768'))
         self.assertLessEqual(exp_reg, set(options.reg))
 
     @patch.object(tap2sna, '_write_z80', mock_write_z80)
     def test_sim_load_with_initial_code_block(self):
         code_start = 65360 # Overwrite return address on stack with...
         code = [128, 128]  # ...32896
         blocks = [
@@ -793,48 +948,45 @@
         tapfile = self._write_tap(blocks)
         z80file = '{}/out.z80'.format(self.make_directory())
         output, error = self.run_tap2sna(f'--sim-load {tapfile} {z80file}')
         out_lines = output.strip().split('\n')
         exp_out_lines = [
             'Bytes: CODE block    ',
             'Fast loading data block: 65360,2',
-            '',
             'Tape finished',
             'Simulation stopped (PC in RAM): PC=32896',
         ]
         self.assertEqual(exp_out_lines, out_lines)
         self.assertEqual(error, '')
         self.assertEqual(code, snapshot[code_start:code_start + len(code)])
-        exp_reg = set(('SP=65362', 'IX=65362', 'IY=23610', 'PC=32896'))
+        exp_reg = set(('^F=129', 'SP=65362', 'IX=65362', 'IY=23610', 'PC=32896'))
         self.assertLessEqual(exp_reg, set(options.reg))
 
     @patch.object(tap2sna, '_write_z80', mock_write_z80)
     def test_sim_load_with_given_start_address(self):
         code_start = 32768
         start = 32769
         code = [175, 201]
         tapfile, basic_data = self._write_basic_loader(code_start, code)
         z80file = '{}/out.z80'.format(self.make_directory())
         output, error = self.run_tap2sna(f'--sim-load --start {start} {tapfile} {z80file}')
         out_lines = output.strip().split('\n')
         exp_out_lines = [
             'Program: simloadbas',
             'Fast loading data block: 23755,20',
-            '',
             'Bytes: simloadbyt',
             'Fast loading data block: 32768,2',
-            '',
             'Tape finished',
             'Simulation stopped (PC at start address): PC=32769',
         ]
         self.assertEqual(exp_out_lines, out_lines)
         self.assertEqual(error, '')
         self.assertEqual(basic_data, snapshot[23755:23755 + len(basic_data)])
         self.assertEqual(code, snapshot[code_start:code_start + len(code)])
-        exp_reg = set(('SP=65344', 'IX=32770', 'IY=23610', 'PC=32769'))
+        exp_reg = set(('^F=129', 'SP=65344', 'IX=32770', 'IY=23610', 'PC=32769'))
         self.assertLessEqual(exp_reg, set(options.reg))
 
     @patch.object(tap2sna, '_write_z80', mock_write_z80)
     def test_sim_load_with_character_array(self):
         code_start = 32768
         code_start_str = [ord(c) for c in str(code_start)]
         basic_data = [
@@ -865,30 +1017,27 @@
         tapfile = self._write_tap(blocks)
         z80file = '{}/out.z80'.format(self.make_directory())
         output, error = self.run_tap2sna(f'--sim-load {tapfile} {z80file}')
         out_lines = output.strip().split('\n')
         exp_out_lines = [
             'Program: simloadbas',
             'Fast loading data block: 23755,29',
-            '',
             'Character array: characters',
             'Fast loading data block: 23787,8',
-            '',
             'Bytes: simloadbyt',
             'Fast loading data block: 32768,2',
-            '',
             'Tape finished',
             'Simulation stopped (PC in RAM): PC=32768',
         ]
         self.assertEqual(exp_out_lines, out_lines)
         self.assertEqual(error, '')
         self.assertEqual(basic_data, snapshot[23755:23755 + len(basic_data)])
         self.assertEqual(ca_data, snapshot[23787:23787 + len(ca_data)])
         self.assertEqual(code, snapshot[code_start:code_start + len(code)])
-        exp_reg = set(('SP=65344', 'IX=32770', 'IY=23610', 'PC=32768'))
+        exp_reg = set(('^F=129', 'SP=65344', 'IX=32770', 'IY=23610', 'PC=32768'))
         self.assertLessEqual(exp_reg, set(options.reg))
 
     @patch.object(tap2sna, '_write_z80', mock_write_z80)
     def test_sim_load_with_number_array(self):
         code_start = 32768
         code_start_str = [ord(c) for c in str(code_start)]
         basic_data = [
@@ -919,30 +1068,27 @@
         tapfile = self._write_tap(blocks)
         z80file = '{}/out.z80'.format(self.make_directory())
         output, error = self.run_tap2sna(f'--sim-load {tapfile} {z80file}')
         out_lines = output.strip().split('\n')
         exp_out_lines = [
             'Program: simloadbas',
             'Fast loading data block: 23755,28',
-            '',
             'Number array: numbers   ',
             'Fast loading data block: 23786,16',
-            '',
             'Bytes: simloadbyt',
             'Fast loading data block: 32768,2',
-            '',
             'Tape finished',
             'Simulation stopped (PC in RAM): PC=32768',
         ]
         self.assertEqual(exp_out_lines, out_lines)
         self.assertEqual(error, '')
         self.assertEqual(basic_data, snapshot[23755:23755 + len(basic_data)])
         self.assertEqual(na_data, snapshot[23786:23786 + len(na_data)])
         self.assertEqual(code, snapshot[code_start:code_start + len(code)])
-        exp_reg = set(('SP=65344', 'IX=32770', 'IY=23610', 'PC=32768'))
+        exp_reg = set(('^F=129', 'SP=65344', 'IX=32770', 'IY=23610', 'PC=32768'))
         self.assertLessEqual(exp_reg, set(options.reg))
 
     @patch.object(tap2sna, '_write_z80', mock_write_z80)
     def test_sim_load_with_headerless_block(self):
         code_start = 32768
         code_start_str = [ord(c) for c in str(code_start)]
         basic_data = [
@@ -975,29 +1121,26 @@
         tapfile = self._write_tap(blocks)
         z80file = '{}/out.z80'.format(self.make_directory())
         output, error = self.run_tap2sna(f'--sim-load {tapfile} {z80file}')
         out_lines = output.strip().split('\n')
         exp_out_lines = [
             'Program: simloadbas',
             'Fast loading data block: 23755,20',
-            '',
             'Bytes: simloadbyt',
             'Fast loading data block: 32768,14',
-            '',
             'Fast loading data block: 49152,2',
-            '',
             'Tape finished',
             'Simulation stopped (PC in RAM): PC=49152',
         ]
         self.assertEqual(exp_out_lines, out_lines)
         self.assertEqual(error, '')
         self.assertEqual(basic_data, snapshot[23755:23755 + len(basic_data)])
         self.assertEqual(code, snapshot[code_start:code_start + len(code)])
         self.assertEqual(code2, snapshot[49152:49152 + len(code2)])
-        exp_reg = set(('SP=65344', 'IX=49154', 'IY=23610', 'PC=49152'))
+        exp_reg = set(('^F=187', 'SP=65344', 'IX=49154', 'IY=23610', 'PC=49152'))
         self.assertLessEqual(exp_reg, set(options.reg))
 
     @patch.object(tap2sna, '_write_z80', mock_write_z80)
     def test_sim_load_with_overlong_blocks(self):
         code_start = 32768
         code_start_str = [ord(c) for c in str(code_start)]
         basic_data = [
@@ -1033,26 +1176,24 @@
         tapfile = self._write_tap(blocks)
         z80file = '{}/out.z80'.format(self.make_directory())
         output, error = self.run_tap2sna(f'--sim-load {tapfile} {z80file}')
         out_lines = output.strip().split('\n')
         exp_out_lines = [
             'Program: simloadbas',
             'Fast loading data block: 23755,20',
-            '',
             'Bytes: simloadbyt',
             'Fast loading data block: 32768,2',
-            '',
             'Tape finished',
             'Simulation stopped (PC in RAM): PC=32768',
         ]
         self.assertEqual(exp_out_lines, out_lines)
         self.assertEqual(error, '')
         self.assertEqual(basic_data + [128], snapshot[23755:23755 + len(basic_data) + 1])
         self.assertEqual(code + [0], snapshot[code_start:code_start + len(code) + 1])
-        exp_reg = set(('SP=65344', 'IX=32770', 'IY=23610', 'PC=32768'))
+        exp_reg = set(('^F=129', 'SP=65344', 'IX=32770', 'IY=23610', 'PC=32768'))
         self.assertLessEqual(exp_reg, set(options.reg))
 
     @patch.object(tap2sna, '_write_z80', mock_write_z80)
     def test_sim_load_with_undersize_block(self):
         code2 = [201]
         code2_start = 49152
         code2_end = code2_start + len(code2)
@@ -1089,27 +1230,24 @@
         z80file = '{}/out.z80'.format(self.make_directory())
         output, error = self.run_tap2sna(f'--sim-load {tapfile} {z80file}')
 
         self.assertEqual(basic_data, snapshot[23755:23755 + len(basic_data)])
         self.assertEqual(code, snapshot[code_start:code_start + len(code)])
         self.assertEqual(code2, snapshot[code2_start:code2_end])
         self.assertEqual(snapshot[code2_end], code2_data_block[-1])
-        exp_reg = set(('SP=65344', f'IX={code2_end+1}', 'E=3', 'D=0', 'IY=23610', 'PC=49152', 'F=0'))
+        exp_reg = set(('^F=187', 'SP=65344', f'IX={code2_end+1}', 'E=3', 'D=0', 'IY=23610', 'PC=49152', 'F=64'))
         self.assertLessEqual(exp_reg, set(options.reg))
 
         out_lines = output.strip().split('\n')
         exp_out_lines = [
             'Program: simloadbas',
             'Fast loading data block: 23755,20',
-            '',
             'Bytes: simloadbyt',
             'Fast loading data block: 32768,14',
-            '',
             'Fast loading data block: 49152,5',
-            '',
             'Tape finished',
             'Simulation stopped (PC in RAM): PC=49152'
         ]
         self.assertEqual(exp_out_lines, out_lines)
         self.assertEqual(error, '')
 
     @patch.object(tap2sna, '_write_z80', mock_write_z80)
@@ -1148,60 +1286,53 @@
         ]
         tapfile = self._write_tap(blocks)
         z80file = '{}/out.z80'.format(self.make_directory())
         output, error = self.run_tap2sna(f'--sim-load {tapfile} {z80file}')
         out_lines = output.strip().split('\n')
         exp_out_lines = [
             'Data block (18 bytes) [skipped]',
-            '',
             'Program: simloadbas',
             'Fast loading data block: 23755,20',
-            '',
             'Bytes: simloadbyt',
             'Fast loading data block: 32768,18',
-            '',
             'Bytes: IGNORE ME  [skipped]',
-            '',
             'Fast loading data block: 49152,2',
-            '',
             'Tape finished',
             'Simulation stopped (PC in RAM): PC=32780',
         ]
         self.assertEqual(exp_out_lines, out_lines)
         self.assertEqual(error, '')
         self.assertEqual(basic_data, snapshot[23755:23755 + len(basic_data)])
         self.assertEqual(code, snapshot[code_start:code_start + len(code)])
         self.assertEqual(code2, snapshot[49152:49152 + len(code2)])
-        exp_reg = set(('SP=65344', 'IX=49154', 'IY=23610', 'PC=32780', 'F=1'))
+        exp_reg = set(('^F=187', 'SP=65344', 'IX=49154', 'IY=23610', 'PC=32780', 'F=1'))
         self.assertLessEqual(exp_reg, set(options.reg))
 
     @patch.object(tap2sna, '_write_z80', mock_write_z80)
     def test_sim_load_ignores_extra_byte_at_end_of_tape(self):
         code_start = 32768
         code = [4, 5]
         blocks, basic_data = self._write_basic_loader(code_start, code, False)
         tapfile = self._write_tap(blocks + [[0]])
         z80file = '{}/out.z80'.format(self.make_directory())
         output, error = self.run_tap2sna(f'--sim-load {tapfile} {z80file}')
         out_lines = output.strip().split('\n')
         exp_out_lines = [
             'Program: simloadbas',
             'Fast loading data block: 23755,20',
-            '',
             'Bytes: simloadbyt',
             'Fast loading data block: 32768,2',
-            '',
             'Tape finished',
             'Simulation stopped (PC in RAM): PC=32768',
         ]
         self.assertEqual(exp_out_lines, out_lines)
         self.assertEqual(error, '')
         self.assertEqual(basic_data, snapshot[23755:23755 + len(basic_data)])
         self.assertEqual(code, snapshot[code_start:code_start + len(code)])
-        exp_reg = set(('SP=65344', 'IX=32770', 'IY=23610', 'PC=32768'))
+        exp_reg = set(('^F=129', 'SP=65344', 'IX=32770', 'IY=23610', 'PC=32768'))
         self.assertLessEqual(exp_reg, set(options.reg))
 
     @patch.object(tap2sna, '_write_z80', mock_write_z80)
     def test_sim_load_preserves_border_colour(self):
         code_start = 32768
         code_start_str = [ord(c) for c in str(code_start)]
         basic_data = [
@@ -1228,18 +1359,16 @@
         tapfile = self._write_tap(blocks)
         z80file = '{}/out.z80'.format(self.make_directory())
         output, error = self.run_tap2sna(f'--sim-load {tapfile} {z80file}')
         out_lines = output.strip().split('\n')
         exp_out_lines = [
             'Program: simloadbas',
             'Fast loading data block: 23755,26',
-            '',
             'Bytes: simloadbyt',
             'Fast loading data block: 32768,1',
-            '',
             'Tape finished',
             'Simulation stopped (PC in RAM): PC=32768',
         ]
         self.assertEqual(exp_out_lines, out_lines)
         self.assertEqual(error, '')
         self.assertIn('border=3', options.state)
 
@@ -1255,27 +1384,129 @@
         tapfile, basic_data = self._write_basic_loader(code_start, code)
         z80file = '{}/out.z80'.format(self.make_directory())
         output, error = self.run_tap2sna(f'--sim-load --start {start} {tapfile} {z80file}')
         out_lines = output.strip().split('\n')
         exp_out_lines = [
             'Program: simloadbas',
             'Fast loading data block: 23755,20',
-            '',
             'Bytes: simloadbyt',
             'Fast loading data block: 32768,4',
-            '',
             'Tape finished',
             'Simulation stopped (PC at start address): PC=32771',
         ]
         self.assertEqual(exp_out_lines, out_lines)
         self.assertEqual(error, '')
         self.assertIn('im=2', options.state)
         self.assertIn('iff=0', options.state)
 
     @patch.object(tap2sna, '_write_z80', mock_write_z80)
+    def test_sim_load_fast_load_does_not_overwrite_rom(self):
+        start_str = [ord(c) for c in "16384"]
+        basic_data = [
+            0, 10,            # Line 10
+            16, 0,            # Line length
+            239, 34, 34, 175, # LOAD ""CODE
+            58,               # :
+            249, 192, 176,    # RANDOMIZE USR VAL
+            34,               # "
+            *start_str,       # start address
+            34,               # "
+            13                # ENTER
+        ]
+        start = 16380
+        code = [
+            0x01, 0x02, 0x03, 0x04, # 16380 DEFB 1,2,3,4
+            0x21, 0xFC, 0x3F,       # 16384 LD HL,16380
+            0x11, 0x00, 0x80,       # 16387 LD DE,32768
+            0x01, 0x04, 0x00,       # 16390 LD BC,4
+            0xED, 0xB0,             # 16393 LDIR
+            0xC9,                   # 16395 RET
+        ]
+        blocks = [
+            create_tap_header_block('simloadbas', 10, len(basic_data), 0),
+            create_tap_data_block(basic_data),
+            create_tap_header_block('simloadrom', start, len(code)),
+            create_tap_data_block(code)
+        ]
+        tapfile = self._write_tap(blocks)
+        z80file = '{}/out.z80'.format(self.make_directory())
+        output, error = self.run_tap2sna(f'--sim-load --start 16395 {tapfile} {z80file}')
+        out_lines = output.strip().split('\n')
+        exp_out_lines = [
+            'Program: simloadbas',
+            'Fast loading data block: 23755,20',
+            'Bytes: simloadrom',
+            'Fast loading data block: 16380,16',
+            'Tape finished',
+            'Simulation stopped (PC at start address): PC=16395',
+        ]
+        self.assertEqual(exp_out_lines, out_lines)
+        self.assertEqual(error, '')
+        self.assertEqual([161, 153, 66, 60], snapshot[32768:32772])
+        self.assertEqual(code[4:], snapshot[start + 4:start + len(code)])
+        exp_reg = set(('^F=129', 'SP=65344', 'IX=16396', 'IY=23610', 'PC=16395'))
+        self.assertLessEqual(exp_reg, set(options.reg))
+
+    @patch.object(tap2sna, '_write_z80', mock_write_z80)
+    def test_sim_load_fast_load_checks_parity(self):
+        code_start = 32768
+        code_start_str = [ord(c) for c in str(code_start)]
+        basic_data = [
+            0, 10,            # Line 10
+            16, 0,            # Line length
+            239, 34, 34, 175, # LOAD ""CODE
+            58,               # :
+            249, 192, 176,    # RANDOMIZE USR VAL
+            34,               # "
+            *code_start_str,  # start address
+            34,               # "
+            13                # ENTER
+        ]
+        code = [
+            221, 33, 0, 192,  # 32768 LD IX,49152
+            17, 2, 0,         # 32772 LD DE,2
+            55,               # 32775 SCF
+            159,              # 32776 SBC A,A
+            205, 86, 5,       # 32777 CALL 1366
+            48, 2,            # 32780 JR NC,32787 ; Jump if load failed as expected
+            22, 128,          # 32782 LD D,128    ; Signal test failure
+            201               # 32784 RET
+        ]
+        code2 = [128, 129]
+        code2_block = create_tap_data_block(code2)
+        code2_block[-1] ^= 255 # Break parity check
+        blocks = [
+            create_tap_header_block("simloadbas", 10, len(basic_data), 0),
+            create_tap_data_block(basic_data),
+            create_tap_header_block("simloadbyt", code_start, len(code)),
+            create_tap_data_block(code),
+            code2_block
+        ]
+        tapfile = self._write_tap(blocks)
+        z80file = '{}/out.z80'.format(self.make_directory())
+        output, error = self.run_tap2sna(f'--sim-load --start 32784 {tapfile} {z80file}')
+        out_lines = output.strip().split('\n')
+        exp_out_lines = [
+            'Program: simloadbas',
+            'Fast loading data block: 23755,20',
+            'Bytes: simloadbyt',
+            'Fast loading data block: 32768,17',
+            'Fast loading data block: 49152,2',
+            'Tape finished',
+            'Simulation stopped (PC at start address): PC=32784',
+        ]
+        self.assertEqual(exp_out_lines, out_lines)
+        self.assertEqual(error, '')
+        self.assertEqual(basic_data, snapshot[23755:23755 + len(basic_data)])
+        self.assertEqual(code, snapshot[code_start:code_start + len(code)])
+        self.assertEqual(code2, snapshot[49152:49152 + len(code2)])
+        exp_reg = set(('^F=187', 'D=0', 'SP=65344', 'IX=49154', 'IY=23610', 'PC=32784'))
+        self.assertLessEqual(exp_reg, set(options.reg))
+
+    @patch.object(tap2sna, '_write_z80', mock_write_z80)
     def test_sim_load_with_ram_call(self):
         ram_module = """
             def fix(snapshot):
                 snapshot[32768:32772] = [1, 2, 3, 4]
         """
         module_dir = self.make_directory()
         module_name = 'simloadram'
@@ -1285,102 +1516,94 @@
         code = [4, 5]
         tapfile, basic_data = self._write_basic_loader(code_start, code)
         output, error = self.run_tap2sna(f'--sim-load --ram call={module_dir}:{module_name}.fix {tapfile} out.z80')
         out_lines = output.strip().split('\n')
         exp_out_lines = [
             'Program: simloadbas',
             'Fast loading data block: 23755,20',
-            '',
             'Bytes: simloadbyt',
             'Fast loading data block: 32768,2',
-            '',
             'Tape finished',
             'Simulation stopped (PC in RAM): PC=32768',
         ]
         self.assertEqual(exp_out_lines, out_lines)
         self.assertEqual(error, '')
         self.assertEqual(basic_data, snapshot[23755:23755 + len(basic_data)])
         self.assertEqual([1, 2, 3, 4], snapshot[32768:32772])
-        exp_reg = set(('SP=65344', 'IX=32770', 'IY=23610', 'PC=32768'))
+        exp_reg = set(('^F=129', 'SP=65344', 'IX=32770', 'IY=23610', 'PC=32768'))
         self.assertLessEqual(exp_reg, set(options.reg))
 
     @patch.object(tap2sna, '_write_z80', mock_write_z80)
     def test_sim_load_with_ram_move(self):
         code_start = 32768
         code = [4, 5]
         tapfile, basic_data = self._write_basic_loader(code_start, code)
         output, error = self.run_tap2sna(f'--sim-load --ram move=32768,2,32770 {tapfile} out.z80')
         out_lines = output.strip().split('\n')
         exp_out_lines = [
             'Program: simloadbas',
             'Fast loading data block: 23755,20',
-            '',
             'Bytes: simloadbyt',
             'Fast loading data block: 32768,2',
-            '',
             'Tape finished',
             'Simulation stopped (PC in RAM): PC=32768',
         ]
         self.assertEqual(exp_out_lines, out_lines)
         self.assertEqual(error, '')
         self.assertEqual(basic_data, snapshot[23755:23755 + len(basic_data)])
         self.assertEqual([4, 5, 4, 5], snapshot[32768:32772])
-        exp_reg = set(('SP=65344', 'IX=32770', 'IY=23610', 'PC=32768'))
+        exp_reg = set(('^F=129', 'SP=65344', 'IX=32770', 'IY=23610', 'PC=32768'))
         self.assertLessEqual(exp_reg, set(options.reg))
 
     @patch.object(tap2sna, '_write_z80', mock_write_z80)
     def test_sim_load_with_ram_poke(self):
         code_start = 32768
         code = [4, 5]
         tapfile, basic_data = self._write_basic_loader(code_start, code)
         output, error = self.run_tap2sna(f'--sim-load --ram poke=32768-32770-2,1 {tapfile} out.z80')
         out_lines = output.strip().split('\n')
         exp_out_lines = [
             'Program: simloadbas',
             'Fast loading data block: 23755,20',
-            '',
             'Bytes: simloadbyt',
             'Fast loading data block: 32768,2',
-            '',
             'Tape finished',
             'Simulation stopped (PC in RAM): PC=32768',
         ]
         self.assertEqual(exp_out_lines, out_lines)
         self.assertEqual(error, '')
         self.assertEqual(basic_data, snapshot[23755:23755 + len(basic_data)])
         self.assertEqual([1, 5, 1], snapshot[32768:32771])
-        exp_reg = set(('SP=65344', 'IX=32770', 'IY=23610', 'PC=32768'))
+        exp_reg = set(('^F=129', 'SP=65344', 'IX=32770', 'IY=23610', 'PC=32768'))
         self.assertLessEqual(exp_reg, set(options.reg))
 
     @patch.object(tap2sna, '_write_z80', mock_write_z80)
     def test_sim_load_with_ram_sysvars(self):
         code_start = 32768
         code = [4, 5]
         tapfile, basic_data = self._write_basic_loader(code_start, code)
         output, error = self.run_tap2sna(f'--sim-load --ram sysvars {tapfile} out.z80')
         out_lines = output.strip().split('\n')
         exp_out_lines = [
             'Program: simloadbas',
             'Fast loading data block: 23755,20',
-            '',
             'Bytes: simloadbyt',
             'Fast loading data block: 32768,2',
-            '',
             'Tape finished',
             'Simulation stopped (PC in RAM): PC=32768',
         ]
         self.assertEqual(exp_out_lines, out_lines)
         self.assertEqual(error, '')
         self.assertEqual(basic_data, snapshot[23755:23755 + len(basic_data)])
         self.assertEqual([203, 92], snapshot[23627:23629]) # VARS=23755
         self.assertEqual([204, 92], snapshot[23641:23643]) # E-LINE=23756
         self.assertEqual([206, 92], snapshot[23649:23651]) # WORKSP=23758
         self.assertEqual([206, 92], snapshot[23651:23653]) # STKBOT=23758
         self.assertEqual([206, 92], snapshot[23653:23655]) # STKEND=23758
-        exp_reg = set(('SP=65344', 'IX=32770', 'IY=23610', 'PC=32768'))
+        exp_reg = set(('^F=129', 'SP=65344', 'IX=32770', 'IY=23610', 'PC=32768'))
         self.assertLessEqual(exp_reg, set(options.reg))
 
     @patch.object(tap2sna, '_write_z80', mock_write_z80)
     def test_sim_load_with_unexpected_end_of_tape(self):
         basic_data = [
             0, 10,       # Line 10
             4, 0,        # Line length
@@ -1395,15 +1618,14 @@
         z80file = '{}/out.z80'.format(self.make_directory())
         with self.assertRaises(SkoolKitError) as cm:
             self.run_tap2sna(f'--sim-load {tapfile} {z80file}')
         out_lines = self.out.getvalue().strip().split('\n')
         exp_out_lines = [
             'Program: simloadbas',
             'Fast loading data block: 23755,8',
-            '',
             'Tape finished'
         ]
         self.assertEqual(exp_out_lines, out_lines)
         self.assertEqual(cm.exception.args[0], 'Error while getting snapshot out.z80: Failed to fast load block: unexpected end of tape')
         self.assertEqual(self.err.getvalue(), '')
 
     @patch.object(tap2sna, '_write_z80', mock_write_z80)
@@ -1460,91 +1682,177 @@
         z80file = '{}/out.z80'.format(self.make_directory())
         with self.assertRaises(SkoolKitError) as cm:
             self.run_tap2sna(f'--sim-load {tzxfile} {z80file}')
         self.assertEqual(cm.exception.args[0], 'Error while getting snapshot out.z80: TZX Generalized Data Block (0x19) not supported')
         self.assertEqual(self.out.getvalue(), '')
         self.assertEqual(self.err.getvalue(), '')
 
+    @patch.object(tap2sna, '_write_z80', mock_write_z80)
+    def test_sim_load_with_trace(self):
+        basic_data = [
+            0, 10,               # Line 10
+            14, 0,               # Line length
+            249, 192,            # RANDOMIZE USR
+            51, 50, 55, 54, 56,  # 32768 in ASCII
+            14, 0, 0, 0, 128, 0, # 32768 in floating point form
+            13                   # ENTER
+        ]
+        blocks = [
+            create_tap_header_block("simloadbas", 10, len(basic_data), 0),
+            create_tap_data_block(basic_data),
+        ]
+        tapfile = self._write_tap(blocks)
+        tracefile = '{}/sim-load.trace'.format(self.make_directory())
+        output, error = self.run_tap2sna(f'--sim-load -c trace={tracefile} {tapfile} out.z80')
+        out_lines = output.strip().split('\n')
+        exp_out_lines = [
+            'Program: simloadbas',
+            'Fast loading data block: 23755,18',
+            'Tape finished',
+            'Simulation stopped (PC in RAM): PC=32768',
+        ]
+        self.assertEqual(exp_out_lines, out_lines)
+        self.assertEqual(error, '')
+        self.assertEqual(basic_data, snapshot[23755:23755 + len(basic_data)])
+        exp_reg = set(('^F=69', 'SP=65344', 'IX=23773', 'IY=23610', 'PC=32768'))
+        self.assertLessEqual(exp_reg, set(options.reg))
+        with open(tracefile, 'r') as f:
+            trace_lines = f.read().rstrip().split('\n')
+        self.assertEqual(len(trace_lines), 8101)
+        self.assertEqual(trace_lines[0], '$0605 POP AF')
+        self.assertEqual(trace_lines[8100], '$34BB RET')
+
+    def test_sim_load_config_help(self):
+        for option in ('-c', '--sim-load-config'):
+            output, error = self.run_tap2sna(f'{option} help')
+            self.assertTrue(output.startswith('Usage: --sim-load-config accelerator=NAME\n'))
+            self.assertEqual(error, '')
+
     def test_default_state(self):
         block = create_tap_data_block([0])
         tapfile = self._write_tap([block])
-        z80file = self.write_bin_file(suffix='.z80')
-        output, error = self.run_tap2sna('--force --ram load=1,16384 {} {}'.format(tapfile, z80file))
+        z80file = '{}/out.z80'.format(self.make_directory())
+        output, error = self.run_tap2sna(f'--ram load=1,16384 {tapfile} {z80file}')
         self.assertEqual(error, '')
         with open(z80file, 'rb') as f:
             z80_header = f.read(30)
         self.assertEqual(z80_header[12] & 14, 0) # border=0
         self.assertEqual(z80_header[27], 1) # iff1=1
         self.assertEqual(z80_header[28], 1) # iff2=1
         self.assertEqual(z80_header[29] & 3, 1) # im=1
 
     def test_state_iff(self):
         block = create_tap_data_block([0])
         tapfile = self._write_tap([block])
-        z80file = self.write_bin_file(suffix='.z80')
+        z80file = '{}/out.z80'.format(self.make_directory())
         iff_value = 0
-        output, error = self.run_tap2sna('--force --ram load=1,16384 --state iff={} {} {}'.format(iff_value, tapfile, z80file))
+        output, error = self.run_tap2sna(f'--ram load=1,16384 --state iff={iff_value} {tapfile} {z80file}')
         self.assertEqual(error, '')
         with open(z80file, 'rb') as f:
             z80_header = f.read(29)
         self.assertEqual(z80_header[27], iff_value)
         self.assertEqual(z80_header[28], iff_value)
 
     def test_state_iff_bad_value(self):
         self._test_bad_spec('--state iff=fa', 'Cannot parse integer: iff=fa')
 
     def test_state_im(self):
         block = create_tap_data_block([0])
         tapfile = self._write_tap([block])
-        z80file = self.write_bin_file(suffix='.z80')
+        z80file = '{}/out.z80'.format(self.make_directory())
         im_value = 2
-        output, error = self.run_tap2sna('--force --ram load=1,16384 --state im={} {} {}'.format(im_value, tapfile, z80file))
+        output, error = self.run_tap2sna(f'--ram load=1,16384 --state im={im_value} {tapfile} {z80file}')
         self.assertEqual(error, '')
         with open(z80file, 'rb') as f:
             z80_header = f.read(30)
         self.assertEqual(z80_header[29] & 3, im_value)
 
     def test_state_im_bad_value(self):
         self._test_bad_spec('--state im=Q', 'Cannot parse integer: im=Q')
 
     def test_state_border(self):
         block = create_tap_data_block([0])
         tapfile = self._write_tap([block])
-        z80file = self.write_bin_file(suffix='.z80')
+        z80file = '{}/out.z80'.format(self.make_directory())
         border = 4
-        output, error = self.run_tap2sna('--force --ram load=1,16384 --state border={} {} {}'.format(border, tapfile, z80file))
+        output, error = self.run_tap2sna(f'--ram load=1,16384 --state border={border} {tapfile} {z80file}')
         self.assertEqual(error, '')
         with open(z80file, 'rb') as f:
             z80_header = f.read(13)
         self.assertEqual((z80_header[12] // 2) & 7, border)
 
     def test_state_border_bad_value(self):
         self._test_bad_spec('--state border=x!', 'Cannot parse integer: border=x!')
 
+    def test_state_tstates(self):
+        block = create_tap_data_block([0])
+        tapfile = self._write_tap([block])
+        z80file = os.path.join(self.make_directory(), 'out.z80')
+        tstates = 31445
+        output, error = self.run_tap2sna(f'--ram load=1,16384 --state tstates={tstates} {tapfile} {z80file}')
+        self.assertEqual(error, '')
+        with open(z80file, 'rb') as f:
+            z80_header = tuple(f.read(58))
+        t1 = (z80_header[55] + 256 * z80_header[56]) % 17472
+        t2 = (2 - z80_header[57]) % 4
+        self.assertEqual(69887 - t2 * 17472 - t1, tstates)
+
+    def test_state_tstates_bad_value(self):
+        self._test_bad_spec('--state tstates=?', 'Cannot parse integer: tstates=?')
+
     def test_state_invalid_parameter(self):
         self._test_bad_spec('--state baz=2', 'Invalid parameter: baz=2')
 
     def test_state_help(self):
         output, error = self.run_tap2sna('--state help')
-        self.assertTrue(output.startswith('Usage: --state name=value\n'))
         self.assertEqual(error, '')
+        exp_output = """
+            Usage: --state name=value
+
+            Set a hardware state attribute. Recognised names and their default values are:
+
+              border  - border colour (default=0)
+              iff     - interrupt flip-flop: 0=disabled, 1=enabled (default=1)
+              im      - interrupt mode (default=1)
+              tstates - T-states elapsed since start of frame (default=0)
+        """
+        self.assertEqual(textwrap.dedent(exp_output).lstrip(), output)
 
     def test_args_from_file(self):
         data = [1, 2, 3, 4]
         start = 49152
         args = """
             ; Comment
             # Another comment
             --force ; Overwrite
             --ram load=1,{} # Load first block
         """.format(start)
         args_file = self.write_text_file(textwrap.dedent(args).strip(), suffix='.t2s')
         snapshot = self._get_snapshot(start, data, '@{}'.format(args_file))
         self.assertEqual(data, snapshot[start:start + len(data)])
 
+    def test_quoted_args_from_file(self):
+        code = [1, 2, 3]
+        code_start = 24576
+        tap_data = create_tap_header_block(start=code_start) + create_tap_data_block(code)
+        odir = self.make_directory()
+        tapfile = self.write_bin_file(tap_data, f'{odir}/all the data.tap')
+        z80file = f'{odir}/my snapshot.z80'
+        args = f"""
+            --ram poke=32768,255
+            "{tapfile}"
+            '{z80file}'
+        """
+        args_file = self.write_text_file(textwrap.dedent(args).strip(), suffix='.t2s')
+        output, error = self.run_tap2sna(f'@{args_file}')
+        self.assertEqual(error, '')
+        snapshot = get_snapshot(z80file)
+        self.assertEqual(code, snapshot[code_start:code_start + len(code)])
+        self.assertEqual(snapshot[32768], 255)
+
     @patch.object(tap2sna, 'urlopen', Mock(return_value=BytesIO(bytearray(create_tap_data_block([2, 3])))))
     @patch.object(tap2sna, '_write_z80', mock_write_z80)
     def test_remote_download(self):
         data = [2, 3]
         start = 17000
         url = 'http://example.com/test.tap'
         output, error = self.run_tap2sna('--ram load=1,{} {} {}/test.z80'.format(start, url, self.make_directory()))
```

### Comparing `skoolkit-8.8/tests/test_tapinfo.py` & `skoolkit-8.9/tests/test_tapinfo.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,15 @@
                           create_tzx_header_block, create_tzx_data_block)
 from skoolkit import SkoolKitError, tapinfo, get_word, VERSION
 
 TZX_DATA_BLOCK = (16, 0, 0, 3, 0, 255, 0, 0)
 
 TZX_DATA_BLOCK_DESC = """
 {}: Standard speed data (0x10)
+  Pause: 0ms
   Type: Data block
   Length: 3
   Data: 255, 0, 0
 """
 
 def _get_archive_info(text_id, text):
     return [text_id, len(text)] + [ord(c) for c in text]
@@ -88,41 +89,74 @@
             4:
               Type: Data block
               Length: 5
               Data: 255, 8, 16, 32, 199
         """
         self.assertEqual(dedent(exp_output).lstrip(), output)
 
+    def test_tap_file_with_extraneous_byte(self):
+        data = [1, 2, 4]
+        tap_data = create_tap_data_block(data)
+        tap_data.append(0)
+        tapfile = self.write_bin_file(tap_data, suffix='.tap')
+        output, error = self.run_tapinfo(tapfile)
+        self.assertEqual(error, 'WARNING: Extraneous byte at end of file\n')
+        exp_output = """
+            1:
+              Type: Data block
+              Length: 5
+              Data: 255, 1, 2, 4, 248
+        """
+        self.assertEqual(dedent(exp_output).lstrip(), output)
+
+    def test_tap_file_with_missing_bytes(self):
+        data = [1, 2, 4]
+        tap_data = create_tap_data_block(data)[:-2]
+        tapfile = self.write_bin_file(tap_data, suffix='.tap')
+        output, error = self.run_tapinfo(tapfile)
+        self.assertEqual(error, 'WARNING: Missing 2 data byte(s) at end of file\n')
+        exp_output = """
+            1:
+              Type: Data block
+              Length: 3
+              Data: 255, 1, 2
+        """
+        self.assertEqual(dedent(exp_output).lstrip(), output)
+
     def test_tzx_file(self):
         blocks = []
-        blocks.append(create_tzx_header_block('<TEST_tzx>', data_type=0))
-        blocks.append(create_tzx_data_block([1, 4, 16]))
+        blocks.append(create_tzx_header_block('<TEST_tzx>', data_type=0, pause=1000))
+        blocks.append(create_tzx_data_block([1, 4, 16], pause=500))
         blocks.append(create_tzx_header_block('characters', data_type=2))
         blocks.append(create_tzx_data_block([64, 0]))
 
         tzxfile = self._write_tzx(blocks)
         output, error = self.run_tapinfo(tzxfile)
         self.assertEqual(error, '')
         exp_output = """
             Version: 1.20
             1: Standard speed data (0x10)
+              Pause: 1000ms
               Type: Header block
               Program: <TEST_tzx>
               Length: 19
               Data: 0, 0, 60, 84, 69, 83, 84 ... 0, 0, 0, 0, 0, 0, 61
             2: Standard speed data (0x10)
+              Pause: 500ms
               Type: Data block
               Length: 5
               Data: 255, 1, 4, 16, 234
             3: Standard speed data (0x10)
+              Pause: 0ms
               Type: Header block
               Character array: characters
               Length: 19
               Data: 0, 2, 99, 104, 97, 114, 97 ... 0, 0, 0, 0, 0, 0, 8
             4: Standard speed data (0x10)
+              Pause: 0ms
               Type: Data block
               Length: 4
               Data: 255, 64, 0, 191
         """
         self.assertEqual(dedent(exp_output).lstrip(), output)
 
     def test_invalid_tzx_file(self):
@@ -143,21 +177,38 @@
         tzxfile = self._write_tzx([block])
         with self.assertRaises(SkoolKitError) as cm:
             self.run_tapinfo(tzxfile)
         self.assertEqual(cm.exception.args[0], 'Unknown block ID: 0x{:02X}'.format(block_id))
 
     def test_tzx_block_0x11(self):
         data = [0, 1, 2]
-        block = [17] # Block ID
-        block.extend([0] * 15)
+        block = [
+            17,      # Block ID
+            119, 8,  # Pilot pulse length
+            154, 2,  # Sync pulse 1 length
+            224, 2,  # Sync pulse 2 length
+            170, 1,  # 0-pulse length
+            71, 3,   # 1-pulse length
+            152, 12, # Pilot tone pulses
+            5,       # Used bits in last byte
+            234, 3   # Pause
+        ]
         data_block = create_data_block(data)
         block.extend((len(data_block), 0, 0))
         block.extend(data_block)
         exp_output = """
             1: Turbo speed data (0x11)
+              Pilot pulse: 2167
+              Sync pulse 1: 666
+              Sync pulse 2: 736
+              0-pulse: 426
+              1-pulse: 839
+              Pilot length: 3224 pulses
+              Used bits in last byte: 5
+              Pause: 1002ms
               Length: 5
               Data: 255, 0, 1, 2, 252
         """
         self._test_tzx_block(block, exp_output)
 
     def test_tzx_block_0x12(self):
         block = [18] # Block ID
@@ -504,14 +555,15 @@
         block3.extend((0, 0, 0, 0))
         blocks.append(block3)
 
         tzxfile = self._write_tzx(blocks)
         exp_output = """
             Version: 1.20
             1: Standard speed data (0x10)
+              Pause: 0ms
               Type: Data block
               Length: 4
               Data: 255, 0, 1, 254
             3: Stop the tape if in 48K mode (0x2A)
         """
 
         for option in ('-b', '--tzx-blocks'):
@@ -528,14 +580,15 @@
         block2.extend((0, 0, 0, 0))
         blocks.append(block2)
 
         tzxfile = self._write_tzx(blocks)
         exp_output = """
             Version: 1.20
             1: Standard speed data (0x10)
+              Pause: 0ms
               Type: Data block
               Length: 4
               Data: 255, 0, 1, 254
         """
 
         output, error = self.run_tapinfo('-b 10,2z {}'.format(tzxfile))
         self.assertEqual(error, '')
@@ -641,15 +694,15 @@
         blocks = []
         blocks.append(create_tzx_header_block('test_tzx02', data_type=0))
         blocks.append(create_tzx_data_block([1, 4, 16]))
 
         # Turbo speed data
         data = list(range(48, 94))
         block = [0x11] # Block ID
-        block.extend([0] * 15)
+        block.extend([1] * 15)
         data_block = create_data_block(data)
         block.extend((len(data_block), 0, 0))
         block.extend(data_block)
         blocks.append(block)
 
         # Pure data
         data = [65, 66, 67, 68]
@@ -664,24 +717,34 @@
 
         tzxfile = self._write_tzx(blocks)
         output, error = self.run_tapinfo('-d {}'.format(tzxfile))
         self.assertEqual(error, '')
         exp_output = """
             Version: 1.20
             1: Standard speed data (0x10)
+              Pause: 0ms
               Type: Header block
               Program: test_tzx02
               Length: 19
               0000  00 00 74 65 73 74 5F 74 7A 78 30 32 00 00 00 00  ..test_tzx02....
               0010  00 00 3D                                         ..=
             2: Standard speed data (0x10)
+              Pause: 0ms
               Type: Data block
               Length: 5
               0000  FF 01 04 10 EA                                   .....
             3: Turbo speed data (0x11)
+              Pilot pulse: 257
+              Sync pulse 1: 257
+              Sync pulse 2: 257
+              0-pulse: 257
+              1-pulse: 257
+              Pilot length: 257 pulses
+              Used bits in last byte: 1
+              Pause: 257ms
               Length: 48
               0000  FF 30 31 32 33 34 35 36 37 38 39 3A 3B 3C 3D 3E  .0123456789:;<=>
               0010  3F 40 41 42 43 44 45 46 47 48 49 4A 4B 4C 4D 4E  ?@ABCDEFGHIJKLMN
               0020  4F 50 51 52 53 54 55 56 57 58 59 5A 5B 5C 5D FE  OPQRSTUVWXYZ[\].
             4: Pure data (0x14)
               0-pulse: 513
               1-pulse: 1027
```

### Comparing `skoolkit-8.8/tests/test_textutils.py` & `skoolkit-8.9/tests/test_textutils.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/tests/test_trace.py` & `skoolkit-8.9/tests/test_trace.py`

 * *Files 23% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         z80file, options = run_args
         self.assertEqual(z80file, 'test.z80')
         self.assertIsNone(options.start)
         self.assertIsNone(options.stop)
         self.assertFalse(options.audio)
         self.assertEqual(options.depth, 2)
         self.assertIsNone(options.dump)
+        self.assertFalse(options.interrupts)
         self.assertEqual(options.max_operations, 0)
         self.assertEqual(options.max_tstates, 0)
         self.assertIsNone(options.org)
         self.assertEqual(options.pokes, [])
         self.assertEqual(options.reg, [])
         self.assertIsNone(options.rom)
         self.assertFalse(options.stats)
@@ -77,15 +78,15 @@
         snafile = self.write_bin_file(header + ram, suffix='.sna')
         exp_output = """
             $6000 00       NOP              A=16 F=00010101 BC=0F0E DE=0D0C HL=0B0A IX=1312 IY=1110 IR=0115
                                             A'=09 F'=00001000 BC'=0706 DE'=0504 HL'=0302 SP=4002
             Stopped at $6001
         """
         self._test_trace(f'-vv -S 24577 {snafile}', exp_output)
-        self.assertEqual(simulator.iff2, 1)
+        self.assertEqual(simulator.iff, 1)
         self.assertEqual(simulator.imode, 2)
 
     @patch.object(trace, 'Simulator', TestSimulator)
     def test_z80(self):
         registers = {
             'A': 1,
             'F': 2,
@@ -109,59 +110,63 @@
             '^D': 19,
             '^E': 20,
             '^H': 21,
             '^L': 22,
             'PC': 32768,
             'iff1': 1,
             'iff2': 1,
-            'im': 2
+            'im': 2,
+            'tstates': 20000
         }
         ram = [0] * 49152
         z80file = self.write_z80_file(None, ram, registers=registers)
         exp_output = """
             $8000 00       NOP              A=01 F=00000010 BC=0304 DE=0506 HL=0708 IX=0B0C IY=090A IR=0D0F
                                             A'=0F F'=00010000 BC'=1112 DE'=1314 HL'=1516 SP=FFFF
             Stopped at $8001
         """
         self._test_trace(f'-vv -S 32769 {z80file}', exp_output)
-        self.assertEqual(simulator.iff2, 1)
+        self.assertEqual(simulator.iff, 1)
         self.assertEqual(simulator.imode, 2)
+        self.assertEqual(simulator.registers[25], 20004)
 
     @patch.object(trace, 'Simulator', TestSimulator)
     def test_szx(self):
         registers = (
-            1, 2,   # AF
-            3, 4,   # BC
-            5, 6,   # DE
-            7, 8,   # HL
-            9, 10,  # AF'
-            11, 12, # BC'
-            13, 14, # DE'
-            15, 16, # HL'
-            17, 18, # IX
-            19, 20, # IY
-            0, 128, # SP=32768
-            0, 192, # PC=49152
-            21,     # I
-            22,     # R
-            1, 1,   # iff1, iff2
-            0,      # im
+            1, 2,       # AF
+            3, 4,       # BC
+            5, 6,       # DE
+            7, 8,       # HL
+            9, 10,      # AF'
+            11, 12,     # BC'
+            13, 14,     # DE'
+            15, 16,     # HL'
+            17, 18,     # IX
+            19, 20,     # IY
+            0, 128,     # SP=32768
+            0, 192,     # PC=49152
+            21,         # I
+            22,         # R
+            1, 1,       # iff1, iff2
+            0,          # im
+            1, 1, 0, 0, # dwCyclesStart=257
         )
         ram = [0] * 49152
         szxfile = self.write_szx(ram, registers=registers)
         output, error = self.run_trace(f'-vv -S 49153 {szxfile}')
         self.assertEqual(error, '')
         exp_output = """
             $C000 00       NOP              A=02 F=00000001 BC=0403 DE=0605 HL=0807 IX=1211 IY=1413 IR=1517
                                             A'=0A F'=00001001 BC'=0C0B DE'=0E0D HL'=100F SP=8000
             Stopped at $C001
         """
         self.assertEqual(dedent(exp_output).strip(), output.rstrip())
-        self.assertEqual(simulator.iff2, 1)
+        self.assertEqual(simulator.iff, 1)
         self.assertEqual(simulator.imode, 0)
+        self.assertEqual(simulator.registers[25], 261)
 
     def test_no_snapshot(self):
         output, error = self.run_trace(f'-v -S 1 .')
         self.assertEqual(error, '')
         exp_output = """
             $0000 F3       DI
             Stopped at $0001
@@ -251,31 +256,31 @@
                                             A'=0   F'=00000000 BC'=0     DE'=0     HL'=0     SP=23552
             65508 DD216EB2 LD IX,45678      A=0   F=00000000 BC=12345 DE=23456 HL=34567 IX=45678 IY=23610 I=63  R=5  
                                             A'=0   F'=00000000 BC'=0     DE'=0     HL'=0     SP=23552
             65512 FD21D5DD LD IY,56789      A=0   F=00000000 BC=12345 DE=23456 HL=34567 IX=45678 IY=56789 I=63  R=7  
                                             A'=0   F'=00000000 BC'=0     DE'=0     HL'=0     SP=23552
             65516 90       SUB B            A=208 F=10000011 BC=12345 DE=23456 HL=34567 IX=45678 IY=56789 I=63  R=8  
                                             A'=0   F'=00000000 BC'=0     DE'=0     HL'=0     SP=23552
-            65517 ED4F     LD R,A           A=208 F=10000011 BC=12345 DE=23456 HL=34567 IX=45678 IY=56789 I=63  R=210
+            65517 ED4F     LD R,A           A=208 F=10000011 BC=12345 DE=23456 HL=34567 IX=45678 IY=56789 I=63  R=208
                                             A'=0   F'=00000000 BC'=0     DE'=0     HL'=0     SP=23552
-            65519 ED47     LD I,A           A=208 F=10000011 BC=12345 DE=23456 HL=34567 IX=45678 IY=56789 I=208 R=212
+            65519 ED47     LD I,A           A=208 F=10000011 BC=12345 DE=23456 HL=34567 IX=45678 IY=56789 I=208 R=210
                                             A'=0   F'=00000000 BC'=0     DE'=0     HL'=0     SP=23552
-            65521 D9       EXX              A=208 F=10000011 BC=0     DE=0     HL=0     IX=45678 IY=56789 I=208 R=213
+            65521 D9       EXX              A=208 F=10000011 BC=0     DE=0     HL=0     IX=45678 IY=56789 I=208 R=211
                                             A'=0   F'=00000000 BC'=12345 DE'=23456 HL'=34567 SP=23552
-            65522 0198FF   LD BC,65432      A=208 F=10000011 BC=65432 DE=0     HL=0     IX=45678 IY=56789 I=208 R=214
+            65522 0198FF   LD BC,65432      A=208 F=10000011 BC=65432 DE=0     HL=0     IX=45678 IY=56789 I=208 R=212
                                             A'=0   F'=00000000 BC'=12345 DE'=23456 HL'=34567 SP=23552
-            65525 1131D4   LD DE,54321      A=208 F=10000011 BC=65432 DE=54321 HL=0     IX=45678 IY=56789 I=208 R=215
+            65525 1131D4   LD DE,54321      A=208 F=10000011 BC=65432 DE=54321 HL=0     IX=45678 IY=56789 I=208 R=213
                                             A'=0   F'=00000000 BC'=12345 DE'=23456 HL'=34567 SP=23552
-            65528 21CAA8   LD HL,43210      A=208 F=10000011 BC=65432 DE=54321 HL=43210 IX=45678 IY=56789 I=208 R=216
+            65528 21CAA8   LD HL,43210      A=208 F=10000011 BC=65432 DE=54321 HL=43210 IX=45678 IY=56789 I=208 R=214
                                             A'=0   F'=00000000 BC'=12345 DE'=23456 HL'=34567 SP=23552
-            65531 08       EX AF,AF'        A=0   F=00000000 BC=65432 DE=54321 HL=43210 IX=45678 IY=56789 I=208 R=217
+            65531 08       EX AF,AF'        A=0   F=00000000 BC=65432 DE=54321 HL=43210 IX=45678 IY=56789 I=208 R=215
                                             A'=208 F'=10000011 BC'=12345 DE'=23456 HL'=34567 SP=23552
-            65532 90       SUB B            A=1   F=00010011 BC=65432 DE=54321 HL=43210 IX=45678 IY=56789 I=208 R=218
+            65532 90       SUB B            A=1   F=00010011 BC=65432 DE=54321 HL=43210 IX=45678 IY=56789 I=208 R=216
                                             A'=208 F'=10000011 BC'=12345 DE'=23456 HL'=34567 SP=23552
-            65533 316D7D   LD SP,32109      A=1   F=00010011 BC=65432 DE=54321 HL=43210 IX=45678 IY=56789 I=208 R=219
+            65533 316D7D   LD SP,32109      A=1   F=00010011 BC=65432 DE=54321 HL=43210 IX=45678 IY=56789 I=208 R=217
                                             A'=208 F'=10000011 BC'=12345 DE'=23456 HL'=34567 SP=32109
             Stopped at 0
         """
         for option in ('-D', '--decimal'):
             output, error = self.run_trace(f'-vv -S 0 {option} {binfile}')
             self.assertEqual(error, '')
             self.assertEqual(dedent(exp_output).strip(), output.rstrip())
@@ -397,29 +402,329 @@
             'bc=32119',
             'de=5112',
             'hl=0',
             'ix=3442',
             'iy=10030',
             'sp=48873',
             'i=255',
-            'r=145',
+            'r=143',
             '^a=255',
             '^f=187',
             '^bc=4232',
             '^de=21432',
             '^hl=25431',
             f'pc={stop}'
         )
-        exp_state = ('border=1', 'iff=0', 'im=2')
+        exp_state = ('border=1', 'iff=0', 'im=2', 'tstates=166')
         self.assertEqual(dedent(exp_output).strip(), output.rstrip())
         self.assertEqual(z80fname, outfile)
         self.assertEqual(data, snapshot[start:stop])
         self.assertEqual(exp_reg, z80reg)
         self.assertEqual(exp_state, z80state)
 
+    def test_option_interrupts_mode_0(self):
+        data = [
+            0xED, 0x46, # $8000 IM 0
+            0x76,       # $8002 HALT
+            0xAF,       # $8003 XOR A
+        ]
+        binfile = self.write_bin_file(data, suffix='.bin')
+        start = 0x8000
+        stop = 0x8004
+        output, error = self.run_trace(f'--interrupts -o {start} -S {stop} -v {binfile}')
+        self.assertEqual(error, '')
+        output_lines = output.split('\n')
+        self.assertEqual(output_lines[0], '$8000 ED46     IM 0')
+        self.assertEqual(output_lines[1:17471], ['$8002 76       HALT'] * 17470)
+        self.assertEqual(output_lines[17471], '$0038 F5       PUSH AF')
+        self.assertEqual(output_lines[17579], '$0052 C9       RET')
+        self.assertEqual(output_lines[17580], '$8003 AF       XOR A')
+        self.assertEqual(output_lines[17581], 'Stopped at $8004')
+
+    def test_option_interrupts_mode_1(self):
+        data = [
+            0xED, 0x56, # $8000 IM 1
+            0x76,       # $8002 HALT
+            0xAF,       # $8003 XOR A
+        ]
+        binfile = self.write_bin_file(data, suffix='.bin')
+        start = 0x8000
+        stop = 0x8004
+        output, error = self.run_trace(f'-i -o {start} -S {stop} -v {binfile}')
+        self.assertEqual(error, '')
+        output_lines = output.split('\n')
+        self.assertEqual(output_lines[0], '$8000 ED56     IM 1')
+        self.assertEqual(output_lines[1:17471], ['$8002 76       HALT'] * 17470)
+        self.assertEqual(output_lines[17471], '$0038 F5       PUSH AF')
+        self.assertEqual(output_lines[17579], '$0052 C9       RET')
+        self.assertEqual(output_lines[17580], '$8003 AF       XOR A')
+        self.assertEqual(output_lines[17581], 'Stopped at $8004')
+
+    def test_option_interrupts_mode_2(self):
+        data = [
+            0x76,       # $7FFB HALT
+            0xAF,       # $7FFC XOR A
+            0x00,       # $7FFD NOP
+            0xC9,       # $7FFE RET
+            0xFE, 0x7F, # $7FFF DEFW $7FFE
+        ]
+        binfile = self.write_bin_file(data, suffix='.bin')
+        start = 0x7ffb
+        stop = 0x7ffd
+        ram = [0] * 49152
+        ram[start - 0x4000:start - 0x4000 + len(data)] = data
+        registers = {'PC': start, 'I': 127, 'iff2': 1, 'im': 2, 'tstates': 69882}
+        z80file = self.write_z80_file(None, ram, registers=registers)
+        output, error = self.run_trace(f'--interrupts -S {stop} -v {z80file}')
+        self.assertEqual(error, '')
+        output_lines = output.split('\n')
+        self.assertEqual(output_lines[0], '$7FFB 76       HALT')
+        self.assertEqual(output_lines[1], '$7FFB 76       HALT')
+        self.assertEqual(output_lines[2], '$7FFE C9       RET')
+        self.assertEqual(output_lines[3], '$7FFC AF       XOR A')
+        self.assertEqual(output_lines[4], 'Stopped at $7FFD')
+
+    def test_option_interrupts_without_halt(self):
+        data = [
+            0x00, # $8000 NOP ; t=69882
+            0x00, # $8001 NOP ; t=69886 (interrupt follows)
+            0x00, # $8002 NOP
+        ]
+        start = 0x8000
+        stop = 0x8003
+        ram = [0] * 49152
+        ram[start - 0x4000:start - 0x4000 + len(data)] = data
+        registers = {'PC': start, 'iff2': 1, 'im': 1, 'tstates': 69882}
+        z80file = self.write_z80_file(None, ram, registers=registers)
+        output, error = self.run_trace(f'-i -S {stop} -v {z80file}')
+        self.assertEqual(error, '')
+        output_lines = output.split('\n')
+        self.assertEqual(output_lines[0], '$8000 00       NOP')
+        self.assertEqual(output_lines[1], '$8001 00       NOP')
+        self.assertEqual(output_lines[2], '$0038 F5       PUSH AF')
+        self.assertEqual(output_lines[110], '$0052 C9       RET')
+        self.assertEqual(output_lines[111], '$8002 00       NOP')
+        self.assertEqual(output_lines[112], 'Stopped at $8003')
+
+    def test_option_interrupts_with_ei(self):
+        data = [
+            0x00, # $8000 NOP ; t=69882
+            0xFB, # $8001 EI  ; t=69886 (no interrupt accepted after EI)
+            0x00, # $8002 NOP ; t=69890 (interrupt follows)
+            0x00, # $8003 NOP
+        ]
+        start = 0x8000
+        stop = 0x8004
+        ram = [0] * 49152
+        ram[start - 0x4000:start - 0x4000 + len(data)] = data
+        registers = {'PC': start, 'iff2': 1, 'im': 1, 'tstates': 69882}
+        z80file = self.write_z80_file(None, ram, registers=registers)
+        output, error = self.run_trace(f'--interrupts -S {stop} -v {z80file}')
+        self.assertEqual(error, '')
+        output_lines = output.split('\n')
+        self.assertEqual(output_lines[0], '$8000 00       NOP')
+        self.assertEqual(output_lines[1], '$8001 FB       EI')
+        self.assertEqual(output_lines[2], '$8002 00       NOP')
+        self.assertEqual(output_lines[3], '$0038 F5       PUSH AF')
+        self.assertEqual(output_lines[111], '$0052 C9       RET')
+        self.assertEqual(output_lines[112], '$8003 00       NOP')
+        self.assertEqual(output_lines[113], 'Stopped at $8004')
+
+    def test_option_interrupts_with_di(self):
+        data = [
+            0x00, # $8000 NOP ; t=69882
+            0xF3, # $8001 DI  ; t=69886 (no interrupt accepted after DI)
+            0x00, # $8002 NOP ; t=69890
+            0x00, # $8003 NOP ; t=69894
+        ]
+        start = 0x8000
+        stop = 0x8004
+        ram = [0] * 49152
+        ram[start - 0x4000:start - 0x4000 + len(data)] = data
+        registers = {'PC': start, 'iff2': 1, 'im': 1, 'tstates': 69882}
+        z80file = self.write_z80_file(None, ram, registers=registers)
+        output, error = self.run_trace(f'--interrupts -S {stop} -v {z80file}')
+        self.assertEqual(error, '')
+        output_lines = output.split('\n')
+        self.assertEqual(output_lines[0], '$8000 00       NOP')
+        self.assertEqual(output_lines[1], '$8001 F3       DI')
+        self.assertEqual(output_lines[2], '$8002 00       NOP')
+        self.assertEqual(output_lines[3], '$8003 00       NOP')
+        self.assertEqual(output_lines[4], 'Stopped at $8004')
+
+    def test_option_interrupts_with_dd_prefix(self):
+        data = [
+            0xDD, # $8000 DEFB $DD ; t=69886 (no interrupt accepted after DD)
+            0x00, # $8001 NOP      ; t=69890 (interrupt follows)
+            0x00, # $8002 NOP
+        ]
+        start = 0x8000
+        stop = 0x8003
+        ram = [0] * 49152
+        ram[0x1C00] = ram[0x1C04] = 0xFF # KSTATE0/4
+        ram[start - 0x4000:start - 0x4000 + len(data)] = data
+        registers = {'PC': start, 'iff2': 1, 'im': 1, 'tstates': 69886}
+        z80file = self.write_z80_file(None, ram, registers=registers)
+        output, error = self.run_trace(f'--interrupts -S {stop} -v {z80file}')
+        self.assertEqual(error, '')
+        output_lines = output.split('\n')
+        self.assertEqual(output_lines[0], '$8000 DD       DEFB $DD')
+        self.assertEqual(output_lines[1], '$8001 00       NOP')
+        self.assertEqual(output_lines[2], '$0038 F5       PUSH AF')
+        self.assertEqual(output_lines[102], '$0052 C9       RET')
+        self.assertEqual(output_lines[103], '$8002 00       NOP')
+        self.assertEqual(output_lines[104], 'Stopped at $8003')
+
+    def test_option_interrupts_with_fd_prefix(self):
+        data = [
+            0xFD, # $8000 DEFB $FD ; t=69886 (no interrupt accepted after FD)
+            0x00, # $8001 NOP      ; t=69890 (interrupt follows)
+            0x00, # $8002 NOP
+        ]
+        start = 0x8000
+        stop = 0x8003
+        ram = [0] * 49152
+        ram[0x1C00] = ram[0x1C04] = 0xFF # KSTATE0/4
+        ram[start - 0x4000:start - 0x4000 + len(data)] = data
+        registers = {'PC': start, 'iff2': 1, 'im': 1, 'tstates': 69886}
+        z80file = self.write_z80_file(None, ram, registers=registers)
+        output, error = self.run_trace(f'--interrupts -S {stop} -v {z80file}')
+        self.assertEqual(error, '')
+        output_lines = output.split('\n')
+        self.assertEqual(output_lines[0], '$8000 FD       DEFB $FD')
+        self.assertEqual(output_lines[1], '$8001 00       NOP')
+        self.assertEqual(output_lines[2], '$0038 F5       PUSH AF')
+        self.assertEqual(output_lines[102], '$0052 C9       RET')
+        self.assertEqual(output_lines[103], '$8002 00       NOP')
+        self.assertEqual(output_lines[104], 'Stopped at $8003')
+
+    def test_option_interrupts_with_ddfd_chain(self):
+        data = [
+            0xDD, # $8000 DEFB $DD ; t=69886 (no interrupt accepted after DD)
+            0xFD, # $8001 DEFB $FD ; t=69890 (no interrupt accepted after FD)
+            0xDD, # $8002 DEFB $DD ; t=69894 (no interrupt accepted after DD)
+            0xFD, # $8003 DEFB $FD ; t=69898 (no interrupt accepted after FD)
+            0x00, # $8004 NOP      ; t=69902 (interrupt follows)
+            0x00, # $8005 NOP
+        ]
+        start = 0x8000
+        stop = 0x8006
+        ram = [0] * 49152
+        ram[0x1C00] = ram[0x1C04] = 0xFF # KSTATE0/4
+        ram[start - 0x4000:start - 0x4000 + len(data)] = data
+        registers = {'PC': start, 'iff2': 1, 'im': 1, 'tstates': 69886}
+        z80file = self.write_z80_file(None, ram, registers=registers)
+        output, error = self.run_trace(f'--interrupts -S {stop} -v {z80file}')
+        self.assertEqual(error, '')
+        output_lines = output.split('\n')
+        self.assertEqual(output_lines[0], '$8000 DD       DEFB $DD')
+        self.assertEqual(output_lines[1], '$8001 FD       DEFB $FD')
+        self.assertEqual(output_lines[2], '$8002 DD       DEFB $DD')
+        self.assertEqual(output_lines[3], '$8003 FD       DEFB $FD')
+        self.assertEqual(output_lines[4], '$8004 00       NOP')
+        self.assertEqual(output_lines[5], '$0038 F5       PUSH AF')
+        self.assertEqual(output_lines[105], '$0052 C9       RET')
+        self.assertEqual(output_lines[106], '$8005 00       NOP')
+        self.assertEqual(output_lines[107], 'Stopped at $8006')
+
+    def test_option_interrupts_at_exact_frame_boundary(self):
+        data = [
+            0x78, # $8000 LD A,B ; t=69884 (+4=69888: frame boundary)
+            0x78, # $8001 LD A,B
+        ]
+        start = 0x8000
+        stop = 0x8002
+        ram = [0] * 49152
+        ram[start - 0x4000:start - 0x4000 + len(data)] = data
+        registers = {'PC': start, 'iff2': 1, 'im': 1, 'tstates': 69884}
+        z80file = self.write_z80_file(None, ram, registers=registers)
+        output, error = self.run_trace(f'--interrupts -S {stop} -v {z80file}')
+        self.assertEqual(error, '')
+        output_lines = output.split('\n')
+        self.assertEqual(output_lines[0], '$8000 78       LD A,B')
+        self.assertEqual(output_lines[1], '$0038 F5       PUSH AF')
+        self.assertEqual(output_lines[109], '$0052 C9       RET')
+        self.assertEqual(output_lines[110], '$8001 78       LD A,B')
+        self.assertEqual(output_lines[111], 'Stopped at $8002')
+
+    @patch.object(trace, 'write_z80v3', mock_write_z80v3)
+    def test_option_interrupts_with_djnz(self):
+        data = [
+            0x21, 0x00, 0x80,       # $7FEF LD HL,$8000   ; t=69805 T-states
+            0x22, 0xFF, 0xFE,       # $7FF2 LD ($FEFF),HL ; t=69815
+            0x3E, 0xFE,             # $7FF5 LD A,$FE      ; t=69831
+            0xED, 0x47,             # $7FF7 LD I,A        ; t=69838
+            0xED, 0x5E,             # $7FF9 IM 2          ; t=69847
+            0x06, 0x04,             # $7FFB LD B,$04      ; t=69855
+            0x10, 0xFE,             # $7FFD DJNZ $7FFD    ; t=69862/69875/interrupted
+            0x00,                   # $7FFF NOP
+            0xED, 0x43, 0x00, 0xC0, # $8000 LD ($C000),BC
+            0xC9,                   # $8004 RET
+        ]
+        outfile = os.path.join(self.make_directory(), 'dump.z80')
+        start = 0x7fef
+        stop = 0x7fff
+        ram = [0] * 49152
+        ram[start - 0x4000:start - 0x4000 + len(data)] = data
+        registers = {'PC': start, 'iff2': 1, 'im': 1, 'tstates': 69805}
+        z80file = self.write_z80_file(None, ram, registers=registers)
+        output, error = self.run_trace(f'--interrupts -S {stop} --dump {outfile} -v {z80file}')
+        self.assertEqual(error, '')
+        self.assertEqual(snapshot[0xc001], 2) # DJNZ interrupted when B=2
+
+    @patch.object(trace, 'write_z80v3', mock_write_z80v3)
+    def test_option_interrupts_with_ldir(self):
+        data = [
+            0x21, 0x00, 0x80,       # $7FEE LD HL,$8000   ; t=69805 T-states
+            0x22, 0xFF, 0xFE,       # $7FF1 LD ($FEFF),HL ; t=69815
+            0x3E, 0xFE,             # $7FF4 LD A,$FE      ; t=69831
+            0xED, 0x47,             # $7FF6 LD I,A        ; t=69838
+            0xED, 0x5E,             # $7FF8 IM 2          ; t=69847
+            0x01, 0x04, 0x00,       # $7FFA LD BC,$0004   ; t=69855
+            0xED, 0xB0,             # $7FFD LDIR          ; t=69865/69886/interrupted
+            0x00,                   # $7FFF NOP
+            0xED, 0x43, 0x00, 0xC0, # $8000 LD ($C000),BC
+            0xC9,                   # $8004 RET
+        ]
+        outfile = os.path.join(self.make_directory(), 'dump.z80')
+        start = 0x7fee
+        stop = 0x7fff
+        ram = [0] * 49152
+        ram[start - 0x4000:start - 0x4000 + len(data)] = data
+        registers = {'PC': start, 'iff2': 1, 'im': 1, 'tstates': 69805}
+        z80file = self.write_z80_file(None, ram, registers=registers)
+        output, error = self.run_trace(f'--interrupts -S {stop} --dump {outfile} -v {z80file}')
+        self.assertEqual(error, '')
+        self.assertEqual(snapshot[0xc000], 2) # LDIR interrupted when BC=2
+
+    @patch.object(trace, 'write_z80v3', mock_write_z80v3)
+    def test_option_interrupts_with_lddr(self):
+        data = [
+            0x21, 0x00, 0x80,       # $7FEE LD HL,$8000   ; t=69805 T-states
+            0x22, 0xFF, 0xFE,       # $7FF1 LD ($FEFF),HL ; t=69815
+            0x3E, 0xFE,             # $7FF4 LD A,$FE      ; t=69831
+            0xED, 0x47,             # $7FF6 LD I,A        ; t=69838
+            0xED, 0x5E,             # $7FF8 IM 2          ; t=69847
+            0x01, 0x04, 0x00,       # $7FFA LD BC,$0004   ; t=69855
+            0xED, 0xB8,             # $7FFD LDDR          ; t=69865/69886/interrupted
+            0x00,                   # $7FFF NOP
+            0xED, 0x43, 0x00, 0xC0, # $8000 LD ($C000),BC
+            0xC9,                   # $8004 RET
+        ]
+        outfile = os.path.join(self.make_directory(), 'dump.z80')
+        start = 0x7fee
+        stop = 0x7fff
+        ram = [0] * 49152
+        ram[start - 0x4000:start - 0x4000 + len(data)] = data
+        registers = {'PC': start, 'iff2': 1, 'im': 1, 'tstates': 69805}
+        z80file = self.write_z80_file(None, ram, registers=registers)
+        output, error = self.run_trace(f'--interrupts -S {stop} --dump {outfile} -v {z80file}')
+        self.assertEqual(error, '')
+        self.assertEqual(snapshot[0xc000], 2) # LDDR interrupted when BC=2
+
     def test_option_max_operations(self):
         data = [
             0xAF, # XOR A
             0x3C, # INC A
         ]
         binfile = self.write_bin_file(data, suffix='.bin')
         start = 32768
@@ -540,14 +845,32 @@
         self.assertEqual(error, '')
         o_lines = output.split('\n')
         self.assertEqual(o_lines[0], 'Stopped at $8002')
         self.assertEqual(o_lines[1], 'Z80 execution time: 8 T-states (0.000s)')
         self.assertEqual(o_lines[2], 'Instructions executed: 2')
         self.assertEqual(o_lines[3][:17], 'Simulation time: ')
 
+    def test_option_stats_with_non_zero_start_time(self):
+        data = [
+            175, # XOR A
+            60,  # INC A
+        ]
+        start, stop = 32768, 32770
+        ram = [0] * 49152
+        ram[start - 0x4000:start - 0x4000 + len(data)] = data
+        registers = {'PC': start, 'tstates': 10000}
+        z80file = self.write_z80_file(None, ram, registers=registers)
+        output, error = self.run_trace(f'-S {stop} --stats {z80file}')
+        self.assertEqual(error, '')
+        o_lines = output.split('\n')
+        self.assertEqual(o_lines[0], 'Stopped at $8002')
+        self.assertEqual(o_lines[1], 'Z80 execution time: 8 T-states (0.000s)')
+        self.assertEqual(o_lines[2], 'Instructions executed: 2')
+        self.assertEqual(o_lines[3][:17], 'Simulation time: ')
+
     def test_option_stop(self):
         for option in ('-S 57', '--stop 0x0039'):
             output, error = self.run_trace(f'-v -s 56 {option} .')
             self.assertEqual(error, '')
             exp_output = """
                 $0038 F5       PUSH AF
                 Stopped at $0039
```

### Comparing `skoolkit-8.8/tests/test_traceutils.py` & `skoolkit-8.9/tests/test_traceutils.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/tests/test_z80.py` & `skoolkit-8.9/tests/test_z80.py`

 * *Files identical despite different names*

### Comparing `skoolkit-8.8/trace.py` & `skoolkit-8.9/trace.py`

 * *Files identical despite different names*

