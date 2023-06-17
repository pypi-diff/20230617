# Comparing `tmp/CtrlF_TF-1.0b3.tar.gz` & `tmp/CtrlF_TF-1.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CtrlF_TF-1.0b3.tar", last modified: Fri Mar  3 03:13:12 2023, max compression
+gzip compressed data, was "CtrlF_TF-1.0b4.tar", last modified: Sat Jun 17 01:09:15 2023, max compression
```

## Comparing `CtrlF_TF-1.0b3.tar` & `CtrlF_TF-1.0b4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 zmielko   (1000) zmielko   (1000)        0 2023-03-03 03:13:12.364368 CtrlF_TF-1.0b3/
--rw-rw-r--   0 zmielko   (1000) zmielko   (1000)     1522 2023-03-02 18:39:28.000000 CtrlF_TF-1.0b3/LICENSE
--rw-rw-r--   0 zmielko   (1000) zmielko   (1000)     1338 2023-03-03 03:13:12.364368 CtrlF_TF-1.0b3/PKG-INFO
--rw-rw-r--   0 zmielko   (1000) zmielko   (1000)      806 2023-03-02 18:39:28.000000 CtrlF_TF-1.0b3/README.md
--rw-rw-r--   0 zmielko   (1000) zmielko   (1000)      791 2023-03-03 03:13:12.364368 CtrlF_TF-1.0b3/setup.cfg
--rw-rw-r--   0 zmielko   (1000) zmielko   (1000)       39 2023-03-02 18:39:28.000000 CtrlF_TF-1.0b3/setup.py
-drwxrwxr-x   0 zmielko   (1000) zmielko   (1000)        0 2023-03-03 03:13:12.360368 CtrlF_TF-1.0b3/src/
-drwxrwxr-x   0 zmielko   (1000) zmielko   (1000)        0 2023-03-03 03:13:12.360368 CtrlF_TF-1.0b3/src/CtrlF_TF.egg-info/
--rw-rw-r--   0 zmielko   (1000) zmielko   (1000)     1338 2023-03-03 03:13:12.000000 CtrlF_TF-1.0b3/src/CtrlF_TF.egg-info/PKG-INFO
--rw-rw-r--   0 zmielko   (1000) zmielko   (1000)      590 2023-03-03 03:13:12.000000 CtrlF_TF-1.0b3/src/CtrlF_TF.egg-info/SOURCES.txt
--rw-rw-r--   0 zmielko   (1000) zmielko   (1000)        1 2023-03-03 03:13:12.000000 CtrlF_TF-1.0b3/src/CtrlF_TF.egg-info/dependency_links.txt
--rw-rw-r--   0 zmielko   (1000) zmielko   (1000)       49 2023-03-03 03:13:12.000000 CtrlF_TF-1.0b3/src/CtrlF_TF.egg-info/entry_points.txt
--rw-rw-r--   0 zmielko   (1000) zmielko   (1000)       51 2023-03-03 03:13:12.000000 CtrlF_TF-1.0b3/src/CtrlF_TF.egg-info/requires.txt
--rw-rw-r--   0 zmielko   (1000) zmielko   (1000)        9 2023-03-03 03:13:12.000000 CtrlF_TF-1.0b3/src/CtrlF_TF.egg-info/top_level.txt
-drwxrwxr-x   0 zmielko   (1000) zmielko   (1000)        0 2023-03-03 03:13:12.364368 CtrlF_TF-1.0b3/src/ctrlf_tf/
--rw-rw-r--   0 zmielko   (1000) zmielko   (1000)      313 2023-03-02 18:39:28.000000 CtrlF_TF-1.0b3/src/ctrlf_tf/__init__.py
--rw-rw-r--   0 zmielko   (1000) zmielko   (1000)    13538 2023-03-03 02:24:24.000000 CtrlF_TF-1.0b3/src/ctrlf_tf/cli_prgm.py
--rw-rw-r--   0 zmielko   (1000) zmielko   (1000)    18833 2023-03-02 18:51:12.000000 CtrlF_TF-1.0b3/src/ctrlf_tf/compile_utils.py
--rw-rw-r--   0 zmielko   (1000) zmielko   (1000)    27417 2023-03-02 22:04:36.000000 CtrlF_TF-1.0b3/src/ctrlf_tf/ctrlf_core.py
--rw-rw-r--   0 zmielko   (1000) zmielko   (1000)    16533 2023-03-02 23:25:35.000000 CtrlF_TF-1.0b3/src/ctrlf_tf/optimize_core.py
--rw-rw-r--   0 zmielko   (1000) zmielko   (1000)    19252 2023-03-03 02:46:46.000000 CtrlF_TF-1.0b3/src/ctrlf_tf/optimize_utils.py
--rw-rw-r--   0 zmielko   (1000) zmielko   (1000)     8341 2023-03-02 18:39:28.000000 CtrlF_TF-1.0b3/src/ctrlf_tf/parse_utils.py
--rw-rw-r--   0 zmielko   (1000) zmielko   (1000)    11817 2023-03-02 18:39:28.000000 CtrlF_TF-1.0b3/src/ctrlf_tf/pwm_utils.py
--rw-rw-r--   0 zmielko   (1000) zmielko   (1000)    16635 2023-03-02 23:18:20.000000 CtrlF_TF-1.0b3/src/ctrlf_tf/site_call_utils.py
--rw-rw-r--   0 zmielko   (1000) zmielko   (1000)     5762 2023-03-02 20:40:48.000000 CtrlF_TF-1.0b3/src/ctrlf_tf/str_utils.py
--rw-rw-r--   0 zmielko   (1000) zmielko   (1000)     6936 2023-03-02 18:39:28.000000 CtrlF_TF-1.0b3/src/ctrlf_tf/threshold_utils.py
-drwxrwxr-x   0 zmielko   (1000) zmielko   (1000)        0 2023-03-03 03:13:12.364368 CtrlF_TF-1.0b3/tests/
--rw-rw-r--   0 zmielko   (1000) zmielko   (1000)     2239 2023-03-02 18:39:28.000000 CtrlF_TF-1.0b3/tests/test_str_utils.py
+drwxrwxr-x   0 zmielko   (1000) zmielko   (1000)        0 2023-06-17 01:09:15.299077 CtrlF_TF-1.0b4/
+-rw-rw-r--   0 zmielko   (1000) zmielko   (1000)     1522 2023-06-16 19:53:58.000000 CtrlF_TF-1.0b4/LICENSE
+-rw-rw-r--   0 zmielko   (1000) zmielko   (1000)     1338 2023-06-17 01:09:15.299077 CtrlF_TF-1.0b4/PKG-INFO
+-rw-rw-r--   0 zmielko   (1000) zmielko   (1000)      806 2023-06-16 19:53:58.000000 CtrlF_TF-1.0b4/README.md
+-rw-rw-r--   0 zmielko   (1000) zmielko   (1000)      791 2023-06-17 01:09:15.299077 CtrlF_TF-1.0b4/setup.cfg
+-rw-rw-r--   0 zmielko   (1000) zmielko   (1000)       39 2023-06-16 19:53:58.000000 CtrlF_TF-1.0b4/setup.py
+drwxrwxr-x   0 zmielko   (1000) zmielko   (1000)        0 2023-06-17 01:09:15.295077 CtrlF_TF-1.0b4/src/
+drwxrwxr-x   0 zmielko   (1000) zmielko   (1000)        0 2023-06-17 01:09:15.295077 CtrlF_TF-1.0b4/src/CtrlF_TF.egg-info/
+-rw-rw-r--   0 zmielko   (1000) zmielko   (1000)     1338 2023-06-17 01:09:15.000000 CtrlF_TF-1.0b4/src/CtrlF_TF.egg-info/PKG-INFO
+-rw-rw-r--   0 zmielko   (1000) zmielko   (1000)      590 2023-06-17 01:09:15.000000 CtrlF_TF-1.0b4/src/CtrlF_TF.egg-info/SOURCES.txt
+-rw-rw-r--   0 zmielko   (1000) zmielko   (1000)        1 2023-06-17 01:09:15.000000 CtrlF_TF-1.0b4/src/CtrlF_TF.egg-info/dependency_links.txt
+-rw-rw-r--   0 zmielko   (1000) zmielko   (1000)       49 2023-06-17 01:09:15.000000 CtrlF_TF-1.0b4/src/CtrlF_TF.egg-info/entry_points.txt
+-rw-rw-r--   0 zmielko   (1000) zmielko   (1000)       51 2023-06-17 01:09:15.000000 CtrlF_TF-1.0b4/src/CtrlF_TF.egg-info/requires.txt
+-rw-rw-r--   0 zmielko   (1000) zmielko   (1000)        9 2023-06-17 01:09:15.000000 CtrlF_TF-1.0b4/src/CtrlF_TF.egg-info/top_level.txt
+drwxrwxr-x   0 zmielko   (1000) zmielko   (1000)        0 2023-06-17 01:09:15.299077 CtrlF_TF-1.0b4/src/ctrlf_tf/
+-rw-rw-r--   0 zmielko   (1000) zmielko   (1000)      299 2023-06-16 19:53:58.000000 CtrlF_TF-1.0b4/src/ctrlf_tf/__init__.py
+-rw-rw-r--   0 zmielko   (1000) zmielko   (1000)    14906 2023-06-16 19:53:58.000000 CtrlF_TF-1.0b4/src/ctrlf_tf/cli_prgm.py
+-rw-rw-r--   0 zmielko   (1000) zmielko   (1000)    18582 2023-06-16 19:53:58.000000 CtrlF_TF-1.0b4/src/ctrlf_tf/compile_utils.py
+-rw-rw-r--   0 zmielko   (1000) zmielko   (1000)    31161 2023-06-16 19:53:58.000000 CtrlF_TF-1.0b4/src/ctrlf_tf/ctrlf_core.py
+-rw-rw-r--   0 zmielko   (1000) zmielko   (1000)    16870 2023-06-16 19:53:58.000000 CtrlF_TF-1.0b4/src/ctrlf_tf/optimize_core.py
+-rw-rw-r--   0 zmielko   (1000) zmielko   (1000)    19230 2023-06-16 19:53:58.000000 CtrlF_TF-1.0b4/src/ctrlf_tf/optimize_utils.py
+-rw-rw-r--   0 zmielko   (1000) zmielko   (1000)     8481 2023-06-16 19:53:58.000000 CtrlF_TF-1.0b4/src/ctrlf_tf/parse_utils.py
+-rw-rw-r--   0 zmielko   (1000) zmielko   (1000)    11873 2023-06-16 19:53:58.000000 CtrlF_TF-1.0b4/src/ctrlf_tf/pwm_utils.py
+-rw-rw-r--   0 zmielko   (1000) zmielko   (1000)    18317 2023-06-16 19:56:17.000000 CtrlF_TF-1.0b4/src/ctrlf_tf/site_call_utils.py
+-rw-rw-r--   0 zmielko   (1000) zmielko   (1000)     8110 2023-06-16 19:53:58.000000 CtrlF_TF-1.0b4/src/ctrlf_tf/str_utils.py
+-rw-rw-r--   0 zmielko   (1000) zmielko   (1000)     6936 2023-06-16 19:53:58.000000 CtrlF_TF-1.0b4/src/ctrlf_tf/threshold_utils.py
+drwxrwxr-x   0 zmielko   (1000) zmielko   (1000)        0 2023-06-17 01:09:15.299077 CtrlF_TF-1.0b4/tests/
+-rw-rw-r--   0 zmielko   (1000) zmielko   (1000)     2239 2023-06-16 19:53:58.000000 CtrlF_TF-1.0b4/tests/test_str_utils.py
```

### Comparing `CtrlF_TF-1.0b3/LICENSE` & `CtrlF_TF-1.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `CtrlF_TF-1.0b3/PKG-INFO` & `CtrlF_TF-1.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CtrlF_TF
-Version: 1.0b3
+Version: 1.0b4
 Summary: Protein-DNA binding site caller from kmer data
 Author: Zachery Mielko
 License: BSD 3-Clause License
 Keywords: Bioinformatics,Scientific Computing
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `CtrlF_TF-1.0b3/README.md` & `CtrlF_TF-1.0b4/README.md`

 * *Files identical despite different names*

### Comparing `CtrlF_TF-1.0b3/setup.cfg` & `CtrlF_TF-1.0b4/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = CtrlF_TF
-version = 1.0b3
+version = 1.0b4
 author = Zachery Mielko
 keywords = Bioinformatics, Scientific Computing
 description = Protein-DNA binding site caller from kmer data
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = BSD 3-Clause License
 classifiers =
