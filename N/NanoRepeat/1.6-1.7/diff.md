# Comparing `tmp/NanoRepeat-1.6.tar.gz` & `tmp/NanoRepeat-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NanoRepeat-1.6.tar", last modified: Sun Jun  4 11:28:52 2023, max compression
+gzip compressed data, was "NanoRepeat-1.7.tar", last modified: Sat Jun 17 08:00:24 2023, max compression
```

## Comparing `NanoRepeat-1.6.tar` & `NanoRepeat-1.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 fangli    (1002) fangli    (1002)        0 2023-06-04 11:28:52.334905 NanoRepeat-1.6/
--rw-rw-r--   0 fangli    (1002) fangli    (1002)     1097 2023-05-11 08:33:58.000000 NanoRepeat-1.6/LICENSE
--rw-rw-r--   0 fangli    (1002) fangli    (1002)    16291 2023-06-04 11:28:52.334905 NanoRepeat-1.6/PKG-INFO
--rw-rw-r--   0 fangli    (1002) fangli    (1002)    15958 2023-05-17 14:33:11.000000 NanoRepeat-1.6/README.md
--rw-rw-r--   0 fangli    (1002) fangli    (1002)       38 2023-06-04 11:28:52.334905 NanoRepeat-1.6/setup.cfg
--rw-rw-r--   0 fangli    (1002) fangli    (1002)      801 2023-06-04 10:48:01.000000 NanoRepeat-1.6/setup.py
-drwxrwxr-x   0 fangli    (1002) fangli    (1002)        0 2023-06-04 11:28:52.330905 NanoRepeat-1.6/src/
-drwxrwxr-x   0 fangli    (1002) fangli    (1002)        0 2023-06-04 11:28:52.330905 NanoRepeat-1.6/src/NanoRepeat/
--rw-rw-r--   0 fangli    (1002) fangli    (1002)      186 2023-05-11 08:33:58.000000 NanoRepeat-1.6/src/NanoRepeat/__init__.py
--rwxrwxr-x   0 fangli    (1002) fangli    (1002)    36432 2023-05-13 06:07:32.000000 NanoRepeat-1.6/src/NanoRepeat/nanoRepeat-joint.py
--rwxrwxr-x   0 fangli    (1002) fangli    (1002)    10989 2023-05-22 01:41:48.000000 NanoRepeat-1.6/src/NanoRepeat/nanoRepeat.py
--rw-rw-r--   0 fangli    (1002) fangli    (1002)    32046 2023-06-04 10:45:36.000000 NanoRepeat-1.6/src/NanoRepeat/nanoRepeat_bam.py
--rw-rw-r--   0 fangli    (1002) fangli    (1002)     3078 2023-05-13 06:08:14.000000 NanoRepeat-1.6/src/NanoRepeat/paf.py
--rw-rw-r--   0 fangli    (1002) fangli    (1002)     4487 2023-06-03 08:25:19.000000 NanoRepeat-1.6/src/NanoRepeat/repeat_region.py
--rw-rw-r--   0 fangli    (1002) fangli    (1002)    31135 2023-05-14 07:24:25.000000 NanoRepeat-1.6/src/NanoRepeat/split_alleles.py
--rw-rw-r--   0 fangli    (1002) fangli    (1002)    16195 2023-05-17 13:58:21.000000 NanoRepeat-1.6/src/NanoRepeat/tk.py
-drwxrwxr-x   0 fangli    (1002) fangli    (1002)        0 2023-06-04 11:28:52.334905 NanoRepeat-1.6/src/NanoRepeat.egg-info/
--rw-rw-r--   0 fangli    (1002) fangli    (1002)    16291 2023-06-04 11:28:52.000000 NanoRepeat-1.6/src/NanoRepeat.egg-info/PKG-INFO
--rw-rw-r--   0 fangli    (1002) fangli    (1002)      446 2023-06-04 11:28:52.000000 NanoRepeat-1.6/src/NanoRepeat.egg-info/SOURCES.txt
--rw-rw-r--   0 fangli    (1002) fangli    (1002)        1 2023-06-04 11:28:52.000000 NanoRepeat-1.6/src/NanoRepeat.egg-info/dependency_links.txt
--rw-rw-r--   0 fangli    (1002) fangli    (1002)       53 2023-06-04 11:28:52.000000 NanoRepeat-1.6/src/NanoRepeat.egg-info/requires.txt
--rw-rw-r--   0 fangli    (1002) fangli    (1002)       11 2023-06-04 11:28:52.000000 NanoRepeat-1.6/src/NanoRepeat.egg-info/top_level.txt
+drwxrwxr-x   0 fangli    (1002) fangli    (1002)        0 2023-06-17 08:00:24.676031 NanoRepeat-1.7/
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)     1097 2023-06-17 07:53:23.000000 NanoRepeat-1.7/LICENSE
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)    16291 2023-06-17 08:00:24.676031 NanoRepeat-1.7/PKG-INFO
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)    15958 2023-06-17 07:53:23.000000 NanoRepeat-1.7/README.md
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)       38 2023-06-17 08:00:24.676031 NanoRepeat-1.7/setup.cfg
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)      801 2023-06-17 07:59:49.000000 NanoRepeat-1.7/setup.py
+drwxrwxr-x   0 fangli    (1002) fangli    (1002)        0 2023-06-17 08:00:24.672031 NanoRepeat-1.7/src/
+drwxrwxr-x   0 fangli    (1002) fangli    (1002)        0 2023-06-17 08:00:24.676031 NanoRepeat-1.7/src/NanoRepeat/
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)      186 2023-06-17 07:53:23.000000 NanoRepeat-1.7/src/NanoRepeat/__init__.py
+-rwxrwxr-x   0 fangli    (1002) fangli    (1002)    36432 2023-06-17 07:53:23.000000 NanoRepeat-1.7/src/NanoRepeat/nanoRepeat-joint.py
+-rwxrwxr-x   0 fangli    (1002) fangli    (1002)    11145 2023-06-17 07:53:23.000000 NanoRepeat-1.7/src/NanoRepeat/nanoRepeat.py
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)    32156 2023-06-17 07:53:23.000000 NanoRepeat-1.7/src/NanoRepeat/nanoRepeat_bam.py
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)     3078 2023-06-17 07:53:23.000000 NanoRepeat-1.7/src/NanoRepeat/paf.py
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)     4487 2023-06-17 07:53:23.000000 NanoRepeat-1.7/src/NanoRepeat/repeat_region.py
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)    31135 2023-06-17 07:53:23.000000 NanoRepeat-1.7/src/NanoRepeat/split_alleles.py
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)    16195 2023-06-17 07:53:23.000000 NanoRepeat-1.7/src/NanoRepeat/tk.py
+drwxrwxr-x   0 fangli    (1002) fangli    (1002)        0 2023-06-17 08:00:24.676031 NanoRepeat-1.7/src/NanoRepeat.egg-info/
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)    16291 2023-06-17 08:00:24.000000 NanoRepeat-1.7/src/NanoRepeat.egg-info/PKG-INFO
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)      446 2023-06-17 08:00:24.000000 NanoRepeat-1.7/src/NanoRepeat.egg-info/SOURCES.txt
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)        1 2023-06-17 08:00:24.000000 NanoRepeat-1.7/src/NanoRepeat.egg-info/dependency_links.txt
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)       53 2023-06-17 08:00:24.000000 NanoRepeat-1.7/src/NanoRepeat.egg-info/requires.txt
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)       11 2023-06-17 08:00:24.000000 NanoRepeat-1.7/src/NanoRepeat.egg-info/top_level.txt
```

### Comparing `NanoRepeat-1.6/LICENSE` & `NanoRepeat-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `NanoRepeat-1.6/PKG-INFO` & `NanoRepeat-1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NanoRepeat
-Version: 1.6
+Version: 1.7
 Summary: NanoRepeat: quantification of Short Tandem Repeats (STRs) from long-read sequencing data
 Home-page: https://github.com/WGLab/NanoRepeat
 Author: Li Fang, Kai Wang
 Author-email: fangli9@sysu.edu.cn
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NanoRepeat-1.6/README.md` & `NanoRepeat-1.7/README.md`

 * *Files identical despite different names*

