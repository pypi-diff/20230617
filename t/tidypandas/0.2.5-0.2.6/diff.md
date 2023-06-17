# Comparing `tmp/tidypandas-0.2.5.tar.gz` & `tmp/tidypandas-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidypandas-0.2.5.tar", max compression
+gzip compressed data, was "tidypandas-0.2.6.tar", max compression
```

## Comparing `tidypandas-0.2.5.tar` & `tidypandas-0.2.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rwxr-xr-x   0        0        0     1098 2022-06-01 03:01:28.446490 tidypandas-0.2.5/LICENSE
--rw-r--r--   0        0        0     2932 2022-11-09 05:24:19.264063 tidypandas-0.2.5/README.md
--rw-r--r--   0        0        0     1185 2023-06-13 07:39:15.211492 tidypandas-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      156 2022-06-01 03:01:28.571841 tidypandas-0.2.5/src/tidypandas/__init__.py
--rw-r--r--   0        0        0     6485 2022-11-09 05:24:11.774773 tidypandas-0.2.5/src/tidypandas/_unexported_utils.py
--rw-r--r--   0        0        0     8284 2022-06-12 16:20:45.789325 tidypandas-0.2.5/src/tidypandas/format.py
--rw-r--r--   0        0        0    18139 2022-06-01 03:01:28.572904 tidypandas-0.2.5/src/tidypandas/series_utils.py
--rw-r--r--   0        0        0    22204 2022-06-14 04:50:48.045274 tidypandas-0.2.5/src/tidypandas/tidy_accessor.py
--rw-r--r--   0        0        0    10583 2023-01-27 16:34:38.208900 tidypandas-0.2.5/src/tidypandas/tidy_utils.py
--rw-r--r--   0        0        0   235601 2023-06-13 07:39:15.213244 tidypandas-0.2.5/src/tidypandas/tidyframe_class.py
--rw-r--r--   0        0        0     3950 2023-06-13 07:41:56.352638 tidypandas-0.2.5/setup.py
--rw-r--r--   0        0        0     3960 2023-06-13 07:41:56.353056 tidypandas-0.2.5/PKG-INFO
+-rwxr-xr-x   0        0        0     1098 2022-06-01 03:01:28.446490 tidypandas-0.2.6/LICENSE
+-rw-r--r--   0        0        0     2932 2022-11-09 05:24:19.264063 tidypandas-0.2.6/README.md
+-rw-r--r--   0        0        0     1187 2023-06-17 19:31:36.264153 tidypandas-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      156 2022-06-01 03:01:28.571841 tidypandas-0.2.6/src/tidypandas/__init__.py
+-rw-r--r--   0        0        0     6485 2022-11-09 05:24:11.774773 tidypandas-0.2.6/src/tidypandas/_unexported_utils.py
+-rw-r--r--   0        0        0     8284 2022-06-12 16:20:45.789325 tidypandas-0.2.6/src/tidypandas/format.py
+-rw-r--r--   0        0        0    18139 2022-06-01 03:01:28.572904 tidypandas-0.2.6/src/tidypandas/series_utils.py
+-rw-r--r--   0        0        0    22298 2023-06-17 19:31:36.265082 tidypandas-0.2.6/src/tidypandas/tidy_accessor.py
+-rw-r--r--   0        0        0    10583 2023-01-27 16:34:38.208900 tidypandas-0.2.6/src/tidypandas/tidy_utils.py
+-rw-r--r--   0        0        0   235987 2023-06-17 19:31:36.266651 tidypandas-0.2.6/src/tidypandas/tidyframe_class.py
+-rw-r--r--   0        0        0     3936 2023-06-17 19:32:09.892749 tidypandas-0.2.6/setup.py
+-rw-r--r--   0        0        0     3946 2023-06-17 19:32:09.893539 tidypandas-0.2.6/PKG-INFO
```

### Comparing `tidypandas-0.2.5/LICENSE` & `tidypandas-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tidypandas-0.2.5/README.md` & `tidypandas-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `tidypandas-0.2.5/pyproject.toml` & `tidypandas-0.2.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "tidypandas"
-version = "0.2.5"
+version = "0.2.6"
 description = "A grammar of data manipulation for pandas inspired by tidyverse"
 authors = ["Srikanth Komala Sheshachala <sri.teach@gmail.com>", "Ashish Raj <ashishrj.162@gmail.com>"]
 maintainers = ["Srikanth Komala Sheshachala <sri.teach@gmail.com>", "Ashish Raj <ashishrj.162@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://talegari.github.io/tidypandas/"
 repository = "https://github.com/talegari/tidypandas"
 documentation = "https://talegari.github.io/tidypandas/_build/html/autoapi/index.html"
 classifiers = ["Development Status :: 4 - Beta"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pandas = ">=1.0.0"
-collections-extended = "^2.0.2"
-skimpy = {version = "^0.0.5", optional = true}
+collections-extended = ">=2.0.2"
+skimpy = {version = ">=0.0.5", optional = true}
 
 [tool.poetry.extras]
 skimpy = ["skimpy"]
 
 [tool.poetry.dev-dependencies]
 myst-nb = {version = "^0.13.2", python = "^3.8"}
 sphinx-autoapi = "^1.8.4"
```

