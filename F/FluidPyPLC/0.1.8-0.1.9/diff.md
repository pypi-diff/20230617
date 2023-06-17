# Comparing `tmp/FluidPyPLC-0.1.8.tar.gz` & `tmp/FluidPyPLC-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FluidPyPLC-0.1.8.tar", last modified: Thu Jun 15 08:39:18 2023, max compression
+gzip compressed data, was "FluidPyPLC-0.1.9.tar", last modified: Sat Jun 17 20:23:52 2023, max compression
```

## Comparing `FluidPyPLC-0.1.8.tar` & `FluidPyPLC-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 08:39:18.397968 FluidPyPLC-0.1.8/
-drwxrwxrwx   0        0        0        0 2023-06-15 08:39:18.359681 FluidPyPLC-0.1.8/FluidPyPLC/
--rw-rw-rw-   0        0        0     7297 2023-06-14 20:24:29.000000 FluidPyPLC-0.1.8/FluidPyPLC/GUI.py
--rw-rw-rw-   0        0        0        0 2023-06-14 20:16:54.000000 FluidPyPLC-0.1.8/FluidPyPLC/__init__.py
--rw-rw-rw-   0        0        0     2770 2023-06-14 09:49:52.000000 FluidPyPLC-0.1.8/FluidPyPLC/data.py
--rw-rw-rw-   0        0        0     3734 2023-06-14 20:26:13.000000 FluidPyPLC-0.1.8/FluidPyPLC/diagrams.py
--rw-rw-rw-   0        0        0     2763 2023-06-15 08:38:30.000000 FluidPyPLC-0.1.8/FluidPyPLC/f.py
--rw-rw-rw-   0        0        0     2342 2023-06-02 12:32:53.000000 FluidPyPLC-0.1.8/FluidPyPLC/get_sequence.py
--rw-rw-rw-   0        0        0    13777 2023-06-02 21:04:22.000000 FluidPyPLC-0.1.8/FluidPyPLC/plc.bak.py
--rw-rw-rw-   0        0        0     9617 2023-06-08 07:50:29.000000 FluidPyPLC-0.1.8/FluidPyPLC/plc.bak2.py
--rw-rw-rw-   0        0        0    14521 2023-06-14 20:24:49.000000 FluidPyPLC-0.1.8/FluidPyPLC/plc.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:39:18.394972 FluidPyPLC-0.1.8/FluidPyPLC/resources/
--rw-rw-rw-   0        0        0       59 2023-06-14 19:54:48.000000 FluidPyPLC-0.1.8/FluidPyPLC/resources/config.json
--rw-rw-rw-   0        0        0      889 2023-06-03 13:58:59.000000 FluidPyPLC-0.1.8/FluidPyPLC/set_groups.py
--rw-rw-rw-   0        0        0     1120 2023-06-03 13:58:52.000000 FluidPyPLC-0.1.8/FluidPyPLC/set_switches.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:39:18.394097 FluidPyPLC-0.1.8/FluidPyPLC.egg-info/
--rw-rw-rw-   0        0        0     1413 2023-06-15 08:39:18.000000 FluidPyPLC-0.1.8/FluidPyPLC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      506 2023-06-15 08:39:18.000000 FluidPyPLC-0.1.8/FluidPyPLC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 08:39:18.000000 FluidPyPLC-0.1.8/FluidPyPLC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-15 08:39:18.000000 FluidPyPLC-0.1.8/FluidPyPLC.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       33 2023-06-15 08:39:18.000000 FluidPyPLC-0.1.8/FluidPyPLC.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-15 08:39:18.000000 FluidPyPLC-0.1.8/FluidPyPLC.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2023-05-29 12:32:57.000000 FluidPyPLC-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     1413 2023-06-15 08:39:18.396965 FluidPyPLC-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     5225 2023-06-14 21:04:11.000000 FluidPyPLC-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2023-06-15 08:39:18.397968 FluidPyPLC-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1378 2023-06-15 08:39:03.000000 FluidPyPLC-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 20:23:52.370508 FluidPyPLC-0.1.9/
+drwxrwxrwx   0        0        0        0 2023-06-17 20:23:52.314065 FluidPyPLC-0.1.9/FluidPyPLC/
+-rw-rw-rw-   0        0        0     7297 2023-06-14 20:24:29.000000 FluidPyPLC-0.1.9/FluidPyPLC/GUI.py
+-rw-rw-rw-   0        0        0        0 2023-06-14 20:16:54.000000 FluidPyPLC-0.1.9/FluidPyPLC/__init__.py
+-rw-rw-rw-   0        0        0     2770 2023-06-14 09:49:52.000000 FluidPyPLC-0.1.9/FluidPyPLC/data.py
+-rw-rw-rw-   0        0        0     3734 2023-06-14 20:26:13.000000 FluidPyPLC-0.1.9/FluidPyPLC/diagrams.py
+-rw-rw-rw-   0        0        0     2763 2023-06-15 08:38:30.000000 FluidPyPLC-0.1.9/FluidPyPLC/f.py
+-rw-rw-rw-   0        0        0     2342 2023-06-02 12:32:53.000000 FluidPyPLC-0.1.9/FluidPyPLC/get_sequence.py
+-rw-rw-rw-   0        0        0    13777 2023-06-02 21:04:22.000000 FluidPyPLC-0.1.9/FluidPyPLC/plc.bak.py
+-rw-rw-rw-   0        0        0     9617 2023-06-08 07:50:29.000000 FluidPyPLC-0.1.9/FluidPyPLC/plc.bak2.py
+-rw-rw-rw-   0        0        0    14557 2023-06-17 20:20:36.000000 FluidPyPLC-0.1.9/FluidPyPLC/plc.py
+drwxrwxrwx   0        0        0        0 2023-06-17 20:23:52.368476 FluidPyPLC-0.1.9/FluidPyPLC/resources/
+-rw-rw-rw-   0        0        0       59 2023-06-14 19:54:48.000000 FluidPyPLC-0.1.9/FluidPyPLC/resources/config.json
+-rw-rw-rw-   0        0        0      889 2023-06-03 13:58:59.000000 FluidPyPLC-0.1.9/FluidPyPLC/set_groups.py
+-rw-rw-rw-   0        0        0     1120 2023-06-03 13:58:52.000000 FluidPyPLC-0.1.9/FluidPyPLC/set_switches.py
+drwxrwxrwx   0        0        0        0 2023-06-17 20:23:52.356572 FluidPyPLC-0.1.9/FluidPyPLC.egg-info/
+-rw-rw-rw-   0        0        0     1413 2023-06-17 20:23:52.000000 FluidPyPLC-0.1.9/FluidPyPLC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      506 2023-06-17 20:23:52.000000 FluidPyPLC-0.1.9/FluidPyPLC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 20:23:52.000000 FluidPyPLC-0.1.9/FluidPyPLC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-17 20:23:52.000000 FluidPyPLC-0.1.9/FluidPyPLC.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       33 2023-06-17 20:23:52.000000 FluidPyPLC-0.1.9/FluidPyPLC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-17 20:23:52.000000 FluidPyPLC-0.1.9/FluidPyPLC.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2023-05-29 12:32:57.000000 FluidPyPLC-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     1413 2023-06-17 20:23:52.369482 FluidPyPLC-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5151 2023-06-15 09:15:39.000000 FluidPyPLC-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-17 20:23:52.370508 FluidPyPLC-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1378 2023-06-17 20:22:47.000000 FluidPyPLC-0.1.9/setup.py
```

### Comparing `FluidPyPLC-0.1.8/FluidPyPLC/GUI.py` & `FluidPyPLC-0.1.9/FluidPyPLC/GUI.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.8/FluidPyPLC/data.py` & `FluidPyPLC-0.1.9/FluidPyPLC/data.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.8/FluidPyPLC/diagrams.py` & `FluidPyPLC-0.1.9/FluidPyPLC/diagrams.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.8/FluidPyPLC/f.py` & `FluidPyPLC-0.1.9/FluidPyPLC/f.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.8/FluidPyPLC/get_sequence.py` & `FluidPyPLC-0.1.9/FluidPyPLC/get_sequence.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.8/FluidPyPLC/plc.bak.py` & `FluidPyPLC-0.1.9/FluidPyPLC/plc.bak.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.8/FluidPyPLC/plc.bak2.py` & `FluidPyPLC-0.1.9/FluidPyPLC/plc.bak2.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.8/FluidPyPLC/plc.py` & `FluidPyPLC-0.1.9/FluidPyPLC/plc.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,62 +180,63 @@
                     stroke_index += 1
                     finish_group += 1
                 # when the first group is finishes, then the limit switch that activates the first memory is triggered
                 f.write(f'IF {relay_memory_switches[0][0]} THEN\n\t\t')
                 f.write(f'{relay_memory_label[0]} := TRUE;\n\t')
                 f.write('END_IF;\n')
                 # then we need to close the IF statement *
