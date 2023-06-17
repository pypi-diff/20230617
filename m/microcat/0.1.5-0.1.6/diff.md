# Comparing `tmp/microcat-0.1.5.tar.gz` & `tmp/microcat-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microcat-0.1.5.tar", last modified: Wed Jun 14 02:39:30 2023, max compression
+gzip compressed data, was "microcat-0.1.6.tar", last modified: Sat Jun 17 14:38:34 2023, max compression
```

## Comparing `microcat-0.1.5.tar` & `microcat-0.1.6.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:39:30.557833 microcat-0.1.5/
--rw-r--r--   0 root         (0) root         (0)    34599 2023-06-09 02:02:59.000000 microcat-0.1.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      396 2023-06-09 03:45:47.000000 microcat-0.1.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1298 2023-06-14 02:39:30.557833 microcat-0.1.5/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      383 2023-05-18 11:49:26.000000 microcat-0.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:39:30.549833 microcat-0.1.5/microcat/
--rwxrwxr-x   0 root         (0) root         (0)       73 2023-06-14 02:37:50.000000 microcat-0.1.5/microcat/__about__.py
--rwxrwxr-x   0 root         (0) root         (0)      911 2023-06-09 03:13:23.000000 microcat-0.1.5/microcat/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:39:30.553833 microcat-0.1.5/microcat/config/
--rw-r--r--   0 root         (0) root         (0)     2655 2023-06-08 02:42:59.000000 microcat-0.1.5/microcat/config/config.yaml
--rwxr-xr-x   0 root         (0) root         (0)     8766 2023-06-09 03:49:23.000000 microcat-0.1.5/microcat/configer.py
--rwxr-xr-x   0 root         (0) root         (0)    18610 2023-06-14 02:37:44.000000 microcat-0.1.5/microcat/corer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:39:30.553833 microcat-0.1.5/microcat/envs/
--rw-r--r--   0 root         (0) root         (0)      153 2023-06-14 02:38:16.000000 microcat-0.1.5/microcat/envs/kmer_python.yaml
--rw-r--r--   0 root         (0) root         (0)      390 2023-06-14 02:38:08.000000 microcat-0.1.5/microcat/envs/kmer_qc.yaml
--rw-rw-r--   0 root         (0) root         (0)      164 2023-06-14 02:38:19.000000 microcat-0.1.5/microcat/envs/kraken2.yaml
--rw-r--r--   0 root         (0) root         (0)      133 2023-05-31 02:41:36.000000 microcat-0.1.5/microcat/envs/krakenuniq.yaml
--rw-r--r--   0 root         (0) root         (0)      109 2023-06-03 12:24:08.000000 microcat-0.1.5/microcat/envs/metaphlan.yaml
--rwxr-xr-x   0 root         (0) root         (0)      145 2023-06-03 12:24:08.000000 microcat-0.1.5/microcat/envs/pathseq.yaml
--rw-r--r--   0 root         (0) root         (0)      100 2023-06-07 06:24:12.000000 microcat-0.1.5/microcat/envs/star.yaml
--rw-r--r--   0 root         (0) root         (0)      140 2023-05-31 02:41:36.000000 microcat-0.1.5/microcat/envs/trimming.yaml
--rw-r--r--   0 root         (0) root         (0)     3558 2023-06-10 01:56:12.000000 microcat-0.1.5/microcat/prepare.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:39:30.549833 microcat-0.1.5/microcat/profiles/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:39:30.553833 microcat-0.1.5/microcat/profiles/lsf/
--rw-r--r--   0 root         (0) root         (0)      955 2023-06-14 02:37:56.000000 microcat-0.1.5/microcat/profiles/lsf/CookieCutter.py
--rw-r--r--   0 root         (0) root         (0)     2242 2023-06-03 12:24:08.000000 microcat-0.1.5/microcat/profiles/lsf/OSLayer.py
--rw-r--r--   0 root         (0) root         (0)      297 2023-06-03 12:24:08.000000 microcat-0.1.5/microcat/profiles/lsf/config.yaml
--rwxr-xr-x   0 root         (0) root         (0)     1124 2023-06-03 12:24:08.000000 microcat-0.1.5/microcat/profiles/lsf/lsf_cancel.py
--rw-r--r--   0 root         (0) root         (0)     1978 2023-06-03 12:24:08.000000 microcat-0.1.5/microcat/profiles/lsf/lsf_config.py
--rwxr-xr-x   0 root         (0) root         (0)       48 2023-06-03 12:24:08.000000 microcat-0.1.5/microcat/profiles/lsf/lsf_jobscript.sh
--rwxr-xr-x   0 root         (0) root         (0)     7511 2023-06-03 12:24:08.000000 microcat-0.1.5/microcat/profiles/lsf/lsf_status.py
--rwxr-xr-x   0 root         (0) root         (0)     8281 2023-06-03 12:24:08.000000 microcat-0.1.5/microcat/profiles/lsf/lsf_submit.py
--rw-r--r--   0 root         (0) root         (0)     3775 2023-06-03 12:24:08.000000 microcat-0.1.5/microcat/profiles/lsf/memory_units.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:39:30.557833 microcat-0.1.5/microcat/rules/
--rw-r--r--   0 root         (0) root         (0)     1107 2023-06-09 02:29:19.000000 microcat-0.1.5/microcat/rules/ERCC.smk
--rw-r--r--   0 root         (0) root         (0)     2225 2023-06-10 01:41:24.000000 microcat-0.1.5/microcat/rules/build.smk
--rw-r--r--   0 root         (0) root         (0)    40814 2023-06-09 02:28:56.000000 microcat-0.1.5/microcat/rules/classfier.smk
--rw-r--r--   0 root         (0) root         (0)     3981 2023-06-07 01:22:00.000000 microcat-0.1.5/microcat/rules/database.smk
--rw-r--r--   0 root         (0) root         (0)    42271 2023-06-14 02:39:14.000000 microcat-0.1.5/microcat/rules/host.smk
--rwxr-xr-x   0 root         (0) root         (0)    10460 2023-06-05 09:08:14.000000 microcat-0.1.5/microcat/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:39:30.557833 microcat-0.1.5/microcat/scripts/
--rw-r--r--   0 root         (0) root         (0)    15479 2023-06-08 03:30:56.000000 microcat-0.1.5/microcat/scripts/INVADEseq.py
--rwxrwxrwx   0 root         (0) root         (0)    19072 2023-06-07 07:14:07.000000 microcat-0.1.5/microcat/scripts/extract_kraken_reads.py
--rwxrwxrwx   0 root         (0) root         (0)     3849 2023-06-07 07:14:23.000000 microcat-0.1.5/microcat/scripts/extract_microbiome_output.R
--rwxr-xr-x   0 root         (0) root         (0)     7896 2023-06-03 12:24:08.000000 microcat-0.1.5/microcat/scripts/get_ncbi_domains.py
--rw-r--r--   0 root         (0) root         (0)     1185 2023-06-07 07:15:11.000000 microcat-0.1.5/microcat/scripts/krak2_output_denosing.R
--rwxr-xr-x   0 root         (0) root         (0)     6942 2023-06-07 07:15:43.000000 microcat-0.1.5/microcat/scripts/kraken2mpa.py
--rwxr-xr-x   0 root         (0) root         (0)    14784 2023-06-07 07:15:24.000000 microcat-0.1.5/microcat/scripts/kraken2sc.py
--rw-r--r--   0 root         (0) root         (0)     4698 2023-06-07 07:14:59.000000 microcat-0.1.5/microcat/scripts/sample_denosing.R
--rwxrwxrwx   0 root         (0) root         (0)    15665 2023-06-07 07:13:48.000000 microcat-0.1.5/microcat/scripts/sckmer_unpaired.R
--rwxr-xr-x   0 root         (0) root         (0)     2367 2023-06-03 12:24:08.000000 microcat-0.1.5/microcat/scripts/spilt_bam_by_tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:39:30.557833 microcat-0.1.5/microcat/snakefiles/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:37:58.000000 microcat-0.1.5/microcat/snakefiles/bulk_wf.smk
--rw-r--r--   0 root         (0) root         (0)     1832 2023-06-09 04:28:17.000000 microcat-0.1.5/microcat/snakefiles/scRNA_wf.smk
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:38:06.000000 microcat-0.1.5/microcat/snakefiles/spatial_wf.smk
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:39:30.553833 microcat-0.1.5/microcat.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1298 2023-06-14 02:39:30.000000 microcat-0.1.5/microcat.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1539 2023-06-14 02:39:30.000000 microcat-0.1.5/microcat.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 02:39:30.000000 microcat-0.1.5/microcat.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-06-14 02:39:30.000000 microcat-0.1.5/microcat.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 02:39:30.000000 microcat-0.1.5/microcat.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-14 02:39:30.000000 microcat-0.1.5/microcat.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-06-09 01:50:10.000000 microcat-0.1.5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 02:39:30.557833 microcat-0.1.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2273 2023-06-09 03:43:47.000000 microcat-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:38:34.903153 microcat-0.1.6/
+-rw-r--r--   0 root         (0) root         (0)    34599 2023-06-09 02:02:59.000000 microcat-0.1.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      396 2023-06-09 03:45:47.000000 microcat-0.1.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-06-17 14:38:34.903153 microcat-0.1.6/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      383 2023-05-18 11:49:26.000000 microcat-0.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:38:34.895153 microcat-0.1.6/microcat/
+-rwxrwxr-x   0 root         (0) root         (0)       73 2023-06-17 14:38:32.000000 microcat-0.1.6/microcat/__about__.py
+-rwxrwxr-x   0 root         (0) root         (0)      913 2023-06-17 14:38:27.000000 microcat-0.1.6/microcat/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:38:34.899153 microcat-0.1.6/microcat/config/
+-rw-r--r--   0 root         (0) root         (0)     2840 2023-06-17 11:49:35.000000 microcat-0.1.6/microcat/config/config.yaml
+-rwxr-xr-x   0 root         (0) root         (0)     8766 2023-06-09 03:49:23.000000 microcat-0.1.6/microcat/configer.py
+-rwxr-xr-x   0 root         (0) root         (0)    36419 2023-06-17 14:26:11.000000 microcat-0.1.6/microcat/corer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:38:34.899153 microcat-0.1.6/microcat/envs/
+-rw-r--r--   0 root         (0) root         (0)      125 2023-06-17 10:22:04.000000 microcat-0.1.6/microcat/envs/kmer_python.yaml
+-rw-r--r--   0 root         (0) root         (0)      390 2023-06-14 02:38:08.000000 microcat-0.1.6/microcat/envs/kmer_qc.yaml
+-rw-rw-r--   0 root         (0) root         (0)      164 2023-06-14 02:38:19.000000 microcat-0.1.6/microcat/envs/kraken2.yaml
+-rw-r--r--   0 root         (0) root         (0)      133 2023-05-31 02:41:36.000000 microcat-0.1.6/microcat/envs/krakenuniq.yaml
+-rw-r--r--   0 root         (0) root         (0)      109 2023-06-03 12:24:08.000000 microcat-0.1.6/microcat/envs/metaphlan.yaml
+-rwxr-xr-x   0 root         (0) root         (0)      145 2023-06-03 12:24:08.000000 microcat-0.1.6/microcat/envs/pathseq.yaml
+-rw-r--r--   0 root         (0) root         (0)      100 2023-06-07 06:24:12.000000 microcat-0.1.6/microcat/envs/star.yaml
+-rw-r--r--   0 root         (0) root         (0)      140 2023-05-31 02:41:36.000000 microcat-0.1.6/microcat/envs/trimming.yaml
+-rwxr-xr-x   0 root         (0) root         (0)     4320 2023-06-17 14:16:31.000000 microcat-0.1.6/microcat/prepare.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:38:34.895153 microcat-0.1.6/microcat/profiles/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:38:34.899153 microcat-0.1.6/microcat/profiles/lsf/
+-rw-r--r--   0 root         (0) root         (0)      955 2023-06-14 02:37:56.000000 microcat-0.1.6/microcat/profiles/lsf/CookieCutter.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2023-06-03 12:24:08.000000 microcat-0.1.6/microcat/profiles/lsf/OSLayer.py
+-rw-r--r--   0 root         (0) root         (0)      297 2023-06-03 12:24:08.000000 microcat-0.1.6/microcat/profiles/lsf/config.yaml
+-rwxr-xr-x   0 root         (0) root         (0)     1124 2023-06-03 12:24:08.000000 microcat-0.1.6/microcat/profiles/lsf/lsf_cancel.py
+-rw-r--r--   0 root         (0) root         (0)     1978 2023-06-03 12:24:08.000000 microcat-0.1.6/microcat/profiles/lsf/lsf_config.py
+-rwxr-xr-x   0 root         (0) root         (0)       48 2023-06-03 12:24:08.000000 microcat-0.1.6/microcat/profiles/lsf/lsf_jobscript.sh
+-rwxr-xr-x   0 root         (0) root         (0)     7511 2023-06-03 12:24:08.000000 microcat-0.1.6/microcat/profiles/lsf/lsf_status.py
+-rwxr-xr-x   0 root         (0) root         (0)     8281 2023-06-03 12:24:08.000000 microcat-0.1.6/microcat/profiles/lsf/lsf_submit.py
+-rw-r--r--   0 root         (0) root         (0)     3775 2023-06-03 12:24:08.000000 microcat-0.1.6/microcat/profiles/lsf/memory_units.py
+-rwxr-xr-x   0 root         (0) root         (0)    21400 2023-06-16 11:13:16.000000 microcat-0.1.6/microcat/rich_agrpase.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:38:34.899153 microcat-0.1.6/microcat/rules/
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-06-09 02:29:19.000000 microcat-0.1.6/microcat/rules/ERCC.smk
+-rw-r--r--   0 root         (0) root         (0)     2225 2023-06-10 01:41:24.000000 microcat-0.1.6/microcat/rules/build.smk
+-rw-r--r--   0 root         (0) root         (0)    40814 2023-06-09 02:28:56.000000 microcat-0.1.6/microcat/rules/classfier.smk
+-rw-r--r--   0 root         (0) root         (0)     3981 2023-06-07 01:22:00.000000 microcat-0.1.6/microcat/rules/database.smk
+-rw-r--r--   0 root         (0) root         (0)    42505 2023-06-17 11:13:48.000000 microcat-0.1.6/microcat/rules/host.smk
+-rwxr-xr-x   0 root         (0) root         (0)    10460 2023-06-05 09:08:14.000000 microcat-0.1.6/microcat/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:38:34.899153 microcat-0.1.6/microcat/scripts/
+-rw-r--r--   0 root         (0) root         (0)    15479 2023-06-08 03:30:56.000000 microcat-0.1.6/microcat/scripts/INVADEseq.py
+-rwxrwxrwx   0 root         (0) root         (0)    19072 2023-06-07 07:14:07.000000 microcat-0.1.6/microcat/scripts/extract_kraken_reads.py
+-rwxrwxrwx   0 root         (0) root         (0)     3849 2023-06-07 07:14:23.000000 microcat-0.1.6/microcat/scripts/extract_microbiome_output.R
+-rwxr-xr-x   0 root         (0) root         (0)     7896 2023-06-03 12:24:08.000000 microcat-0.1.6/microcat/scripts/get_ncbi_domains.py
+-rw-r--r--   0 root         (0) root         (0)     1185 2023-06-07 07:15:11.000000 microcat-0.1.6/microcat/scripts/krak2_output_denosing.R
+-rwxr-xr-x   0 root         (0) root         (0)     6942 2023-06-07 07:15:43.000000 microcat-0.1.6/microcat/scripts/kraken2mpa.py
+-rwxr-xr-x   0 root         (0) root         (0)    14784 2023-06-07 07:15:24.000000 microcat-0.1.6/microcat/scripts/kraken2sc.py
+-rw-r--r--   0 root         (0) root         (0)     4698 2023-06-07 07:14:59.000000 microcat-0.1.6/microcat/scripts/sample_denosing.R
+-rwxrwxrwx   0 root         (0) root         (0)    15665 2023-06-07 07:13:48.000000 microcat-0.1.6/microcat/scripts/sckmer_unpaired.R
+-rwxr-xr-x   0 root         (0) root         (0)     2367 2023-06-03 12:24:08.000000 microcat-0.1.6/microcat/scripts/spilt_bam_by_tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:38:34.903153 microcat-0.1.6/microcat/snakefiles/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:37:58.000000 microcat-0.1.6/microcat/snakefiles/bulk_wf.smk
+-rw-r--r--   0 root         (0) root         (0)     1832 2023-06-09 04:28:17.000000 microcat-0.1.6/microcat/snakefiles/scRNA_wf.smk
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:38:06.000000 microcat-0.1.6/microcat/snakefiles/spatial_wf.smk
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:38:34.899153 microcat-0.1.6/microcat.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-06-17 14:38:34.000000 microcat-0.1.6/microcat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1564 2023-06-17 14:38:34.000000 microcat-0.1.6/microcat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-17 14:38:34.000000 microcat-0.1.6/microcat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-06-17 14:38:34.000000 microcat-0.1.6/microcat.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-17 14:38:34.000000 microcat-0.1.6/microcat.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-17 14:38:34.000000 microcat-0.1.6/microcat.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-09 01:50:10.000000 microcat-0.1.6/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-17 14:38:34.903153 microcat-0.1.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-06-09 03:43:47.000000 microcat-0.1.6/setup.py
```

### Comparing `microcat-0.1.5/LICENSE` & `microcat-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `microcat-0.1.5/PKG-INFO` & `microcat-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microcat
-Version: 0.1.5
+Version: 0.1.6
 Summary: a computational toolbox to identificated microbiome from Omics
 Home-page: https://github.com/ChangxingSu/MicroCAT
 Author: Changxing Su
 Author-email: changxingsu42@gmail.com
 License: GPLv3+
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `microcat-0.1.5/microcat/__init__.py` & `microcat-0.1.6/microcat/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 from microcat.configer import MicrocatConfig
 from microcat.configer import parse_yaml
 from microcat.configer import update_config
