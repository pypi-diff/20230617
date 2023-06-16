# Comparing `tmp/laptrack-0.9.0.tar.gz` & `tmp/laptrack-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laptrack-0.9.0.tar", max compression
+gzip compressed data, was "laptrack-0.9.1.tar", max compression
```

## Comparing `laptrack-0.9.0.tar` & `laptrack-0.9.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1524 2022-11-05 13:50:44.242469 laptrack-0.9.0/LICENSE.rst
--rw-r--r--   0        0        0     8691 2022-11-05 13:50:44.242469 laptrack-0.9.0/README.rst
--rw-r--r--   0        0        0     2091 2022-11-05 13:50:55.903593 laptrack-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      385 2022-11-05 13:50:44.258470 laptrack-0.9.0/src/laptrack/__init__.py
--rw-r--r--   0        0        0      206 2022-11-05 13:50:44.258470 laptrack-0.9.0/src/laptrack/__main__.py
--rw-r--r--   0        0        0     6407 2022-11-05 13:50:44.258470 laptrack-0.9.0/src/laptrack/_coo_matrix_builder.py
--rw-r--r--   0        0        0     7660 2022-11-05 13:50:44.258470 laptrack-0.9.0/src/laptrack/_cost_matrix.py
--rw-r--r--   0        0        0      861 2022-11-05 13:50:44.258470 laptrack-0.9.0/src/laptrack/_optimization.py
--rw-r--r--   0        0        0    37675 2022-11-05 13:50:44.258470 laptrack-0.9.0/src/laptrack/_tracking.py
--rw-r--r--   0        0        0      556 2022-11-05 13:50:44.258470 laptrack-0.9.0/src/laptrack/_typing_utils.py
--rw-r--r--   0        0        0     8590 2022-11-05 13:50:44.258470 laptrack-0.9.0/src/laptrack/data_conversion.py
--rw-r--r--   0        0        0     3227 2022-11-05 13:50:44.258470 laptrack-0.9.0/src/laptrack/metric_utils.py
--rw-r--r--   0        0        0        0 2022-11-05 13:50:44.258470 laptrack-0.9.0/src/laptrack/py.typed
--rw-r--r--   0        0        0     7149 2022-11-05 13:50:44.258470 laptrack-0.9.0/src/laptrack/scores.py
--rw-r--r--   0        0        0      620 2022-11-05 13:50:44.258470 laptrack-0.9.0/src/laptrack/utils.py
--rw-r--r--   0        0        0     9873 1970-01-01 00:00:00.000000 laptrack-0.9.0/setup.py
--rw-r--r--   0        0        0    10149 1970-01-01 00:00:00.000000 laptrack-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1524 2022-11-06 12:59:58.902862 laptrack-0.9.1/LICENSE.rst
+-rw-r--r--   0        0        0     8691 2022-11-06 12:59:58.902862 laptrack-0.9.1/README.rst
+-rw-r--r--   0        0        0     2150 2022-11-06 13:00:06.978795 laptrack-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      408 2022-11-06 13:00:06.978795 laptrack-0.9.1/src/laptrack/__init__.py
+-rw-r--r--   0        0        0      206 2022-11-06 12:59:58.910862 laptrack-0.9.1/src/laptrack/__main__.py
+-rw-r--r--   0        0        0     6407 2022-11-06 12:59:58.910862 laptrack-0.9.1/src/laptrack/_coo_matrix_builder.py
+-rw-r--r--   0        0        0     7660 2022-11-06 12:59:58.910862 laptrack-0.9.1/src/laptrack/_cost_matrix.py
+-rw-r--r--   0        0        0      861 2022-11-06 12:59:58.910862 laptrack-0.9.1/src/laptrack/_optimization.py
+-rw-r--r--   0        0        0    37675 2022-11-06 12:59:58.910862 laptrack-0.9.1/src/laptrack/_tracking.py
+-rw-r--r--   0        0        0      556 2022-11-06 12:59:58.910862 laptrack-0.9.1/src/laptrack/_typing_utils.py
+-rw-r--r--   0        0        0     8590 2022-11-06 12:59:58.910862 laptrack-0.9.1/src/laptrack/data_conversion.py
+-rw-r--r--   0        0        0     3527 2022-11-06 13:00:06.978795 laptrack-0.9.1/src/laptrack/metric_utils.py
+-rw-r--r--   0        0        0        0 2022-11-06 12:59:58.910862 laptrack-0.9.1/src/laptrack/py.typed
+-rw-r--r--   0        0        0     7149 2022-11-06 12:59:58.910862 laptrack-0.9.1/src/laptrack/scores.py
+-rw-r--r--   0        0        0      620 2022-11-06 12:59:58.910862 laptrack-0.9.1/src/laptrack/utils.py
+-rw-r--r--   0        0        0     9873 1970-01-01 00:00:00.000000 laptrack-0.9.1/setup.py
+-rw-r--r--   0        0        0    10149 1970-01-01 00:00:00.000000 laptrack-0.9.1/PKG-INFO
```

### Comparing `laptrack-0.9.0/LICENSE.rst` & `laptrack-0.9.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `laptrack-0.9.0/README.rst` & `laptrack-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `laptrack-0.9.0/pyproject.toml` & `laptrack-0.9.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "laptrack"
-version = "0.9.0"
+version = "0.9.1"
 description = "LapTrack"
 authors = ["Yohsuke Fukai <ysk@yfukai.net>"]
 license = "BSD-3-Clause"
 readme = "README.rst"
 homepage = "https://github.com/yfukai/laptrack"
 repository = "https://github.com/yfukai/laptrack"
 documentation = "https://laptrack.readthedocs.io"