-                f.write('\nEND_IF;\n\n')
+                f.write('\nEND_IF;\n')
             else:
                 # if the first group is composed by just one stroke then we pass to the next group by activating the first memory
                 stroke_index = 1
                 f.write(f'IF {relay_memory_switches[0][0]} THEN\n\t\t')
                 f.write(f'{relay_memory_label[0]} := TRUE;\n\t')
                 f.write('END_IF;\n')
                 # we close the IF statement *
-                f.write('END_IF;\n\n')
+                f.write('END_IF;\n')
             # first group is Done!
 
             # first memory relay activation
             f.write(f'\nIF {relay_memory_label[0]} THEN\n')
             if merge:
                 # if the last group can be merged with the first one, then we include those strokes
                 merged_groups = []
                 merged_groups = plc_groups[0] + plc_groups[-1]
                 for k in range(len(plc_groups[0]) + len(plc_groups[-1])):
                     f.write(f'\t{merged_groups[k]} := FALSE;\n')
-                f.write('END_IF;\n\n')
+                f.write('END_IF;\n')
             else:
                 # if not, write only the group strokes
                 for k in range(len(plc_groups[0])):
                     f.write(f'\t{plc_groups[0][k]} := FALSE;\n')
-                f.write('END_IF;\n\n')
+                f.write('END_IF;\n')
 
             #------------NEXT GROUPS-------------------------
             stroke_index_return = stroke_index
             for j in range(number_of_memories):
                 finish_group = 0
 
                 f.write(f'IF {limit_switches[stroke_index - 1]} AND {relay_memory_label[j]} THEN\n')
                 f.write(f'\t{solenoids[stroke_index]} := TRUE;\n')
                 while finish_group < len(plc_groups[j + 1]):
                     stroke_index += 1
                     finish_group += 1
