# Comparing `tmp/python-usernames-0.3.1.tar.gz` & `tmp/python-usernames-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-usernames-0.3.1.tar", last modified: Tue May  5 08:53:20 2020, max compression
+gzip compressed data, was "python-usernames-0.4.1.tar", last modified: Sat Jun 17 08:43:02 2023, max compression
```

## Comparing `python-usernames-0.3.1.tar` & `python-usernames-0.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 theskumar   (501) staff       (20)        0 2020-05-05 08:53:20.000000 python-usernames-0.3.1/
--rw-r--r--   0 theskumar   (501) staff       (20)     1081 2015-09-28 03:36:37.000000 python-usernames-0.3.1/LICENSE
--rw-r--r--   0 theskumar   (501) staff       (20)       27 2015-10-08 05:39:29.000000 python-usernames-0.3.1/MANIFEST.in
--rw-r--r--   0 theskumar   (501) staff       (20)     4420 2020-05-05 08:53:20.000000 python-usernames-0.3.1/PKG-INFO
--rw-r--r--   0 theskumar   (501) staff       (20)     2595 2020-05-05 08:06:59.000000 python-usernames-0.3.1/README.md
-drwxr-xr-x   0 theskumar   (501) staff       (20)        0 2020-05-05 08:53:20.000000 python-usernames-0.3.1/python_usernames.egg-info/
--rw-r--r--   0 theskumar   (501) staff       (20)     4420 2020-05-05 08:53:20.000000 python-usernames-0.3.1/python_usernames.egg-info/PKG-INFO
--rw-r--r--   0 theskumar   (501) staff       (20)      321 2020-05-05 08:53:20.000000 python-usernames-0.3.1/python_usernames.egg-info/SOURCES.txt
--rw-r--r--   0 theskumar   (501) staff       (20)        1 2020-05-05 08:53:20.000000 python-usernames-0.3.1/python_usernames.egg-info/dependency_links.txt
--rw-r--r--   0 theskumar   (501) staff       (20)        1 2020-05-05 08:53:20.000000 python-usernames-0.3.1/python_usernames.egg-info/not-zip-safe
--rw-r--r--   0 theskumar   (501) staff       (20)       10 2020-05-05 08:53:20.000000 python-usernames-0.3.1/python_usernames.egg-info/top_level.txt
--rw-r--r--   0 theskumar   (501) staff       (20)      235 2020-05-05 08:53:20.000000 python-usernames-0.3.1/setup.cfg
--rw-r--r--   0 theskumar   (501) staff       (20)     2699 2020-05-05 08:53:15.000000 python-usernames-0.3.1/setup.py
-drwxr-xr-x   0 theskumar   (501) staff       (20)        0 2020-05-05 08:53:20.000000 python-usernames-0.3.1/usernames/
--rw-r--r--   0 theskumar   (501) staff       (20)       97 2019-09-19 10:47:27.000000 python-usernames-0.3.1/usernames/__init__.py
--rw-r--r--   0 theskumar   (501) staff       (20)     3483 2019-09-19 10:47:34.000000 python-usernames-0.3.1/usernames/reserved_words.py
--rw-r--r--   0 theskumar   (501) staff       (20)     1170 2020-05-05 07:56:53.000000 python-usernames-0.3.1/usernames/validators.py
+drwxr-xr-x   0 theskumar   (501) staff       (20)        0 2023-06-17 08:43:02.239773 python-usernames-0.4.1/
+-rw-r--r--   0 theskumar   (501) staff       (20)     1081 2023-06-17 08:04:29.000000 python-usernames-0.4.1/LICENSE
+-rw-r--r--   0 theskumar   (501) staff       (20)       27 2023-06-17 08:04:29.000000 python-usernames-0.4.1/MANIFEST.in
+-rw-r--r--   0 theskumar   (501) staff       (20)     3771 2023-06-17 08:43:02.239852 python-usernames-0.4.1/PKG-INFO
+-rw-r--r--   0 theskumar   (501) staff       (20)     2595 2023-06-17 08:31:45.000000 python-usernames-0.4.1/README.md
+drwxr-xr-x   0 theskumar   (501) staff       (20)        0 2023-06-17 08:43:02.239304 python-usernames-0.4.1/python_usernames.egg-info/
+-rw-r--r--   0 theskumar   (501) staff       (20)     3771 2023-06-17 08:43:02.000000 python-usernames-0.4.1/python_usernames.egg-info/PKG-INFO
+-rw-r--r--   0 theskumar   (501) staff       (20)      321 2023-06-17 08:43:02.000000 python-usernames-0.4.1/python_usernames.egg-info/SOURCES.txt
+-rw-r--r--   0 theskumar   (501) staff       (20)        1 2023-06-17 08:43:02.000000 python-usernames-0.4.1/python_usernames.egg-info/dependency_links.txt
+-rw-r--r--   0 theskumar   (501) staff       (20)        1 2023-06-17 08:43:02.000000 python-usernames-0.4.1/python_usernames.egg-info/not-zip-safe
+-rw-r--r--   0 theskumar   (501) staff       (20)       10 2023-06-17 08:43:02.000000 python-usernames-0.4.1/python_usernames.egg-info/top_level.txt
+-rw-r--r--   0 theskumar   (501) staff       (20)      234 2023-06-17 08:43:02.240094 python-usernames-0.4.1/setup.cfg
+-rw-r--r--   0 theskumar   (501) staff       (20)     2699 2023-06-17 08:35:55.000000 python-usernames-0.4.1/setup.py
+drwxr-xr-x   0 theskumar   (501) staff       (20)        0 2023-06-17 08:43:02.239660 python-usernames-0.4.1/usernames/
+-rw-r--r--   0 theskumar   (501) staff       (20)       97 2023-06-17 08:31:45.000000 python-usernames-0.4.1/usernames/__init__.py
+-rw-r--r--   0 theskumar   (501) staff       (20)     3835 2023-06-17 08:31:45.000000 python-usernames-0.4.1/usernames/reserved_words.py
+-rw-r--r--   0 theskumar   (501) staff       (20)     1170 2023-06-17 08:31:45.000000 python-usernames-0.4.1/usernames/validators.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `python-usernames-0.3.1/LICENSE` & `python-usernames-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-usernames-0.3.1/PKG-INFO` & `python-usernames-0.4.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,98 +1,16 @@
 Metadata-Version: 2.1
 Name: python-usernames
-Version: 0.3.1
+Version: 0.4.1
 Summary: Python library to validate usernames suitable for use in public facing applications.
 Home-page: http://github.com/theskumar/python-usernames
 Author: Saurabh Kumar
 Author-email: me+github@saurabh-kumar.com
 License: MIT
-Description: python-usernames
-        ================
-        
-        [![Build
-        Status](https://travis-ci.org/theskumar/python-usernames.svg?branch=v0.1.0)](https://travis-ci.org/theskumar/python-usernames)
-        [![Coverage
-        Status](https://coveralls.io/repos/theskumar/python-usernames/badge.svg?branch=master&service=github)](https://coveralls.io/github/theskumar/python-usernames?branch=master)
-        [![PyPI
-        version](https://badge.fury.io/py/python-usernames.svg)](http://badge.fury.io/py/python-usernames)
-        
-        Python library to validate usernames suitable for use in public facing
-        applications where use can choose login names and sub-domains.
-        
-        Features
-        --------
-        
-        -   Provides a default regex validator
-        -   Validates against list of [banned
-            words](https://github.com/theskumar/python-usernames/blob/master/usernames/reserved_words.py)
-            that should not be used as username.
-        -   Python 2.7, 3.4, 3.5, 3.6, 3.7, 3.8 & pypi
-        
-        Installation
-        ------------
-        
-            pip install python-usernames
-        
-        Usages
-        ------
-        
-        ``` {.sourceCode .python}
-        from usernames import is_safe_username
-        
-        >>> is_safe_username("jerk")
-        False  # contains one of the banned words
-        
-        >>> is_safe_username("handsome!")
-        False  # contains non-url friendly `!`
-        ```
-        
-        **is\_safe\_username** takes the following optional arguments:
-        
-        -   `whitelist`: a case insensitive list of words that should be
-            considered as always safe. Default: `[]`
-        -   `blacklist`: a case insensitive list of words that should be
-            considered as unsafe. Default: `[]`
-        -   `max_length`: specify the maximun character a username can have.
-            Default: `None`
-        
-        - `regex`: regular expression string that must pass before the banned
-        :   words is checked.
-        
-        The default regular expression is as follows:
-        
-            ^                       # beginning of string
-            (?!_$)                  # no only _
-            (?![-.])                # no - or . at the beginning
-            (?!.*[_.-]{2})          # no __ or _. or ._ or .. or -- inside
-            [a-zA-Z0-9_.-]+         # allowed characters, atleast one must be present
-            (?<![.-])               # no - or . at the end
-            $                       # end of string
-        
-        **Further Reading**
-        
-        -   [Let’s talk about
-            usernames](https://www.b-list.org/weblog/2018/feb/11/usernames/)
-        
-        **Note:**
-        
-        Words like `bigcock12` will validated just fine, only equality against
-        the [banned word
-        lists](https://github.com/theskumar/python-usernames/blob/master/usernames/reserved_words.py)
-        is checked. We don't try to be smart to avoid [Scunthorpe
-        problem](https://en.wikipedia.org/wiki/Scunthorpe_problem). If you can
-        come up with a algorithm/solution, please create an issue/pr :).
-        
-        License
-        -------
-        
-        MIT
-        
 Keywords: username,validation,registration,python,safe,signup
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
@@ -102,7 +20,89 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+python-usernames
+================
+
+[![Build
+Status](https://travis-ci.org/theskumar/python-usernames.svg?branch=v0.1.0)](https://travis-ci.org/theskumar/python-usernames)
+[![Coverage
+Status](https://coveralls.io/repos/theskumar/python-usernames/badge.svg?branch=master&service=github)](https://coveralls.io/github/theskumar/python-usernames?branch=master)
+[![PyPI
+version](https://badge.fury.io/py/python-usernames.svg)](http://badge.fury.io/py/python-usernames)
+
+Python library to validate usernames suitable for use in public facing
+applications where use can choose login names and sub-domains.
+
+Features
+--------
+
+-   Provides a default regex validator
+-   Validates against list of [banned
+    words](https://github.com/theskumar/python-usernames/blob/master/usernames/reserved_words.py)
+    that should not be used as username.
+-   Python 2.7, 3.4, 3.5, 3.6, 3.7, 3.8 & pypi
+
+Installation
+------------
+
+    pip install python-usernames
+
+Usages
+------
+
+``` {.sourceCode .python}
+from usernames import is_safe_username
+
+>>> is_safe_username("jerk")
+False  # contains one of the banned words
+
+>>> is_safe_username("handsome!")
+False  # contains non-url friendly `!`
+```
+
+**is\_safe\_username** takes the following optional arguments:
+
+-   `whitelist`: a case insensitive list of words that should be
+    considered as always safe. Default: `[]`
+-   `blacklist`: a case insensitive list of words that should be
+    considered as unsafe. Default: `[]`
+-   `max_length`: specify the maximun character a username can have.
+    Default: `None`
+
+- `regex`: regular expression string that must pass before the banned
+:   words is checked.
+
+The default regular expression is as follows:
+
+    ^                       # beginning of string
+    (?!_$)                  # no only _
+    (?![-.])                # no - or . at the beginning
+    (?!.*[_.-]{2})          # no __ or _. or ._ or .. or -- inside
+    [a-zA-Z0-9_.-]+         # allowed characters, atleast one must be present
+    (?<![.-])               # no - or . at the end
+    $                       # end of string
+
+**Further Reading**
+
+-   [Let’s talk about
+    usernames](https://www.b-list.org/weblog/2018/feb/11/usernames/)
+
+**Note:**
+
+Words like `bigcock12` will validated just fine, only equality against
+the [banned word
+lists](https://github.com/theskumar/python-usernames/blob/master/usernames/reserved_words.py)
+is checked. We don't try to be smart to avoid [Scunthorpe
+problem](https://en.wikipedia.org/wiki/Scunthorpe_problem). If you can
+come up with a algorithm/solution, please create an issue/pr :).
+
+License
+-------
+
+MIT
```

