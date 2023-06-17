# Comparing `tmp/accelerator-toolbox-0.3.0.tar.gz` & `tmp/accelerator_toolbox-0.4.0-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelerator-toolbox-0.3.0.tar", last modified: Sat Sep 24 14:00:41 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

