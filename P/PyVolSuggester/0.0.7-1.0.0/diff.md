# Comparing `tmp/pyvolsuggester-0.0.7.tar.gz` & `tmp/pyvolsuggester-1.0.0.tar.gz`

## Comparing `pyvolsuggester-0.0.7.tar` & `pyvolsuggester-1.0.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.7/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.7/License.txt
--rw-r--r--   0        0        0     9423 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.7/README.md
--rw-r--r--   0        0        0     8529 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.7/pyproject.toml
--rw-r--r--   0        0        0    11815 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pyvolsuggester-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pyvolsuggester-1.0.0/License.txt
+-rw-r--r--   0        0        0     9597 2020-02-02 00:00:00.000000 pyvolsuggester-1.0.0/README.md
+-rw-r--r--   0        0        0     8529 2020-02-02 00:00:00.000000 pyvolsuggester-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    11965 2020-02-02 00:00:00.000000 pyvolsuggester-1.0.0/PKG-INFO
```

### Comparing `pyvolsuggester-0.0.7/License.txt` & `pyvolsuggester-1.0.0/License.txt`

 * *Files identical despite different names*

### Comparing `pyvolsuggester-0.0.7/README.md` & `pyvolsuggester-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -115,53 +115,77 @@
 		- `Mel Frequency Cepstral Coefficients`
 		- `Mel Frequency Spectogram`
 		- `Chroma Feature`
 		- `Tempogram`
 
     3. Player for playing selected audio file
 	
-	4. Suggestion on volume on the basis of various feature extraction.
+    4. Suggestion on volume on the basis of various feature extraction.
 
 ****
 
 ### 📌Prerequisites:
 - In order to use this package, one need to ensure the following requirements:
     - Python 3.7 or later installed on your machine.
+    - ffmpeg pacakge must be installed and its PATH must be added to Environment variables.
 
 ****
 
 ### 📌Package Usage
+This command will install all the uninstalled required libraries used in script.
 ```
-- from PyVolSuggester import Suggester
-    - This command will install all the uninstalled required libraries used in script.
-- Suggester.main()
-    - This will prompt user for input of audio file selection.
-- Suggester.extract()
-	- This will extract the generic features of the selected audio file.
-- Suggester.play_pause_stop()
-	- This will allow user to play, plause and stop the audio file.
-- Suggester.amplitude_wave()
-	- This will generate a amplitude over time plot and save it as an image to output directory.
-- Suggester.spectogram()
-	- This will generate a spectogram plot and save it as an image to output directory.
-- Suggester.rms_energy_spectogram()
-	- This will generate a RMS/Energy Spectogram plot and save it as an image to output directory.
-- Suggester.zero_crossing_rate()
-	- This will generate a Zero Crossing Rate plot and save it as an image to output directory.
-- Suggester.mel_frequency_cepstral_coefficients()
-	- This will generate a Mel Frequency Cepstral Coefficients plot and save it as an image to output directory.
-- Suggester.mel_frequency_spectogram()
-	- This will generate a Mel Frequency Spectogram plot and save it as an image to output directory.
-- Suggester.chroma_feature()
-	- This will generate a Chroma Feature plot and save it as an image to output directory.
-- Suggester.tempogram()
-	- This will generate a tempogram plot and save it as an image to output directory.
-- Suggester.suggest_volume()
-	- This will suggest user the most feasible volume for that particular audio.
-
+from PyVolSuggester import Suggester
+```
+This will prompt user for input of `ffmpeg` path and audio file selection(.wav format).
+```
+Suggester.main()
+```
+This will extract the generic features of the selected audio file.
+```
+Suggester.extract()
+```
+This will allow user to play, plause and stop the audio file.
+```
+Suggester.play_pause_stop()
+```
+This will generate a amplitude over time plot and save it as an image to output directory.
+```
+Suggester.amplitude_wave()
+```
+This will generate a spectogram plot and save it as an image to output directory.
+```
+Suggester.spectogram()
+```
+This will generate a RMS/Energy Spectogram plot and save it as an image to output directory.
+```
+Suggester.rms_energy_spectogram()
+```
+This will generate a Zero Crossing Rate plot and save it as an image to output directory.
+```
+Suggester.zero_crossing_rate()
+```
+This will generate a Mel Frequency Cepstral Coefficients plot and save it as an image to output directory.
+```
+Suggester.mel_frequency_cepstral_coefficients()
+```
+This will generate a Mel Frequency Spectogram plot and save it as an image to output directory.
+```
+Suggester.mel_frequency_spectogram()
+```
+This will generate a Chroma Feature plot and save it as an image to output directory.
+```
+Suggester.chroma_feature()
+```
+This will generate a tempogram plot and save it as an image to output directory.
+```
+Suggester.tempogram()
+```
+This will suggest user the most feasible volume for that particular audio.
+```
+Suggester.suggest_volume()
 ```
 
 ****
 
 ### 📌Package Installation
 ```bash
 pip install PyVolSuggester
```

