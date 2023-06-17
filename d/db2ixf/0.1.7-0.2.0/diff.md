# Comparing `tmp/db2ixf-0.1.7.tar.gz` & `tmp/db2ixf-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "db2ixf-0.1.7.tar", last modified: Tue Jun  6 21:45:49 2023, max compression
+gzip compressed data, was "db2ixf-0.2.0.tar", last modified: Sat Jun 17 01:43:40 2023, max compression
```

## Comparing `db2ixf-0.1.7.tar` & `db2ixf-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:45:49.596060 db2ixf-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-06 21:44:32.000000 db2ixf-0.1.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34512 2023-06-06 21:44:32.000000 db2ixf-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7856 2023-06-06 21:45:49.596060 db2ixf-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-06-06 21:44:32.000000 db2ixf-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-06-06 21:44:32.000000 db2ixf-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 21:45:49.596060 db2ixf-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-06 21:44:32.000000 db2ixf-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:45:49.592059 db2ixf-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:45:49.592059 db2ixf-0.1.7/src/db2ixf/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-06 21:44:32.000000 db2ixf-0.1.7/src/db2ixf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-06 21:45:49.000000 db2ixf-0.1.7/src/db2ixf/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-06-06 21:44:32.000000 db2ixf-0.1.7/src/db2ixf/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9210 2023-06-06 21:44:32.000000 db2ixf-0.1.7/src/db2ixf/collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-06-06 21:44:32.000000 db2ixf-0.1.7/src/db2ixf/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-06 21:44:32.000000 db2ixf-0.1.7/src/db2ixf/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-06 21:44:32.000000 db2ixf-0.1.7/src/db2ixf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-06-06 21:44:32.000000 db2ixf-0.1.7/src/db2ixf/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18174 2023-06-06 21:44:32.000000 db2ixf-0.1.7/src/db2ixf/ixf.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-06 21:44:32.000000 db2ixf-0.1.7/src/db2ixf/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:45:49.596060 db2ixf-0.1.7/src/db2ixf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7856 2023-06-06 21:45:49.000000 db2ixf-0.1.7/src/db2ixf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-06 21:45:49.000000 db2ixf-0.1.7/src/db2ixf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 21:45:49.000000 db2ixf-0.1.7/src/db2ixf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-06 21:45:49.000000 db2ixf-0.1.7/src/db2ixf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 21:45:48.000000 db2ixf-0.1.7/src/db2ixf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-06 21:45:49.000000 db2ixf-0.1.7/src/db2ixf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-06 21:45:49.000000 db2ixf-0.1.7/src/db2ixf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:43:40.338937 db2ixf-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-17 01:42:28.000000 db2ixf-0.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34512 2023-06-17 01:42:28.000000 db2ixf-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-06-17 01:43:40.338937 db2ixf-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-06-17 01:42:28.000000 db2ixf-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-06-17 01:42:28.000000 db2ixf-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 01:43:40.338937 db2ixf-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-17 01:42:28.000000 db2ixf-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:43:40.334937 db2ixf-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:43:40.334937 db2ixf-0.2.0/src/db2ixf/
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-17 01:42:28.000000 db2ixf-0.2.0/src/db2ixf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-17 01:43:40.000000 db2ixf-0.2.0/src/db2ixf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-06-17 01:42:28.000000 db2ixf-0.2.0/src/db2ixf/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-06-17 01:42:28.000000 db2ixf-0.2.0/src/db2ixf/collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-06-17 01:42:28.000000 db2ixf-0.2.0/src/db2ixf/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-17 01:42:28.000000 db2ixf-0.2.0/src/db2ixf/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-06-17 01:42:28.000000 db2ixf-0.2.0/src/db2ixf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-06-17 01:42:28.000000 db2ixf-0.2.0/src/db2ixf/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18939 2023-06-17 01:42:28.000000 db2ixf-0.2.0/src/db2ixf/ibmcodecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18084 2023-06-17 01:42:28.000000 db2ixf-0.2.0/src/db2ixf/ixf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-17 01:42:28.000000 db2ixf-0.2.0/src/db2ixf/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:43:40.334937 db2ixf-0.2.0/src/db2ixf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-06-17 01:43:40.000000 db2ixf-0.2.0/src/db2ixf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-17 01:43:40.000000 db2ixf-0.2.0/src/db2ixf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 01:43:40.000000 db2ixf-0.2.0/src/db2ixf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-17 01:43:40.000000 db2ixf-0.2.0/src/db2ixf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 01:43:39.000000 db2ixf-0.2.0/src/db2ixf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-17 01:43:40.000000 db2ixf-0.2.0/src/db2ixf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-17 01:43:40.000000 db2ixf-0.2.0/src/db2ixf.egg-info/top_level.txt
```

### Comparing `db2ixf-0.1.7/CHANGELOG.md` & `db2ixf-0.2.0/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -8,14 +8,33 @@
 
 This project uses [*towncrier*](https://towncrier.readthedocs.io/) and the
 changes for the upcoming release may be found
 in [here](https://github.com/ismailhammounou/db2ixf/tree/main/resources/changelog)
 .
 
 <!-- release notes start -->
+## [0.2.0](https://github.com/ismailhammounou/db2ixf/tree/0.2.0) - 2023-06-17
+
+
+### Added
+
+- Add unit tests [db2ixf-3](https://github.com/ismailhammounou/db2ixf/issues/3)
+- Add ibm encoding to use on the fly by reading ixf file [db2ixf-23](https://github.com/ismailhammounou/db2ixf/issues/23)
+
+
+### Changed
+
+- improve CLI and adapt it [db2ixf-24](https://github.com/ismailhammounou/db2ixf/issues/24)
+
+
+### Removed
+
+- Delete encoding because IXF file contains the encoding [db2ixf-20](https://github.com/ismailhammounou/db2ixf/issues/20)
+- Drop support for python 3.7 [db2ixf-22](https://github.com/ismailhammounou/db2ixf/issues/22)
+
 
 ## [0.1.7](https://github.com/ismailhammounou/db2ixf/tree/0.1.7) - 2023-06-06
 
 
 ### Added
 
 - Add support for CLOB data type [db2ixf-16](https://github.com/ismailhammounou/db2ixf/issues/16)
```

### Comparing `db2ixf-0.1.7/LICENSE` & `db2ixf-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `db2ixf-0.1.7/PKG-INFO` & `db2ixf-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 Metadata-Version: 2.1
 Name: db2ixf
-Version: 0.1.7
+Version: 0.2.0
 Summary: Parsing and processing of IBM eXchange format (IXF)
 Author-email: Ismail Hammounou <ismail.hammounou@gmail.com>
 Maintainer-email: Ismail Hammounou <ismail.hammounou@gmail.com>
 License: AGPL-3.0
 Project-URL: homepage, https://pypi.org/project/db2ixf/
 Project-URL: documentation, https://ismailhammounou.github.io/db2ixf/
 Project-URL: repository, https://github.com/ismailhammounou/db2ixf.git
 Project-URL: changelog, https://github.com/ismailhammounou/db2ixf/blob/main/CHANGELOG.md
 Keywords: PC,IXF,IBM,DB2,Development,Tools,Package,Parsing,Format,Data,Analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Python](https://img.shields.io/badge/Python-37|38|39|310|311-green.svg)](https://www.python.org/)
-[![License](https://img.shields.io/badge/License-AGPLv3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
-[![Pipeline](https://github.com/ismailhammounou/db2ixf/actions/workflows/db2ixf.yml/badge.svg)](https://github.com/ismailhammounou/db2ixf/actions/workflows/db2ixf.yml)
+
+[![Language](https://img.shields.io/pypi/pyversions/db2ixf?color=ffde57&logo=python&style=for-the-badge)](https://www.python.org/)
+[![License](https://img.shields.io/pypi/l/db2ixf?color=3775A9&style=for-the-badge&logo=unlicense)](https://www.gnu.org/licenses/agpl-3.0)
+
+[![Pipeline](https://img.shields.io/github/actions/workflow/status/ismailhammounou/db2ixf/db2ixf.yml?branch=main&style=for-the-badge&logo=gitHub-actions)](https://github.com/ismailhammounou/db2ixf/actions/workflows/db2ixf.yml)
+[![Release](https://img.shields.io/github/v/release/ismailhammounou/db2ixf?display_name=tag&sort=semver&style=for-the-badge&logo=semver)](https://github.com/ismailhammounou/db2ixf/releases/latest)
+[![Pypi](https://img.shields.io/pypi/v/db2ixf?color=3775A9&logo=pypi&style=for-the-badge)](https://github.com/ismailhammounou/db2ixf/releases/latest)
+
+
+[![Downloads](https://img.shields.io/pypi/dm/db2ixf?style=for-the-badge)](https://pypi.org/project/db2ixf/)
+
 
 # DB2IXF Parser
 
 <div align="center">
   <img src="https://github.com/ismailhammounou/db2ixf/blob/main/resources/images/db2ixf-logo.png?raw=true" alt="Logo" width="300" height="300">
 </div>
 
@@ -45,16 +52,16 @@
 - **Convert to multiple formats**: The parsed data can be easily converted to
   JSON, CSV, or Parquet format, providing flexibility for further analysis and
   integration with other systems.
 - **Support for file-like objects**: IXF Parser supports file-like objects as
   input, enabling direct parsing of IXF data from file objects, making it
   convenient for handling large datasets without the need for intermediate file
   storage.
-- **Minimal dependencies**: The package has only 2 dependencies, pyarrow and
-  typer, which are automatically installed alongside the package.
+- **Minimal dependencies**: The package has only 3 dependencies (pyarrow,
+  typer and ebcdic) which are automatically installed alongside the package.
 - **CLI**: command line tool called ``db2ixf`` comes with the package.
 
 ## Hypothesis
 
 - **One** IXF file contains **One** table.
 
 ## Getting Started
```

### Comparing `db2ixf-0.1.7/README.md` & `db2ixf-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,18 @@
-[![Python](https://img.shields.io/badge/Python-37|38|39|310|311-green.svg)](https://www.python.org/)
-[![License](https://img.shields.io/badge/License-AGPLv3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
-[![Pipeline](https://github.com/ismailhammounou/db2ixf/actions/workflows/db2ixf.yml/badge.svg)](https://github.com/ismailhammounou/db2ixf/actions/workflows/db2ixf.yml)
+
+[![Language](https://img.shields.io/pypi/pyversions/db2ixf?color=ffde57&logo=python&style=for-the-badge)](https://www.python.org/)
+[![License](https://img.shields.io/pypi/l/db2ixf?color=3775A9&style=for-the-badge&logo=unlicense)](https://www.gnu.org/licenses/agpl-3.0)
+
+[![Pipeline](https://img.shields.io/github/actions/workflow/status/ismailhammounou/db2ixf/db2ixf.yml?branch=main&style=for-the-badge&logo=gitHub-actions)](https://github.com/ismailhammounou/db2ixf/actions/workflows/db2ixf.yml)
+[![Release](https://img.shields.io/github/v/release/ismailhammounou/db2ixf?display_name=tag&sort=semver&style=for-the-badge&logo=semver)](https://github.com/ismailhammounou/db2ixf/releases/latest)
+[![Pypi](https://img.shields.io/pypi/v/db2ixf?color=3775A9&logo=pypi&style=for-the-badge)](https://github.com/ismailhammounou/db2ixf/releases/latest)
+
+
+[![Downloads](https://img.shields.io/pypi/dm/db2ixf?style=for-the-badge)](https://pypi.org/project/db2ixf/)
+
 
 # DB2IXF Parser
 
 <div align="center">
   <img src="https://github.com/ismailhammounou/db2ixf/blob/main/resources/images/db2ixf-logo.png?raw=true" alt="Logo" width="300" height="300">
 </div>
 
@@ -21,16 +29,16 @@
 - **Convert to multiple formats**: The parsed data can be easily converted to
   JSON, CSV, or Parquet format, providing flexibility for further analysis and
   integration with other systems.
 - **Support for file-like objects**: IXF Parser supports file-like objects as
   input, enabling direct parsing of IXF data from file objects, making it
   convenient for handling large datasets without the need for intermediate file
   storage.
-- **Minimal dependencies**: The package has only 2 dependencies, pyarrow and
-  typer, which are automatically installed alongside the package.
+- **Minimal dependencies**: The package has only 3 dependencies (pyarrow,
+  typer and ebcdic) which are automatically installed alongside the package.
 - **CLI**: command line tool called ``db2ixf`` comes with the package.
 
 ## Hypothesis
 
 - **One** IXF file contains **One** table.
 
 ## Getting Started
@@ -191,8 +199,8 @@
 ## Conclusion
 
 IXF Parser offers a convenient solution for parsing and processing IBM DB2's IXF
 files. With its ease of use and support for various output formats, it provides
 a valuable tool for working with DB2 data. We hope that you find this package
 useful in your data analysis and integration workflows.
 
-Give it a try and let us know your feedback. Happy parsing!
+Give it a try and let us know your feedback. Happy parsing!
```

### Comparing `db2ixf-0.1.7/pyproject.toml` & `db2ixf-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,27 +18,27 @@
 ]
 description = 'Parsing and processing of IBM eXchange format (IXF)'
 keywords = [
     'PC', 'IXF', 'IBM', 'DB2', 'Development', 'Tools', 'Package', 'Parsing',
     'Format', "Data", "Analysis"
 ]
 license = { text = "AGPL-3.0" }
-requires-python = '>=3.7'
+requires-python = '>=3.8'
 dynamic = ['version', 'readme']
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: GNU Affero General Public License v3',
-    'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
 ]
 dependencies = [
+    'ebcdic',
     'pyarrow',
     'typer[all]',
 ]
 
 [project.optional-dependencies]
 
 [project.scripts]
```

### Comparing `db2ixf-0.1.7/src/db2ixf/cli.py` & `db2ixf-0.2.0/src/db2ixf/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,50 +38,40 @@
                           typer.Argument(
                               help='Path to the `json` OUTPUT file.',
                               dir_okay=False,
                               readable=False,
                               resolve_path=True,
                               rich_help_panel='Optional Arguments',
                           )] = None,
-        encoding: Annotated[Union[str, None],
-                            typer.Option(
-                                '--encoding',
-                                '-e',
-                                help='IXF file encoding.',
-                                rich_help_panel='Command Options',
-                            )] = 'latin-1',
         verbose: Annotated[int,
                            typer.Option(
                                '--verbose',
                                '-v',
-                               help='Verbosity level.',
+                               metavar='',
+                               help='Counter for verbosity level.',
                                count=True,
                            )] = 0,
 ):
     """
     Parse ixf ``FILE`` and convert it to a **json** ``OUTPUT``.
     """
     if output is None:
         output = Path.cwd()
         filename = file.name.lower().removesuffix('.ixf') + '.json'
         output /= filename
 
-    if encoding is None:
-        encoding = 'latin-1'
-
     if verbose > 2:
         logger.setLevel(VERBOSE_MAPPING[2])
     else:
         logger.setLevel(VERBOSE_MAPPING[verbose])
 
     logger.info(f'IXF file: {file}')
-    logger.info(f'IXF file encoding: {encoding}')
     logger.info(f'JSON file: {output}')
 
-    parser = IXFParser(file, encoding)
+    parser = IXFParser(file)
     parser.to_json(output)
     raise typer.Exit()
 
 
 @app.command(epilog='Made with heart :D')
 def csv(
         file: Annotated[Path,
@@ -96,61 +86,51 @@
                           typer.Argument(
                               help='Path to the `csv` OUTPUT file.',
                               dir_okay=False,
                               readable=False,
                               resolve_path=True,
                               rich_help_panel='Optional Arguments',
                           )] = None,
-        encoding: Annotated[Union[str, None],
-                            typer.Option(
-                                '--encoding',
-                                '-e',
-                                help='IXF file encoding.',
-                                rich_help_panel='Command Options',
-                            )] = 'latin-1',
         sep: Annotated[Union[str, None],
                        typer.Option(
                            '--sep',
                            '-s',
                            help='Separator/Delimiter of the csv file.',
                            rich_help_panel='Command Options',
                        )] = '|',
         verbose: Annotated[int,
                            typer.Option(
                                '--verbose',
                                '-v',
-                               help='Verbosity level.',
+                               metavar='',
+                               help='Counter for verbosity level.',
                                count=True,
                            )] = 0,
 ):
     """
     Parse ixf ``FILE`` and convert it to a **csv** ``OUTPUT``.
     """
     if output is None:
         output = Path.cwd()
         filename = file.name.lower().removesuffix('.ixf') + '.csv'
         output /= filename
 
-    if encoding is None:
-        encoding = 'latin-1'
-
     if sep is None:
         sep = '|'
 
     if verbose > 2:
         logger.setLevel(VERBOSE_MAPPING[2])
     else:
         logger.setLevel(VERBOSE_MAPPING[verbose])
 
     logger.info(f'IXF file: {file}')
-    logger.info(f'IXF file encoding: {encoding}')
     logger.info(f'CSV file: {output}')
     logger.info(f'CSV file separator/delimiter: {sep}')
 
-    parser = IXFParser(file, encoding)
+    parser = IXFParser(file)
     parser.to_csv(output, str(sep))
     raise typer.Exit()
 
 
 @app.command(epilog='Made with heart :D')
 def parquet(
         file: Annotated[Path,
@@ -165,21 +145,14 @@
                           typer.Argument(
                               help='Path to the `parquet` OUTPUT file.',
                               dir_okay=False,
                               readable=False,
                               resolve_path=True,
                               rich_help_panel='Optional Arguments',
                           )] = None,
-        encoding: Annotated[Union[str, None],
-                            typer.Option(
-                                '--encoding',
-                                '-e',
-                                help='IXF file encoding.',
-                                rich_help_panel='Command Options',
-                            )] = 'latin-1',
         version: Annotated[Union[str, None],
                            typer.Option(
                                '--version',
                                help='Parquet version. Please look '
                                     'at pyarrow documentation.',
                                rich_help_panel='Command Options',
                            )] = '1.0',
@@ -193,47 +166,44 @@
                                        'for memory optimization.',
                                   rich_help_panel='Command Options',
                               )] = 500,
         verbose: Annotated[int,
                            typer.Option(
                                '--verbose',
                                '-v',
-                               help='Verbosity level.',
+                               metavar='',
+                               help='Counter for verbosity level.',
                                count=True,
                            )] = 0,
 ):
     """
     Parse ixf ``FILE`` and convert it to a **parquet** ``OUTPUT``.
     """
     if output is None:
         output = Path.cwd()
         filename = file.name.lower().removesuffix('.ixf') + '.parquet'
         output /= filename
 
-    if encoding is None:
-        encoding = 'latin-1'
-
     if version is None:
         version = '1.0'
 
     if batch_size is None:
         batch_size = 500
 
     if verbose > 2:
         logger.setLevel(VERBOSE_MAPPING[2])
     else:
         logger.setLevel(VERBOSE_MAPPING[verbose])
 
     logger.info(f'IXF file: {file}')
-    logger.info(f'IXF file encoding: {encoding}')
     logger.info(f'PARQUET file: {output}')
     logger.info(f'PARQUET version: {version}')
     logger.info(f'Batch size: {batch_size}')
 
-    parser = IXFParser(file, encoding)
+    parser = IXFParser(file)
     parser.to_parquet(output, int(batch_size), str(version))
     raise typer.Exit()
 
 
 def version_callback(value: bool):
     if value:
         print(f"{__version__}")
```

### Comparing `db2ixf-0.1.7/src/db2ixf/collectors.py` & `db2ixf-0.2.0/src/db2ixf/collectors.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # coding=utf-8
 """Collects data from the fields extracted from the data records (D)."""
 from datetime import datetime, date, time
-from db2ixf.exceptions import LargeObjectLengthException, \
-    BinaryLengthException, ExceedingDefinedMaximumLengthException
+from db2ixf.exceptions import (LargeObjectLengthException,
+                               BinaryLengthException,
+                               CLOBCodePageException,
+                               CharLengthException,
+                               VarCharLengthException)
+from db2ixf.helpers import get_ccsid_from_column
 from struct import unpack
 from typing import Union
 
 
-def collect_binary(c, fields, pos, encoding) -> bytes:
+def collect_binary(c, fields, pos) -> bytes:
     """Collects BINARY data type from ixf as a bytes.
 
     Parameters
     ----------
     c : dict
-        Column descriptor extracted from IXF.
+        Column descriptor extracted from IXF file.
     fields : str
-        Binary string containing data of the row.
+        Bytes string containing data of the row.
     pos : int
         Position of the column in the `fields`.
-    encoding : str
-        Encoding of the ixf file.
 
     Returns
     -------
     bytes:
         a binary string data.
     """
     length = int(c['IXFCLENG'])
@@ -32,96 +34,88 @@
         raise BinaryLengthException(msg)
 
     field = fields[pos:pos + length]
 
     return field
 
 
-def collect_smallint(c, fields, pos, encoding) -> int:
+def collect_smallint(c, fields, pos) -> int:
     """Collects SMALLINT data type from ixf as an integer.
 
     Parameters
     ----------
     c : dict
-        Column descriptor extracted from IXF.
+        Column descriptor extracted from IXF file.
     fields : str
-        Binary string containing data of the row.
+        Bytes string containing data of the row.
     pos : int
         Position of the column in the `fields`.
-    encoding : str
-        Encoding of the ixf file.
 
     Returns
     -------
     int:
         Integer.
     """
     field = int(unpack('<i', fields[pos:pos + 2])[0])
     return field
 
 
-def collect_integer(c, fields, pos, encoding) -> int:
+def collect_integer(c, fields, pos) -> int:
     """Collects INTEGER data type from ixf as an integer.
 
     Parameters
     ----------
     c : dict
-        Column descriptor extracted from IXF.
+        Column descriptor extracted from IXF file.
     fields : str
-        Binary string containing data of the row.
+        Bytes string containing data of the row.
     pos : int
         Position of the column in the `fields`.
-    encoding : str
-        Encoding of the ixf file.
 
     Returns
     -------
     int:
         Integer.
     """
     field = int(unpack('<i', fields[pos:pos + 4])[0])
     return field
 
 
-def collect_bigint(c, fields, pos, encoding) -> int:
+def collect_bigint(c, fields, pos) -> int:
     """Collects BIGINT data type from ixf as an integer.
 
     Parameters
     ----------
     c : dict
-        Column descriptor extracted from IXF.
+        Column descriptor extracted from IXF file.
     fields : str
-        Binary string containing data of the row.
+        Bytes string containing data of the row.
     pos : int
         Position of the column in the `fields`.
-    encoding : str
-        Encoding of the ixf file.
 
     Returns
     -------
     int:
         Integer.
     """
     field = int(unpack('<q', fields[pos:pos + 8])[0])
     return field
 
 
-def collect_decimal(c, fields, pos, encoding) -> Union[int, float]:
+def collect_decimal(c, fields, pos) -> Union[int, float]:
     """Collects DECIMAL data type from ixf as a integer or a float.
 
     Parameters
     ----------
     c : dict
-        Column descriptor extracted from IXF.
+        Column descriptor extracted from IXF file.
     fields : str
-        Binary string containing data of the row.
+        Bytes string containing data of the row.
     pos : int
         Position of the column in the `fields`.
-    encoding : str
-        Encoding of the ixf file.
 
     Returns
     -------
     Union[int, float]:
         Integer or Float
     """
     p = int(c['IXFCLENG'][0:3])
@@ -139,227 +133,276 @@
 
     if s == 0:
         return int(dec)
 
     return dec / pow(10, s)
 
 
-def collect_floating_point(c, fields, pos, encoding) -> float:
+def collect_floating_point(c, fields, pos) -> float:
     """Collects FLOATING POINT data type from ixf as a float.
 
     Parameters
     ----------
     c : dict
-        Column descriptor extracted from IXF.
+        Column descriptor extracted from IXF file.
     fields : str
-        Binary string containing data of the row.
+        Bytes string containing data of the row.
     pos : int
         Position of the column in the `fields`.
-    encoding : str
-        Encoding of the ixf file.
 
     Returns
     -------
     float
         A python float object.
     """
     length = int(c['IXFCLENG'])
     fmt = '!d' if length == 8 else '!f'
     field = float(unpack(fmt, fields[pos:pos + length])[0])
     return field
 
 
-def collect_char(c, fields, pos, encoding) -> str:
+def collect_char(c, fields, pos) -> str:
     """Collects CHAR data type from ixf as a string.
 
     Parameters
     ----------
     c : dict
-        Column descriptor extracted from IXF.
+        Column descriptor extracted from IXF file.
     fields : str
-        Binary string containing data of the row.
+        Bytes string containing data of the row.
     pos : int
         Position of the column in the `fields`.
-    encoding : str
-        Encoding of the ixf file.
 
     Returns
     -------
     str:
         String.
     """
     length = int(c['IXFCLENG'])
-    field = str(fields[pos:pos + length], encoding=encoding)
+    if length > 254:
+        msg = 'Length of a char data types should not exceed 254 bytes.'
+        raise CharLengthException(msg)
+
+    sbcp, dbcp = get_ccsid_from_column(c)
+
+    if dbcp != 0:
+        field = fields[pos:pos + length].decode(f'cp{dbcp}')
+    else:
+        if sbcp == 0:
+            field = bin(int(fields[pos:pos + length], 2))
+        else:
+            field = fields[pos:pos + length].decode(f'cp{sbcp}')
+
     return field.strip()
 
 
-def collect_varchar(c, fields, pos, encoding) -> str:
+def collect_varchar(c, fields, pos) -> str:
     """Collects VARCHAR data type from ixf as a string.
 
     Parameters
     ----------
     c : dict
-        Column descriptor extracted from IXF.
+        Column descriptor extracted from IXF file.
     fields : str
-        Binary string containing data of the row.
+        Bytes string containing data of the row.
     pos : int
         Position of the column in the `fields`.
-    encoding : str
-        Encoding of the ixf file.
 
     Returns
     -------
     str:
         String.
     """
+    max_length = int(c['IXFCLENG'])
+    # if max_length > 254:
+    #     msg = f'Max length of a varchar data type (={max_length}) ' \
+    #           f'must be less than 254 bytes.'
+    #     raise ExceedingDefinedMaximumLengthException(msg)
+
     length = int(unpack('<h', fields[pos:pos + 2])[0])
+    if length > max_length:
+        msg = f'Length {length} exceeds the maximum length {max_length}.'
+        raise VarCharLengthException(msg)
+
     pos += 2
-    field = str(fields[pos:pos + length], encoding=encoding)
+
+    sbcp, dbcp = get_ccsid_from_column(c)
+
+    if dbcp != 0:
+        field = fields[pos:pos + length].decode(f'cp{dbcp}')
+    else:
+        if sbcp == 0:
+            field = bin(int(fields[pos:pos + length], 2))
+        else:
+            field = fields[pos:pos + length].decode(f'cp{sbcp}')
+
     return field.strip()
 
 
-def collect_date(c, fields, pos, encoding) -> date:
+def collect_date(c, fields, pos) -> date:
     """Collects DATE data type from ixf as a date object.
 
     Parameters
     ----------
     c : dict
-        Column descriptor extracted from IXF.
+        Column descriptor extracted from IXF file.
     fields : str
-        Binary string containing data of the row.
+        Bytes string containing data of the row.
     pos : int
         Position of the column in the `fields`.
-    encoding : str
-        Encoding of the ixf file.
 
     Returns
     -------
     date:
         Date of format yyyy-mm-dd.
     """
-    field = str(fields[pos:pos + 10], encoding=encoding)
+    field = str(fields[pos:pos + 10], encoding='utf-8')
     return datetime.strptime(field, '%Y-%m-%d').date()
 
 
-def collect_time(c, fields, pos, encoding) -> time:
+def collect_time(c, fields, pos) -> time:
     """Collects TIME data type from ixf as a time object.
 
     Parameters
     ----------
     c : dict
-        Column descriptor extracted from IXF.
+        Column descriptor extracted from IXF file.
     fields : str
-        Binary string containing data of the row.
+        Bytes string containing data of the row.
     pos : int
         Position of the column in the `fields`.
-    encoding : str
-        Encoding of the ixf file.
 
     Returns
     -------
     time:
         Time of format HH:MM:SS.
     """
-    field = str(fields[pos:pos + 8], encoding=encoding)
+    field = str(fields[pos:pos + 8], encoding='utf-8')
     return datetime.strptime(field, '%H.%M.%S').time()
 
 
-def collect_timestamp(c, fields, pos, encoding) -> datetime:
+def collect_timestamp(c, fields, pos) -> datetime:
     """Collects TIMESTAMP data type from ixf as a datetime object.
 
     Parameters
     ----------
     c : dict
-        Column descriptor extracted from IXF.
+        Column descriptor extracted from IXF file.
     fields : str
-        Binary string containing data of the row.
+        Bytes string containing data of the row.
     pos : int
         Position of the column in the `fields`.
-    encoding : str
-        Encoding of the ixf file.
 
     Returns
     -------
     timestamp:
         Timestamp of format yyyy-mm-dd-HH.MM.SS.UUUUUU
 
     Raises
     ------
     LargeObjectLengthException
         When the length of the large object exceeds the maximum length.
     """
-    field = str(fields[pos:pos + 26], encoding=encoding)
+    field = str(fields[pos:pos + 26], encoding='utf-8')
     return datetime.strptime(field, '%Y-%m-%d-%H.%M.%S.%f')
 
 
-def collect_clob(c, fields, pos, encoding) -> str:
+def collect_clob(c, fields, pos) -> str:
     """Collects CLOB data type from ixf as a string object.
 
     Parameters
     ----------
     c : dict
-        Column descriptor extracted from IXF.
+        Column descriptor extracted from IXF file.
     fields : str
-        Binary string containing data of the row.
+        Bytes string containing data of the row.
     pos : int
         Position of the column in the `fields`.
-    encoding : str
-        Encoding of the ixf file.
 
     Returns
     -------
     str
         String representing the CLOB (Character Large Object).
+
+    Raises
+    ------
+    ExceedingDefinedMaximumLengthException
+        When the maximum length exceeds the defined limit which is 32767 bytes.
+    LargeObjectLengthException
+        When the length of the large object exceeds the maximum length.
+    CLOBCodePageException
+        When SBCP and DBCP are simultaneously equal to 0.
     """
     max_length = int(c['IXFCLENG'])
-    if max_length > 32767:
-        msg = 'For CLOB data type, max length must be less than 32767 Bytes.'
-        raise ExceedingDefinedMaximumLengthException(msg)
+    # if max_length > 32767:
+    #     msg = f'For CLOB data type, max length (={max_length}) must be ' \
+    #           f'less than 32767 Bytes.'
+    #     raise ExceedingDefinedMaximumLengthException(msg)
 
     length = int(unpack('<h', fields[pos:pos + 4])[0])
     if length > max_length:
-        msg = f'Length exceeds the maximum length {max_length}.'
+        msg = f'Length {length} exceeds the maximum length {max_length}.'
         raise LargeObjectLengthException(msg)
 
     pos += 4
-    field = str(fields[pos:pos + length], encoding=encoding)
+
+    sbcp, dbcp = get_ccsid_from_column(c)
+
+    if dbcp != 0:
+        field = fields[pos:pos + length].decode(f'cp{dbcp}')
+    else:
+        if sbcp == 0:
+            msg = 'CLOB data type can not be a bit string as BLOB, ' \
+                  'the SBCP and DBCP should not simultaneously be equal to 0.'
+            raise CLOBCodePageException(msg)
+        else:
+            field = fields[pos:pos + length].decode(f'cp{sbcp}')
+
     return field.strip()
 
 
-def collect_blob(c, fields, pos, encoding) -> bytes:
-    """Collects BLOB data type from ixf as a binary string large object.
+def collect_blob(c, fields, pos) -> str:
+    """Collects BLOB data type from ixf as a string.
 
     Parameters
     ----------
     c : dict
-        Column descriptor extracted from IXF.
+        Column descriptor extracted from IXF file.
     fields : str
-        Binary string containing data of the row.
+        Bytes string containing data of the row.
     pos : int
         Position of the column in the `fields`.
-    encoding : str
-        Encoding of the ixf file.
 
     Returns
     -------
-    bytes
-        Binary string representing the BLOB (Blob Large Object).
+    str
+        string representing the BLOB (Blob Large Object) or a string
+        of bit data.
 
     Raises
     ------
+    ExceedingDefinedMaximumLengthException
+        When the maximum length exceeds the defined limit which is 32767 bytes.
     LargeObjectLengthException
         When the length of the large object exceeds the maximum length.
+
     """
     max_length = int(c['IXFCLENG'])
-    if max_length > 32767:
-        msg = 'For BLOB data type, max length must be less than 32767 Bytes.'
-        raise ExceedingDefinedMaximumLengthException(msg)
+    # if max_length > 32767:
+    #     msg = 'For BLOB data type, max length must be less than 32767 Bytes.'
+    #     raise ExceedingDefinedMaximumLengthException(msg)
 
     length = int(unpack('<h', fields[pos:pos + 4])[0])
     if length > max_length:
-        msg = f'Length exceeds the maximum length {max_length}.'
+        msg = f'Length {length} exceeds the maximum length {max_length}.'
         raise LargeObjectLengthException(msg)
 
     pos += 4
-    field = fields[pos:pos + length]
 
-    return field
+    sbcp, _ = get_ccsid_from_column(c)
+
+    if sbcp == 0:
+        field = bin(int(fields[pos:pos + length], 2))
+    else:
+        field = fields[pos:pos + length].decode(f'cp{sbcp}')
+
+    return field.strip()
```

### Comparing `db2ixf-0.1.7/src/db2ixf/exceptions.py` & `db2ixf-0.2.0/src/db2ixf/exceptions.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,75 +2,124 @@
 """Custom exceptions for IXF parsing."""
 
 
 class NotValidColumnDescriptorException(Exception):
     """
     Exception raised when encountering a non valid column descriptor.
 
-    Read the [doc](https://www.ibm.com/docs/en/db2/11.5?topic=format-pcixf-record-types)
+    Read the
+    [doc](https://www.ibm.com/docs/en/db2/11.5?topic=format-pcixf-record-types)
     """
 
     def __init__(self, message):
         self.message = message
         super().__init__(self.message)
 
 
 class UnknownDataTypeException(Exception):
     """
     Exception raised when encountering an unknown data type.
 
-    Read the [doc](https://www.ibm.com/docs/en/db2/11.5?topic=format-pcixf-data-types).
+    Read the
+    [doc](https://www.ibm.com/docs/en/db2/11.5?topic=format-pcixf-data-types).
     """
 
     def __init__(self, message):
         self.message = message
         super().__init__(self.message)
 
 
 class NotValidDataPrecisionException(Exception):
     """
     Exception raised when encountering a non valid data precision.
 
-    Read the [doc](https://www.ibm.com/docs/en/db2/11.5?topic=format-pcixf-data-types).
+    Read the
+    [doc](https://www.ibm.com/docs/en/db2/11.5?topic=format-pcixf-data-types).
     """
 
     def __init__(self, message):
         self.message = message
         super().__init__(self.message)
 
 
 class ExceedingDefinedMaximumLengthException(Exception):
     """
     Exception raised when encountering an object length exceeds the defined
     maximum length.
 
-    Read the [doc](https://www.ibm.com/docs/en/db2/11.5?topic=format-pcixf-data-types).
+    Read the
+    [doc](https://www.ibm.com/docs/en/db2/11.5?topic=format-pcixf-data-types).
     """
 
     def __init__(self, message):
         self.message = message
         super().__init__(self.message)
 
 
 class LargeObjectLengthException(Exception):
     """
     Exception raised when encountering a large object length exceeding the
     maximum length.
 
-    Read the [doc](https://www.ibm.com/docs/en/db2/11.5?topic=format-pcixf-data-types).
+    Read the
+    [doc](https://www.ibm.com/docs/en/db2/11.5?topic=format-pcixf-data-types).
     """
 
     def __init__(self, message):
         self.message = message
         super().__init__(self.message)
 
 
 class BinaryLengthException(Exception):
     """
-    Exception raised when encountering a length exceeding the maximum length.
+    Exception raised when encountering binary data type with a length exceeding
+    the maximum length.
 
-    Read the [doc](https://www.ibm.com/docs/en/db2/11.5?topic=format-pcixf-data-types).
+    Read the
+    [doc](https://www.ibm.com/docs/en/db2/11.5?topic=format-pcixf-data-types).
+    """
+
+    def __init__(self, message):
+        self.message = message
+        super().__init__(self.message)
+
+
+class CharLengthException(Exception):
+    """
+    Exception raised when encountering char data type with a length exceeding
+    the maximum length.
+
+    Read the
+    [doc](https://www.ibm.com/docs/en/db2/11.5?topic=format-pcixf-data-types).
+    """
+
+    def __init__(self, message):
+        self.message = message
+        super().__init__(self.message)
+
+
+class VarCharLengthException(Exception):
+    """
+    Exception raised when encountering varchar data type with a length
+    exceeding the maximum length.
+
+    Read the
+    [doc](https://www.ibm.com/docs/en/db2/11.5?topic=format-pcixf-data-types).
+    """
+
+    def __init__(self, message):
+        self.message = message
+        super().__init__(self.message)
+
+
+class CLOBCodePageException(Exception):
+    """
+    Exception raised when encountering CLOB data type where SBCP and DBCP are
+    simultaneously equal to 0
+
+    Read the
+    [doc](https://www.ibm.com/docs/en/db2/11.5?topic=format-pcixf-data-types).
     """
 
     def __init__(self, message):
         self.message = message
         super().__init__(self.message)
```

### Comparing `db2ixf-0.1.7/src/db2ixf/helpers.py` & `db2ixf-0.2.0/src/db2ixf/helpers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding=utf-8
 """Create helper function for schema generation and others."""
 import pyarrow
 from db2ixf.constants import IXF_DTYPES
 from db2ixf.exceptions import NotValidDataPrecisionException
-from typing import Generator, Dict
+from typing import Generator, Dict, BinaryIO, Tuple
 
 
 def get_pyarrow_schema(cols: list[dict]) -> dict[str, object]:
     """
     Creates a pyarrow schema of the columns extracted from IXF file.
 
     Parameters
@@ -116,15 +116,14 @@
         dtype = mapper[IXF_DTYPES[ctype]]
 
         if ctype == 480:
             length = int(c['IXFCLENG'])
             dtype = 'float32' if length == 4 else dtype
 
         if ctype == 484:
-            precision = int(c['IXFCLENG'][0:3])
             scale = int(c['IXFCLENG'][3:5])
             if scale == 0:
                 dtype = 'int64'
             else:
                 dtype = 'float32'
 
         schema[cname] = dtype
@@ -145,15 +144,16 @@
     Returns
     -------
     dict[str, list]
         A dictionary where each key is mapped to a list of values.
 
     Examples
     --------
-    >>> ex = [{'key1': 'value1', 'key2': 'value2'}, {'key1': 'value3', 'key2': 'value4'}]
+    >>> ex = [{'key1': 'value1', 'key2': 'value2'}] # noqa
+    >>> ex.append({'key1': 'value3', 'key2': 'value4'})
     >>> merge_dicts(ex)
     {'key1': ['value1', 'value3'], 'key2': ['value2', 'value4']}
     """
 
     result = {}
 
     for dictionary in dicts:
@@ -192,25 +192,81 @@
 
     >>> for b in batch_generator:
     ...     # Process the batch of rows
     ...     process_batch(b) # noqa
 
     Notes
     -----
-    - The function accumulates rows until the number of rows reaches the specified `size`.
+    - The function accumulates rows until the number of rows reaches the
+      specified `size`.
     - Once the accumulated rows reach the `size`, a batch is formed and yielded.
-    - If there are remaining rows that do not form a complete batch, they are yielded as the last batch.
-    - The `merge_dicts` function should be implemented separately and used to merge the rows into a single dictionary.
+    - If there are remaining rows that do not form a complete batch, they are
+      yielded as the last batch.
+    - The `merge_dicts` function should be implemented separately and used
+      to merge the rows into a single dictionary.
     """
 
     rows = []
     for i, row in enumerate(generator()):
         rows.append(row)
         if (i + 1) % size == 0:
             batch = merge_dicts(rows)
             yield batch
             rows = []
 
     # Yield the remaining rows as the last batch
     if rows:
         batch = merge_dicts(rows)
         yield batch
+
+
+def get_ccsid_from_header(header: dict) -> Tuple[int, int]:
+    """
+    Get the coded character set identifiers for single and double
+    bytes data type. Which means the code page for singular/double byte
+    data type.
+    """
+    sbcp = str(header['IXFHSBCP'], 'utf-8').strip()
+    dbcp = str(header['IXFHDBCP'], 'utf-8').strip()
+
+    sbcp = int(sbcp) if sbcp else 0
+    dbcp = int(dbcp) if dbcp else 0
+
+    if sbcp == 0:
+        dbcp = 0
+
+    return sbcp, dbcp
+
+
+def get_ccsid_from_column(column: dict) -> Tuple[int, int]:
+    """
+    Get the coded character set identifiers for single and double bytes
+    data type. Which means the code page for singular/double byte data type.
+    """
+    sbcp = str(column['IXFCSBCP'], 'utf-8').strip()
+    dbcp = str(column['IXFCDBCP'], 'utf-8').strip()
+
+    sbcp = int(sbcp) if sbcp else 0
+    dbcp = int(dbcp) if dbcp else 0
+
+    if sbcp == 0:
+        dbcp = 0
+
+    return sbcp, dbcp
+
+
+def get_record_length_and_type(file: BinaryIO) -> Tuple[int, str]:
+    """Get record length and its type.
+
+    Parameters
+    ----------
+    file : BinaryIO.
+        File-like object representing the IXF file.
+
+    Returns
+    -------
+    Tuple[int, str]
+        record length, record type
+    """
+    recl: int = int(file.read(6))
+    rect: str = file.read(1).decode("utf-8")
+    return recl, rect
```

### Comparing `db2ixf-0.1.7/src/db2ixf/ixf.py` & `db2ixf-0.2.0/src/db2ixf/ixf.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,18 +21,18 @@
                                collect_clob,
                                collect_binary)
 from db2ixf.constants import (HEADER_RECORD_TYPE,
                               TABLE_RECORD_TYPE,
                               COL_DESCRIPTOR_RECORD_TYPE,
                               DATA_RECORD_TYPE)
 from db2ixf.encoders import CustomJSONEncoder
-from db2ixf.exceptions import (
-    NotValidColumnDescriptorException,
-    UnknownDataTypeException)
-from db2ixf.helpers import get_batch, get_pyarrow_schema
+from db2ixf.exceptions import (NotValidColumnDescriptorException,
+                               UnknownDataTypeException)
+from db2ixf.helpers import (get_batch,
+                            get_pyarrow_schema)
 from db2ixf.logger import logger
 from os import PathLike
 from pathlib import Path
 from pyarrow.parquet import ParquetWriter
 from typing import Union, List, BinaryIO, TextIO
 
 
@@ -40,16 +40,14 @@
     """
     PC/IXF Parser.
 
     Attributes
     ----------
     file : str, Path, PathLike or File-Like Object
         Input file and it is better to use file-like object.
-    encoding: str, default: latin-1
-        Encoding of the ixf file. Defaults to latin-1 (ISO 8859-1).
     """
     header_info: dict
     """Contains header informations from input ixf file."""
     table_info: dict
     """Contains table informations from input ixf file."""
     columns_info: List[dict]
     """Contains columns description from input ixf file."""
@@ -61,37 +59,33 @@
     """Flag the end of data records in the input ixf file."""
     current_row: dict
     """Contains parsed data extracted from a data record of the input ixf 
     file."""
     number_rows: int
     """Number of rows extracted from the input ixf file."""
 
-    def __init__(self,
-                 file: Union[str, Path, PathLike, BinaryIO],
-                 encoding: str = 'latin-1'):
+    def __init__(self, file: Union[str, Path, PathLike, BinaryIO]):
         """Init the instance."""
         logger.debug('Start initializing the parser')
 
         if isinstance(file, (str, Path, PathLike)):
             file = open(file, mode='rb')
             logger.debug('File opened in read & binary mode')
 
         try:
             if file.mode != 'rb':
-                msg = 'file-like object should be opened in ' \
-                      'read and binary mode'
+                msg = 'file-like object should be opened in read-binary mode'
                 raise ValueError(msg)
         except Exception as e:
             logger.error('Parser has an error while reading the ixf file')
             logger.error(e)
             sys.exit(1)  # Exit the program with a non-zero exit code
 
         # Init instance attributes
         self.file = file
-        self.encoding = encoding
 
         # State
         self.header_info = {}
         self.table_info = {}
         self.columns_info = []
         self.schema = {}
         self.current_data_record = {}
@@ -170,25 +164,27 @@
         # 'IXFTCCNT' contains number of columns in the table
         for _ in range(0, int(self.table_info['IXFTCCNT'])):
 
             column = {}
             for i, j in record_type.items():
                 column[i] = self.file.read(j)
 
-            try:
-                if column['IXFCRECT'] != b'C':
-                    c = str(column['IXFCNAME'], encoding=self.encoding).strip()
-                    msg = f'IXF file is not valid, it contains a not ' \
-                          f'valid column descriptor (see {c}).'
-                    raise NotValidColumnDescriptorException(msg)
-            except Exception as e:
-                logger.error(e)
-                sys.exit(1)
+            if column['IXFCRECT'] != b'C':
+                msg1 = f'Non valid IXF file: It either contains non ' \
+                       f'supported record type/subtype like application ' \
+                       f'one or it contains a non valid column descriptor ' \
+                       f'(see the column {column["IXFCNAME"]}).'
+                logger.error(msg1)
+                msg2 = 'Hint: try to recreate IXF file without any ' \
+                       'application record or any SQL error.'
+                logger.info(msg2)
+                raise NotValidColumnDescriptorException(msg1)
 
             column['IXFCDSIZ'] = self.file.read(int(column['IXFCRECL']) - 862)
+
             self.columns_info.append(column)
         return self.columns_info
 
     def parse_data_record(self, record_type: dict = None):
         """Parse one data record.
 
         Parameters
@@ -222,15 +218,15 @@
         dict:
             Dictionary containing all extracted data from fields of
             the data record.
         """
         # Start Extraction
         r = {}
         for c in self.columns_info:
-            col_name = str(c['IXFCNAME'], encoding=self.encoding).strip()
+            col_name = str(c['IXFCNAME'], encoding='utf-8').strip()
             col_type = int(c['IXFCTYPE'])
             col_is_nullable = c['IXFCNULL'] == b'Y'
             col_position = int(c['IXFCPOSN'])
 
             # Parse next data record in case a column is in position 1
             if col_position == 1:
                 self.parse_data_record()
@@ -278,16 +274,15 @@
                     msg = f'The column {col_name} has unknown data ' \
                           f'type {col_type}'
                     raise UnknownDataTypeException(msg)
                 else:
                     r[col_name] = func(
                         c,
                         self.current_data_record['IXFDCOLS'],
-                        pos,
-                        self.encoding
+                        pos
                     )
             except Exception as e:
                 logger.error(e)
                 sys.exit(1)
 
         return r
 
@@ -460,16 +455,15 @@
         self.parse_columns()
 
         logger.debug("Start writing in the csv file")
         with output as out:
             writer = csv.writer(out, delimiter=sep)
             cols = [
                 str(
-                    c['IXFCNAME'],
-                    encoding=self.encoding
+                    c['IXFCNAME'], encoding='utf-8'
                 ).strip() for c in self.columns_info
             ]
             writer.writerow(cols)
             for r in self.parse_data():
                 writer.writerow(r.values())
 
         logger.info(f'Number of rows is: {self.number_rows}')
```

### Comparing `db2ixf-0.1.7/src/db2ixf/logger.py` & `db2ixf-0.2.0/src/db2ixf/logger.py`

 * *Files identical despite different names*

### Comparing `db2ixf-0.1.7/src/db2ixf.egg-info/PKG-INFO` & `db2ixf-0.2.0/src/db2ixf.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 Metadata-Version: 2.1
 Name: db2ixf
-Version: 0.1.7
+Version: 0.2.0
 Summary: Parsing and processing of IBM eXchange format (IXF)
 Author-email: Ismail Hammounou <ismail.hammounou@gmail.com>
 Maintainer-email: Ismail Hammounou <ismail.hammounou@gmail.com>
 License: AGPL-3.0
 Project-URL: homepage, https://pypi.org/project/db2ixf/
 Project-URL: documentation, https://ismailhammounou.github.io/db2ixf/
 Project-URL: repository, https://github.com/ismailhammounou/db2ixf.git
 Project-URL: changelog, https://github.com/ismailhammounou/db2ixf/blob/main/CHANGELOG.md
 Keywords: PC,IXF,IBM,DB2,Development,Tools,Package,Parsing,Format,Data,Analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Python](https://img.shields.io/badge/Python-37|38|39|310|311-green.svg)](https://www.python.org/)
-[![License](https://img.shields.io/badge/License-AGPLv3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
-[![Pipeline](https://github.com/ismailhammounou/db2ixf/actions/workflows/db2ixf.yml/badge.svg)](https://github.com/ismailhammounou/db2ixf/actions/workflows/db2ixf.yml)
+
+[![Language](https://img.shields.io/pypi/pyversions/db2ixf?color=ffde57&logo=python&style=for-the-badge)](https://www.python.org/)
+[![License](https://img.shields.io/pypi/l/db2ixf?color=3775A9&style=for-the-badge&logo=unlicense)](https://www.gnu.org/licenses/agpl-3.0)
+
+[![Pipeline](https://img.shields.io/github/actions/workflow/status/ismailhammounou/db2ixf/db2ixf.yml?branch=main&style=for-the-badge&logo=gitHub-actions)](https://github.com/ismailhammounou/db2ixf/actions/workflows/db2ixf.yml)
+[![Release](https://img.shields.io/github/v/release/ismailhammounou/db2ixf?display_name=tag&sort=semver&style=for-the-badge&logo=semver)](https://github.com/ismailhammounou/db2ixf/releases/latest)
+[![Pypi](https://img.shields.io/pypi/v/db2ixf?color=3775A9&logo=pypi&style=for-the-badge)](https://github.com/ismailhammounou/db2ixf/releases/latest)
+
+
+[![Downloads](https://img.shields.io/pypi/dm/db2ixf?style=for-the-badge)](https://pypi.org/project/db2ixf/)
+
 
 # DB2IXF Parser
 
 <div align="center">
   <img src="https://github.com/ismailhammounou/db2ixf/blob/main/resources/images/db2ixf-logo.png?raw=true" alt="Logo" width="300" height="300">
 </div>
 
@@ -45,16 +52,16 @@
 - **Convert to multiple formats**: The parsed data can be easily converted to
   JSON, CSV, or Parquet format, providing flexibility for further analysis and
   integration with other systems.
 - **Support for file-like objects**: IXF Parser supports file-like objects as
   input, enabling direct parsing of IXF data from file objects, making it
   convenient for handling large datasets without the need for intermediate file
   storage.
-- **Minimal dependencies**: The package has only 2 dependencies, pyarrow and
-  typer, which are automatically installed alongside the package.
+- **Minimal dependencies**: The package has only 3 dependencies (pyarrow,
+  typer and ebcdic) which are automatically installed alongside the package.
 - **CLI**: command line tool called ``db2ixf`` comes with the package.
 
 ## Hypothesis
 
 - **One** IXF file contains **One** table.
 
 ## Getting Started
```

### Comparing `db2ixf-0.1.7/src/db2ixf.egg-info/SOURCES.txt` & `db2ixf-0.2.0/src/db2ixf.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/db2ixf/_version.py
 src/db2ixf/cli.py
 src/db2ixf/collectors.py
 src/db2ixf/constants.py
 src/db2ixf/encoders.py
 src/db2ixf/exceptions.py
 src/db2ixf/helpers.py
+src/db2ixf/ibmcodecs.py
 src/db2ixf/ixf.py
 src/db2ixf/logger.py
 src/db2ixf.egg-info/PKG-INFO
 src/db2ixf.egg-info/SOURCES.txt
 src/db2ixf.egg-info/dependency_links.txt
 src/db2ixf.egg-info/entry_points.txt
 src/db2ixf.egg-info/not-zip-safe
```

