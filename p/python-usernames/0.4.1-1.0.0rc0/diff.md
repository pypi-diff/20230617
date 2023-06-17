# Comparing `tmp/python-usernames-0.4.1.tar.gz` & `tmp/python_usernames-1.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-usernames-0.4.1.tar", last modified: Sat Jun 17 08:43:02 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `python-usernames-0.4.1.tar` & `python_usernames-1.0.0rc0.tar`

### file list

```diff
@@ -1,17 +1,9 @@
-drwxr-xr-x   0 theskumar   (501) staff       (20)        0 2023-06-17 08:43:02.239773 python-usernames-0.4.1/
--rw-r--r--   0 theskumar   (501) staff       (20)     1081 2023-06-17 08:04:29.000000 python-usernames-0.4.1/LICENSE
--rw-r--r--   0 theskumar   (501) staff       (20)       27 2023-06-17 08:04:29.000000 python-usernames-0.4.1/MANIFEST.in
--rw-r--r--   0 theskumar   (501) staff       (20)     3771 2023-06-17 08:43:02.239852 python-usernames-0.4.1/PKG-INFO
--rw-r--r--   0 theskumar   (501) staff       (20)     2595 2023-06-17 08:31:45.000000 python-usernames-0.4.1/README.md
-drwxr-xr-x   0 theskumar   (501) staff       (20)        0 2023-06-17 08:43:02.239304 python-usernames-0.4.1/python_usernames.egg-info/
--rw-r--r--   0 theskumar   (501) staff       (20)     3771 2023-06-17 08:43:02.000000 python-usernames-0.4.1/python_usernames.egg-info/PKG-INFO
--rw-r--r--   0 theskumar   (501) staff       (20)      321 2023-06-17 08:43:02.000000 python-usernames-0.4.1/python_usernames.egg-info/SOURCES.txt
--rw-r--r--   0 theskumar   (501) staff       (20)        1 2023-06-17 08:43:02.000000 python-usernames-0.4.1/python_usernames.egg-info/dependency_links.txt
--rw-r--r--   0 theskumar   (501) staff       (20)        1 2023-06-17 08:43:02.000000 python-usernames-0.4.1/python_usernames.egg-info/not-zip-safe
--rw-r--r--   0 theskumar   (501) staff       (20)       10 2023-06-17 08:43:02.000000 python-usernames-0.4.1/python_usernames.egg-info/top_level.txt
--rw-r--r--   0 theskumar   (501) staff       (20)      234 2023-06-17 08:43:02.240094 python-usernames-0.4.1/setup.cfg
--rw-r--r--   0 theskumar   (501) staff       (20)     2699 2023-06-17 08:35:55.000000 python-usernames-0.4.1/setup.py
-drwxr-xr-x   0 theskumar   (501) staff       (20)        0 2023-06-17 08:43:02.239660 python-usernames-0.4.1/usernames/
--rw-r--r--   0 theskumar   (501) staff       (20)       97 2023-06-17 08:31:45.000000 python-usernames-0.4.1/usernames/__init__.py
--rw-r--r--   0 theskumar   (501) staff       (20)     3835 2023-06-17 08:31:45.000000 python-usernames-0.4.1/usernames/reserved_words.py
--rw-r--r--   0 theskumar   (501) staff       (20)     1170 2023-06-17 08:31:45.000000 python-usernames-0.4.1/usernames/validators.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 python_usernames-1.0.0rc0/src/python_usernames/__about__.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 python_usernames-1.0.0rc0/src/python_usernames/__init__.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 python_usernames-1.0.0rc0/src/python_usernames/reserved_words.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 python_usernames-1.0.0rc0/src/python_usernames/validators.py
+-rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 python_usernames-1.0.0rc0/src/python_usernames/words.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 python_usernames-1.0.0rc0/.gitignore
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 python_usernames-1.0.0rc0/README.md
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 python_usernames-1.0.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 python_usernames-1.0.0rc0/PKG-INFO
```

### Comparing `python-usernames-0.4.1/PKG-INFO` & `python_usernames-1.0.0rc0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,61 @@
 Metadata-Version: 2.1
 Name: python-usernames
-Version: 0.4.1
+Version: 1.0.0rc0
 Summary: Python library to validate usernames suitable for use in public facing applications.
