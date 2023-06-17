# Comparing `tmp/jx-python-4.35.21121.tar.gz` & `tmp/jx_python-4.420.23168-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\jx-python-4.35.21121.tar", last modified: Sat May  1 15:34:10 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