```

### Comparing `CtrlF_TF-1.0b3/src/CtrlF_TF.egg-info/PKG-INFO` & `CtrlF_TF-1.0b4/src/CtrlF_TF.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CtrlF-TF
-Version: 1.0b3
+Version: 1.0b4
 Summary: Protein-DNA binding site caller from kmer data
 Author: Zachery Mielko
 License: BSD 3-Clause License
 Keywords: Bioinformatics,Scientific Computing
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `CtrlF_TF-1.0b3/src/CtrlF_TF.egg-info/SOURCES.txt` & `CtrlF_TF-1.0b4/src/CtrlF_TF.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CtrlF_TF-1.0b3/src/ctrlf_tf/cli_prgm.py` & `CtrlF_TF-1.0b4/src/ctrlf_tf/cli_prgm.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,137 +4,140 @@
 import argparse
 import sys
 
 import pandas as pd
 import ctrlf_tf as cftf
 
 
-MAIN_DESCRIPTION = ("CtrlF-TF: TF Binding Site Search via Aligned Sequences.")
+MAIN_DESCRIPTION = ("CtrlF-TF: Transcription Factor Binding Site Search via Aligned Sequences.")
 
 
-def _config_compile_parser(parser):
-    """Configure the arguments for the align subprogram."""
-    required = parser.add_argument_group("required arguments")
-    optimization = parser.add_argument_group("optimization arguments")
-    required.add_argument("-a",
+def _add_output_to_parser(parser):
+    parser.add_argument("-o",
+                        "--output",
+                        type=str,
+                        default=None,
+                        help="Output file, stdout by default")
+    return parser
+
+
+def _add_alignparams_to_parser(parser):
+    alignment = parser.add_argument_group("Alignment Parameters")
+    alignment.add_argument("-a",
                           "--align_model",
                           required=True,
                           type=str,
                           help="Alignment model")
-    required.add_argument("-k",
+    alignment.add_argument("-k",
                           "--kmer_file",
                           required=True,
                           type=str,
-                          help="Kmer file in a")
-    parser.add_argument("-o",
-                        "--output",
-                        type=str,
-                        default=None,
-                        help="Output file, stdout by default")
-    parser.add_argument("-p",
+                          help="File with k-mers and a ranked score.")
+    alignment.add_argument("-p",
                         "--palindrome",
                         action="store_true",
                         help="Boolean flag if the model is palindromic")
-    parser.add_argument("-m",
+    alignment.add_argument("-m",
                         "--meme",
                         action="store_true",
                         help="Boolean flag if the model is in MEME format")
-    parser.add_argument("-g",
+    alignment.add_argument("-g",
                         "--gap_limit",
                         type=int,
                         default=0,
                         help="""Filters the kmer dataframe for kmers with a
                                  max count of gaps. Must be 0 or a positive
                                  integer (default is 0).""")
-    parser.add_argument("-t",
+    alignment.add_argument("-t",
                         "--threshold",
                         type=float,
                         help=("Threshold score for kmers to align, if no "
                               "-tc argument provided, uses 3rd column."))
-    parser.add_argument("-tc",
+    alignment.add_argument("-tc",
                         "--threshold_column",
                         type=str,
                         help=("Column in the kmer dataframe to use for the "
                               "rank score (Default is 3rd column)."))
-    parser.add_argument("-r",
+    alignment.add_argument("-r",
                         "--range",
                         nargs=2,
                         type=int,
                         default=(0, 0),
                         help="""Core range for PWM model (1-based), default is
                                  the whole input""")
-    parser.add_argument("-cg",
+    alignment.add_argument("-cg",
                         "--core_gap",
                         nargs='*',
                         type=int,
                         default=None,
                         help="""Positions within the core range (1-based,
                         relative to core range '-r') that are not part of the
                         kmer description of a site. Must be given with the '-r'
                         argument""")
-    parser.add_argument("-rc",
+    alignment.add_argument("-rc",
                         "--range_consensus",
                         type=str,
                         default=None,
                         help="""Definition of -r and -cg using the alignment of a
                         consensus site instead. A '.' character in the
                         consensus string indicates a -cg position.""")
-    optimization.add_argument("-opt",
-                              "--optimize",
-                              action="store_true",
-                              help="Boolean flag to perform optimization on classified sequences.")
+    return parser
+
+
+def _config_optimize_parser(parser):
+    parser = _add_alignparams_to_parser(parser)
+    parser = _add_output_to_parser(parser)
+    optimization = parser.add_argument_group("Optimization Parameters")
     optimization.add_argument("-c",
                               "--classify_file",
                               type=str,
                               help="Output file from 'ctrlf classify'")
     optimization.add_argument("-fpr",
                               "--fpr_threshold",
                               type=float,
                               default=0.01,
                               help="FPR target for optimization on de bruijn data.")
-    optimization.add_argument("-orep",
-                              "--output_report",
-                              type=str,
-                              default=None,
-                              help="Output file location for Optimization Report (Default is no output)")
     optimization.add_argument("-gthr",
                               "--gap_thresholds",
                               nargs='*',
-                              default=[0.25, 0.35, 0.38],
+                              default=[0.35, 0.35, 0.38],
                               type=float,
                               help="Rank score thresholds for optimizing gaps (Default is E-score based)")
-    optimization.add_argument("-opt_only",
-                              "--optimization_only",
-                              action="store_true",
-                              help="Boolean flag, if used the program only does the optimization and does not compile the top answer.")
+    return parser
+
+
+def _config_align_compile_parser(parser):
+    parser = _add_alignparams_to_parser(parser)
+    parser = _add_output_to_parser(parser)
+    parser.add_argument("-oi",
+                        "--optimize_input",
+                        type=str,
+                        default=None,
+                        help="Use parameters from an optimization report as input in addition to -a and -k.")
     return parser
 
 
 def _config_call_parser(parser):
     """Configure the arguments for the call subprogram parser."""
     required = parser.add_argument_group("required arguments")
-    required.add_argument("-c",
-                          "--consensus_sites",
+    required.add_argument("-i",
+                          "--input_model",
                           required=True,
                           type=str,
-                          help="Compiled consensus sites file.")
+                          help="Input of Aligned k-mers or Compiled Solutions.")
     required.add_argument("-f",
                           "--fasta_file",
                           required=True,
                           type=str,
                           help="Fasta file of DNA sequences")
-    parser.add_argument("-o",
-                        "--output",
-                        type=str,
-                        default=None,
-                        help="Output file, stdout by default")
     parser.add_argument("-gc",
                         "--genomic_coordinates",
                         action="store_true",
                         help="Parse fasta input for genomic coordinates")
+    parser = _add_output_to_parser(parser)
     return parser
 
 
 def _config_classify_parser(parser):
     """Configure the arguments for the classify subprogram parser."""
     required = parser.add_argument_group("required arguments")
     required.add_argument("-i",
@@ -180,20 +183,28 @@
     """Parse arguments for ctrlf_cli."""
     # Define main parser
     main_parser = argparse.ArgumentParser(description=MAIN_DESCRIPTION)
     main_parser.add_argument('-v', '--version',action="store_true", help="Return version.")
     subparsers = main_parser.add_subparsers(dest="program",
                                             help="Available subcommands:")
     # Align program parser definition
-    align_parser = subparsers.add_parser("compile",
-                                         help="Align and compile k-mers into aligned sequences containing sites.")
-    align_parser = _config_compile_parser(align_parser)
+    align_parser = subparsers.add_parser("align",
+                                         help="Align k-mers to a model.")
+    align_parser = _config_align_compile_parser(align_parser)
+    # Compile program parser definition
+    compile_parser = subparsers.add_parser("compile",
+                                         help="Compile k-mers into aligned consensus sites by generating all possible solutions.")
+    compile_parser = _config_align_compile_parser(compile_parser)
+    # Optimization
+    optimize_parser = subparsers.add_parser("optimize",
+                                            help="Optimize alignment parameters based on de Bruijn sequence classification.")
+    optimize_parser = _config_optimize_parser(optimize_parser)
     # Call program parser definition
-    call_parser = subparsers.add_parser("sitecall",
-                                        help="Call sites using the aligned sequences containing sites.")
+    call_parser = subparsers.add_parser("callsites",
+                                        help="Call sites using aligned k-mers or compiled solutions.")
     call_parser = _config_call_parser(call_parser)
     # Classify program parser
     classify_parser = subparsers.add_parser("classify",
                                             help="Classify a table of values and sequences for optimization.")
     classify_parser = _config_classify_parser(classify_parser)
     return main_parser
 
@@ -230,35 +241,59 @@
     if args.core_gap is not None and args.range is None:
         parser.error("'-cg' was given without specifying '-r'")
     if args.range_consensus and args.range != (0, 0):
         parser.error("-r must be specified with either -r or -rc, not both.")
     return True
 
 
+def _align_program(args):
+    parameters = _args_to_align_parameters(args)
+    if args.optimize_input:
+        opt_obj = cftf.Optimize.load_from_file(args.optimize_input)
+        parameters = opt_obj.optimal_parameters
+        parameters.pwm_file = args.align_model
+        parameters.kmer_file = args.kmer_file
+    aligned_kmers = cftf.AlignedKmers.from_parameters(parameters)
+    aligned_kmers.save_alignment(args.output)
+
+
 def _compile_program(args):
     parameters = _args_to_align_parameters(args)
-    if args.optimize:
-        gap_thresholds = {}
-        for idx, i in enumerate(args.gap_thresholds):
-            gap_thresholds[idx] = i
-        classified_seqs = cftf.ClassifiedSequences.load_from_file(args.classify_file)
-        opt_obj = cftf.Optimize(align_parameters=parameters,
-                                classified_df=classified_seqs.dataframe,
-                                fpr_threshold=args.fpr_threshold,
-                                gap_thresholds=gap_thresholds)
+    if args.optimize_input:
+        opt_obj = cftf.Optimize.load_from_file(args.optimize_input)
         parameters = opt_obj.optimal_parameters
-        if args.output_report:
-            opt_obj.save_to_file(args.output_report)
-    if args.optimization_only is False:
-        compiled_kmers = cftf.CompiledKmers.from_parameters(parameters)
-        compiled_kmers.save_compiled_sites(args.output)
+        parameters.pwm_file = args.align_model
+        parameters.kmer_file = args.kmer_file
+    compiled_kmers = cftf.CtrlF.from_parameters(parameters)
+    compiled_kmers.compile_all_solutions()
+    compiled_kmers.save_compiled_sites(args.output)
+
+
+def _optimize_program(args):
+    parameters = _args_to_align_parameters(args)
+    gap_thresholds = {}
+    for idx, i in enumerate(args.gap_thresholds):
+        gap_thresholds[idx] = i
+    classified_seqs = cftf.ClassifiedSequences.load_from_file(args.classify_file)
+    opt_obj = cftf.Optimize(align_parameters=parameters,
+                            classified_df=classified_seqs.dataframe,
+                            fpr_threshold=args.fpr_threshold,
+                            gap_thresholds=gap_thresholds)
+    parameters = opt_obj.optimal_parameters
+    opt_obj.save_to_file(args.output)
 
 
 def _call_program(args):
-    ctrlf_object = cftf.CtrlF.from_compiled_sites(args.consensus_sites)
+    # Determine if to init CtrlF from k-mers or solutions
+    with open(args.input_model) as read_obj:
+        lines = read_obj.readlines()
+        if lines[1].startswith("#Palindrome"):
+            ctrlf_object = cftf.CtrlF.from_alignment_file(args.input_model)
+        else:
+            ctrlf_object = cftf.CtrlF.from_compiled_sites(args.input_model)
     if args.output:
         output = args.output
     else:
         output = sys.stdout
     ctrlf_object.call_sites_from_fasta(args.fasta_file,
                                        args.genomic_coordinates,
                                        output)
@@ -292,17 +327,23 @@
     """CtrlF-TF CLI logic."""
     parser = _cli_parser()
     arguments = parser.parse_args()
     # If the main program is run
     if arguments.program == "compile":
         _align_parser_validation(parser, arguments)
         _compile_program(arguments)
+    elif arguments.program == "align":
+        _align_parser_validation(parser, arguments)
+        _align_program(arguments)
+    elif arguments.program == "optimize":
+        _align_parser_validation(parser, arguments)
+        _optimize_program(arguments)
     elif arguments.program == "classify":
         _classify_program(arguments)
     elif arguments.version:
         print(cftf.__version__)
-    elif arguments.program == "sitecall":
+    elif arguments.program == "callsites":
         _call_program(arguments)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `CtrlF_TF-1.0b3/src/ctrlf_tf/compile_utils.py` & `CtrlF_TF-1.0b4/src/ctrlf_tf/compile_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,22 +10,14 @@
 import pandas as pd
 import ctrlf_tf.str_utils
 
 COMPILED_LABEL = "Aligned_Binding_Sites"
 ALIGNED_POSITION_LABEL = "Relative_Position"
 
 