-Home-page: http://github.com/theskumar/python-usernames
-Author: Saurabh Kumar
-Author-email: me+github@saurabh-kumar.com
-License: MIT
-Keywords: username,validation,registration,python,safe,signup
-Classifier: Development Status :: 1 - Planning
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Project-URL: Documentation, https://github.com/theskumar/python-usernames/tree/main#readme
+Project-URL: Source, https://github.com/theskumar/python-usernames
+Project-URL: Tracker, https://github.com/theskumar/python-usernames/issues
+Author-email: Saurabh Kumar <python-usernames@saurabh-kumar.com>
+License-Expression: MIT
+Keywords: regex,safe,security,signup,user registration,username,validation
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Security
 Classifier: Topic :: Utilities
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
-python-usernames
-================
+# python-usernames
 
 [![Build
 Status](https://travis-ci.org/theskumar/python-usernames.svg?branch=v0.1.0)](https://travis-ci.org/theskumar/python-usernames)
 [![Coverage
 Status](https://coveralls.io/repos/theskumar/python-usernames/badge.svg?branch=master&service=github)](https://coveralls.io/github/theskumar/python-usernames?branch=master)
 [![PyPI
 version](https://badge.fury.io/py/python-usernames.svg)](http://badge.fury.io/py/python-usernames)
 
 Python library to validate usernames suitable for use in public facing
 applications where use can choose login names and sub-domains.
 
-Features
---------
+## Features
 
 -   Provides a default regex validator
 -   Validates against list of [banned
     words](https://github.com/theskumar/python-usernames/blob/master/usernames/reserved_words.py)
     that should not be used as username.
--   Python 2.7, 3.4, 3.5, 3.6, 3.7, 3.8 & pypi
+-   Python 3.8+
 
-Installation
-------------
+## Installation
 
     pip install python-usernames
 
-Usages
-------
+## Usages
 
-``` {.sourceCode .python}
-from usernames import is_safe_username
+```python
+from python_usernames import is_safe_username
 
 >>> is_safe_username("jerk")
 False  # contains one of the banned words
 
 >>> is_safe_username("handsome!")
 False  # contains non-url friendly `!`
 ```
@@ -84,25 +78,24 @@
     (?!_$)                  # no only _
     (?![-.])                # no - or . at the beginning
     (?!.*[_.-]{2})          # no __ or _. or ._ or .. or -- inside
     [a-zA-Z0-9_.-]+         # allowed characters, atleast one must be present
     (?<![.-])               # no - or . at the end
     $                       # end of string
 
-**Further Reading**
+## Further Reading
 
 -   [Let’s talk about
     usernames](https://www.b-list.org/weblog/2018/feb/11/usernames/)
 
-**Note:**
+## Gotchas
 
 Words like `bigcock12` will validated just fine, only equality against
 the [banned word
 lists](https://github.com/theskumar/python-usernames/blob/master/usernames/reserved_words.py)
 is checked. We don't try to be smart to avoid [Scunthorpe
 problem](https://en.wikipedia.org/wiki/Scunthorpe_problem). If you can
 come up with a algorithm/solution, please create an issue/pr :).
 
-License
--------
+## License
 
 MIT
```

### Comparing `python-usernames-0.4.1/README.md` & `python_usernames-1.0.0rc0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,35 @@
-python-usernames
-================
+# python-usernames
 
 [![Build
 Status](https://travis-ci.org/theskumar/python-usernames.svg?branch=v0.1.0)](https://travis-ci.org/theskumar/python-usernames)
 [![Coverage
 Status](https://coveralls.io/repos/theskumar/python-usernames/badge.svg?branch=master&service=github)](https://coveralls.io/github/theskumar/python-usernames?branch=master)
 [![PyPI
 version](https://badge.fury.io/py/python-usernames.svg)](http://badge.fury.io/py/python-usernames)
 
 Python library to validate usernames suitable for use in public facing
 applications where use can choose login names and sub-domains.
 
-Features
---------
+## Features
 
 -   Provides a default regex validator
 -   Validates against list of [banned
     words](https://github.com/theskumar/python-usernames/blob/master/usernames/reserved_words.py)
     that should not be used as username.
--   Python 2.7, 3.4, 3.5, 3.6, 3.7, 3.8 & pypi
+-   Python 3.8+
 
-Installation
-------------
+## Installation
 
     pip install python-usernames
 
-Usages
-------
+## Usages
 
-``` {.sourceCode .python}
-from usernames import is_safe_username
+```python
+from python_usernames import is_safe_username
 
 >>> is_safe_username("jerk")
 False  # contains one of the banned words
 
 >>> is_safe_username("handsome!")
 False  # contains non-url friendly `!`
 ```
@@ -56,25 +52,24 @@
     (?!_$)                  # no only _
     (?![-.])                # no - or . at the beginning
     (?!.*[_.-]{2})          # no __ or _. or ._ or .. or -- inside
     [a-zA-Z0-9_.-]+         # allowed characters, atleast one must be present
     (?<![.-])               # no - or . at the end
     $                       # end of string
 
-**Further Reading**
+## Further Reading
 
 -   [Let’s talk about
     usernames](https://www.b-list.org/weblog/2018/feb/11/usernames/)
 
-**Note:**
+## Gotchas
 
 Words like `bigcock12` will validated just fine, only equality against
 the [banned word
 lists](https://github.com/theskumar/python-usernames/blob/master/usernames/reserved_words.py)
 is checked. We don't try to be smart to avoid [Scunthorpe
 problem](https://en.wikipedia.org/wiki/Scunthorpe_problem). If you can
 come up with a algorithm/solution, please create an issue/pr :).
 
-License
--------
+## License
 
 MIT
```

### Comparing `python-usernames-0.4.1/usernames/reserved_words.py` & `python_usernames-1.0.0rc0/src/python_usernames/words.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-# -*- coding: utf-8 -*-
-from __future__ import unicode_literals
-
-"""
-List of reserved usernames (pre-defined list of special banned and reserved keywords in names,
-such as "root", "www", "admin"). Useful when creating public systems, where users can choose
-a login name or a sub-domain name.
-__References:__
-1. http://www.bannedwordlist.com/
-2. http://blog.postbit.com/reserved-username-list.html
-3. https://ldpreload.com/blog/names-to-reserve
-"""
-
-_d = """
 about
 abuse
 access
 account
 accounts
 add
 address
@@ -48,21 +34,23 @@
 authentication
 authority
 autoconfig
 avatar
 backup
 balls
 ballsack
+banned
 banner
 banners
 bastard
 biatch
 billing
 bin
 bitch
+blocked
 blog
 blogs
 bloody
 blowjob
 board
 bollock
 bollok
@@ -134,14 +122,15 @@
 edit
 editor
 email
 end
 errors
 events
 example
+exploit
 fag
 faq
 faqs
 favorite
 feck
 feed
 feedback
@@ -168,14 +157,15 @@
 god
 goddamn
 group
 groups
 guarantee
 guest
 guests
+hacker
 hell
 help
 home
 homepage
 homo
 host
 hosting
@@ -183,14 +173,15 @@
 hostname
 hpg
 hr
 html
 http
 httpd
 https
+illegal
 image
 images
 imap
 img
 index
 indice
 info
@@ -284,26 +275,28 @@
 newsletter
 nginx
 nick
 nickname
 nigga
 nigger
 no-reply
+noaccess
 nobody
 noc
 noreply
 notes
 noticias
 ns
 ns1
 ns2
 ns3
 ns4
 ntp
 null
+offensive
 old
 omg
 online
 operator
 operators
 order
 orders
@@ -351,14 +344,15 @@
 pub
 pube
 public
 purchase
 pussy
 python
 queer
+qwerty
 random
 redir
 refund
 refunds
 register
 registration
 return
@@ -367,14 +361,15 @@
 root
 rss
 ruby
 sale
 sales
 sample
 samples
+scammer
 script
 scripts
 scrotum
 search
 secure
 security
 send
@@ -393,14 +388,15 @@
 site
 sitemap
 sites
 slut
 smegma
 smtp
 soporte
+spammer
 spunk
 sql
 squid
 ssh
 ssl
 ssladmin
 ssladministrator
@@ -418,14 +414,15 @@
 subdomain
 subscribe
 sudo
 superuser
 suporte
 support
 survey
+suspended
 sync
 sys
 sysadmin
 syslog
 sysop
 system
 tablet
@@ -440,14 +437,15 @@
 test
 test1
 test2
 test3
 teste
 testimonials
 tests
+testuser
 theme
 themes
 tit
 tmp
 todo
 tools
 tosser
@@ -467,14 +465,15 @@
 usuario
 uucp
 vagina
 vendas
 video
 videos
 visitor
+vulgarity
 wank
 web
 webmail
 webmaster
 website
 websites
 wheel
@@ -498,16 +497,7 @@
 xpg
 xxx
 you
 yourdomain
 yourname
 yoursite
 yourusername
-"""
-
-
-
-def get_reserved_wordlist():
-    return set(_d.splitlines())
-
-
-__all__ = ["get_reserved_wordlist"]
```

