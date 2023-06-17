# Comparing `tmp/pandoc-numbering-3.4.0.1.tar.gz` & `tmp/pandoc_numbering-3.4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandoc-numbering-3.4.0.1.tar", last modified: Wed Oct 26 16:27:33 2022, max compression
+gzip compressed data, was "pandoc_numbering-3.4.0.2.tar", max compression
```

## Comparing `pandoc-numbering-3.4.0.1.tar` & `pandoc_numbering-3.4.0.2.tar`

### file list

```diff
@@ -1,15 +1,5 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 16:27:33.791261 pandoc-numbering-3.4.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1521 2022-10-26 16:27:17.000000 pandoc-numbering-3.4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-10-26 16:27:17.000000 pandoc-numbering-3.4.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    10421 2022-10-26 16:27:33.791261 pandoc-numbering-3.4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9206 2022-10-26 16:27:17.000000 pandoc-numbering-3.4.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 16:27:33.791261 pandoc-numbering-3.4.0.1/pandoc_numbering.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10421 2022-10-26 16:27:33.000000 pandoc-numbering-3.4.0.1/pandoc_numbering.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-10-26 16:27:33.000000 pandoc-numbering-3.4.0.1/pandoc_numbering.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 16:27:33.000000 pandoc-numbering-3.4.0.1/pandoc_numbering.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-10-26 16:27:33.000000 pandoc-numbering-3.4.0.1/pandoc_numbering.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-10-26 16:27:33.000000 pandoc-numbering-3.4.0.1/pandoc_numbering.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-26 16:27:33.000000 pandoc-numbering-3.4.0.1/pandoc_numbering.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    47324 2022-10-26 16:27:17.000000 pandoc-numbering-3.4.0.1/pandoc_numbering.py
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-10-26 16:27:33.791261 pandoc-numbering-3.4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3963 2022-10-26 16:27:17.000000 pandoc-numbering-3.4.0.1/setup.py
+-rw-r--r--   0        0        0     1521 2023-06-17 12:48:51.084426 pandoc_numbering-3.4.0.2/LICENSE
+-rw-r--r--   0        0        0     9037 2023-06-17 12:48:51.084426 pandoc_numbering-3.4.0.2/README.md
+-rw-r--r--   0        0        0    49076 2023-06-17 12:48:51.088427 pandoc_numbering-3.4.0.2/pandoc_numbering.py
+-rw-r--r--   0        0        0     2926 2023-06-17 12:48:51.088427 pandoc_numbering-3.4.0.2/pyproject.toml
+-rw-r--r--   0        0        0    10167 1970-01-01 00:00:00.000000 pandoc_numbering-3.4.0.2/PKG-INFO
```

### Comparing `pandoc-numbering-3.4.0.1/LICENSE` & `pandoc_numbering-3.4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pandoc-numbering-3.4.0.1/PKG-INFO` & `pandoc_numbering-3.4.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,110 +1,107 @@
 Metadata-Version: 2.1
 Name: pandoc-numbering
-Version: 3.4.0.1
+Version: 3.4.0.2
 Summary: A pandoc filter for automatic numbering
 Home-page: https://github.com/chdemko/pandoc-numbering
-Download-URL: https://github.com/chdemko/pandoc-numbering/archive/develop.zip
+License: BSD-3-Clause
+Keywords: pandoc,filters,numbering
 Author: Christophe Demko
 Author-email: chdemko@gmail.com
-Maintainer: Christophe Demko
-Maintainer-email: chdemko@gmail.com
-License: BSD-3-Clause
-Keywords: pandoc filters numbering
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
-Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Text Processing :: Filters
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Natural Language :: English
+Requires-Dist: panflute (>=2.3.0,<3.0.0)
 Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: test
-License-File: LICENSE
 
