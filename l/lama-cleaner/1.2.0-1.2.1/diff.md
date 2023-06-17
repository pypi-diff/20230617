# Comparing `tmp/lama-cleaner-1.2.0.tar.gz` & `tmp/lama-cleaner-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lama-cleaner-1.2.0.tar", last modified: Tue Jun  6 13:50:21 2023, max compression
+gzip compressed data, was "lama-cleaner-1.2.1.tar", last modified: Sat Jun 17 14:06:15 2023, max compression
```

## Comparing `lama-cleaner-1.2.0.tar` & `lama-cleaner-1.2.1.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-06-06 13:50:21.468504 lama-cleaner-1.2.0/
--rw-r--r--   0 cwq        (501) staff       (20)    11357 2023-02-05 13:09:10.000000 lama-cleaner-1.2.0/LICENSE
--rw-r--r--   0 cwq        (501) staff       (20)     4918 2023-06-06 13:50:21.468293 lama-cleaner-1.2.0/PKG-INFO
--rw-r--r--   0 cwq        (501) staff       (20)     3459 2023-05-19 13:47:09.000000 lama-cleaner-1.2.0/README.md
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-06-06 13:50:21.428929 lama-cleaner-1.2.0/lama_cleaner/
--rw-r--r--   0 cwq        (501) staff       (20)      488 2023-04-02 07:46:39.000000 lama-cleaner-1.2.0/lama_cleaner/__init__.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-06-06 13:50:21.425191 lama-cleaner-1.2.0/lama_cleaner/app/
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-06-06 13:50:21.430992 lama-cleaner-1.2.0/lama_cleaner/app/build/
--rw-r--r--   0 cwq        (501) staff       (20)     6148 2023-05-19 13:47:41.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/.DS_Store
--rw-r--r--   0 cwq        (501) staff       (20)     4559 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/asset-manifest.json
--rw-r--r--   0 cwq        (501) staff       (20)    67646 2023-05-19 13:47:41.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/favicon.ico
--rw-r--r--   0 cwq        (501) staff       (20)      719 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/index.html
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-06-06 13:50:21.425421 lama-cleaner-1.2.0/lama_cleaner/app/build/static/
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-06-06 13:50:21.431209 lama-cleaner-1.2.0/lama_cleaner/app/build/static/css/
--rw-r--r--   0 cwq        (501) staff       (20)    39068 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/css/main.ce986cc8.css
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-06-06 13:50:21.433524 lama-cleaner-1.2.0/lama_cleaner/app/build/static/js/
--rw-r--r--   0 cwq        (501) staff       (20)   831766 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/js/main.1fda6320.js
--rw-r--r--   0 cwq        (501) staff       (20)     1971 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/js/main.1fda6320.js.LICENSE.txt
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-06-06 13:50:21.455982 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/
--rw-r--r--   0 cwq        (501) staff       (20)   102868 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-Black.15ca31c0a2a68f76d2d1.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   138764 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-Black.c6938660eec019fefd68.woff
--rw-r--r--   0 cwq        (501) staff       (20)   146824 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-BlackItalic.ca1e738e4f349f27514d.woff
--rw-r--r--   0 cwq        (501) staff       (20)   108752 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-BlackItalic.cb2a7335650c690077fe.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   143208 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-Bold.93c1301bd9f486c573b3.woff
--rw-r--r--   0 cwq        (501) staff       (20)   106140 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-Bold.ec64ea577b0349e055ad.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   111808 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-BoldItalic.2d26c56a606662486796.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   151052 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-BoldItalic.b376885042f6c961a541.woff
--rw-r--r--   0 cwq        (501) staff       (20)   106108 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-ExtraBold.cbe0ae49c52c920fd563.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   142920 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-ExtraBold.d0fa3bb2b7c9063dc594.woff
--rw-r--r--   0 cwq        (501) staff       (20)   111708 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-ExtraBoldItalic.535a6cf662596b3bd6a6.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   150628 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-ExtraBoldItalic.6ab17abedc4d3f140953.woff
--rw-r--r--   0 cwq        (501) staff       (20)   104232 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-ExtraLight.72505e6a122c6acd5471.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   140724 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-ExtraLight.c4248615291a9e8f1fb7.woff
--rw-r--r--   0 cwq        (501) staff       (20)   149996 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-ExtraLightItalic.170dddfca278d3c2ad4a.woff
--rw-r--r--   0 cwq        (501) staff       (20)   111392 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-ExtraLightItalic.5c7d7d6deb1d2ec8d48c.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   144372 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-Italic.890025e726861dba417f.woff
--rw-r--r--   0 cwq        (501) staff       (20)   106876 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-Italic.cb10ffd7684cd9836a05.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   104332 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-Light.2d5198822ab091ce4305.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   140632 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-Light.994e34451cc19ede31d3.woff
--rw-r--r--   0 cwq        (501) staff       (20)   150092 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-LightItalic.ef9f65d91d2b0ba9b2e4.woff
--rw-r--r--   0 cwq        (501) staff       (20)   111332 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-LightItalic.f86952265d7b0f02c921.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   105924 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-Medium.293fd13dbca5a3e450ef.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   142552 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-Medium.9053572c46aeb4b16caa.woff
--rw-r--r--   0 cwq        (501) staff       (20)   112184 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-MediumItalic.085cb93e613ba3d40d2b.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   150988 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-MediumItalic.3d0107dd43d0101274d3.woff
--rw-r--r--   0 cwq        (501) staff       (20)   133844 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-Regular.8c206db99195777c6769.woff
--rw-r--r--   0 cwq        (501) staff       (20)    98868 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-Regular.c8ba52b05a9ef10f4758.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   105804 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-SemiBold.b5f0f109bc88052d4000.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   142932 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-SemiBold.cca62d21c8c555c392e5.woff
--rw-r--r--   0 cwq        (501) staff       (20)   151180 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-SemiBoldItalic.463bdbfb28abad0fa6df.woff
--rw-r--r--   0 cwq        (501) staff       (20)   112048 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-SemiBoldItalic.d9467ee321a8f38aefff.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   135920 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-Thin.29b9c616a95a912abf73.woff
--rw-r--r--   0 cwq        (501) staff       (20)    99632 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-Thin.fff2a096db014f6239d4.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   145480 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-ThinItalic.bae95eb2f889c797e435.woff
--rw-r--r--   0 cwq        (501) staff       (20)   106496 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-ThinItalic.bf213704dce6b437ede4.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   245036 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-italic.var.30807be7abc48ba8c73c.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   227180 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-roman.var.ba4caefcdf5b36b438db.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   324864 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter.var.c2fe3cb2b7c746f7966a.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   431724 2023-05-19 13:47:58.000000 lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/coffee-machine-lineal.ee32631219cc3986f861.gif
--rw-r--r--   0 cwq        (501) staff       (20)     3244 2023-02-05 13:09:10.000000 lama-cleaner-1.2.0/lama_cleaner/benchmark.py
--rw-r--r--   0 cwq        (501) staff       (20)     5145 2023-05-19 13:47:19.000000 lama-cleaner-1.2.0/lama_cleaner/const.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-06-06 13:50:21.457380 lama-cleaner-1.2.0/lama_cleaner/file_manager/
--rw-r--r--   0 cwq        (501) staff       (20)       38 2023-02-05 13:09:10.000000 lama-cleaner-1.2.0/lama_cleaner/file_manager/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)     8685 2023-04-02 07:46:39.000000 lama-cleaner-1.2.0/lama_cleaner/file_manager/file_manager.py
--rw-r--r--   0 cwq        (501) staff       (20)     1293 2023-02-05 13:09:10.000000 lama-cleaner-1.2.0/lama_cleaner/file_manager/storage_backends.py
--rw-r--r--   0 cwq        (501) staff       (20)     1758 2023-02-05 13:09:10.000000 lama-cleaner-1.2.0/lama_cleaner/file_manager/utils.py
--rw-r--r--   0 cwq        (501) staff       (20)     8651 2023-05-19 13:47:19.000000 lama-cleaner-1.2.0/lama_cleaner/helper.py
--rw-r--r--   0 cwq        (501) staff       (20)      232 2023-04-02 07:46:39.000000 lama-cleaner-1.2.0/lama_cleaner/installer.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-06-06 13:50:21.462484 lama-cleaner-1.2.0/lama_cleaner/model/
--rw-r--r--   0 cwq        (501) staff       (20)        0 2023-02-05 13:09:10.000000 lama-cleaner-1.2.0/lama_cleaner/model/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)     9606 2023-05-19 13:47:19.000000 lama-cleaner-1.2.0/lama_cleaner/model/base.py
--rw-r--r--   0 cwq        (501) staff       (20)    10883 2023-05-19 13:47:19.000000 lama-cleaner-1.2.0/lama_cleaner/model/controlnet.py
--rw-r--r--   0 cwq        (501) staff       (20)     6881 2023-02-05 13:09:10.000000 lama-cleaner-1.2.0/lama_cleaner/model/ddim_sampler.py
--rw-r--r--   0 cwq        (501) staff       (20)    57098 2023-02-27 13:02:16.000000 lama-cleaner-1.2.0/lama_cleaner/model/fcf.py
--rw-r--r--   0 cwq        (501) staff       (20)     3175 2023-03-01 13:56:56.000000 lama-cleaner-1.2.0/lama_cleaner/model/instruct_pix2pix.py
--rw-r--r--   0 cwq        (501) staff       (20)     1480 2023-02-27 13:02:16.000000 lama-cleaner-1.2.0/lama_cleaner/model/lama.py
--rw-r--r--   0 cwq        (501) staff       (20)    11275 2023-02-27 13:02:16.000000 lama-cleaner-1.2.0/lama_cleaner/model/ldm.py
--rw-r--r--   0 cwq        (501) staff       (20)     2884 2023-04-02 07:46:39.000000 lama-cleaner-1.2.0/lama_cleaner/model/manga.py
--rw-r--r--   0 cwq        (501) staff       (20)    62625 2023-04-02 07:46:39.000000 lama-cleaner-1.2.0/lama_cleaner/model/mat.py
--rw-r--r--   0 cwq        (501) staff       (20)      716 2023-02-19 13:09:51.000000 lama-cleaner-1.2.0/lama_cleaner/model/opencv2.py
--rw-r--r--   0 cwq        (501) staff       (20)     2934 2023-03-01 13:56:56.000000 lama-cleaner-1.2.0/lama_cleaner/model/paint_by_example.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-06-06 13:50:21.462983 lama-cleaner-1.2.0/lama_cleaner/model/pipeline/
--rw-r--r--   0 cwq        (501) staff       (20)      108 2023-05-01 05:55:02.000000 lama-cleaner-1.2.0/lama_cleaner/model/pipeline/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)    28156 2023-05-19 13:47:19.000000 lama-cleaner-1.2.0/lama_cleaner/model/pipeline/pipeline_stable_diffusion_controlnet_inpaint.py
--rw-r--r--   0 cwq        (501) staff       (20)    11851 2023-02-05 13:09:10.000000 lama-cleaner-1.2.0/lama_cleaner/model/plms_sampler.py
--rw-r--r--   0 cwq        (501) staff       (20)     6644 2023-05-19 13:47:19.000000 lama-cleaner-1.2.0/lama_cleaner/model/sd.py
--rw-r--r--   0 cwq        (501) staff       (20)    33811 2023-04-02 07:46:39.000000 lama-cleaner-1.2.0/lama_cleaner/model/utils.py
--rw-r--r--   0 cwq        (501) staff       (20)    15637 2023-04-16 13:06:47.000000 lama-cleaner-1.2.0/lama_cleaner/model/zits.py
--rw-r--r--   0 cwq        (501) staff       (20)     4091 2023-05-19 13:47:19.000000 lama-cleaner-1.2.0/lama_cleaner/model_manager.py
--rw-r--r--   0 cwq        (501) staff       (20)     8695 2023-05-29 13:40:18.000000 lama-cleaner-1.2.0/lama_cleaner/parse_args.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-06-06 13:50:21.464582 lama-cleaner-1.2.0/lama_cleaner/plugins/
--rw-r--r--   0 cwq        (501) staff       (20)      263 2023-05-19 13:47:19.000000 lama-cleaner-1.2.0/lama_cleaner/plugins/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)    13473 2023-05-19 13:47:19.000000 lama-cleaner-1.2.0/lama_cleaner/plugins/anime_seg.py
--rw-r--r--   0 cwq        (501) staff       (20)      280 2023-04-02 07:46:39.000000 lama-cleaner-1.2.0/lama_cleaner/plugins/base_plugin.py
--rw-r--r--   0 cwq        (501) staff       (20)     2400 2023-04-03 05:14:59.000000 lama-cleaner-1.2.0/lama_cleaner/plugins/gfpgan_plugin.py
--rw-r--r--   0 cwq        (501) staff       (20)     2750 2023-04-02 07:46:39.000000 lama-cleaner-1.2.0/lama_cleaner/plugins/gfpganer.py
--rw-r--r--   0 cwq        (501) staff       (20)     4156 2023-04-02 07:46:39.000000 lama-cleaner-1.2.0/lama_cleaner/plugins/gif.py
--rw-r--r--   0 cwq        (501) staff       (20)     2555 2023-04-06 14:12:49.000000 lama-cleaner-1.2.0/lama_cleaner/plugins/interactive_seg.py
--rw-r--r--   0 cwq        (501) staff       (20)     3573 2023-04-03 05:31:35.000000 lama-cleaner-1.2.0/lama_cleaner/plugins/realesrgan.py
--rw-r--r--   0 cwq        (501) staff       (20)     1053 2023-05-19 13:47:19.000000 lama-cleaner-1.2.0/lama_cleaner/plugins/remove_bg.py
--rw-r--r--   0 cwq        (501) staff       (20)     1747 2023-04-03 05:15:02.000000 lama-cleaner-1.2.0/lama_cleaner/plugins/restoreformer.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-06-06 13:50:21.465225 lama-cleaner-1.2.0/lama_cleaner/plugins/segment_anything/
--rw-r--r--   0 cwq        (501) staff       (20)      363 2023-04-06 14:12:49.000000 lama-cleaner-1.2.0/lama_cleaner/plugins/segment_anything/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)     2929 2023-04-06 14:12:49.000000 lama-cleaner-1.2.0/lama_cleaner/plugins/segment_anything/build_sam.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-06-06 13:50:21.466218 lama-cleaner-1.2.0/lama_cleaner/plugins/segment_anything/modeling/
--rw-r--r--   0 cwq        (501) staff       (20)      385 2023-04-06 14:12:49.000000 lama-cleaner-1.2.0/lama_cleaner/plugins/segment_anything/modeling/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)     1479 2023-04-06 14:12:49.000000 lama-cleaner-1.2.0/lama_cleaner/plugins/segment_anything/modeling/common.py
--rw-r--r--   0 cwq        (501) staff       (20)    14407 2023-04-06 14:12:49.000000 lama-cleaner-1.2.0/lama_cleaner/plugins/segment_anything/modeling/image_encoder.py
--rw-r--r--   0 cwq        (501) staff       (20)     6614 2023-04-06 14:12:49.000000 lama-cleaner-1.2.0/lama_cleaner/plugins/segment_anything/modeling/mask_decoder.py
--rw-r--r--   0 cwq        (501) staff       (20)     8594 2023-04-06 14:12:49.000000 lama-cleaner-1.2.0/lama_cleaner/plugins/segment_anything/modeling/prompt_encoder.py
--rw-r--r--   0 cwq        (501) staff       (20)     7225 2023-04-06 14:12:49.000000 lama-cleaner-1.2.0/lama_cleaner/plugins/segment_anything/modeling/sam.py
--rw-r--r--   0 cwq        (501) staff       (20)     8396 2023-04-06 14:12:49.000000 lama-cleaner-1.2.0/lama_cleaner/plugins/segment_anything/modeling/transformer.py
--rw-r--r--   0 cwq        (501) staff       (20)    11845 2023-04-10 01:29:17.000000 lama-cleaner-1.2.0/lama_cleaner/plugins/segment_anything/predictor.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-06-06 13:50:21.466494 lama-cleaner-1.2.0/lama_cleaner/plugins/segment_anything/utils/
--rw-r--r--   0 cwq        (501) staff       (20)      197 2023-04-06 14:12:49.000000 lama-cleaner-1.2.0/lama_cleaner/plugins/segment_anything/utils/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)     4054 2023-04-06 14:12:49.000000 lama-cleaner-1.2.0/lama_cleaner/plugins/segment_anything/utils/transforms.py
--rw-r--r--   0 cwq        (501) staff       (20)     1374 2023-04-16 13:06:47.000000 lama-cleaner-1.2.0/lama_cleaner/runtime.py
--rw-r--r--   0 cwq        (501) staff       (20)     3361 2023-05-19 13:47:19.000000 lama-cleaner-1.2.0/lama_cleaner/schema.py
--rw-r--r--   0 cwq        (501) staff       (20)    18543 2023-05-20 04:34:21.000000 lama-cleaner-1.2.0/lama_cleaner/server.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-06-06 13:50:21.468060 lama-cleaner-1.2.0/lama_cleaner/tests/
--rw-r--r--   0 cwq        (501) staff       (20)        0 2023-02-05 13:09:10.000000 lama-cleaner-1.2.0/lama_cleaner/tests/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)     6219 2023-05-19 13:47:19.000000 lama-cleaner-1.2.0/lama_cleaner/tests/test_controlnet.py
--rw-r--r--   0 cwq        (501) staff       (20)     2322 2023-05-19 13:47:19.000000 lama-cleaner-1.2.0/lama_cleaner/tests/test_instruct_pix2pix.py
--rw-r--r--   0 cwq        (501) staff       (20)      596 2023-02-05 13:09:10.000000 lama-cleaner-1.2.0/lama_cleaner/tests/test_load_img.py
--rw-r--r--   0 cwq        (501) staff       (20)     5826 2023-04-02 07:46:39.000000 lama-cleaner-1.2.0/lama_cleaner/tests/test_model.py
--rw-r--r--   0 cwq        (501) staff       (20)     1505 2023-05-19 13:47:19.000000 lama-cleaner-1.2.0/lama_cleaner/tests/test_model_md5.py
--rw-r--r--   0 cwq        (501) staff       (20)     3985 2023-02-05 13:09:10.000000 lama-cleaner-1.2.0/lama_cleaner/tests/test_paint_by_example.py
--rw-r--r--   0 cwq        (501) staff       (20)     2965 2023-05-19 13:47:19.000000 lama-cleaner-1.2.0/lama_cleaner/tests/test_plugins.py
--rw-r--r--   0 cwq        (501) staff       (20)     1128 2023-05-19 13:47:19.000000 lama-cleaner-1.2.0/lama_cleaner/tests/test_save_exif.py
--rw-r--r--   0 cwq        (501) staff       (20)     7647 2023-04-02 07:46:39.000000 lama-cleaner-1.2.0/lama_cleaner/tests/test_sd_model.py
--rw-r--r--   0 cwq        (501) staff       (20)     8530 2023-05-19 13:47:19.000000 lama-cleaner-1.2.0/lama_cleaner/web_config.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-06-06 13:50:21.429767 lama-cleaner-1.2.0/lama_cleaner.egg-info/
--rw-r--r--   0 cwq        (501) staff       (20)     4918 2023-06-06 13:50:21.000000 lama-cleaner-1.2.0/lama_cleaner.egg-info/PKG-INFO
--rw-r--r--   0 cwq        (501) staff       (20)     6141 2023-06-06 13:50:21.000000 lama-cleaner-1.2.0/lama_cleaner.egg-info/SOURCES.txt
--rw-r--r--   0 cwq        (501) staff       (20)        1 2023-06-06 13:50:21.000000 lama-cleaner-1.2.0/lama_cleaner.egg-info/dependency_links.txt
--rw-r--r--   0 cwq        (501) staff       (20)       59 2023-06-06 13:50:21.000000 lama-cleaner-1.2.0/lama_cleaner.egg-info/entry_points.txt
--rw-r--r--   0 cwq        (501) staff       (20)      232 2023-06-06 13:50:21.000000 lama-cleaner-1.2.0/lama_cleaner.egg-info/requires.txt
--rw-r--r--   0 cwq        (501) staff       (20)       13 2023-06-06 13:50:21.000000 lama-cleaner-1.2.0/lama_cleaner.egg-info/top_level.txt
--rw-r--r--   0 cwq        (501) staff       (20)       38 2023-06-06 13:50:21.468549 lama-cleaner-1.2.0/setup.cfg
--rw-r--r--   0 cwq        (501) staff       (20)     1616 2023-06-06 13:36:34.000000 lama-cleaner-1.2.0/setup.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-06-17 14:06:15.967591 lama-cleaner-1.2.1/
+-rw-r--r--   0 cwq        (501) staff       (20)    11357 2023-02-05 13:09:10.000000 lama-cleaner-1.2.1/LICENSE
+-rw-r--r--   0 cwq        (501) staff       (20)     4273 2023-06-17 14:06:15.967476 lama-cleaner-1.2.1/PKG-INFO
+-rw-r--r--   0 cwq        (501) staff       (20)     3544 2023-06-17 14:05:39.000000 lama-cleaner-1.2.1/README.md
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-06-17 14:06:15.929493 lama-cleaner-1.2.1/lama_cleaner/
+-rw-r--r--   0 cwq        (501) staff       (20)      488 2023-04-02 07:46:39.000000 lama-cleaner-1.2.1/lama_cleaner/__init__.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-06-17 14:06:15.926660 lama-cleaner-1.2.1/lama_cleaner/app/
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-06-17 14:06:15.931649 lama-cleaner-1.2.1/lama_cleaner/app/build/
+-rw-r--r--   0 cwq        (501) staff       (20)     6148 2023-05-19 13:47:41.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/.DS_Store
+-rw-r--r--   0 cwq        (501) staff       (20)     4559 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/asset-manifest.json
+-rw-r--r--   0 cwq        (501) staff       (20)    67646 2023-05-19 13:47:41.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/favicon.ico
+-rw-r--r--   0 cwq        (501) staff       (20)      719 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/index.html
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-06-17 14:06:15.926922 lama-cleaner-1.2.1/lama_cleaner/app/build/static/
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-06-17 14:06:15.931878 lama-cleaner-1.2.1/lama_cleaner/app/build/static/css/
+-rw-r--r--   0 cwq        (501) staff       (20)    39068 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/css/main.ce986cc8.css
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-06-17 14:06:15.933730 lama-cleaner-1.2.1/lama_cleaner/app/build/static/js/
+-rw-r--r--   0 cwq        (501) staff       (20)   831766 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/js/main.1fda6320.js
+-rw-r--r--   0 cwq        (501) staff       (20)     1971 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/js/main.1fda6320.js.LICENSE.txt
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-06-17 14:06:15.957407 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/
+-rw-r--r--   0 cwq        (501) staff       (20)   102868 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-Black.15ca31c0a2a68f76d2d1.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   138764 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-Black.c6938660eec019fefd68.woff
+-rw-r--r--   0 cwq        (501) staff       (20)   146824 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-BlackItalic.ca1e738e4f349f27514d.woff
+-rw-r--r--   0 cwq        (501) staff       (20)   108752 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-BlackItalic.cb2a7335650c690077fe.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   143208 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-Bold.93c1301bd9f486c573b3.woff
+-rw-r--r--   0 cwq        (501) staff       (20)   106140 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-Bold.ec64ea577b0349e055ad.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   111808 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-BoldItalic.2d26c56a606662486796.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   151052 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-BoldItalic.b376885042f6c961a541.woff
+-rw-r--r--   0 cwq        (501) staff       (20)   106108 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-ExtraBold.cbe0ae49c52c920fd563.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   142920 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-ExtraBold.d0fa3bb2b7c9063dc594.woff
+-rw-r--r--   0 cwq        (501) staff       (20)   111708 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-ExtraBoldItalic.535a6cf662596b3bd6a6.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   150628 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-ExtraBoldItalic.6ab17abedc4d3f140953.woff
+-rw-r--r--   0 cwq        (501) staff       (20)   104232 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-ExtraLight.72505e6a122c6acd5471.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   140724 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-ExtraLight.c4248615291a9e8f1fb7.woff
+-rw-r--r--   0 cwq        (501) staff       (20)   149996 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-ExtraLightItalic.170dddfca278d3c2ad4a.woff
+-rw-r--r--   0 cwq        (501) staff       (20)   111392 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-ExtraLightItalic.5c7d7d6deb1d2ec8d48c.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   144372 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-Italic.890025e726861dba417f.woff
+-rw-r--r--   0 cwq        (501) staff       (20)   106876 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-Italic.cb10ffd7684cd9836a05.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   104332 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-Light.2d5198822ab091ce4305.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   140632 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-Light.994e34451cc19ede31d3.woff
+-rw-r--r--   0 cwq        (501) staff       (20)   150092 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-LightItalic.ef9f65d91d2b0ba9b2e4.woff
+-rw-r--r--   0 cwq        (501) staff       (20)   111332 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-LightItalic.f86952265d7b0f02c921.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   105924 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-Medium.293fd13dbca5a3e450ef.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   142552 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-Medium.9053572c46aeb4b16caa.woff
+-rw-r--r--   0 cwq        (501) staff       (20)   112184 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-MediumItalic.085cb93e613ba3d40d2b.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   150988 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-MediumItalic.3d0107dd43d0101274d3.woff
+-rw-r--r--   0 cwq        (501) staff       (20)   133844 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-Regular.8c206db99195777c6769.woff
+-rw-r--r--   0 cwq        (501) staff       (20)    98868 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-Regular.c8ba52b05a9ef10f4758.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   105804 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-SemiBold.b5f0f109bc88052d4000.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   142932 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-SemiBold.cca62d21c8c555c392e5.woff
+-rw-r--r--   0 cwq        (501) staff       (20)   151180 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-SemiBoldItalic.463bdbfb28abad0fa6df.woff
+-rw-r--r--   0 cwq        (501) staff       (20)   112048 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-SemiBoldItalic.d9467ee321a8f38aefff.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   135920 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-Thin.29b9c616a95a912abf73.woff
+-rw-r--r--   0 cwq        (501) staff       (20)    99632 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-Thin.fff2a096db014f6239d4.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   145480 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-ThinItalic.bae95eb2f889c797e435.woff
+-rw-r--r--   0 cwq        (501) staff       (20)   106496 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-ThinItalic.bf213704dce6b437ede4.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   245036 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-italic.var.30807be7abc48ba8c73c.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   227180 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-roman.var.ba4caefcdf5b36b438db.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   324864 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter.var.c2fe3cb2b7c746f7966a.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   431724 2023-05-19 13:47:58.000000 lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/coffee-machine-lineal.ee32631219cc3986f861.gif
+-rw-r--r--   0 cwq        (501) staff       (20)     3244 2023-02-05 13:09:10.000000 lama-cleaner-1.2.1/lama_cleaner/benchmark.py
+-rw-r--r--   0 cwq        (501) staff       (20)     5145 2023-05-19 13:47:19.000000 lama-cleaner-1.2.1/lama_cleaner/const.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-06-17 14:06:15.960240 lama-cleaner-1.2.1/lama_cleaner/file_manager/
+-rw-r--r--   0 cwq        (501) staff       (20)       38 2023-02-05 13:09:10.000000 lama-cleaner-1.2.1/lama_cleaner/file_manager/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)     8685 2023-04-02 07:46:39.000000 lama-cleaner-1.2.1/lama_cleaner/file_manager/file_manager.py
+-rw-r--r--   0 cwq        (501) staff       (20)     1293 2023-02-05 13:09:10.000000 lama-cleaner-1.2.1/lama_cleaner/file_manager/storage_backends.py
+-rw-r--r--   0 cwq        (501) staff       (20)     1758 2023-02-05 13:09:10.000000 lama-cleaner-1.2.1/lama_cleaner/file_manager/utils.py
+-rw-r--r--   0 cwq        (501) staff       (20)     8651 2023-05-19 13:47:19.000000 lama-cleaner-1.2.1/lama_cleaner/helper.py
+-rw-r--r--   0 cwq        (501) staff       (20)      232 2023-04-02 07:46:39.000000 lama-cleaner-1.2.1/lama_cleaner/installer.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-06-17 14:06:15.962284 lama-cleaner-1.2.1/lama_cleaner/model/
+-rw-r--r--   0 cwq        (501) staff       (20)        0 2023-02-05 13:09:10.000000 lama-cleaner-1.2.1/lama_cleaner/model/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)     9606 2023-05-19 13:47:19.000000 lama-cleaner-1.2.1/lama_cleaner/model/base.py
+-rw-r--r--   0 cwq        (501) staff       (20)    10883 2023-05-19 13:47:19.000000 lama-cleaner-1.2.1/lama_cleaner/model/controlnet.py
+-rw-r--r--   0 cwq        (501) staff       (20)     6881 2023-02-05 13:09:10.000000 lama-cleaner-1.2.1/lama_cleaner/model/ddim_sampler.py
+-rw-r--r--   0 cwq        (501) staff       (20)    57098 2023-02-27 13:02:16.000000 lama-cleaner-1.2.1/lama_cleaner/model/fcf.py
+-rw-r--r--   0 cwq        (501) staff       (20)     3175 2023-03-01 13:56:56.000000 lama-cleaner-1.2.1/lama_cleaner/model/instruct_pix2pix.py
+-rw-r--r--   0 cwq        (501) staff       (20)     1480 2023-02-27 13:02:16.000000 lama-cleaner-1.2.1/lama_cleaner/model/lama.py
+-rw-r--r--   0 cwq        (501) staff       (20)    11275 2023-02-27 13:02:16.000000 lama-cleaner-1.2.1/lama_cleaner/model/ldm.py
+-rw-r--r--   0 cwq        (501) staff       (20)     2884 2023-04-02 07:46:39.000000 lama-cleaner-1.2.1/lama_cleaner/model/manga.py
+-rw-r--r--   0 cwq        (501) staff       (20)    62625 2023-04-02 07:46:39.000000 lama-cleaner-1.2.1/lama_cleaner/model/mat.py
+-rw-r--r--   0 cwq        (501) staff       (20)      716 2023-02-19 13:09:51.000000 lama-cleaner-1.2.1/lama_cleaner/model/opencv2.py
+-rw-r--r--   0 cwq        (501) staff       (20)     2934 2023-03-01 13:56:56.000000 lama-cleaner-1.2.1/lama_cleaner/model/paint_by_example.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-06-17 14:06:15.962621 lama-cleaner-1.2.1/lama_cleaner/model/pipeline/
+-rw-r--r--   0 cwq        (501) staff       (20)      108 2023-05-01 05:55:02.000000 lama-cleaner-1.2.1/lama_cleaner/model/pipeline/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)    28156 2023-05-19 13:47:19.000000 lama-cleaner-1.2.1/lama_cleaner/model/pipeline/pipeline_stable_diffusion_controlnet_inpaint.py
+-rw-r--r--   0 cwq        (501) staff       (20)    11851 2023-02-05 13:09:10.000000 lama-cleaner-1.2.1/lama_cleaner/model/plms_sampler.py
+-rw-r--r--   0 cwq        (501) staff       (20)     6644 2023-05-19 13:47:19.000000 lama-cleaner-1.2.1/lama_cleaner/model/sd.py
+-rw-r--r--   0 cwq        (501) staff       (20)    33811 2023-04-02 07:46:39.000000 lama-cleaner-1.2.1/lama_cleaner/model/utils.py
+-rw-r--r--   0 cwq        (501) staff       (20)    15637 2023-04-16 13:06:47.000000 lama-cleaner-1.2.1/lama_cleaner/model/zits.py
+-rw-r--r--   0 cwq        (501) staff       (20)     4091 2023-05-19 13:47:19.000000 lama-cleaner-1.2.1/lama_cleaner/model_manager.py
+-rw-r--r--   0 cwq        (501) staff       (20)     8695 2023-05-29 13:40:18.000000 lama-cleaner-1.2.1/lama_cleaner/parse_args.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-06-17 14:06:15.963889 lama-cleaner-1.2.1/lama_cleaner/plugins/
+-rw-r--r--   0 cwq        (501) staff       (20)      263 2023-05-19 13:47:19.000000 lama-cleaner-1.2.1/lama_cleaner/plugins/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)    13473 2023-05-19 13:47:19.000000 lama-cleaner-1.2.1/lama_cleaner/plugins/anime_seg.py
+-rw-r--r--   0 cwq        (501) staff       (20)      280 2023-04-02 07:46:39.000000 lama-cleaner-1.2.1/lama_cleaner/plugins/base_plugin.py
+-rw-r--r--   0 cwq        (501) staff       (20)     2400 2023-04-03 05:14:59.000000 lama-cleaner-1.2.1/lama_cleaner/plugins/gfpgan_plugin.py
+-rw-r--r--   0 cwq        (501) staff       (20)     2750 2023-04-02 07:46:39.000000 lama-cleaner-1.2.1/lama_cleaner/plugins/gfpganer.py
+-rw-r--r--   0 cwq        (501) staff       (20)     4156 2023-04-02 07:46:39.000000 lama-cleaner-1.2.1/lama_cleaner/plugins/gif.py
+-rw-r--r--   0 cwq        (501) staff       (20)     2555 2023-04-06 14:12:49.000000 lama-cleaner-1.2.1/lama_cleaner/plugins/interactive_seg.py
+-rw-r--r--   0 cwq        (501) staff       (20)     3573 2023-04-03 05:31:35.000000 lama-cleaner-1.2.1/lama_cleaner/plugins/realesrgan.py
+-rw-r--r--   0 cwq        (501) staff       (20)     1053 2023-05-19 13:47:19.000000 lama-cleaner-1.2.1/lama_cleaner/plugins/remove_bg.py
+-rw-r--r--   0 cwq        (501) staff       (20)     1747 2023-04-03 05:15:02.000000 lama-cleaner-1.2.1/lama_cleaner/plugins/restoreformer.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-06-17 14:06:15.964209 lama-cleaner-1.2.1/lama_cleaner/plugins/segment_anything/
+-rw-r--r--   0 cwq        (501) staff       (20)      363 2023-04-06 14:12:49.000000 lama-cleaner-1.2.1/lama_cleaner/plugins/segment_anything/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)     2929 2023-04-06 14:12:49.000000 lama-cleaner-1.2.1/lama_cleaner/plugins/segment_anything/build_sam.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-06-17 14:06:15.965119 lama-cleaner-1.2.1/lama_cleaner/plugins/segment_anything/modeling/
+-rw-r--r--   0 cwq        (501) staff       (20)      385 2023-04-06 14:12:49.000000 lama-cleaner-1.2.1/lama_cleaner/plugins/segment_anything/modeling/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)     1479 2023-04-06 14:12:49.000000 lama-cleaner-1.2.1/lama_cleaner/plugins/segment_anything/modeling/common.py
+-rw-r--r--   0 cwq        (501) staff       (20)    14407 2023-04-06 14:12:49.000000 lama-cleaner-1.2.1/lama_cleaner/plugins/segment_anything/modeling/image_encoder.py
+-rw-r--r--   0 cwq        (501) staff       (20)     6614 2023-04-06 14:12:49.000000 lama-cleaner-1.2.1/lama_cleaner/plugins/segment_anything/modeling/mask_decoder.py
+-rw-r--r--   0 cwq        (501) staff       (20)     8594 2023-04-06 14:12:49.000000 lama-cleaner-1.2.1/lama_cleaner/plugins/segment_anything/modeling/prompt_encoder.py
+-rw-r--r--   0 cwq        (501) staff       (20)     7225 2023-04-06 14:12:49.000000 lama-cleaner-1.2.1/lama_cleaner/plugins/segment_anything/modeling/sam.py
+-rw-r--r--   0 cwq        (501) staff       (20)     8396 2023-04-06 14:12:49.000000 lama-cleaner-1.2.1/lama_cleaner/plugins/segment_anything/modeling/transformer.py
+-rw-r--r--   0 cwq        (501) staff       (20)    11845 2023-04-10 01:29:17.000000 lama-cleaner-1.2.1/lama_cleaner/plugins/segment_anything/predictor.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-06-17 14:06:15.965495 lama-cleaner-1.2.1/lama_cleaner/plugins/segment_anything/utils/
+-rw-r--r--   0 cwq        (501) staff       (20)      197 2023-04-06 14:12:49.000000 lama-cleaner-1.2.1/lama_cleaner/plugins/segment_anything/utils/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)     4054 2023-04-06 14:12:49.000000 lama-cleaner-1.2.1/lama_cleaner/plugins/segment_anything/utils/transforms.py
+-rw-r--r--   0 cwq        (501) staff       (20)     1374 2023-04-16 13:06:47.000000 lama-cleaner-1.2.1/lama_cleaner/runtime.py
+-rw-r--r--   0 cwq        (501) staff       (20)     3361 2023-05-19 13:47:19.000000 lama-cleaner-1.2.1/lama_cleaner/schema.py
+-rw-r--r--   0 cwq        (501) staff       (20)    18878 2023-06-17 14:05:39.000000 lama-cleaner-1.2.1/lama_cleaner/server.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-06-17 14:06:15.967198 lama-cleaner-1.2.1/lama_cleaner/tests/
+-rw-r--r--   0 cwq        (501) staff       (20)        0 2023-02-05 13:09:10.000000 lama-cleaner-1.2.1/lama_cleaner/tests/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)     6219 2023-05-19 13:47:19.000000 lama-cleaner-1.2.1/lama_cleaner/tests/test_controlnet.py
+-rw-r--r--   0 cwq        (501) staff       (20)     2322 2023-05-19 13:47:19.000000 lama-cleaner-1.2.1/lama_cleaner/tests/test_instruct_pix2pix.py
+-rw-r--r--   0 cwq        (501) staff       (20)      596 2023-02-05 13:09:10.000000 lama-cleaner-1.2.1/lama_cleaner/tests/test_load_img.py
+-rw-r--r--   0 cwq        (501) staff       (20)     5826 2023-04-02 07:46:39.000000 lama-cleaner-1.2.1/lama_cleaner/tests/test_model.py
+-rw-r--r--   0 cwq        (501) staff       (20)     1505 2023-05-19 13:47:19.000000 lama-cleaner-1.2.1/lama_cleaner/tests/test_model_md5.py
+-rw-r--r--   0 cwq        (501) staff       (20)     3985 2023-02-05 13:09:10.000000 lama-cleaner-1.2.1/lama_cleaner/tests/test_paint_by_example.py
+-rw-r--r--   0 cwq        (501) staff       (20)     2965 2023-05-19 13:47:19.000000 lama-cleaner-1.2.1/lama_cleaner/tests/test_plugins.py
+-rw-r--r--   0 cwq        (501) staff       (20)     1128 2023-05-19 13:47:19.000000 lama-cleaner-1.2.1/lama_cleaner/tests/test_save_exif.py
+-rw-r--r--   0 cwq        (501) staff       (20)     7647 2023-04-02 07:46:39.000000 lama-cleaner-1.2.1/lama_cleaner/tests/test_sd_model.py
+-rw-r--r--   0 cwq        (501) staff       (20)     8530 2023-05-19 13:47:19.000000 lama-cleaner-1.2.1/lama_cleaner/web_config.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-06-17 14:06:15.930239 lama-cleaner-1.2.1/lama_cleaner.egg-info/
+-rw-r--r--   0 cwq        (501) staff       (20)     4273 2023-06-17 14:06:15.000000 lama-cleaner-1.2.1/lama_cleaner.egg-info/PKG-INFO
+-rw-r--r--   0 cwq        (501) staff       (20)     6141 2023-06-17 14:06:15.000000 lama-cleaner-1.2.1/lama_cleaner.egg-info/SOURCES.txt
+-rw-r--r--   0 cwq        (501) staff       (20)        1 2023-06-17 14:06:15.000000 lama-cleaner-1.2.1/lama_cleaner.egg-info/dependency_links.txt
+-rw-r--r--   0 cwq        (501) staff       (20)       58 2023-06-17 14:06:15.000000 lama-cleaner-1.2.1/lama_cleaner.egg-info/entry_points.txt
+-rw-r--r--   0 cwq        (501) staff       (20)      232 2023-06-17 14:06:15.000000 lama-cleaner-1.2.1/lama_cleaner.egg-info/requires.txt
+-rw-r--r--   0 cwq        (501) staff       (20)       13 2023-06-17 14:06:15.000000 lama-cleaner-1.2.1/lama_cleaner.egg-info/top_level.txt
+-rw-r--r--   0 cwq        (501) staff       (20)       38 2023-06-17 14:06:15.967635 lama-cleaner-1.2.1/setup.cfg
+-rw-r--r--   0 cwq        (501) staff       (20)     1616 2023-06-17 14:05:54.000000 lama-cleaner-1.2.1/setup.py
```

### Comparing `lama-cleaner-1.2.0/LICENSE` & `lama-cleaner-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/PKG-INFO` & `lama-cleaner-1.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,108 +1,108 @@
 Metadata-Version: 2.1
 Name: lama-cleaner