@@ -79,7 +79,9 @@
 show_column_numbers = true
 show_error_codes = true
 show_error_context = true
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.poetry_bumpversion.file."src/laptrack/__init__.py"]
```

### Comparing `laptrack-0.9.0/src/laptrack/_coo_matrix_builder.py` & `laptrack-0.9.1/src/laptrack/_coo_matrix_builder.py`

 * *Files identical despite different names*

### Comparing `laptrack-0.9.0/src/laptrack/_cost_matrix.py` & `laptrack-0.9.1/src/laptrack/_cost_matrix.py`

 * *Files identical despite different names*

### Comparing `laptrack-0.9.0/src/laptrack/_optimization.py` & `laptrack-0.9.1/src/laptrack/_optimization.py`

 * *Files identical despite different names*

### Comparing `laptrack-0.9.0/src/laptrack/_tracking.py` & `laptrack-0.9.1/src/laptrack/_tracking.py`

 * *Files identical despite different names*

### Comparing `laptrack-0.9.0/src/laptrack/_typing_utils.py` & `laptrack-0.9.1/src/laptrack/_typing_utils.py`

 * *Files identical despite different names*

### Comparing `laptrack-0.9.0/src/laptrack/data_conversion.py` & `laptrack-0.9.1/src/laptrack/data_conversion.py`

 * *Files identical despite different names*

### Comparing `laptrack-0.9.0/src/laptrack/metric_utils.py` & `laptrack-0.9.1/src/laptrack/metric_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Utilities for metric calculation."""
+from typing import List
 from typing import Tuple
+from typing import Union
 
 import numpy as np
 import pandas as pd
 from skimage.measure import regionprops_table
 
 from ._typing_utils import Float
 from ._typing_utils import Int
@@ -28,22 +30,26 @@
         bbox = []
         for i in range(self.ndim):
             y0 = min(r1[f"bbox-{i}"], r2[f"bbox-{i}"])
             y1 = max(r1[f"bbox-{i+self.ndim}"], r2[f"bbox-{i+self.ndim}"])
             bbox.append((y0, y1))
         return bbox
 
-    def __init__(self, label_images: IntArray):
+    def __init__(self, label_images: Union[IntArray, List[IntArray]]):
         """Summarise the segmentation properties and initialize the object.
 
         Parameters
         ----------
