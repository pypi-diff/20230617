# Comparing `tmp/ensta-2.5.tar.gz` & `tmp/ensta-2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensta-2.5.tar", last modified: Thu Jun 15 14:36:48 2023, max compression
+gzip compressed data, was "ensta-2.6.tar", last modified: Sat Jun 17 09:36:53 2023, max compression
```

## Comparing `ensta-2.5.tar` & `ensta-2.6.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:36:48.465971 ensta-2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-15 14:36:30.000000 ensta-2.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-06-15 14:36:48.465971 ensta-2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-06-15 14:36:30.000000 ensta-2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:36:48.465971 ensta-2.5/ensta/
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-15 14:36:30.000000 ensta-2.5/ensta/Authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-06-15 14:36:30.000000 ensta-2.5/ensta/Guest.py
--rw-r--r--   0 runner    (1001) docker     (123)    19848 2023-06-15 14:36:30.000000 ensta-2.5/ensta/Host.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-15 14:36:30.000000 ensta-2.5/ensta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:36:48.465971 ensta-2.5/ensta/containers/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-15 14:36:30.000000 ensta-2.5/ensta/containers/FollowPerson.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-15 14:36:30.000000 ensta-2.5/ensta/containers/FollowedStatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-15 14:36:30.000000 ensta-2.5/ensta/containers/Profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-15 14:36:30.000000 ensta-2.5/ensta/containers/ProfileHost.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-15 14:36:30.000000 ensta-2.5/ensta/containers/UnfollowedStatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-15 14:36:30.000000 ensta-2.5/ensta/containers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:36:48.465971 ensta-2.5/ensta/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-15 14:36:30.000000 ensta-2.5/ensta/lib/Commons.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-15 14:36:30.000000 ensta-2.5/ensta/lib/Exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-15 14:36:30.000000 ensta-2.5/ensta/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:36:48.465971 ensta-2.5/ensta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-06-15 14:36:48.000000 ensta-2.5/ensta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-15 14:36:48.000000 ensta-2.5/ensta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:36:48.000000 ensta-2.5/ensta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 14:36:48.000000 ensta-2.5/ensta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 14:36:48.000000 ensta-2.5/ensta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-15 14:36:48.465971 ensta-2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-15 14:36:30.000000 ensta-2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 09:36:53.806376 ensta-2.6/
+-rw-rw-rw-   0        0        0     1081 2023-06-06 15:38:39.000000 ensta-2.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     5716 2023-06-17 09:36:53.806376 ensta-2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4710 2023-06-15 06:34:08.000000 ensta-2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 09:36:53.723050 ensta-2.6/ensta/
+-rw-rw-rw-   0        0        0     2566 2023-06-15 10:21:57.000000 ensta-2.6/ensta/Authentication.py
+-rw-rw-rw-   0        0        0     9955 2023-06-15 13:55:13.000000 ensta-2.6/ensta/Guest.py
+-rw-rw-rw-   0        0        0    30175 2023-06-16 16:47:35.000000 ensta-2.6/ensta/Host.py
+-rw-rw-rw-   0        0        0      136 2023-06-17 09:26:48.000000 ensta-2.6/ensta/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 09:36:53.771389 ensta-2.6/ensta/containers/
+-rw-rw-rw-   0        0        0      420 2023-06-15 10:26:52.000000 ensta-2.6/ensta/containers/FollowPerson.py
+-rw-rw-rw-   0        0        0      222 2023-06-09 08:46:48.000000 ensta-2.6/ensta/containers/FollowedStatus.py
+-rw-rw-rw-   0        0        0     3702 2023-06-16 16:54:33.000000 ensta-2.6/ensta/containers/Post.py
+-rw-rw-rw-   0        0        0      703 2023-06-16 15:13:40.000000 ensta-2.6/ensta/containers/PostUser.py
+-rw-rw-rw-   0        0        0     1074 2023-06-15 13:41:12.000000 ensta-2.6/ensta/containers/Profile.py
+-rw-rw-rw-   0        0        0      467 2023-06-15 13:54:39.000000 ensta-2.6/ensta/containers/ProfileHost.py
+-rw-rw-rw-   0        0        0      153 2023-06-09 08:28:13.000000 ensta-2.6/ensta/containers/UnfollowedStatus.py
+-rw-rw-rw-   0        0        0      256 2023-06-16 12:04:09.000000 ensta-2.6/ensta/containers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 09:36:53.797029 ensta-2.6/ensta/lib/
+-rw-rw-rw-   0        0        0     2776 2023-06-16 09:56:28.000000 ensta-2.6/ensta/lib/Commons.py
+-rw-rw-rw-   0        0        0     1008 2023-06-15 09:37:02.000000 ensta-2.6/ensta/lib/Exceptions.py
+-rw-rw-rw-   0        0        0      360 2023-06-15 09:37:20.000000 ensta-2.6/ensta/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 09:36:53.747084 ensta-2.6/ensta.egg-info/
+-rw-rw-rw-   0        0        0     5716 2023-06-17 09:36:53.000000 ensta-2.6/ensta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      570 2023-06-17 09:36:53.000000 ensta-2.6/ensta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 09:36:53.000000 ensta-2.6/ensta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-17 09:36:53.000000 ensta-2.6/ensta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-17 09:36:53.000000 ensta-2.6/ensta.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-17 09:36:53.810031 ensta-2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1402 2023-06-17 09:35:02.000000 ensta-2.6/setup.py
```

### Comparing `ensta-2.5/LICENSE.txt` & `ensta-2.6/LICENSE.txt`

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

### Comparing `ensta-2.5/PKG-INFO` & `ensta-2.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-Metadata-Version: 2.1
-Name: ensta
-Version: 2.5
-Summary: 🔥 Fastest & Simplest Python Package For Instagram Automation
-Home-page: https://github.com/diezo/ensta
-Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v2.5.tar.gz
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
+Version: 2.6
+Summary: 🔥 Fastest & Simplest Python Package For Instagram Automation
+Home-page: https://github.com/diezo/ensta
+Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v2.6.tar.gz
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