### Comparing `python-usernames-0.3.1/README.md` & `python-usernames-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `python-usernames-0.3.1/python_usernames.egg-info/PKG-INFO` & `python-usernames-0.4.1/python_usernames.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,98 +1,16 @@
 Metadata-Version: 2.1
 Name: python-usernames
-Version: 0.3.1
+Version: 0.4.1
 Summary: Python library to validate usernames suitable for use in public facing applications.
 Home-page: http://github.com/theskumar/python-usernames
 Author: Saurabh Kumar
 Author-email: me+github@saurabh-kumar.com
 License: MIT
-Description: python-usernames
-        ================
-        
-        [![Build
-        Status](https://travis-ci.org/theskumar/python-usernames.svg?branch=v0.1.0)](https://travis-ci.org/theskumar/python-usernames)
-        [![Coverage
-        Status](https://coveralls.io/repos/theskumar/python-usernames/badge.svg?branch=master&service=github)](https://coveralls.io/github/theskumar/python-usernames?branch=master)
-        [![PyPI
-        version](https://badge.fury.io/py/python-usernames.svg)](http://badge.fury.io/py/python-usernames)
-        
-        Python library to validate usernames suitable for use in public facing
-        applications where use can choose login names and sub-domains.
-        
-        Features
-        --------
-        
-        -   Provides a default regex validator
-        -   Validates against list of [banned
-            words](https://github.com/theskumar/python-usernames/blob/master/usernames/reserved_words.py)
-            that should not be used as username.
-        -   Python 2.7, 3.4, 3.5, 3.6, 3.7, 3.8 & pypi
-        
-        Installation
-        ------------
-        
-            pip install python-usernames
-        
-        Usages
-        ------
-        
-        ``` {.sourceCode .python}
-        from usernames import is_safe_username
-        
-        >>> is_safe_username("jerk")
-        False  # contains one of the banned words
-        
-        >>> is_safe_username("handsome!")
-        False  # contains non-url friendly `!`
-        ```
-        
-        **is\_safe\_username** takes the following optional arguments:
-        
-        -   `whitelist`: a case insensitive list of words that should be
-            considered as always safe. Default: `[]`
-        -   `blacklist`: a case insensitive list of words that should be
-            considered as unsafe. Default: `[]`
-        -   `max_length`: specify the maximun character a username can have.
-            Default: `None`
-        
-        - `regex`: regular expression string that must pass before the banned
-        :   words is checked.
-        
-        The default regular expression is as follows:
-        
-            ^                       # beginning of string
-            (?!_$)                  # no only _
-            (?![-.])                # no - or . at the beginning
-            (?!.*[_.-]{2})          # no __ or _. or ._ or .. or -- inside
-            [a-zA-Z0-9_.-]+         # allowed characters, atleast one must be present
-            (?<![.-])               # no - or . at the end
-            $                       # end of string
-        
-        **Further Reading**
-        
-        -   [Let’s talk about
-            usernames](https://www.b-list.org/weblog/2018/feb/11/usernames/)
-        
-        **Note:**
-        
-        Words like `bigcock12` will validated just fine, only equality against
-        the [banned word
-        lists](https://github.com/theskumar/python-usernames/blob/master/usernames/reserved_words.py)
-        is checked. We don't try to be smart to avoid [Scunthorpe
-        problem](https://en.wikipedia.org/wiki/Scunthorpe_problem). If you can
-        come up with a algorithm/solution, please create an issue/pr :).
-        
-        License
-        -------
-        
-        MIT
-        
 Keywords: username,validation,registration,python,safe,signup
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
@@ -102,7 +20,89 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+python-usernames
+================
+
+[![Build
+Status](https://travis-ci.org/theskumar/python-usernames.svg?branch=v0.1.0)](https://travis-ci.org/theskumar/python-usernames)
+[![Coverage
+Status](https://coveralls.io/repos/theskumar/python-usernames/badge.svg?branch=master&service=github)](https://coveralls.io/github/theskumar/python-usernames?branch=master)
+[![PyPI
+version](https://badge.fury.io/py/python-usernames.svg)](http://badge.fury.io/py/python-usernames)
+
+Python library to validate usernames suitable for use in public facing
+applications where use can choose login names and sub-domains.
+
+Features
+--------
+
+-   Provides a default regex validator
+-   Validates against list of [banned
+    words](https://github.com/theskumar/python-usernames/blob/master/usernames/reserved_words.py)
+    that should not be used as username.
+-   Python 2.7, 3.4, 3.5, 3.6, 3.7, 3.8 & pypi
+
+Installation
+------------
+
+    pip install python-usernames
+
+Usages
+------
+
+``` {.sourceCode .python}
+from usernames import is_safe_username
+
+>>> is_safe_username("jerk")
+False  # contains one of the banned words
+
+>>> is_safe_username("handsome!")
+False  # contains non-url friendly `!`
+```
+
+**is\_safe\_username** takes the following optional arguments:
+
+-   `whitelist`: a case insensitive list of words that should be
+    considered as always safe. Default: `[]`
+-   `blacklist`: a case insensitive list of words that should be
+    considered as unsafe. Default: `[]`
+-   `max_length`: specify the maximun character a username can have.
+    Default: `None`
+
+- `regex`: regular expression string that must pass before the banned
+:   words is checked.
+
+The default regular expression is as follows:
+
+    ^                       # beginning of string
+    (?!_$)                  # no only _
+    (?![-.])                # no - or . at the beginning
+    (?!.*[_.-]{2})          # no __ or _. or ._ or .. or -- inside
+    [a-zA-Z0-9_.-]+         # allowed characters, atleast one must be present
+    (?<![.-])               # no - or . at the end
+    $                       # end of string
+
+**Further Reading**
+
+-   [Let’s talk about
+    usernames](https://www.b-list.org/weblog/2018/feb/11/usernames/)
+
+**Note:**
+
+Words like `bigcock12` will validated just fine, only equality against
+the [banned word
+lists](https://github.com/theskumar/python-usernames/blob/master/usernames/reserved_words.py)
+is checked. We don't try to be smart to avoid [Scunthorpe
+problem](https://en.wikipedia.org/wiki/Scunthorpe_problem). If you can
+come up with a algorithm/solution, please create an issue/pr :).
+
+License
+-------
+
+MIT
```

### Comparing `python-usernames-0.3.1/setup.py` & `python-usernames-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     readme = readme_file.read()
 
 setup(
     name="python-usernames",
     description="Python library to validate usernames suitable for use in public facing applications.",
     long_description=readme,
     long_description_content_type="text/markdown",
-    version="0.3.1",
+    version="0.4.1",
     author="Saurabh Kumar",
     author_email="me+github@saurabh-kumar.com",
     url="http://github.com/theskumar/python-usernames",
 
     packages=[
         str('usernames'),
     ],
@@ -54,17 +54,17 @@
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         # 'Topic :: System :: Systems Administration',
         'Topic :: Utilities',
         # 'Environment :: Web Environment',
         # 'Framework :: Django',
     ],
-    keywords=(
+    keywords=[
         'username', 'validation', 'registration', 'python', 'safe', 'signup'
-    ),
+    ],
 )
 
 # (*) Please direct queries to the discussion group, rather than to me directly
 #     Doing so helps ensure your question is helpful to other users.
 #     Queries directly to my email are likely to receive a canned response.
 #
 #     Many thanks for your understanding.
```

### Comparing `python-usernames-0.3.1/usernames/reserved_words.py` & `python-usernames-0.4.1/usernames/reserved_words.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,34 +19,38 @@
 accounts
 add
 address
 adm
 admin
 administration
 administrator
+ads
 adult
 advertising
 affiliate
 affiliates
 ajax
 anal
 analytics
 android
 anon
 anonymous
 anus
+apache
 api
 app
 apps
 archive
 arse
 ass
 atom
+audio
 auth
 authentication
+authority
 autoconfig
 avatar
 backup
 balls
 ballsack
 banner
 banners
@@ -68,53 +72,62 @@
 bots
 broadcasthost
 bugger
 bum
 business
 butt
 buttplug
+ca
 cache
 cadastro
 calendar
 campaign
 careers
+ceo
+cert
 cgi
 chat
 client
 cliente
 clitoris
 cock
 code
 comercial
+commerce
 compare
 compras
 config
 connect
+console
 contact
 contest
 coon
 copyright
 crap
 create
+crt
 css
 cunt
+daemon
 damn
 dashboard
 data
 db
 delete
 demo
 design
 designer
 dev
 devel
+devs
 dick
 dildo
 dir
 directory
+dns
 doc
 docs
 domain
 download
 downloads
 dyke
 ecommerce
@@ -133,14 +146,15 @@
 feed
 feedback
 felching
 fellate
 fellatio
 file
 files
+firewall
 flange
 flog
 follow
 forum
 forums
 free
 ftp
@@ -164,14 +178,15 @@
 homepage
 homo
 host
 hosting
 hostmaster
 hostname
 hpg
+hr
 html
 http
 httpd
 https
 image
 images
 imap
@@ -181,14 +196,16 @@
 info
 information
 inquiry
 intranet
 intro
 introduction
 invite
+invoice
+invoices
 ipad
 iphone
 irc
 is
 isatap
 it
 java
@@ -198,18 +215,22 @@
 job
 jobs
 js
 knob
 knobend
 knowledgebase
 labia
+licence
+license
 licensing
 links
 list
+list-request
 lists
+live
 lmao
 lmfao
 localdomain
 localhost
 log
 login
 logout
@@ -220,27 +241,32 @@
 mail2
 mail3
 mail4
 mail5
 mailer
 mailer-daemon
 mailing
+maintainer
 manager
 marketing
 master
 me
 media
 message
 messenger
 microblog
 microblogs
 mine
 mis
 mob
 mobile
+mod
+moderator
+moderators
+mods
 motherfucker
 movie
 movies
 mp3
 msg
 msn
 muff
@@ -252,14 +278,15 @@
 name
 named
 net
 network
 new
 news
 newsletter
+nginx
 nick
 nickname
 nigga
 nigger
 no-reply
 nobody
 noc
@@ -267,26 +294,32 @@
 notes
 noticias
 ns
 ns1
 ns2
 ns3
 ns4
+ntp
+null
 old
 omg
 online
 operator
+operators
 order
 orders
 packer
 page
 pager
 pages
 panel
+passwd
 password
+pay
+payment
 payments
 penis
 perl
 photo
 photoalbum
 photos
 php
@@ -300,28 +333,34 @@
 poop
 pop
 pop3
 post
 postfix
 postmaster
 posts
+pr
 pricing
 prick
+printer
 privacy
 profile
 project
 projects
 promo
+promotion
+proxy
 pub
 pube
 public
+purchase
 pussy
 python
 queer
 random
+redir
 refund
 refunds
 register
 registration
 return
 returns
 reviews
@@ -335,14 +374,15 @@
 script
 scripts
 scrotum
 search
 secure
 security
 send
+sendmail
 service
 services
 setting
 settings
 setup
 sex
 sh1t
@@ -355,41 +395,51 @@
 sites
 slut
 smegma
 smtp
 soporte
 spunk
 sql
+squid
 ssh
+ssl
 ssladmin
 ssladministrator
 sslwebmaster
 stage
 staging
 start
 stat
 static
 stats
 status
 store
 stores
+stream
 subdomain
 subscribe
+sudo
+superuser
 suporte
 support
 survey
+sync
+sys
 sysadmin
+syslog
+sysop
 system
 tablet
 tablets
 talk
 task
 tasks
 tech
 telnet
+terminal
 terms
 test
 test1
 test2
 test3
 teste
 testimonials
@@ -407,14 +457,15 @@
 twat
 update
 upload
 url
 usage
 usenet
 user
+userdb
 username
 users
 usuario
 uucp
 vagina
 vendas
 video
@@ -422,14 +473,15 @@
 visitor
 wank
 web
 webmail
 webmaster
 website
 websites
+wheel
 whore
 win
 workshop
 wpad
 wtf
 ww
 wws
@@ -449,12 +501,13 @@
 yourdomain
 yourname
 yoursite
 yourusername
 """
 
 
+
 def get_reserved_wordlist():
     return set(_d.splitlines())
 
 
 __all__ = ["get_reserved_wordlist"]
```

### Comparing `python-usernames-0.3.1/usernames/validators.py` & `python-usernames-0.4.1/usernames/validators.py`

 * *Files identical despite different names*

