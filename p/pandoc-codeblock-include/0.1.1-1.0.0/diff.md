# Comparing `tmp/pandoc-codeblock-include-0.1.1.tar.gz` & `tmp/pandoc_codeblock_include-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandoc-codeblock-include-0.1.1.tar", last modified: Mon Feb 22 21:17:04 2021, max compression
+gzip compressed data, was "pandoc_codeblock_include-1.0.0.tar", max compression
```

## Comparing `pandoc-codeblock-include-0.1.1.tar` & `pandoc_codeblock_include-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,5 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-22 21:17:04.599636 pandoc-codeblock-include-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1521 2021-02-22 21:16:56.000000 pandoc-codeblock-include-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       55 2021-02-22 21:16:56.000000 pandoc-codeblock-include-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    10773 2021-02-22 21:17:04.599636 pandoc-codeblock-include-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9177 2021-02-22 21:16:56.000000 pandoc-codeblock-include-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-22 21:17:04.599636 pandoc-codeblock-include-0.1.1/pandoc_codeblock_include.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10773 2021-02-22 21:17:04.000000 pandoc-codeblock-include-0.1.1/pandoc_codeblock_include.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      366 2021-02-22 21:17:04.000000 pandoc-codeblock-include-0.1.1/pandoc_codeblock_include.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-02-22 21:17:04.000000 pandoc-codeblock-include-0.1.1/pandoc_codeblock_include.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       76 2021-02-22 21:17:04.000000 pandoc-codeblock-include-0.1.1/pandoc_codeblock_include.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      110 2021-02-22 21:17:04.000000 pandoc-codeblock-include-0.1.1/pandoc_codeblock_include.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2021-02-22 21:17:04.000000 pandoc-codeblock-include-0.1.1/pandoc_codeblock_include.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4214 2021-02-22 21:16:56.000000 pandoc-codeblock-include-0.1.1/pandoc_codeblock_include.py
--rw-r--r--   0 runner    (1001) docker     (121)      286 2021-02-22 21:17:04.599636 pandoc-codeblock-include-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3623 2021-02-22 21:16:56.000000 pandoc-codeblock-include-0.1.1/setup.py
+-rw-r--r--   0        0        0     1521 2023-06-17 21:05:23.304509 pandoc_codeblock_include-1.0.0/LICENSE
+-rw-r--r--   0        0        0     8963 2023-06-17 21:05:23.304509 pandoc_codeblock_include-1.0.0/README.md
+-rw-r--r--   0        0        0     4225 2023-06-17 21:05:23.304509 pandoc_codeblock_include-1.0.0/pandoc_codeblock_include.py
+-rw-r--r--   0        0        0     2927 2023-06-17 21:05:23.304509 pandoc_codeblock_include-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    10073 1970-01-01 00:00:00.000000 pandoc_codeblock_include-1.0.0/PKG-INFO
```

### Comparing `pandoc-codeblock-include-0.1.1/LICENSE` & `pandoc_codeblock_include-1.0.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2018-2019, Christophe Demko
+Copyright (c) 2018-2023, Christophe Demko
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `pandoc-codeblock-include-0.1.1/PKG-INFO` & `pandoc_codeblock_include-1.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,95 +1,86 @@
 Metadata-Version: 2.1
 Name: pandoc-codeblock-include
-Version: 0.1.1
+Version: 1.0.0
 Summary: A pandoc filter for including file in block code
 Home-page: https://github.com/chdemko/pandoc-codeblock-include
+License: BSD-3-Clause
+Keywords: pandoc,filters,codeblock,include
 Author: Christophe Demko
 Author-email: chdemko@gmail.com
-Maintainer: Christophe Demko
-Maintainer-email: chdemko@gmail.com
-License: BSD-3-Clause
-Download-URL: https://github.com/chdemko/pandoc-codeblock-include/archive/develop.zip
-Description: # pandoc-codeblock-include
-        ![Python package](https://github.com/chdemko/pandoc-codeblock-include/workflows/Python%20package/badge.svg?branch=0.1.1)
-        [![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-codeblock-include/0.1.1.svg?logo=Codecov&logoColor=white)](https://coveralls.io/github/chdemko/pandoc-codeblock-include?branch=0.1.1)
-        [![Code Climate](https://codeclimate.com/github/chdemko/pandoc-codeblock-include/badges/gpa.svg)](https://codeclimate.com/github/chdemko/pandoc-codeblock-include/)
-        [![Code Beat](https://codebeat.co/badges/acdf2439-b9df-42df-8387-bd5f70e14314)](https://codebeat.co/projects/github-com-chdemko-pandoc-codeblock-include-develop/)
-        [![Codacy](https://img.shields.io/codacy/grade/26716ef242ba4089aff55eff7ca592a9.svg?logo=codacy&logoColor=white)](https://www.codacy.com/app/chdemko/pandoc-codeblock-include)
-        [![PyPI version](https://img.shields.io/pypi/v/pandoc-codeblock-include.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-codeblock-include/)
-        [![PyPI format](https://img.shields.io/pypi/format/pandoc-codeblock-include.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiYw92eBNAAAAgJJREFUeNrt3T1WwkAUgNH31Br3ogWptdAlgyvQxYgHeh0LKKxI+PHAzNyvRo8xlxl5CZKllBIaax0Rr5n53tqB3Ti3k7qPiEUpZQAAggEACAYAIBgAgGAAoG8Ey9oRAHBas9oR5NgcIDOz5TN4pjnIJiJeapwTWAFGfMR2CDRlJViUUuYAtAfgOSK+Jv5N8FbddlBGav4M7+9795jHUsqqTGtdFQIAxgE0jQCAaQCaRQDAdABNIgDgMADNIQDgcAB/EHxWjwCA4wDsvvahegQAHA+gCQQAnAagegQAnA6gagQAnAdArQhcDdx//D+ZeXvg95tHxDK21wbG2mTm/SWP38Wgcz+jMj8i4ikiVhMePrv0z3vnlO1/grS+DVoBehfuVwCAABAAAkAAqLO6nwP896Tz2ucIVgBbgAAQAAJAAAgAASAABIAAEAACQAAIADXZyfcD9P55A7W/c8oKYAsQAAJAAAgAASBzgJ5eB1sBBIAAEAACQAAIAJkDTM/9AO4HEAACQAAIAAEgANTPHMD9AFYAASAABIAAEAACQP3MAWq/H6D3OYYVwBYgAASAABAAAkDmAF5HWwEEgAAQAAJAAAgAASAABIAAEAACQAAIAAEgAASAABAAAkAACAABIAAEgAAQAAJAAAgAXVWj/x+g988FtAIIAAEgAASAABAAaqhfB1BFkJjdTNQAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-codeblock-include/)
-        [![License](https://img.shields.io/pypi/l/pandoc-codeblock-include.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAABmCAYAAAADI5lUAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiQKA106BAAABUNJREFUeNrtnV2IFlUYx3/P625qbrGlpWmWdaMVKau2EmpCrSDqxRpUUkr0SYVEFyFRUXQhfUAihTdCESVpKpKQpLZBsghltn605VVKpmZgGYvmbhpPFzMbWu3LO7szO1//H+zN7sw5c57nd8685+zMeY0quLsB04FW4A7gWmAMMAyRRbqBE8BRYCfwMfCNmXlfJ1iV5LcAbwBNimuu+Q54xcw21iSAuzcA7wOLFLtCsQl4yMxO9ymAu48HtgK3Kl6F5ACw0Mx++o8AYc/fBUxWnArN98DtZtYFULngDx8o+aXgZuDdi0YAd58fDv2iPMwzs+0WTvX2qfeXjv1Ak7n7DOBLxaOU3FYhWOQR5aS1AsxWHErLnArB8q4oJ+PM3buBoRFO6gJ2K3aZpBm4PMLxPXh09ijO2cTd90RNZkVhKzcSQAIICSAkgJAAQgIICSAkgJAAQgIICSAKT91gVOLui4EVKbZzvZm9kGD7rgHmEbw9NRoYCTQCvwInCd7UaQPaep/GLZUABP+ivDHFdo5KKPHTgNeAu6jyllXIk8A5d/8QeN7MjusWkGPcfRnBs5QtNSS/l3rgQaDT3e+UAPlN/iPA2wMYQa8APnH3ZgmQv+SPBlbGUNRw4D13r5MA+WIF0R67qsZNwMMSID+9vwF4IOZin5AA+WE+8W+O0eTuN0iAfNCSs3IlQMxMSqjciRIgH0wsmgCDNQU5CKxJMXHtMXwAHAJcndD1jSu0AGbWHkcSUmZEgmVfqltA9kkySQ0SIPsMyWnZEiAm/kiw7DMSIPt0AecSKvukBMg4ZvYXcCSh4g9LgHzwVc7KzcY00N0XAM+kmLitZrYqhnLagPsTuL7PCy0AwUJHS4oCHMpwok4AnboF5ONzwJFwFIiTd6pt5y4BssebMZbVA6xOszESIDrbiW+TrDVm9rMEyNdtwIHHgPMDLOoX4KW02yMB+ifBAWCgs4qnzex3CZBfXgS+7ee568xsQxYaIQH6Pwr0ELzk8WfEU48Dy7LSDgkwMAn2Eu2dRwceNbPfJEBxeD3s1bWwzcw+zdLFD9ZK4DHiX0CJwsEkbwXuvrrGkWBl5vTVXsGxxHBaDXE76+71CV+H9gpOiRM1HHPKzM5l7cIlQDxcX8Mxo9x9uAQoJktqOKYeuE8CFO/+P5NgabgWXnX3sRKgOMmfDWyJMJsaA+xw9wkSIN+Jr7j7U+HUdmTE028Bdrv73NKsA4Q9ZUmK7Ww3s7UxtaUZeAuYMYBirgpHgg3AcjP7sdACEOyE8XjKsq8dSI8H5gLPEu+jbfcCi9x9PbDKzDqKKkBeh/rpwN0Eu4Jcl1A19cBSYKm77wXWAZvN7AcJkG7ypwBfD3K1TeHPy+7eaGbnk65QHwL7ZlKKdY8AxmsWkC5XlqF+CdA3jWWoXwL0TUPK9V8mAdLlkpTrr5cA6VInAcpNfRnqHyzLu4jvBc3+0J8NGE6lfM1nB6UWPRJWHPRImNBnACEBhAQQEkBIACEBhAQQEkBIACEBhAQQ/8bcvRsYGuGcLuLbJ0/ESzPRvtW0x9z9MDBBsSslhyoE27eIcnKsAuxUHErLFxWC15tFOdli7m7AXmCK4lEq9gFTK+Hmx88pHqVjuZkFj4SZ2TZgs2JSGjaa2WcA1vsbd28AdgGTFZ9Csx+YaWZn4IKVQDM7DSwIDxDFve8v7E3+RQKEEhwFZgGbFKvC8REwK8wx/ytA70hgZvcQbInSobjlns6w1y++sOf/k+9qZ4ZTxKlAKzCH4OvfxgLDFNdM0k2wc/lRggW+LUBHtW8l+xuWwqBw5I0ApAAAAABJRU5ErkJggg==)](https://raw.githubusercontent.com/chdemko/pandoc-codeblock-include/0.1.1/LICENSE)
-        [![Python version](https://img.shields.io/pypi/pyversions/pandoc-codeblock-include.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-codeblock-include/)
-        [![Downloads](https://pepy.tech/badge/pandoc-codeblock-include)](https://pepy.tech/project/pandoc-codeblock-include)
-        [![Development Status](https://img.shields.io/pypi/status/pandoc-codeblock-include.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiUnX5lXMAAAAlBJREFUeNrt3b1qlEEUBuB3TNDCP7wDOwv/cgv+pDC3YcDe+xBFFFLoDWhhpxiD12Ch1mJsg7irjRLGYjcKEbLC92n223meMgQSzrx7Zs6wMAkAAAAAAAAAAAAAAAAAAAAw78r+H9RaLyZZT3Itydkkx5XpUH1L8iHJVpJHpZS3/yQAtdZjSe4muZXkiLrPpd0kG0lul1K+9xaA6eK/SHJFjQfhdZIbfYRg75N+z+IPytUkd3rpANM9/422P8jt4HIp5V3XDrBu8QdpKcnNPraA62o5WKt9bAHjJCfUcpDGpZRTXQNQ1fGAApVSDvPvz1qfrv+fvb9xAiAACACDVf80qrU+q7Wecwhs4BB4gM+ZXBRt6wBtOpO/uC7WARa3AyTJqJRyWgdo18xLIgEwBSAACABt3hOYAhZ7Cph9TyAAzQYgSZ4KQNsBGAlA2wFwCDQFIAAIAAKAACAACAACgAAgAAgAAoAAIAAIAIvniwC07aVvBM2wwN8I2kmyogO0Z5TkSZKVUsqnZfVou4PpAKYABAABYDHnfAFofM6feUh0D7Cw9wA7e6OeDtDwnD/rl90DNN6hdABTAAJAs5aTjJOcVIreT+H/68DXuQNsW+bB+thHAF6p42Btdp4iaq0XMnk2bkk9B2U3yaVSyvtOHWD6Fu2Geg7Ow66Ln/x+OvZokueZPBjN/NtKslZK+dHLGDh9g3YtyYNpa2F+2/79vhb/VwfYN/acz+RFytVMno/3puDh+prJ8/GbSR730fYBAAAAAAAAAAAAAAAAAACAYfkJuHbYr8dtGYwAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-codeblock-include/)
-        [![Docs](https://img.shields.io/badge/docs-wiki-green.svg?logo=read-the-docs&logoColor=white)](https://github.com/chdemko/pandoc-codeblock-include/wiki)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAwCAYAAABXAvmHAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAAOxAAADsQBlSsOGwAAABl0RVh0U29mdHdhcmUAd3d3Lmlua3NjYXBlLm9yZ5vuPBoAAANwSURBVGiB7Zndi1VlFIefNZPR9GkTmSkOhIZYeBFiIDEYNUREXVQEQUhK4hdEf0GQf0IUU2BdhHUjNQTpRRdl0NdFXYRZCA0SJTZ9CJEDmY49Xewzw57Xfc7+OGfOEJzn5vCuvfbav/Wutd+993tgwIAB/2ui3xdUVwKPAbcDPwDHIuJiv3XURr1HPaTOuphpdeNy6ytEvUbdoX5pZ75Xr15uvQuoa9WX1N9KhOfZsdyih9QJ9Yg6V0P4PF8sl/CV6gvq6QaiU7b0U/g29bB6oQfC5znUD+HXqu/2UHSeWbNltjJDDXKYBJ4EfgFeBo42iNGO64BnexhvMeoqsxt0Vh3L2V/tYRVOqZUfsHUrcCcwDJyKiJ9y9g9rxunERuDBqs51Ezjb+t2UrwDwcM04Zeyv6lj7XUj9GtgCzABHgA3AI3XjlDAH3BERZ3ocF9TnetjvnThYRU+TCowAZ4DRuufWZAYYi4hLnZxqL6MR8TfwVlNVNVgNPL4kkdUN6uU+tNEnZVo6VkC9tcgeEdPAR83Sr8V29e5ODmUttLvDscn6ehpReUldhLpebTvL6rD6Yx/a6C/1xnY6OlVgf6fjEXEZeKPSbHTHDcAztc5QR9Q/1OOJfSgZr1b/6UMVTrTT2m6GnwZuKbBvVRfW/4iYAaaqT01jNqvjRQfaJdDuxhkBdia21xqKqku1m9ls+2OetIXuN9sGSVvpRB/a6KK6JtVbVIHnS3JcD0wktterTE6XrAB2pcZ0JkfJ+r+MA8n4MHC+sbTq7FGH84a0AjvJ+ryMR819D0TEeeDtruWVMwbcmzcsJGD2GbevYqBhYE9i69eTeVV+kK/ANrJPxqrsNrcdGBEngU+701aJb/ODfAJ1xAPcBjyR2Ja6Cu9FxOm8IZ/AdIOA6c08RfYhshQcB/amxnwCXwHf1Qw6rm6eH7T2+d9sJK+YObJJmYiIByLiXEfv1kPs15IHWcpk4rPOZpu7ec6qB9W1tVNWR9UX1Z8LEhgvuNgVr7vq+w1E/6t+rD6lrqgtvCCRq0x2i9U1rQulHEj8Hqoh/E/1FXVT16IrJjZVIOJk4hPqZyXCv1H3qtf3RXhO3M3qsQJB2xO/dS2ReS6o76j39UpP438p1QlgK3BTy/R5RHyQ+AyRbTveBZwDjkbE702vOWDAgCv5DyyzjR7/CUzHAAAAAElFTkSuQmCC)](https://pypi.org/project/black/)
-        
-        license icon by [Daniel Bruce](https://www.iconfinder.com/icons/216659/license_icon), format icon by [Picol](https://www.iconfinder.com/icons/103509/document_text_icon), status icon by [Just Icon](https://www.iconfinder.com/icons/2672768/app_battery_essential_object_status_ui_ux_icon), code style icon by [Google Material Design icons](https://www.iconfinder.com/icons/352148/style_icon)
-        
-        
-        *pandoc-codeblock-include* is a [pandoc] filter for including files in `CodeBlock` elements.
-        
-        [pandoc]: http://pandoc.org/
-        
-        Documentation
-        -------------
-        
-        See the [wiki pages](https://github.com/chdemko/pandoc-codeblock-include/wiki).
-        
-        Usage
-        -----
-        
-        To apply the filter, use the following option with pandoc:
-        
-            --filter pandoc-codeblock-include
-        
-        Installation
-        ------------
-        
-        *pandoc-codeblock-include* requires [python], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows]. Either python 2.7 or 3.x will do.
-        
-        Install *pandoc-codeblock-include* as root using the bash command
-        
-            pip install pandoc-codeblock-include
-        
-        To upgrade to the most recent release, use
-        
-            pip install --upgrade pandoc-codeblock-include
-        
-        To upgrade to the current code, use
-        
-            pip install --upgrade --force git+https://github.com/chdemko/pandoc-codeblock-include
-        
-        `pip` is a script that downloads and installs modules from the Python Package Index, [PyPI].  It should come installed with your python distribution. If you are running linux, `pip` may be bundled separately. On a Debian-based system (including Ubuntu), you can install it as root using
-        
-            apt-get update
-            apt-get install python-pip
-        
-        [python]: https://www.python.org
-        [on Windows]: https://www.python.org/downloads/windows
-        [PyPI]: https://pypi.org
-        
-        
-        Getting Help
-        ------------
-        
-        If you have any difficulties with *pandoc-codeblock-include*, please feel welcome to [file an issue] on github so that we can help.
-        
-        [file an issue]: https://github.com/chdemko/pandoc-codeblock-include/issues
-        
-        
-Keywords: pandoc filters codeblock include
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
-Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Documentation
+Classifier: Topic :: Text Processing :: Filters
+Requires-Dist: panflute (>=2.3.0,<3.0.0)
 Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: test
+
+Installation
+============
+
+![Python package](https://github.com/chdemko/pandoc-codeblock-include/workflows/Python%20package/badge.svg?branch=develop)
+[![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-codeblock-include/develop.svg?logo=Codecov&logoColor=white)](https://coveralls.io/github/chdemko/pandoc-codeblock-include?branch=develop)
+[![Code Climate](https://codeclimate.com/github/chdemko/pandoc-codeblock-include/badges/gpa.svg)](https://codeclimate.com/github/chdemko/pandoc-codeblock-include/)
+[![Code Beat](https://codebeat.co/badges/c0e680bd-9c47-4180-8d3f-b706905d0e73)](https://codebeat.co/projects/github-com-chdemko-pandoc-codeblock-include-develop/)
+[![Codacy](https://img.shields.io/codacy/grade/26716ef242ba4089aff55eff7ca592a9.svg?logo=codacy&logoColor=white)](https://app.codacy.com/gh/chdemko/pandoc-codeblock-include/)
+[![PyPI version](https://img.shields.io/pypi/v/pandoc-codeblock-include.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-codeblock-include/)
+[![PyPI format](https://img.shields.io/pypi/format/pandoc-codeblock-include.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiYw92eBNAAAAgJJREFUeNrt3T1WwkAUgNH31Br3ogWptdAlgyvQxYgHeh0LKKxI+PHAzNyvRo8xlxl5CZKllBIaax0Rr5n53tqB3Ti3k7qPiEUpZQAAggEACAYAIBgAgGAAoG8Ey9oRAHBas9oR5NgcIDOz5TN4pjnIJiJeapwTWAFGfMR2CDRlJViUUuYAtAfgOSK+Jv5N8FbddlBGav4M7+9795jHUsqqTGtdFQIAxgE0jQCAaQCaRQDAdABNIgDgMADNIQDgcAB/EHxWjwCA4wDsvvahegQAHA+gCQQAnAagegQAnA6gagQAnAdArQhcDdx//D+ZeXvg95tHxDK21wbG2mTm/SWP38Wgcz+jMj8i4ikiVhMePrv0z3vnlO1/grS+DVoBehfuVwCAABAAAkAAqLO6nwP896Tz2ucIVgBbgAAQAAJAAAgAASAABIAAEAACQAAIADXZyfcD9P55A7W/c8oKYAsQAAJAAAgAASBzgJ5eB1sBBIAAEAACQAAIAJkDTM/9AO4HEAACQAAIAAEgANTPHMD9AFYAASAABIAAEAACQP3MAWq/H6D3OYYVwBYgAASAABAAAkDmAF5HWwEEgAAQAAJAAAgAASAABIAAEAACQAAIAAEgAASAABAAAkAACAABIAAEgAAQAAJAAAgAXVWj/x+g988FtAIIAAEgAASAABAAaqhfB1BFkJjdTNQAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-codeblock-include/)
+[![License](https://img.shields.io/pypi/l/pandoc-codeblock-include.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAABmCAYAAAADI5lUAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiQKA106BAAABUNJREFUeNrtnV2IFlUYx3/P625qbrGlpWmWdaMVKau2EmpCrSDqxRpUUkr0SYVEFyFRUXQhfUAihTdCESVpKpKQpLZBsghltn605VVKpmZgGYvmbhpPFzMbWu3LO7szO1//H+zN7sw5c57nd8685+zMeY0quLsB04FW4A7gWmAMMAyRRbqBE8BRYCfwMfCNmXlfJ1iV5LcAbwBNimuu+Q54xcw21iSAuzcA7wOLFLtCsQl4yMxO9ymAu48HtgK3Kl6F5ACw0Mx++o8AYc/fBUxWnArN98DtZtYFULngDx8o+aXgZuDdi0YAd58fDv2iPMwzs+0WTvX2qfeXjv1Ak7n7DOBLxaOU3FYhWOQR5aS1AsxWHErLnArB8q4oJ+PM3buBoRFO6gJ2K3aZpBm4PMLxPXh09ijO2cTd90RNZkVhKzcSQAIICSAkgJAAQgIICSAkgJAAQgIICSAKT91gVOLui4EVKbZzvZm9kGD7rgHmEbw9NRoYCTQCvwInCd7UaQPaep/GLZUABP+ivDHFdo5KKPHTgNeAu6jyllXIk8A5d/8QeN7MjusWkGPcfRnBs5QtNSS/l3rgQaDT3e+UAPlN/iPA2wMYQa8APnH3ZgmQv+SPBlbGUNRw4D13r5MA+WIF0R67qsZNwMMSID+9vwF4IOZin5AA+WE+8W+O0eTuN0iAfNCSs3IlQMxMSqjciRIgH0wsmgCDNQU5CKxJMXHtMXwAHAJcndD1jSu0AGbWHkcSUmZEgmVfqltA9kkySQ0SIPsMyWnZEiAm/kiw7DMSIPt0AecSKvukBMg4ZvYXcCSh4g9LgHzwVc7KzcY00N0XAM+kmLitZrYqhnLagPsTuL7PCy0AwUJHS4oCHMpwok4AnboF5ONzwJFwFIiTd6pt5y4BssebMZbVA6xOszESIDrbiW+TrDVm9rMEyNdtwIHHgPMDLOoX4KW02yMB+ifBAWCgs4qnzex3CZBfXgS+7ee568xsQxYaIQH6Pwr0ELzk8WfEU48Dy7LSDgkwMAn2Eu2dRwceNbPfJEBxeD3s1bWwzcw+zdLFD9ZK4DHiX0CJwsEkbwXuvrrGkWBl5vTVXsGxxHBaDXE76+71CV+H9gpOiRM1HHPKzM5l7cIlQDxcX8Mxo9x9uAQoJktqOKYeuE8CFO/+P5NgabgWXnX3sRKgOMmfDWyJMJsaA+xw9wkSIN+Jr7j7U+HUdmTE028Bdrv73NKsA4Q9ZUmK7Ww3s7UxtaUZeAuYMYBirgpHgg3AcjP7sdACEOyE8XjKsq8dSI8H5gLPEu+jbfcCi9x9PbDKzDqKKkBeh/rpwN0Eu4Jcl1A19cBSYKm77wXWAZvN7AcJkG7ypwBfD3K1TeHPy+7eaGbnk65QHwL7ZlKKdY8AxmsWkC5XlqF+CdA3jWWoXwL0TUPK9V8mAdLlkpTrr5cA6VInAcpNfRnqHyzLu4jvBc3+0J8NGE6lfM1nB6UWPRJWHPRImNBnACEBhAQQEkBIACEBhAQQEkBIACEBhAQQ/8bcvRsYGuGcLuLbJ0/ESzPRvtW0x9z9MDBBsSslhyoE27eIcnKsAuxUHErLFxWC15tFOdli7m7AXmCK4lEq9gFTK+Hmx88pHqVjuZkFj4SZ2TZgs2JSGjaa2WcA1vsbd28AdgGTFZ9Csx+YaWZn4IKVQDM7DSwIDxDFve8v7E3+RQKEEhwFZgGbFKvC8REwK8wx/ytA70hgZvcQbInSobjlns6w1y++sOf/k+9qZ4ZTxKlAKzCH4OvfxgLDFNdM0k2wc/lRggW+LUBHtW8l+xuWwqBw5I0ApAAAAABJRU5ErkJggg==)](https://raw.githubusercontent.com/chdemko/pandoc-codeblock-include/develop/LICENSE)
+[![Python version](https://img.shields.io/pypi/pyversions/pandoc-codeblock-include.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-codeblock-include/)
+[![Downloads](https://pepy.tech/badge/pandoc-codeblock-include)](https://pepy.tech/project/pandoc-codeblock-include)
+[![Development Status](https://img.shields.io/pypi/status/pandoc-codeblock-include.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiUnX5lXMAAAAlBJREFUeNrt3b1qlEEUBuB3TNDCP7wDOwv/cgv+pDC3YcDe+xBFFFLoDWhhpxiD12Ch1mJsg7irjRLGYjcKEbLC92n223meMgQSzrx7Zs6wMAkAAAAAAAAAAAAAAAAAAAAw78r+H9RaLyZZT3Itydkkx5XpUH1L8iHJVpJHpZS3/yQAtdZjSe4muZXkiLrPpd0kG0lul1K+9xaA6eK/SHJFjQfhdZIbfYRg75N+z+IPytUkd3rpANM9/422P8jt4HIp5V3XDrBu8QdpKcnNPraA62o5WKt9bAHjJCfUcpDGpZRTXQNQ1fGAApVSDvPvz1qfrv+fvb9xAiAACACDVf80qrU+q7Wecwhs4BB4gM+ZXBRt6wBtOpO/uC7WARa3AyTJqJRyWgdo18xLIgEwBSAACABt3hOYAhZ7Cph9TyAAzQYgSZ4KQNsBGAlA2wFwCDQFIAAIAAKAACAACAACgAAgAAgAAoAAIAAIAIvniwC07aVvBM2wwN8I2kmyogO0Z5TkSZKVUsqnZfVou4PpAKYABAABYDHnfAFofM6feUh0D7Cw9wA7e6OeDtDwnD/rl90DNN6hdABTAAJAs5aTjJOcVIreT+H/68DXuQNsW+bB+thHAF6p42Btdp4iaq0XMnk2bkk9B2U3yaVSyvtOHWD6Fu2Geg7Ow66Ln/x+OvZokueZPBjN/NtKslZK+dHLGDh9g3YtyYNpa2F+2/79vhb/VwfYN/acz+RFytVMno/3puDh+prJ8/GbSR730fYBAAAAAAAAAAAAAAAAAACAYfkJuHbYr8dtGYwAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-codeblock-include/)
+[![Docs](https://img.shields.io/badge/docs-wiki-green.svg?logo=read-the-docs&logoColor=white)](https://github.com/chdemko/pandoc-codeblock-include/wiki)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAwCAYAAABXAvmHAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAAOxAAADsQBlSsOGwAAABl0RVh0U29mdHdhcmUAd3d3Lmlua3NjYXBlLm9yZ5vuPBoAAANwSURBVGiB7Zndi1VlFIefNZPR9GkTmSkOhIZYeBFiIDEYNUREXVQEQUhK4hdEf0GQf0IUU2BdhHUjNQTpRRdl0NdFXYRZCA0SJTZ9CJEDmY49Xewzw57Xfc7+OGfOEJzn5vCuvfbav/Wutd+993tgwIAB/2ui3xdUVwKPAbcDPwDHIuJiv3XURr1HPaTOuphpdeNy6ytEvUbdoX5pZ75Xr15uvQuoa9WX1N9KhOfZsdyih9QJ9Yg6V0P4PF8sl/CV6gvq6QaiU7b0U/g29bB6oQfC5znUD+HXqu/2UHSeWbNltjJDDXKYBJ4EfgFeBo42iNGO64BnexhvMeoqsxt0Vh3L2V/tYRVOqZUfsHUrcCcwDJyKiJ9y9g9rxunERuDBqs51Ezjb+t2UrwDwcM04Zeyv6lj7XUj9GtgCzABHgA3AI3XjlDAH3BERZ3ocF9TnetjvnThYRU+TCowAZ4DRuufWZAYYi4hLnZxqL6MR8TfwVlNVNVgNPL4kkdUN6uU+tNEnZVo6VkC9tcgeEdPAR83Sr8V29e5ODmUttLvDscn6ehpReUldhLpebTvL6rD6Yx/a6C/1xnY6OlVgf6fjEXEZeKPSbHTHDcAztc5QR9Q/1OOJfSgZr1b/6UMVTrTT2m6GnwZuKbBvVRfW/4iYAaaqT01jNqvjRQfaJdDuxhkBdia21xqKqku1m9ls+2OetIXuN9sGSVvpRB/a6KK6JtVbVIHnS3JcD0wktterTE6XrAB2pcZ0JkfJ+r+MA8n4MHC+sbTq7FGH84a0AjvJ+ryMR819D0TEeeDtruWVMwbcmzcsJGD2GbevYqBhYE9i69eTeVV+kK/ANrJPxqrsNrcdGBEngU+701aJb/ODfAJ1xAPcBjyR2Ja6Cu9FxOm8IZ/AdIOA6c08RfYhshQcB/amxnwCXwHf1Qw6rm6eH7T2+d9sJK+YObJJmYiIByLiXEfv1kPs15IHWcpk4rPOZpu7ec6qB9W1tVNWR9UX1Z8LEhgvuNgVr7vq+w1E/6t+rD6lrqgtvCCRq0x2i9U1rQulHEj8Hqoh/E/1FXVT16IrJjZVIOJk4hPqZyXCv1H3qtf3RXhO3M3qsQJB2xO/dS2ReS6o76j39UpP438p1QlgK3BTy/R5RHyQ+AyRbTveBZwDjkbE702vOWDAgCv5DyyzjR7/CUzHAAAAAElFTkSuQmCC)](https://pypi.org/project/black/)
+
+license icon by [Daniel Bruce](https://www.iconfinder.com/icons/216659/license_icon), format icon by [Picol](https://www.iconfinder.com/icons/103509/document_text_icon), status icon by [Just Icon](https://www.iconfinder.com/icons/2672768/app_battery_essential_object_status_ui_ux_icon), code style icon by [Google Material Design icons](https://www.iconfinder.com/icons/352148/style_icon)
+
+
+*pandoc-codeblock-include* is a [pandoc] filter for including files in `CodeBlock` elements.
+
+[pandoc]: http://pandoc.org/
+
+Instructions
+------------
+
+*pandoc-codeblock-include* requires [python], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows]. Either python 2.7 or 3.x will do.
+
+Install *pandoc-codeblock-include* as root using the bash command
+
+    pip install pandoc-codeblock-include
+
+To upgrade to the most recent release, use
+
+    pip install --upgrade pandoc-codeblock-include
+
+To upgrade to the current code, use
+
+    pip install --upgrade --force git+https://github.com/chdemko/pandoc-codeblock-include
+
+`pip` is a script that downloads and installs modules from the Python Package Index, [PyPI].  It should come installed with your python distribution. If you are running linux, `pip` may be bundled separately. On a Debian-based system (including Ubuntu), you can install it as root using
+
+    apt-get update
+    apt-get install python-pip
+
+[python]: https://www.python.org
+[on Windows]: https://www.python.org/downloads/windows
+[PyPI]: https://pypi.org
+
+
+Getting Help
+------------
+
+If you have any difficulties with *pandoc-codeblock-include*, please feel welcome to [file an issue] on github so that we can help.
+
+[file an issue]: https://github.com/chdemko/pandoc-codeblock-include/issues
+
+
```