-def bounds_from_aligned_positions(aligned_positions: Iterable[int],
-                                  max_word_len: int) -> tuple:
-    """Returns a left and right bound integer as a tuple."""
-    left_bound = min(aligned_positions)
-    right_bound = max(aligned_positions) + max_word_len
-    return (left_bound, right_bound)
-
-
 def sequence_position(sequence: str) -> tuple:
     """Return tuple with start and end positions of an aligned sequence."""
     # Initialize parameters
     left = -1
     right = len(sequence) - 1
     found_sequence=False
     for idx, letter in enumerate(sequence):
@@ -379,16 +371,16 @@
             result.add(sol_query)
     return result
 
 
 def bounds_from_aligned_kmer_df(kmer_dataframe):
     max_word_len = max([len(kmer) for kmer in kmer_dataframe.iloc[:, 0]])
     aligned_positions = kmer_dataframe.iloc[:, 1]
-    left_bound, right_bound = bounds_from_aligned_positions(aligned_positions,
-                                                            max_word_len)
+    left_bound, right_bound = ctrlf_tf.str_utils.bounds_from_aligned_positions(aligned_positions,
+                                                                               max_word_len)
     return (left_bound, right_bound)
 
 
 def relative_consensus_df_from_abs(input_df, abs_core_start):
     df = input_df.copy(deep=True)
     df["Align_Position"] = df[COMPILED_LABEL].apply(lambda x: get_align_position(x))
     df[COMPILED_LABEL] = df[COMPILED_LABEL].apply(lambda x: x.strip('.'))
