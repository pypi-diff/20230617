# Comparing `tmp/udl_vis-0.3.1.tar.gz` & `tmp/udl_vis-0.3.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\udl_vis-0.3.1.tar", last modified: Fri Jun  9 18:39:18 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