### Comparing `pandoc-codeblock-include-0.1.1/README.md` & `pandoc_codeblock_include-1.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,32 @@
-# pandoc-codeblock-include
-![Python package](https://github.com/chdemko/pandoc-codeblock-include/workflows/Python%20package/badge.svg?branch=0.1.1)
-[![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-codeblock-include/0.1.1.svg?logo=Codecov&logoColor=white)](https://coveralls.io/github/chdemko/pandoc-codeblock-include?branch=0.1.1)
+Installation
+============
+
+![Python package](https://github.com/chdemko/pandoc-codeblock-include/workflows/Python%20package/badge.svg?branch=develop)
+[![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-codeblock-include/develop.svg?logo=Codecov&logoColor=white)](https://coveralls.io/github/chdemko/pandoc-codeblock-include?branch=develop)
 [![Code Climate](https://codeclimate.com/github/chdemko/pandoc-codeblock-include/badges/gpa.svg)](https://codeclimate.com/github/chdemko/pandoc-codeblock-include/)
-[![Code Beat](https://codebeat.co/badges/acdf2439-b9df-42df-8387-bd5f70e14314)](https://codebeat.co/projects/github-com-chdemko-pandoc-codeblock-include-develop/)
-[![Codacy](https://img.shields.io/codacy/grade/26716ef242ba4089aff55eff7ca592a9.svg?logo=codacy&logoColor=white)](https://www.codacy.com/app/chdemko/pandoc-codeblock-include)
+[![Code Beat](https://codebeat.co/badges/c0e680bd-9c47-4180-8d3f-b706905d0e73)](https://codebeat.co/projects/github-com-chdemko-pandoc-codeblock-include-develop/)
+[![Codacy](https://img.shields.io/codacy/grade/26716ef242ba4089aff55eff7ca592a9.svg?logo=codacy&logoColor=white)](https://app.codacy.com/gh/chdemko/pandoc-codeblock-include/)
 [![PyPI version](https://img.shields.io/pypi/v/pandoc-codeblock-include.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-codeblock-include/)
 [![PyPI format](https://img.shields.io/pypi/format/pandoc-codeblock-include.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiYw92eBNAAAAgJJREFUeNrt3T1WwkAUgNH31Br3ogWptdAlgyvQxYgHeh0LKKxI+PHAzNyvRo8xlxl5CZKllBIaax0Rr5n53tqB3Ti3k7qPiEUpZQAAggEACAYAIBgAgGAAoG8Ey9oRAHBas9oR5NgcIDOz5TN4pjnIJiJeapwTWAFGfMR2CDRlJViUUuYAtAfgOSK+Jv5N8FbddlBGav4M7+9795jHUsqqTGtdFQIAxgE0jQCAaQCaRQDAdABNIgDgMADNIQDgcAB/EHxWjwCA4wDsvvahegQAHA+gCQQAnAagegQAnA6gagQAnAdArQhcDdx//D+ZeXvg95tHxDK21wbG2mTm/SWP38Wgcz+jMj8i4ikiVhMePrv0z3vnlO1/grS+DVoBehfuVwCAABAAAkAAqLO6nwP896Tz2ucIVgBbgAAQAAJAAAgAASAABIAAEAACQAAIADXZyfcD9P55A7W/c8oKYAsQAAJAAAgAASBzgJ5eB1sBBIAAEAACQAAIAJkDTM/9AO4HEAACQAAIAAEgANTPHMD9AFYAASAABIAAEAACQP3MAWq/H6D3OYYVwBYgAASAABAAAkDmAF5HWwEEgAAQAAJAAAgAASAABIAAEAACQAAIAAEgAASAABAAAkAACAABIAAEgAAQAAJAAAgAXVWj/x+g988FtAIIAAEgAASAABAAaqhfB1BFkJjdTNQAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-codeblock-include/)
-[![License](https://img.shields.io/pypi/l/pandoc-codeblock-include.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAABmCAYAAAADI5lUAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiQKA106BAAABUNJREFUeNrtnV2IFlUYx3/P625qbrGlpWmWdaMVKau2EmpCrSDqxRpUUkr0SYVEFyFRUXQhfUAihTdCESVpKpKQpLZBsghltn605VVKpmZgGYvmbhpPFzMbWu3LO7szO1//H+zN7sw5c57nd8685+zMeY0quLsB04FW4A7gWmAMMAyRRbqBE8BRYCfwMfCNmXlfJ1iV5LcAbwBNimuu+Q54xcw21iSAuzcA7wOLFLtCsQl4yMxO9ymAu48HtgK3Kl6F5ACw0Mx++o8AYc/fBUxWnArN98DtZtYFULngDx8o+aXgZuDdi0YAd58fDv2iPMwzs+0WTvX2qfeXjv1Ak7n7DOBLxaOU3FYhWOQR5aS1AsxWHErLnArB8q4oJ+PM3buBoRFO6gJ2K3aZpBm4PMLxPXh09ijO2cTd90RNZkVhKzcSQAIICSAkgJAAQgIICSAkgJAAQgIICSAKT91gVOLui4EVKbZzvZm9kGD7rgHmEbw9NRoYCTQCvwInCd7UaQPaep/GLZUABP+ivDHFdo5KKPHTgNeAu6jyllXIk8A5d/8QeN7MjusWkGPcfRnBs5QtNSS/l3rgQaDT3e+UAPlN/iPA2wMYQa8APnH3ZgmQv+SPBlbGUNRw4D13r5MA+WIF0R67qsZNwMMSID+9vwF4IOZin5AA+WE+8W+O0eTuN0iAfNCSs3IlQMxMSqjciRIgH0wsmgCDNQU5CKxJMXHtMXwAHAJcndD1jSu0AGbWHkcSUmZEgmVfqltA9kkySQ0SIPsMyWnZEiAm/kiw7DMSIPt0AecSKvukBMg4ZvYXcCSh4g9LgHzwVc7KzcY00N0XAM+kmLitZrYqhnLagPsTuL7PCy0AwUJHS4oCHMpwok4AnboF5ONzwJFwFIiTd6pt5y4BssebMZbVA6xOszESIDrbiW+TrDVm9rMEyNdtwIHHgPMDLOoX4KW02yMB+ifBAWCgs4qnzex3CZBfXgS+7ee568xsQxYaIQH6Pwr0ELzk8WfEU48Dy7LSDgkwMAn2Eu2dRwceNbPfJEBxeD3s1bWwzcw+zdLFD9ZK4DHiX0CJwsEkbwXuvrrGkWBl5vTVXsGxxHBaDXE76+71CV+H9gpOiRM1HHPKzM5l7cIlQDxcX8Mxo9x9uAQoJktqOKYeuE8CFO/+P5NgabgWXnX3sRKgOMmfDWyJMJsaA+xw9wkSIN+Jr7j7U+HUdmTE028Bdrv73NKsA4Q9ZUmK7Ww3s7UxtaUZeAuYMYBirgpHgg3AcjP7sdACEOyE8XjKsq8dSI8H5gLPEu+jbfcCi9x9PbDKzDqKKkBeh/rpwN0Eu4Jcl1A19cBSYKm77wXWAZvN7AcJkG7ypwBfD3K1TeHPy+7eaGbnk65QHwL7ZlKKdY8AxmsWkC5XlqF+CdA3jWWoXwL0TUPK9V8mAdLlkpTrr5cA6VInAcpNfRnqHyzLu4jvBc3+0J8NGE6lfM1nB6UWPRJWHPRImNBnACEBhAQQEkBIACEBhAQQEkBIACEBhAQQ/8bcvRsYGuGcLuLbJ0/ESzPRvtW0x9z9MDBBsSslhyoE27eIcnKsAuxUHErLFxWC15tFOdli7m7AXmCK4lEq9gFTK+Hmx88pHqVjuZkFj4SZ2TZgs2JSGjaa2WcA1vsbd28AdgGTFZ9Csx+YaWZn4IKVQDM7DSwIDxDFve8v7E3+RQKEEhwFZgGbFKvC8REwK8wx/ytA70hgZvcQbInSobjlns6w1y++sOf/k+9qZ4ZTxKlAKzCH4OvfxgLDFNdM0k2wc/lRggW+LUBHtW8l+xuWwqBw5I0ApAAAAABJRU5ErkJggg==)](https://raw.githubusercontent.com/chdemko/pandoc-codeblock-include/0.1.1/LICENSE)
+[![License](https://img.shields.io/pypi/l/pandoc-codeblock-include.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAABmCAYAAAADI5lUAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiQKA106BAAABUNJREFUeNrtnV2IFlUYx3/P625qbrGlpWmWdaMVKau2EmpCrSDqxRpUUkr0SYVEFyFRUXQhfUAihTdCESVpKpKQpLZBsghltn605VVKpmZgGYvmbhpPFzMbWu3LO7szO1//H+zN7sw5c57nd8685+zMeY0quLsB04FW4A7gWmAMMAyRRbqBE8BRYCfwMfCNmXlfJ1iV5LcAbwBNimuu+Q54xcw21iSAuzcA7wOLFLtCsQl4yMxO9ymAu48HtgK3Kl6F5ACw0Mx++o8AYc/fBUxWnArN98DtZtYFULngDx8o+aXgZuDdi0YAd58fDv2iPMwzs+0WTvX2qfeXjv1Ak7n7DOBLxaOU3FYhWOQR5aS1AsxWHErLnArB8q4oJ+PM3buBoRFO6gJ2K3aZpBm4PMLxPXh09ijO2cTd90RNZkVhKzcSQAIICSAkgJAAQgIICSAkgJAAQgIICSAKT91gVOLui4EVKbZzvZm9kGD7rgHmEbw9NRoYCTQCvwInCd7UaQPaep/GLZUABP+ivDHFdo5KKPHTgNeAu6jyllXIk8A5d/8QeN7MjusWkGPcfRnBs5QtNSS/l3rgQaDT3e+UAPlN/iPA2wMYQa8APnH3ZgmQv+SPBlbGUNRw4D13r5MA+WIF0R67qsZNwMMSID+9vwF4IOZin5AA+WE+8W+O0eTuN0iAfNCSs3IlQMxMSqjciRIgH0wsmgCDNQU5CKxJMXHtMXwAHAJcndD1jSu0AGbWHkcSUmZEgmVfqltA9kkySQ0SIPsMyWnZEiAm/kiw7DMSIPt0AecSKvukBMg4ZvYXcCSh4g9LgHzwVc7KzcY00N0XAM+kmLitZrYqhnLagPsTuL7PCy0AwUJHS4oCHMpwok4AnboF5ONzwJFwFIiTd6pt5y4BssebMZbVA6xOszESIDrbiW+TrDVm9rMEyNdtwIHHgPMDLOoX4KW02yMB+ifBAWCgs4qnzex3CZBfXgS+7ee568xsQxYaIQH6Pwr0ELzk8WfEU48Dy7LSDgkwMAn2Eu2dRwceNbPfJEBxeD3s1bWwzcw+zdLFD9ZK4DHiX0CJwsEkbwXuvrrGkWBl5vTVXsGxxHBaDXE76+71CV+H9gpOiRM1HHPKzM5l7cIlQDxcX8Mxo9x9uAQoJktqOKYeuE8CFO/+P5NgabgWXnX3sRKgOMmfDWyJMJsaA+xw9wkSIN+Jr7j7U+HUdmTE028Bdrv73NKsA4Q9ZUmK7Ww3s7UxtaUZeAuYMYBirgpHgg3AcjP7sdACEOyE8XjKsq8dSI8H5gLPEu+jbfcCi9x9PbDKzDqKKkBeh/rpwN0Eu4Jcl1A19cBSYKm77wXWAZvN7AcJkG7ypwBfD3K1TeHPy+7eaGbnk65QHwL7ZlKKdY8AxmsWkC5XlqF+CdA3jWWoXwL0TUPK9V8mAdLlkpTrr5cA6VInAcpNfRnqHyzLu4jvBc3+0J8NGE6lfM1nB6UWPRJWHPRImNBnACEBhAQQEkBIACEBhAQQEkBIACEBhAQQ/8bcvRsYGuGcLuLbJ0/ESzPRvtW0x9z9MDBBsSslhyoE27eIcnKsAuxUHErLFxWC15tFOdli7m7AXmCK4lEq9gFTK+Hmx88pHqVjuZkFj4SZ2TZgs2JSGjaa2WcA1vsbd28AdgGTFZ9Csx+YaWZn4IKVQDM7DSwIDxDFve8v7E3+RQKEEhwFZgGbFKvC8REwK8wx/ytA70hgZvcQbInSobjlns6w1y++sOf/k+9qZ4ZTxKlAKzCH4OvfxgLDFNdM0k2wc/lRggW+LUBHtW8l+xuWwqBw5I0ApAAAAABJRU5ErkJggg==)](https://raw.githubusercontent.com/chdemko/pandoc-codeblock-include/develop/LICENSE)
 [![Python version](https://img.shields.io/pypi/pyversions/pandoc-codeblock-include.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-codeblock-include/)
 [![Downloads](https://pepy.tech/badge/pandoc-codeblock-include)](https://pepy.tech/project/pandoc-codeblock-include)
 [![Development Status](https://img.shields.io/pypi/status/pandoc-codeblock-include.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiUnX5lXMAAAAlBJREFUeNrt3b1qlEEUBuB3TNDCP7wDOwv/cgv+pDC3YcDe+xBFFFLoDWhhpxiD12Ch1mJsg7irjRLGYjcKEbLC92n223meMgQSzrx7Zs6wMAkAAAAAAAAAAAAAAAAAAAAw78r+H9RaLyZZT3Itydkkx5XpUH1L8iHJVpJHpZS3/yQAtdZjSe4muZXkiLrPpd0kG0lul1K+9xaA6eK/SHJFjQfhdZIbfYRg75N+z+IPytUkd3rpANM9/422P8jt4HIp5V3XDrBu8QdpKcnNPraA62o5WKt9bAHjJCfUcpDGpZRTXQNQ1fGAApVSDvPvz1qfrv+fvb9xAiAACACDVf80qrU+q7Wecwhs4BB4gM+ZXBRt6wBtOpO/uC7WARa3AyTJqJRyWgdo18xLIgEwBSAACABt3hOYAhZ7Cph9TyAAzQYgSZ4KQNsBGAlA2wFwCDQFIAAIAAKAACAACAACgAAgAAgAAoAAIAAIAIvniwC07aVvBM2wwN8I2kmyogO0Z5TkSZKVUsqnZfVou4PpAKYABAABYDHnfAFofM6feUh0D7Cw9wA7e6OeDtDwnD/rl90DNN6hdABTAAJAs5aTjJOcVIreT+H/68DXuQNsW+bB+thHAF6p42Btdp4iaq0XMnk2bkk9B2U3yaVSyvtOHWD6Fu2Geg7Ow66Ln/x+OvZokueZPBjN/NtKslZK+dHLGDh9g3YtyYNpa2F+2/79vhb/VwfYN/acz+RFytVMno/3puDh+prJ8/GbSR730fYBAAAAAAAAAAAAAAAAAACAYfkJuHbYr8dtGYwAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-codeblock-include/)
 [![Docs](https://img.shields.io/badge/docs-wiki-green.svg?logo=read-the-docs&logoColor=white)](https://github.com/chdemko/pandoc-codeblock-include/wiki)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAwCAYAAABXAvmHAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAAOxAAADsQBlSsOGwAAABl0RVh0U29mdHdhcmUAd3d3Lmlua3NjYXBlLm9yZ5vuPBoAAANwSURBVGiB7Zndi1VlFIefNZPR9GkTmSkOhIZYeBFiIDEYNUREXVQEQUhK4hdEf0GQf0IUU2BdhHUjNQTpRRdl0NdFXYRZCA0SJTZ9CJEDmY49Xewzw57Xfc7+OGfOEJzn5vCuvfbav/Wutd+993tgwIAB/2ui3xdUVwKPAbcDPwDHIuJiv3XURr1HPaTOuphpdeNy6ytEvUbdoX5pZ75Xr15uvQuoa9WX1N9KhOfZsdyih9QJ9Yg6V0P4PF8sl/CV6gvq6QaiU7b0U/g29bB6oQfC5znUD+HXqu/2UHSeWbNltjJDDXKYBJ4EfgFeBo42iNGO64BnexhvMeoqsxt0Vh3L2V/tYRVOqZUfsHUrcCcwDJyKiJ9y9g9rxunERuDBqs51Ezjb+t2UrwDwcM04Zeyv6lj7XUj9GtgCzABHgA3AI3XjlDAH3BERZ3ocF9TnetjvnThYRU+TCowAZ4DRuufWZAYYi4hLnZxqL6MR8TfwVlNVNVgNPL4kkdUN6uU+tNEnZVo6VkC9tcgeEdPAR83Sr8V29e5ODmUttLvDscn6ehpReUldhLpebTvL6rD6Yx/a6C/1xnY6OlVgf6fjEXEZeKPSbHTHDcAztc5QR9Q/1OOJfSgZr1b/6UMVTrTT2m6GnwZuKbBvVRfW/4iYAaaqT01jNqvjRQfaJdDuxhkBdia21xqKqku1m9ls+2OetIXuN9sGSVvpRB/a6KK6JtVbVIHnS3JcD0wktterTE6XrAB2pcZ0JkfJ+r+MA8n4MHC+sbTq7FGH84a0AjvJ+ryMR819D0TEeeDtruWVMwbcmzcsJGD2GbevYqBhYE9i69eTeVV+kK/ANrJPxqrsNrcdGBEngU+701aJb/ODfAJ1xAPcBjyR2Ja6Cu9FxOm8IZ/AdIOA6c08RfYhshQcB/amxnwCXwHf1Qw6rm6eH7T2+d9sJK+YObJJmYiIByLiXEfv1kPs15IHWcpk4rPOZpu7ec6qB9W1tVNWR9UX1Z8LEhgvuNgVr7vq+w1E/6t+rD6lrqgtvCCRq0x2i9U1rQulHEj8Hqoh/E/1FXVT16IrJjZVIOJk4hPqZyXCv1H3qtf3RXhO3M3qsQJB2xO/dS2ReS6o76j39UpP438p1QlgK3BTy/R5RHyQ+AyRbTveBZwDjkbE702vOWDAgCv5DyyzjR7/CUzHAAAAAElFTkSuQmCC)](https://pypi.org/project/black/)
 
 license icon by [Daniel Bruce](https://www.iconfinder.com/icons/216659/license_icon), format icon by [Picol](https://www.iconfinder.com/icons/103509/document_text_icon), status icon by [Just Icon](https://www.iconfinder.com/icons/2672768/app_battery_essential_object_status_ui_ux_icon), code style icon by [Google Material Design icons](https://www.iconfinder.com/icons/352148/style_icon)
 
 
 *pandoc-codeblock-include* is a [pandoc] filter for including files in `CodeBlock` elements.
 
 [pandoc]: http://pandoc.org/
 
-Documentation
--------------
-
-See the [wiki pages](https://github.com/chdemko/pandoc-codeblock-include/wiki).
-
-Usage
------
-
-To apply the filter, use the following option with pandoc:
-
-    --filter pandoc-codeblock-include
-
-Installation
+Instructions
 ------------
 
 *pandoc-codeblock-include* requires [python], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows]. Either python 2.7 or 3.x will do.
 
 Install *pandoc-codeblock-include* as root using the bash command
 
     pip install pandoc-codeblock-include
```

### Comparing `pandoc-codeblock-include-0.1.1/pandoc_codeblock_include.py` & `pandoc_codeblock_include-1.0.0/pandoc_codeblock_include.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 #!/usr/bin/env python
 
 """
-Pandoc filter for including file in code block
+Pandoc filter for including file in code block.
 """
 
-from panflute import run_filter, debug, CodeBlock
+from panflute import CodeBlock, debug, run_filters  # type: ignore
 
 
 def parse_include(parsed, name, value):
     """
     Extract include information from attributes.
 
     Arguments
     ---------
-        parsed:
-            A dictionnary of attributes
-        name:
-            attribute name
-        value:
-            attribute value
+    parsed
+        A dictionnary of attributes
+    name
+        attribute name
+    value
+        attribute value
     """
     if name == "include":
         try:
-            file_content = open(value, "r").readlines()
+            with open(value, "r", encoding="utf-8") as stream:
+                file_content = stream.readlines()
             parsed["content"] = file_content
             parsed["include"] = value
         except IOError:
             debug("[WARNING] pandoc-codeblock-include: " + value + " not found")
         except UnicodeDecodeError:
             debug(
                 "[WARNING] pandoc-codeblock-include: file "
@@ -37,20 +38,20 @@
 
 def parse_start_from(parsed, name, value):
     """
     Extract startFrom information from attributes.
 
     Arguments
     ---------
-        parsed:
-            A dictionnary of attributes
-        name:
-            attribute name
-        value:
-            attribute value
+    parsed
+        A dictionnary of attributes
+    name
+        attribute name
+    value
+        attribute value
     """
     if name == "startFrom":
         try:
             parsed["start_from"] = int(value) - 1
         except ValueError:
             debug(
                 "[WARNING] pandoc-codeblock-include: "
@@ -61,20 +62,20 @@
 
 def parse_end_at(parsed, name, value):
     """
     Extract entAt information from attributes.
 
     Arguments
     ---------
-        parsed:
-            A dictionnary of attributes
-        name:
-            attribute name
-        value:
-            attribute value
+    parsed
+        A dictionnary of attributes
+    name
+        attribute name
+    value
+        attribute value
     """
     if name == "endAt":
         try:
             parsed["end_at"] = int(value)
         except ValueError:
             debug(
                 "[WARNING] pandoc-codeblock-include: "
@@ -85,16 +86,16 @@
 
 def parse_attributes(items):
     """
     Extract usefull information from attributes.
 
     Arguments
     ---------
-        items:
-            element attributes
+    items
+        element attributes
 
     Returns
     -------
         a mapping containing possible 'content', 'start_from' and 'end_at'
     """
     parsed = {}
     for name, value in items:
@@ -106,18 +107,18 @@
 
 def inject_content(elem, parsed):
     """
     Inject parsed attributes into element content.
 
     Arguments
     ---------
-        elem:
-            Pandoc element
-        parsed:
-            dictionnary of attributes
+    elem
+        Pandoc element
+    parsed
+        dictionnary of attributes
     """
     start_from = parsed.get("start_from", 0)
     end_at = parsed.get("end_at", len(parsed["content"]))
     text = parsed["content"][start_from:end_at]
 
     # inject file content in element text
     try:
@@ -134,50 +135,54 @@
 
 def clear_latex_attributes(elem):
     """
     Clear LaTeX attributes.
 
     Arguments
     ---------
-        elem:
-            current element
+    elem
+        current element
     """
     # Clear the attributes else latex will get a problem with the listings
-    for attribute in ["include", "endAt"]:
+    for attribute in ("include", "endAt"):
         if attribute in elem.attributes:
             del elem.attributes[attribute]
 
 
 def include(elem, doc):
     """
     Transform CodeBlock element.
 
     Arguments
     ---------
-        elem:
-            current element
-        doc:
-            pandoc document
+    elem
+        current element
+    doc
+        pandoc document
     """
     # Is it a CodeBlock?
     if isinstance(elem, CodeBlock):
         parsed = parse_attributes(elem.attributes.items())
         if "content" in parsed:
             inject_content(elem, parsed)
-        if doc.format in ["latex", "beamer"]:
+        if doc.format in ("latex", "beamer"):
             clear_latex_attributes(elem)
 
 
 def main(doc=None):
     """
-    main function.
+    Convert the pandoc document.
 
     Arguments
     ---------
-        doc:
-            pandoc document
+    doc
+        pandoc document
+
+    Returns
+    -------
+        The modified pandoc document.
     """
-    return run_filter(include, doc=doc)
+    return run_filters([include], doc=doc)
 
 
 if __name__ == "__main__":
     main()
```

