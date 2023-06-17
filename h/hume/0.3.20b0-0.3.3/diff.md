# Comparing `tmp/hume-0.3.20b0.tar.gz` & `tmp/hume-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hume-0.3.20b0.tar", last modified: Sat Jun  1 23:14:25 2019, max compression
+gzip compressed data, was "hume-0.3.3.tar", max compression
```

## Comparing `hume-0.3.20b0.tar` & `hume-0.3.3.tar`

### file list

```diff
@@ -1,8 +1,33 @@
--rw-r--r--   0        0        0     1067 2019-05-28 18:43:24.499597 hume-0.3.20b0/LICENSE
--rw-r--r--   0        0        0     3712 2019-05-30 17:08:33.892698 hume-0.3.20b0/README.md
--rw-r--r--   0        0        0    72163 2019-05-28 18:24:11.503000 hume-0.3.20b0/docs/console_demo.png
--rw-r--r--   0        0        0       25 2019-05-28 11:29:38.076584 hume-0.3.20b0/hume/decorators/__init__.py
--rw-r--r--   0        0        0     4764 2019-05-29 22:06:28.379043 hume-0.3.20b0/hume/decorators/profilers.py
--rw-r--r--   0        0        0     1109 2019-06-01 23:12:11.740831 hume-0.3.20b0/pyproject.toml
--rw-r--r--   0        0        0     4445 1970-01-01 00:00:00.000000 hume-0.3.20b0/setup.py
--rw-r--r--   0        0        0     4642 1970-01-01 00:00:00.000000 hume-0.3.20b0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-24 18:35:19.356412 hume-0.3.3/LICENSE
+-rw-r--r--   0        0        0     2303 2023-05-05 00:20:11.927638 hume-0.3.3/README.md
+-rw-r--r--   0        0        0      567 2023-05-03 18:27:10.048390 hume-0.3.3/hume/__init__.py
+-rw-r--r--   0        0        0      500 2023-05-03 18:27:10.048676 hume-0.3.3/hume/_batch/__init__.py
+-rw-r--r--   0        0        0     3464 2023-05-03 20:14:45.408723 hume-0.3.3/hume/_batch/batch_job.py
+-rw-r--r--   0        0        0     5800 2023-05-03 20:20:07.806749 hume-0.3.3/hume/_batch/batch_job_details.py
+-rw-r--r--   0        0        0      630 2023-05-03 20:19:40.816995 hume-0.3.3/hume/_batch/batch_job_state.py
+-rw-r--r--   0        0        0      993 2023-05-01 17:29:24.001284 hume-0.3.3/hume/_batch/batch_job_status.py
+-rw-r--r--   0        0        0     9282 2023-06-17 07:43:05.282946 hume-0.3.3/hume/_batch/hume_batch_client.py
+-rw-r--r--   0        0        0      939 2023-05-03 21:06:47.512368 hume-0.3.3/hume/_batch/transcription_config.py
+-rw-r--r--   0        0        0       19 2022-10-05 20:58:45.000000 hume-0.3.3/hume/_common/__init__.py
+-rw-r--r--   0        0        0      124 2023-04-24 18:35:19.357658 hume-0.3.3/hume/_common/api_type.py
+-rw-r--r--   0        0        0     1459 2023-05-02 20:54:26.057155 hume-0.3.3/hume/_common/client_base.py
+-rw-r--r--   0        0        0     1795 2023-05-02 20:54:26.057667 hume-0.3.3/hume/_common/config_base.py
+-rw-r--r--   0        0        0     2320 2023-05-02 00:14:43.888549 hume-0.3.3/hume/_common/config_utils.py
+-rw-r--r--   0        0        0     3227 2023-06-11 17:16:41.157744 hume-0.3.3/hume/_common/retry_utils.py
+-rw-r--r--   0        0        0      191 2023-04-24 18:35:19.358014 hume-0.3.3/hume/_stream/__init__.py
+-rw-r--r--   0        0        0     3908 2023-06-09 21:16:30.099495 hume-0.3.3/hume/_stream/hume_stream_client.py
+-rw-r--r--   0        0        0     8132 2023-06-09 21:16:30.099662 hume-0.3.3/hume/_stream/stream_socket.py
+-rw-r--r--   0        0        0       19 2023-04-24 18:35:19.358285 hume-0.3.3/hume/error/__init__.py
+-rw-r--r--   0        0        0      571 2023-04-24 18:35:19.358345 hume-0.3.3/hume/error/hume_client_exception.py
+-rw-r--r--   0        0        0       96 2023-04-24 18:35:19.358433 hume-0.3.3/hume/models/__init__.py
+-rw-r--r--   0        0        0      587 2023-04-24 18:35:19.358535 hume-0.3.3/hume/models/config/__init__.py
+-rw-r--r--   0        0        0      497 2023-04-24 18:35:19.358607 hume-0.3.3/hume/models/config/burst_config.py
+-rw-r--r--   0        0        0     2777 2023-05-03 20:19:40.817539 hume-0.3.3/hume/models/config/face_config.py
+-rw-r--r--   0        0        0      509 2023-05-05 00:20:11.928431 hume-0.3.3/hume/models/config/facemesh_config.py
+-rw-r--r--   0        0        0     2235 2023-05-04 23:18:49.287324 hume-0.3.3/hume/models/config/language_config.py
+-rw-r--r--   0        0        0      631 2023-05-02 20:54:26.059076 hume-0.3.3/hume/models/config/model_config_base.py
+-rw-r--r--   0        0        0     1000 2023-05-03 20:19:40.817946 hume-0.3.3/hume/models/config/ner_config.py
+-rw-r--r--   0        0        0     1785 2023-06-09 21:21:24.616184 hume-0.3.3/hume/models/config/prosody_config.py
+-rw-r--r--   0        0        0      804 2023-04-24 18:35:19.359005 hume-0.3.3/hume/models/model_type.py
+-rw-r--r--   0        0        0     2527 2023-06-17 07:43:05.283295 hume-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     3558 1970-01-01 00:00:00.000000 hume-0.3.3/PKG-INFO
```

### Comparing `hume-0.3.20b0/LICENSE` & `hume-0.3.3/LICENSE`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2018 Real Python
+Copyright (c) 2022 Hume AI, Inc.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