-        label_images : IntArray
-            The labeled images. The first dimension is interpreted as the time dimension.
+        label_images : Union[IntArray,List[IntArray]]
+            The labeled images. The first dimension is interpreted as the frame dimension.
         """
+        if not isinstance(label_images, np.ndarray):
+            label_images = np.array(label_images)
+        if label_images.ndim < 3:
+            raise ValueError("label_images dimension must be >=3.")
         self.label_images = label_images
         self.ndim = label_images.ndim - 1
         dfs = []
         for frame in range(label_images.shape[0]):
             df = pd.DataFrame(
                 regionprops_table(label_images[frame], properties=["label", "bbox"])
             )
```

### Comparing `laptrack-0.9.0/src/laptrack/scores.py` & `laptrack-0.9.1/src/laptrack/scores.py`

 * *Files identical despite different names*

### Comparing `laptrack-0.9.0/src/laptrack/utils.py` & `laptrack-0.9.1/src/laptrack/utils.py`

 * *Files identical despite different names*

### Comparing `laptrack-0.9.0/setup.py` & `laptrack-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'typing-extensions>=4.1.0,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['laptrack = laptrack.__main__:main']}
 
 setup_kwargs = {
     'name': 'laptrack',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': 'LapTrack',
     'long_description': "LapTrack\n========\n\n|PyPI| |Status| |Python Version| |License|\n\n|Read the Docs| |Tests| |Codecov|\n\n|pre-commit| |Black| |Zenodo|\n\n.. |PyPI| image:: https://img.shields.io/pypi/v/laptrack.svg\n   :target: https://pypi.org/project/laptrack/\n   :alt: PyPI\n.. |Status| image:: https://img.shields.io/pypi/status/laptrack.svg\n   :target: https://pypi.org/project/laptrack/\n   :alt: Status\n.. |Python Version| image:: https://img.shields.io/pypi/pyversions/laptrack\n   :target: https://pypi.org/project/laptrack\n   :alt: Python Version\n.. |License| image:: https://img.shields.io/pypi/l/laptrack\n   :target: https://opensource.org/licenses/BSD-3-Clause\n   :alt: License\n.. |Read the Docs| image:: https://img.shields.io/readthedocs/laptrack/latest.svg?label=Read%20the%20Docs\n   :target: https://laptrack.readthedocs.io/\n   :alt: Read the documentation at https://laptrack.readthedocs.io/\n.. |Tests| image:: https://github.com/yfukai/laptrack/workflows/Tests/badge.svg\n   :target: https://github.com/yfukai/laptrack/actions?workflow=Tests\n   :alt: Tests\n.. |Codecov| image:: https://codecov.io/gh/yfukai/laptrack/branch/main/graph/badge.svg\n   :target: https://codecov.io/gh/yfukai/laptrack\n   :alt: Codecov\n.. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white\n   :target: https://github.com/pre-commit/pre-commit\n   :alt: pre-commit\n.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg\n   :target: https://github.com/psf/black\n   :alt: Black\n.. |Zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5519538.svg\n   :target: https://doi.org/10.5281/zenodo.5519538\n   :alt: Zenodo\n\nFeatures\n--------\n\nProvides a robust particle tracking algorithm using the Linear Assignment Problem, with various cost functions for linking.\n\nSee the `preprint`_ and `associated repository`_ for the algorithm and parameter optimization by `Ray-Tune`_.\n\nRequirements\n------------\n\nPython >= 3.7.11 is supported.\nThe software is tested against Python 3.7-3.10 in Ubuntu, and 3.10 in MacOS and Windows environments,\nbut the other combinations should also be fine. Please `file an issue`_ if you encounter any problem.\n\nInstallation\n------------\n\nYou can install *LapTrack* via pip_ from PyPI_:\n\n.. code:: console\n\n   $ pip install laptrack\n\nIn Google Colaboratory, try\n\n.. code:: console\n\n   $ pip install --upgrade laptrack spacy flask matplotlib\n\nto update the pre-installed packages.\n\n\nUsage\n-----\n\nPlease see the Usage_ for details.\nThe example notebooks are provided in `docs/examples <https://github.com/yfukai/laptrack/tree/main/docs/examples>`_.\n\n\n================================= ============================================================================================ ======================\n notebook name                     short description                                                                            Google Colaboratory\n--------------------------------- -------------------------------------------------------------------------------------------- ----------------------\n `api_example.ipynb`_              Introducing the package API by a simple example.                                               |colab|\n--------------------------------- -------------------------------------------------------------------------------------------- ----------------------\n `bright_spots.ipynb`_             Application example: detecting bright spots by scikit-image `blob_log` and tracking them.\n--------------------------------- -------------------------------------------------------------------------------------------- ----------------------\n `cell_segmentation.ipynb`_        Application example: tracking centroids of the segmented C2C12 cells undergoing divisions.\n--------------------------------- -------------------------------------------------------------------------------------------- ----------------------\n `napari_interactive_fix.ipynb`_   Illustrates the usage of the ground-truth-preserved tracking with `napari`.\n--------------------------------- -------------------------------------------------------------------------------------------- ----------------------\n `overlap_tracking.ipynb`_         Illustrates the usage of the custom metric to use segmentation overlaps for tracking.\n================================= ============================================================================================ ======================\n\n.. _api_example.ipynb:            https://github.com/yfukai/laptrack/tree/main/docs/examples/api_example.ipynb\n.. _bright_spots.ipynb:           https://github.com/yfukai/laptrack/tree/main/docs/examples/bright_spots.ipynb\n.. _cell_segmentation.ipynb:      https://github.com/yfukai/laptrack/tree/main/docs/examples/cell_segmentation.ipynb\n.. _napari_interactive_fix.ipynb: https://github.com/yfukai/laptrack/tree/main/docs/examples/napari_interactive_fix.ipynb\n.. _overlap_tracking.ipynb:       https://github.com/yfukai/laptrack/tree/main/docs/examples/overlap_tracking.ipynb\n\n.. |colab| image:: https://colab.research.google.com/assets/colab-badge.svg\n           :target: https://colab.research.google.com/github/yfukai/laptrack/blob/main/docs/examples/api_example.ipynb\n\nThe `API reference <https://laptrack.readthedocs.io/en/latest/reference.html>`_ covers the main classes and functions provided by LapTrack.\n\nContributing\n------------\n\nContributions are very welcome.\nTo learn more, see the `Contributor Guide`_.\n\n\nLicense\n-------\n\nDistributed under the terms of the `The 3-Clause BSD License`_,\n*LapTrack* is free and open source software.\n\n\nIssues\n------\n\nIf you encounter any problems,\nplease `file an issue <https://github.com/yfukai/laptrack/issues>`_ along with a detailed description.\n\n\nCredits\n-------\n\n- This program implements a modified version of the algorithm in the `K. Jaqaman et al. (2008)`_.\n\n- Inspired by TrackMate_ a lot. See documentation_ for its detailed algorithm, the `2016 paper`_, and the `2021 paper`_.\n\n- The data in `docs/examples/napari_interactive_fix_data` are generated by cropping images in `10.5281/zenodo.6087728 <https://doi.org/10.5281/zenodo.6087728>`_, which is distributed with `Creative Commons Attribution 4.0 International`_.\n\n- The data in `docs/examples/cell_segmentation_data` are generated by cropping and resizing images in https://osf.io/ysaq2/, which is distributed with `Creative Commons Attribution 4.0 International`_. See `10.1038/sdata.2018.237 <https://doi.org/10.1038/sdata.2018.237>`_ for details.\n\n- The data in `docs/examples/overlap_tracking_data` is generated by cropping `segmentation.npy` in https://github.com/NoneqPhysLivingMatterLab/cell_interaction_gnn, which is distributed with `Apache License 2.0`_. See the `original paper <https://doi.org/10.1371/journal.pcbi.1010477>`_ for details.\n\n- This project was generated from `@cjolowicz`_'s `Hypermodern Python Cookiecutter`_ template.\n\n\nCitation\n--------\n\nIf you use this program for your research, please cite it and help us build more.\n\n.. code-block:: bib\n\n   @misc{fukai_2022,\n     title = {{{LapTrack}}: {{Linear}} Assignment Particle Tracking with Tunable Metrics},\n     shorttitle = {{{LapTrack}}},\n     author = {Fukai, Yohsuke T. and Kawaguchi, Kyogo},\n     year = {2022},\n     month = oct,\n     pages = {2022.10.05.511038},\n     publisher = {{bioRxiv}},\n     doi = {10.1101/2022.10.05.511038},\n   }\n   @misc{laptrack,\n      author = {Yohsuke T. Fukai},\n      title = {laptrack},\n      year  = {2021},\n      url   = {https://doi.org/10.5281/zenodo.5519537},\n   }\n\n.. _preprint: https://www.biorxiv.org/content/10.1101/2022.10.05.511038v1\n.. _associated repository: https://github.com/NoneqPhysLivingMatterLab/laptrack-optimization\n.. _Ray-Tune: https://www.ray.io/ray-tune\n\n.. _K. Jaqaman et al. (2008): https://www.nature.com/articles/nmeth.1237\n.. _TrackMate: https://imagej.net/plugins/trackmate/\n.. _documentation: https://imagej.net/plugins/trackmate/algorithms\n.. _2016 paper: https://doi.org/10.1016/j.ymeth.2016.09.016\n.. _2021 paper: https://doi.org/10.1101/2021.09.03.458852\n.. _Creative Commons Attribution 4.0 International: https://creativecommons.org/licenses/by/4.0/legalcode\n.. _The 3-Clause BSD License: https://opensource.org/licenses/BSD-3-Clause\n.. _Apache License 2.0: https://opensource.org/licenses/Apache-2.0\n\n.. _@cjolowicz: https://github.com/cjolowicz\n.. _Cookiecutter: https://github.com/audreyr/cookiecutter\n.. _PyPI: https://pypi.org/\n.. _Hypermodern Python Cookiecutter: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n.. _pip: https://pip.pypa.io/\n.. github-only\n.. _Contributor Guide: CONTRIBUTING.rst\n.. _Usage: https://laptrack.readthedocs.io/en/latest/usage.html\n",
     'author': 'Yohsuke Fukai',
     'author_email': 'ysk@yfukai.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/yfukai/laptrack',
```

### Comparing `laptrack-0.9.0/PKG-INFO` & `laptrack-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laptrack
-Version: 0.9.0
+Version: 0.9.1
 Summary: LapTrack
 Home-page: https://github.com/yfukai/laptrack
 License: BSD-3-Clause
 Author: Yohsuke Fukai
 Author-email: ysk@yfukai.net
 Requires-Python: >=3.7.11,<3.11
 Classifier: Development Status :: 4 - Beta
```