-                f.write('END_IF;\n\n')
+                f.write('END_IF;\n')
             
             stroke_index = stroke_index_return
             for j in range(number_of_memories):
                 finish_group = 0
                 f.write(f'\nIF {relay_memory_label[j]} THEN\n\t')
                 while finish_group < len(plc_groups[j + 1]):
                     # while the group isn't finished continue to write the triggered limit switches and solenoids
                     if finish_group != (len(plc_groups[j+1]) - 1):
                         f.write(f'IF {limit_switches[stroke_index]} THEN\n\t')
                         stroke_index += 1
                         f.write(f'\t{solenoids[stroke_index]} := TRUE;\n\t')
+                        f.write('END_IF;\n\t')
                     else:
                         stroke_index += 1
                     if finish_group > 0:
                         f.write('END_IF;\n\t')
                     # we move by one index at the time until the group does not finish
                     finish_group += 1
                 
@@ -245,15 +246,15 @@
                 f.write(f'{relay_memory_label[j]} := FALSE;\n\t')
                 f.write('END_IF;\n')
 
                 f.write(f'\tIF NOT {relay_memory_label[j]} THEN\n')
                 for k in range(len(plc_groups[j + 1])):
                     f.write(f'\t\t{plc_groups[j + 1][k]} := FALSE;\n')
                 f.write('\tEND_IF;\n')
