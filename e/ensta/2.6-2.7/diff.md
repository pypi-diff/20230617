# Comparing `tmp/ensta-2.6.tar.gz` & `tmp/ensta-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensta-2.6.tar", last modified: Sat Jun 17 09:36:53 2023, max compression
+gzip compressed data, was "ensta-2.7.tar", last modified: Sat Jun 17 10:14:03 2023, max compression
```

## Comparing `ensta-2.6.tar` & `ensta-2.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 09:36:53.806376 ensta-2.6/
--rw-rw-rw-   0        0        0     1081 2023-06-06 15:38:39.000000 ensta-2.6/LICENSE.txt
--rw-rw-rw-   0        0        0     5716 2023-06-17 09:36:53.806376 ensta-2.6/PKG-INFO
--rw-rw-rw-   0        0        0     4710 2023-06-15 06:34:08.000000 ensta-2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 09:36:53.723050 ensta-2.6/ensta/
--rw-rw-rw-   0        0        0     2566 2023-06-15 10:21:57.000000 ensta-2.6/ensta/Authentication.py
--rw-rw-rw-   0        0        0     9955 2023-06-15 13:55:13.000000 ensta-2.6/ensta/Guest.py
--rw-rw-rw-   0        0        0    30175 2023-06-16 16:47:35.000000 ensta-2.6/ensta/Host.py
--rw-rw-rw-   0        0        0      136 2023-06-17 09:26:48.000000 ensta-2.6/ensta/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 09:36:53.771389 ensta-2.6/ensta/containers/
--rw-rw-rw-   0        0        0      420 2023-06-15 10:26:52.000000 ensta-2.6/ensta/containers/FollowPerson.py
--rw-rw-rw-   0        0        0      222 2023-06-09 08:46:48.000000 ensta-2.6/ensta/containers/FollowedStatus.py
--rw-rw-rw-   0        0        0     3702 2023-06-16 16:54:33.000000 ensta-2.6/ensta/containers/Post.py
--rw-rw-rw-   0        0        0      703 2023-06-16 15:13:40.000000 ensta-2.6/ensta/containers/PostUser.py
--rw-rw-rw-   0        0        0     1074 2023-06-15 13:41:12.000000 ensta-2.6/ensta/containers/Profile.py
--rw-rw-rw-   0        0        0      467 2023-06-15 13:54:39.000000 ensta-2.6/ensta/containers/ProfileHost.py
--rw-rw-rw-   0        0        0      153 2023-06-09 08:28:13.000000 ensta-2.6/ensta/containers/UnfollowedStatus.py
--rw-rw-rw-   0        0        0      256 2023-06-16 12:04:09.000000 ensta-2.6/ensta/containers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 09:36:53.797029 ensta-2.6/ensta/lib/
--rw-rw-rw-   0        0        0     2776 2023-06-16 09:56:28.000000 ensta-2.6/ensta/lib/Commons.py
--rw-rw-rw-   0        0        0     1008 2023-06-15 09:37:02.000000 ensta-2.6/ensta/lib/Exceptions.py
--rw-rw-rw-   0        0        0      360 2023-06-15 09:37:20.000000 ensta-2.6/ensta/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 09:36:53.747084 ensta-2.6/ensta.egg-info/
--rw-rw-rw-   0        0        0     5716 2023-06-17 09:36:53.000000 ensta-2.6/ensta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      570 2023-06-17 09:36:53.000000 ensta-2.6/ensta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 09:36:53.000000 ensta-2.6/ensta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-17 09:36:53.000000 ensta-2.6/ensta.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-17 09:36:53.000000 ensta-2.6/ensta.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-17 09:36:53.810031 ensta-2.6/setup.cfg
--rw-rw-rw-   0        0        0     1402 2023-06-17 09:35:02.000000 ensta-2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:14:03.922889 ensta-2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-17 10:13:54.000000 ensta-2.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-06-17 10:14:03.922889 ensta-2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-06-17 10:13:54.000000 ensta-2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:14:03.922889 ensta-2.7/ensta/
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-17 10:13:54.000000 ensta-2.7/ensta/Authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-06-17 10:13:54.000000 ensta-2.7/ensta/Guest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29495 2023-06-17 10:13:54.000000 ensta-2.7/ensta/Host.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-17 10:13:54.000000 ensta-2.7/ensta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:14:03.922889 ensta-2.7/ensta/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-17 10:13:54.000000 ensta-2.7/ensta/containers/FollowPerson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-17 10:13:54.000000 ensta-2.7/ensta/containers/FollowedStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-06-17 10:13:54.000000 ensta-2.7/ensta/containers/Post.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-17 10:13:54.000000 ensta-2.7/ensta/containers/PostUser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-17 10:13:54.000000 ensta-2.7/ensta/containers/Profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-17 10:13:54.000000 ensta-2.7/ensta/containers/ProfileHost.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-17 10:13:54.000000 ensta-2.7/ensta/containers/UnfollowedStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-17 10:13:54.000000 ensta-2.7/ensta/containers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:14:03.922889 ensta-2.7/ensta/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-17 10:13:54.000000 ensta-2.7/ensta/lib/Commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-17 10:13:54.000000 ensta-2.7/ensta/lib/Exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-17 10:13:54.000000 ensta-2.7/ensta/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:14:03.922889 ensta-2.7/ensta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-06-17 10:14:03.000000 ensta-2.7/ensta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-17 10:14:03.000000 ensta-2.7/ensta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 10:14:03.000000 ensta-2.7/ensta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-17 10:14:03.000000 ensta-2.7/ensta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-17 10:14:03.000000 ensta-2.7/ensta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-17 10:14:03.922889 ensta-2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-17 10:13:54.000000 ensta-2.7/setup.py
```

### Comparing `ensta-2.6/LICENSE.txt` & `ensta-2.7/LICENSE.txt`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Ensta
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2023 Ensta
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `ensta-2.6/PKG-INFO` & `ensta-2.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-Metadata-Version: 2.1
-Name: ensta
-Version: 2.6
-Summary: 🔥 Fastest & Simplest Python Package For Instagram Automation
-Home-page: https://github.com/diezo/ensta
-Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v2.6.tar.gz
-Author: Deepak Soni
-Author-email: lonelycube@proton.me
-License: MIT
-Keywords: instagram-client,instagram,api-wrapper,instagram-scraper,instagram-api,instagram-sdk,instagram-photos,instagram-api-python,instabot,instagram-stories,instagram-bot,instapy,instagram-downloader,instagram-account,instagram-crawler,instagram-private-api,igtv,instagram-automation,reels,instagram-feed
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# 🤖 Ensta - Simple Instagram API
-[![PyPI](https://img.shields.io/pypi/v/ensta)](https://pypi.org/project/ensta)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ensta)]()
-[![Downloads](https://static.pepy.tech/badge/ensta)](https://pepy.tech/project/ensta)
-[![Twitter Share](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)](https://twitter.com/intent/tweet?text=Wow:&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)
-
-<img style="border-radius: 10px" src="https://imgtr.ee/images/2023/06/14/Twfd4.png"/>
-
-This package lets you use Instagram's Internal Web API through simple functions and classes. Ensta uses Instagram's Original Web API to scrape data which makes it a reliable choice over other third-party scrapers. This library mainly focuses on Simplicity & Reliability.
-
-Two type of classes are supported - ***Guest & Host***.
-
-[<img style="margin-top: 10px" src="https://www.buymeacoffee.com/assets/img/guidelines/download-assets-sm-1.svg" width="160"/>](https://buymeacoffee.com/diezo)
-
-## 📢 Announcement
-Users can now log in through their **Username** and **Password** to generate SessionId! [See this](https://github.com/diezo/ensta#:~:text=NewSessionID(%22username%22%2C%20%22password%22))
-
-## Installation
-To install this package using [Python's PIP](https://pypi.org/project/pip/), run this command in a terminal window:
-```shell
-$ pip install ensta
-```
-
-To update the existing package, run:
-```shell
-$ pip install ensta --upgrade
-```
-
-## 🧔🏻‍♂️ Guest Mode
-This mode doesn't require login and can be used to fetch publicly available data from Instagram's Servers. Following methods are supported till now:
-- Check if username is available for registration
-- Fetch someone's profile data
-- Convert username to userid
-- Convert userid to username
-
-Here's an example where an instance of *Guest Class* is created to fetch [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) profile information:
-
-```python
-from ensta import Guest
-
-guest = Guest()
-profile = guest.profile("cristiano")
-
-if profile is None:
-    print("Something went wrong.")
-else:
-    print(profile.biography)
-    print(profile.follower_count)
-    print(profile.following_count)
-```
-
-## 🧔🏻‍♂️ Host Mode
-Host mode requires login through SessionID, which should be passed as an argument during initialization.
-It can be used to take actions that require login. Additionally, users can manage their own profile through this class.
-
-These are the methods supported till now:
-- Check authentication status of the user
-- Follow/unfollow users
-- Fetch someone's follower/following list
-- Switch account type - 'Public' or 'Private'
-
-Here's an example where an instance of *Host Class* is created to follow [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) account:
-
-```python
-from ensta import Host, NewSessionID
-
-sessionid = NewSessionID("username", "password")
-
-host = Host(sessionid)
-status = host.follow("cristiano")
-
-if status is None:
-    print("Something went wrong.")
-else:
-    if status.following:
-        print("Following!")
-    
-    elif status.follow_requested:
-        print("Requested to follow!")
-```
-
-> ### **Note:**
-> When you create a new sessionid through *NewSessionID()*, it's recommended to save it somewhere, and use the same sessionid (instead of creating a new one each time you need) until it expires or becomes invalid.
->
-> This should be done to avoid unnecessary prolonged wait time while generating a new sessionid and also to prevent getting your account from getting flagged because of repetitive logins.
-
-## 📋 Remember
-Every function should return **None** on failure. So, it's recommended to add an *if statement* before using the actual data to avoid TypeErrors. Here's an example:
-```python
-from ensta import Guest
-
-guest = Guest()
-available = guest.username_availability("cristiano")
-
-if available is None:  # 'None' indicates failure
-    print("Something went wrong.")
-else:
-    print(available)
-```
-
-## ❤️ Donate
-If you wish to help me in the development of Ensta, consider donating:
-
-[<img src="https://www.buymeacoffee.com/assets/img/guidelines/download-assets-sm-1.svg" width="150"/>](https://buymeacoffee.com/diezo)
-
-## Disclaimer
-This is a third-party package, and not approved by Instagram. It doesn't promote illegal activities or activities that violate [Instagram's Community Guidelines](https://help.instagram.com/477434105621119/) such as spamming users, creating bot accounts, misusing data etc. You are solely responsible for all the actions you take using this package.
+Metadata-Version: 2.1
+Name: ensta
+Version: 2.7
+Summary: 🔥 Fastest & Simplest Python Package For Instagram Automation
+Home-page: https://github.com/diezo/ensta
+Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v2.7.tar.gz
+Author: Deepak Soni
+Author-email: lonelycube@proton.me
+License: MIT
+Keywords: instagram-client,instagram,api-wrapper,instagram-scraper,instagram-api,instagram-sdk,instagram-photos,instagram-api-python,instabot,instagram-stories,instagram-bot,instapy,instagram-downloader,instagram-account,instagram-crawler,instagram-private-api,igtv,instagram-automation,reels,instagram-feed
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# 🤖 Ensta - Simple Instagram API
+[![PyPI](https://img.shields.io/pypi/v/ensta)](https://pypi.org/project/ensta)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ensta)]()
+[![Downloads](https://static.pepy.tech/badge/ensta)](https://pepy.tech/project/ensta)
+[![Twitter Share](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)](https://twitter.com/intent/tweet?text=Wow:&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)
+
+<img style="border-radius: 10px" src="https://imgtr.ee/images/2023/06/14/Twfd4.png"/>
+
+This package lets you use Instagram's Internal Web API through simple functions and classes. Ensta uses Instagram's Original Web API to scrape data which makes it a reliable choice over other third-party scrapers. This library mainly focuses on Simplicity & Reliability.
+
+Two type of classes are supported - ***Guest & Host***.
+
+[<img style="margin-top: 10px" src="https://www.buymeacoffee.com/assets/img/guidelines/download-assets-sm-1.svg" width="160"/>](https://buymeacoffee.com/diezo)
+
+## 📢 Announcement
+Users can now log in through their **Username** and **Password** to generate SessionId! [See this](https://github.com/diezo/ensta#:~:text=NewSessionID(%22username%22%2C%20%22password%22))
+
+## Installation
+To install this package using [Python's PIP](https://pypi.org/project/pip/), run this command in a terminal window:
+```shell
+$ pip install ensta
+```
+
+To update the existing package, run:
+```shell
+$ pip install ensta --upgrade
+```
+
+## 🧔🏻‍♂️ Guest Mode
+This mode doesn't require login and can be used to fetch publicly available data from Instagram's Servers. Following methods are supported till now:
+- Check if username is available for registration
+- Fetch someone's profile data
+- Convert username to userid
+- Convert userid to username
+
+Here's an example where an instance of *Guest Class* is created to fetch [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) profile information:
+
+```python
+from ensta import Guest
+
+guest = Guest()
+profile = guest.profile("cristiano")
+
+if profile is None:
+    print("Something went wrong.")
+else:
+    print(profile.biography)
+    print(profile.follower_count)
+    print(profile.following_count)
+```
+
+## 🧔🏻‍♂️ Host Mode
+Host mode requires login through SessionID, which should be passed as an argument during initialization.
+It can be used to take actions that require login. Additionally, users can manage their own profile through this class.
+
+These are the methods supported till now:
+- Check authentication status of the user
+- Follow/unfollow users
+- Fetch someone's follower/following list
+- Switch account type - 'Public' or 'Private'
+
+Here's an example where an instance of *Host Class* is created to follow [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) account:
+
+```python
+from ensta import Host, NewSessionID
+
+sessionid = NewSessionID("username", "password")
+
+host = Host(sessionid)
+status = host.follow("cristiano")
+
+if status is None:
+    print("Something went wrong.")
+else:
+    if status.following:
+        print("Following!")
+    
+    elif status.follow_requested:
+        print("Requested to follow!")
+```
+
+> ### **Note:**
+> When you create a new sessionid through *NewSessionID()*, it's recommended to save it somewhere, and use the same sessionid (instead of creating a new one each time you need) until it expires or becomes invalid.
+>
+> This should be done to avoid unnecessary prolonged wait time while generating a new sessionid and also to prevent getting your account from getting flagged because of repetitive logins.
+
+## 📋 Remember
+Every function should return **None** on failure. So, it's recommended to add an *if statement* before using the actual data to avoid TypeErrors. Here's an example:
+```python
+from ensta import Guest
+
+guest = Guest()
+available = guest.username_availability("cristiano")
+
+if available is None:  # 'None' indicates failure
+    print("Something went wrong.")
+else:
+    print(available)
+```
+
+## ❤️ Donate
+If you wish to help me in the development of Ensta, consider donating:
+
+[<img src="https://www.buymeacoffee.com/assets/img/guidelines/download-assets-sm-1.svg" width="150"/>](https://buymeacoffee.com/diezo)
+
+## Disclaimer
+This is a third-party package, and not approved by Instagram. It doesn't promote illegal activities or activities that violate [Instagram's Community Guidelines](https://help.instagram.com/477434105621119/) such as spamming users, creating bot accounts, misusing data etc. You are solely responsible for all the actions you take using this package.
```

### Comparing `ensta-2.6/README.md` & `ensta-2.7/README.md`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-# 🤖 Ensta - Simple Instagram API
-[![PyPI](https://img.shields.io/pypi/v/ensta)](https://pypi.org/project/ensta)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ensta)]()
-[![Downloads](https://static.pepy.tech/badge/ensta)](https://pepy.tech/project/ensta)
-[![Twitter Share](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)](https://twitter.com/intent/tweet?text=Wow:&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)
-
-<img style="border-radius: 10px" src="https://imgtr.ee/images/2023/06/14/Twfd4.png"/>
-
-This package lets you use Instagram's Internal Web API through simple functions and classes. Ensta uses Instagram's Original Web API to scrape data which makes it a reliable choice over other third-party scrapers. This library mainly focuses on Simplicity & Reliability.
-
-Two type of classes are supported - ***Guest & Host***.
-
-[<img style="margin-top: 10px" src="https://www.buymeacoffee.com/assets/img/guidelines/download-assets-sm-1.svg" width="160"/>](https://buymeacoffee.com/diezo)
-
-## 📢 Announcement
-Users can now log in through their **Username** and **Password** to generate SessionId! [See this](https://github.com/diezo/ensta#:~:text=NewSessionID(%22username%22%2C%20%22password%22))
-
-## Installation
-To install this package using [Python's PIP](https://pypi.org/project/pip/), run this command in a terminal window:
-```shell
-$ pip install ensta
-```
-
-To update the existing package, run:
-```shell
-$ pip install ensta --upgrade
-```
-
-## 🧔🏻‍♂️ Guest Mode
-This mode doesn't require login and can be used to fetch publicly available data from Instagram's Servers. Following methods are supported till now:
-- Check if username is available for registration
-- Fetch someone's profile data
-- Convert username to userid
-- Convert userid to username
-
-Here's an example where an instance of *Guest Class* is created to fetch [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) profile information:
-
-```python
-from ensta import Guest
-
-guest = Guest()
-profile = guest.profile("cristiano")
-
-if profile is None:
-    print("Something went wrong.")
-else:
-    print(profile.biography)
-    print(profile.follower_count)
-    print(profile.following_count)
-```
-
-## 🧔🏻‍♂️ Host Mode
-Host mode requires login through SessionID, which should be passed as an argument during initialization.
-It can be used to take actions that require login. Additionally, users can manage their own profile through this class.
-
-These are the methods supported till now:
-- Check authentication status of the user
-- Follow/unfollow users
-- Fetch someone's follower/following list
-- Switch account type - 'Public' or 'Private'
-
-Here's an example where an instance of *Host Class* is created to follow [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) account:
-
-```python
-from ensta import Host, NewSessionID
-
-sessionid = NewSessionID("username", "password")
-
-host = Host(sessionid)
-status = host.follow("cristiano")
-
-if status is None:
-    print("Something went wrong.")
-else:
-    if status.following:
-        print("Following!")
-    
-    elif status.follow_requested:
-        print("Requested to follow!")
-```
-
-> ### **Note:**
-> When you create a new sessionid through *NewSessionID()*, it's recommended to save it somewhere, and use the same sessionid (instead of creating a new one each time you need) until it expires or becomes invalid.
->
-> This should be done to avoid unnecessary prolonged wait time while generating a new sessionid and also to prevent getting your account from getting flagged because of repetitive logins.
-
-## 📋 Remember
-Every function should return **None** on failure. So, it's recommended to add an *if statement* before using the actual data to avoid TypeErrors. Here's an example:
-```python
-from ensta import Guest
-
-guest = Guest()
-available = guest.username_availability("cristiano")
-
-if available is None:  # 'None' indicates failure
-    print("Something went wrong.")
-else:
-    print(available)
-```
-
-## ❤️ Donate
-If you wish to help me in the development of Ensta, consider donating:
-
-[<img src="https://www.buymeacoffee.com/assets/img/guidelines/download-assets-sm-1.svg" width="150"/>](https://buymeacoffee.com/diezo)
-
-## Disclaimer
-This is a third-party package, and not approved by Instagram. It doesn't promote illegal activities or activities that violate [Instagram's Community Guidelines](https://help.instagram.com/477434105621119/) such as spamming users, creating bot accounts, misusing data etc. You are solely responsible for all the actions you take using this package.
+# 🤖 Ensta - Simple Instagram API
+[![PyPI](https://img.shields.io/pypi/v/ensta)](https://pypi.org/project/ensta)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ensta)]()
+[![Downloads](https://static.pepy.tech/badge/ensta)](https://pepy.tech/project/ensta)
+[![Twitter Share](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)](https://twitter.com/intent/tweet?text=Wow:&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)
+
+<img style="border-radius: 10px" src="https://imgtr.ee/images/2023/06/14/Twfd4.png"/>
+
+This package lets you use Instagram's Internal Web API through simple functions and classes. Ensta uses Instagram's Original Web API to scrape data which makes it a reliable choice over other third-party scrapers. This library mainly focuses on Simplicity & Reliability.
+
+Two type of classes are supported - ***Guest & Host***.
+
+[<img style="margin-top: 10px" src="https://www.buymeacoffee.com/assets/img/guidelines/download-assets-sm-1.svg" width="160"/>](https://buymeacoffee.com/diezo)
+
+## 📢 Announcement
+Users can now log in through their **Username** and **Password** to generate SessionId! [See this](https://github.com/diezo/ensta#:~:text=NewSessionID(%22username%22%2C%20%22password%22))
+
+## Installation
+To install this package using [Python's PIP](https://pypi.org/project/pip/), run this command in a terminal window:
+```shell
+$ pip install ensta
+```
+
+To update the existing package, run:
+```shell
+$ pip install ensta --upgrade
+```
+
+## 🧔🏻‍♂️ Guest Mode
+This mode doesn't require login and can be used to fetch publicly available data from Instagram's Servers. Following methods are supported till now:
+- Check if username is available for registration
+- Fetch someone's profile data
+- Convert username to userid
+- Convert userid to username
+
+Here's an example where an instance of *Guest Class* is created to fetch [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) profile information:
+
+```python
+from ensta import Guest
+
+guest = Guest()
+profile = guest.profile("cristiano")
+
+if profile is None:
+    print("Something went wrong.")
+else:
+    print(profile.biography)
+    print(profile.follower_count)
+    print(profile.following_count)
+```
+
+## 🧔🏻‍♂️ Host Mode
+Host mode requires login through SessionID, which should be passed as an argument during initialization.
+It can be used to take actions that require login. Additionally, users can manage their own profile through this class.
+
+These are the methods supported till now:
+- Check authentication status of the user
+- Follow/unfollow users
+- Fetch someone's follower/following list
+- Switch account type - 'Public' or 'Private'
+
+Here's an example where an instance of *Host Class* is created to follow [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) account:
+
+```python
+from ensta import Host, NewSessionID
+
+sessionid = NewSessionID("username", "password")
+
+host = Host(sessionid)
+status = host.follow("cristiano")
+
+if status is None:
+    print("Something went wrong.")
+else:
+    if status.following:
+        print("Following!")
+    
+    elif status.follow_requested:
+        print("Requested to follow!")
+```
+
+> ### **Note:**
+> When you create a new sessionid through *NewSessionID()*, it's recommended to save it somewhere, and use the same sessionid (instead of creating a new one each time you need) until it expires or becomes invalid.
+>
+> This should be done to avoid unnecessary prolonged wait time while generating a new sessionid and also to prevent getting your account from getting flagged because of repetitive logins.
+
+## 📋 Remember
+Every function should return **None** on failure. So, it's recommended to add an *if statement* before using the actual data to avoid TypeErrors. Here's an example:
+```python
+from ensta import Guest
+
+guest = Guest()
+available = guest.username_availability("cristiano")
+
+if available is None:  # 'None' indicates failure
+    print("Something went wrong.")
+else:
+    print(available)
+```
+
+## ❤️ Donate
+If you wish to help me in the development of Ensta, consider donating:
+
+[<img src="https://www.buymeacoffee.com/assets/img/guidelines/download-assets-sm-1.svg" width="150"/>](https://buymeacoffee.com/diezo)
+
+## Disclaimer
+This is a third-party package, and not approved by Instagram. It doesn't promote illegal activities or activities that violate [Instagram's Community Guidelines](https://help.instagram.com/477434105621119/) such as spamming users, creating bot accounts, misusing data etc. You are solely responsible for all the actions you take using this package.
```

### Comparing `ensta-2.6/ensta/Guest.py` & `ensta-2.7/ensta/Guest.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,203 +1,203 @@
-from json import JSONDecodeError
-import random
-import requests
-from .lib.Commons import (
-    update_session,
-    update_homepage_source,
-    update_app_id,
-    refresh_csrf_token,
-    format_username,
-    format_uid
-)
-from .lib.Exceptions import APIError
-from .containers.Profile import Profile
-from .containers.ProfileHost import ProfileHost
-import dataclasses
-
-
-class Guest:
-    request_session: requests.Session = None
-    homepage_source: str = None
-    insta_app_id: str = None
-    csrf_token: str = None
-
-    def __init__(self, homepage_source: str = None, app_id: str | int = None) -> None:
-        update_session(self)
-
-        if homepage_source is not None:
-            self.homepage_source = homepage_source
-        else:
-            update_homepage_source(self)
-
-        if app_id is not None:
-            self.insta_app_id = str(app_id)
-        else:
-            update_app_id(self)
-
-    def username_availability(self, username: str) -> bool | None:
-        username = format_username(username)
-        refresh_csrf_token(self)
-        body_json = {
-            "email": f"{username}@{self.csrf_token}.com",
-            "username": username,
-            "first_name": username.capitalize(),
-            "opt_into_one_tap": False
-        }
-        request_headers = {
-            "accept": "*/*",
-            "accept-language": "en-US,en;q=0.9",
-            "content-type": "application/x-www-form-urlencoded",
-            "sec-ch-prefers-color-scheme": random.choice(["light", "dark"]),
-            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
-            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
-            "sec-ch-ua-mobile": "?0",
-            "sec-ch-ua-platform": "\"Windows\"",
-            "sec-ch-ua-platform-version": "\"15.0.0\"",
-            "sec-fetch-dest": "empty",
-            "sec-fetch-mode": "cors",
-            "sec-fetch-site": "same-origin",
-            "viewport-width": "1475",
-            "x-asbd-id": "198387",
-            "x-csrftoken": self.csrf_token,
-            "x-ig-app-id": self.insta_app_id,
-            "x-ig-www-claim": "0",
-            "x-instagram-ajax": "1007614758",
-            "x-requested-with": "XMLHttpRequest",
-            "Referer": "https://www.instagram.com/accounts/emailsignup/",
-            "Referrer-Policy": "strict-origin-when-cross-origin"
-        }
-
-        try:
-            http_response = self.request_session.post("https://www.instagram.com/api/v1/web/accounts/web_create_ajax/attempt/", headers=request_headers, data=body_json)
-            response_json = http_response.json()
-
-            if "errors" in response_json:
-                return "username" not in response_json["errors"]
-        except JSONDecodeError:
-            return None
-
-    def profile(self, username: str, __session__: requests.Session | None = None) -> Profile | ProfileHost | None:
-        username: str = format_username(username)
-        refresh_csrf_token(self)
-        request_headers: dict = {
-            "accept": "*/*",
-            "accept-language": "en-US,en;q=0.9",
-            "sec-ch-prefers-color-scheme": random.choice(["light", "dark"]),
-            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
-            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
-            "sec-ch-ua-mobile": "?0",
-            "sec-ch-ua-platform": "\"Windows\"",
-            "sec-ch-ua-platform-version": "\"15.0.0\"",
-            "sec-fetch-dest": "empty",
-            "sec-fetch-mode": "cors",
-            "sec-fetch-site": "same-origin",
-            "viewport-width": "1475",
-            "x-asbd-id": "198387",
-            "x-csrftoken": self.csrf_token,
-            "x-ig-app-id": self.insta_app_id,
-            "x-ig-www-claim": "0",
-            "x-requested-with": "XMLHttpRequest",
-            "Referer": f"https://www.instagram.com/{username}/",
-            "Referrer-Policy": "strict-origin-when-cross-origin"
-        }
-
-        try:
-            session: requests.Session = __session__
-            if __session__ is None: session: requests.Session = self.request_session
-
-            http_response: requests.Response = session.get(
-                f"https://www.instagram.com/api/v1/users/web_profile_info/?username={username}",
-                headers=request_headers
-            )
-            response_json: dict = http_response.json()
-
-            if "status" in response_json:
-                if response_json["status"] == "ok" and "data" in response_json:
-                    if "user" in response_json["data"]:
-                        try:
-                            data: dict = response_json["data"]["user"]
-
-                            if data is None:
-                                return None
-
-                            profile = Profile(
-                                biography=data["biography"],
-                                biography_links=data["bio_links"],
-                                country_block=data["country_block"],
-                                full_name=data["full_name"],
-                                follower_count=data["edge_followed_by"]["count"],
-                                following_count=data["edge_follow"]["count"],
-                                user_id=data["id"],
-                                is_business_account=data["is_business_account"],
-                                is_professional_account=data["is_professional_account"],
-                                is_supervision_enabled=data["is_supervision_enabled"],
-                                is_joined_recently=data["is_joined_recently"],
-                                is_private=data["is_private"],
-                                is_verified=data["is_verified"],
-                                profile_picture_url=data["profile_pic_url"],
-                                profile_picture_url_hd=data["profile_pic_url_hd"],
-                                pronouns=data["pronouns"],
-                                has_ar_effects=data["has_ar_effects"],
-                                has_clips=data["has_clips"],
-                                has_guides=data["has_guides"],
-                                has_channel=data["has_channel"],
-                                highlight_count=data["highlight_reel_count"],
-                                hide_like_and_view_counts=data["hide_like_and_view_counts"],
-                                is_embeds_disabled=data["is_embeds_disabled"],
-                                is_verified_by_mv4b=data["is_verified_by_mv4b"],
-                                should_show_category=data["should_show_category"],
-                                should_show_public_contacts=data["should_show_public_contacts"],
-                                show_account_transparency_details=data["show_account_transparency_details"],
-                                total_post_count=data["edge_owner_to_timeline_media"]["count"]
-                            )
-
-                            if __session__ is not None:
-                                profile_host = ProfileHost()
-
-                                for key, value in dataclasses.asdict(profile).items():
-                                    setattr(profile_host, key, value)
-
-                                profile_host.blocked_by_viewer = data["blocked_by_viewer"]
-                                profile_host.followed_by_viewer = data["followed_by_viewer"]
-                                profile_host.follows_viewer = data["follows_viewer"]
-                                profile_host.has_blocked_viewer = data["has_blocked_viewer"]
-                                profile_host.has_requested_viewer = data["has_requested_viewer"]
-                                profile_host.is_guardian_of_viewer = data["is_guardian_of_viewer"]
-                                profile_host.is_supervised_by_viewer = data["is_supervised_by_viewer"]
-                                profile_host.requested_by_viewer = data["requested_by_viewer"]
-                                profile_host.mutual_follower_count = data["edge_mutual_followed_by"]["count"]
-
-                                return profile_host
-
-                            return profile
-                        except KeyError:
-                            raise APIError()
-        except JSONDecodeError:
-            return None
-
-    def get_uid(self, username: str) -> str | None:
-        username: str = username.strip().lower().replace(" ", "")
-        response: Profile | None = self.profile(username)
-
-        if response.user_id is not None:
-            return format_uid(response.user_id)
-
-    def get_username(self, uid: str | int, __session__: requests.Session | None = None) -> str | None:
-        uid = format_uid(uid)
-        refresh_csrf_token(self)
-        request_headers = {
-            "User-Agent": "Instagram 76.0.0.15.395 Android (24/7.0; 640dpi; 1440x2560; samsung; SM-G930F; herolte; samsungexynos8890; en_US; 138226743)"
-        }
-
-        try:
-            session: requests.Session = __session__
-            if __session__ is None: session: requests.Session = self.request_session
-
-            http_response = session.get(f"https://i.instagram.com/api/v1/users/{uid}/info/", headers=request_headers)
-            response_json = http_response.json()
-
-            if "status" in response_json and response_json["status"] == "ok" and "user" in response_json and "username" in response_json["user"]:
-                return format_username(response_json["user"]["username"])
-
-        except JSONDecodeError:
-            return None
+from json import JSONDecodeError
+import random
+import requests
+from .lib.Commons import (
+    update_session,
+    update_homepage_source,
+    update_app_id,
+    refresh_csrf_token,
+    format_username,
+    format_uid
+)
+from .lib.Exceptions import APIError
+from .containers.Profile import Profile
+from .containers.ProfileHost import ProfileHost
+import dataclasses
+
+
+class Guest:
+    request_session: requests.Session = None
+    homepage_source: str = None
+    insta_app_id: str = None
+    csrf_token: str = None
+
+    def __init__(self, homepage_source: str = None, app_id: str | int = None) -> None:
+        update_session(self)
+
+        if homepage_source is not None:
+            self.homepage_source = homepage_source
+        else:
+            update_homepage_source(self)
+
+        if app_id is not None:
+            self.insta_app_id = str(app_id)
+        else:
+            update_app_id(self)
+
+    def username_availability(self, username: str) -> bool | None:
+        username = format_username(username)
+        refresh_csrf_token(self)
+        body_json = {
+            "email": f"{username}@{self.csrf_token}.com",
+            "username": username,
+            "first_name": username.capitalize(),
+            "opt_into_one_tap": False
+        }
+        request_headers = {
+            "accept": "*/*",
+            "accept-language": "en-US,en;q=0.9",
+            "content-type": "application/x-www-form-urlencoded",
+            "sec-ch-prefers-color-scheme": random.choice(["light", "dark"]),
+            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
+            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
+            "sec-ch-ua-mobile": "?0",
+            "sec-ch-ua-platform": "\"Windows\"",
+            "sec-ch-ua-platform-version": "\"15.0.0\"",
+            "sec-fetch-dest": "empty",
+            "sec-fetch-mode": "cors",
+            "sec-fetch-site": "same-origin",
+            "viewport-width": "1475",
+            "x-asbd-id": "198387",
+            "x-csrftoken": self.csrf_token,
+            "x-ig-app-id": self.insta_app_id,
+            "x-ig-www-claim": "0",
+            "x-instagram-ajax": "1007614758",
+            "x-requested-with": "XMLHttpRequest",
+            "Referer": "https://www.instagram.com/accounts/emailsignup/",
+            "Referrer-Policy": "strict-origin-when-cross-origin"
+        }
+
+        try:
+            http_response = self.request_session.post("https://www.instagram.com/api/v1/web/accounts/web_create_ajax/attempt/", headers=request_headers, data=body_json)
+            response_json = http_response.json()
+
+            if "errors" in response_json:
+                return "username" not in response_json["errors"]
+        except JSONDecodeError:
+            return None
+
+    def profile(self, username: str, __session__: requests.Session | None = None) -> Profile | ProfileHost | None:
+        username: str = format_username(username)
+        refresh_csrf_token(self)
+        request_headers: dict = {
+            "accept": "*/*",
+            "accept-language": "en-US,en;q=0.9",
+            "sec-ch-prefers-color-scheme": random.choice(["light", "dark"]),
+            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
+            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
+            "sec-ch-ua-mobile": "?0",
+            "sec-ch-ua-platform": "\"Windows\"",
+            "sec-ch-ua-platform-version": "\"15.0.0\"",
+            "sec-fetch-dest": "empty",
+            "sec-fetch-mode": "cors",
+            "sec-fetch-site": "same-origin",
+            "viewport-width": "1475",
+            "x-asbd-id": "198387",
+            "x-csrftoken": self.csrf_token,
+            "x-ig-app-id": self.insta_app_id,
+            "x-ig-www-claim": "0",
+            "x-requested-with": "XMLHttpRequest",
+            "Referer": f"https://www.instagram.com/{username}/",
+            "Referrer-Policy": "strict-origin-when-cross-origin"
+        }
+
+        try:
+            session: requests.Session = __session__
+            if __session__ is None: session: requests.Session = self.request_session
+
+            http_response: requests.Response = session.get(
+                f"https://www.instagram.com/api/v1/users/web_profile_info/?username={username}",
+                headers=request_headers
+            )
+            response_json: dict = http_response.json()
+
+            if "status" in response_json:
+                if response_json["status"] == "ok" and "data" in response_json:
+                    if "user" in response_json["data"]:
+                        try:
+                            data: dict = response_json["data"]["user"]
+
+                            if data is None:
+                                return None
+
+                            profile = Profile(
+                                biography=data["biography"],
+                                biography_links=data["bio_links"],
+                                country_block=data["country_block"],
+                                full_name=data["full_name"],
+                                follower_count=data["edge_followed_by"]["count"],
+                                following_count=data["edge_follow"]["count"],
+                                user_id=data["id"],
+                                is_business_account=data["is_business_account"],
+                                is_professional_account=data["is_professional_account"],
+                                is_supervision_enabled=data["is_supervision_enabled"],
+                                is_joined_recently=data["is_joined_recently"],
+                                is_private=data["is_private"],
+                                is_verified=data["is_verified"],
+                                profile_picture_url=data["profile_pic_url"],
+                                profile_picture_url_hd=data["profile_pic_url_hd"],
+                                pronouns=data["pronouns"],
+                                has_ar_effects=data["has_ar_effects"],
+                                has_clips=data["has_clips"],
+                                has_guides=data["has_guides"],
+                                has_channel=data["has_channel"],
+                                highlight_count=data["highlight_reel_count"],
+                                hide_like_and_view_counts=data["hide_like_and_view_counts"],
+                                is_embeds_disabled=data["is_embeds_disabled"],
+                                is_verified_by_mv4b=data["is_verified_by_mv4b"],
+                                should_show_category=data["should_show_category"],
+                                should_show_public_contacts=data["should_show_public_contacts"],
+                                show_account_transparency_details=data["show_account_transparency_details"],
+                                total_post_count=data["edge_owner_to_timeline_media"]["count"]
+                            )
+
+                            if __session__ is not None:
+                                profile_host = ProfileHost()
+
+                                for key, value in dataclasses.asdict(profile).items():
+                                    setattr(profile_host, key, value)
+
+                                profile_host.blocked_by_viewer = data["blocked_by_viewer"]
+                                profile_host.followed_by_viewer = data["followed_by_viewer"]
+                                profile_host.follows_viewer = data["follows_viewer"]
+                                profile_host.has_blocked_viewer = data["has_blocked_viewer"]
+                                profile_host.has_requested_viewer = data["has_requested_viewer"]
+                                profile_host.is_guardian_of_viewer = data["is_guardian_of_viewer"]
+                                profile_host.is_supervised_by_viewer = data["is_supervised_by_viewer"]
+                                profile_host.requested_by_viewer = data["requested_by_viewer"]
+                                profile_host.mutual_follower_count = data["edge_mutual_followed_by"]["count"]
+
+                                return profile_host
+
+                            return profile
+                        except KeyError:
+                            raise APIError()
+        except JSONDecodeError:
+            return None
+
+    def get_uid(self, username: str) -> str | None:
+        username: str = username.strip().lower().replace(" ", "")
+        response: Profile | None = self.profile(username)
+
+        if response.user_id is not None:
+            return format_uid(response.user_id)
+
+    def get_username(self, uid: str | int, __session__: requests.Session | None = None) -> str | None:
+        uid = format_uid(uid)
+        refresh_csrf_token(self)
+        request_headers = {
+            "User-Agent": "Instagram 76.0.0.15.395 Android (24/7.0; 640dpi; 1440x2560; samsung; SM-G930F; herolte; samsungexynos8890; en_US; 138226743)"
+        }
+
+        try:
+            session: requests.Session = __session__
+            if __session__ is None: session: requests.Session = self.request_session
+
+            http_response = session.get(f"https://i.instagram.com/api/v1/users/{uid}/info/", headers=request_headers)
+            response_json = http_response.json()
+
+            if "status" in response_json and response_json["status"] == "ok" and "user" in response_json and "username" in response_json["user"]:
+                return format_username(response_json["user"]["username"])
+
+        except JSONDecodeError:
+            return None
```

### Comparing `ensta-2.6/ensta/Host.py` & `ensta-2.7/ensta/Host.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,669 +1,669 @@
-import requests
-import random
-import string
-import json
-from json import JSONDecodeError
-from collections.abc import Generator
-from .Guest import Guest
-from .lib.Commons import (
-    refresh_csrf_token,
-    update_app_id,
-    update_homepage_source,
-    update_session,
-    format_identifier,
-    format_url,
-    format_username
-)
-from .lib import (
-    SessionError,
-    NetworkError,
-    IdentifierError,
-    DevelopmentError,
-    APIError
-)
-from .containers import (FollowedStatus, UnfollowedStatus, FollowPerson)
-from .containers.ProfileHost import ProfileHost
-from .containers.Post import Post
-from .containers.PostUser import PostUser
-
-USERNAME = 0
-UID = 1
-
-
-class Host:
-    request_session: requests.Session = None
-    homepage_source: str = None
-    insta_app_id: str = None
-    preferred_color_scheme: str = "dark"
-    x_ig_www_claim: str = None
-    csrf_token: str = None
-    guest: Guest = None
-
-    def __init__(self, session_id: str) -> None:
-        self.x_ig_www_claim = "hmac." + "".join(random.choices(string.ascii_letters + string.digits + "_-", k=48))
-        update_session(self)
-        update_homepage_source(self)
-        update_app_id(self)
-
-        self.guest = Guest(
-            homepage_source=self.homepage_source,
-            app_id=self.insta_app_id
-        )
-
-        self.request_session.cookies.set("sessionid", session_id)
-
-        if not self.authenticated():
-            raise SessionError("SessionID is incorrect or expired.")
-
-    def update_homepage_source(self) -> None:
-        temp_homepage_source = requests.get("https://www.instagram.com/").text.strip()
-
-        if temp_homepage_source == "":
-            raise NetworkError("Couldn't load instagram homepage.")
-
-        self.homepage_source = temp_homepage_source
-
-    def authenticated(self) -> bool:
-        refresh_csrf_token(self)
-        request_headers = {
-            "accept": "*/*",
-            "accept-language": "en-US,en;q=0.9",
-            "sec-ch-prefers-color-scheme": self.preferred_color_scheme,
-            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
-            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
-            "sec-ch-ua-mobile": "?0",
-            "sec-ch-ua-platform": "\"Windows\"",
-            "sec-ch-ua-platform-version": "\"15.0.0\"",
-            "sec-fetch-dest": "empty",
-            "sec-fetch-mode": "cors",
-            "sec-fetch-site": "same-origin",
-            "viewport-width": "1475",
-            "x-asbd-id": "198387",
-            "x-csrftoken": self.csrf_token,
-            "x-ig-app-id": self.insta_app_id,
-            "x-ig-www-claim": self.x_ig_www_claim,
-            "x-requested-with": "XMLHttpRequest",
-            "Referer": "https://www.instagram.com/accounts/edit/",
-            "Referrer-Policy": "strict-origin-when-cross-origin"
-        }
-        http_response = self.request_session.get("https://www.instagram.com/api/v1/accounts/edit/web_form_data/", headers=request_headers)
-
-        try:
-            http_response.json()
-            return True
-        except JSONDecodeError:
-            return False
-
-    def follow(self, identifier: str | int) -> FollowedStatus | None:
-        conversion_success, identifier = self._identifier(identifier, UID)
-        if not conversion_success: return None
-
-        # Actual Request
-        refresh_csrf_token(self)
-        body_json = {
-            "container_module": "profile",
-            "nav_chain": f"PolarisProfileRoot:profilePage:1:via_cold_start",
-            "user_id": identifier
-        }
-        request_headers = {
-            "accept": "*/*",
-            "accept-language": "en-US,en;q=0.9",
-            "content-type": "application/x-www-form-urlencoded",
-            "sec-ch-prefers-color-scheme": self.preferred_color_scheme,
-            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
-            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
-            "sec-ch-ua-mobile": "?0",
-            "sec-ch-ua-platform": "\"Windows\"",
-            "sec-ch-ua-platform-version": "\"15.0.0\"",
-            "sec-fetch-dest": "empty",
-            "sec-fetch-mode": "cors",
-            "sec-fetch-site": "same-origin",
-            "viewport-width": "1475",
-            "x-asbd-id": "198387",
-            "x-csrftoken": self.csrf_token,
-            "x-ig-app-id": self.insta_app_id,
-            "x-ig-www-claim": self.x_ig_www_claim,
-            "x-instagram-ajax": "1007616494",
-            "x-requested-with": "XMLHttpRequest",
-            "Referer": f"https://www.instagram.com/{''.join(random.choices(string.ascii_lowercase, k=5))}/",
-            "Referrer-Policy": "strict-origin-when-cross-origin"
-        }
-
-        try:
-            http_response = self.request_session.post(f"https://www.instagram.com/api/v1/friendships/create/{identifier}/", headers=request_headers, data=body_json)
-            response_json = http_response.json()
-
-            if "status" in response_json:
-                if response_json["status"] == "ok" and "friendship_status" in response_json:
-                    if "following" in response_json["friendship_status"] \
-                            and "outgoing_request" in response_json["friendship_status"] \
-                            and "followed_by" in response_json["friendship_status"] \
-                            and "previous_following" in response_json:
-                        return FollowedStatus(
-                            following=response_json["friendship_status"]["following"],
-                            follow_requested=response_json["friendship_status"]["outgoing_request"],
-                            is_my_follower=response_json["friendship_status"]["followed_by"],
-                            previous_following=response_json["previous_following"]
-                        )
-        except JSONDecodeError:
-            return None
-
-    def unfollow(self, identifier: str | int) -> UnfollowedStatus | None:
-        conversion_success, identifier = self._identifier(identifier, UID)
-        if not conversion_success: return None
-
-        # Actual Request
-        refresh_csrf_token(self)
-        body_json = {
-            "container_module": "profile",
-            "nav_chain": f"PolarisProfileRoot:profilePage:1:via_cold_start",
-            "user_id": identifier
-        }
-        request_headers = {
-            "accept": "*/*",
-            "accept-language": "en-US,en;q=0.9",
-            "content-type": "application/x-www-form-urlencoded",
-            "sec-ch-prefers-color-scheme": self.preferred_color_scheme,
-            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
-            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
-            "sec-ch-ua-mobile": "?0",
-            "sec-ch-ua-platform": "\"Windows\"",
-            "sec-ch-ua-platform-version": "\"15.0.0\"",
-            "sec-fetch-dest": "empty",
-            "sec-fetch-mode": "cors",
-            "sec-fetch-site": "same-origin",
-            "viewport-width": "1475",
-            "x-asbd-id": "198387",
-            "x-csrftoken": self.csrf_token,
-            "x-ig-app-id": self.insta_app_id,
-            "x-ig-www-claim": self.x_ig_www_claim,
-            "x-instagram-ajax": "1007616494",
-            "x-requested-with": "XMLHttpRequest",
-            "Referer": f"https://www.instagram.com/{''.join(random.choices(string.ascii_lowercase, k=6))}/",
-            "Referrer-Policy": "strict-origin-when-cross-origin"
-        }
-
-        try:
-            http_response = self.request_session.post(f"https://www.instagram.com/api/v1/friendships/destroy/{identifier}/", headers=request_headers, data=body_json)
-            response_json = http_response.json()
-
-            if "status" in response_json:
-                if response_json["status"] == "ok" and "friendship_status" in response_json:
-                    if "following" in response_json["friendship_status"] \
-                            and "outgoing_request" in response_json["friendship_status"] \
-                            and "followed_by" in response_json["friendship_status"]:
-                        return UnfollowedStatus(
-                            unfollowed=not response_json["friendship_status"]["following"] and not response_json["friendship_status"]["outgoing_request"],
-                            is_my_follower=response_json["friendship_status"]["followed_by"]
-                        )
-        except JSONDecodeError:
-            return None
-
-    def followers(self, identifier: str | int, count: int = 0) -> Generator[FollowPerson, None, None]:
-        conversion_success, identifier = self._identifier(identifier, UID)
-        if not conversion_success:
-            yield None
-            return None
-
-        # Actual Request
-        refresh_csrf_token(self)
-        request_headers: dict = {
-            "accept": "*/*",
-            "accept-language": "en-US,en;q=0.9",
-            "sec-ch-prefers-color-scheme": self.preferred_color_scheme,
-            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
-            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
-            "sec-ch-ua-mobile": "?0",
-            "sec-ch-ua-platform": "\"Windows\"",
-            "sec-ch-ua-platform-version": "\"15.0.0\"",
-            "sec-fetch-dest": "empty",
-            "sec-fetch-mode": "cors",
-            "sec-fetch-site": "same-origin",
-            "viewport-width": "1475",
-            "x-asbd-id": "198387",
-            "x-csrftoken": self.csrf_token,
-            "x-ig-app-id": self.insta_app_id,
-            "x-ig-www-claim": self.x_ig_www_claim,
-            "x-requested-with": "XMLHttpRequest",
-            "Referer": f"https://www.instagram.com/{''.join(random.choices(string.ascii_lowercase, k=6))}/followers/",
-            "Referrer-Policy": "strict-origin-when-cross-origin"
-        }
-
-        current_max_id: str = ""
-        generated_count: int = 0
-
-        while True:
-            current_max_id_text: str = ""
-
-            if current_max_id != "":
-                current_max_id_text: str = f"&max_id={current_max_id}"
-
-            try:
-                count_text = 35
-
-                if count < 35:
-                    count_text = count
-
-                http_response = self.request_session.get(f"https://www.instagram.com/api/v1/friendships/{identifier}/followers/?count={str(count_text)}{current_max_id_text}&search_surface=follow_list_page", headers=request_headers)
-                response_json = http_response.json()
-
-                if "status" not in response_json or "users" not in response_json:
-                    yield None
-                    return None
-
-                if response_json["status"] != "ok":
-                    yield None
-                    return None
-
-                for each_item in response_json["users"]:
-                    if generated_count < count or count == 0:
-
-                        try:
-                            yield FollowPerson(
-                                has_anonymous_profile_picture=each_item["has_anonymous_profile_picture"],
-                                user_id=each_item["pk"],
-                                username=each_item["username"],
-                                full_name=each_item["full_name"],
-                                is_private=each_item["is_private"],
-                                is_verified=each_item["is_verified"],
-                                profile_picture_url=each_item["profile_pic_url"],
-                                badges=each_item["account_badges"],
-                                third_party_downloads_enabled=each_item["third_party_downloads_enabled"],
-                                is_possible_scammer=each_item["is_possible_scammer"]
-                            )
-
-                        except KeyError:
-                            raise APIError()
-
-                        generated_count += 1
-
-                if (generated_count < count or count == 0) and "next_max_id" in response_json:
-                    current_max_id = response_json["next_max_id"]
-                else:
-                    return None
-            except JSONDecodeError:
-                yield None
-                return None
-
-    def followings(self, identifier: str | int, count: int = 0) -> Generator[FollowPerson, None, None]:
-        conversion_success, identifier = self._identifier(identifier, UID)
-        if not conversion_success:
-            yield None
-            return None
-
-        # Actual Request
-        refresh_csrf_token(self)
-        request_headers = {
-            "accept": "*/*",
-            "accept-language": "en-US,en;q=0.9",
-            "sec-ch-prefers-color-scheme": self.preferred_color_scheme,
-            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
-            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
-            "sec-ch-ua-mobile": "?0",
-            "sec-ch-ua-platform": "\"Windows\"",
-            "sec-ch-ua-platform-version": "\"15.0.0\"",
-            "sec-fetch-dest": "empty",
-            "sec-fetch-mode": "cors",
-            "sec-fetch-site": "same-origin",
-            "viewport-width": "1475",
-            "x-asbd-id": "198387",
-            "x-csrftoken": self.csrf_token,
-            "x-ig-app-id": self.insta_app_id,
-            "x-ig-www-claim": self.x_ig_www_claim,
-            "x-requested-with": "XMLHttpRequest",
-            "Referer": f"https://www.instagram.com/{''.join(random.choices(string.ascii_lowercase, k=6))}/following/",
-            "Referrer-Policy": "strict-origin-when-cross-origin"
-        }
-
-        current_max_id = ""
-        generated_count = 0
-
-        while True:
-            current_max_id_text = ""
-
-            if current_max_id != "":
-                current_max_id_text = f"&max_id={current_max_id}"
-
-            try:
-                count_text = 35
-
-                if count < 35:
-                    count_text = count
-
-                http_response = self.request_session.get(
-                    f"https://www.instagram.com/api/v1/friendships/{identifier}/following/?count={str(count_text)}{current_max_id_text}",
-                    headers=request_headers)
-                response_json = http_response.json()
-
-                if "status" not in response_json or "users" not in response_json:
-                    yield None
-                    return None
-
-                if response_json["status"] != "ok":
-                    yield None
-                    return None
-
-                for each_item in response_json["users"]:
-                    if generated_count < count or count == 0:
-
-                        try:
-                            yield FollowPerson(
-                                has_anonymous_profile_picture=each_item["has_anonymous_profile_picture"],
-                                user_id=each_item["pk"],
-                                username=each_item["username"],
-                                full_name=each_item["full_name"],
-                                is_private=each_item["is_private"],
-                                is_verified=each_item["is_verified"],
-                                profile_picture_url=each_item["profile_pic_url"],
-                                is_possible_scammer=each_item["is_possible_scammer"]
-                            )
-
-                        except KeyError:
-                            raise APIError()
-
-                        generated_count += 1
-
-                if (generated_count < count or count == 0) and "next_max_id" in response_json:
-                    current_max_id = response_json["next_max_id"]
-                else:
-                    return None
-            except JSONDecodeError:
-                yield None
-                return None
-
-    def posts(self, username: str, count: int = 0) -> Generator[Post, None, None]:
-        username = format_username(username)
-
-        refresh_csrf_token(self)
-        request_headers = {
-            "accept": "*/*",
-            "accept-language": "en-US,en;q=0.9",
-            "sec-ch-prefers-color-scheme": self.preferred_color_scheme,
-            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
-            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.110\", \"Google Chrome\";v=\"114.0.5735.110\"",
-            "sec-ch-ua-mobile": "?0",
-            "sec-ch-ua-platform": "\"Windows\"",
-            "sec-ch-ua-platform-version": "\"15.0.0\"",
-            "sec-fetch-dest": "empty",
-            "sec-fetch-mode": "cors",
-            "sec-fetch-site": "same-origin",
-            "viewport-width": "1475",
-            "x-asbd-id": "129477",
-            "x-csrftoken": self.csrf_token,
-            "x-ig-app-id": self.insta_app_id,
-            "x-ig-www-claim": self.x_ig_www_claim,
-            "x-requested-with": "XMLHttpRequest",
-            "Referer": f"https://www.instagram.com/{username}/",
-            "Referrer-Policy": "strict-origin-when-cross-origin"
-        }
-
-        current_max_id = ""
-        generated_count = 0
-
-        while True:
-            current_max_id_text = ""
-
-            if current_max_id != "":
-                current_max_id_text = f"&max_id={current_max_id}"
-
-            try:
-                count_text = 35
-
-                if count < 35:
-                    count_text = count
-
-                http_response = self.request_session.get(f"https://www.instagram.com/api/v1/feed/user/{username}/username/?count={count_text}{current_max_id_text}", headers=request_headers)
-                response_json = http_response.json()
-
-                if "status" not in response_json or "items" not in response_json:
-                    yield None
-                    return None
-
-                if response_json["status"] != "ok":
-                    yield None
-                    return None
-
-                for each_item in response_json["items"]:
-                    if generated_count < count or count == 0:
-
-                        yield self._process_post_data(each_item)
-                        generated_count += 1
-
-                if (generated_count < count or count == 0) and "next_max_id" in response_json:
-                    current_max_id = response_json["next_max_id"]
-                else:
-                    return None
-            except JSONDecodeError:
-                yield None
-                return None
-
-    def _identifier(self, identifier: str | int, required: str | int):
-        identifier = format_identifier(identifier)
-
-        if len(identifier) <= 0:
-            raise IdentifierError("No identifier was given. Please pass either UserId or Username as an argument.")
-
-        # Identifier: Username or UID?
-        is_username = False
-        for letter in identifier:
-            if letter not in string.digits:
-                is_username = True
-                break
-
-        if is_username and required == USERNAME:
-            return True, identifier
-
-        elif is_username and required == UID:
-            user_id = self.guest.get_uid(identifier)
-
-            if user_id is not None and user_id != "":
-                return True, user_id
-            else:
-                return False, None
-
-        elif not is_username and required == USERNAME:
-            username = self.guest.get_username(identifier)
-
-            if username is not None and username != "":
-                return True, username
-            else:
-                return False, None
-
-        elif not is_username and required == UID:
-            return True, identifier
-
-        else:
-            raise DevelopmentError("Identifier Conversion (Else Block)")
-
-    def _set_account_privacy(self, privacy: str) -> bool:
-        is_private = (privacy == "private")
-
-        if privacy != "private" and privacy != "public":
-            raise DevelopmentError("_set_account_privacy")
-
-        refresh_csrf_token(self)
-        body_json = {
-            "is_private": is_private
-        }
-        request_headers = {
-            "accept": "*/*",
-            "accept-language": "en-US,en;q=0.9",
-            "content-type": "application/x-www-form-urlencoded",
-            "sec-ch-prefers-color-scheme": self.preferred_color_scheme,
-            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
-            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
-            "sec-ch-ua-mobile": "?0",
-            "sec-ch-ua-platform": "\"Windows\"",
-            "sec-ch-ua-platform-version": "\"15.0.0\"",
-            "sec-fetch-dest": "empty",
-            "sec-fetch-mode": "cors",
-            "sec-fetch-site": "same-origin",
-            "viewport-width": "1475",
-            "x-asbd-id": "198387",
-            "x-csrftoken": self.csrf_token,
-            "x-ig-app-id": self.insta_app_id,
-            "x-ig-www-claim": self.x_ig_www_claim,
-            "x-instagram-ajax": "1007616494",
-            "x-requested-with": "XMLHttpRequest",
-            "Referer": "https://www.instagram.com/accounts/who_can_see_your_content/",
-            "Referrer-Policy": "strict-origin-when-cross-origin"
-        }
-
-        try:
-            http_response = self.request_session.post("https://www.instagram.com/api/v1/web/accounts/set_private/", headers=request_headers, data=body_json)
-            response_json = http_response.json()
-
-            if "status" not in response_json:
-                return False
-
-            if response_json["status"] != "ok":
-                return False
-
-            return True
-        except JSONDecodeError:
-            return False
-
-    def switch_to_private_account(self) -> bool:
-        return self._set_account_privacy("private")
-
-    def switch_to_public_account(self) -> bool:
-        return self._set_account_privacy("public")
-
-    def profile(self, username: str) -> ProfileHost | None:
-        return self.guest.profile(username, __session__=self.request_session)
-
-    def get_username(self, uid: str | int) -> str | None:
-        return self.guest.get_username(uid, __session__=self.request_session)
-
-    def post(self, share_url: str) -> Post | None:
-        share_url: str = format_url(share_url)
-        request_headers = {
-            "accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
-            "accept-language": "en-US,en;q=0.9",
-            "cache-control": "max-age=0",
-            "sec-ch-prefers-color-scheme": "dark",
-            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
-            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.110\", \"Google Chrome\";v=\"114.0.5735.110\"",
-            "sec-ch-ua-mobile": "?0",
-            "sec-ch-ua-platform": "\"Windows\"",
-            "sec-ch-ua-platform-version": "\"15.0.0\"",
-            "sec-fetch-dest": "document",
-            "sec-fetch-mode": "navigate",
-            "sec-fetch-site": "same-origin",
-            "sec-fetch-user": "?1",
-            "upgrade-insecure-requests": "1",
-            "viewport-width": "1475",
-            "referrerPolicy": "strict-origin-when-cross-origin"
-        }
-
-        http_response = self.request_session.get(share_url, headers=request_headers)
-        response_text = http_response.text
-
-        required_text = "{\"response\":\"{\\\"items\\\":"
-
-        initial_index = response_text.rfind(required_text)
-        if initial_index == -1: raise APIError()
-
-        rest_text = response_text[initial_index - len(required_text) + len(required_text): len(response_text)]
-        end_text = "\\\"auto_load_more_enabled\\\":false}\",\"status_code\":200}"
-        end_index = rest_text.find(end_text)
-
-        try:
-            data: dict = json.loads(rest_text[:end_index + len(end_text)])
-
-            if "response" in data:
-                response_data: dict = json.loads(data["response"])
-
-                if "items" in response_data:
-                    items_data: list = response_data["items"]
-
-                    if len(items_data) > 0:
-                        selected_post: dict = items_data[len(items_data) - 1]
-
-                        if selected_post is not None:
-                            return self._process_post_data(selected_post)
-
-        except JSONDecodeError:
-            return None
-
-    def _process_post_data(self, data: dict) -> Post:
-
-        caption: dict = data.get("caption", None)
-
-        caption_text = ""
-        is_caption_covered = False
-        caption_created_at = 0
-        caption_share_enabled = False
-        caption_did_report_as_spam = False
-
-        if caption is not None:
-            caption_text = caption.get("text", "")
-            is_caption_covered = caption.get("is_covered", False)
-            caption_created_at = caption.get("created_at", 0)
-            caption_share_enabled = caption.get("share_enabled", False)
-            caption_did_report_as_spam = caption.get("did_report_as_spam", False)
-
-        user: PostUser = PostUser()
-        user_data: dict = data.get("user", None)
-
-        if user_data is not None:
-            user: PostUser = PostUser(
-                has_anonymous_profile_picture=user_data.get("has_anonymous_profile_picture", False),
-                fbid_v2=user_data.get("fbid_v2", ""),
-                transparency_product_enabled=user_data.get("transparency_product_enabled", False),
-                is_favorite=user_data.get("is_favorite", False),
-                is_unpublished=user_data.get("is_unpublished", False),
-                uid=user_data.get("pk", ""),
-                username=user_data.get("username", ""),
-                full_name=user_data.get("full_name", ""),
-                is_private=user_data.get("is_private", False),
-                is_verified=user_data.get("is_verified", False),
-                profile_picture_id=user_data.get("profile_pic_id", ""),
-                profile_picture_url=user_data.get("profile_pic_url", ""),
-                account_badges=user_data.get("account_badges", []),
-                feed_post_reshare_disabled=user_data.get("feed_post_reshare_disabled", False),
-                show_account_transparency_details=user_data.get("show_account_transparency_details", False),
-                third_party_downloads_enabled=user_data.get("third_party_downloads_enabled", 0),
-                latest_reel_media=user_data.get("latest_reel_media", 0)
-            )
-
-        return Post(
-            _instance=self.__class__,
-            share_url=f"https://www.instagram.com/p/{data.get('code', '')}",
-            taken_at=data.get("taken_at", 0),
-            unique_key=data.get("pk", ""),
-            media_type=data.get("media_type", 0),
-            code=data.get("code", ""),
-            caption_is_edited=data.get("caption_is_edited", False),
-            original_media_has_visual_reply_media=data.get("original_media_has_visual_reply_media", False),
-            like_and_view_counts_disabled=data.get("like_and_view_counts_disabled", False),
-            can_viewer_save=data.get("can_viewer_save", False),
-            profile_grid_control_enabled=data.get("profile_grid_control_enabled", False),
-            is_comments_gif_composer_enabled=data.get("is_comments_gif_composer_enabled", False),
-            comment_threading_enabled=data.get("comment_threading_enabled", False),
-            comment_count=data.get("comment_count", 0),
-            has_liked=data.get("has_liked", False),
-            user=user,
-            can_viewer_reshare=data.get("can_viewer_reshare", False),
-            like_count=data.get("like_count", 0),
-            top_likers=data.get("top_likers", []),
-            caption_text=caption_text,
-            is_caption_covered=is_caption_covered,
-            caption_created_at=caption_created_at,
-            caption_share_enabled=caption_share_enabled,
-            caption_did_report_as_spam=caption_did_report_as_spam,
-            is_paid_partnership=data.get("is_paid_partnership", False),
-            show_shop_entrypoint=data.get("show_shop_entrypoint", False),
-            deleted_reason=data.get("deleted_reason", 0),
-            integrity_review_decision=data.get("integrity_review_decision", ""),
-            ig_media_sharing_disabled=data.get("ig_media_sharing_disabled", False),
-            has_shared_to_fb=data.get("has_shared_to_fb", False),
-            is_unified_video=data.get("is_unified_video", False),
-            should_request_ads=data.get("should_request_ads", False),
-            is_visual_reply_commenter_notice_enabled=data.get("is_visual_reply_commenter_notice_enabled", False),
-            commerciality_status=data.get("commerciality_status", ""),
-            explore_hide_comments=data.get("explore_hide_comments", False),
-            has_delayed_metadata=data.get("has_delayed_metadata", False),
-            location_latitude=data.get("lat", 0),
-            location_longitude=data.get("lng", 0)
-        )
+import requests
+import random
+import string
+import json
+from json import JSONDecodeError
+from collections.abc import Generator
+from .lib.Commons import (
+    refresh_csrf_token,
+    update_app_id,
+    update_homepage_source,
+    update_session,
+    format_identifier,
+    format_url,
+    format_username
+)
+from .lib import (
+    SessionError,
+    NetworkError,
+    IdentifierError,
+    DevelopmentError,
+    APIError
+)
+from .containers import (FollowedStatus, UnfollowedStatus, FollowPerson)
+from .containers.ProfileHost import ProfileHost
+from .containers.PostUser import PostUser
+from .containers.Post import Post
+from .Guest import Guest
+
+USERNAME = 0
+UID = 1
+
+
+class Host:
+    request_session: requests.Session = None
+    homepage_source: str = None
+    insta_app_id: str = None
+    preferred_color_scheme: str = "dark"
+    x_ig_www_claim: str = None
+    csrf_token: str = None
+    guest: Guest = None
+
+    def __init__(self, session_id: str) -> None:
+        self.x_ig_www_claim = "hmac." + "".join(random.choices(string.ascii_letters + string.digits + "_-", k=48))
+        update_session(self)
+        update_homepage_source(self)
+        update_app_id(self)
+
+        self.guest = Guest(
+            homepage_source=self.homepage_source,
+            app_id=self.insta_app_id
+        )
+
+        self.request_session.cookies.set("sessionid", session_id)
+
+        if not self.authenticated():
+            raise SessionError("SessionID is incorrect or expired.")
+
+    def update_homepage_source(self) -> None:
+        temp_homepage_source = requests.get("https://www.instagram.com/").text.strip()
+
+        if temp_homepage_source == "":
+            raise NetworkError("Couldn't load instagram homepage.")
+
+        self.homepage_source = temp_homepage_source
+
+    def authenticated(self) -> bool:
+        refresh_csrf_token(self)
+        request_headers = {
+            "accept": "*/*",
+            "accept-language": "en-US,en;q=0.9",
+            "sec-ch-prefers-color-scheme": self.preferred_color_scheme,
+            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
+            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
+            "sec-ch-ua-mobile": "?0",
+            "sec-ch-ua-platform": "\"Windows\"",
+            "sec-ch-ua-platform-version": "\"15.0.0\"",
+            "sec-fetch-dest": "empty",
+            "sec-fetch-mode": "cors",
+            "sec-fetch-site": "same-origin",
+            "viewport-width": "1475",
+            "x-asbd-id": "198387",
+            "x-csrftoken": self.csrf_token,
+            "x-ig-app-id": self.insta_app_id,
+            "x-ig-www-claim": self.x_ig_www_claim,
+            "x-requested-with": "XMLHttpRequest",
+            "Referer": "https://www.instagram.com/accounts/edit/",
+            "Referrer-Policy": "strict-origin-when-cross-origin"
+        }
+        http_response = self.request_session.get("https://www.instagram.com/api/v1/accounts/edit/web_form_data/", headers=request_headers)
+
+        try:
+            http_response.json()
+            return True
+        except JSONDecodeError:
+            return False
+
+    def follow(self, identifier: str | int) -> FollowedStatus | None:
+        conversion_success, identifier = self._identifier(identifier, UID)
+        if not conversion_success: return None
+
+        # Actual Request
+        refresh_csrf_token(self)
+        body_json = {
+            "container_module": "profile",
+            "nav_chain": f"PolarisProfileRoot:profilePage:1:via_cold_start",
+            "user_id": identifier
+        }
+        request_headers = {
+            "accept": "*/*",
+            "accept-language": "en-US,en;q=0.9",
+            "content-type": "application/x-www-form-urlencoded",
+            "sec-ch-prefers-color-scheme": self.preferred_color_scheme,
+            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
+            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
+            "sec-ch-ua-mobile": "?0",
+            "sec-ch-ua-platform": "\"Windows\"",
+            "sec-ch-ua-platform-version": "\"15.0.0\"",
+            "sec-fetch-dest": "empty",
+            "sec-fetch-mode": "cors",
+            "sec-fetch-site": "same-origin",
+            "viewport-width": "1475",
+            "x-asbd-id": "198387",
+            "x-csrftoken": self.csrf_token,
+            "x-ig-app-id": self.insta_app_id,
+            "x-ig-www-claim": self.x_ig_www_claim,
+            "x-instagram-ajax": "1007616494",
+            "x-requested-with": "XMLHttpRequest",
+            "Referer": f"https://www.instagram.com/{''.join(random.choices(string.ascii_lowercase, k=5))}/",
+            "Referrer-Policy": "strict-origin-when-cross-origin"
+        }
+
+        try:
+            http_response = self.request_session.post(f"https://www.instagram.com/api/v1/friendships/create/{identifier}/", headers=request_headers, data=body_json)
+            response_json = http_response.json()
+
+            if "status" in response_json:
+                if response_json["status"] == "ok" and "friendship_status" in response_json:
+                    if "following" in response_json["friendship_status"] \
+                            and "outgoing_request" in response_json["friendship_status"] \
+                            and "followed_by" in response_json["friendship_status"] \
+                            and "previous_following" in response_json:
+                        return FollowedStatus(
+                            following=response_json["friendship_status"]["following"],
+                            follow_requested=response_json["friendship_status"]["outgoing_request"],
+                            is_my_follower=response_json["friendship_status"]["followed_by"],
+                            previous_following=response_json["previous_following"]
+                        )
+        except JSONDecodeError:
+            return None
+
+    def unfollow(self, identifier: str | int) -> UnfollowedStatus | None:
+        conversion_success, identifier = self._identifier(identifier, UID)
+        if not conversion_success: return None
+
+        # Actual Request
+        refresh_csrf_token(self)
+        body_json = {
+            "container_module": "profile",
+            "nav_chain": f"PolarisProfileRoot:profilePage:1:via_cold_start",
+            "user_id": identifier
+        }
+        request_headers = {
+            "accept": "*/*",
+            "accept-language": "en-US,en;q=0.9",
+            "content-type": "application/x-www-form-urlencoded",
+            "sec-ch-prefers-color-scheme": self.preferred_color_scheme,
+            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
+            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
+            "sec-ch-ua-mobile": "?0",
+            "sec-ch-ua-platform": "\"Windows\"",
+            "sec-ch-ua-platform-version": "\"15.0.0\"",
+            "sec-fetch-dest": "empty",
+            "sec-fetch-mode": "cors",
+            "sec-fetch-site": "same-origin",
+            "viewport-width": "1475",
+            "x-asbd-id": "198387",
+            "x-csrftoken": self.csrf_token,
+            "x-ig-app-id": self.insta_app_id,
+            "x-ig-www-claim": self.x_ig_www_claim,
+            "x-instagram-ajax": "1007616494",
+            "x-requested-with": "XMLHttpRequest",
+            "Referer": f"https://www.instagram.com/{''.join(random.choices(string.ascii_lowercase, k=6))}/",
+            "Referrer-Policy": "strict-origin-when-cross-origin"
+        }
+
+        try:
+            http_response = self.request_session.post(f"https://www.instagram.com/api/v1/friendships/destroy/{identifier}/", headers=request_headers, data=body_json)
+            response_json = http_response.json()
+
+            if "status" in response_json:
+                if response_json["status"] == "ok" and "friendship_status" in response_json:
+                    if "following" in response_json["friendship_status"] \
+                            and "outgoing_request" in response_json["friendship_status"] \
+                            and "followed_by" in response_json["friendship_status"]:
+                        return UnfollowedStatus(
+                            unfollowed=not response_json["friendship_status"]["following"] and not response_json["friendship_status"]["outgoing_request"],
+                            is_my_follower=response_json["friendship_status"]["followed_by"]
+                        )
+        except JSONDecodeError:
+            return None
+
+    def followers(self, identifier: str | int, count: int = 0) -> Generator[FollowPerson, None, None]:
+        conversion_success, identifier = self._identifier(identifier, UID)
+        if not conversion_success:
+            yield None
+            return None
+
+        # Actual Request
+        refresh_csrf_token(self)
+        request_headers: dict = {
+            "accept": "*/*",
+            "accept-language": "en-US,en;q=0.9",
+            "sec-ch-prefers-color-scheme": self.preferred_color_scheme,
+            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
+            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
+            "sec-ch-ua-mobile": "?0",
+            "sec-ch-ua-platform": "\"Windows\"",
+            "sec-ch-ua-platform-version": "\"15.0.0\"",
+            "sec-fetch-dest": "empty",
+            "sec-fetch-mode": "cors",
+            "sec-fetch-site": "same-origin",
+            "viewport-width": "1475",
+            "x-asbd-id": "198387",
+            "x-csrftoken": self.csrf_token,
+            "x-ig-app-id": self.insta_app_id,
+            "x-ig-www-claim": self.x_ig_www_claim,
+            "x-requested-with": "XMLHttpRequest",
+            "Referer": f"https://www.instagram.com/{''.join(random.choices(string.ascii_lowercase, k=6))}/followers/",
+            "Referrer-Policy": "strict-origin-when-cross-origin"
+        }
+
+        current_max_id: str = ""
+        generated_count: int = 0
+
+        while True:
+            current_max_id_text: str = ""
+
+            if current_max_id != "":
+                current_max_id_text: str = f"&max_id={current_max_id}"
+
+            try:
+                count_text = 35
+
+                if count < 35:
+                    count_text = count
+
+                http_response = self.request_session.get(f"https://www.instagram.com/api/v1/friendships/{identifier}/followers/?count={str(count_text)}{current_max_id_text}&search_surface=follow_list_page", headers=request_headers)
+                response_json = http_response.json()
+
+                if "status" not in response_json or "users" not in response_json:
+                    yield None
+                    return None
+
+                if response_json["status"] != "ok":
+                    yield None
+                    return None
+
+                for each_item in response_json["users"]:
+                    if generated_count < count or count == 0:
+
+                        try:
+                            yield FollowPerson(
+                                has_anonymous_profile_picture=each_item["has_anonymous_profile_picture"],
+                                user_id=each_item["pk"],
+                                username=each_item["username"],
+                                full_name=each_item["full_name"],
+                                is_private=each_item["is_private"],
+                                is_verified=each_item["is_verified"],
+                                profile_picture_url=each_item["profile_pic_url"],
+                                badges=each_item["account_badges"],
+                                third_party_downloads_enabled=each_item["third_party_downloads_enabled"],
+                                is_possible_scammer=each_item["is_possible_scammer"]
+                            )
+
+                        except KeyError:
+                            raise APIError()
+
+                        generated_count += 1
+
+                if (generated_count < count or count == 0) and "next_max_id" in response_json:
+                    current_max_id = response_json["next_max_id"]
+                else:
+                    return None
+            except JSONDecodeError:
+                yield None
+                return None
+
+    def followings(self, identifier: str | int, count: int = 0) -> Generator[FollowPerson, None, None]:
+        conversion_success, identifier = self._identifier(identifier, UID)
+        if not conversion_success:
+            yield None
+            return None
+
+        # Actual Request
+        refresh_csrf_token(self)
+        request_headers = {
+            "accept": "*/*",
+            "accept-language": "en-US,en;q=0.9",
+            "sec-ch-prefers-color-scheme": self.preferred_color_scheme,
+            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
+            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
+            "sec-ch-ua-mobile": "?0",
+            "sec-ch-ua-platform": "\"Windows\"",
+            "sec-ch-ua-platform-version": "\"15.0.0\"",
+            "sec-fetch-dest": "empty",
+            "sec-fetch-mode": "cors",
+            "sec-fetch-site": "same-origin",
+            "viewport-width": "1475",
+            "x-asbd-id": "198387",
+            "x-csrftoken": self.csrf_token,
+            "x-ig-app-id": self.insta_app_id,
+            "x-ig-www-claim": self.x_ig_www_claim,
+            "x-requested-with": "XMLHttpRequest",
+            "Referer": f"https://www.instagram.com/{''.join(random.choices(string.ascii_lowercase, k=6))}/following/",
+            "Referrer-Policy": "strict-origin-when-cross-origin"
+        }
+
+        current_max_id = ""
+        generated_count = 0
+
+        while True:
+            current_max_id_text = ""
+
+            if current_max_id != "":
+                current_max_id_text = f"&max_id={current_max_id}"
+
+            try:
+                count_text = 35
+
+                if count < 35:
+                    count_text = count
+
+                http_response = self.request_session.get(
+                    f"https://www.instagram.com/api/v1/friendships/{identifier}/following/?count={str(count_text)}{current_max_id_text}",
+                    headers=request_headers)
+                response_json = http_response.json()
+
+                if "status" not in response_json or "users" not in response_json:
+                    yield None
+                    return None
+
+                if response_json["status"] != "ok":
+                    yield None
+                    return None
+
+                for each_item in response_json["users"]:
+                    if generated_count < count or count == 0:
+
+                        try:
+                            yield FollowPerson(
+                                has_anonymous_profile_picture=each_item["has_anonymous_profile_picture"],
+                                user_id=each_item["pk"],
+                                username=each_item["username"],
+                                full_name=each_item["full_name"],
+                                is_private=each_item["is_private"],
+                                is_verified=each_item["is_verified"],
+                                profile_picture_url=each_item["profile_pic_url"],
+                                is_possible_scammer=each_item["is_possible_scammer"]
+                            )
+
+                        except KeyError:
+                            raise APIError()
+
+                        generated_count += 1
+
+                if (generated_count < count or count == 0) and "next_max_id" in response_json:
+                    current_max_id = response_json["next_max_id"]
+                else:
+                    return None
+            except JSONDecodeError:
+                yield None
+                return None
+
+    def _identifier(self, identifier: str | int, required: str | int):
+        identifier = format_identifier(identifier)
+
+        if len(identifier) <= 0:
+            raise IdentifierError("No identifier was given. Please pass either UserId or Username as an argument.")
+
+        # Identifier: Username or UID?
+        is_username = False
+        for letter in identifier:
+            if letter not in string.digits:
+                is_username = True
+                break
+
+        if is_username and required == USERNAME:
+            return True, identifier
+
+        elif is_username and required == UID:
+            user_id = self.guest.get_uid(identifier)
+
+            if user_id is not None and user_id != "":
+                return True, user_id
+            else:
+                return False, None
+
+        elif not is_username and required == USERNAME:
+            username = self.guest.get_username(identifier)
+
+            if username is not None and username != "":
+                return True, username
+            else:
+                return False, None
+
+        elif not is_username and required == UID:
+            return True, identifier
+
+        else:
+            raise DevelopmentError("Identifier Conversion (Else Block)")
+
+    def _set_account_privacy(self, privacy: str) -> bool:
+        is_private = (privacy == "private")
+
+        if privacy != "private" and privacy != "public":
+            raise DevelopmentError("_set_account_privacy")
+
+        refresh_csrf_token(self)
+        body_json = {
+            "is_private": is_private
+        }
+        request_headers = {
+            "accept": "*/*",
+            "accept-language": "en-US,en;q=0.9",
+            "content-type": "application/x-www-form-urlencoded",
+            "sec-ch-prefers-color-scheme": self.preferred_color_scheme,
+            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
+            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
+            "sec-ch-ua-mobile": "?0",
+            "sec-ch-ua-platform": "\"Windows\"",
+            "sec-ch-ua-platform-version": "\"15.0.0\"",
+            "sec-fetch-dest": "empty",
+            "sec-fetch-mode": "cors",
+            "sec-fetch-site": "same-origin",
+            "viewport-width": "1475",
+            "x-asbd-id": "198387",
+            "x-csrftoken": self.csrf_token,
+            "x-ig-app-id": self.insta_app_id,
+            "x-ig-www-claim": self.x_ig_www_claim,
+            "x-instagram-ajax": "1007616494",
+            "x-requested-with": "XMLHttpRequest",
+            "Referer": "https://www.instagram.com/accounts/who_can_see_your_content/",
+            "Referrer-Policy": "strict-origin-when-cross-origin"
+        }
+
+        try:
+            http_response = self.request_session.post("https://www.instagram.com/api/v1/web/accounts/set_private/", headers=request_headers, data=body_json)
+            response_json = http_response.json()
+
+            if "status" not in response_json:
+                return False
+
+            if response_json["status"] != "ok":
+                return False
+
+            return True
+        except JSONDecodeError:
+            return False
+
+    def switch_to_private_account(self) -> bool:
+        return self._set_account_privacy("private")
+
+    def switch_to_public_account(self) -> bool:
+        return self._set_account_privacy("public")
+
+    def profile(self, username: str) -> ProfileHost | None:
+        return self.guest.profile(username, __session__=self.request_session)
+
+    def get_username(self, uid: str | int) -> str | None:
+        return self.guest.get_username(uid, __session__=self.request_session)
+
+    def posts(self, username: str, count: int = 0) -> Generator[Post, None, None]:
+        username = format_username(username)
+
+        refresh_csrf_token(self)
+        request_headers = {
+            "accept": "*/*",
+            "accept-language": "en-US,en;q=0.9",
+            "sec-ch-prefers-color-scheme": self.preferred_color_scheme,
+            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
+            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.110\", \"Google Chrome\";v=\"114.0.5735.110\"",
+            "sec-ch-ua-mobile": "?0",
+            "sec-ch-ua-platform": "\"Windows\"",
+            "sec-ch-ua-platform-version": "\"15.0.0\"",
+            "sec-fetch-dest": "empty",
+            "sec-fetch-mode": "cors",
+            "sec-fetch-site": "same-origin",
+            "viewport-width": "1475",
+            "x-asbd-id": "129477",
+            "x-csrftoken": self.csrf_token,
+            "x-ig-app-id": self.insta_app_id,
+            "x-ig-www-claim": self.x_ig_www_claim,
+            "x-requested-with": "XMLHttpRequest",
+            "Referer": f"https://www.instagram.com/{username}/",
+            "Referrer-Policy": "strict-origin-when-cross-origin"
+        }
+
+        current_max_id = ""
+        generated_count = 0
+
+        while True:
+            current_max_id_text = ""
+
+            if current_max_id != "":
+                current_max_id_text = f"&max_id={current_max_id}"
+
+            try:
+                count_text = 35
+
+                if count < 35:
+                    count_text = count
+
+                http_response = self.request_session.get(f"https://www.instagram.com/api/v1/feed/user/{username}/username/?count={count_text}{current_max_id_text}", headers=request_headers)
+                response_json = http_response.json()
+
+                if "status" not in response_json or "items" not in response_json:
+                    yield None
+                    return None
+
+                if response_json["status"] != "ok":
+                    yield None
+                    return None
+
+                for each_item in response_json["items"]:
+                    if generated_count < count or count == 0:
+
+                        yield self._process_post_data(each_item)
+                        generated_count += 1
+
+                if (generated_count < count or count == 0) and "next_max_id" in response_json:
+                    current_max_id = response_json["next_max_id"]
+                else:
+                    return None
+            except JSONDecodeError:
+                yield None
+                return None
+
+    def post(self, share_url: str) -> Post | None:
+        share_url: str = format_url(share_url)
+        request_headers = {
+            "accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
+            "accept-language": "en-US,en;q=0.9",
+            "cache-control": "max-age=0",
+            "sec-ch-prefers-color-scheme": "dark",
+            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
+            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.110\", \"Google Chrome\";v=\"114.0.5735.110\"",
+            "sec-ch-ua-mobile": "?0",
+            "sec-ch-ua-platform": "\"Windows\"",
+            "sec-ch-ua-platform-version": "\"15.0.0\"",
+            "sec-fetch-dest": "document",
+            "sec-fetch-mode": "navigate",
+            "sec-fetch-site": "same-origin",
+            "sec-fetch-user": "?1",
+            "upgrade-insecure-requests": "1",
+            "viewport-width": "1475",
+            "referrerPolicy": "strict-origin-when-cross-origin"
+        }
+
+        http_response = self.request_session.get(share_url, headers=request_headers)
+        response_text = http_response.text
+
+        required_text = "{\"response\":\"{\\\"items\\\":"
+
+        initial_index = response_text.rfind(required_text)
+        if initial_index == -1: raise APIError()
+
+        rest_text = response_text[initial_index - len(required_text) + len(required_text): len(response_text)]
+        end_text = "\\\"auto_load_more_enabled\\\":false}\",\"status_code\":200}"
+        end_index = rest_text.find(end_text)
+
+        try:
+            data: dict = json.loads(rest_text[:end_index + len(end_text)])
+
+            if "response" in data:
+                response_data: dict = json.loads(data["response"])
+
+                if "items" in response_data:
+                    items_data: list = response_data["items"]
+
+                    if len(items_data) > 0:
+                        selected_post: dict = items_data[len(items_data) - 1]
+
+                        if selected_post is not None:
+                            return self._process_post_data(selected_post)
+
+        except JSONDecodeError:
+            return None
+
+    def _process_post_data(self, data: dict) -> Post:
+
+        caption: dict = data.get("caption", None)
+
+        caption_text = ""
+        is_caption_covered = False
+        caption_created_at = 0
+        caption_share_enabled = False
+        caption_did_report_as_spam = False
+
+        if caption is not None:
+            caption_text = caption.get("text", "")
+            is_caption_covered = caption.get("is_covered", False)
+            caption_created_at = caption.get("created_at", 0)
+            caption_share_enabled = caption.get("share_enabled", False)
+            caption_did_report_as_spam = caption.get("did_report_as_spam", False)
+
+        user: PostUser = PostUser()
+        user_data: dict = data.get("user", None)
+
+        if user_data is not None:
+            user: PostUser = PostUser(
+                has_anonymous_profile_picture=user_data.get("has_anonymous_profile_picture", False),
+                fbid_v2=user_data.get("fbid_v2", ""),
+                transparency_product_enabled=user_data.get("transparency_product_enabled", False),
+                is_favorite=user_data.get("is_favorite", False),
+                is_unpublished=user_data.get("is_unpublished", False),
+                uid=user_data.get("pk", ""),
+                username=user_data.get("username", ""),
+                full_name=user_data.get("full_name", ""),
+                is_private=user_data.get("is_private", False),
+                is_verified=user_data.get("is_verified", False),
+                profile_picture_id=user_data.get("profile_pic_id", ""),
+                profile_picture_url=user_data.get("profile_pic_url", ""),
+                account_badges=user_data.get("account_badges", []),
+                feed_post_reshare_disabled=user_data.get("feed_post_reshare_disabled", False),
+                show_account_transparency_details=user_data.get("show_account_transparency_details", False),
+                third_party_downloads_enabled=user_data.get("third_party_downloads_enabled", 0),
+                latest_reel_media=user_data.get("latest_reel_media", 0)
+            )
+
+        return Post(
+            instance=self,
+            share_url=f"https://www.instagram.com/p/{data.get('code', '')}",
+            taken_at=data.get("taken_at", 0),
+            unique_key=data.get("pk", ""),
+            media_type=data.get("media_type", 0),
+            code=data.get("code", ""),
+            caption_is_edited=data.get("caption_is_edited", False),
+            original_media_has_visual_reply_media=data.get("original_media_has_visual_reply_media", False),
+            like_and_view_counts_disabled=data.get("like_and_view_counts_disabled", False),
+            can_viewer_save=data.get("can_viewer_save", False),
+            profile_grid_control_enabled=data.get("profile_grid_control_enabled", False),
+            is_comments_gif_composer_enabled=data.get("is_comments_gif_composer_enabled", False),
+            comment_threading_enabled=data.get("comment_threading_enabled", False),
+            comment_count=data.get("comment_count", 0),
+            has_liked=data.get("has_liked", False),
+            user=user,
+            can_viewer_reshare=data.get("can_viewer_reshare", False),
+            like_count=data.get("like_count", 0),
+            top_likers=data.get("top_likers", []),
+            caption_text=caption_text,
+            is_caption_covered=is_caption_covered,
+            caption_created_at=caption_created_at,
+            caption_share_enabled=caption_share_enabled,
+            caption_did_report_as_spam=caption_did_report_as_spam,
+            is_paid_partnership=data.get("is_paid_partnership", False),
+            show_shop_entrypoint=data.get("show_shop_entrypoint", False),
+            deleted_reason=data.get("deleted_reason", 0),
+            integrity_review_decision=data.get("integrity_review_decision", ""),
+            ig_media_sharing_disabled=data.get("ig_media_sharing_disabled", False),
+            has_shared_to_fb=data.get("has_shared_to_fb", False),
+            is_unified_video=data.get("is_unified_video", False),
+            should_request_ads=data.get("should_request_ads", False),
+            is_visual_reply_commenter_notice_enabled=data.get("is_visual_reply_commenter_notice_enabled", False),
+            commerciality_status=data.get("commerciality_status", ""),
+            explore_hide_comments=data.get("explore_hide_comments", False),
+            has_delayed_metadata=data.get("has_delayed_metadata", False),
+            location_latitude=data.get("lat", 0),
+            location_longitude=data.get("lng", 0)
+        )
```

### Comparing `ensta-2.6/ensta/containers/Post.py` & `ensta-2.7/ensta/containers/Post.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,92 +1,91 @@
-from ensta.containers import PostUser
-from dataclasses import dataclass, field
-from ensta import Host
-from ensta.lib.Commons import refresh_csrf_token
-from json import JSONDecodeError
-
-
-@dataclass(frozen=False)
-class Post:
-    _instance: type[Host] | None = None
-    share_url: str = ""
-    taken_at: int = 0
-    unique_key: str = ""
-    media_type: int = 0
-    code: str = ""
-    caption_is_edited: bool = False
-    original_media_has_visual_reply_media: bool = False
-    like_and_view_counts_disabled: bool = False
-    can_viewer_save: bool = False
-    profile_grid_control_enabled: bool = False
-    is_comments_gif_composer_enabled: bool = False
-    comment_threading_enabled: bool = False
-    comment_count: int = 0
-    has_liked: bool = False
-    user: PostUser = field(default_factory=PostUser)
-    can_viewer_reshare: bool = False
-    like_count: int = 0
-    top_likers: list[str] = field(default_factory=list)
-    caption_text: str = ""
-    is_caption_covered: bool = False
-    caption_created_at: int = 0
-    caption_share_enabled: bool = False
-    caption_did_report_as_spam: bool = False
-    is_paid_partnership: bool = False
-    show_shop_entrypoint: bool = False
-    deleted_reason: int = 0
-    integrity_review_decision: str = ""
-    ig_media_sharing_disabled: bool = False
-    has_shared_to_fb: int = 0
-    is_unified_video: bool = False
-    should_request_ads: bool = False
-    is_visual_reply_commenter_notice_enabled: bool = False
-    commerciality_status: str = ""
-    explore_hide_comments: bool = False
-    has_delayed_metadata: bool = False
-    location_latitude: float = 0
-    location_longitude: float = 0
-
-    def _like_action(self, action: str = "like") -> bool:
-        if self.unique_key == "": return False
-
-        refresh_csrf_token(self._instance)
-        request_headers = {
-            "accept": "*/*",
-            "accept-language": "en-US,en;q=0.9",
-            "content-type": "application/x-www-form-urlencoded",
-            "sec-ch-prefers-color-scheme": self._instance.preferred_color_scheme,
-            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
-            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.110\", \"Google Chrome\";v=\"114.0.5735.110\"",
-            "sec-ch-ua-mobile": "?0",
-            "sec-ch-ua-platform": "\"Windows\"",
-            "sec-ch-ua-platform-version": "\"15.0.0\"",
-            "sec-fetch-dest": "empty",
-            "sec-fetch-mode": "cors",
-            "sec-fetch-site": "same-origin",
-            "viewport-width": "1475",
-            "x-asbd-id": "129477",
-            "x-csrftoken": self._instance.csrf_token,
-            "x-ig-app-id": self._instance.insta_app_id,
-            "x-ig-www-claim": self._instance.x_ig_www_claim,
-            "x-instagram-ajax": "1007670408",
-            "x-requested-with": "XMLHttpRequest",
-            "Referer": f"https://www.instagram.com/p/{self.code}/",
-            "Referrer-Policy": "strict-origin-when-cross-origin"
-        }
-
-        try:
-            http_response = self._instance.request_session.post(f"https://www.instagram.com/api/v1/web/likes/{self.unique_key}/{action}/", headers=request_headers)
-            response_json = http_response.json()
-
-            if "status" in response_json:
-                return response_json["status"] == "ok"
-            else:
-                return False
-        except JSONDecodeError:
-            return False
-
-    def like(self) -> bool:
-        return self._like_action("like")
-
-    def unlike(self) -> bool:
-        return self._like_action("unlike")
+from ensta.containers import PostUser
+from dataclasses import dataclass, field
+from ensta.lib.Commons import refresh_csrf_token
+from json import JSONDecodeError
+
+
+@dataclass(frozen=False)
+class Post:
+    instance: any = None
+    share_url: str = ""
+    taken_at: int = 0
+    unique_key: str = ""
+    media_type: int = 0
+    code: str = ""
+    caption_is_edited: bool = False
+    original_media_has_visual_reply_media: bool = False
+    like_and_view_counts_disabled: bool = False
+    can_viewer_save: bool = False
+    profile_grid_control_enabled: bool = False
+    is_comments_gif_composer_enabled: bool = False
+    comment_threading_enabled: bool = False
+    comment_count: int = 0
+    has_liked: bool = False
+    user: PostUser = field(default_factory=PostUser)
+    can_viewer_reshare: bool = False
+    like_count: int = 0
+    top_likers: list[str] = field(default_factory=list)
+    caption_text: str = ""
+    is_caption_covered: bool = False
+    caption_created_at: int = 0
+    caption_share_enabled: bool = False
+    caption_did_report_as_spam: bool = False
+    is_paid_partnership: bool = False
+    show_shop_entrypoint: bool = False
+    deleted_reason: int = 0
+    integrity_review_decision: str = ""
+    ig_media_sharing_disabled: bool = False
+    has_shared_to_fb: int = 0
+    is_unified_video: bool = False
+    should_request_ads: bool = False
+    is_visual_reply_commenter_notice_enabled: bool = False
+    commerciality_status: str = ""
+    explore_hide_comments: bool = False
+    has_delayed_metadata: bool = False
+    location_latitude: float = 0
+    location_longitude: float = 0
+
+    def _like_action(self, action: str = "like") -> bool:
+        if self.unique_key == "": return False
+
+        refresh_csrf_token(self.instance)
+        request_headers = {
+            "accept": "*/*",
+            "accept-language": "en-US,en;q=0.9",
+            "content-type": "application/x-www-form-urlencoded",
+            "sec-ch-prefers-color-scheme": self.instance.preferred_color_scheme,
+            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
+            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.110\", \"Google Chrome\";v=\"114.0.5735.110\"",
+            "sec-ch-ua-mobile": "?0",
+            "sec-ch-ua-platform": "\"Windows\"",
+            "sec-ch-ua-platform-version": "\"15.0.0\"",
+            "sec-fetch-dest": "empty",
+            "sec-fetch-mode": "cors",
+            "sec-fetch-site": "same-origin",
+            "viewport-width": "1475",
+            "x-asbd-id": "129477",
+            "x-csrftoken": self.instance.csrf_token,
+            "x-ig-app-id": self.instance.insta_app_id,
+            "x-ig-www-claim": self.instance.x_ig_www_claim,
+            "x-instagram-ajax": "1007670408",
+            "x-requested-with": "XMLHttpRequest",
+            "Referer": f"https://www.instagram.com/p/{self.code}/",
+            "Referrer-Policy": "strict-origin-when-cross-origin"
+        }
+
+        try:
+            http_response = self.instance.request_session.post(f"https://www.instagram.com/api/v1/web/likes/{self.unique_key}/{action}/", headers=request_headers)
+            response_json = http_response.json()
+
+            if "status" in response_json:
+                return response_json["status"] == "ok"
+            else:
+                return False
+        except JSONDecodeError:
+            return False
+
+    def like(self) -> bool:
+        return self._like_action("like")
+
+    def unlike(self) -> bool:
+        return self._like_action("unlike")
```

### Comparing `ensta-2.6/ensta/containers/PostUser.py` & `ensta-2.7/ensta/containers/PostUser.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from dataclasses import dataclass, field
-
-
-@dataclass(frozen=False)
-class PostUser:
-    has_anonymous_profile_picture: bool = False
-    fbid_v2: str = ""
-    transparency_product_enabled: bool = False
-    is_favorite: bool = False
-    is_unpublished: bool = False
-    uid: str = ""
-    username: str = ""
-    full_name: str = ""
-    is_private: bool = False
-    is_verified: bool = False
-    profile_picture_id: str = ""
-    profile_picture_url: str = ""
-    account_badges: list = field(default_factory=list)
-    feed_post_reshare_disabled: bool = False
-    show_account_transparency_details: bool = False
-    third_party_downloads_enabled: int = 0
-    latest_reel_media: int = 0
+from dataclasses import dataclass, field
+
+
+@dataclass(frozen=False)
+class PostUser:
+    has_anonymous_profile_picture: bool = False
+    fbid_v2: str = ""
+    transparency_product_enabled: bool = False
+    is_favorite: bool = False
+    is_unpublished: bool = False
+    uid: str = ""
+    username: str = ""
+    full_name: str = ""
+    is_private: bool = False
+    is_verified: bool = False
+    profile_picture_id: str = ""
+    profile_picture_url: str = ""
+    account_badges: list = field(default_factory=list)
+    feed_post_reshare_disabled: bool = False
+    show_account_transparency_details: bool = False
+    third_party_downloads_enabled: int = 0
+    latest_reel_media: int = 0
```

### Comparing `ensta-2.6/ensta/lib/Commons.py` & `ensta-2.7/ensta/lib/Commons.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-import string
-import requests
-import requests.cookies
-import random
-from requests.cookies import RequestsCookieJar
-from .Exceptions import NetworkError
-
-
-def update_app_id(self) -> None:
-    app_id_occurrence_string = "\"APP_ID\":\""
-    app_id_first_occurrence = self.homepage_source.index(app_id_occurrence_string)
-    app_id_raw_text = self.homepage_source[
-                      app_id_first_occurrence + len(app_id_occurrence_string): app_id_first_occurrence + 30]
-    self.insta_app_id = app_id_raw_text[: app_id_raw_text.index("\"")]
-
-
-def refresh_csrf_token(self) -> None:
-    self.csrf_token = "".join(random.choices(string.ascii_letters + string.digits, k=32))
-
-    cookie_jar: RequestsCookieJar = self.request_session.cookies
-    cookies = list(cookie_jar.items())
-    cookie_jar.clear()
-    final_cookies = {}
-
-    for key, value in cookies:
-        final_cookies[key] = value
-
-    final_cookies["csrftoken"] = self.csrf_token
-
-    for key in final_cookies:
-        cookie_jar.set(key, final_cookies[key])
-
-
-def update_session(self) -> None:
-    self.request_session = requests.Session()
-
-
-def update_homepage_source(self) -> None:
-    request_headers = {
-        "accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
-        "accept-language": "en-US,en;q=0.9",
-        "sec-ch-prefers-color-scheme": random.choice(["light", "dark"]),
-        "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
-        "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.110\", \"Google Chrome\";v=\"114.0.5735.110\"",
-        "sec-ch-ua-mobile": "?0",
-        "sec-ch-ua-platform": "\"Windows\"",
-        "sec-ch-ua-platform-version": "\"15.0.0\"",
-        "sec-fetch-dest": "document",
-        "sec-fetch-mode": "navigate",
-        "sec-fetch-site": "none",
-        "sec-fetch-user": "?1",
-        "upgrade-insecure-requests": "1",
-        "viewport-width": "1475",
-        "Referrer-Policy": "strict-origin-when-cross-origin"
-    }
-    temp_homepage_source = requests.get("https://www.instagram.com/", headers=request_headers).text.strip()
-
-    if temp_homepage_source != "":
-        self.homepage_source = temp_homepage_source
-    else:
-        raise NetworkError("Couldn't load instagram homepage.")
-
-
-def format_username(username: str) -> str:
-    return username.replace(" ", "").lower()
-
-
-def format_uid(uid: str) -> str:
-    return uid.replace(" ", "")
-
-
-def format_identifier(identifier: str | int) -> str:
-    return str(identifier).lower().replace(" ", "")
-
-
-def format_url(url: str) -> str:
-    return url.strip()
+import string
+import requests
+import requests.cookies
+import random
+from requests.cookies import RequestsCookieJar
+from .Exceptions import NetworkError
+
+
+def update_app_id(self) -> None:
+    app_id_occurrence_string = "\"APP_ID\":\""
+    app_id_first_occurrence = self.homepage_source.index(app_id_occurrence_string)
+    app_id_raw_text = self.homepage_source[
+                      app_id_first_occurrence + len(app_id_occurrence_string): app_id_first_occurrence + 30]
+    self.insta_app_id = app_id_raw_text[: app_id_raw_text.index("\"")]
+
+
+def refresh_csrf_token(self) -> None:
+    self.csrf_token = "".join(random.choices(string.ascii_letters + string.digits, k=32))
+
+    cookie_jar: RequestsCookieJar = self.request_session.cookies
+    cookies = list(cookie_jar.items())
+    cookie_jar.clear()
+    final_cookies = {}
+
+    for key, value in cookies:
+        final_cookies[key] = value
+
+    final_cookies["csrftoken"] = self.csrf_token
+
+    for key in final_cookies:
+        cookie_jar.set(key, final_cookies[key])
+
+
+def update_session(self) -> None:
+    self.request_session = requests.Session()
+
+
+def update_homepage_source(self) -> None:
+    request_headers = {
+        "accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
+        "accept-language": "en-US,en;q=0.9",
+        "sec-ch-prefers-color-scheme": random.choice(["light", "dark"]),
+        "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
+        "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.110\", \"Google Chrome\";v=\"114.0.5735.110\"",
+        "sec-ch-ua-mobile": "?0",
+        "sec-ch-ua-platform": "\"Windows\"",
+        "sec-ch-ua-platform-version": "\"15.0.0\"",
+        "sec-fetch-dest": "document",
+        "sec-fetch-mode": "navigate",
+        "sec-fetch-site": "none",
+        "sec-fetch-user": "?1",
+        "upgrade-insecure-requests": "1",
+        "viewport-width": "1475",
+        "Referrer-Policy": "strict-origin-when-cross-origin"
+    }
+    temp_homepage_source = requests.get("https://www.instagram.com/", headers=request_headers).text.strip()
+
+    if temp_homepage_source != "":
+        self.homepage_source = temp_homepage_source
+    else:
+        raise NetworkError("Couldn't load instagram homepage.")
+
+
+def format_username(username: str) -> str:
+    return username.replace(" ", "").lower()
+
+
+def format_uid(uid: str) -> str:
+    return uid.replace(" ", "")
+
+
+def format_identifier(identifier: str | int) -> str:
+    return str(identifier).lower().replace(" ", "")
+
+
+def format_url(url: str) -> str:
+    return url.strip()
```

### Comparing `ensta-2.6/ensta.egg-info/PKG-INFO` & `ensta-2.7/ensta.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-Metadata-Version: 2.1
-Name: ensta
-Version: 2.6
-Summary: 🔥 Fastest & Simplest Python Package For Instagram Automation
-Home-page: https://github.com/diezo/ensta
-Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v2.6.tar.gz
-Author: Deepak Soni
-Author-email: lonelycube@proton.me
-License: MIT
-Keywords: instagram-client,instagram,api-wrapper,instagram-scraper,instagram-api,instagram-sdk,instagram-photos,instagram-api-python,instabot,instagram-stories,instagram-bot,instapy,instagram-downloader,instagram-account,instagram-crawler,instagram-private-api,igtv,instagram-automation,reels,instagram-feed
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# 🤖 Ensta - Simple Instagram API
-[![PyPI](https://img.shields.io/pypi/v/ensta)](https://pypi.org/project/ensta)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ensta)]()
-[![Downloads](https://static.pepy.tech/badge/ensta)](https://pepy.tech/project/ensta)
-[![Twitter Share](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)](https://twitter.com/intent/tweet?text=Wow:&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)
-
-<img style="border-radius: 10px" src="https://imgtr.ee/images/2023/06/14/Twfd4.png"/>
-
-This package lets you use Instagram's Internal Web API through simple functions and classes. Ensta uses Instagram's Original Web API to scrape data which makes it a reliable choice over other third-party scrapers. This library mainly focuses on Simplicity & Reliability.
-
-Two type of classes are supported - ***Guest & Host***.
-
-[<img style="margin-top: 10px" src="https://www.buymeacoffee.com/assets/img/guidelines/download-assets-sm-1.svg" width="160"/>](https://buymeacoffee.com/diezo)
-
-## 📢 Announcement
-Users can now log in through their **Username** and **Password** to generate SessionId! [See this](https://github.com/diezo/ensta#:~:text=NewSessionID(%22username%22%2C%20%22password%22))
-
-## Installation
-To install this package using [Python's PIP](https://pypi.org/project/pip/), run this command in a terminal window:
-```shell
-$ pip install ensta
-```
-
-To update the existing package, run:
-```shell
-$ pip install ensta --upgrade
-```
-
-## 🧔🏻‍♂️ Guest Mode
-This mode doesn't require login and can be used to fetch publicly available data from Instagram's Servers. Following methods are supported till now:
-- Check if username is available for registration
-- Fetch someone's profile data
-- Convert username to userid
-- Convert userid to username
-
-Here's an example where an instance of *Guest Class* is created to fetch [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) profile information:
-
-```python
-from ensta import Guest
-
-guest = Guest()
-profile = guest.profile("cristiano")
-
-if profile is None:
-    print("Something went wrong.")
-else:
-    print(profile.biography)
-    print(profile.follower_count)
-    print(profile.following_count)
-```
-
-## 🧔🏻‍♂️ Host Mode
-Host mode requires login through SessionID, which should be passed as an argument during initialization.
-It can be used to take actions that require login. Additionally, users can manage their own profile through this class.
-
-These are the methods supported till now:
-- Check authentication status of the user
-- Follow/unfollow users
-- Fetch someone's follower/following list
-- Switch account type - 'Public' or 'Private'
-
-Here's an example where an instance of *Host Class* is created to follow [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) account:
-
-```python
-from ensta import Host, NewSessionID
-
-sessionid = NewSessionID("username", "password")
-
-host = Host(sessionid)
-status = host.follow("cristiano")
-
-if status is None:
-    print("Something went wrong.")
-else:
-    if status.following:
-        print("Following!")
-    
-    elif status.follow_requested:
-        print("Requested to follow!")
-```
-
-> ### **Note:**
-> When you create a new sessionid through *NewSessionID()*, it's recommended to save it somewhere, and use the same sessionid (instead of creating a new one each time you need) until it expires or becomes invalid.
->
-> This should be done to avoid unnecessary prolonged wait time while generating a new sessionid and also to prevent getting your account from getting flagged because of repetitive logins.
-
-## 📋 Remember
-Every function should return **None** on failure. So, it's recommended to add an *if statement* before using the actual data to avoid TypeErrors. Here's an example:
-```python
-from ensta import Guest
-
-guest = Guest()
-available = guest.username_availability("cristiano")
-
-if available is None:  # 'None' indicates failure
-    print("Something went wrong.")
-else:
-    print(available)
-```
-
-## ❤️ Donate
-If you wish to help me in the development of Ensta, consider donating:
-
-[<img src="https://www.buymeacoffee.com/assets/img/guidelines/download-assets-sm-1.svg" width="150"/>](https://buymeacoffee.com/diezo)
-
-## Disclaimer
-This is a third-party package, and not approved by Instagram. It doesn't promote illegal activities or activities that violate [Instagram's Community Guidelines](https://help.instagram.com/477434105621119/) such as spamming users, creating bot accounts, misusing data etc. You are solely responsible for all the actions you take using this package.
+Metadata-Version: 2.1
+Name: ensta
+Version: 2.7
+Summary: 🔥 Fastest & Simplest Python Package For Instagram Automation
+Home-page: https://github.com/diezo/ensta
+Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v2.7.tar.gz
+Author: Deepak Soni
+Author-email: lonelycube@proton.me
+License: MIT
+Keywords: instagram-client,instagram,api-wrapper,instagram-scraper,instagram-api,instagram-sdk,instagram-photos,instagram-api-python,instabot,instagram-stories,instagram-bot,instapy,instagram-downloader,instagram-account,instagram-crawler,instagram-private-api,igtv,instagram-automation,reels,instagram-feed
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# 🤖 Ensta - Simple Instagram API
+[![PyPI](https://img.shields.io/pypi/v/ensta)](https://pypi.org/project/ensta)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ensta)]()
+[![Downloads](https://static.pepy.tech/badge/ensta)](https://pepy.tech/project/ensta)
+[![Twitter Share](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)](https://twitter.com/intent/tweet?text=Wow:&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)
+
+<img style="border-radius: 10px" src="https://imgtr.ee/images/2023/06/14/Twfd4.png"/>
+
+This package lets you use Instagram's Internal Web API through simple functions and classes. Ensta uses Instagram's Original Web API to scrape data which makes it a reliable choice over other third-party scrapers. This library mainly focuses on Simplicity & Reliability.
+
+Two type of classes are supported - ***Guest & Host***.
+
+[<img style="margin-top: 10px" src="https://www.buymeacoffee.com/assets/img/guidelines/download-assets-sm-1.svg" width="160"/>](https://buymeacoffee.com/diezo)
+
+## 📢 Announcement
+Users can now log in through their **Username** and **Password** to generate SessionId! [See this](https://github.com/diezo/ensta#:~:text=NewSessionID(%22username%22%2C%20%22password%22))
+
+## Installation
+To install this package using [Python's PIP](https://pypi.org/project/pip/), run this command in a terminal window:
+```shell
+$ pip install ensta
+```
+
+To update the existing package, run:
+```shell
+$ pip install ensta --upgrade
+```
+
+## 🧔🏻‍♂️ Guest Mode
+This mode doesn't require login and can be used to fetch publicly available data from Instagram's Servers. Following methods are supported till now:
+- Check if username is available for registration
+- Fetch someone's profile data
+- Convert username to userid
+- Convert userid to username
+
+Here's an example where an instance of *Guest Class* is created to fetch [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) profile information:
+
+```python
+from ensta import Guest
+
+guest = Guest()
+profile = guest.profile("cristiano")
+
+if profile is None:
+    print("Something went wrong.")
+else:
+    print(profile.biography)
+    print(profile.follower_count)
+    print(profile.following_count)
+```
+
+## 🧔🏻‍♂️ Host Mode
+Host mode requires login through SessionID, which should be passed as an argument during initialization.
+It can be used to take actions that require login. Additionally, users can manage their own profile through this class.
+
+These are the methods supported till now:
+- Check authentication status of the user
+- Follow/unfollow users
+- Fetch someone's follower/following list
+- Switch account type - 'Public' or 'Private'
+
+Here's an example where an instance of *Host Class* is created to follow [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) account:
+
+```python
+from ensta import Host, NewSessionID
+
+sessionid = NewSessionID("username", "password")
+
+host = Host(sessionid)
+status = host.follow("cristiano")
+
+if status is None:
+    print("Something went wrong.")
+else:
+    if status.following:
+        print("Following!")
+    
+    elif status.follow_requested:
+        print("Requested to follow!")
+```
+
+> ### **Note:**
+> When you create a new sessionid through *NewSessionID()*, it's recommended to save it somewhere, and use the same sessionid (instead of creating a new one each time you need) until it expires or becomes invalid.
+>
+> This should be done to avoid unnecessary prolonged wait time while generating a new sessionid and also to prevent getting your account from getting flagged because of repetitive logins.
+
+## 📋 Remember
+Every function should return **None** on failure. So, it's recommended to add an *if statement* before using the actual data to avoid TypeErrors. Here's an example:
+```python
+from ensta import Guest
+
+guest = Guest()
+available = guest.username_availability("cristiano")
+
+if available is None:  # 'None' indicates failure
+    print("Something went wrong.")
+else:
+    print(available)
+```
+
+## ❤️ Donate
+If you wish to help me in the development of Ensta, consider donating:
+
+[<img src="https://www.buymeacoffee.com/assets/img/guidelines/download-assets-sm-1.svg" width="150"/>](https://buymeacoffee.com/diezo)
+
+## Disclaimer
+This is a third-party package, and not approved by Instagram. It doesn't promote illegal activities or activities that violate [Instagram's Community Guidelines](https://help.instagram.com/477434105621119/) such as spamming users, creating bot accounts, misusing data etc. You are solely responsible for all the actions you take using this package.
```

### Comparing `ensta-2.6/ensta.egg-info/SOURCES.txt` & `ensta-2.7/ensta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ensta-2.6/setup.py` & `ensta-2.7/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from distutils.core import setup
-from pathlib import Path
-
-long_description = (Path(__file__).parent / "README.md").read_text(encoding="utf-8")
-
-setup(
-    name="ensta",
-    packages=["ensta", "ensta.lib", "ensta.containers"],
-    version="2.6",
-    license="MIT",
-    description="🔥 Fastest & Simplest Python Package For Instagram Automation",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    author="Deepak Soni",
-    author_email="lonelycube@proton.me",
-    url="https://github.com/diezo/ensta",
-    download_url="https://github.com/diezo/ensta/archive/refs/tags/v2.6.tar.gz",
-    keywords=["instagram-client", "instagram", "api-wrapper", "instagram-scraper", "instagram-api", "instagram-sdk", "instagram-photos", "instagram-api-python", "instabot", "instagram-stories", "instagram-bot", "instapy", "instagram-downloader", "instagram-account", "instagram-crawler", "instagram-private-api", "igtv", "instagram-automation", "reels", "instagram-feed"],
-    install_requires=["requests", "selenium"],
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Intended Audience :: Developers",
-        "Topic :: Software Development :: Build Tools",
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.10"
-    ]
-)
+from distutils.core import setup
+from pathlib import Path
+
+long_description = (Path(__file__).parent / "README.md").read_text(encoding="utf-8")
+
+setup(
+    name="ensta",
+    packages=["ensta", "ensta.lib", "ensta.containers"],
+    version="2.7",
+    license="MIT",
+    description="🔥 Fastest & Simplest Python Package For Instagram Automation",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    author="Deepak Soni",
+    author_email="lonelycube@proton.me",
+    url="https://github.com/diezo/ensta",
+    download_url="https://github.com/diezo/ensta/archive/refs/tags/v2.7.tar.gz",
+    keywords=["instagram-client", "instagram", "api-wrapper", "instagram-scraper", "instagram-api", "instagram-sdk", "instagram-photos", "instagram-api-python", "instabot", "instagram-stories", "instagram-bot", "instapy", "instagram-downloader", "instagram-account", "instagram-crawler", "instagram-private-api", "igtv", "instagram-automation", "reels", "instagram-feed"],
+    install_requires=["requests", "selenium"],
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "Topic :: Software Development :: Build Tools",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.10"
+    ]
+)
```

