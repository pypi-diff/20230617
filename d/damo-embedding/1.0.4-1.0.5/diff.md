# Comparing `tmp/damo-embedding-1.0.4.tar.gz` & `tmp/damo_embedding-1.0.5-cp310-cp310-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "damo-embedding-1.0.4.tar", last modified: Sat Jun  3 15:20:41 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