### Comparing `pyvolsuggester-0.0.7/pyproject.toml` & `pyvolsuggester-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 name = "PyVolSuggester"  # Required ## --------------------------------------------------------------------------------------------------------------------------------------
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "0.0.7"  # Required ## --------------------------------------------------------------------------------------------------------------------------------------
+version = "1.0.0"  # Required ## --------------------------------------------------------------------------------------------------------------------------------------
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "Does audio feature extraction and suggest the feasible volumne for better feeling and experience."  # Optional ## --------------------------------------------------------------------------------------------------------------------------------------
 
 # This is an optional longer description of your project that represents
```

### Comparing `pyvolsuggester-0.0.7/PKG-INFO` & `pyvolsuggester-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyVolSuggester
-Version: 0.0.7
+Version: 1.0.0
 Summary: Does audio feature extraction and suggest the feasible volumne for better feeling and experience.
 Project-URL: Homepage, https://github.com/akash-rajak/PyVolSuggester
 Project-URL: Bug Reports, https://github.com/akash-rajak/PyVolSuggester/issues
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Source, https://github.com/akash-rajak/PyVolSuggester
 Author-email: Akash Rajak <aakashrajak02@gmail.com>
 Maintainer-email: Akash Rajak <aakashrajak02@gmail.com>
@@ -161,53 +161,77 @@
 		- `Mel Frequency Cepstral Coefficients`
 		- `Mel Frequency Spectogram`
 		- `Chroma Feature`
 		- `Tempogram`
 
     3. Player for playing selected audio file
 	
-	4. Suggestion on volume on the basis of various feature extraction.
+    4. Suggestion on volume on the basis of various feature extraction.
 
 ****
 
 ### 📌Prerequisites:
 - In order to use this package, one need to ensure the following requirements:
     - Python 3.7 or later installed on your machine.
+    - ffmpeg pacakge must be installed and its PATH must be added to Environment variables.
 
 ****
 
 ### 📌Package Usage
+This command will install all the uninstalled required libraries used in script.
 ```
-- from PyVolSuggester import Suggester
-    - This command will install all the uninstalled required libraries used in script.
-- Suggester.main()
-    - This will prompt user for input of audio file selection.
-- Suggester.extract()
-	- This will extract the generic features of the selected audio file.
-- Suggester.play_pause_stop()
-	- This will allow user to play, plause and stop the audio file.
-- Suggester.amplitude_wave()
-	- This will generate a amplitude over time plot and save it as an image to output directory.
-- Suggester.spectogram()
-	- This will generate a spectogram plot and save it as an image to output directory.
-- Suggester.rms_energy_spectogram()
-	- This will generate a RMS/Energy Spectogram plot and save it as an image to output directory.
-- Suggester.zero_crossing_rate()
-	- This will generate a Zero Crossing Rate plot and save it as an image to output directory.
-- Suggester.mel_frequency_cepstral_coefficients()
-	- This will generate a Mel Frequency Cepstral Coefficients plot and save it as an image to output directory.
-- Suggester.mel_frequency_spectogram()
-	- This will generate a Mel Frequency Spectogram plot and save it as an image to output directory.
-- Suggester.chroma_feature()
-	- This will generate a Chroma Feature plot and save it as an image to output directory.
-- Suggester.tempogram()
-	- This will generate a tempogram plot and save it as an image to output directory.
-- Suggester.suggest_volume()
-	- This will suggest user the most feasible volume for that particular audio.
-
+from PyVolSuggester import Suggester
+```
+This will prompt user for input of `ffmpeg` path and audio file selection(.wav format).
+```
+Suggester.main()
+```
+This will extract the generic features of the selected audio file.
+```
+Suggester.extract()
+```
+This will allow user to play, plause and stop the audio file.
+```
+Suggester.play_pause_stop()
+```
+This will generate a amplitude over time plot and save it as an image to output directory.
+```
+Suggester.amplitude_wave()
+```
+This will generate a spectogram plot and save it as an image to output directory.
+```
+Suggester.spectogram()
+```
+This will generate a RMS/Energy Spectogram plot and save it as an image to output directory.
+```
+Suggester.rms_energy_spectogram()
+```
+This will generate a Zero Crossing Rate plot and save it as an image to output directory.
+```
+Suggester.zero_crossing_rate()
+```
+This will generate a Mel Frequency Cepstral Coefficients plot and save it as an image to output directory.
+```
+Suggester.mel_frequency_cepstral_coefficients()
+```
+This will generate a Mel Frequency Spectogram plot and save it as an image to output directory.
+```
+Suggester.mel_frequency_spectogram()
+```
+This will generate a Chroma Feature plot and save it as an image to output directory.
+```
+Suggester.chroma_feature()
+```
+This will generate a tempogram plot and save it as an image to output directory.
+```
+Suggester.tempogram()
+```
+This will suggest user the most feasible volume for that particular audio.
+```
+Suggester.suggest_volume()
 ```
 
 ****
 
 ### 📌Package Installation
 ```bash
 pip install PyVolSuggester
```