-from microcat.configer import custom_help_formatter
+# from microcat.configer import custom_help_formatter
 
 from microcat.sample import HEADERS
 from microcat.sample import parse_samples
 from microcat.sample import parse_bam_samples
 
 
 from microcat.sample import get_starsolo_sample_id
```

### Comparing `microcat-0.1.5/microcat/config/config.yaml` & `microcat-0.1.6/microcat/config/config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -27,19 +27,19 @@
     kraken2uniq:
       do: true
       kraken2_database: "/data/database/kraken2_RefSeqV217_Complete_Chrom_nont"
       threads: 40
       mem_mb: 200000
     pathseq:
       do: false
-      microbe_bwa_image: /data/database/pathseq_database/ref201_CSI/reference.fasta.img
-      microbe_dict: /data/database/pathseq_database/ref201_CSI/microbev1.dict
-      host_bfi: /data/database/pathseq_database/ref201_CSI/pathseq_host.bfi
-      taxonomy_db: /data/database/pathseq_database/ref201_CSI/microbev1_release201_taxonomy.db
-      host_bwa_image: /data/database/pathseq_database/ref201_CSI/pathseq_host.fa.img
+      microbe_bwa_image: /data/database/pathseq_database/refv218/microbiome_RefseqV218_Compelete-Chromon.fasta.img
+      microbe_dict: /data/database/pathseq_database/refv218/microbiome_RefseqV218_Compelete-Chromon.dict
+      host_bfi: /data/database/pathseq_database/refv218/pathseq_resources_pathseq_host.bfi
+      taxonomy_db: /data/database/pathseq_database/refv218/microbiome_RefseqV218_Compelete-Chromon.db
+      host_bwa_image: /data/database/pathseq_database/refv218/pathseq_resources_pathseq_host.fa.img
       threads: 24
       mem_mb: 200000
     pathseqscore: ""
     
     metaphlan:
       do: false
       threads: 24