@@ -399,16 +391,16 @@
 
 def compile_consensus_sites(kmer_dataframe, core_positions):
     kmer_dataframe = kmer_dataframe.drop_duplicates().reset_index(drop=True)
     # Calculate bounds
     kmers = kmer_dataframe.iloc[:, 0]
     max_word_len = max([len(kmer) for kmer in kmer_dataframe.iloc[:, 0]])
     aligned_positions = kmer_dataframe.iloc[:, 1]
-    left_bound, right_bound = bounds_from_aligned_positions(aligned_positions,
-                                                            max_word_len)
+    left_bound, right_bound = ctrlf_tf.str_utils.bounds_from_aligned_positions(aligned_positions,
+                                                                               max_word_len)
     # Pad k-mers relative to bounds
     padded_kmers = []
     for row in kmer_dataframe.itertuples():
         padded_kmer = pad_k(row.Kmer, row.Align_Position, left_bound, right_bound)
         padded_kmers.append(padded_kmer)
     #Create Matricies
     traverse_m, compat_m = create_traverse_compatibility_matricies(padded_kmers)
```

### Comparing `CtrlF_TF-1.0b3/src/ctrlf_tf/ctrlf_core.py` & `CtrlF_TF-1.0b4/src/ctrlf_tf/ctrlf_core.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,24 +13,25 @@
 
 import copy
 from dataclasses import dataclass, fields
 from io import StringIO
 import sys
 from typing import Iterable, Tuple
 
+import networkx as nx
 import numpy as np
 import pandas as pd
 
 import ctrlf_tf.pwm_utils
 import ctrlf_tf.str_utils
 import ctrlf_tf.parse_utils
 import ctrlf_tf.compile_utils
 import ctrlf_tf.site_call_utils
 
-__version__ = "1.0b3"
+__version__ = "1.0b4"
 __author__ = "Zachery Mielko"
 
 
 @dataclass
 class AlignParameters:
     """Dataclass for input parameters to align k-mers to a model.
 
@@ -166,23 +167,27 @@
     def __init__(self,
                  core_positions: Tuple[int] = None,
                  aligned_kmer_dataframe: pd.DataFrame = None,
                  k: int = None,
                  palindrome: bool = None,
                  pwm: np.ndarray = None,
                  version: str = None,
-                 kmer_dataframe: pd.DataFrame = None):
+                 kmer_dataframe: pd.DataFrame = None,
+                 traversal_graph: nx.Graph = None):
         """Class initialization."""
         self.core_positions = core_positions
         self.aligned_kmer_dataframe = aligned_kmer_dataframe
         self.k = k
         self.palindrome = palindrome
         self.pwm = pwm
         self.version = version
         self.kmer_dataframe = kmer_dataframe
+        self.traversal_graph = traversal_graph
+        if self.core_positions:
+            self.core_span = max(self.core_positions)
 
     @classmethod
     def from_parameters(cls, parameters: AlignParameters):
         """Construcor using an AlignedParameters object.
 
         A factory constructor that aligned kmers to a PWM model using
         parameters defined in a *AlignParameters* class.
@@ -207,32 +212,36 @@
         if parameters.pwm_reverse_complement:
             pwm = pwm[::-1, ::-1]
         # Specify core range
         core_range = (parameters.core_start, parameters.core_end)
         pwm = ctrlf_tf.pwm_utils.trim_pwm_by_core(pwm, core_range, parameters.core_gaps)
         # Find core absolute start position and relative positions
         core_positions = ctrlf_tf.pwm_utils.core_positions_from_pwm(pwm,
-                                                               parameters.core_gaps)
+                                                                    parameters.core_gaps)
         core_absolute_start = core_positions[0] + pad_length
         # Pad PWM with equiprobable flanks
         pwm_padded = ctrlf_tf.pwm_utils.pad_pwm_equiprobable(pwm, pad_length)
         pwm_dict = ctrlf_tf.pwm_utils.pwm_ndarray_to_dict(pwm_padded)