### Comparing `tidypandas-0.2.5/src/tidypandas/_unexported_utils.py` & `tidypandas-0.2.6/src/tidypandas/_unexported_utils.py`

 * *Files identical despite different names*

### Comparing `tidypandas-0.2.5/src/tidypandas/format.py` & `tidypandas-0.2.6/src/tidypandas/format.py`

 * *Files identical despite different names*

### Comparing `tidypandas-0.2.5/src/tidypandas/series_utils.py` & `tidypandas-0.2.6/src/tidypandas/series_utils.py`

 * *Files identical despite different names*

### Comparing `tidypandas-0.2.5/src/tidypandas/tidy_accessor.py` & `tidypandas-0.2.6/src/tidypandas/tidy_accessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -344,23 +344,25 @@
                     , names_from
                     , values_from
                     , values_fill = None
                     , values_fn = None
                     , id_cols = None
                     , sep = "__"
                     , names_prefix = ""
+                    , id_expand = False
                     ):
         tf = tidyframe(self._obj, copy = False, check = False)
         return tf.pivot_wider(names_from = names_from
                               , values_from = values_from
                               , values_fill = values_fill
                               , values_fn = values_fn
                               , id_cols = id_cols
                               , sep = sep
                               , names_prefix = names_prefix
+                              , id_expand = id_expand
                               ).to_pandas(copy = False)
     
     def pivot_longer(self
                      , cols
                      , names_to = "name"
                      , values_to = "value"
                      , include = True
```

### Comparing `tidypandas-0.2.5/src/tidypandas/tidy_utils.py` & `tidypandas-0.2.6/src/tidypandas/tidy_utils.py`

 * *Files identical despite different names*

### Comparing `tidypandas-0.2.5/src/tidypandas/tidyframe_class.py` & `tidypandas-0.2.6/src/tidypandas/tidyframe_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -3655,22 +3655,23 @@
             res = self.mutate({name: np.array(count_value)})
         else:
             res = self.left_join(count_frame, on = column_names)
         
         return res
     
     # pivot methods
-    def pivot_wider(self
-                    , names_from
-                    , values_from
-                    , values_fill = None
-                    , values_fn = None
-                    , id_cols = None
-                    , sep = "__"
-                    , names_prefix = ""
+    def pivot_wider(self,
+                    names_from,
+                    values_from,
+                    values_fill = None,
+                    values_fn = None,
+                    id_cols = None,
+                    sep = "__",
+                    names_prefix = "",
+                    id_expand = False
                     ):
         '''
         Pivot data from long to wide
         
         Parameters
         ----------
         names_from: string or list of strings
@@ -3697,14 +3698,19 @@
             
         sep: string
             seperator to use while creating resulting column names
             
         names_prefix: string
             prefix for new columns
             
+        id_expand: flag
+            Should the values in the id_cols columns be expanded before 
+            pivoting? This results in more rows, the output will contain a
+            complete expansion of all possible values in id_cols.
+            
         Returns
         -------
         tidyframe
         
         Examples
         --------
         >>> from palmerpenguins import load_penguins
@@ -3866,29 +3872,32 @@
         assert isinstance(sep, str),\
             "arg 'sep' should be a string"
             
         assert isinstance(names_prefix, str),\
             "arg 'names_prefix' should be a string without spaces"
         assert ' ' not in names_prefix,\
             "arg 'names_prefix' should be a string without spaces"
+            
+        assert isinstance(id_expand, bool),\
+            "arg 'id_expand' should be a flag"
         
         # make values_from a scalar if it is
         if len(values_from) == 1:
             values_from = values_from[0]
         
         # core pivoting logic
-        res = pd.pivot_table(data         = self.__data
-                             , index      = id_cols
-                             , columns    = names_from
-                             , values     = values_from
-                             , fill_value = values_fill
-                             , aggfunc    = values_fn
-                             , margins    = False
-                             , dropna     = False
-                             , observed   = True
+        res = pd.pivot_table(data       = self.__data,
+                             index      = id_cols,
+                             columns    = names_from,
+                             values     = values_from,
+                             fill_value = values_fill,
+                             aggfunc    = values_fn,
+                             margins    = False,
+                             dropna     = not id_expand,
+                             observed   = True
                              )
         
         res = tidyframe(simplify(res), copy = False, check = False)
         
         # add names prefix
         if names_prefix != "":
             org_cn = self.colnames
```

### Comparing `tidypandas-0.2.5/setup.py` & `tidypandas-0.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 packages = \
 ['tidypandas']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['collections-extended>=2.0.2,<3.0.0', 'pandas>=1.0.0']
+['collections-extended>=2.0.2', 'pandas>=1.0.0']
 
 extras_require = \
-{'skimpy': ['skimpy>=0.0.5,<0.0.6']}
+{'skimpy': ['skimpy>=0.0.5']}
 
 setup_kwargs = {
     'name': 'tidypandas',
-    'version': '0.2.5',
+    'version': '0.2.6',
     'description': 'A grammar of data manipulation for pandas inspired by tidyverse',
     'long_description': "![](docs/logo.png)\n\n[![PyPI\nversion](https://badge.fury.io/py/tidypandas.svg)](https://badge.fury.io/py/tidypandas)\n\n# `tidypandas`\n\n> A **grammar of data manipulation** for\n> [pandas](https://pandas.pydata.org/docs/index.html) inspired by\n> [tidyverse](https://tidyverse.tidyverse.org/)\n\n`tidypandas` python package provides *minimal, pythonic* API for common\ndata manipulation tasks:\n\n-   `tidyframe` class (wrapper over pandas dataframe) provides a\n    dataframe with simplified index structure (no more resetting indexes\n    and multi indexes)\n-   Consistent ‘verbs’ (`select`, `arrange`, `distinct`, …) as methods\n    to `tidyframe` class which mostly return a `tidyframe`\n-   Unified interface for summarizing (aggregation) and mutate (assign)\n    operations across groups\n-   Utilites for pandas dataframes and series\n-   Uses simple python data structures, No esoteric classes, No pipes,\n    No Non-standard evaluation\n-   No copy data conversion between `tidyframe` and pandas dataframes\n-   An accessor to apply `tidyframe` verbs to simple pandas datarames\n-   …\n\n## Example\n\n-   `tidypandas` code:\n\n<!-- -->\n\n    df.filter(lambda x: x['col_1'] > x['col_1'].mean(), by = 'col_2')\n\n-   equivalent pandas code:\n\n<!-- -->\n\n    (df.groupby('col2')\n       .apply(lambda x: x.loc[x['col_1'] > x['col_1'].mean(), :])\n       .reset_index(drop = True)\n       )\n\n## Why use `tidypandas`\n\n`tidypandas` is for you if:\n\n-   you *frequently* write data manipulation code using pandas\n-   you prefer to have stay in pandas ecosystem (see accessor)\n-   you *prefer* to remember a [limited set of\n    methods](https://medium.com/dunder-data/minimally-sufficient-pandas-a8e67f2a2428)\n-   you do not want to write (or be surprised by)\n    [`reset_index`](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.reset_index.html),\n    [`rename_axis`](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.rename_axis.html)\n    often\n-   you prefer writing free flowing, expressive code in\n    [dplyr](https://dplyr.tidyverse.org/) style\n\n> `tidypandas` relies on the amazing `pandas` library and offers a\n> consistent API with a different\n> [philosophy](https://tidyverse.tidyverse.org/articles/manifesto.html).\n\n## Presentation\n\nLearn more about tidypandas\n([presentation](https://github.com/talegari/tidypandas/blob/master/docs/tp_pres.html))\n\n## Installation\n\n1.  Install release version from Pypi using pip:\n\n        pip install tidypandas\n\n2.  For offline installation, use whl/tar file from the [releases\n    page](https://github.com/talegari/tidypandas/releases) on github.\n\n## Contribution/bug fixes/Issues:\n\n1.  Open an issue/suggestion/bugfix on the github\n    [issues](https://github.com/talegari/tidypandas/issues) page.\n\n2.  Use the master branch from\n    [github](https://github.com/talegari/tidypandas) repo to submit your\n    PR.\n\n------------------------------------------------------------------------\n",
     'author': 'Srikanth Komala Sheshachala',
     'author_email': 'sri.teach@gmail.com',
     'maintainer': 'Srikanth Komala Sheshachala',
     'maintainer_email': 'sri.teach@gmail.com',
     'url': 'https://talegari.github.io/tidypandas/',
```

### Comparing `tidypandas-0.2.5/PKG-INFO` & `tidypandas-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidypandas
-Version: 0.2.5
+Version: 0.2.6
 Summary: A grammar of data manipulation for pandas inspired by tidyverse
 Home-page: https://talegari.github.io/tidypandas/
 License: MIT
 Author: Srikanth Komala Sheshachala
 Author-email: sri.teach@gmail.com
 Maintainer: Srikanth Komala Sheshachala
 Maintainer-email: sri.teach@gmail.com
@@ -12,17 +12,17 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: skimpy
-Requires-Dist: collections-extended (>=2.0.2,<3.0.0)
+Requires-Dist: collections-extended (>=2.0.2)
 Requires-Dist: pandas (>=1.0.0)
-Requires-Dist: skimpy (>=0.0.5,<0.0.6); extra == "skimpy"
+Requires-Dist: skimpy (>=0.0.5); extra == "skimpy"
 Project-URL: Documentation, https://talegari.github.io/tidypandas/_build/html/autoapi/index.html
 Project-URL: Repository, https://github.com/talegari/tidypandas
 Description-Content-Type: text/markdown
 
 ![](docs/logo.png)
 
 [![PyPI
```