### Comparing `ensta-2.5/README.md` & `ensta-2.6/README.md`

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

### Comparing `ensta-2.5/ensta/Guest.py` & `ensta-2.6/ensta/Guest.py`

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

### Comparing `ensta-2.5/ensta/lib/Commons.py` & `ensta-2.6/ensta/lib/Commons.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,73 +1,77 @@
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

### Comparing `ensta-2.5/ensta.egg-info/PKG-INFO` & `ensta-2.6/ensta.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-Metadata-Version: 2.1
-Name: ensta
-Version: 2.5
-Summary: 🔥 Fastest & Simplest Python Package For Instagram Automation
-Home-page: https://github.com/diezo/ensta
-Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v2.5.tar.gz
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
+Version: 2.6
+Summary: 🔥 Fastest & Simplest Python Package For Instagram Automation
+Home-page: https://github.com/diezo/ensta
+Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v2.6.tar.gz
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

### Comparing `ensta-2.5/ensta.egg-info/SOURCES.txt` & `ensta-2.6/ensta.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 ensta.egg-info/PKG-INFO
 ensta.egg-info/SOURCES.txt
 ensta.egg-info/dependency_links.txt
 ensta.egg-info/requires.txt
 ensta.egg-info/top_level.txt
 ensta/containers/FollowPerson.py
 ensta/containers/FollowedStatus.py
+ensta/containers/Post.py
+ensta/containers/PostUser.py
 ensta/containers/Profile.py
 ensta/containers/ProfileHost.py
 ensta/containers/UnfollowedStatus.py
 ensta/containers/__init__.py
 ensta/lib/Commons.py
 ensta/lib/Exceptions.py
 ensta/lib/__init__.py
```

### Comparing `ensta-2.5/setup.py` & `ensta-2.6/setup.py`

 * *Files 16% similar despite different names*

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
-    version="2.5",
-    license="MIT",
-    description="🔥 Fastest & Simplest Python Package For Instagram Automation",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    author="Deepak Soni",
-    author_email="lonelycube@proton.me",
-    url="https://github.com/diezo/ensta",
-    download_url="https://github.com/diezo/ensta/archive/refs/tags/v2.5.tar.gz",
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
+    version="2.6",
+    license="MIT",
+    description="🔥 Fastest & Simplest Python Package For Instagram Automation",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    author="Deepak Soni",
+    author_email="lonelycube@proton.me",
+    url="https://github.com/diezo/ensta",
+    download_url="https://github.com/diezo/ensta/archive/refs/tags/v2.6.tar.gz",
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