-        # Generate aligned kmers and hamming distance graph
+        # Generate aligned kmers
         aligned_kmer_df = ctrlf_tf.pwm_utils.align_kmers_from_df(kmer_df,
-                                                                  pwm_dict,
-                                                                  parameters.palindrome,
-                                                                  core_absolute_start,
-                                                                  rank_score_label)
-        return cls(core_positions,
-                   aligned_kmer_df,
-                   k,
-                   parameters.palindrome,
-                   pwm,
-                   parameters.version,
-                   kmer_df)
+                                                                 pwm_dict,
+                                                                 parameters.palindrome,
+                                                                 core_absolute_start,
+                                                                 rank_score_label)
+        # Generate traversal graph
+        padded_kmers = ctrlf_tf.str_utils.padded_kmers_from_aligned_df(aligned_kmer_df)
+        traversal_graph = ctrlf_tf.str_utils.create_traverse_graph_from_padded_kmers(padded_kmers)
+        return cls(core_positions=core_positions,
+                   aligned_kmer_dataframe=aligned_kmer_df,
+                   k=k,
+                   palindrome=parameters.palindrome,
+                   pwm=pwm,
+                   version=parameters.version,
+                   kmer_dataframe=kmer_df,
+                   traversal_graph=traversal_graph)
 
     @classmethod
     def from_alignment_file(cls, file_path: str):
         """Construct class using a previous AlignedKmers output file.
 
         Parses the information saved from using the method
         *.save_alignment* to make a new class instance.
@@ -246,28 +255,37 @@
             aligned_kmer_data = file_obj.read()
         # Parse parameters in header
         with StringIO(aligned_kmer_data) as data_obj:
             version = data_obj.readline().split(': ')[1].strip()
             palindrome = ctrlf_tf.parse_utils.parse_boolean(data_obj.readline().strip())
             core_positions = ctrlf_tf.parse_utils.parse_core_positions(data_obj.readline().strip())
             pwm = np.loadtxt(data_obj, delimiter='\t', skiprows=1, max_rows=4)
-            # Parse k-mer dataframe
-            aligned_kmer_dataframe = pd.read_csv(data_obj, sep='\t', skiprows=1)
+        dataframe_str, graph_str = aligned_kmer_data.split("#Aligned Kmers\n")[-1].split("#Traversal Graph\n")
+        # Parse k-mer dataframe
+        with StringIO(dataframe_str) as read_obj:
+            aligned_kmer_dataframe = pd.read_csv(read_obj, sep='\t')
+        # Parse Traversal Graph
+        with StringIO(graph_str) as read_obj:
+            adj_lines = []
+            for i in read_obj:
+                adj_lines.append(i.rstrip())
+        traversal_graph = nx.parse_adjlist(adj_lines, nodetype=int)
         # Parse k and max length
         k = ctrlf_tf.str_utils.k_from_kmers(aligned_kmer_dataframe.iloc[:, 0])
         # Return AlignedKmers object
-        return cls(core_positions,
-                   aligned_kmer_dataframe,
-                   k,
-                   palindrome,
-                   pwm,
-                   version)
+        return cls(core_positions=core_positions,
+                   aligned_kmer_dataframe=aligned_kmer_dataframe,
+                   k=k,
+                   palindrome=palindrome,
+                   pwm=pwm,
+                   version=version,
+                   traversal_graph=traversal_graph)
 
     def copy(self):
-        """Create a deep copy of the AlignedKmers object."""
+        """Create a deep copy of the object."""
         return copy.deepcopy(self)
 
     # Public instance methods
     def save_alignment(self, location: str = None):
         """Save alignment data to stdout or a file.
 
         :param location: Output location, if None output will be stdout
@@ -290,60 +308,84 @@
         np.savetxt(output_file_object, self.pwm, delimiter='\t')
         # Write the aligned kmers
         output_file_object.write("#Aligned Kmers\n")
         # Set Align_Score to scientific notation for output
         output_df = self.aligned_kmer_dataframe.copy(deep=True)
         output_df["Align_Score"] = output_df["Align_Score"].apply(lambda x: "{:e}".format(x))
         output_df.to_csv(output_file_object, sep='\t', index=False)
+        # Save Traversal Graph to File
+        output_file_object.write("#Traversal Graph\n")
+        for line in nx.generate_adjlist(self.traversal_graph):
+            output_file_object.write(f"{line}\n")
         # Close file object if needed
         if location != sys.stdout:
             output_file_object.close()
 
-
-class CompiledKmers(AlignedKmers):
-    """Compiles aligned k-mers into consensus sites.
-
-    This class is a child class of AlignedKmers that compiles the
-    k-mers into consensus sites are part of the initialization
-    process. The class also defines how compiled sites are saved
-    and loaded to populate a new CompiledKmers object.
-    """
+class CtrlF(AlignedKmers):
+    """"""
     def __init__(self,
                  core_positions: Tuple[int] = None,
                  aligned_kmer_dataframe: pd.DataFrame = None,
                  k: int = None,
                  palindrome: bool = None,
                  pwm: np.ndarray = None,
                  version: str = None,
                  kmer_dataframe: pd.DataFrame = None,
+                 traversal_graph: nx.Graph = None,
                  compiled_site_dataframe: pd.DataFrame = None,
                  abs_core_start: int = None,
-                 abs_core_end: int = None):
+                 abs_core_end: int = None,
+                 is_compiled: bool = False):
         super().__init__(core_positions=core_positions,
                          aligned_kmer_dataframe=aligned_kmer_dataframe,
                          k=k,
                          palindrome=palindrome,
                          pwm=pwm,
                          version=version,
-                         kmer_dataframe=kmer_dataframe)
+                         kmer_dataframe=kmer_dataframe,
+                         traversal_graph=traversal_graph)
+        # General attributes
+        self.is_compiled = is_compiled
+        # Compiled Solution-Specific Items
         self.compiled_site_dataframe = compiled_site_dataframe
         self.abs_core_start = abs_core_start
         self.abs_core_end = abs_core_end
-        if self.compiled_site_dataframe is None:
-            # Generate compiled sequences
-            self.compiled_site_dataframe = ctrlf_tf.compile_utils.compile_consensus_sites(self.aligned_kmer_dataframe, self.core_positions)
-            # Trim edges to minimal bounds
-            left_idx, right_idx = ctrlf_tf.compile_utils.bounds_from_aligned_sequences(self.compiled_site_dataframe[ctrlf_tf.compile_utils.COMPILED_LABEL])
-            self.compiled_site_dataframe[ctrlf_tf.compile_utils.COMPILED_LABEL] = self.compiled_site_dataframe[ctrlf_tf.compile_utils.COMPILED_LABEL].apply(lambda x: x[left_idx:right_idx])
-        if self.abs_core_start is None and self.abs_core_end is None:
-            self.abs_core_start = abs(min(self.aligned_kmer_dataframe["Align_Position"])) + 1 - left_idx
-            self.abs_core_end = self.abs_core_start + max(self.core_positions)
-        if self.abs_core_start is None or self.abs_core_end is None:
-            raise ValueError("CompiledKmers object initialize with 1 of [abs_core_start, abs_core_end]. Must specify neither or both.")
+        if self.is_compiled:
+            self._update_compile_search_items()
+        # Non-compiled Search Items
+        if self.is_compiled is False:
+            self._update_noncompile_search_items()
+
+    def _update_compile_search_items(self):
+        """If compiled solutions are available, update necessary search items"""
+        self._site_len = ctrlf_tf.str_utils.total_length_aligned_strs(self.compiled_site_dataframe[ctrlf_tf.compile_utils.COMPILED_LABEL])
+        self.site_span = self._site_len - 1
         self.core_span = self.abs_core_end - self.abs_core_start
