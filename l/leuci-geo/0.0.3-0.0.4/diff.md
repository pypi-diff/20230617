# Comparing `tmp/leuci-geo-0.0.3.tar.gz` & `tmp/leuci_geo-0.0.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leuci-geo-0.0.3.tar", last modified: Sun Jun  4 18:18:02 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

