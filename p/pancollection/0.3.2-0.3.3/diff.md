# Comparing `tmp/pancollection-0.3.2.tar.gz` & `tmp/pancollection-0.3.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pancollection-0.3.2.tar", last modified: Fri Jun  9 18:37:07 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