### Comparing `NanoRepeat-1.6/setup.py` & `NanoRepeat-1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     readme = f.read()
     
 setup(
     name='NanoRepeat',
-    version='1.6',
+    version='1.7',
     description='NanoRepeat: quantification of Short Tandem Repeats (STRs) from long-read sequencing data',
     long_description = readme,
     long_description_content_type = 'text/markdown',
     url='https://github.com/WGLab/NanoRepeat',
     author='Li Fang, Kai Wang',
     author_email='fangli9@sysu.edu.cn',
     license='MIT',
```

### Comparing `NanoRepeat-1.6/src/NanoRepeat/nanoRepeat-joint.py` & `NanoRepeat-1.7/src/NanoRepeat/nanoRepeat-joint.py`

 * *Files identical despite different names*

### Comparing `NanoRepeat-1.6/src/NanoRepeat/nanoRepeat.py` & `NanoRepeat-1.7/src/NanoRepeat/nanoRepeat.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,14 +130,15 @@
     parser.add_argument('-c', '--num_cpu', required = False, metavar = 'INT',   type = int, default = 1,  help ='(optional) number of CPU cores (default: 1)')
     parser.add_argument('--samtools', required = False, metavar = 'path/to/samtools',  type = str, default = 'samtools', help ='(optional) path to samtools (default: using environment default)')
     parser.add_argument('--minimap2', required = False, metavar = 'path/to/minimap2',  type = str, default = 'minimap2', help ='(optional) path to minimap2 (default: using environment default)')
     parser.add_argument('--ploidy',   required = False, metavar = 'INT', type = int, default = 2,  help ='(optional) ploidy of the sample (default: 2)')
     parser.add_argument('--anchor_len', required = False, metavar = 'INT', type = int, default = 1000, help ='(optional) length of up/downstream sequence to help identify the repeat region (default: 1000 bp, increase this value if the 1000 bp up/downstream sequences are also repeat)')
     parser.add_argument('--max_mutual_overlap', required = False, metavar = 'FLOAT',  type = float, default = 0.15,  help = 'max mutual overlap of two alleles in terms of repeat size distribution (default value: 0.1). If the Gaussian distribution of two alleles have more overlap than this value, the two alleles will be merged into one allele.')
     parser.add_argument('--remove_noisy_reads', required = False, action='store_true', help = 'remove noisy components when there are more components than ploidy')
+    parser.add_argument('--fast_mode', required = False, action='store_true', help = 'fast quantification for repeat size, accuracy may be a little lower')
     parser.add_argument('--save_temp_files', required = False, action='store_true', help = 'save temporary alignment files')
     parser.add_argument('--max_num_components', required = False, metavar = 'INT',  type = int, default = -1,  help = 'max number of components for the Gaussian mixture model (default value: ploidy + 20). Some noisy reads and outlier reads may form a component. Therefore the number of components is usually larger than ploidy. If your sample have too many outlier reads, you can increase this number.')
     
     if len(sys.argv) < 2 or sys.argv[1] in ['help', 'h', '-help', 'usage']:
         input_args = parser.parse_args(['--help'])
     else:
         input_args = parser.parse_args()
```

### Comparing `NanoRepeat-1.6/src/NanoRepeat/nanoRepeat_bam.py` & `NanoRepeat-1.7/src/NanoRepeat/nanoRepeat_bam.py`

 * *Files 0% similar despite different names*

```diff
@@ -520,37 +520,37 @@
             read_paf_list.clear()
             read_paf_list.append(paf)
 
     round3_estimation_for1read(repeat_region, read_paf_list)
     
     return 
 
-def round3_estimation(minimap2:string, data_type:string, repeat_region:RepeatRegion, num_cpu:int):
+def round3_estimation(minimap2:string, data_type:string, fast_mode, repeat_region:RepeatRegion, num_cpu:int):
     
     round3_paf_file = os.path.join(repeat_region.temp_out_dir, 'round3.paf')
     round3_paf_f = open(round3_paf_file, 'w')
     round3_paf_f.close()
     
     procs = []
 
     for proc_id in range(0, num_cpu):
-        proc = Process(target=round3_align_1process, args=(proc_id, num_cpu, repeat_region, data_type, minimap2))
+        proc = Process(target=round3_align_1process, args=(proc_id, num_cpu, fast_mode, repeat_region, data_type, minimap2))
         procs.append(proc)
         proc.start()
         
     for proc_id in range(0, num_cpu):
         procs[proc_id].join()
         proc_out_paf_file = os.path.join(repeat_region.temp_out_dir, f'round3_align.process{proc_id}.paf')
         cmd = f'cat {proc_out_paf_file} >> {round3_paf_file}'
         tk.run_system_cmd(cmd)
         os.remove(proc_out_paf_file)
     
     round3_estimation_from_paf(repeat_region, round3_paf_file)
 
-def round3_align_1process(proc_id:int, num_cpu:int, repeat_region:RepeatRegion, data_type:string, minimap2:string):
+def round3_align_1process(proc_id:int, num_cpu:int, fast_mode, repeat_region:RepeatRegion, data_type:string, minimap2:string):
     
     read_id = -1
     out_paf_file = os.path.join(repeat_region.temp_out_dir, f'round3_align.process{proc_id}.paf')
     out_paf_f = open(out_paf_file, 'w')
     out_paf_f.close()
     
     for read_name in repeat_region.read_dict:
@@ -559,14 +559,17 @@
         if round2_repeat_size == None: continue
         read_id += 1
         if read_id % num_cpu != proc_id: continue
         
         buffer = max(15, int(round2_repeat_size * 0.05))
         if buffer > 150: buffer = 150
         
+        if fast_mode:
+            buffer = 15
+        
         max_template_repeat_size = int(round2_repeat_size + buffer)
         min_template_repeat_size = int(round2_repeat_size - buffer)
         
         if min_template_repeat_size < 0: min_template_repeat_size = 0
         
         template_fasta_file  = os.path.join(repeat_region.temp_out_dir, f'round3_reference.read{read_id}.fasta')
         template_fasta_fp    = open(template_fasta_file, 'w')
@@ -716,15 +719,15 @@
     make_core_seq_fastq(repeat_region)
 
     tk.eprint('NOTICE: Step 2: round 1 and round 2 estimation')
     round1_and_round2_estimation(input_args.minimap2, input_args.data_type, repeat_region, input_args.num_cpu)
     tk.eprint('NOTICE: Step 2 finished')
 
     tk.eprint('NOTICE: Step 3: round 3 estimation')
-    round3_estimation(input_args.minimap2, input_args.data_type, repeat_region, input_args.num_cpu)
+    round3_estimation(input_args.minimap2, input_args.data_type, input_args.fast_mode, repeat_region, input_args.num_cpu)
     tk.eprint('NOTICE: Step 3 finished')
 
     tk.eprint('NOTICE: Writing to repeat size file...')
     output_repeat_size_1d(repeat_region)
 
     tk.eprint('NOTICE: Step 4: phasing reads using GMM')
     split_allele_using_gmm_1d(repeat_region, input_args.ploidy, error_rate, input_args.max_mutual_overlap, input_args.max_num_components, input_args.remove_noisy_reads)
```

### Comparing `NanoRepeat-1.6/src/NanoRepeat/paf.py` & `NanoRepeat-1.7/src/NanoRepeat/paf.py`

 * *Files identical despite different names*

### Comparing `NanoRepeat-1.6/src/NanoRepeat/repeat_region.py` & `NanoRepeat-1.7/src/NanoRepeat/repeat_region.py`

 * *Files identical despite different names*

### Comparing `NanoRepeat-1.6/src/NanoRepeat/split_alleles.py` & `NanoRepeat-1.7/src/NanoRepeat/split_alleles.py`

 * *Files identical despite different names*

### Comparing `NanoRepeat-1.6/src/NanoRepeat/tk.py` & `NanoRepeat-1.7/src/NanoRepeat/tk.py`

 * *Files identical despite different names*

### Comparing `NanoRepeat-1.6/src/NanoRepeat.egg-info/PKG-INFO` & `NanoRepeat-1.7/src/NanoRepeat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NanoRepeat
-Version: 1.6
+Version: 1.7
 Summary: NanoRepeat: quantification of Short Tandem Repeats (STRs) from long-read sequencing data
 Home-page: https://github.com/WGLab/NanoRepeat
 Author: Li Fang, Kai Wang
 Author-email: fangli9@sysu.edu.cn
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