@@ -75,14 +75,17 @@
   host: "logs/02.host"
   classifier: "logs/03.classifier"
 
 benchmarks:
   host: "benchmarks/02.host"
   classifier: "benchmarks/03.classifier"
 
+datas:
+  barcode_list_dirs:
+    tenX: "/data/project/host-microbiome/microcat/microcat/data/"
 
 envs:
   kraken2: ../envs/kraken2.yaml
   krakenuniq: ../envs/krakenuniq.yaml
   pathseq: ../envs/pathseq.yaml
   metaphlan: ../envs/metaphlan.yaml
   kmer_qc: ../envs/kmer_qc.yaml
```

### Comparing `microcat-0.1.5/microcat/configer.py` & `microcat-0.1.6/microcat/configer.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.5/microcat/profiles/lsf/CookieCutter.py` & `microcat-0.1.6/microcat/profiles/lsf/CookieCutter.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.5/microcat/profiles/lsf/OSLayer.py` & `microcat-0.1.6/microcat/profiles/lsf/OSLayer.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.5/microcat/profiles/lsf/lsf_cancel.py` & `microcat-0.1.6/microcat/profiles/lsf/lsf_cancel.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.5/microcat/profiles/lsf/lsf_config.py` & `microcat-0.1.6/microcat/profiles/lsf/lsf_config.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.5/microcat/profiles/lsf/lsf_status.py` & `microcat-0.1.6/microcat/profiles/lsf/lsf_status.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.5/microcat/profiles/lsf/lsf_submit.py` & `microcat-0.1.6/microcat/profiles/lsf/lsf_submit.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.5/microcat/profiles/lsf/memory_units.py` & `microcat-0.1.6/microcat/profiles/lsf/memory_units.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.5/microcat/rules/ERCC.smk` & `microcat-0.1.6/microcat/rules/ERCC.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.1.5/microcat/rules/build.smk` & `microcat-0.1.6/microcat/rules/build.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.1.5/microcat/rules/classfier.smk` & `microcat-0.1.6/microcat/rules/classfier.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.1.5/microcat/rules/database.smk` & `microcat-0.1.6/microcat/rules/database.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.1.5/microcat/rules/host.smk` & `microcat-0.1.6/microcat/rules/host.smk`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,16 @@
                     barcode_reads = lambda wildcards: microcat.get_starsolo_sample_id(SAMPLES, wildcards, "fq1"),
                     cdna_reads = lambda wildcards: microcat.get_starsolo_sample_id(SAMPLES, wildcards, "fq2"),
                     starsolo_out = os.path.join(
                         config["output"]["host"],
                         "starsolo_count/"),
                     reference = config["params"]["host"]["starsolo"]["reference"],
                     variousParams = config["params"]["host"]["starsolo"]["variousParams"],
-                    threads = config["params"]["host"]["starsolo"]["threads"]
+                    threads = config["params"]["host"]["starsolo"]["threads"],
+                    barcode_list =  os.path.join(config["datas"]["barcode_lists"]["tenX"],"3M-february-2018.txt")
                 log:
                     os.path.join(config["logs"]["host"],
                                 "starsolo/{sample}_starsolo_count.log")
                 benchmark:
                     os.path.join(config["benchmarks"]["host"],
                                 "starsolo/{sample}_starsolo_count.benchmark")
                 conda:
@@ -144,15 +145,15 @@
                 message: "Executing starsolo with {params.threads} threads on the following files {wildcards.sample}.Library with 10x 3' V3"
                 shell:
                     '''
                     mkdir -p {params.starsolo_out}; 
                     cd {params.starsolo_out} ;
                     STAR \
                     --soloType CB_UMI_Simple \
-                    --soloCBwhitelist /data/project/host-microbiome/microcat/microcat/data/3M-february-2018.txt \
+                    --soloCBwhitelist {params.barcode_list} \
                     --soloCBstart 1 \
                     --soloCBlen 16 \
                     --soloUMIstart 17 \
                     --soloUMIlen 12 \
                     --genomeDir {params.reference} \
                     --readFilesIn {params.cdna_reads} {params.barcode_reads} \
                     --runThreadN {params.threads} \
@@ -200,15 +201,16 @@
                     barcode_reads = lambda wildcards: microcat.get_starsolo_sample_id(SAMPLES, wildcards, "fq1"),
                     cdna_reads = lambda wildcards: microcat.get_starsolo_sample_id(SAMPLES, wildcards, "fq2"),
                     starsolo_out = os.path.join(
                         config["output"]["host"],
                         "starsolo_count/"),
                     reference = config["params"]["host"]["starsolo"]["reference"],
                     variousParams = config["params"]["host"]["starsolo"]["variousParams"],
-                    threads = config["params"]["host"]["starsolo"]["threads"]
+                    threads = config["params"]["host"]["starsolo"]["threads"],
+                    barcode_list =  os.path.join(config["datas"]["barcode_lists"]["tenX"],"737K-april-2014_rc.txt")
                 log:
                     os.path.join(config["logs"]["host"],
                                 "starsolo/{sample}_starsolo_count.log")
                 benchmark:
                     os.path.join(config["benchmarks"]["host"],
                                 "starsolo/{sample}_starsolo_count.benchmark")
                 conda:
@@ -216,15 +218,15 @@
                 message: "Executing starsolo with {params.threads} threads on the following files {wildcards.sample}.Library with 10x 3' V1"
                 shell:
                     '''
                     mkdir -p {params.starsolo_out}; 
                     cd {params.starsolo_out} ;
                     STAR \
                     --soloType CB_UMI_Simple \
-                    --soloCBwhitelist ../data/737K-april-2014_rc.txt \
+                    --soloCBwhitelist {params.barcode_list} \
                     --soloCBstart 1 \
                     --soloCBlen 16 \
                     --soloUMIstart 17 \
                     --soloUMIlen 10 \
                     --soloBarcodeReadLength 150 \
                     --genomeDir {params.reference} \
                     --readFilesIn {input.cdna_reads} {input.barcode_reads} \
@@ -274,15 +276,16 @@
                     starsolo_out = os.path.join(
                         config["output"]["host"],
                         "starsolo_count/"),
                     reference = config["params"]["host"]["starsolo"]["reference"],
                     variousParams = config["params"]["host"]["starsolo"]["variousParams"],
                     threads = config["params"]["host"]["starsolo"]["threads"],
                     barcode_reads = lambda wildcards: microcat.get_starsolo_sample_id(SAMPLES, wildcards, "fq1"),
-                    cdna_reads = lambda wildcards: microcat.get_starsolo_sample_id(SAMPLES, wildcards, "fq2")
+                    cdna_reads = lambda wildcards: microcat.get_starsolo_sample_id(SAMPLES, wildcards, "fq2"),
+                    barcode_list =  os.path.join(config["datas"]["barcode_lists"]["tenX"],"737K-august-2016.txt")
                 log:
                     os.path.join(config["logs"]["host"],
                                 "starsolo/{sample}_starsolo_count.log")
                 benchmark:
                     os.path.join(config["benchmarks"]["host"],
                                 "starsolo/{sample}_starsolo_count.benchmark")
                 conda:
@@ -293,15 +296,15 @@
                 message: "Executing starsolo with {params.threads} threads on the following files {wildcards.sample}.Library with 10x 3' V2."
                 shell:
                     '''
                     mkdir -p {params.starsolo_out}; 
                     cd {params.starsolo_out} ;
                     STAR \
                     --soloType CB_UMI_Simple \
-                    --soloCBwhitelist /data/project/host-microbiome/microcat/microcat/data/737K-august-2016.txt \
+                    --soloCBwhitelist {params.barcode_list} \
                     --soloCBstart 1 \
                     --soloCBlen 16 \
                     --soloUMIstart 17 \
                     --soloUMIlen 10 \
                     --genomeDir {params.reference} \
                     --readFilesIn {params.cdna_reads}  {params.barcode_reads} \
                     --runThreadN {params.threads} \
```