-Version: 1.2.0
+Version: 1.2.1
 Summary: Image inpainting tool powered by SOTA AI Model
 Home-page: https://github.com/Sanster/lama-cleaner
 Author: PanicByte
 Author-email: cwq1913@gmail.com
-License: UNKNOWN
-Description: <p align="center">
-           <img alt="logo" height=256 src="./assets/logo.png" />
-        </p>
-        <h1 align="center">Lama Cleaner</h1>
-        <p align="center">A free and open-source inpainting tool powered by SOTA AI model.</p>
-        
-        <p align="center">
-          <a href="https://github.com/Sanster/lama-cleaner">
-            <img alt="total download" src="https://pepy.tech/badge/lama-cleaner" />
-          </a>
-          <a href="https://pypi.org/project/lama-cleaner/">
-            <img alt="version" src="https://img.shields.io/pypi/v/lama-cleaner" />
-          </a>
-          <a href="https://colab.research.google.com/drive/1e3ZkAJxvkK3uzaTGu91N9TvI_Mahs0Wb?usp=sharing">
-            <img alt="Open in Colab" src="https://colab.research.google.com/assets/colab-badge.svg" />
-          </a>
-        
-          <a href="https://huggingface.co/spaces/Sanster/Lama-Cleaner-lama">
-            <img alt="Hugging Face Spaces" src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue" />
-          </a>
-        
-          <a href="">
-            <img alt="python version" src="https://img.shields.io/pypi/pyversions/lama-cleaner" />
-          </a>
-          <a href="https://hub.docker.com/r/cwq1913/lama-cleaner">
-            <img alt="version" src="https://img.shields.io/docker/pulls/cwq1913/lama-cleaner" />
-          </a>
-        </p>
-        
-        https://user-images.githubusercontent.com/3998421/196976498-ba1ad3ab-fa18-4c55-965f-5c6683141375.mp4
-        
-        ## Sponsor
-        
-        <table>
-           <tr>
-            <td >
-                <img src="./assets/GitHub_Copilot_logo.svg" style="background: white;padding: 8px;"/>
-            </td>
-            <td >
-              <a href="https://ko-fi.com/Z8Z1CZJGY/tiers" target="_blank" >
-                ❤️ Your logo
-              </a>
-            </td>
-          </tr>
-        </table>
-        
-        ## Features
-        
-        - Completely free and open-source, fully self-hosted, support CPU & GPU & M1/2
-        - [Windows 1-Click Installer](https://lama-cleaner-docs.vercel.app/install/windows_1click_installer)
-        - Multiple SOTA AI [models](https://lama-cleaner-docs.vercel.app/models)
-          - Erase model: LaMa/LDM/ZITS/MAT/FcF/Manga
-          - Erase and Replace model: Stable Diffusion/Paint by Example
-        - [Plugins](https://lama-cleaner-docs.vercel.app/plugins) for post-processing:
-          - [RemoveBG](https://github.com/danielgatis/rembg): Remove images background 
-          - [RealESRGAN](https://github.com/xinntao/Real-ESRGAN): Super Resolution
-          - [GFPGAN](https://github.com/TencentARC/GFPGAN): Face Restoration
-          - [RestoreFormer](https://github.com/wzhouxiff/RestoreFormer): Face Restoration
-          - [Segment Anything](https://lama-cleaner-docs.vercel.app/plugins#interactive-segmentation): Accurate and fast interactive object segmentation
-        - More features at [lama-cleaner-docs](https://lama-cleaner-docs.vercel.app/)
-        
-        ## Quick Start
-        
-        Lama Cleaner make it easy to use SOTA AI model in just two commands:
-        
-        ```bash
-        # In order to use the GPU, install cuda version of pytorch first.
-        # pip install torch==1.13.1+cu117 torchvision==0.14.1 --extra-index-url https://download.pytorch.org/whl/cu117
-        pip install lama-cleaner
-        lama-cleaner --model=lama --device=cpu --port=8080
-        ```
-        
-        That's it, Lama Cleaner is now running at http://localhost:8080
-        
-        See all command line arguments at [lama-cleaner-docs](https://lama-cleaner-docs.vercel.app/install/pip)
-        
-        ## Development
-        
-        Only needed if you plan to modify the frontend and recompile yourself.
-        
-        ### Frontend
-        
-        Frontend code are modified from [cleanup.pictures](https://github.com/initml/cleanup.pictures), You can experience their
-        great online services [here](https://cleanup.pictures/).
-        
-        - Install dependencies:`cd lama_cleaner/app/ && pnpm install`
-        - Start development server: `pnpm start`
-        - Build: `pnpm build`
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center">
+   <img alt="logo" height=256 src="./assets/logo.png" />
+</p>
+<h1 align="center">Lama Cleaner</h1>
+<p align="center">A free and open-source inpainting tool powered by SOTA AI model.</p>
+
+<p align="center">
+  <a href="https://github.com/Sanster/lama-cleaner">
+    <img alt="total download" src="https://pepy.tech/badge/lama-cleaner" />
+  </a>
+  <a href="https://pypi.org/project/lama-cleaner/">
+    <img alt="version" src="https://img.shields.io/pypi/v/lama-cleaner" />
+  </a>
+  <a href="https://colab.research.google.com/drive/1e3ZkAJxvkK3uzaTGu91N9TvI_Mahs0Wb?usp=sharing">
+    <img alt="Open in Colab" src="https://colab.research.google.com/assets/colab-badge.svg" />
+  </a>
+
+  <a href="https://huggingface.co/spaces/Sanster/Lama-Cleaner-lama">
+    <img alt="Hugging Face Spaces" src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue" />
+  </a>
+
+  <a href="">
+    <img alt="python version" src="https://img.shields.io/pypi/pyversions/lama-cleaner" />
+  </a>
+  <a href="https://hub.docker.com/r/cwq1913/lama-cleaner">
+    <img alt="version" src="https://img.shields.io/docker/pulls/cwq1913/lama-cleaner" />
+  </a>
+</p>
+
+https://user-images.githubusercontent.com/3998421/196976498-ba1ad3ab-fa18-4c55-965f-5c6683141375.mp4
+
+## Sponsor
+
+<table>
+   <tr>
+    <td >
+        <img src="./assets/GitHub_Copilot_logo.svg" style="background: white;padding: 8px;"/>
+    </td>
+    <td >
+      <a href="https://ko-fi.com/Z8Z1CZJGY/tiers" target="_blank" >
+        ❤️ Your logo
+      </a>
+    </td>
+  </tr>
+</table>
+
+## Features
+
+- Completely free and open-source, fully self-hosted, support CPU & GPU & M1/2
+- [Windows 1-Click Installer](https://lama-cleaner-docs.vercel.app/install/windows_1click_installer)
+- [WIP: A native macOS app](https://github.com/Sanster/lama-cleaner/discussions/314)
+- Multiple SOTA AI [models](https://lama-cleaner-docs.vercel.app/models)
+  - Erase model: LaMa/LDM/ZITS/MAT/FcF/Manga
+  - Erase and Replace model: Stable Diffusion/Paint by Example
+- [Plugins](https://lama-cleaner-docs.vercel.app/plugins) for post-processing:
+  - [RemoveBG](https://github.com/danielgatis/rembg): Remove images background 
+  - [RealESRGAN](https://github.com/xinntao/Real-ESRGAN): Super Resolution
+  - [GFPGAN](https://github.com/TencentARC/GFPGAN): Face Restoration
+  - [RestoreFormer](https://github.com/wzhouxiff/RestoreFormer): Face Restoration
+  - [Segment Anything](https://lama-cleaner-docs.vercel.app/plugins#interactive-segmentation): Accurate and fast interactive object segmentation
+- More features at [lama-cleaner-docs](https://lama-cleaner-docs.vercel.app/)
+
+## Quick Start
+
+Lama Cleaner make it easy to use SOTA AI model in just two commands:
+
+```bash
+# In order to use the GPU, install cuda version of pytorch first.
+# pip install torch==1.13.1+cu117 torchvision==0.14.1 --extra-index-url https://download.pytorch.org/whl/cu117
+pip install lama-cleaner
+lama-cleaner --model=lama --device=cpu --port=8080
+```
+
+That's it, Lama Cleaner is now running at http://localhost:8080
+
+See all command line arguments at [lama-cleaner-docs](https://lama-cleaner-docs.vercel.app/install/pip)
+
+## Development
+
+Only needed if you plan to modify the frontend and recompile yourself.
+
+### Frontend
+
+Frontend code are modified from [cleanup.pictures](https://github.com/initml/cleanup.pictures), You can experience their
+great online services [here](https://cleanup.pictures/).
+
+- Install dependencies:`cd lama_cleaner/app/ && pnpm install`
+- Start development server: `pnpm start`
+- Build: `pnpm build`
```

#### html2text {}

```diff
@@ -1,44 +1,44 @@
-Metadata-Version: 2.1 Name: lama-cleaner Version: 1.2.0 Summary: Image
+Metadata-Version: 2.1 Name: lama-cleaner Version: 1.2.1 Summary: Image
 inpainting tool powered by SOTA AI Model Home-page: https://github.com/Sanster/
-lama-cleaner Author: PanicByte Author-email: cwq1913@gmail.com License: UNKNOWN
-Description:
+lama-cleaner Author: PanicByte Author-email: cwq1913@gmail.com Classifier:
+License :: OSI Approved :: Apache Software License Classifier: Operating System
+:: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Topic :: Scientific/
+Engineering :: Artificial Intelligence Requires-Python: >=3.7 Description-
+Content-Type: text/markdown License-File: LICENSE
                                     [logo]
                           ****** Lama Cleaner ******
        A free and open-source inpainting tool powered by SOTA AI model.
    [total_download] [version] [Open_in_Colab] [Hugging_Face_Spaces] [python
                               version] [version]
 https://user-images.githubusercontent.com/3998421/196976498-ba1ad3ab-fa18-4c55-
 965f-5c6683141375.mp4 ## Sponsor
 [./assets/GitHub_Copilot_logo.svg] â¤ï¸_Your_logo
 ## Features - Completely free and open-source, fully self-hosted, support CPU &
 GPU & M1/2 - [Windows 1-Click Installer](https://lama-cleaner-docs.vercel.app/
-install/windows_1click_installer) - Multiple SOTA AI [models](https://lama-
-cleaner-docs.vercel.app/models) - Erase model: LaMa/LDM/ZITS/MAT/FcF/Manga -
-Erase and Replace model: Stable Diffusion/Paint by Example - [Plugins](https://
-lama-cleaner-docs.vercel.app/plugins) for post-processing: - [RemoveBG](https:/
-/github.com/danielgatis/rembg): Remove images background - [RealESRGAN](https:/
-/github.com/xinntao/Real-ESRGAN): Super Resolution - [GFPGAN](https://
-github.com/TencentARC/GFPGAN): Face Restoration - [RestoreFormer](https://
-github.com/wzhouxiff/RestoreFormer): Face Restoration - [Segment Anything]
-(https://lama-cleaner-docs.vercel.app/plugins#interactive-segmentation):
-Accurate and fast interactive object segmentation - More features at [lama-
-cleaner-docs](https://lama-cleaner-docs.vercel.app/) ## Quick Start Lama
-Cleaner make it easy to use SOTA AI model in just two commands: ```bash # In
-order to use the GPU, install cuda version of pytorch first. # pip install
-torch==1.13.1+cu117 torchvision==0.14.1 --extra-index-url https://
+install/windows_1click_installer) - [WIP: A native macOS app](https://
+github.com/Sanster/lama-cleaner/discussions/314) - Multiple SOTA AI [models]
+(https://lama-cleaner-docs.vercel.app/models) - Erase model: LaMa/LDM/ZITS/MAT/
+FcF/Manga - Erase and Replace model: Stable Diffusion/Paint by Example -
+[Plugins](https://lama-cleaner-docs.vercel.app/plugins) for post-processing: -
+[RemoveBG](https://github.com/danielgatis/rembg): Remove images background -
+[RealESRGAN](https://github.com/xinntao/Real-ESRGAN): Super Resolution -
+[GFPGAN](https://github.com/TencentARC/GFPGAN): Face Restoration -
+[RestoreFormer](https://github.com/wzhouxiff/RestoreFormer): Face Restoration -
+[Segment Anything](https://lama-cleaner-docs.vercel.app/plugins#interactive-
+segmentation): Accurate and fast interactive object segmentation - More
+features at [lama-cleaner-docs](https://lama-cleaner-docs.vercel.app/) ## Quick
+Start Lama Cleaner make it easy to use SOTA AI model in just two commands:
+```bash # In order to use the GPU, install cuda version of pytorch first. # pip
+install torch==1.13.1+cu117 torchvision==0.14.1 --extra-index-url https://
 download.pytorch.org/whl/cu117 pip install lama-cleaner lama-cleaner --
 model=lama --device=cpu --port=8080 ``` That's it, Lama Cleaner is now running
 at http://localhost:8080 See all command line arguments at [lama-cleaner-docs]
 (https://lama-cleaner-docs.vercel.app/install/pip) ## Development Only needed
 if you plan to modify the frontend and recompile yourself. ### Frontend
 Frontend code are modified from [cleanup.pictures](https://github.com/initml/
 cleanup.pictures), You can experience their great online services [here](https:
 //cleanup.pictures/). - Install dependencies:`cd lama_cleaner/app/ && pnpm
 install` - Start development server: `pnpm start` - Build: `pnpm build`
-Platform: UNKNOWN Classifier: License :: OSI Approved :: Apache Software
-License Classifier: Operating System :: OS Independent Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `lama-cleaner-1.2.0/README.md` & `lama-cleaner-1.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -44,14 +44,15 @@
   </tr>
 </table>
 
 ## Features
 
 - Completely free and open-source, fully self-hosted, support CPU & GPU & M1/2
 - [Windows 1-Click Installer](https://lama-cleaner-docs.vercel.app/install/windows_1click_installer)
+- [WIP: A native macOS app](https://github.com/Sanster/lama-cleaner/discussions/314)
 - Multiple SOTA AI [models](https://lama-cleaner-docs.vercel.app/models)
   - Erase model: LaMa/LDM/ZITS/MAT/FcF/Manga
   - Erase and Replace model: Stable Diffusion/Paint by Example
 - [Plugins](https://lama-cleaner-docs.vercel.app/plugins) for post-processing:
   - [RemoveBG](https://github.com/danielgatis/rembg): Remove images background 
   - [RealESRGAN](https://github.com/xinntao/Real-ESRGAN): Super Resolution
   - [GFPGAN](https://github.com/TencentARC/GFPGAN): Face Restoration
```

#### html2text {}

```diff
@@ -4,28 +4,29 @@
    [total_download] [version] [Open_in_Colab] [Hugging_Face_Spaces] [python
                               version] [version]
 https://user-images.githubusercontent.com/3998421/196976498-ba1ad3ab-fa18-4c55-
 965f-5c6683141375.mp4 ## Sponsor
 [./assets/GitHub_Copilot_logo.svg] â¤ï¸_Your_logo
 ## Features - Completely free and open-source, fully self-hosted, support CPU &
 GPU & M1/2 - [Windows 1-Click Installer](https://lama-cleaner-docs.vercel.app/
-install/windows_1click_installer) - Multiple SOTA AI [models](https://lama-
-cleaner-docs.vercel.app/models) - Erase model: LaMa/LDM/ZITS/MAT/FcF/Manga -
-Erase and Replace model: Stable Diffusion/Paint by Example - [Plugins](https://
-lama-cleaner-docs.vercel.app/plugins) for post-processing: - [RemoveBG](https:/
-/github.com/danielgatis/rembg): Remove images background - [RealESRGAN](https:/
-/github.com/xinntao/Real-ESRGAN): Super Resolution - [GFPGAN](https://
-github.com/TencentARC/GFPGAN): Face Restoration - [RestoreFormer](https://
-github.com/wzhouxiff/RestoreFormer): Face Restoration - [Segment Anything]
-(https://lama-cleaner-docs.vercel.app/plugins#interactive-segmentation):
-Accurate and fast interactive object segmentation - More features at [lama-
-cleaner-docs](https://lama-cleaner-docs.vercel.app/) ## Quick Start Lama
-Cleaner make it easy to use SOTA AI model in just two commands: ```bash # In
-order to use the GPU, install cuda version of pytorch first. # pip install
-torch==1.13.1+cu117 torchvision==0.14.1 --extra-index-url https://
+install/windows_1click_installer) - [WIP: A native macOS app](https://
+github.com/Sanster/lama-cleaner/discussions/314) - Multiple SOTA AI [models]
+(https://lama-cleaner-docs.vercel.app/models) - Erase model: LaMa/LDM/ZITS/MAT/
+FcF/Manga - Erase and Replace model: Stable Diffusion/Paint by Example -
+[Plugins](https://lama-cleaner-docs.vercel.app/plugins) for post-processing: -
+[RemoveBG](https://github.com/danielgatis/rembg): Remove images background -
+[RealESRGAN](https://github.com/xinntao/Real-ESRGAN): Super Resolution -
+[GFPGAN](https://github.com/TencentARC/GFPGAN): Face Restoration -
+[RestoreFormer](https://github.com/wzhouxiff/RestoreFormer): Face Restoration -
+[Segment Anything](https://lama-cleaner-docs.vercel.app/plugins#interactive-
+segmentation): Accurate and fast interactive object segmentation - More
+features at [lama-cleaner-docs](https://lama-cleaner-docs.vercel.app/) ## Quick
+Start Lama Cleaner make it easy to use SOTA AI model in just two commands:
+```bash # In order to use the GPU, install cuda version of pytorch first. # pip
+install torch==1.13.1+cu117 torchvision==0.14.1 --extra-index-url https://
 download.pytorch.org/whl/cu117 pip install lama-cleaner lama-cleaner --
 model=lama --device=cpu --port=8080 ``` That's it, Lama Cleaner is now running
 at http://localhost:8080 See all command line arguments at [lama-cleaner-docs]
 (https://lama-cleaner-docs.vercel.app/install/pip) ## Development Only needed
 if you plan to modify the frontend and recompile yourself. ### Frontend
 Frontend code are modified from [cleanup.pictures](https://github.com/initml/
 cleanup.pictures), You can experience their great online services [here](https:
```

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/.DS_Store` & `lama-cleaner-1.2.1/lama_cleaner/app/build/.DS_Store`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/asset-manifest.json` & `lama-cleaner-1.2.1/lama_cleaner/app/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/favicon.ico` & `lama-cleaner-1.2.1/lama_cleaner/app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/index.html` & `lama-cleaner-1.2.1/lama_cleaner/app/build/index.html`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/css/main.ce986cc8.css` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/css/main.ce986cc8.css`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/js/main.1fda6320.js` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/js/main.1fda6320.js`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/js/main.1fda6320.js.LICENSE.txt` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/js/main.1fda6320.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-Black.15ca31c0a2a68f76d2d1.woff2` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-Black.15ca31c0a2a68f76d2d1.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-Black.c6938660eec019fefd68.woff` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-Black.c6938660eec019fefd68.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-BlackItalic.ca1e738e4f349f27514d.woff` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-BlackItalic.ca1e738e4f349f27514d.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-BlackItalic.cb2a7335650c690077fe.woff2` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-BlackItalic.cb2a7335650c690077fe.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-Bold.93c1301bd9f486c573b3.woff` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-Bold.93c1301bd9f486c573b3.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-Bold.ec64ea577b0349e055ad.woff2` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-Bold.ec64ea577b0349e055ad.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-BoldItalic.2d26c56a606662486796.woff2` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-BoldItalic.2d26c56a606662486796.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-BoldItalic.b376885042f6c961a541.woff` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-BoldItalic.b376885042f6c961a541.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-ExtraBold.cbe0ae49c52c920fd563.woff2` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-ExtraBold.cbe0ae49c52c920fd563.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-ExtraBold.d0fa3bb2b7c9063dc594.woff` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-ExtraBold.d0fa3bb2b7c9063dc594.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-ExtraBoldItalic.535a6cf662596b3bd6a6.woff2` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-ExtraBoldItalic.535a6cf662596b3bd6a6.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-ExtraBoldItalic.6ab17abedc4d3f140953.woff` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-ExtraBoldItalic.6ab17abedc4d3f140953.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-ExtraLight.72505e6a122c6acd5471.woff2` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-ExtraLight.72505e6a122c6acd5471.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-ExtraLight.c4248615291a9e8f1fb7.woff` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-ExtraLight.c4248615291a9e8f1fb7.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-ExtraLightItalic.170dddfca278d3c2ad4a.woff` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-ExtraLightItalic.170dddfca278d3c2ad4a.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-ExtraLightItalic.5c7d7d6deb1d2ec8d48c.woff2` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-ExtraLightItalic.5c7d7d6deb1d2ec8d48c.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-Italic.890025e726861dba417f.woff` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-Italic.890025e726861dba417f.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-Italic.cb10ffd7684cd9836a05.woff2` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-Italic.cb10ffd7684cd9836a05.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-Light.2d5198822ab091ce4305.woff2` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-Light.2d5198822ab091ce4305.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-Light.994e34451cc19ede31d3.woff` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-Light.994e34451cc19ede31d3.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-LightItalic.ef9f65d91d2b0ba9b2e4.woff` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-LightItalic.ef9f65d91d2b0ba9b2e4.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-LightItalic.f86952265d7b0f02c921.woff2` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-LightItalic.f86952265d7b0f02c921.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-Medium.293fd13dbca5a3e450ef.woff2` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-Medium.293fd13dbca5a3e450ef.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-Medium.9053572c46aeb4b16caa.woff` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-Medium.9053572c46aeb4b16caa.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-MediumItalic.085cb93e613ba3d40d2b.woff2` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-MediumItalic.085cb93e613ba3d40d2b.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-MediumItalic.3d0107dd43d0101274d3.woff` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-MediumItalic.3d0107dd43d0101274d3.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-Regular.8c206db99195777c6769.woff` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-Regular.8c206db99195777c6769.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-Regular.c8ba52b05a9ef10f4758.woff2` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-Regular.c8ba52b05a9ef10f4758.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-SemiBold.b5f0f109bc88052d4000.woff2` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-SemiBold.b5f0f109bc88052d4000.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-SemiBold.cca62d21c8c555c392e5.woff` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-SemiBold.cca62d21c8c555c392e5.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-SemiBoldItalic.463bdbfb28abad0fa6df.woff` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-SemiBoldItalic.463bdbfb28abad0fa6df.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-SemiBoldItalic.d9467ee321a8f38aefff.woff2` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-SemiBoldItalic.d9467ee321a8f38aefff.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-Thin.29b9c616a95a912abf73.woff` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-Thin.29b9c616a95a912abf73.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-Thin.fff2a096db014f6239d4.woff2` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-Thin.fff2a096db014f6239d4.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-ThinItalic.bae95eb2f889c797e435.woff` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-ThinItalic.bae95eb2f889c797e435.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-ThinItalic.bf213704dce6b437ede4.woff2` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-ThinItalic.bf213704dce6b437ede4.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-italic.var.30807be7abc48ba8c73c.woff2` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-italic.var.30807be7abc48ba8c73c.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter-roman.var.ba4caefcdf5b36b438db.woff2` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter-roman.var.ba4caefcdf5b36b438db.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/Inter.var.c2fe3cb2b7c746f7966a.woff2` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/Inter.var.c2fe3cb2b7c746f7966a.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/app/build/static/media/coffee-machine-lineal.ee32631219cc3986f861.gif` & `lama-cleaner-1.2.1/lama_cleaner/app/build/static/media/coffee-machine-lineal.ee32631219cc3986f861.gif`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/benchmark.py` & `lama-cleaner-1.2.1/lama_cleaner/benchmark.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/const.py` & `lama-cleaner-1.2.1/lama_cleaner/const.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/file_manager/file_manager.py` & `lama-cleaner-1.2.1/lama_cleaner/file_manager/file_manager.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/file_manager/storage_backends.py` & `lama-cleaner-1.2.1/lama_cleaner/file_manager/storage_backends.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/file_manager/utils.py` & `lama-cleaner-1.2.1/lama_cleaner/file_manager/utils.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/helper.py` & `lama-cleaner-1.2.1/lama_cleaner/helper.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/model/base.py` & `lama-cleaner-1.2.1/lama_cleaner/model/base.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/model/controlnet.py` & `lama-cleaner-1.2.1/lama_cleaner/model/controlnet.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/model/ddim_sampler.py` & `lama-cleaner-1.2.1/lama_cleaner/model/ddim_sampler.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/model/fcf.py` & `lama-cleaner-1.2.1/lama_cleaner/model/fcf.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/model/instruct_pix2pix.py` & `lama-cleaner-1.2.1/lama_cleaner/model/instruct_pix2pix.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/model/lama.py` & `lama-cleaner-1.2.1/lama_cleaner/model/lama.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/model/ldm.py` & `lama-cleaner-1.2.1/lama_cleaner/model/ldm.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/model/manga.py` & `lama-cleaner-1.2.1/lama_cleaner/model/manga.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/model/mat.py` & `lama-cleaner-1.2.1/lama_cleaner/model/mat.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/model/opencv2.py` & `lama-cleaner-1.2.1/lama_cleaner/model/opencv2.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/model/paint_by_example.py` & `lama-cleaner-1.2.1/lama_cleaner/model/paint_by_example.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/model/pipeline/pipeline_stable_diffusion_controlnet_inpaint.py` & `lama-cleaner-1.2.1/lama_cleaner/model/pipeline/pipeline_stable_diffusion_controlnet_inpaint.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/model/plms_sampler.py` & `lama-cleaner-1.2.1/lama_cleaner/model/plms_sampler.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/model/sd.py` & `lama-cleaner-1.2.1/lama_cleaner/model/sd.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/model/utils.py` & `lama-cleaner-1.2.1/lama_cleaner/model/utils.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/model/zits.py` & `lama-cleaner-1.2.1/lama_cleaner/model/zits.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/model_manager.py` & `lama-cleaner-1.2.1/lama_cleaner/model_manager.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/parse_args.py` & `lama-cleaner-1.2.1/lama_cleaner/parse_args.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/plugins/anime_seg.py` & `lama-cleaner-1.2.1/lama_cleaner/plugins/anime_seg.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/plugins/gfpgan_plugin.py` & `lama-cleaner-1.2.1/lama_cleaner/plugins/gfpgan_plugin.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/plugins/gfpganer.py` & `lama-cleaner-1.2.1/lama_cleaner/plugins/gfpganer.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/plugins/gif.py` & `lama-cleaner-1.2.1/lama_cleaner/plugins/gif.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/plugins/interactive_seg.py` & `lama-cleaner-1.2.1/lama_cleaner/plugins/interactive_seg.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/plugins/realesrgan.py` & `lama-cleaner-1.2.1/lama_cleaner/plugins/realesrgan.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/plugins/remove_bg.py` & `lama-cleaner-1.2.1/lama_cleaner/plugins/remove_bg.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/plugins/restoreformer.py` & `lama-cleaner-1.2.1/lama_cleaner/plugins/restoreformer.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/plugins/segment_anything/build_sam.py` & `lama-cleaner-1.2.1/lama_cleaner/plugins/segment_anything/build_sam.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/plugins/segment_anything/modeling/common.py` & `lama-cleaner-1.2.1/lama_cleaner/plugins/segment_anything/modeling/common.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/plugins/segment_anything/modeling/image_encoder.py` & `lama-cleaner-1.2.1/lama_cleaner/plugins/segment_anything/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/plugins/segment_anything/modeling/mask_decoder.py` & `lama-cleaner-1.2.1/lama_cleaner/plugins/segment_anything/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/plugins/segment_anything/modeling/prompt_encoder.py` & `lama-cleaner-1.2.1/lama_cleaner/plugins/segment_anything/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/plugins/segment_anything/modeling/sam.py` & `lama-cleaner-1.2.1/lama_cleaner/plugins/segment_anything/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/plugins/segment_anything/modeling/transformer.py` & `lama-cleaner-1.2.1/lama_cleaner/plugins/segment_anything/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/plugins/segment_anything/predictor.py` & `lama-cleaner-1.2.1/lama_cleaner/plugins/segment_anything/predictor.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/plugins/segment_anything/utils/transforms.py` & `lama-cleaner-1.2.1/lama_cleaner/plugins/segment_anything/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/runtime.py` & `lama-cleaner-1.2.1/lama_cleaner/runtime.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/schema.py` & `lama-cleaner-1.2.1/lama_cleaner/schema.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/server.py` & `lama-cleaner-1.2.1/lama_cleaner/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,19 +134,28 @@
     if output_dir is None:
         return "--output-dir is None", 500
 
     input = request.files
     filename = request.form["filename"]
     origin_image_bytes = input["image"].read()  # RGB
     ext = get_image_ext(origin_image_bytes)
-    image, _, exif_infos = load_img(origin_image_bytes, return_exif=True)
+    image, alpha_channel, exif_infos = load_img(origin_image_bytes, return_exif=True)
     save_path = os.path.join(output_dir, filename)
 
+    if alpha_channel is not None:
+        if alpha_channel.shape[:2] != image.shape[:2]:
+            alpha_channel = cv2.resize(
+                alpha_channel, dsize=(image.shape[1], image.shape[0])
+            )
+        image = np.concatenate((image, alpha_channel[:, :, np.newaxis]), axis=-1)
+
+    pil_image = Image.fromarray(image)
+
     img_bytes = pil_to_bytes(
-        Image.fromarray(image),
+        pil_image,
         ext,
         quality=image_quality,
         exif_infos=exif_infos,
     )
     with open(save_path, "wb") as fw:
         fw.write(img_bytes)
```

### Comparing `lama-cleaner-1.2.0/lama_cleaner/tests/test_controlnet.py` & `lama-cleaner-1.2.1/lama_cleaner/tests/test_controlnet.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/tests/test_instruct_pix2pix.py` & `lama-cleaner-1.2.1/lama_cleaner/tests/test_instruct_pix2pix.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/tests/test_load_img.py` & `lama-cleaner-1.2.1/lama_cleaner/tests/test_load_img.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/tests/test_model.py` & `lama-cleaner-1.2.1/lama_cleaner/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/tests/test_model_md5.py` & `lama-cleaner-1.2.1/lama_cleaner/tests/test_model_md5.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/tests/test_paint_by_example.py` & `lama-cleaner-1.2.1/lama_cleaner/tests/test_paint_by_example.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/tests/test_plugins.py` & `lama-cleaner-1.2.1/lama_cleaner/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/tests/test_save_exif.py` & `lama-cleaner-1.2.1/lama_cleaner/tests/test_save_exif.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/tests/test_sd_model.py` & `lama-cleaner-1.2.1/lama_cleaner/tests/test_sd_model.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner/web_config.py` & `lama-cleaner-1.2.1/lama_cleaner/web_config.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/lama_cleaner.egg-info/PKG-INFO` & `lama-cleaner-1.2.1/lama_cleaner.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,108 +1,108 @@
 Metadata-Version: 2.1
 Name: lama-cleaner
-Version: 1.2.0
+Version: 1.2.1
 Summary: Image inpainting tool powered by SOTA AI Model
 Home-page: https://github.com/Sanster/lama-cleaner
 Author: PanicByte
 Author-email: cwq1913@gmail.com
-License: UNKNOWN
-Description: <p align="center">
-           <img alt="logo" height=256 src="./assets/logo.png" />
-        </p>
-        <h1 align="center">Lama Cleaner</h1>
-        <p align="center">A free and open-source inpainting tool powered by SOTA AI model.</p>
-        
-        <p align="center">
-          <a href="https://github.com/Sanster/lama-cleaner">
-            <img alt="total download" src="https://pepy.tech/badge/lama-cleaner" />
-          </a>
-          <a href="https://pypi.org/project/lama-cleaner/">
-            <img alt="version" src="https://img.shields.io/pypi/v/lama-cleaner" />
-          </a>
-          <a href="https://colab.research.google.com/drive/1e3ZkAJxvkK3uzaTGu91N9TvI_Mahs0Wb?usp=sharing">
-            <img alt="Open in Colab" src="https://colab.research.google.com/assets/colab-badge.svg" />
-          </a>
-        
-          <a href="https://huggingface.co/spaces/Sanster/Lama-Cleaner-lama">
-            <img alt="Hugging Face Spaces" src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue" />
-          </a>
-        
-          <a href="">
-            <img alt="python version" src="https://img.shields.io/pypi/pyversions/lama-cleaner" />
-          </a>
-          <a href="https://hub.docker.com/r/cwq1913/lama-cleaner">
-            <img alt="version" src="https://img.shields.io/docker/pulls/cwq1913/lama-cleaner" />
-          </a>
-        </p>
-        
-        https://user-images.githubusercontent.com/3998421/196976498-ba1ad3ab-fa18-4c55-965f-5c6683141375.mp4
-        
-        ## Sponsor
-        
-        <table>
-           <tr>
-            <td >
-                <img src="./assets/GitHub_Copilot_logo.svg" style="background: white;padding: 8px;"/>
-            </td>
-            <td >
-              <a href="https://ko-fi.com/Z8Z1CZJGY/tiers" target="_blank" >
-                ❤️ Your logo
-              </a>
-            </td>
-          </tr>
-        </table>
-        
-        ## Features
-        
-        - Completely free and open-source, fully self-hosted, support CPU & GPU & M1/2
-        - [Windows 1-Click Installer](https://lama-cleaner-docs.vercel.app/install/windows_1click_installer)
-        - Multiple SOTA AI [models](https://lama-cleaner-docs.vercel.app/models)
-          - Erase model: LaMa/LDM/ZITS/MAT/FcF/Manga
-          - Erase and Replace model: Stable Diffusion/Paint by Example
-        - [Plugins](https://lama-cleaner-docs.vercel.app/plugins) for post-processing:
-          - [RemoveBG](https://github.com/danielgatis/rembg): Remove images background 
-          - [RealESRGAN](https://github.com/xinntao/Real-ESRGAN): Super Resolution
-          - [GFPGAN](https://github.com/TencentARC/GFPGAN): Face Restoration
-          - [RestoreFormer](https://github.com/wzhouxiff/RestoreFormer): Face Restoration
-          - [Segment Anything](https://lama-cleaner-docs.vercel.app/plugins#interactive-segmentation): Accurate and fast interactive object segmentation
-        - More features at [lama-cleaner-docs](https://lama-cleaner-docs.vercel.app/)
-        
-        ## Quick Start
-        
-        Lama Cleaner make it easy to use SOTA AI model in just two commands:
-        
-        ```bash
-        # In order to use the GPU, install cuda version of pytorch first.
-        # pip install torch==1.13.1+cu117 torchvision==0.14.1 --extra-index-url https://download.pytorch.org/whl/cu117
-        pip install lama-cleaner
-        lama-cleaner --model=lama --device=cpu --port=8080
-        ```
-        
-        That's it, Lama Cleaner is now running at http://localhost:8080
-        
-        See all command line arguments at [lama-cleaner-docs](https://lama-cleaner-docs.vercel.app/install/pip)
-        
-        ## Development
-        
-        Only needed if you plan to modify the frontend and recompile yourself.
-        
-        ### Frontend
-        
-        Frontend code are modified from [cleanup.pictures](https://github.com/initml/cleanup.pictures), You can experience their
-        great online services [here](https://cleanup.pictures/).
-        
-        - Install dependencies:`cd lama_cleaner/app/ && pnpm install`
-        - Start development server: `pnpm start`
-        - Build: `pnpm build`
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center">
+   <img alt="logo" height=256 src="./assets/logo.png" />
+</p>
+<h1 align="center">Lama Cleaner</h1>
+<p align="center">A free and open-source inpainting tool powered by SOTA AI model.</p>
+
+<p align="center">
+  <a href="https://github.com/Sanster/lama-cleaner">
+    <img alt="total download" src="https://pepy.tech/badge/lama-cleaner" />
+  </a>
+  <a href="https://pypi.org/project/lama-cleaner/">
+    <img alt="version" src="https://img.shields.io/pypi/v/lama-cleaner" />
+  </a>
+  <a href="https://colab.research.google.com/drive/1e3ZkAJxvkK3uzaTGu91N9TvI_Mahs0Wb?usp=sharing">
+    <img alt="Open in Colab" src="https://colab.research.google.com/assets/colab-badge.svg" />
+  </a>
+
+  <a href="https://huggingface.co/spaces/Sanster/Lama-Cleaner-lama">
+    <img alt="Hugging Face Spaces" src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue" />
+  </a>
+
+  <a href="">
+    <img alt="python version" src="https://img.shields.io/pypi/pyversions/lama-cleaner" />
+  </a>
+  <a href="https://hub.docker.com/r/cwq1913/lama-cleaner">
+    <img alt="version" src="https://img.shields.io/docker/pulls/cwq1913/lama-cleaner" />
+  </a>
+</p>
+
+https://user-images.githubusercontent.com/3998421/196976498-ba1ad3ab-fa18-4c55-965f-5c6683141375.mp4
+
+## Sponsor
+
+<table>
+   <tr>
+    <td >
+        <img src="./assets/GitHub_Copilot_logo.svg" style="background: white;padding: 8px;"/>
+    </td>
+    <td >
+      <a href="https://ko-fi.com/Z8Z1CZJGY/tiers" target="_blank" >
+        ❤️ Your logo
+      </a>
+    </td>
+  </tr>
+</table>
+
+## Features
+
+- Completely free and open-source, fully self-hosted, support CPU & GPU & M1/2
+- [Windows 1-Click Installer](https://lama-cleaner-docs.vercel.app/install/windows_1click_installer)
+- [WIP: A native macOS app](https://github.com/Sanster/lama-cleaner/discussions/314)
+- Multiple SOTA AI [models](https://lama-cleaner-docs.vercel.app/models)
+  - Erase model: LaMa/LDM/ZITS/MAT/FcF/Manga
+  - Erase and Replace model: Stable Diffusion/Paint by Example
+- [Plugins](https://lama-cleaner-docs.vercel.app/plugins) for post-processing:
+  - [RemoveBG](https://github.com/danielgatis/rembg): Remove images background 
+  - [RealESRGAN](https://github.com/xinntao/Real-ESRGAN): Super Resolution
+  - [GFPGAN](https://github.com/TencentARC/GFPGAN): Face Restoration
+  - [RestoreFormer](https://github.com/wzhouxiff/RestoreFormer): Face Restoration
+  - [Segment Anything](https://lama-cleaner-docs.vercel.app/plugins#interactive-segmentation): Accurate and fast interactive object segmentation
+- More features at [lama-cleaner-docs](https://lama-cleaner-docs.vercel.app/)
+
+## Quick Start
+
+Lama Cleaner make it easy to use SOTA AI model in just two commands:
+
+```bash
+# In order to use the GPU, install cuda version of pytorch first.
+# pip install torch==1.13.1+cu117 torchvision==0.14.1 --extra-index-url https://download.pytorch.org/whl/cu117
+pip install lama-cleaner
+lama-cleaner --model=lama --device=cpu --port=8080
+```
+
+That's it, Lama Cleaner is now running at http://localhost:8080
+
+See all command line arguments at [lama-cleaner-docs](https://lama-cleaner-docs.vercel.app/install/pip)
+
+## Development
+
+Only needed if you plan to modify the frontend and recompile yourself.
+
+### Frontend
+
+Frontend code are modified from [cleanup.pictures](https://github.com/initml/cleanup.pictures), You can experience their
+great online services [here](https://cleanup.pictures/).
+
+- Install dependencies:`cd lama_cleaner/app/ && pnpm install`
+- Start development server: `pnpm start`
+- Build: `pnpm build`
```

#### html2text {}

```diff
@@ -1,44 +1,44 @@
-Metadata-Version: 2.1 Name: lama-cleaner Version: 1.2.0 Summary: Image
+Metadata-Version: 2.1 Name: lama-cleaner Version: 1.2.1 Summary: Image
 inpainting tool powered by SOTA AI Model Home-page: https://github.com/Sanster/
-lama-cleaner Author: PanicByte Author-email: cwq1913@gmail.com License: UNKNOWN
-Description:
+lama-cleaner Author: PanicByte Author-email: cwq1913@gmail.com Classifier:
+License :: OSI Approved :: Apache Software License Classifier: Operating System
+:: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Topic :: Scientific/
+Engineering :: Artificial Intelligence Requires-Python: >=3.7 Description-
+Content-Type: text/markdown License-File: LICENSE
                                     [logo]
                           ****** Lama Cleaner ******
        A free and open-source inpainting tool powered by SOTA AI model.
    [total_download] [version] [Open_in_Colab] [Hugging_Face_Spaces] [python
                               version] [version]
 https://user-images.githubusercontent.com/3998421/196976498-ba1ad3ab-fa18-4c55-
 965f-5c6683141375.mp4 ## Sponsor
 [./assets/GitHub_Copilot_logo.svg] â¤ï¸_Your_logo
 ## Features - Completely free and open-source, fully self-hosted, support CPU &
 GPU & M1/2 - [Windows 1-Click Installer](https://lama-cleaner-docs.vercel.app/
-install/windows_1click_installer) - Multiple SOTA AI [models](https://lama-
-cleaner-docs.vercel.app/models) - Erase model: LaMa/LDM/ZITS/MAT/FcF/Manga -
-Erase and Replace model: Stable Diffusion/Paint by Example - [Plugins](https://
-lama-cleaner-docs.vercel.app/plugins) for post-processing: - [RemoveBG](https:/
-/github.com/danielgatis/rembg): Remove images background - [RealESRGAN](https:/
-/github.com/xinntao/Real-ESRGAN): Super Resolution - [GFPGAN](https://
-github.com/TencentARC/GFPGAN): Face Restoration - [RestoreFormer](https://
-github.com/wzhouxiff/RestoreFormer): Face Restoration - [Segment Anything]
-(https://lama-cleaner-docs.vercel.app/plugins#interactive-segmentation):
-Accurate and fast interactive object segmentation - More features at [lama-
-cleaner-docs](https://lama-cleaner-docs.vercel.app/) ## Quick Start Lama
-Cleaner make it easy to use SOTA AI model in just two commands: ```bash # In
-order to use the GPU, install cuda version of pytorch first. # pip install
-torch==1.13.1+cu117 torchvision==0.14.1 --extra-index-url https://
+install/windows_1click_installer) - [WIP: A native macOS app](https://
+github.com/Sanster/lama-cleaner/discussions/314) - Multiple SOTA AI [models]
+(https://lama-cleaner-docs.vercel.app/models) - Erase model: LaMa/LDM/ZITS/MAT/
+FcF/Manga - Erase and Replace model: Stable Diffusion/Paint by Example -
+[Plugins](https://lama-cleaner-docs.vercel.app/plugins) for post-processing: -
+[RemoveBG](https://github.com/danielgatis/rembg): Remove images background -
+[RealESRGAN](https://github.com/xinntao/Real-ESRGAN): Super Resolution -
+[GFPGAN](https://github.com/TencentARC/GFPGAN): Face Restoration -
+[RestoreFormer](https://github.com/wzhouxiff/RestoreFormer): Face Restoration -
+[Segment Anything](https://lama-cleaner-docs.vercel.app/plugins#interactive-
+segmentation): Accurate and fast interactive object segmentation - More
+features at [lama-cleaner-docs](https://lama-cleaner-docs.vercel.app/) ## Quick
+Start Lama Cleaner make it easy to use SOTA AI model in just two commands:
+```bash # In order to use the GPU, install cuda version of pytorch first. # pip
+install torch==1.13.1+cu117 torchvision==0.14.1 --extra-index-url https://
 download.pytorch.org/whl/cu117 pip install lama-cleaner lama-cleaner --
 model=lama --device=cpu --port=8080 ``` That's it, Lama Cleaner is now running
 at http://localhost:8080 See all command line arguments at [lama-cleaner-docs]
 (https://lama-cleaner-docs.vercel.app/install/pip) ## Development Only needed
 if you plan to modify the frontend and recompile yourself. ### Frontend
 Frontend code are modified from [cleanup.pictures](https://github.com/initml/
 cleanup.pictures), You can experience their great online services [here](https:
 //cleanup.pictures/). - Install dependencies:`cd lama_cleaner/app/ && pnpm
 install` - Start development server: `pnpm start` - Build: `pnpm build`
-Platform: UNKNOWN Classifier: License :: OSI Approved :: Apache Software
-License Classifier: Operating System :: OS Independent Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `lama-cleaner-1.2.0/lama_cleaner.egg-info/SOURCES.txt` & `lama-cleaner-1.2.1/lama_cleaner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.0/setup.py` & `lama-cleaner-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
                 requires.append(line.strip())
     return requires
 
 
 # https://setuptools.readthedocs.io/en/latest/setuptools.html#including-data-files
 setuptools.setup(
     name="lama-cleaner",
-    version="1.2.0",
+    version="1.2.1",
     author="PanicByte",
     author_email="cwq1913@gmail.com",
     description="Image inpainting tool powered by SOTA AI Model",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Sanster/lama-cleaner",
     packages=setuptools.find_packages("./"),
```