+        self._internal_cs_df = self.compiled_site_dataframe.copy(deep=True)
+        self._internal_cs_df["Site_End_Pos"] = self._internal_cs_df[ctrlf_tf.compile_utils.COMPILED_LABEL].apply(lambda x: ctrlf_tf.str_utils.relative_end_positions(x))
+        self._internal_cs_df["Core_End_Pos"] = self._internal_cs_df[ctrlf_tf.compile_utils.COMPILED_LABEL].apply(lambda x: ctrlf_tf.str_utils.relative_end_positions(x, start_position=self.abs_core_start - 1))
+        self._internal_cs_df["Search_Sites"] = self._internal_cs_df[ctrlf_tf.compile_utils.COMPILED_LABEL].apply(lambda x: x.strip('.'))
+        self.compile_automata = ctrlf_tf.site_call_utils.automata_from_sites(self._internal_cs_df["Search_Sites"])
+        self.fixed_length_search_dict = ctrlf_tf.site_call_utils.compiled_dict_from_compiled_sequences(self._internal_cs_df["Search_Sites"],
+                                                                                                       self._internal_cs_df["Site_End_Pos"],
+                                                                                                       self._internal_cs_df["Rank_Score"])
+        self.variable_length_search_dict = ctrlf_tf.site_call_utils.compiled_dict_from_compiled_sequences(self._internal_cs_df["Search_Sites"],
+                                                                                                          self._internal_cs_df["Core_End_Pos"],
+                                                                                                          self._internal_cs_df["Rank_Score"])
+        self.is_compiled = True
+
+    def compile_all_solutions(self):
+        """Generates all possible solutions as ranked patterns (in place)."""
+        self.compiled_site_dataframe = ctrlf_tf.compile_utils.compile_consensus_sites(self.aligned_kmer_dataframe, self.core_positions)
+        # Trim edges to minimal bounds
+        left_idx, right_idx = ctrlf_tf.compile_utils.bounds_from_aligned_sequences(self.compiled_site_dataframe[ctrlf_tf.compile_utils.COMPILED_LABEL])
+        self.compiled_site_dataframe[ctrlf_tf.compile_utils.COMPILED_LABEL] = self.compiled_site_dataframe[ctrlf_tf.compile_utils.COMPILED_LABEL].apply(lambda x: x[left_idx:right_idx])
+        self.abs_core_start = abs(min(self.aligned_kmer_dataframe["Align_Position"])) + 1 - left_idx
+        self.abs_core_end = self.abs_core_start + max(self.core_positions)
+        self._update_compile_search_items()
 
     def save_compiled_sites(self, output=None, minimal=True):
         """Saves compiled sites as a table to a file or stdout.
 
         :param output: Output location (default = stdout)
         :type output: str
         :param minimal: If *true*, removes column showing which kmer indexes
@@ -383,56 +425,18 @@
             palindrome = ctrlf_tf.parse_utils.parse_orientation_bool(file_obj.readline().rstrip())
             abs_core_start, abs_core_end = ctrlf_tf.parse_utils.parse_integer_parameters(file_obj.readline())
             compiled_site_df = pd.read_csv(file_obj, sep='\t')
         return cls(version=version,
                    palindrome=palindrome,
                    abs_core_start=abs_core_start,
                    abs_core_end=abs_core_end,
-                   compiled_site_dataframe=compiled_site_df)
-
+                   compiled_site_dataframe=compiled_site_df,
+                   is_compiled=True)
 
-class CtrlF(CompiledKmers):
-    """Class used to align, compile, and call sites."""
-    def __init__(self,
-                 core_positions: Tuple[int] = None,
-                 aligned_kmer_dataframe: pd.DataFrame = None,
-                 k: int = None,
-                 palindrome: bool = None,
-                 pwm: np.ndarray = None,
-                 version: str = None,
-                 kmer_dataframe: pd.DataFrame = None,
-                 compiled_site_dataframe: pd.DataFrame = None,
-                 abs_core_start: int = None,
-                 abs_core_end: int = None):
-        super().__init__(core_positions=core_positions,
-                         aligned_kmer_dataframe=aligned_kmer_dataframe,
-                         k=k,
-                         palindrome=palindrome,
-                         pwm=pwm,
-                         version=version,
-                         kmer_dataframe=kmer_dataframe,
-                         compiled_site_dataframe=compiled_site_dataframe,
-                         abs_core_start=abs_core_start,
-                         abs_core_end=abs_core_end)
-        # Setup internal copy with end positions for rigid and flexible searches.
-        self._site_len = ctrlf_tf.str_utils.total_length_aligned_strs(self.compiled_site_dataframe[ctrlf_tf.compile_utils.COMPILED_LABEL])
-        self.site_span = self._site_len - 1
-        self._internal_cs_df = self.compiled_site_dataframe.copy(deep=True)
-        self._internal_cs_df["Site_End_Pos"] = self._internal_cs_df[ctrlf_tf.compile_utils.COMPILED_LABEL].apply(lambda x: ctrlf_tf.str_utils.relative_end_positions(x))
-        self._internal_cs_df["Core_End_Pos"] = self._internal_cs_df[ctrlf_tf.compile_utils.COMPILED_LABEL].apply(lambda x: ctrlf_tf.str_utils.relative_end_positions(x, start_position=self.abs_core_start - 1))
-        self._internal_cs_df["Search_Sites"] = self._internal_cs_df[ctrlf_tf.compile_utils.COMPILED_LABEL].apply(lambda x: x.strip('.'))
-        self.automata = ctrlf_tf.site_call_utils.automata_from_sites(self._internal_cs_df["Search_Sites"])
-        self.fixed_length_search_dict = ctrlf_tf.site_call_utils.compiled_dict_from_compiled_sequences(self._internal_cs_df["Search_Sites"],
-                                                                                                self._internal_cs_df["Site_End_Pos"],
-                                                                                                self._internal_cs_df["Rank_Score"])
-        self.variable_length_search_dict = ctrlf_tf.site_call_utils.compiled_dict_from_compiled_sequences(self._internal_cs_df["Search_Sites"],
-                                                                                                   self._internal_cs_df["Core_End_Pos"],
-                                                                                                   self._internal_cs_df["Rank_Score"])
-
-    def call_sites(self, sequence: str, fixed_length=True):
+    def _call_sites_with_compiled_solutions(self, sequence: str, fixed_length=True):
         """Returns a list of SiteTuples from an input sequence.
 
         Given a sequence, returns a list of SiteTuples for each called site.
 
         :param sequence: Input DNA sequence
         :type sequence: str
         :param fixed_length: Search mode assumes a fixed model length
@@ -445,26 +449,77 @@
         compiled_site_dict = self.fixed_length_search_dict
         site_span = self.site_span
         if not fixed_length:
             compiled_site_dict = self.variable_length_search_dict
             site_span = self.core_span
         # Call sites from the input sequence orientation, if palindrome return the results
         orient1 = ctrlf_tf.site_call_utils.site_dict_from_sequence(sequence,
-                                                                   self.automata,
+                                                                   self.compile_automata,
                                                                    compiled_site_dict)
         if self.palindrome:
             return ctrlf_tf.site_call_utils.site_dict_to_sitetuples(orient1, sequence, '.', site_span)
         # Otherwise call sites on the reverse complement and return results from both orientations
         orient2 = ctrlf_tf.site_call_utils.site_dict_from_sequence(ctrlf_tf.str_utils.reverse_complement(sequence),
-                                                                   self.automata,
+                                                                   self.compile_automata,
                                                                    compiled_site_dict)
         pos_sites = ctrlf_tf.site_call_utils.site_dict_to_sitetuples(orient1, sequence, '+', site_span)
         neg_sites = ctrlf_tf.site_call_utils.site_dict_to_sitetuples(orient2, sequence, '-', site_span)
         return pos_sites + neg_sites
 