### Comparing `microcat-0.1.5/microcat/sample.py` & `microcat-0.1.6/microcat/sample.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.5/microcat/scripts/INVADEseq.py` & `microcat-0.1.6/microcat/scripts/INVADEseq.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.5/microcat/scripts/extract_kraken_reads.py` & `microcat-0.1.6/microcat/scripts/extract_kraken_reads.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.5/microcat/scripts/extract_microbiome_output.R` & `microcat-0.1.6/microcat/scripts/extract_microbiome_output.R`

 * *Files identical despite different names*

### Comparing `microcat-0.1.5/microcat/scripts/get_ncbi_domains.py` & `microcat-0.1.6/microcat/scripts/get_ncbi_domains.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.5/microcat/scripts/krak2_output_denosing.R` & `microcat-0.1.6/microcat/scripts/krak2_output_denosing.R`

 * *Files identical despite different names*

### Comparing `microcat-0.1.5/microcat/scripts/kraken2mpa.py` & `microcat-0.1.6/microcat/scripts/kraken2mpa.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.5/microcat/scripts/kraken2sc.py` & `microcat-0.1.6/microcat/scripts/kraken2sc.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.5/microcat/scripts/sample_denosing.R` & `microcat-0.1.6/microcat/scripts/sample_denosing.R`

 * *Files identical despite different names*

