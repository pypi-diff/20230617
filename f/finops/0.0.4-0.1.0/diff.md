# Comparing `tmp/finops-0.0.4.tar.gz` & `tmp/finops-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finops-0.0.4.tar", last modified: Thu Jun 15 19:36:42 2023, max compression
+gzip compressed data, was "finops-0.1.0.tar", last modified: Fri Jun 16 23:13:26 2023, max compression
```

## Comparing `finops-0.0.4.tar` & `finops-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:36:42.714764 finops-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-15 19:36:31.000000 finops-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-15 19:36:42.714764 finops-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:36:31.000000 finops-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:36:42.710764 finops-0.0.4/finops/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:36:31.000000 finops-0.0.4/finops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:36:42.710764 finops-0.0.4/finops/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:36:31.000000 finops-0.0.4/finops/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:36:31.000000 finops-0.0.4/finops/data/shareholders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:36:42.710764 finops-0.0.4/finops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-15 19:36:42.000000 finops-0.0.4/finops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-15 19:36:42.000000 finops-0.0.4/finops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 19:36:42.000000 finops-0.0.4/finops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 19:36:42.000000 finops-0.0.4/finops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 19:36:42.000000 finops-0.0.4/finops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 19:36:42.714764 finops-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-15 19:36:31.000000 finops-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:36:42.714764 finops-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:36:31.000000 finops-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:36:31.000000 finops-0.0.4/tests/test_shareholders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:13:26.561515 finops-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-16 23:13:16.000000 finops-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-16 23:13:26.561515 finops-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-16 23:13:16.000000 finops-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:13:26.561515 finops-0.1.0/finops/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-16 23:13:16.000000 finops-0.1.0/finops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-16 23:13:16.000000 finops-0.1.0/finops/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-16 23:13:16.000000 finops-0.1.0/finops/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-16 23:13:16.000000 finops-0.1.0/finops/tehran_stock_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-16 23:13:16.000000 finops-0.1.0/finops/ticker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:13:26.561515 finops-0.1.0/finops/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 23:13:16.000000 finops-0.1.0/finops/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-16 23:13:16.000000 finops-0.1.0/finops/utils/base_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-16 23:13:16.000000 finops-0.1.0/finops/utils/base_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-16 23:13:16.000000 finops-0.1.0/finops/utils/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:13:26.561515 finops-0.1.0/finops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-16 23:13:26.000000 finops-0.1.0/finops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-16 23:13:26.000000 finops-0.1.0/finops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 23:13:26.000000 finops-0.1.0/finops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 23:13:26.000000 finops-0.1.0/finops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 23:13:26.000000 finops-0.1.0/finops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 23:13:26.561515 finops-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-16 23:13:16.000000 finops-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:13:26.561515 finops-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 23:13:16.000000 finops-0.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-16 23:13:16.000000 finops-0.1.0/tests/test_tehran_stock_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-06-16 23:13:16.000000 finops-0.1.0/tests/test_ticker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:13:26.561515 finops-0.1.0/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 23:13:16.000000 finops-0.1.0/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-16 23:13:16.000000 finops-0.1.0/tests/test_utils/test_base_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-16 23:13:16.000000 finops-0.1.0/tests/test_utils/test_base_scraper.py
```

### Comparing `finops-0.0.4/LICENSE` & `finops-0.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
 OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
 SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
 LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `finops-0.0.4/PKG-INFO` & `finops-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finops
-Version: 0.0.4
+Version: 0.1.0
 Summary: Financial tools for the rest of us.
 Home-page: https://github.com/nixuri/FinOps
 Author: Alireza Nilgaran
 Author-email: alireza.nilgaran@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `finops-0.0.4/finops.egg-info/PKG-INFO` & `finops-0.1.0/finops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finops
-Version: 0.0.4
+Version: 0.1.0
 Summary: Financial tools for the rest of us.
 Home-page: https://github.com/nixuri/FinOps
 Author: Alireza Nilgaran
 Author-email: alireza.nilgaran@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `finops-0.0.4/setup.py` & `finops-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='finops',
-    version='0.0.4',
+    version='0.1.0',
     description='Financial tools for the rest of us.',
     author='Alireza Nilgaran',
     author_email='alireza.nilgaran@gmail.com',
     url='https://github.com/nixuri/FinOps',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