+    def _update_noncompile_search_items(self):
+        """Update attributes required for k-mer based search."""
+        self.index_to_score_dict = ctrlf_tf.site_call_utils.index_to_score_dict_from_aligned_df(self.aligned_kmer_dataframe)
+        self.kmer_to_index_dict = ctrlf_tf.site_call_utils.kmer_to_index_dict_from_aligned_df(self.aligned_kmer_dataframe)
+        self.index_to_core_position_dict = ctrlf_tf.site_call_utils.kmer_idx_to_core_position_dict_from_aligned_df(self.aligned_kmer_dataframe, self.core_positions)
+        self.expanded_kmer_to_original_dict = ctrlf_tf.site_call_utils.expanded_kmer_to_original_dict_from_aligned_df(self.aligned_kmer_dataframe)
+        self.kmer_automata = ctrlf_tf.site_call_utils.automata_from_sites(list(self.expanded_kmer_to_original_dict.keys()))
+        self.site_span = max(self.core_positions)
+
+    def _call_sites_with_kmers(self, sequence: str):
+        """Returns a list of SiteTuples from an input sequence.
+
+        Given a sequence, returns a list of SiteTuples for each called site.
+
+        :param sequence: Input DNA sequence
+        :type sequence: str
+        :param fixed_length: Search mode assumes a fixed model length
+        :type fixed_length: bool
+        :returns: List of SiteTuples
+        """
+        # Set sequence to uppercase so match is case insensisitivw
+        sequence = sequence.upper()
+        # Call sites from the input sequence orientation, if palindrome return the results
+        orient1 = ctrlf_tf.site_call_utils.site_dict_noncompiled_from_sequence(sequence,
+                                                                               self.kmer_automata,
+                                                                               self.expanded_kmer_to_original_dict,
+                                                                               self.kmer_to_index_dict,
+                                                                               self.index_to_score_dict,
+                                                                               self.traversal_graph,
+                                                                               self.index_to_core_position_dict)
+        if self.palindrome:
+            return ctrlf_tf.site_call_utils.site_dict_to_sitetuples(orient1, sequence, '.', self.site_span)
+        # Otherwise call sites on the reverse complement and return results from both orientations
+        orient2 = ctrlf_tf.site_call_utils.site_dict_noncompiled_from_sequence(ctrlf_tf.str_utils.reverse_complement(sequence),
+                                                      self.kmer_automata,
+                                                      self.expanded_kmer_to_original_dict,
+                                                      self.kmer_to_index_dict,
+                                                      self.index_to_score_dict,
+                                                      self.traversal_graph,
+                                                      self.index_to_core_position_dict)
+        pos_sites = ctrlf_tf.site_call_utils.site_dict_to_sitetuples(orient1, sequence, '+', self.site_span)
+        neg_sites = ctrlf_tf.site_call_utils.site_dict_to_sitetuples(orient2, sequence, '-', self.site_span)
+        return pos_sites + neg_sites
+
+
+    def call_sites(self, sequence: str):
+        if self.is_compiled:
+            return self._call_sites_with_compiled_solutions(sequence)
+        else:
+            return self._call_sites_with_kmers(sequence)
+
     def call_sites_as_bed(self,
                           sequence: str,
                           chromosome: str,
                           chromosome_start: int,
                           fixed_length=True):
         """Call sites in BED format.
 
@@ -475,15 +530,15 @@
         :type sequence: str
         :param chromosome: Chromosome label
         :type chromosome: str
         :param chromosome_start: Start position of the input sequence
         :type chromosome_start: int
         :returns: List of BedTuples
         """
-        sites = self.call_sites(sequence, fixed_length)
+        sites = self.call_sites(sequence)
         chromosome_end = chromosome_start + len(sequence)
         bedtuple_result = ctrlf_tf.site_call_utils.site_tuples_to_bed(sites,
                                                                       chromosome,
                                                                       chromosome_start,
                                                                       chromosome_end)
         return bedtuple_result
```

### Comparing `CtrlF_TF-1.0b3/src/ctrlf_tf/optimize_core.py` & `CtrlF_TF-1.0b4/src/ctrlf_tf/optimize_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -309,25 +309,28 @@
             dataframe_strings.split("#Classified_Dataframe:\n")
         classified_df_string, tpr_fpr_string = \
             dataframe_strings.split("#TPR_FPR_Dataframe:\n")
         # Parse classified debruijn and parameter dataframes
         classified_dataframe = pd.read_csv(StringIO(classified_df_string), sep='\t')
         parameter_dataframe = pd.read_csv(StringIO(parameters_string),
                                           sep='\t')
+        # Convert empty list into list instead of a string
+        parameter_dataframe["Core_Gaps"] = parameter_dataframe["Core_Gaps"].apply(lambda x: ctrlf_tf.parse_utils.parse_parameter_str("Core_Gaps", x))
         # Parse tpr_fpr_dictionary from dataframe
         tpr_fpr_dataframe = pd.read_csv(StringIO(tpr_fpr_string), sep='\t')
         tpr_fpr_dictionary = {}
         for key, dataframe in tpr_fpr_dataframe.groupby(by="ID"):
             tpr_fpr_dictionary[key] = dataframe
         # Return class instance
         return cls(align_parameters=init_parameters,
                    classified_df=classified_dataframe,
                    fpr_threshold=fpr_threshold,
                    parameter_dataframe=parameter_dataframe,
-                   tpr_fpr_dictionary=tpr_fpr_dictionary)
+                   tpr_fpr_dictionary=tpr_fpr_dictionary,
+                   optimal_parameters=ctrlf_tf.optimize_utils.optimal_parameters_from_df(parameter_dataframe, init_parameters))
 
     def save_to_file(self, file_path: str):
         """Save optimized parameter information to a text file.
 
         The saved file contains the attributes of the Optimize object,
         including:
         1) Inital AlignParameter
```

### Comparing `CtrlF_TF-1.0b3/src/ctrlf_tf/optimize_utils.py` & `CtrlF_TF-1.0b4/src/ctrlf_tf/optimize_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,27 +229,27 @@
 def tpr_fpr_df_from_parameters(parameters, classified_df) -> float:
     """AUROC from parameters.
 
     Given a start, end, core_gaps, and gap_number, returns a
     AUROC for the parameter set.
     """
     try:
-        ak_obj = ctrlf_tf.ctrlf_core.AlignedKmers.from_parameters(parameters)
+        ctrlf_obj = ctrlf_tf.ctrlf_core.CtrlF.from_parameters(parameters)
     except:
         print("Parameters could not be compiled", parameters, file=sys.stderr)
         raise
-    noncompiled_preprocess = ctrlf_tf.site_call_utils.noncompile_preprocessing_from_aligned_kmers(ak_obj.aligned_kmer_dataframe, ak_obj.core_positions)
-    is_palindrome = parameters.palindrome
+    #noncompiled_preprocess = ctrlf_tf.site_call_utils.noncompile_preprocessing_from_aligned_kmers(ak_obj.aligned_kmer_dataframe, ak_obj.core_positions)
+    #is_palindrome = parameters.palindrome
     scores = []
     site_count = []
     site_scores = []
     site_list = []
     for sequence in classified_df["Sequence"]:
-        sites = ctrlf_tf.site_call_utils.call_sites_with_kmers(sequence, noncompiled_preprocess, is_palindrome)
-        #sites = ctrlf_obj.call_sites(sequence, fixed_length=False)
+        #sites = ctrlf_tf.site_call_utils.call_sites_with_kmers(sequence, noncompiled_preprocess, is_palindrome)
+        sites = ctrlf_obj.call_sites(sequence)
         site_count.append(len(sites))
         if len(sites) == 0:
             scores.append(-math.inf)
             site_scores.append([-math.inf])
             site_list.append([''])
         else:
             site_scores.append(sites)
```

### Comparing `CtrlF_TF-1.0b3/src/ctrlf_tf/parse_utils.py` & `CtrlF_TF-1.0b4/src/ctrlf_tf/parse_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Functions for parsing files."""
 
 from typing import Iterable, Tuple
 import re
 
 import pandas as pd
+import networkx as nx
 
 
 def parse_k(kmer: str) -> int:
     """Return k from a kmer with 0 or more gaps."""
     return len(kmer.replace('.', ''))
 
 def parse_integer_parameters(parameter_str):
@@ -203,19 +204,24 @@
 def parse_parameter_str(label, value):
     # Convert boolean str to bool
     if value == "True":
         return True
     if value == "False":
         return False
     if label == "threshold":
+        if value == "None":
+            return None
         return float(value)
     if label in ("core_start", "core_end", "gap_limit"):
         return int(value)
     if value[0] == '[' and value[-1] == ']':
-        return [int(i) for i in value[1:-1].split()]
+        if value == '[]':
+            return []
+        else:
+            return [int(i) for i in value[1:-1].split()]
     return value
 
 def parameter_dict_from_strs(strs):
     param_dict = {}
     for line in strs:
         label, value = line.split(": ")
         label = label.lstrip("#")