-# pandoc-numbering
+Installation
+============
+
 ![Python package](https://github.com/chdemko/pandoc-numbering/workflows/Python%20package/badge.svg?branch=develop)
-[![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-numbering/3.4.0.1.svg?logo=Codecov&logoColor=white)](https://coveralls.io/github/chdemko/pandoc-numbering?branch=3.4.0.1)
+[![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-numbering/develop.svg?logo=Codecov&logoColor=white)](https://coveralls.io/github/chdemko/pandoc-numbering?branch=develop)
 [![Scrutinizer](https://img.shields.io/scrutinizer/g/chdemko/pandoc-numbering.svg?logo=scrutinizer)](https://scrutinizer-ci.com/g/chdemko/pandoc-numbering/)
 [![PyPI version](https://img.shields.io/pypi/v/pandoc-numbering.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-numbering/)
 [![PyPI format](https://img.shields.io/pypi/format/pandoc-numbering.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiYw92eBNAAAAgJJREFUeNrt3T1WwkAUgNH31Br3ogWptdAlgyvQxYgHeh0LKKxI+PHAzNyvRo8xlxl5CZKllBIaax0Rr5n53tqB3Ti3k7qPiEUpZQAAggEACAYAIBgAgGAAoG8Ey9oRAHBas9oR5NgcIDOz5TN4pjnIJiJeapwTWAFGfMR2CDRlJViUUuYAtAfgOSK+Jv5N8FbddlBGav4M7+9795jHUsqqTGtdFQIAxgE0jQCAaQCaRQDAdABNIgDgMADNIQDgcAB/EHxWjwCA4wDsvvahegQAHA+gCQQAnAagegQAnA6gagQAnAdArQhcDdx//D+ZeXvg95tHxDK21wbG2mTm/SWP38Wgcz+jMj8i4ikiVhMePrv0z3vnlO1/grS+DVoBehfuVwCAABAAAkAAqLO6nwP896Tz2ucIVgBbgAAQAAJAAAgAASAABIAAEAACQAAIADXZyfcD9P55A7W/c8oKYAsQAAJAAAgAASBzgJ5eB1sBBIAAEAACQAAIAJkDTM/9AO4HEAACQAAIAAEgANTPHMD9AFYAASAABIAAEAACQP3MAWq/H6D3OYYVwBYgAASAABAAAkDmAF5HWwEEgAAQAAJAAAgAASAABIAAEAACQAAIAAEgAASAABAAAkAACAABIAAEgAAQAAJAAAgAXVWj/x+g988FtAIIAAEgAASAABAAaqhfB1BFkJjdTNQAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-numbering/)
-[![License](https://img.shields.io/pypi/l/pandoc-numbering.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAABmCAYAAAADI5lUAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiQKA106BAAABUNJREFUeNrtnV2IFlUYx3/P625qbrGlpWmWdaMVKau2EmpCrSDqxRpUUkr0SYVEFyFRUXQhfUAihTdCESVpKpKQpLZBsghltn605VVKpmZgGYvmbhpPFzMbWu3LO7szO1//H+zN7sw5c57nd8685+zMeY0quLsB04FW4A7gWmAMMAyRRbqBE8BRYCfwMfCNmXlfJ1iV5LcAbwBNimuu+Q54xcw21iSAuzcA7wOLFLtCsQl4yMxO9ymAu48HtgK3Kl6F5ACw0Mx++o8AYc/fBUxWnArN98DtZtYFULngDx8o+aXgZuDdi0YAd58fDv2iPMwzs+0WTvX2qfeXjv1Ak7n7DOBLxaOU3FYhWOQR5aS1AsxWHErLnArB8q4oJ+PM3buBoRFO6gJ2K3aZpBm4PMLxPXh09ijO2cTd90RNZkVhKzcSQAIICSAkgJAAQgIICSAkgJAAQgIICSAKT91gVOLui4EVKbZzvZm9kGD7rgHmEbw9NRoYCTQCvwInCd7UaQPaep/GLZUABP+ivDHFdo5KKPHTgNeAu6jyllXIk8A5d/8QeN7MjusWkGPcfRnBs5QtNSS/l3rgQaDT3e+UAPlN/iPA2wMYQa8APnH3ZgmQv+SPBlbGUNRw4D13r5MA+WIF0R67qsZNwMMSID+9vwF4IOZin5AA+WE+8W+O0eTuN0iAfNCSs3IlQMxMSqjciRIgH0wsmgCDNQU5CKxJMXHtMXwAHAJcndD1jSu0AGbWHkcSUmZEgmVfqltA9kkySQ0SIPsMyWnZEiAm/kiw7DMSIPt0AecSKvukBMg4ZvYXcCSh4g9LgHzwVc7KzcY00N0XAM+kmLitZrYqhnLagPsTuL7PCy0AwUJHS4oCHMpwok4AnboF5ONzwJFwFIiTd6pt5y4BssebMZbVA6xOszESIDrbiW+TrDVm9rMEyNdtwIHHgPMDLOoX4KW02yMB+ifBAWCgs4qnzex3CZBfXgS+7ee568xsQxYaIQH6Pwr0ELzk8WfEU48Dy7LSDgkwMAn2Eu2dRwceNbPfJEBxeD3s1bWwzcw+zdLFD9ZK4DHiX0CJwsEkbwXuvrrGkWBl5vTVXsGxxHBaDXE76+71CV+H9gpOiRM1HHPKzM5l7cIlQDxcX8Mxo9x9uAQoJktqOKYeuE8CFO/+P5NgabgWXnX3sRKgOMmfDWyJMJsaA+xw9wkSIN+Jr7j7U+HUdmTE028Bdrv73NKsA4Q9ZUmK7Ww3s7UxtaUZeAuYMYBirgpHgg3AcjP7sdACEOyE8XjKsq8dSI8H5gLPEu+jbfcCi9x9PbDKzDqKKkBeh/rpwN0Eu4Jcl1A19cBSYKm77wXWAZvN7AcJkG7ypwBfD3K1TeHPy+7eaGbnk65QHwL7ZlKKdY8AxmsWkC5XlqF+CdA3jWWoXwL0TUPK9V8mAdLlkpTrr5cA6VInAcpNfRnqHyzLu4jvBc3+0J8NGE6lfM1nB6UWPRJWHPRImNBnACEBhAQQEkBIACEBhAQQEkBIACEBhAQQ/8bcvRsYGuGcLuLbJ0/ESzPRvtW0x9z9MDBBsSslhyoE27eIcnKsAuxUHErLFxWC15tFOdli7m7AXmCK4lEq9gFTK+Hmx88pHqVjuZkFj4SZ2TZgs2JSGjaa2WcA1vsbd28AdgGTFZ9Csx+YaWZn4IKVQDM7DSwIDxDFve8v7E3+RQKEEhwFZgGbFKvC8REwK8wx/ytA70hgZvcQbInSobjlns6w1y++sOf/k+9qZ4ZTxKlAKzCH4OvfxgLDFNdM0k2wc/lRggW+LUBHtW8l+xuWwqBw5I0ApAAAAABJRU5ErkJggg==)](https://raw.githubusercontent.com/chdemko/pandoc-numbering/3.4.0.1/LICENSE)
-[![Repo Size](https://img.shields.io/github/repo-size/chdemko/pandoc-numbering.svg)](http://pandoc-numbering.readthedocs.io/en/3.4.0.1/)
+[![License](https://img.shields.io/pypi/l/pandoc-numbering.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAABmCAYAAAADI5lUAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiQKA106BAAABUNJREFUeNrtnV2IFlUYx3/P625qbrGlpWmWdaMVKau2EmpCrSDqxRpUUkr0SYVEFyFRUXQhfUAihTdCESVpKpKQpLZBsghltn605VVKpmZgGYvmbhpPFzMbWu3LO7szO1//H+zN7sw5c57nd8685+zMeY0quLsB04FW4A7gWmAMMAyRRbqBE8BRYCfwMfCNmXlfJ1iV5LcAbwBNimuu+Q54xcw21iSAuzcA7wOLFLtCsQl4yMxO9ymAu48HtgK3Kl6F5ACw0Mx++o8AYc/fBUxWnArN98DtZtYFULngDx8o+aXgZuDdi0YAd58fDv2iPMwzs+0WTvX2qfeXjv1Ak7n7DOBLxaOU3FYhWOQR5aS1AsxWHErLnArB8q4oJ+PM3buBoRFO6gJ2K3aZpBm4PMLxPXh09ijO2cTd90RNZkVhKzcSQAIICSAkgJAAQgIICSAkgJAAQgIICSAKT91gVOLui4EVKbZzvZm9kGD7rgHmEbw9NRoYCTQCvwInCd7UaQPaep/GLZUABP+ivDHFdo5KKPHTgNeAu6jyllXIk8A5d/8QeN7MjusWkGPcfRnBs5QtNSS/l3rgQaDT3e+UAPlN/iPA2wMYQa8APnH3ZgmQv+SPBlbGUNRw4D13r5MA+WIF0R67qsZNwMMSID+9vwF4IOZin5AA+WE+8W+O0eTuN0iAfNCSs3IlQMxMSqjciRIgH0wsmgCDNQU5CKxJMXHtMXwAHAJcndD1jSu0AGbWHkcSUmZEgmVfqltA9kkySQ0SIPsMyWnZEiAm/kiw7DMSIPt0AecSKvukBMg4ZvYXcCSh4g9LgHzwVc7KzcY00N0XAM+kmLitZrYqhnLagPsTuL7PCy0AwUJHS4oCHMpwok4AnboF5ONzwJFwFIiTd6pt5y4BssebMZbVA6xOszESIDrbiW+TrDVm9rMEyNdtwIHHgPMDLOoX4KW02yMB+ifBAWCgs4qnzex3CZBfXgS+7ee568xsQxYaIQH6Pwr0ELzk8WfEU48Dy7LSDgkwMAn2Eu2dRwceNbPfJEBxeD3s1bWwzcw+zdLFD9ZK4DHiX0CJwsEkbwXuvrrGkWBl5vTVXsGxxHBaDXE76+71CV+H9gpOiRM1HHPKzM5l7cIlQDxcX8Mxo9x9uAQoJktqOKYeuE8CFO/+P5NgabgWXnX3sRKgOMmfDWyJMJsaA+xw9wkSIN+Jr7j7U+HUdmTE028Bdrv73NKsA4Q9ZUmK7Ww3s7UxtaUZeAuYMYBirgpHgg3AcjP7sdACEOyE8XjKsq8dSI8H5gLPEu+jbfcCi9x9PbDKzDqKKkBeh/rpwN0Eu4Jcl1A19cBSYKm77wXWAZvN7AcJkG7ypwBfD3K1TeHPy+7eaGbnk65QHwL7ZlKKdY8AxmsWkC5XlqF+CdA3jWWoXwL0TUPK9V8mAdLlkpTrr5cA6VInAcpNfRnqHyzLu4jvBc3+0J8NGE6lfM1nB6UWPRJWHPRImNBnACEBhAQQEkBIACEBhAQQEkBIACEBhAQQ/8bcvRsYGuGcLuLbJ0/ESzPRvtW0x9z9MDBBsSslhyoE27eIcnKsAuxUHErLFxWC15tFOdli7m7AXmCK4lEq9gFTK+Hmx88pHqVjuZkFj4SZ2TZgs2JSGjaa2WcA1vsbd28AdgGTFZ9Csx+YaWZn4IKVQDM7DSwIDxDFve8v7E3+RQKEEhwFZgGbFKvC8REwK8wx/ytA70hgZvcQbInSobjlns6w1y++sOf/k+9qZ4ZTxKlAKzCH4OvfxgLDFNdM0k2wc/lRggW+LUBHtW8l+xuWwqBw5I0ApAAAAABJRU5ErkJggg==)](https://raw.githubusercontent.com/chdemko/pandoc-numbering/develop/LICENSE)
+[![Repo Size](https://img.shields.io/github/repo-size/chdemko/pandoc-numbering.svg)](http://pandoc-numbering.readthedocs.io/en/latest/)
 [![Python version](https://img.shields.io/pypi/pyversions/pandoc-numbering.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-numbering/)
 [![Downloads](https://pepy.tech/badge/pandoc-numbering)](https://pepy.tech/project/pandoc-numbering)
 [![Source Rank](https://img.shields.io/librariesio/sourcerank/pypi/pandoc-numbering.svg?logo=koding&logoColor=white)](https://libraries.io/pypi/pandoc-numbering)
 [![Development Status](https://img.shields.io/pypi/status/pandoc-numbering.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiUnX5lXMAAAAlBJREFUeNrt3b1qlEEUBuB3TNDCP7wDOwv/cgv+pDC3YcDe+xBFFFLoDWhhpxiD12Ch1mJsg7irjRLGYjcKEbLC92n223meMgQSzrx7Zs6wMAkAAAAAAAAAAAAAAAAAAAAw78r+H9RaLyZZT3Itydkkx5XpUH1L8iHJVpJHpZS3/yQAtdZjSe4muZXkiLrPpd0kG0lul1K+9xaA6eK/SHJFjQfhdZIbfYRg75N+z+IPytUkd3rpANM9/422P8jt4HIp5V3XDrBu8QdpKcnNPraA62o5WKt9bAHjJCfUcpDGpZRTXQNQ1fGAApVSDvPvz1qfrv+fvb9xAiAACACDVf80qrU+q7Wecwhs4BB4gM+ZXBRt6wBtOpO/uC7WARa3AyTJqJRyWgdo18xLIgEwBSAACABt3hOYAhZ7Cph9TyAAzQYgSZ4KQNsBGAlA2wFwCDQFIAAIAAKAACAACAACgAAgAAgAAoAAIAAIAIvniwC07aVvBM2wwN8I2kmyogO0Z5TkSZKVUsqnZfVou4PpAKYABAABYDHnfAFofM6feUh0D7Cw9wA7e6OeDtDwnD/rl90DNN6hdABTAAJAs5aTjJOcVIreT+H/68DXuQNsW+bB+thHAF6p42Btdp4iaq0XMnk2bkk9B2U3yaVSyvtOHWD6Fu2Geg7Ow66Ln/x+OvZokueZPBjN/NtKslZK+dHLGDh9g3YtyYNpa2F+2/79vhb/VwfYN/acz+RFytVMno/3puDh+prJ8/GbSR730fYBAAAAAAAAAAAAAAAAAACAYfkJuHbYr8dtGYwAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-numbering/)
-[![Docs](https://img.shields.io/readthedocs/pandoc-numbering.svg?logo=read-the-docs&logoColor=white)](http://pandoc-numbering.readthedocs.io/en/3.4.0.1/)
+[![Docs](https://img.shields.io/readthedocs/pandoc-numbering.svg?logo=read-the-docs&logoColor=white)](http://pandoc-numbering.readthedocs.io/en/latest/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAwCAYAAABXAvmHAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAAOxAAADsQBlSsOGwAAABl0RVh0U29mdHdhcmUAd3d3Lmlua3NjYXBlLm9yZ5vuPBoAAANwSURBVGiB7Zndi1VlFIefNZPR9GkTmSkOhIZYeBFiIDEYNUREXVQEQUhK4hdEf0GQf0IUU2BdhHUjNQTpRRdl0NdFXYRZCA0SJTZ9CJEDmY49Xewzw57Xfc7+OGfOEJzn5vCuvfbav/Wutd+993tgwIAB/2ui3xdUVwKPAbcDPwDHIuJiv3XURr1HPaTOuphpdeNy6ytEvUbdoX5pZ75Xr15uvQuoa9WX1N9KhOfZsdyih9QJ9Yg6V0P4PF8sl/CV6gvq6QaiU7b0U/g29bB6oQfC5znUD+HXqu/2UHSeWbNltjJDDXKYBJ4EfgFeBo42iNGO64BnexhvMeoqsxt0Vh3L2V/tYRVOqZUfsHUrcCcwDJyKiJ9y9g9rxunERuDBqs51Ezjb+t2UrwDwcM04Zeyv6lj7XUj9GtgCzABHgA3AI3XjlDAH3BERZ3ocF9TnetjvnThYRU+TCowAZ4DRuufWZAYYi4hLnZxqL6MR8TfwVlNVNVgNPL4kkdUN6uU+tNEnZVo6VkC9tcgeEdPAR83Sr8V29e5ODmUttLvDscn6ehpReUldhLpebTvL6rD6Yx/a6C/1xnY6OlVgf6fjEXEZeKPSbHTHDcAztc5QR9Q/1OOJfSgZr1b/6UMVTrTT2m6GnwZuKbBvVRfW/4iYAaaqT01jNqvjRQfaJdDuxhkBdia21xqKqku1m9ls+2OetIXuN9sGSVvpRB/a6KK6JtVbVIHnS3JcD0wktterTE6XrAB2pcZ0JkfJ+r+MA8n4MHC+sbTq7FGH84a0AjvJ+ryMR819D0TEeeDtruWVMwbcmzcsJGD2GbevYqBhYE9i69eTeVV+kK/ANrJPxqrsNrcdGBEngU+701aJb/ODfAJ1xAPcBjyR2Ja6Cu9FxOm8IZ/AdIOA6c08RfYhshQcB/amxnwCXwHf1Qw6rm6eH7T2+d9sJK+YObJJmYiIByLiXEfv1kPs15IHWcpk4rPOZpu7ec6qB9W1tVNWR9UX1Z8LEhgvuNgVr7vq+w1E/6t+rD6lrqgtvCCRq0x2i9U1rQulHEj8Hqoh/E/1FXVT16IrJjZVIOJk4hPqZyXCv1H3qtf3RXhO3M3qsQJB2xO/dS2ReS6o76j39UpP438p1QlgK3BTy/R5RHyQ+AyRbTveBZwDjkbE702vOWDAgCv5DyyzjR7/CUzHAAAAAElFTkSuQmCC)](https://pypi.org/project/black/)
 
 license icon by [Daniel Bruce](https://www.iconfinder.com/icons/216659/license_icon),
 format icon by [Picol](https://www.iconfinder.com/icons/103509/document_text_icon),
 status icon by [Just Icon](https://www.iconfinder.com/icons/2672768/app_battery_essential_object_status_ui_ux_icon),
 code style icon by [Google Material Design icons](https://www.iconfinder.com/icons/352148/style_icon)
 
 *pandoc-numbering* is a [pandoc] filter for numbering all kinds of things.
 
 [pandoc]: http://pandoc.org/
 
-Documentation
--------------
-
-See the [Read the docs pages](http://pandoc-numbering.readthedocs.io/en/3.4.0.1/).
-
-Usage
------
-
-To apply the filter, use the following option with pandoc:
-
-    --filter pandoc-numbering
-
-Installation
+Instructions
 ------------
 
 *pandoc-numbering* requires [python], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows]. Either python 2.7 or 3.x will do.
 
-Install *pandoc-numbering* as root using the bash command
+Install *pandoc-numbering* using the bash command
 
-    pip install pandoc-numbering
+~~~shell
+$ pip install pandoc-numbering
+~~~
 
 To upgrade to the most recent release, use
 
-    pip install --upgrade pandoc-numbering
+~~~shell
+$ pip install --upgrade pandoc-numbering
+~~~
 
 To upgrade to the current code, use
 
-    pip install --upgrade --force --no-cache git+https://github.com/chdemko/pandoc-numbering
+~~~shell
+$ pip install --upgrade --force --no-cache git+https://github.com/chdemko/pandoc-numbering
+~~~
 
 `pip` is a script that downloads and installs modules from the Python Package Index, [PyPI].  It should come installed with your python distribution. If you are running linux, `pip` may be bundled separately. On a Debian-based system (including Ubuntu), you can install it as root using
 
-    apt-get update
-    apt-get install python-pip
+~~~shell
+$ sudo apt-get install python3-pip
+~~~
 
 Make sure you have the
 
 * *tocloft*
 
 LaTeX package. On linux you have to install some extra libraries **before**
 *pandoc-numbering*. On a Debian-based system (including Ubuntu), you can install it as
 root using
 
-	apt-get install texlive-latex-extra
+~~~shell
+$ sudo apt-get install texlive-latex-extra
+~~~
 
 [python]: https://www.python.org/
 [on Windows]: https://www.python.org/downloads/windows/
 [PyPI]: https://pypi.python.org/pypi
 
 
 Getting Help
 ------------
 
 If you have any difficulties with *pandoc-numbering*, please feel welcome to [file an issue] on github so that we can help.
 
 [file an issue]: https://github.com/chdemko/pandoc-numbering/issues
+
```

### Comparing `pandoc-numbering-3.4.0.1/README.md` & `pandoc_numbering-3.4.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,74 +1,73 @@
-# pandoc-numbering
+Installation
+============
+
 ![Python package](https://github.com/chdemko/pandoc-numbering/workflows/Python%20package/badge.svg?branch=develop)
-[![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-numbering/3.4.0.1.svg?logo=Codecov&logoColor=white)](https://coveralls.io/github/chdemko/pandoc-numbering?branch=3.4.0.1)
+[![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-numbering/develop.svg?logo=Codecov&logoColor=white)](https://coveralls.io/github/chdemko/pandoc-numbering?branch=develop)
 [![Scrutinizer](https://img.shields.io/scrutinizer/g/chdemko/pandoc-numbering.svg?logo=scrutinizer)](https://scrutinizer-ci.com/g/chdemko/pandoc-numbering/)
 [![PyPI version](https://img.shields.io/pypi/v/pandoc-numbering.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-numbering/)
 [![PyPI format](https://img.shields.io/pypi/format/pandoc-numbering.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiYw92eBNAAAAgJJREFUeNrt3T1WwkAUgNH31Br3ogWptdAlgyvQxYgHeh0LKKxI+PHAzNyvRo8xlxl5CZKllBIaax0Rr5n53tqB3Ti3k7qPiEUpZQAAggEACAYAIBgAgGAAoG8Ey9oRAHBas9oR5NgcIDOz5TN4pjnIJiJeapwTWAFGfMR2CDRlJViUUuYAtAfgOSK+Jv5N8FbddlBGav4M7+9795jHUsqqTGtdFQIAxgE0jQCAaQCaRQDAdABNIgDgMADNIQDgcAB/EHxWjwCA4wDsvvahegQAHA+gCQQAnAagegQAnA6gagQAnAdArQhcDdx//D+ZeXvg95tHxDK21wbG2mTm/SWP38Wgcz+jMj8i4ikiVhMePrv0z3vnlO1/grS+DVoBehfuVwCAABAAAkAAqLO6nwP896Tz2ucIVgBbgAAQAAJAAAgAASAABIAAEAACQAAIADXZyfcD9P55A7W/c8oKYAsQAAJAAAgAASBzgJ5eB1sBBIAAEAACQAAIAJkDTM/9AO4HEAACQAAIAAEgANTPHMD9AFYAASAABIAAEAACQP3MAWq/H6D3OYYVwBYgAASAABAAAkDmAF5HWwEEgAAQAAJAAAgAASAABIAAEAACQAAIAAEgAASAABAAAkAACAABIAAEgAAQAAJAAAgAXVWj/x+g988FtAIIAAEgAASAABAAaqhfB1BFkJjdTNQAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-numbering/)
-[![License](https://img.shields.io/pypi/l/pandoc-numbering.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAABmCAYAAAADI5lUAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiQKA106BAAABUNJREFUeNrtnV2IFlUYx3/P625qbrGlpWmWdaMVKau2EmpCrSDqxRpUUkr0SYVEFyFRUXQhfUAihTdCESVpKpKQpLZBsghltn605VVKpmZgGYvmbhpPFzMbWu3LO7szO1//H+zN7sw5c57nd8685+zMeY0quLsB04FW4A7gWmAMMAyRRbqBE8BRYCfwMfCNmXlfJ1iV5LcAbwBNimuu+Q54xcw21iSAuzcA7wOLFLtCsQl4yMxO9ymAu48HtgK3Kl6F5ACw0Mx++o8AYc/fBUxWnArN98DtZtYFULngDx8o+aXgZuDdi0YAd58fDv2iPMwzs+0WTvX2qfeXjv1Ak7n7DOBLxaOU3FYhWOQR5aS1AsxWHErLnArB8q4oJ+PM3buBoRFO6gJ2K3aZpBm4PMLxPXh09ijO2cTd90RNZkVhKzcSQAIICSAkgJAAQgIICSAkgJAAQgIICSAKT91gVOLui4EVKbZzvZm9kGD7rgHmEbw9NRoYCTQCvwInCd7UaQPaep/GLZUABP+ivDHFdo5KKPHTgNeAu6jyllXIk8A5d/8QeN7MjusWkGPcfRnBs5QtNSS/l3rgQaDT3e+UAPlN/iPA2wMYQa8APnH3ZgmQv+SPBlbGUNRw4D13r5MA+WIF0R67qsZNwMMSID+9vwF4IOZin5AA+WE+8W+O0eTuN0iAfNCSs3IlQMxMSqjciRIgH0wsmgCDNQU5CKxJMXHtMXwAHAJcndD1jSu0AGbWHkcSUmZEgmVfqltA9kkySQ0SIPsMyWnZEiAm/kiw7DMSIPt0AecSKvukBMg4ZvYXcCSh4g9LgHzwVc7KzcY00N0XAM+kmLitZrYqhnLagPsTuL7PCy0AwUJHS4oCHMpwok4AnboF5ONzwJFwFIiTd6pt5y4BssebMZbVA6xOszESIDrbiW+TrDVm9rMEyNdtwIHHgPMDLOoX4KW02yMB+ifBAWCgs4qnzex3CZBfXgS+7ee568xsQxYaIQH6Pwr0ELzk8WfEU48Dy7LSDgkwMAn2Eu2dRwceNbPfJEBxeD3s1bWwzcw+zdLFD9ZK4DHiX0CJwsEkbwXuvrrGkWBl5vTVXsGxxHBaDXE76+71CV+H9gpOiRM1HHPKzM5l7cIlQDxcX8Mxo9x9uAQoJktqOKYeuE8CFO/+P5NgabgWXnX3sRKgOMmfDWyJMJsaA+xw9wkSIN+Jr7j7U+HUdmTE028Bdrv73NKsA4Q9ZUmK7Ww3s7UxtaUZeAuYMYBirgpHgg3AcjP7sdACEOyE8XjKsq8dSI8H5gLPEu+jbfcCi9x9PbDKzDqKKkBeh/rpwN0Eu4Jcl1A19cBSYKm77wXWAZvN7AcJkG7ypwBfD3K1TeHPy+7eaGbnk65QHwL7ZlKKdY8AxmsWkC5XlqF+CdA3jWWoXwL0TUPK9V8mAdLlkpTrr5cA6VInAcpNfRnqHyzLu4jvBc3+0J8NGE6lfM1nB6UWPRJWHPRImNBnACEBhAQQEkBIACEBhAQQEkBIACEBhAQQ/8bcvRsYGuGcLuLbJ0/ESzPRvtW0x9z9MDBBsSslhyoE27eIcnKsAuxUHErLFxWC15tFOdli7m7AXmCK4lEq9gFTK+Hmx88pHqVjuZkFj4SZ2TZgs2JSGjaa2WcA1vsbd28AdgGTFZ9Csx+YaWZn4IKVQDM7DSwIDxDFve8v7E3+RQKEEhwFZgGbFKvC8REwK8wx/ytA70hgZvcQbInSobjlns6w1y++sOf/k+9qZ4ZTxKlAKzCH4OvfxgLDFNdM0k2wc/lRggW+LUBHtW8l+xuWwqBw5I0ApAAAAABJRU5ErkJggg==)](https://raw.githubusercontent.com/chdemko/pandoc-numbering/3.4.0.1/LICENSE)
-[![Repo Size](https://img.shields.io/github/repo-size/chdemko/pandoc-numbering.svg)](http://pandoc-numbering.readthedocs.io/en/3.4.0.1/)
+[![License](https://img.shields.io/pypi/l/pandoc-numbering.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAABmCAYAAAADI5lUAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiQKA106BAAABUNJREFUeNrtnV2IFlUYx3/P625qbrGlpWmWdaMVKau2EmpCrSDqxRpUUkr0SYVEFyFRUXQhfUAihTdCESVpKpKQpLZBsghltn605VVKpmZgGYvmbhpPFzMbWu3LO7szO1//H+zN7sw5c57nd8685+zMeY0quLsB04FW4A7gWmAMMAyRRbqBE8BRYCfwMfCNmXlfJ1iV5LcAbwBNimuu+Q54xcw21iSAuzcA7wOLFLtCsQl4yMxO9ymAu48HtgK3Kl6F5ACw0Mx++o8AYc/fBUxWnArN98DtZtYFULngDx8o+aXgZuDdi0YAd58fDv2iPMwzs+0WTvX2qfeXjv1Ak7n7DOBLxaOU3FYhWOQR5aS1AsxWHErLnArB8q4oJ+PM3buBoRFO6gJ2K3aZpBm4PMLxPXh09ijO2cTd90RNZkVhKzcSQAIICSAkgJAAQgIICSAkgJAAQgIICSAKT91gVOLui4EVKbZzvZm9kGD7rgHmEbw9NRoYCTQCvwInCd7UaQPaep/GLZUABP+ivDHFdo5KKPHTgNeAu6jyllXIk8A5d/8QeN7MjusWkGPcfRnBs5QtNSS/l3rgQaDT3e+UAPlN/iPA2wMYQa8APnH3ZgmQv+SPBlbGUNRw4D13r5MA+WIF0R67qsZNwMMSID+9vwF4IOZin5AA+WE+8W+O0eTuN0iAfNCSs3IlQMxMSqjciRIgH0wsmgCDNQU5CKxJMXHtMXwAHAJcndD1jSu0AGbWHkcSUmZEgmVfqltA9kkySQ0SIPsMyWnZEiAm/kiw7DMSIPt0AecSKvukBMg4ZvYXcCSh4g9LgHzwVc7KzcY00N0XAM+kmLitZrYqhnLagPsTuL7PCy0AwUJHS4oCHMpwok4AnboF5ONzwJFwFIiTd6pt5y4BssebMZbVA6xOszESIDrbiW+TrDVm9rMEyNdtwIHHgPMDLOoX4KW02yMB+ifBAWCgs4qnzex3CZBfXgS+7ee568xsQxYaIQH6Pwr0ELzk8WfEU48Dy7LSDgkwMAn2Eu2dRwceNbPfJEBxeD3s1bWwzcw+zdLFD9ZK4DHiX0CJwsEkbwXuvrrGkWBl5vTVXsGxxHBaDXE76+71CV+H9gpOiRM1HHPKzM5l7cIlQDxcX8Mxo9x9uAQoJktqOKYeuE8CFO/+P5NgabgWXnX3sRKgOMmfDWyJMJsaA+xw9wkSIN+Jr7j7U+HUdmTE028Bdrv73NKsA4Q9ZUmK7Ww3s7UxtaUZeAuYMYBirgpHgg3AcjP7sdACEOyE8XjKsq8dSI8H5gLPEu+jbfcCi9x9PbDKzDqKKkBeh/rpwN0Eu4Jcl1A19cBSYKm77wXWAZvN7AcJkG7ypwBfD3K1TeHPy+7eaGbnk65QHwL7ZlKKdY8AxmsWkC5XlqF+CdA3jWWoXwL0TUPK9V8mAdLlkpTrr5cA6VInAcpNfRnqHyzLu4jvBc3+0J8NGE6lfM1nB6UWPRJWHPRImNBnACEBhAQQEkBIACEBhAQQEkBIACEBhAQQ/8bcvRsYGuGcLuLbJ0/ESzPRvtW0x9z9MDBBsSslhyoE27eIcnKsAuxUHErLFxWC15tFOdli7m7AXmCK4lEq9gFTK+Hmx88pHqVjuZkFj4SZ2TZgs2JSGjaa2WcA1vsbd28AdgGTFZ9Csx+YaWZn4IKVQDM7DSwIDxDFve8v7E3+RQKEEhwFZgGbFKvC8REwK8wx/ytA70hgZvcQbInSobjlns6w1y++sOf/k+9qZ4ZTxKlAKzCH4OvfxgLDFNdM0k2wc/lRggW+LUBHtW8l+xuWwqBw5I0ApAAAAABJRU5ErkJggg==)](https://raw.githubusercontent.com/chdemko/pandoc-numbering/develop/LICENSE)
+[![Repo Size](https://img.shields.io/github/repo-size/chdemko/pandoc-numbering.svg)](http://pandoc-numbering.readthedocs.io/en/latest/)
 [![Python version](https://img.shields.io/pypi/pyversions/pandoc-numbering.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-numbering/)
 [![Downloads](https://pepy.tech/badge/pandoc-numbering)](https://pepy.tech/project/pandoc-numbering)
 [![Source Rank](https://img.shields.io/librariesio/sourcerank/pypi/pandoc-numbering.svg?logo=koding&logoColor=white)](https://libraries.io/pypi/pandoc-numbering)
 [![Development Status](https://img.shields.io/pypi/status/pandoc-numbering.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiUnX5lXMAAAAlBJREFUeNrt3b1qlEEUBuB3TNDCP7wDOwv/cgv+pDC3YcDe+xBFFFLoDWhhpxiD12Ch1mJsg7irjRLGYjcKEbLC92n223meMgQSzrx7Zs6wMAkAAAAAAAAAAAAAAAAAAAAw78r+H9RaLyZZT3Itydkkx5XpUH1L8iHJVpJHpZS3/yQAtdZjSe4muZXkiLrPpd0kG0lul1K+9xaA6eK/SHJFjQfhdZIbfYRg75N+z+IPytUkd3rpANM9/422P8jt4HIp5V3XDrBu8QdpKcnNPraA62o5WKt9bAHjJCfUcpDGpZRTXQNQ1fGAApVSDvPvz1qfrv+fvb9xAiAACACDVf80qrU+q7Wecwhs4BB4gM+ZXBRt6wBtOpO/uC7WARa3AyTJqJRyWgdo18xLIgEwBSAACABt3hOYAhZ7Cph9TyAAzQYgSZ4KQNsBGAlA2wFwCDQFIAAIAAKAACAACAACgAAgAAgAAoAAIAAIAIvniwC07aVvBM2wwN8I2kmyogO0Z5TkSZKVUsqnZfVou4PpAKYABAABYDHnfAFofM6feUh0D7Cw9wA7e6OeDtDwnD/rl90DNN6hdABTAAJAs5aTjJOcVIreT+H/68DXuQNsW+bB+thHAF6p42Btdp4iaq0XMnk2bkk9B2U3yaVSyvtOHWD6Fu2Geg7Ow66Ln/x+OvZokueZPBjN/NtKslZK+dHLGDh9g3YtyYNpa2F+2/79vhb/VwfYN/acz+RFytVMno/3puDh+prJ8/GbSR730fYBAAAAAAAAAAAAAAAAAACAYfkJuHbYr8dtGYwAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-numbering/)
-[![Docs](https://img.shields.io/readthedocs/pandoc-numbering.svg?logo=read-the-docs&logoColor=white)](http://pandoc-numbering.readthedocs.io/en/3.4.0.1/)
+[![Docs](https://img.shields.io/readthedocs/pandoc-numbering.svg?logo=read-the-docs&logoColor=white)](http://pandoc-numbering.readthedocs.io/en/latest/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAwCAYAAABXAvmHAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAAOxAAADsQBlSsOGwAAABl0RVh0U29mdHdhcmUAd3d3Lmlua3NjYXBlLm9yZ5vuPBoAAANwSURBVGiB7Zndi1VlFIefNZPR9GkTmSkOhIZYeBFiIDEYNUREXVQEQUhK4hdEf0GQf0IUU2BdhHUjNQTpRRdl0NdFXYRZCA0SJTZ9CJEDmY49Xewzw57Xfc7+OGfOEJzn5vCuvfbav/Wutd+993tgwIAB/2ui3xdUVwKPAbcDPwDHIuJiv3XURr1HPaTOuphpdeNy6ytEvUbdoX5pZ75Xr15uvQuoa9WX1N9KhOfZsdyih9QJ9Yg6V0P4PF8sl/CV6gvq6QaiU7b0U/g29bB6oQfC5znUD+HXqu/2UHSeWbNltjJDDXKYBJ4EfgFeBo42iNGO64BnexhvMeoqsxt0Vh3L2V/tYRVOqZUfsHUrcCcwDJyKiJ9y9g9rxunERuDBqs51Ezjb+t2UrwDwcM04Zeyv6lj7XUj9GtgCzABHgA3AI3XjlDAH3BERZ3ocF9TnetjvnThYRU+TCowAZ4DRuufWZAYYi4hLnZxqL6MR8TfwVlNVNVgNPL4kkdUN6uU+tNEnZVo6VkC9tcgeEdPAR83Sr8V29e5ODmUttLvDscn6ehpReUldhLpebTvL6rD6Yx/a6C/1xnY6OlVgf6fjEXEZeKPSbHTHDcAztc5QR9Q/1OOJfSgZr1b/6UMVTrTT2m6GnwZuKbBvVRfW/4iYAaaqT01jNqvjRQfaJdDuxhkBdia21xqKqku1m9ls+2OetIXuN9sGSVvpRB/a6KK6JtVbVIHnS3JcD0wktterTE6XrAB2pcZ0JkfJ+r+MA8n4MHC+sbTq7FGH84a0AjvJ+ryMR819D0TEeeDtruWVMwbcmzcsJGD2GbevYqBhYE9i69eTeVV+kK/ANrJPxqrsNrcdGBEngU+701aJb/ODfAJ1xAPcBjyR2Ja6Cu9FxOm8IZ/AdIOA6c08RfYhshQcB/amxnwCXwHf1Qw6rm6eH7T2+d9sJK+YObJJmYiIByLiXEfv1kPs15IHWcpk4rPOZpu7ec6qB9W1tVNWR9UX1Z8LEhgvuNgVr7vq+w1E/6t+rD6lrqgtvCCRq0x2i9U1rQulHEj8Hqoh/E/1FXVT16IrJjZVIOJk4hPqZyXCv1H3qtf3RXhO3M3qsQJB2xO/dS2ReS6o76j39UpP438p1QlgK3BTy/R5RHyQ+AyRbTveBZwDjkbE702vOWDAgCv5DyyzjR7/CUzHAAAAAElFTkSuQmCC)](https://pypi.org/project/black/)
 
 license icon by [Daniel Bruce](https://www.iconfinder.com/icons/216659/license_icon),
 format icon by [Picol](https://www.iconfinder.com/icons/103509/document_text_icon),
 status icon by [Just Icon](https://www.iconfinder.com/icons/2672768/app_battery_essential_object_status_ui_ux_icon),
 code style icon by [Google Material Design icons](https://www.iconfinder.com/icons/352148/style_icon)
 
 *pandoc-numbering* is a [pandoc] filter for numbering all kinds of things.
 
 [pandoc]: http://pandoc.org/
 
-Documentation
--------------
-
-See the [Read the docs pages](http://pandoc-numbering.readthedocs.io/en/3.4.0.1/).
-
-Usage
------
-
-To apply the filter, use the following option with pandoc:
-
-    --filter pandoc-numbering
-
-Installation
+Instructions
 ------------
 
 *pandoc-numbering* requires [python], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows]. Either python 2.7 or 3.x will do.
 
-Install *pandoc-numbering* as root using the bash command
+Install *pandoc-numbering* using the bash command
 
-    pip install pandoc-numbering
+~~~shell
+$ pip install pandoc-numbering
+~~~
 
 To upgrade to the most recent release, use
 
-    pip install --upgrade pandoc-numbering
+~~~shell
+$ pip install --upgrade pandoc-numbering
+~~~
 
 To upgrade to the current code, use
 
-    pip install --upgrade --force --no-cache git+https://github.com/chdemko/pandoc-numbering
+~~~shell
+$ pip install --upgrade --force --no-cache git+https://github.com/chdemko/pandoc-numbering
+~~~
 
 `pip` is a script that downloads and installs modules from the Python Package Index, [PyPI].  It should come installed with your python distribution. If you are running linux, `pip` may be bundled separately. On a Debian-based system (including Ubuntu), you can install it as root using
 
-    apt-get update
-    apt-get install python-pip
+~~~shell
+$ sudo apt-get install python3-pip
+~~~
 
 Make sure you have the
 
 * *tocloft*
 
 LaTeX package. On linux you have to install some extra libraries **before**
 *pandoc-numbering*. On a Debian-based system (including Ubuntu), you can install it as
 root using
 
-	apt-get install texlive-latex-extra
+~~~shell
+$ sudo apt-get install texlive-latex-extra
+~~~
 
 [python]: https://www.python.org/
 [on Windows]: https://www.python.org/downloads/windows/
 [PyPI]: https://pypi.python.org/pypi
 
 
 Getting Help
```

### Comparing `pandoc-numbering-3.4.0.1/pandoc_numbering.py` & `pandoc_numbering-3.4.0.2/pandoc_numbering.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 #!/usr/bin/env python
 
 # pylint: disable=too-many-lines
 
-"""
-Pandoc filter to number all kinds of things.
-"""
+"""Pandoc filter to number all kinds of things."""
 
 import copy
 import re
 import unicodedata
 from functools import partial
 
 from panflute import (  # type: ignore
@@ -26,43 +24,43 @@
     HorizontalRule,
     Image,
     LineBlock,
     LineBreak,
     LineItem,
     Link,
     ListItem,
+    MetaBool,
+    MetaInlines,
+    MetaList,
+    MetaMap,
+    MetaString,
     Note,
     Para,
     Plain,
     RawBlock,
     RawInline,
     SoftBreak,
     Space,
     Span,
     Str,
     Strong,
     Table,
     TableCell,
     TableRow,
-    MetaBool,
-    MetaInlines,
-    MetaList,
-    MetaMap,
-    MetaString,
-    run_filters,
-    stringify,
     convert_text,
     debug,
+    run_filters,
+    stringify,
 )
 
 
 # pylint: disable=bad-option-value,useless-object-inheritance
-class Numbered(object):
+class Numbered:
     """
-    Numbered elements
+    Numbered elements.
     """
 
     # pylint: disable=too-many-instance-attributes
     __slots__ = [
         "_elem",
         "_doc",
         "_match",
@@ -84,92 +82,140 @@
         "_section_alias",
         "_alias",
     ]
 
     @property
     def tag(self):
         """
-        Get tag property.
+        Get the tag property.
+
+        Returns
+        -------
+            The tag property.
         """
         return self._tag
 
     @property
     def entry(self):
         """
-        Get entry property.
+        Get the entry property.
+
+        Returns
+        -------
+            The entry property.
         """
         return self._entry
 
     @property
     def link(self):
         """
-        Get link property.
+        Get the link property.
+
+        Returns
+        -------
+            The link property.
         """
         return self._link
 
     @property
     def title(self):
         """
-        Get title property.
+        Get the title property.
+
+        Returns
+        -------
+            The title property.
         """
         return self._title
 
     @property
     def description(self):
         """
-        Get description property.
+        Get the description property.
+
+        Returns
+        -------
+            The description property.
         """
         return self._description
 
     @property
     def global_number(self):
         """
-        Get global_number property.
+        Get the global_number property.
+
+        Returns
+        -------
+            The global_number property.
         """
         return self._global_number
 
     @property
     def section_number(self):
         """
-        Get section_number property.
+        Get the section_number property.
+
+        Returns
+        -------
+            The section_number property.
         """
         return self._section_number
 
     @property
     def section_alias(self):
         """
-        Get section_alias property.
+        Get the section_alias property.
+
+        Returns
+        -------
+            The section_alias property.
         """
         return self._section_alias
 
     @property
     def alias(self):
         """
-        Get alias property.
+        Get the alias property.
+
+        Returns
+        -------
+            The alias property.
         """
         return self._alias
 
     @property
     def local_number(self):
         """
-        Get local_number property.
+        Get the local_number property.
+
+        Returns
+        -------
+            The local_number property.
         """
         return self._local_number
 
     @property
     def category(self):
         """
-        Get category property.
+        Get the category property.
+
+        Returns
+        -------
+            The category property.
         """
         return self._category
 
     @property
     def caption(self):
         """
-        Get caption property.
+        Get the caption property.
+
+        Returns
+        -------
+            The caption property.
         """
         return self._caption
 
     number_regex = "#((?P<prefix>[a-zA-Z][\\w.-]*):)?(?P<name>[a-zA-Z][\\w:.-]*)?"
     _regex = "(?P<header>(?P<hidden>(-\\.)*)(\\+\\.)*)"
     header_regex = "^" + _regex + "$"
     marker_regex = "^" + _regex + number_regex + "$"
@@ -185,19 +231,27 @@
     def _identifier(string):
         # replace invalid characters by dash
         string = re.sub(
             "[^0-9a-zA-Z_-]+", "-", Numbered._remove_accents(string.lower())
         )
 
         # Remove leading digits
-        string = re.sub("^[^a-zA-Z]+", "", string)
-
-        return string
+        return re.sub("^[^a-zA-Z]+", "", string)
 
     def __init__(self, elem, doc):
+        """
+        Initialise an instance.
+
+        Arguments
+        ---------
+        elem
+            An element.
+        doc
+            The document.
+        """
         self._elem = elem
         self._doc = doc
         self._tag = None
         self._entry = Span(classes=["pandoc-numbering-entry"])
         self._link = Span(classes=["pandoc-numbering-link"])
         self._caption = None
         self._title = None
@@ -257,15 +311,15 @@
 
     def _compute_title(self):
         self._title = []
         if (
             isinstance(self._get_content()[-3], Str)
             and self._get_content()[-3].text[-1:] == ")"
         ):
-            for (i, item) in enumerate(self._get_content()):
+            for i, item in enumerate(self._get_content()):
                 if isinstance(item, Str) and item.text[0] == "(":
                     self._title = self._get_content()[i:-2]
                     # Detach from original parent
                     self._title.parent = None
                     self._title[0].text = self._title[0].text[1:]
                     self._title[-1].text = self._title[-1].text[:-1]
                     del self._get_content()[i - 1 : -2]
@@ -290,15 +344,15 @@
 
     def _compute_levels(self):
         # Compute the first and last section level values
         self._first_section_level = len(self._match.group("hidden")) // 2
         self._last_section_level = len(self._match.group("header")) // 2
 
         # Get the default first and last section level
-        if self._first_section_level == 0 and self._last_section_level == 0:
+        if self._first_section_level == self._last_section_level == 0:
             self._first_section_level = self._doc.defined[self._basic_category][
                 "first-section-level"
             ]
             self._last_section_level = self._doc.defined[self._basic_category][
                 "last-section-level"
             ]
 
@@ -389,15 +443,15 @@
         # Compute the global number
         if self._section_number:
             self._global_number = self._section_number + "." + self._number
         else:
             self._global_number = self._number
 
     def _compute_data(self):
-        # pylint: disable=too-many-statements
+        # pylint: disable=too-many-statements,no-member
         classes = self._doc.defined[self._basic_category]["classes"]
         self._set_content(
             [
                 Span(identifier=self._alias),
                 Span(identifier=self._tag, classes=["pandoc-numbering-text"] + classes),
             ]
         )
@@ -428,15 +482,15 @@
             self._entry.content = copy.deepcopy(
                 self._doc.defined[self._basic_category]["format-entry-classic"]
             )
             self._caption = self._doc.defined[self._basic_category][
                 "format-caption-classic"
             ]
 
-        # Compute caption (delay replacing %c at the end since it is not known for the moment)
+        # Compute caption (delay replacing %c at the end)
         title = stringify(Span(*self._title))
         description = stringify(Span(*self._description))
         self._caption = self._caption.replace("%t", title.lower())
         self._caption = self._caption.replace("%T", title)
         self._caption = self._caption.replace("%d", description.lower())
         self._caption = self._caption.replace("%D", description)
         self._caption = self._caption.replace("%s", self._section_number)
@@ -483,138 +537,148 @@
             )
             self._get_content()[1].content.insert(
                 0, RawInline("\\label{" + self._tag + "}", "tex")
             )
 
             latex_category = re.sub("[^a-z]+", "", self._basic_category)
             latex = (
-                "\\phantomsection\\addcontentsline{"
-                + latex_category
-                + "}{"
-                + latex_category
-                + "}{\\protect\\numberline {"
-                + self._leading
-                + self._number
-                + "}{\\ignorespaces "
-                + to_latex(self._entry)
-                + "}}"
+                "\\phantomsection"
+                f"\\addcontentsline{{{latex_category}}}{{{latex_category}}}"
+                f"{{\\protect\\numberline {{{self._leading + self._number}}}"
+                f"{{\\ignorespaces {to_latex(self._entry)}"
+                "}}"
             )
             self._get_content().insert(0, RawInline(latex, "tex"))
 
 
 def replace_description(where, description):
     """
     Replace description in where.
 
     Arguments
     ---------
-        where: where to replace
-        description: replace %D and %d by description
+    where
+        where to replace
+    description
+        replace %D and %d by description
     """
     where.walk(partial(replacing, search="%D", replace=copy.deepcopy(description)))
     where.walk(
         partial(
             replacing,
             search="%d",
-            replace=list(item.walk(lowering) for item in copy.deepcopy(description)),
+            replace=[item.walk(lowering) for item in copy.deepcopy(description)],
         )
     )
 
 
 def replace_title(where, title):
     """
     Replace title in where.
 
     Arguments
     ---------
-        where: where to replace
-        title: replace %T and %t by title
+    where
+        where to replace
+    title
+        replace %T and %t by title
     """
     where.walk(partial(replacing, search="%T", replace=copy.deepcopy(title)))
     where.walk(
         partial(
             replacing,
             search="%t",
-            replace=list(item.walk(lowering) for item in copy.deepcopy(title)),
+            replace=[item.walk(lowering) for item in copy.deepcopy(title)],
         )
     )
 
 
 def replace_section_number(where, section_number):
     """
     Replace section number in where.
 
     Arguments
     ---------
-        where: where to replace
-        section_number: replace %s by section_number
+    where
+        where to replace
+    section_number
+        replace %s by section_number
     """
     where.walk(partial(replacing, search="%s", replace=[Str(section_number)]))
 
 
 def replace_global_number(where, global_number):
     """
     Replace global number in where.
 
     Arguments
     ---------
-        where: where to replace
-        global_number: replace %g by global_number
+    where
+        where to replace
+    global_number
+        replace %g by global_number
     """
     where.walk(partial(replacing, search="%g", replace=[Str(global_number)]))
 
 
 def replace_local_number(where, local_number):
     """
     Replace local number in where.
 
     Arguments
     ---------
-        where: where to replace
-        local_number: replace %n and # by local_number
+    where
+        where to replace
+    local_number
+        replace %n and # by local_number
     """
     where.walk(partial(replacing, search="%n", replace=[Str(local_number)]))
     where.walk(partial(replacing, search="#", replace=[Str(local_number)]))
 
 
 def replace_page_number(where, tag):
     """
     Replace page number in where.
 
     Arguments
     ---------
-        where: where to replace
-        tag: replace %p by tag
+    where
+        where to replace
+    tag
+        replace %p by tag
     """
     where.walk(
         partial(
             replacing, search="%p", replace=[RawInline("\\pageref{" + tag + "}", "tex")]
         )
     )
 
 
 def replace_count(where, count):
     """
     Replace count in where.
 
     Arguments
     ---------
-        where: where to replace
-        count: replace %c by count
+    where
+        where to replace
+    count
+        replace %c by count
     """
     where.walk(partial(replacing, search="%c", replace=[Str(count)]))
 
 
 def remove_useless_latex(elem, _):
     """
     Clean up LaTeX element for entries.
 
     Arguments
     ---------
-        elem: elem to scan
+    elem
+        elem to scan
 
     Returns
     -------
         []: if elem is an instance to remove
         None: otherwise
     """
     if isinstance(
@@ -652,15 +716,16 @@
 
 def to_latex(elem):
     """
     Convert element to LaTeX.
 
     Arguments
     ---------
-        elem: elem to convert
+    elem
+        elem to convert
 
     Returns
     -------
         LaTex string
     """
     return convert_text(
         run_filters([remove_useless_latex], doc=Plain(elem)),
@@ -672,16 +737,18 @@
 
 def define(category, doc):
     """
     Define a category in document.
 
     Arguments
     ---------
-        category: category to define
-        doc: pandoc document
+    category
+        category to define
+    doc
+        pandoc document
     """
     # pylint: disable=line-too-long
     doc.defined[category] = {
         "first-section-level": 0,
         "last-section-level": 0,
         "format-text-classic": [Strong(Str("%D"), Space(), Str("%n"))],
         "format-text-title": [
@@ -713,37 +780,41 @@
 
 def lowering(elem, _):
     """
     Lower element.
 
     Arguments
     ---------
-        elem: element to lower
+    elem
+        element to lower
     """
     if isinstance(elem, Str):
         elem.text = elem.text.lower()
 
 
 def replacing(elem, _, search=None, replace=None):
     """
-    Function to replace.
+    Replace an element.
 
     Arguments
     ---------
-        elem: element to scan
+    elem
+        element to scan
+    search
+        string to search
+    replace
+        string to replace
 
-    Keyword arguments
-    -----------------
-        search: string to search
-        replace: string to replace
+    Returns
+    -------
+        The modified elements.
     """
     if isinstance(elem, Str):
         search_splitted = elem.text.split(search)
         if len(search_splitted) > 1:
-
             text = []
 
             if search_splitted[0] != "":
                 text.append(Str(search_splitted[0]))
 
             for string in search_splitted[1:]:
                 text.extend(replace)
@@ -753,56 +824,66 @@
             return text
 
     return [elem]
 
 
 def numbering(elem, doc):
     """
-    number element.
+    Add the numbering of an element.
 
     Arguments
     ---------
-        elem: element to number
-        doc: pandoc document
+    elem
+        element to number
+    doc
+        pandoc document
     """
     if isinstance(elem, Header):
         update_header_numbers(elem, doc)
         update_header_aliases(elem, doc)
     elif isinstance(elem, (Para, DefinitionItem)):
         numbered = Numbered(elem, doc)
         if numbered.tag is not None:
             doc.information[numbered.tag] = numbered
 
 
 def referencing(elem, doc):
     """
-    reference element.
+    Add a reference for an element.
 
     Arguments
     ---------
-        elem: element to reference
-        doc: pandoc document
+    elem
+        element to reference
+    doc
+        pandoc document
+
+    Returns
+    -------
+        A Link or None
     """
     if isinstance(elem, Link):
         return referencing_link(elem, doc)
     if isinstance(elem, Cite):
         return referencing_cite(elem, doc)
     if isinstance(elem, Span) and elem.identifier in doc.information:
         replace_count(elem, str(doc.count[doc.information[elem.identifier].category]))
     return None
 
 
 def referencing_link(elem, doc):
     """
-    reference link.
+    Add a eference link.
 
     Arguments
     ---------
-        elem: element to reference
-        doc: pandoc document
+    elem
+        element to reference
+    doc
+        pandoc document
     """
     match = re.match("^#(?P<tag>([a-zA-Z][\\w:.-]*))$", elem.url)
     if match:
         tag = match.group("tag")
         if tag in doc.information:
             replace_title(elem, doc.information[tag].title)
             replace_description(elem, doc.information[tag].description)
@@ -828,20 +909,26 @@
             )
             if doc.format in {"tex", "latex"}:
                 elem.title = elem.title.replace("%p", "\\pageref{" + tag + "}")
 
 
 def referencing_cite(elem, doc):
     """
-    reference cite.
+    Cite reference.
 
     Arguments
     ---------
-        elem: element to reference
-        doc: pandoc document
+    elem
+        element to reference
+    doc
+        pandoc document
+
+    Returns
+    -------
+        A Link or None
     """
     if len(elem.content) == 1 and isinstance(elem.content[0], Str):
         match = re.match(
             "^(@(?P<tag>(?P<category>[a-zA-Z][\\w.-]*):(([a-zA-Z][\\w.-]*)|(\\d*(\\.\\d*)*))))$",
             elem.content[0].text,
         )
         if match:
@@ -860,48 +947,53 @@
                     replace_count(ret, str(doc.count[doc.information[tag].category]))
                     return ret
     return None
 
 
 def update_header_numbers(elem, doc):
     """
-    update header numbers.
+    Update header numbers.
 
     Arguments
     ---------
-        elem: element to update
-        doc: pandoc document
+    elem
+        element to update
+    doc
+        pandoc document
     """
     if "unnumbered" not in elem.classes:
         doc.headers[elem.level - 1] = doc.headers[elem.level - 1] + 1
         for index in range(elem.level, 6):
             doc.headers[index] = 0
 
 
 def update_header_aliases(elem, doc):
     """
-    update header aliases.
+    Update header aliases.
 
     Arguments
     ---------
-        elem: element to update
-        doc: pandoc document
+    elem
+        element to update
+    doc
+        pandoc document
     """
     doc.aliases[elem.level - 1] = elem.identifier
     for index in range(elem.level, 6):
         doc.aliases[index] = ""
 
 
 def prepare(doc):
     """
     Prepare document.
 
     Arguments
     ---------
-        doc: pandoc document
+    doc
+        pandoc document
     """
     doc.headers = [0, 0, 0, 0, 0, 0]
     doc.aliases = ["", "", "", "", "", ""]
     doc.information = {}
     doc.defined = {}
 
     if "pandoc-numbering" in doc.metadata.content and isinstance(
@@ -919,17 +1011,20 @@
 
 def add_definition(category, definition, doc):
     """
     Add definition for a category.
 
     Arguments
     ---------
-        category:
-        definition:
-        defined:
+    category
+        The category
+    definition
+        The definition
+    doc
+        The pandoc document
     """
     # Create the category with options by default
     define(category, doc)
 
     # Detect general options
     if "general" in definition:
         meta_cite(category, definition["general"], doc.defined)
@@ -957,17 +1052,20 @@
 
 def meta_cite(category, definition, defined):
     """
     Compute cite for a category.
 
     Arguments
     ---------
-        category:
-        definition:
-        defined:
+    category
+        The category
+    definition
+        The definition
+    defined
+        The defined parameter
     """
     if "cite-shortcut" in definition:
         if isinstance(definition["cite-shortcut"], MetaBool):
             defined[category]["cite-shortcut"] = definition["cite-shortcut"].boolean
         else:
             debug(
                 "[WARNING] pandoc-numbering: cite-shortcut is not correct for category "
@@ -978,17 +1076,20 @@
 # pylint:disable=too-many-branches
 def meta_listing(category, definition, defined):
     """
     Compute listing for a category.
 
     Arguments
     ---------
-        category:
-        definition:
-        defined:
+    category
+        The category
+    definition
+        The definition
+    defined
+        The defined parameter
     """
     if "listing-title" in definition:
         if isinstance(definition["listing-title"], MetaInlines):
             defined[category]["listing-title"] = definition["listing-title"].content
             # Detach from original parent
             defined[category]["listing-title"].parent = None
         else:
@@ -999,26 +1100,26 @@
     if "listing-unnumbered" in definition:
         if isinstance(definition["listing-unnumbered"], MetaBool):
             defined[category]["listing-unnumbered"] = definition[
                 "listing-unnumbered"
             ].boolean
         else:
             debug(
-                "[WARNING] pandoc-numbering: listing-unnumbered is not correct for category "
-                + category
+                "[WARNING] pandoc-numbering: "
+                "listing-unnumbered is not correct for category " + category
             )
     if "listing-unlisted" in definition:
         if isinstance(definition["listing-unlisted"], MetaBool):
             defined[category]["listing-unlisted"] = definition[
                 "listing-unlisted"
             ].boolean
         else:
             debug(
-                "[WARNING] pandoc-numbering: listing-unlisted is not correct for category "
-                + category
+                "[WARNING] pandoc-numbering: "
+                "listing-unlisted is not correct for category " + category
             )
     if "listing-identifier" in definition:
         if isinstance(definition["listing-identifier"], MetaBool):
             defined[category]["listing-identifier"] = definition[
                 "listing-identifier"
             ].boolean
         elif (
@@ -1027,172 +1128,187 @@
             and isinstance(definition["listing-identifier"].content[0], Str)
         ):
             defined[category]["listing-identifier"] = (
                 definition["listing-identifier"].content[0].text
             )
         else:
             debug(
-                "[WARNING] pandoc-numbering: listing-identifier is not correct for category "
-                + category
+                "[WARNING] pandoc-numbering: "
+                "listing-identifier is not correct for category " + category
             )
 
 
 def meta_format_text(category, definition, defined):
     """
     Compute format text for a category.
 
     Arguments
     ---------
-        category:
-        definition:
-        defined:
+    category
+        The category
+    definition
+        The definition
+    defined
+        The defined parameter
     """
     if "format-text-classic" in definition:
         if isinstance(definition["format-text-classic"], MetaInlines):
             defined[category]["format-text-classic"] = definition[
                 "format-text-classic"
             ].content
             # Detach from original parent
             defined[category]["format-text-classic"].parent = None
         else:
             debug(
-                "[WARNING] pandoc-numbering: format-text-classic is not correct for category "
-                + category
+                "[WARNING] pandoc-numbering: "
+                "format-text-classic is not correct for category " + category
             )
 
     if "format-text-title" in definition:
         if isinstance(definition["format-text-title"], MetaInlines):
             defined[category]["format-text-title"] = definition[
                 "format-text-title"
             ].content
             # Detach from original parent
             defined[category]["format-text-title"].parent = None
         else:
             debug(
-                "[WARNING] pandoc-numbering: format-text-title is not correct for category "
-                + category
+                "[WARNING] pandoc-numbering: "
+                "format-text-title is not correct for category " + category
             )
 
 
 def meta_format_link(category, definition, defined):
     """
     Compute format link for a category.
 
     Arguments
     ---------
-        category:
-        definition:
-        defined:
+    category
+        The category
+    definition
+        The definition
+    defined
+        The defined parameter
     """
     if "format-link-classic" in definition:
         if isinstance(definition["format-link-classic"], MetaInlines):
             defined[category]["format-link-classic"] = definition[
                 "format-link-classic"
             ].content
             # Detach from original parent
             defined[category]["format-link-classic"].parent = None
         else:
             debug(
-                "[WARNING] pandoc-numbering: format-link-classic is not correct for category "
-                + category
+                "[WARNING] pandoc-numbering: "
+                "format-link-classic is not correct for category " + category
             )
 
     if "format-link-title" in definition:
         if isinstance(definition["format-link-title"], MetaInlines):
             defined[category]["format-link-title"] = definition[
                 "format-link-title"
             ].content
             # Detach from original parent
             defined[category]["format-link-title"].parent = None
         else:
             debug(
-                "[WARNING] pandoc-numbering: format-link-title is not correct for category "
-                + category
+                "[WARNING] pandoc-numbering: "
+                "format-link-title is not correct for category " + category
             )
 
 
 def meta_format_caption(category, definition, defined):
     """
     Compute format caption for a category.
 
     Arguments
     ---------
-        category:
-        definition:
-        defined:
+    category
+        The category
+    definition
+        The definition
+    defined
+        The defined parameter
     """
     if "format-caption-classic" in definition:
         if isinstance(definition["format-caption-classic"], MetaInlines):
             defined[category]["format-caption-classic"] = stringify(
                 definition["format-caption-classic"]
             )
         else:
             debug(
-                "[WARNING] pandoc-numbering: format-caption-classic is not correct for category "
-                + category
+                "[WARNING] pandoc-numbering: "
+                "format-caption-classic is not correct for category " + category
             )
 
     if "format-caption-title" in definition:
         if isinstance(definition["format-caption-title"], MetaInlines):
             defined[category]["format-caption-title"] = stringify(
                 definition["format-caption-title"]
             )
         else:
             debug(
-                "[WARNING] pandoc-numbering: format-caption-title is not correct for category "
-                + category
+                "[WARNING] pandoc-numbering: "
+                "format-caption-title is not correct for category " + category
             )
 
 
 def meta_format_entry(category, definition, defined):
     """
     Compute format entry for a category.
 
     Arguments
     ---------
-        category:
-        definition:
-        defined:
+    category
+        The category
+    definition
+        The definition
+    defined
+        The defined parameter
     """
     if "format-entry-classic" in definition:
         if isinstance(definition["format-entry-classic"], MetaInlines):
             defined[category]["format-entry-classic"] = definition[
                 "format-entry-classic"
             ].content
             # Detach from original parent
             defined[category]["format-entry-classic"].parent = None
         else:
             debug(
-                "[WARNING] pandoc-numbering: format-entry-classic is not correct for category "
-                + category
+                "[WARNING] pandoc-numbering: "
+                "format-entry-classic is not correct for category " + category
             )
 
     if "format-entry-title" in definition:
         if isinstance(definition["format-entry-title"], MetaInlines):
             defined[category]["format-entry-title"] = definition[
                 "format-entry-title"
             ].content
             # Detach from original parent
             defined[category]["format-entry-title"].parent = None
         else:
             debug(
-                "[WARNING] pandoc-numbering: format-entry-title is not correct for category "
-                + category
+                "[WARNING] pandoc-numbering: "
+                "format-entry-title is not correct for category " + category
             )
 
 
 def meta_entry_tab(category, definition, defined):
     """
     Compute entry tab for a category.
 
     Arguments
     ---------
-        category:
-        definition:
-        defined:
+    category
+        The category
+    definition
+        The definition
+    defined
+        The defined parameter
     """
     if "entry-tab" in definition:
         if isinstance(definition["entry-tab"], MetaString):
             value = definition["entry-tab"].text
         elif (
             isinstance(definition["entry-tab"], MetaInlines)
             and len(definition["entry-tab"].content) == 1
@@ -1207,33 +1323,36 @@
         # Get the tab
         try:
             tab = float(value)
             if tab > 0:
                 defined[category]["entry-tab"] = tab
             else:
                 debug(
-                    "[WARNING] pandoc-numbering: entry-tab must be positive for category "
-                    + category
+                    "[WARNING] pandoc-numbering: "
+                    "entry-tab must be positive for category " + category
                 )
         except ValueError:
             debug(
                 "[WARNING] pandoc-numbering: entry-tab is not correct for category "
                 + category
             )
 
 
 def meta_entry_space(category, definition, defined):
     """
     Compute entry space for a category.
 
     Arguments
     ---------
-        category:
-        definition:
-        defined:
+    category
+        The category
+    definition
+        The definition
+    defined
+        The defined parameter
     """
     if "entry-space" in definition:
         if isinstance(definition["entry-space"], MetaString):
             value = definition["entry-space"].text
         elif (
             isinstance(definition["entry-space"], MetaInlines)
             and len(definition["entry-space"].content) == 1
@@ -1248,33 +1367,36 @@
         # Get the space
         try:
             space = float(value)
             if space > 0:
                 defined[category]["entry-space"] = space
             else:
                 debug(
-                    "[WARNING] pandoc-numbering: entry-space must be positive for category "
-                    + category
+                    "[WARNING] pandoc-numbering: "
+                    "entry-space must be positive for category " + category
                 )
         except ValueError:
             debug(
                 "[WARNING] pandoc-numbering: entry-space is not correct for category "
                 + category
             )
 
 
 def meta_levels(category, definition, defined):
     """
     Compute level for a category.
 
     Arguments
     ---------
-        category:
-        definition:
-        defined:
+    category
+        The category
+    definition
+        The definition
+    defined
+        The defined parameter
     """
     if (
         "sectioning-levels" in definition
         and isinstance(definition["sectioning-levels"], MetaInlines)
         and len(definition["sectioning-levels"].content) == 1
     ):
         match = re.match(
@@ -1290,95 +1412,98 @@
         elif (
             isinstance(definition["first-section-level"], MetaInlines)
             and len(definition["first-section-level"].content) == 1
         ):
             value = definition["first-section-level"].content[0].text
         else:
             debug(
-                "[WARNING] pandoc-numbering: first-section-level is not correct for category "
-                + category
+                "[WARNING] pandoc-numbering: "
+                "first-section-level is not correct for category " + category
             )
             return
 
         # Get the level
         try:
             level = int(value) - 1
         except ValueError:
             debug(
-                "[WARNING] pandoc-numbering: first-section-level is not correct for category "
-                + category
+                "[WARNING] pandoc-numbering: "
+                "first-section-level is not correct for category " + category
             )
 
         if 0 <= level <= 6:
             defined[category]["first-section-level"] = level
         else:
             # pylint: disable=line-too-long
             debug(
-                "[WARNING] pandoc-numbering: first-section-level must be positive or zero for category "
-                + category
+                "[WARNING] pandoc-numbering: "
+                "first-section-level must be positive or zero for category " + category
             )
 
     if "last-section-level" in definition:
         if isinstance(definition["last-section-level"], MetaString):
             value = definition["last-section-level"].text
         elif (
             isinstance(definition["last-section-level"], MetaInlines)
             and len(definition["last-section-level"].content) == 1
         ):
             value = definition["last-section-level"].content[0].text
         else:
             debug(
-                "[WARNING] pandoc-numbering: last-section-level is not correct for category "
-                + category
+                "[WARNING] pandoc-numbering: "
+                "last-section-level is not correct for category " + category
             )
             return
 
         # Get the level
         try:
             level = int(value)
         except ValueError:
             debug(
-                "[WARNING] pandoc-numbering: last-section-level is not correct for category "
-                + category
+                "[WARNING] pandoc-numbering: "
+                "last-section-level is not correct for category " + category
             )
 
         if 0 <= level <= 6:
             defined[category]["last-section-level"] = level
         else:
             # pylint: disable=line-too-long
             debug(
-                "[WARNING] pandoc-numbering: last-section-level must be positive or zero for category "
-                + category
+                "[WARNING] pandoc-numbering: "
+                "last-section-level must be positive or zero for category " + category
             )
 
 
 def meta_classes(category, definition, defined):
     """
     Compute classes for a category.
 
     Arguments
     ---------
-        category:
-        definition:
-        defined:
+    category
+        The category
+    definition
+        The definition
+    defined
+        The defined parameter
     """
     if "classes" in definition and isinstance(definition["classes"], MetaList):
-        classes = []
-        for elt in definition["classes"].content:
-            classes.append(stringify(elt))
-        defined[category]["classes"] = classes
+        defined[category]["classes"] = [
+            stringify(elt) for elt in definition["classes"].content
+        ]
 
 
 def finalize(doc):
     """
     Finalize document.
 
     Arguments
     ---------
-        doc: pandoc document
+    doc
+        The pandoc document
     """
     # Loop on all listings definition
 
     if doc.format in {"tex", "latex"}:
         # Add header-includes if necessary
         if "header-includes" not in doc.metadata:
             doc.metadata["header-includes"] = MetaList()
@@ -1417,15 +1542,15 @@
                         latex_category,
                         latex_category,
                     )
                 )
                 doc.metadata["header-includes"].append(
                     MetaInlines(RawInline(latex, "tex"))
                 )
-                listof.append(r"\listof%s" % latex_category)
+                listof.append(f"\\listof{latex_category}")
             else:
                 classes = ["pandoc-numbering-listing"] + definition["classes"]
 
                 if definition["listing-unnumbered"]:
                     classes.append("unnumbered")
 
                 if definition["listing-unlisted"]:
@@ -1446,15 +1571,15 @@
                         output_format="panflute",
                     )[0]
                 else:
                     header = Header(
                         *definition["listing-title"],
                         level=1,
                         classes=classes,
-                        identifier=definition["listing-identifier"]
+                        identifier=definition["listing-identifier"],
                     )
 
                 doc.content.insert(i, header)
                 i = i + 1
 
                 table = table_other(doc, category, definition)
 
@@ -1478,55 +1603,61 @@
 
 def table_other(doc, category, _):
     """
     Compute other code for table.
 
     Arguments
     ---------
-        doc: pandoc document
-        category: category numbered
-        definition: definition
+    doc
+        pandoc document
+    category
+        category numbered
+
+    Returns
+    -------
+        A BulletList or None
     """
     if category in doc.collections:
-        # Prepare the list
-        elements = []
-        # Loop on the collection
-        for tag in doc.collections[category]:
-            # Add an item to the list
-            elements.append(
+        # Return a bullet list
+        return BulletList(
+            *(
                 ListItem(Plain(Link(doc.information[tag].entry, url="#" + tag)))
+                for tag in doc.collections[category]
             )
-        # Return a bullet list
-        return BulletList(*elements)
+        )
     return None
 
 
 def link_color(doc):
     """
     Compute LaTeX code for toc.
 
     Arguments
     ---------
-        doc: pandoc document
+    doc
+        pandoc document
+
+    Returns
+    -------
+        LaTeX code for links.
     """
     # Get the link color
     metadata = doc.get_metadata()
     if "toccolor" in metadata:
         return "\\hypersetup{linkcolor=" + str(metadata["toccolor"]) + "}"
     return "\\hypersetup{linkcolor=black}"
 
 
-def main(doc=None):
+def main(doc=None) -> None:
     """
-    main function.
+    Produce the final document.
 
-    Arguments
-    ---------
-        doc: pandoc document
+    Parameters
+    ----------
+    doc
+        pandoc document
     """
-    return run_filters(
-        [numbering, referencing], prepare=prepare, doc=doc, finalize=finalize
-    )
+    run_filters([numbering, referencing], prepare=prepare, doc=doc, finalize=finalize)
 
 
 if __name__ == "__main__":
     main()
```