-                f.write('END_IF;\n\n')
+                f.write('END_IF;\n')
                 #------------------------------------
             if merge:
                 f.write(f'IF {limit_switches[stroke_index - 1]} AND NOT {relay_memory_label[0]} ')
                 if len(plc_groups[-1]) > 1:
                     for i in range(1, number_of_memories):
                         f.write(f'AND NOT {relay_memory_label[i]} ')
                     f.write('THEN\n')
```

### Comparing `FluidPyPLC-0.1.8/FluidPyPLC/set_groups.py` & `FluidPyPLC-0.1.9/FluidPyPLC/set_groups.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.8/FluidPyPLC/set_switches.py` & `FluidPyPLC-0.1.9/FluidPyPLC/set_switches.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.8/FluidPyPLC.egg-info/PKG-INFO` & `FluidPyPLC-0.1.9/FluidPyPLC.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FluidPyPLC
-Version: 0.1.8
+Version: 0.1.9
 Summary: FluidSim Circuits Analyzer & PLC ST Code Generator
 Home-page: https://github.com/MrLostInTheInternet/FluidPyPLC
 Author: MrLostInTheInternet (Eugen Iofciu Vasile)
 Author-email: <eugen.iofciuvasile@hotmail.com>
 License: GPLv3
 Keywords: python,plc,fluidsim,structured text,plc python,codesys,circuits,pneumatics,oleodynamics,plc programming
 Classifier: Development Status :: 1 - Planning
```

### Comparing `FluidPyPLC-0.1.8/LICENSE` & `FluidPyPLC-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.8/PKG-INFO` & `FluidPyPLC-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FluidPyPLC
-Version: 0.1.8
+Version: 0.1.9
 Summary: FluidSim Circuits Analyzer & PLC ST Code Generator
 Home-page: https://github.com/MrLostInTheInternet/FluidPyPLC
 Author: MrLostInTheInternet (Eugen Iofciu Vasile)
 Author-email: <eugen.iofciuvasile@hotmail.com>
 License: GPLv3
 Keywords: python,plc,fluidsim,structured text,plc python,codesys,circuits,pneumatics,oleodynamics,plc programming
 Classifier: Development Status :: 1 - Planning
```

### Comparing `FluidPyPLC-0.1.8/README.md` & `FluidPyPLC-0.1.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -41,28 +41,19 @@
 ```
 ## ⬇️ Installation <a name="installation"></a>
 Use pip to install FluidPyPLC:
 ```bash
 pip install FluidPyPLC
 ```
 
-Before you use it, you have to config the config.json file. Change the "folder_path" in the config.json file:
-
-```bash
-config.json :
-{
-  "folder_path": "full/path/to/the/folder/that/you/want"
-}
-```
-
-Now you need to create the Plot and the plc folder. You can do it manually or you can use:
+Now you need to set a main folder where to save your data, and you need to create there the Plot and the plc folder. You can do it manually or you can use:
 ```bash
 fluidpy --folder path/to/your/folder
 ```
-And FluidPyPLC will create the two folders for you.
+And FluidPyPLC will create the two folders for you, and change the config.json file "folder_path" to "your folder path".
 
 [+] For Windows Users. If you want an icon to execute the GUI faster -> create a new shortcut and assign the Target:
 ```bash
 Target: fluidpy.exe --gui
 ```
 Windows will automatically locate the fluidpy.exe script in your Python/scripts folder and you can launch the app from your icon now.
```

### Comparing `FluidPyPLC-0.1.8/setup.py` & `FluidPyPLC-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.8'
+VERSION = '0.1.9'
 DESCRIPTION = 'FluidSim Circuits Analyzer & PLC ST Code Generator'
 
 with open("FluidPyPLC/README.md", "r") as f:
     long_description = f.read()
 
 # Setting up
 setup(
```