```

### Comparing `CtrlF_TF-1.0b3/src/ctrlf_tf/pwm_utils.py` & `CtrlF_TF-1.0b4/src/ctrlf_tf/pwm_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,14 +190,15 @@
                       core_range,
                       core_gaps):
     """Trim a PWM model by core definitions."""
     start_idx = core_range[0] - 1
     end_idx = core_range[1]
     pwm = pwm[:, start_idx:end_idx]
     if core_gaps:
+        print("CORE GAPS:", core_gaps, type(core_gaps))
         for i in core_gaps:
             pwm[:, i-1] = 0.25
     return pwm
 
 
 def trim_pwm_wrapper(pwm: np.ndarray,
                      core_range: tuple = None,
```

### Comparing `CtrlF_TF-1.0b3/src/ctrlf_tf/site_call_utils.py` & `CtrlF_TF-1.0b4/src/ctrlf_tf/site_call_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python3
+"""Site calling utilites."""
 
 from collections import namedtuple, defaultdict
 from typing import Iterable, List
 
 import ahocorasick
 import ctrlf_tf.str_utils
 import ctrlf_tf.compile_utils
@@ -210,15 +210,15 @@
 def padded_kmers_from_aligned_df(aligned_df):
     """Return padded k-mers from an aligned k-mer dataframe"""
     kmer_dataframe = aligned_df.drop_duplicates().reset_index(drop=True)
     # Calculate bounds
     kmers = kmer_dataframe.iloc[:, 0]
     max_word_len = max([len(kmer) for kmer in kmer_dataframe.iloc[:, 0]])
     aligned_positions = kmer_dataframe.iloc[:, 1]
-    left_bound, right_bound = ctrlf_tf.compile_utils.bounds_from_aligned_positions(aligned_positions, max_word_len)
+    left_bound, right_bound = ctrlf_tf.str_utils.bounds_from_aligned_positions(aligned_positions, max_word_len)
     # Pad k-mers relative to bounds
     padded_kmers = []
     for row in kmer_dataframe.itertuples():
         padded_kmer = pad_k(row.Kmer, row.Align_Position, left_bound, right_bound)
         padded_kmers.append(padded_kmer)
     return padded_kmers
 
@@ -301,32 +301,38 @@
         if len(i) > 1:
             connected_groups.append(list(i))
     return connected_groups
 
 def score_site_from_candidate_list(candidate_list,
                                    index_to_score_dict,
                                    traversal_graph,
-                                   kmer_idx_to_core_position_dict):
-    """Current method = N2, could be NlogN"""
-    candidate_list = sorted(candidate_list)
-    kmer_idx_set = set()
-    kmer_idx_set.add(candidate_list[0])
-    for idx in range(2, len(candidate_list[1:])):
-        candidate_indexes = candidate_list[:idx]
-        kmer_idx_set.add(candidate_list[idx - 1])
-        # Check for connected groups
-        for connected_groups in overlapping_kmers(traversal_graph, kmer_idx_set):
-            core_descriptions = [kmer_idx_to_core_position_dict[i] for i in connected_groups]
-            if ctrlf_tf.compile_utils.is_core_described(core_descriptions):
-                return index_to_score_dict[candidate_indexes[-1]]
+                                   kmer_idx_to_core_position_dict) -> float:
+    """Determine if a candidate site is real and score if so.
+    
+    Given a list of candidate kmer indicies (variable) and information from
+    the alignment of k-mers (index_to_score_dict, traversal_graph,
+    kmer_idx_to_core_position_dict), finds the maximum k-mer score of a valid
+    solution. If there is one, returns the score. Otherwise, returns None. 
+    """
+    # List of candidate kmer indicies (equivalent to their ranks)
+    if len(candidate_list) >= 2: # If there are the minimum number of k-mers or more
+        # Sort the lists by rank in increasing order
+        candidate_list = sorted(candidate_list)
+        # Iteratively add to the set
+        kmer_idx_set = set()
+        kmer_idx_set.add(candidate_list[0])
+        for i in candidate_list[1:]:
+            kmer_idx_set.add(i)
+            # For each addition, check if there is an answer and if so return its score
+            for connected_groups in overlapping_kmers(traversal_graph, kmer_idx_set):
+                core_descriptions = [kmer_idx_to_core_position_dict[i] for i in connected_groups]
+                if ctrlf_tf.compile_utils.is_core_described(core_descriptions):
+                    return index_to_score_dict[i]
     return None
 
-# Search a string for all matches
-
-
 
 NonCompilePreprocess = namedtuple("NonCompilePreprocess", ["kmer_automata",
                                                            "expanded_kmer_to_original_dict",
                                                            "kmer_to_index_dict",
                                                            "index_to_score_dict",
                                                            "index_to_core_position_dict",
                                                            "traversal_graph",
@@ -347,29 +353,49 @@
                                 index_to_score_dict,
                                 index_to_core_position_dict,
                                 traverse_graph,
                                 site_span)
 
 
 def site_dict_noncompiled_from_sequence(sequence,
-                                        noncompilepreprocess):
+                                        automata,
+                                        expanded_kmer_to_original_dict,
+                                        kmer_to_index_dict,
+                                        index_to_score_dict,
+                                        traversal_graph,
+                                        index_to_core_position_dict):
+    """From a string, return a dictionary of binding sites (keys) and their scores (values).
+    
+    Given a DNA sequence to search for binding sites, returns a dictionary where the keys 
+    are positions of the binding sites and the values are the scores. This is done by first
+    running the aho-corasick automata to find all possible matches of k-mers. Then, for all
+    groups of candidate sites, they are evaluated and scored. 
+    """
     candidate_site_dict = defaultdict(list)
-    for match in noncompilepreprocess.kmer_automata.iter(sequence):
+    # For each match from the automata match iterator:
+    for match in automata.iter(sequence):
+        # parse the sequence and position of the k-mer
         match_sequence = match[1][1]
+        # match[0] will be for the end of the matched string
+        # This adjusts to have match_position at the start
         match_position = match[0] - len(match_sequence) + 1
-        for original_kmer in noncompilepreprocess.expanded_kmer_to_original_dict[match_sequence]:
-            align_position = noncompilepreprocess.expanded_kmer_to_original_dict[match_sequence][original_kmer]
+        # Expand the k-mers to account for gapped k-mers (1-1 if no-gap else 1-many)
+        for original_kmer in expanded_kmer_to_original_dict[match_sequence]:
+            align_position = expanded_kmer_to_original_dict[match_sequence][original_kmer]
+            # Determine where the binding site is relative to the k-mer match
             rel_core = (align_position * -1) + match_position
-            candidate_site_dict[rel_core].append(noncompilepreprocess.kmer_to_index_dict[original_kmer][align_position])
-    site_dict = {}
+            # Then associate the k-mer with that site
+            candidate_site_dict[rel_core].append(kmer_to_index_dict[original_kmer][align_position])
+    site_dict = {} # Dictionary of binding sites
     for i in candidate_site_dict:
+        # Score the candidate site and if it is valid, add it to the site dictionary
         score = score_site_from_candidate_list(candidate_site_dict[i],
-                                               noncompilepreprocess.index_to_score_dict,
-                                               noncompilepreprocess.traversal_graph,
-                                               noncompilepreprocess.index_to_core_position_dict)
+                                               index_to_score_dict,
+                                               traversal_graph,
+                                               index_to_core_position_dict)
         if score is not None:
             site_dict[i] = score
     return site_dict
 
 
 def call_sites_with_kmers(sequence: str, noncompilepreprocess, is_palindrome):
     """Returns a list of SiteTuples from an input sequence.
```

### Comparing `CtrlF_TF-1.0b3/src/ctrlf_tf/threshold_utils.py` & `CtrlF_TF-1.0b4/src/ctrlf_tf/threshold_utils.py`

 * *Files identical despite different names*

### Comparing `CtrlF_TF-1.0b3/tests/test_str_utils.py` & `CtrlF_TF-1.0b4/tests/test_str_utils.py`

 * *Files identical despite different names*