### Comparing `microcat-0.1.5/microcat/scripts/sckmer_unpaired.R` & `microcat-0.1.6/microcat/scripts/sckmer_unpaired.R`

 * *Files identical despite different names*

### Comparing `microcat-0.1.5/microcat/scripts/spilt_bam_by_tag.py` & `microcat-0.1.6/microcat/scripts/spilt_bam_by_tag.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.5/microcat/snakefiles/scRNA_wf.smk` & `microcat-0.1.6/microcat/snakefiles/scRNA_wf.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.1.5/microcat.egg-info/PKG-INFO` & `microcat-0.1.6/microcat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microcat
-Version: 0.1.5
+Version: 0.1.6
 Summary: a computational toolbox to identificated microbiome from Omics
 Home-page: https://github.com/ChangxingSu/MicroCAT
 Author: Changxing Su
 Author-email: changxingsu42@gmail.com
 License: GPLv3+
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `microcat-0.1.5/microcat.egg-info/SOURCES.txt` & `microcat-0.1.6/microcat.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 requirements.txt
 setup.py
 microcat/__about__.py
 microcat/__init__.py
 microcat/configer.py
 microcat/corer.py
 microcat/prepare.py
+microcat/rich_agrpase.py
 microcat/sample.py
 microcat.egg-info/PKG-INFO
 microcat.egg-info/SOURCES.txt
 microcat.egg-info/dependency_links.txt
 microcat.egg-info/entry_points.txt
 microcat.egg-info/requires.txt
 microcat.egg-info/top_level.txt
```

### Comparing `microcat-0.1.5/setup.py` & `microcat-0.1.6/setup.py`

 * *Files identical despite different names*

