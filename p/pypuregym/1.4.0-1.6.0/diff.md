# Comparing `tmp/pypuregym-v1.4.0.tar.gz` & `tmp/pypuregym-v1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypuregym-1.4.0.tar", last modified: Tue Mar  2 01:05:59 2021, max compression
+gzip compressed data, was "pypuregym-1.6.0.tar", last modified: Sat Jun 17 08:40:03 2023, max compression
```

## Comparing `pypuregym-v1.4.0.tar` & `pypuregym-v1.6.0.tar`

### file list

```diff
@@ -1,23 +1,30 @@
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2021-03-02 01:05:59.471538 pypuregym-1.4.0/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2020-10-19 10:23:27.000000 pypuregym-1.4.0/MANIFEST.in
--rw-r--r--   0 jeffrey    (501) staff       (20)     6240 2021-03-02 01:05:59.471959 pypuregym-1.4.0/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)     5054 2020-10-21 01:04:37.000000 pypuregym-1.4.0/README.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2021-03-02 01:05:59.467202 pypuregym-1.4.0/pypuregym/
--rw-r--r--   0 jeffrey    (501) staff       (20)      375 2021-03-02 01:05:43.000000 pypuregym-1.4.0/pypuregym/__init__.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2021-03-02 01:05:59.471008 pypuregym-1.4.0/pypuregym/cli/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2020-11-23 14:38:26.000000 pypuregym-1.4.0/pypuregym/cli/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1490 2021-01-28 00:54:37.000000 pypuregym-1.4.0/pypuregym/cli/book.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1970 2020-10-21 00:48:10.000000 pypuregym-1.4.0/pypuregym/cli/cli.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1294 2020-10-21 00:46:46.000000 pypuregym-1.4.0/pypuregym/cli/location.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1055 2020-10-21 00:46:55.000000 pypuregym-1.4.0/pypuregym/cli/schedule.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6651 2021-03-02 01:03:00.000000 pypuregym-1.4.0/pypuregym/pure_api.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      356 2020-10-20 11:27:54.000000 pypuregym-1.4.0/pypuregym/utilities.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2021-03-02 01:05:59.469002 pypuregym-1.4.0/pypuregym.egg-info/
--rw-r--r--   0 jeffrey    (501) staff       (20)     6240 2021-03-02 01:05:59.000000 pypuregym-1.4.0/pypuregym.egg-info/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)      428 2021-03-02 01:05:59.000000 pypuregym-1.4.0/pypuregym.egg-info/SOURCES.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)        1 2021-03-02 01:05:59.000000 pypuregym-1.4.0/pypuregym.egg-info/dependency_links.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       54 2021-03-02 01:05:59.000000 pypuregym-1.4.0/pypuregym.egg-info/entry_points.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      224 2021-03-02 01:05:59.000000 pypuregym-1.4.0/pypuregym.egg-info/requires.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       10 2021-03-02 01:05:59.000000 pypuregym-1.4.0/pypuregym.egg-info/top_level.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      412 2021-03-02 01:05:59.472974 pypuregym-1.4.0/setup.cfg
--rw-r--r--   0 jeffrey    (501) staff       (20)     1721 2020-10-20 10:56:37.000000 pypuregym-1.4.0/setup.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-06-17 08:40:03.518227 pypuregym-1.6.0/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1071 2023-06-17 08:31:14.000000 pypuregym-1.6.0/LICENSE
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2023-06-17 08:31:14.000000 pypuregym-1.6.0/MANIFEST.in
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5551 2023-06-17 08:40:03.518275 pypuregym-1.6.0/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5054 2023-06-17 08:31:14.000000 pypuregym-1.6.0/README.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-06-17 08:40:03.516425 pypuregym-1.6.0/pypuregym/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      365 2023-06-17 08:38:16.000000 pypuregym-1.6.0/pypuregym/__init__.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-06-17 08:40:03.517631 pypuregym-1.6.0/pypuregym/cli/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2023-06-17 08:31:14.000000 pypuregym-1.6.0/pypuregym/cli/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1515 2023-06-17 08:37:40.000000 pypuregym-1.6.0/pypuregym/cli/book.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1965 2023-06-17 08:37:40.000000 pypuregym-1.6.0/pypuregym/cli/cli.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1408 2023-06-17 08:37:40.000000 pypuregym-1.6.0/pypuregym/cli/location.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1147 2023-06-17 08:37:40.000000 pypuregym-1.6.0/pypuregym/cli/schedule.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6926 2023-06-17 08:37:40.000000 pypuregym-1.6.0/pypuregym/pure_api.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      345 2023-06-17 08:37:40.000000 pypuregym-1.6.0/pypuregym/utilities.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-06-17 08:40:03.517034 pypuregym-1.6.0/pypuregym.egg-info/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5551 2023-06-17 08:40:03.000000 pypuregym-1.6.0/pypuregym.egg-info/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)      563 2023-06-17 08:40:03.000000 pypuregym-1.6.0/pypuregym.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)        1 2023-06-17 08:40:03.000000 pypuregym-1.6.0/pypuregym.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)       53 2023-06-17 08:40:03.000000 pypuregym-1.6.0/pypuregym.egg-info/entry_points.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)      224 2023-06-17 08:40:03.000000 pypuregym-1.6.0/pypuregym.egg-info/requires.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)       10 2023-06-17 08:40:03.000000 pypuregym-1.6.0/pypuregym.egg-info/top_level.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)      412 2023-06-17 08:40:03.518436 pypuregym-1.6.0/setup.cfg
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1721 2023-06-17 08:40:01.000000 pypuregym-1.6.0/setup.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-06-17 08:40:03.518103 pypuregym-1.6.0/tests/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      891 2023-06-17 08:31:14.000000 pypuregym-1.6.0/tests/test_authenticate.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      300 2023-06-17 08:31:14.000000 pypuregym-1.6.0/tests/test_booking.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      810 2023-06-17 08:31:14.000000 pypuregym-1.6.0/tests/test_get_locations.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1181 2023-06-17 08:31:14.000000 pypuregym-1.6.0/tests/test_get_schedule.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      162 2023-06-17 08:31:14.000000 pypuregym-1.6.0/tests/test_pure_api.py
```

### Comparing `pypuregym-1.4.0/PKG-INFO` & `pypuregym-1.6.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,100 +1,100 @@
 Metadata-Version: 2.1
 Name: pypuregym
-Version: 1.4.0
+Version: 1.6.0
 Summary: A library to interact with Pure Fitness/Pure Yoga APIs.
 Home-page: https://github.com/j-muller/pypuregym
 Author: Jeffrey Muller
 Author-email: hello@jeffrey.wtf
-License: UNKNOWN
-Description: [![Documentation Status](https://readthedocs.org/projects/pypuregym/badge/?version=latest)](https://pypuregym.readthedocs.io/en/latest/?badge=latest) [![Build Status](https://travis-ci.com/j-muller/pypuregym.svg?branch=master)](https://travis-ci.com/j-muller/pypuregym) [![codecov](https://codecov.io/gh/j-muller/pypuregym/branch/master/graph/badge.svg)](https://codecov.io/gh/j-muller/pypuregym)
-        
-        pypuregym
-        =================
-        
-        A Python library to interact with Pure Fitness/Pure Yoga APIs.
-        This library helps you to get the schedule of a Pure studio and book classes.
-        Currently, the following Pure locations are supported:
-        
-        * Hong Kong
-        * Singapore
-        * Shanghai
-        
-        ## Installation
-        
-        ```
-        $ pip install pypuregym
-        ```
-        
-        ## CLI usage
-        
-        ```
-        $ pypuregym --help
-        Interact with Pure Fitness/Yoga service.
-        
-        Usage:
-          pypuregym location <gym-type> <region-id>
-          pypuregym schedule <region-id> <location-id> <date>
-          pypuregym book <region-id> <class-id> <username> <password> [--wait-until <wait>] [--retry <retry>]
-        
-        Options:
-          <gym-type>                  Can be "fitness" or "yoga".
-          <region-id>                 Can be "HK", "CN" or "SG".
-          <location-id>               ID of the studio (given with the "location" command).
-          <date>                      Date to get the schedule for.
-          <class-id>                  Class ID to book.
-          <username>                  Your Pure username/email.
-          <password>                  Your Pure password.
-          --wait-until <wait>         When booking a class, wait until the specified date time before booking.
-          --retry <retry>             Number of time to retry when booking the class.
-        ```
-        
-        #### Get Pure locations
-        
-        ```
-        $ pypuregym location fitness hk
-        ╒══════╤═════════════════╤══════════════════════════════╤══════════════╕
-        │   ID │ Code            │ Name                         │ District     │
-        ╞══════╪═════════════════╪══════════════════════════════╪══════════════╡
-        │    4 │ LTP             │ Lee Theatre                  │ Causeway Bay │
-        ├──────┼─────────────────┼──────────────────────────────┼──────────────┤
-        │    6 │ LPF             │ Langham Place                │ Mongkok      │
-        ├──────┼─────────────────┼──────────────────────────────┼──────────────┤
-        │    8 │ KIN             │ Kinwick Centre               │ Central      │
-        ╘══════╧═════════════════╧══════════════════════════════╧══════════════╛
-        ```
-        
-        #### Get Pure schedule
-        
-        ```
-        $ pypuregym schedule hk 4 2020-01-01
-        ╒═══════╤═════════════════════╤═══════════╤══════════════╤════════════╕
-        │    ID │ Class Name          │ Teacher   │ Start Time   │ End Time   │
-        ╞═══════╪═════════════════════╪═══════════╪══════════════╪════════════╡
-        │ 71647 │ BODYATTACK™         │ John D.   │ 10:00:00     │ 11:00:00   │
-        ├───────┼─────────────────────┼───────────┼──────────────┼────────────┤
-        │ 71648 │ RPM™                │ John D.   │ 11:15:00     │ 12:05:00   │
-        ├───────┼─────────────────────┼───────────┼──────────────┼────────────┤
-        │ 71649 │ BODYPUMP™           │ Jane F.   │ 11:15:00     │ 12:15:00   │
-        ├───────┼─────────────────────┼───────────┼──────────────┼────────────┤
-        │ 71650 │ ABS, BUTTS & THIGHS │ Jane F.   │ 12:30:00     │ 13:30:00   │
-        ╘═══════╧═════════════════════╧═══════════╧══════════════╧════════════╛
-        ```
-        
-        #### Book a class
-        
-        ```
-        $ pypuregym book hk 155188 $PURE_USERNAME $PURE_PASSWORD
-        ```
-        
-        ## Documentation
-        
-        You can read the documentation here.
-        This project has been tested under Python 3.6+
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: doc
 Provides-Extra: dev
+License-File: LICENSE
+
+[![Documentation Status](https://readthedocs.org/projects/pypuregym/badge/?version=latest)](https://pypuregym.readthedocs.io/en/latest/?badge=latest) [![Build Status](https://travis-ci.com/j-muller/pypuregym.svg?branch=master)](https://travis-ci.com/j-muller/pypuregym) [![codecov](https://codecov.io/gh/j-muller/pypuregym/branch/master/graph/badge.svg)](https://codecov.io/gh/j-muller/pypuregym)
+
+pypuregym
+=================
+
+A Python library to interact with Pure Fitness/Pure Yoga APIs.
+This library helps you to get the schedule of a Pure studio and book classes.
+Currently, the following Pure locations are supported:
+
+* Hong Kong
+* Singapore
+* Shanghai
+
+## Installation
+
+```
+$ pip install pypuregym
+```
+
+## CLI usage
+
+```
+$ pypuregym --help
+Interact with Pure Fitness/Yoga service.
+
+Usage:
+  pypuregym location <gym-type> <region-id>
+  pypuregym schedule <region-id> <location-id> <date>
+  pypuregym book <region-id> <class-id> <username> <password> [--wait-until <wait>] [--retry <retry>]
+
+Options:
+  <gym-type>                  Can be "fitness" or "yoga".
+  <region-id>                 Can be "HK", "CN" or "SG".
+  <location-id>               ID of the studio (given with the "location" command).
+  <date>                      Date to get the schedule for.
+  <class-id>                  Class ID to book.
+  <username>                  Your Pure username/email.
+  <password>                  Your Pure password.
+  --wait-until <wait>         When booking a class, wait until the specified date time before booking.
+  --retry <retry>             Number of time to retry when booking the class.
+```
+
+#### Get Pure locations
+
+```
+$ pypuregym location fitness hk
+╒══════╤═════════════════╤══════════════════════════════╤══════════════╕
+│   ID │ Code            │ Name                         │ District     │
+╞══════╪═════════════════╪══════════════════════════════╪══════════════╡
+│    4 │ LTP             │ Lee Theatre                  │ Causeway Bay │
+├──────┼─────────────────┼──────────────────────────────┼──────────────┤
+│    6 │ LPF             │ Langham Place                │ Mongkok      │
+├──────┼─────────────────┼──────────────────────────────┼──────────────┤
+│    8 │ KIN             │ Kinwick Centre               │ Central      │
+╘══════╧═════════════════╧══════════════════════════════╧══════════════╛
+```
+
+#### Get Pure schedule
+
+```
+$ pypuregym schedule hk 4 2020-01-01
+╒═══════╤═════════════════════╤═══════════╤══════════════╤════════════╕
+│    ID │ Class Name          │ Teacher   │ Start Time   │ End Time   │
+╞═══════╪═════════════════════╪═══════════╪══════════════╪════════════╡
+│ 71647 │ BODYATTACK™         │ John D.   │ 10:00:00     │ 11:00:00   │
+├───────┼─────────────────────┼───────────┼──────────────┼────────────┤
+│ 71648 │ RPM™                │ John D.   │ 11:15:00     │ 12:05:00   │
+├───────┼─────────────────────┼───────────┼──────────────┼────────────┤
+│ 71649 │ BODYPUMP™           │ Jane F.   │ 11:15:00     │ 12:15:00   │
+├───────┼─────────────────────┼───────────┼──────────────┼────────────┤
+│ 71650 │ ABS, BUTTS & THIGHS │ Jane F.   │ 12:30:00     │ 13:30:00   │
+╘═══════╧═════════════════════╧═══════════╧══════════════╧════════════╛
+```
+
+#### Book a class
+
+```
+$ pypuregym book hk 155188 $PURE_USERNAME $PURE_PASSWORD
+```
+
+## Documentation
+
+You can read the documentation here.
+This project has been tested under Python 3.6+
```

### Comparing `pypuregym-1.4.0/README.md` & `pypuregym-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pypuregym-1.4.0/pypuregym/cli/book.py` & `pypuregym-1.6.0/pypuregym/cli/book.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,42 +7,44 @@
 from pypuregym import PureAPI, Region
 
 LOGGER = logging.getLogger(__name__)
 
 
 # pylint: disable=too-many-arguments
 def book_class(region_id, class_id, username, password, wait_until, retry):
-    """Get Pure schedule.
-    """
-    LOGGER.info('Booking class #%d', class_id)
+    """Get Pure schedule."""
+    LOGGER.info("Booking class #%d", class_id)
 
     try:
         region = Region[region_id.upper()]
     except KeyError:
         raise ValueError(
-            '"%s" is not a valid region. Should be one of: %s' % (
+            '"%s" is not a valid region. Should be one of: %s'
+            % (
                 region_id,
-                ', '.join([e.name for e in Region]),
-            )) from None
+                ", ".join([e.name for e in Region]),
+            )
+        ) from None
 
     api = PureAPI(
         username=username,
         password=password,
         region=region,
     )
 
     if wait_until is not None:
         wait_until = dateutil.parser.parse(wait_until)
         now = datetime.datetime.now()
         delta = wait_until - now
 
-        assert now <= wait_until, (
-            '--wait-until can not be lower than current time')
+        assert (
+            now <= wait_until
+        ), "--wait-until can not be lower than current time"
 
-        LOGGER.info('Wait until %s before booking...', wait_until)
+        LOGGER.info("Wait until %s before booking...", wait_until)
         time.sleep(delta.seconds)
 
     retry = int(retry) if retry is not None else 1
     exception = None
 
     for _ in range(retry):
         # pylint: disable=broad-except
@@ -51,8 +53,8 @@
             exception = None
             break
         except Exception as exc:
             exception = exc
 
     if exception is not None:
         raise exception
-    LOGGER.info('The class has been successfully booked!')
+    LOGGER.info("The class has been successfully booked!")
```

### Comparing `pypuregym-1.4.0/pypuregym/cli/cli.py` & `pypuregym-1.6.0/pypuregym/cli/cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -23,40 +23,39 @@
 from pypuregym import __version__
 from pypuregym.cli.location import get_location
 from pypuregym.cli.schedule import get_schedule
 from pypuregym.cli.book import book_class
 
 
 def main():
-    """CLI entry point.
-    """
+    """CLI entry point."""
     args = docopt(__doc__, version=__version__)
 
     logging.basicConfig(
-        format='%(asctime)s - %(levelname)s - %(message)s',
+        format="%(asctime)s - %(levelname)s - %(message)s",
         level=logging.INFO,
     )
 
-    if args['location']:
+    if args["location"]:
         get_location(
-            gym_type=args['<gym-type>'],
-            region_id=args['<region-id>'],
+            gym_type=args["<gym-type>"],
+            region_id=args["<region-id>"],
         )
-    elif args['schedule']:
+    elif args["schedule"]:
         get_schedule(
-            region_id=args['<region-id>'],
-            location_id=int(args['<location-id>']),
-            date=args['<date>'],
+            region_id=args["<region-id>"],
+            location_id=int(args["<location-id>"]),
+            date=args["<date>"],
         )
-    elif args['book']:
+    elif args["book"]:
         book_class(
-            region_id=args['<region-id>'],
-            class_id=int(args['<class-id>']),
-            username=args['<username>'],
-            password=args['<password>'],
-            wait_until=args['--wait-until'],
-            retry=args['--retry'],
+            region_id=args["<region-id>"],
+            class_id=int(args["<class-id>"]),
+            username=args["<username>"],
+            password=args["<password>"],
+            wait_until=args["--wait-until"],
+            retry=args["--retry"],
         )
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `pypuregym-1.4.0/pypuregym/cli/location.py` & `pypuregym-1.6.0/pypuregym/cli/location.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,41 +9,50 @@
     :param gym_type: `str` Type of the studio.
     :param region_id: `str` region location of the studio.
     """
     try:
         region = Region[region_id.upper()]
     except KeyError:
         raise ValueError(
-            '"%s" is not a valid region. Should be one of: %s' % (
+            '"%s" is not a valid region. Should be one of: %s'
+            % (
                 region_id,
-                ', '.join([e.name for e in Region]),
-            )) from None
+                ", ".join([e.name for e in Region]),
+            )
+        ) from None
 
     try:
         gym_type = GymType[gym_type.upper()]
     except KeyError:
         raise ValueError(
-            '"%s" is not a valid gym type. Should be one of: %s' % (
+            '"%s" is not a valid gym type. Should be one of: %s'
+            % (
                 gym_type,
-                ', '.join([e.name for e in GymType]),
-            )) from None
+                ", ".join([e.name for e in GymType]),
+            )
+        ) from None
 
     api = PureAPI(
         username=None,
         password=None,
         region=region,
     )
     response = api.get_locations(gym_type)
 
     # Format response
-    response = [{
-        'ID': entry['id'],
-        'Code': entry['code'],
-        'Name': entry['short_name']['en'],
-        'District': entry['district']['en'],
-    } for entry in response]
+    response = [
+        {
+            "ID": entry["id"],
+            "Code": entry["code"],
+            "Name": entry["short_name"]["en"],
+            "District": entry["district"]["en"],
+        }
+        for entry in response
+    ]
 
-    print(tabulate(
-        sorted(response, key=lambda e: e['ID']),
-        headers='keys',
-        tablefmt='fancy_grid',
-    ))
+    print(
+        tabulate(
+            sorted(response, key=lambda e: e["ID"]),
+            headers="keys",
+            tablefmt="fancy_grid",
+        )
+    )
```

### Comparing `pypuregym-1.4.0/pypuregym/cli/schedule.py` & `pypuregym-1.6.0/pypuregym/cli/schedule.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 from tabulate import tabulate
 
 from pypuregym import PureAPI, Region
 
 
 def get_schedule(region_id, location_id, date):
-    """Get Pure schedule.
-    """
+    """Get Pure schedule."""
     try:
         region = Region[region_id.upper()]
     except KeyError:
         raise ValueError(
-            '"%s" is not a valid region. Should be one of: %s' % (
+            '"%s" is not a valid region. Should be one of: %s'
+            % (
                 region_id,
-                ', '.join([e.name for e in Region]),
-            )) from None
+                ", ".join([e.name for e in Region]),
+            )
+        ) from None
 
     api = PureAPI(
         username=None,
         password=None,
         region=region,
     )
     response = api.get_schedule(
         start_date=date,
         last_date=date,
         location_id=location_id,
     )
 
     # Format response
-    response = [{
-        'ID': entry['id'],
-        'Class Name': entry['class_type']['name'],
-        'Teacher': entry['teacher']['name'],
-        'Start Time': entry['start_time'],
-        'End Time': entry['end_time'],
-    } for entry in response]
-
-    print(tabulate(
-        sorted(response, key=lambda e: e['Start Time']),
-        headers='keys',
-        tablefmt='fancy_grid',
-    ))
+    response = [
+        {
+            "ID": entry["id"],
+            "Class Name": entry["class_type"]["name"],
+            "Teacher": entry["teacher"]["name"],
+            "Start Time": entry["start_time"],
+            "End Time": entry["end_time"],
+        }
+        for entry in response
+    ]
+
+    print(
+        tabulate(
+            sorted(response, key=lambda e: e["Start Time"]),
+            headers="keys",
+            tablefmt="fancy_grid",
+        )
+    )
```

### Comparing `pypuregym-1.4.0/pypuregym/pure_api.py` & `pypuregym-1.6.0/pypuregym/pure_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,203 +1,222 @@
 import json
 import logging
 import re
+import time
 
 import dateutil.parser
 import requests
 
 
 LOGGER = logging.getLogger(__name__)
 
 
 # pylint: disable=too-many-instance-attributes
 class PureAPI:
-    """A class to perform queries through Pure Fitness/Yoga API.
-    """
+    """A class to perform queries through Pure Fitness/Yoga API."""
 
-    def __init__(self, username, password, region):
+    def __init__(self, region, username=None, password=None):
         """Create a PureAPI object.
 
+        :param region: `pypuregym.Region` Pure region.
         :param username: `str` Pure Fitness/Yoga username.
         :param password: `str` Pure Fitness/Yoga password.
-        :param region: `pypuregym.Region` Pure region.
         """
         self._username = username
         self._password = password
 
         self._region = region
 
         self._jwt_token = None
         self._token = None
         self._date = None
 
         self._session = requests.Session()
         self._session.headers = {
-            'user-agent': ('Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) '
-                           'AppleWebKit/537.36 (KHTML, like Gecko) '
-                           'Chrome/80.0.3987.163 Safari/537.36'),
+            "user-agent": (
+                "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) "
+                "AppleWebKit/537.36 (KHTML, like Gecko) "
+                "Chrome/80.0.3987.163 Safari/537.36"
+            ),
         }
 
     def authenticate(self):
-        """Authenticate on Pure Fitness API.
-        """
+        """Authenticate on Pure Fitness API."""
         # No matter the gym type and subscription, everybody can log in to Pure
         # Fitness or (Pure Yoga).
-        url = 'https://pure360.pure-fitness.com/en/%s' % (
-            self._region.name.lower())
+        url = "https://pure360.pure-fitness.com/en/%s" % (
+            self._region.name.lower()
+        )
 
-        LOGGER.debug('Get token from: %s', url)
+        LOGGER.debug("Get token from: %s", url)
 
         response = self._session.get(url=url, timeout=3)
         response.raise_for_status()
 
         match = re.search(
-            r'"X-Date":(?P<date>\d+)."X-Token":"(?P<token>[a-z0-9]+)"',
-            response.content.decode('utf-8'),
+            r"<meta name=\"token\" content=\"(?P<token>[a-z0-9]+)\">",
+            response.content.decode("utf-8"),
         )
-        assert match, 'Can not find date and token from: %s' % url
+        assert match, "Can not find token from: %s" % url
 
         match = match.groupdict()
-        self._token = match['token']
-        self._date = match['date']
+        self._token = match["token"]
+        self._date = str(int(time.time()) * 1000)
 
         if self._username and self._password:
-            url = 'https://pure360-api.pure-international.com/api/v3/login'
+            url = "https://pure360-api.pure-international.com/api/v3/login"
 
             LOGGER.debug('Authenticating as "%s" on: %s', self._username, url)
             response = self._session.post(
                 url=url,
                 timeout=3,
                 headers={
-                    'x-date': match['date'],
-                    'x-token': match['token'],
-                    'content-type': 'application/json',
+                    "x-date": self._date,
+                    "x-token": self._token,
+                    "content-type": "application/json",
                 },
-                data=json.dumps({
-                    'username': self._username,
-                    'password': self._password,
-                    'language_id': 1,
-                    'region_id': self._region.value,
-                    'jwt': True,
-                    'platform': 'Web',
-                }))
+                data=json.dumps(
+                    {
+                        "username": self._username,
+                        "password": self._password,
+                        "language_id": 1,
+                        "region_id": self._region.value,
+                        "jwt": True,
+                        "platform": "Web",
+                    }
+                ),
+            )
             response.raise_for_status()
 
             response = response.json()
-            assert response['error']['code'] == 200, (
-                'Authentication failed: %s' % response['error'])
+            assert response["error"]["code"] == 200, (
+                "Authentication failed: %s" % response["error"]
+            )
 
-            self._jwt_token = response['data']['user']['jwt']
+            self._jwt_token = response["data"]["user"]["jwt"]
 
     def get_locations(self, gym_type):
         """Get Pure studios location.
 
         :param gym_type: `pypuregym.GymType` Pure gym type.
         """
         if not self._token or not self._date:
             self.authenticate()
 
-        LOGGER.debug('Get Pure locations')
+        LOGGER.debug("Get Pure locations")
 
-        url = 'https://pure360-api.pure-international.com/api/v3/view_location'
+        url = "https://pure360-api.pure-international.com/api/v3/view_location"
         response = self._session.get(
             url=url,
             timeout=3,
             params={
-                'type': gym_type.value,
-                'language_id': 1,  # English
-                'region_id': self._region.value,
+                "type": gym_type.value,
+                "language_id": 1,  # English
+                "region_id": self._region.value,
             },
             headers={
-                'x-date': self._date,
-                'x-token': self._token,
+                "x-date": self._date,
+                "x-token": self._token,
             },
         )
         response.raise_for_status()
 
         response = response.json()
-        assert response['error']['code'] == 200, (
-            'Failed to get locations: %s' % response['error'])
+        assert response["error"]["code"] == 200, (
+            "Failed to get locations: %s" % response["error"]
+        )
 
-        return response.get('data', {}).get('locations', [])
+        return response.get("data", {}).get("locations", [])
 
     def get_schedule(self, start_date, last_date, location_id):
         """Get classes schedule within a date range in a given location.
 
         You can pass `start_date` and `last_date` as `datetime` or `str`.
 
         :param start_date: First date to get the classes for (inclusive).
         :param last_date: Last date to get the classes for (inclusive).
         """
         if not self._token or not self._date:
             self.authenticate()
 
-        LOGGER.debug('Getting schedule between %s and %s',
-                     start_date, last_date)
+        LOGGER.debug(
+            "Getting schedule between %s and %s", start_date, last_date
+        )
 
         # Convert start and last dates to datetime objects.
         if isinstance(start_date, str):
             start_date = dateutil.parser.parse(start_date)
         if isinstance(last_date, str):
             last_date = dateutil.parser.parse(last_date)
 
-        assert last_date >= start_date, (
-            'Last date can not be < start date (%s < %s)' % (
-                last_date, start_date))
+        assert (
+            last_date >= start_date
+        ), "Last date can not be < start date (%s < %s)" % (
+            last_date,
+            start_date,
+        )
+
+        url = "https://pure360-api.pure-international.com/api/v3/view_schedule"
+        headers = {
+            "x-token": self._token,
+            "x-date": self._date,
+        }
+
+        if self._jwt_token:
+            headers["x-jwt-token"] = self._jwt_token
 
-        url = 'https://pure360-api.pure-international.com/api/v3/view_schedule'
         response = self._session.get(
             url=url,
-            headers={
-                'x-jwt-token': self._jwt_token,
-                'x-token': self._token,
-                'x-date': self._date,
-            },
+            headers=headers,
             params={
-                'language_id': '1',
-                'region_id': self._region.value,
-                'location_ids': location_id,
-                'start_date': start_date.strftime('%Y%m%d'),
-                'days': (last_date - start_date).days + 1,
+                "language_id": "1",
+                "region_id": self._region.value,
+                "location_ids": location_id,
+                "start_date": start_date.strftime("%Y%m%d"),
+                "days": (last_date - start_date).days + 1,
             },
         )
         response.raise_for_status()
 
         response = response.json()
-        assert response['error']['code'] == 200, (
-            'Get schedule failed: %s' % response['error'])
+        assert response["error"]["code"] == 200, (
+            "Get schedule failed: %s" % response["error"]
+        )
 
-        return response['data']['classes']
+        return response["data"]["classes"]
 
     def book(self, class_id):
         """Book a class.
 
         :param class_id: `int` class id to book.
         """
         if not self._jwt_token:
             self.authenticate()
 
-        LOGGER.debug('Booking class id #%d', class_id)
+        LOGGER.debug("Booking class id #%d", class_id)
 
-        url = 'https://pure360-api.pure-international.com/api/v3/booking'
+        url = "https://pure360-api.pure-international.com/api/v3/booking"
         response = self._session.post(
             url=url,
             timeout=3,
             headers={
-                'x-jwt-token': self._jwt_token,
-                'x-token': self._token,
-                'x-date': self._date,
-                'content-type': 'application/json',
+                "x-jwt-token": self._jwt_token,
+                "x-token": self._token,
+                "x-date": self._date,
+                "content-type": "application/json",
             },
-            data=json.dumps({
-                'language_id': 1,
-                'region_id': self._region.value,
-                'class_id': class_id,
-                'booked_from': 'WEB',
-                'book_type': 1,
-            }),
+            data=json.dumps(
+                {
+                    "language_id": 1,
+                    "region_id": self._region.value,
+                    "class_id": class_id,
+                    "booked_from": "WEB",
+                    "book_type": 1,
+                }
+            ),
         )
         response.raise_for_status()
 
         response = response.json()
-        assert response['error']['code'] == 200, (
-            'Failed to book class: %s' % response['error'])
+        assert response["error"]["code"] == 200, (
+            "Failed to book class: %s" % response["error"]
+        )
```

### Comparing `pypuregym-1.4.0/pypuregym.egg-info/PKG-INFO` & `pypuregym-1.6.0/pypuregym.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,100 +1,100 @@
 Metadata-Version: 2.1
 Name: pypuregym
-Version: 1.4.0
+Version: 1.6.0
 Summary: A library to interact with Pure Fitness/Pure Yoga APIs.
 Home-page: https://github.com/j-muller/pypuregym
 Author: Jeffrey Muller
 Author-email: hello@jeffrey.wtf
-License: UNKNOWN
-Description: [![Documentation Status](https://readthedocs.org/projects/pypuregym/badge/?version=latest)](https://pypuregym.readthedocs.io/en/latest/?badge=latest) [![Build Status](https://travis-ci.com/j-muller/pypuregym.svg?branch=master)](https://travis-ci.com/j-muller/pypuregym) [![codecov](https://codecov.io/gh/j-muller/pypuregym/branch/master/graph/badge.svg)](https://codecov.io/gh/j-muller/pypuregym)
-        
-        pypuregym
-        =================
-        
-        A Python library to interact with Pure Fitness/Pure Yoga APIs.
-        This library helps you to get the schedule of a Pure studio and book classes.
-        Currently, the following Pure locations are supported:
-        
-        * Hong Kong
-        * Singapore
-        * Shanghai
-        
-        ## Installation
-        
-        ```
-        $ pip install pypuregym
-        ```
-        
-        ## CLI usage
-        
-        ```
-        $ pypuregym --help
-        Interact with Pure Fitness/Yoga service.
-        
-        Usage:
-          pypuregym location <gym-type> <region-id>
-          pypuregym schedule <region-id> <location-id> <date>
-          pypuregym book <region-id> <class-id> <username> <password> [--wait-until <wait>] [--retry <retry>]
-        
-        Options:
-          <gym-type>                  Can be "fitness" or "yoga".
-          <region-id>                 Can be "HK", "CN" or "SG".
-          <location-id>               ID of the studio (given with the "location" command).
-          <date>                      Date to get the schedule for.
-          <class-id>                  Class ID to book.
-          <username>                  Your Pure username/email.
-          <password>                  Your Pure password.
-          --wait-until <wait>         When booking a class, wait until the specified date time before booking.
-          --retry <retry>             Number of time to retry when booking the class.
-        ```
-        
-        #### Get Pure locations
-        
-        ```
-        $ pypuregym location fitness hk
-        ╒══════╤═════════════════╤══════════════════════════════╤══════════════╕
-        │   ID │ Code            │ Name                         │ District     │
-        ╞══════╪═════════════════╪══════════════════════════════╪══════════════╡
-        │    4 │ LTP             │ Lee Theatre                  │ Causeway Bay │
-        ├──────┼─────────────────┼──────────────────────────────┼──────────────┤
-        │    6 │ LPF             │ Langham Place                │ Mongkok      │
-        ├──────┼─────────────────┼──────────────────────────────┼──────────────┤
-        │    8 │ KIN             │ Kinwick Centre               │ Central      │
-        ╘══════╧═════════════════╧══════════════════════════════╧══════════════╛
-        ```
-        
-        #### Get Pure schedule
-        
-        ```
-        $ pypuregym schedule hk 4 2020-01-01
-        ╒═══════╤═════════════════════╤═══════════╤══════════════╤════════════╕
-        │    ID │ Class Name          │ Teacher   │ Start Time   │ End Time   │
-        ╞═══════╪═════════════════════╪═══════════╪══════════════╪════════════╡
-        │ 71647 │ BODYATTACK™         │ John D.   │ 10:00:00     │ 11:00:00   │
-        ├───────┼─────────────────────┼───────────┼──────────────┼────────────┤
-        │ 71648 │ RPM™                │ John D.   │ 11:15:00     │ 12:05:00   │
-        ├───────┼─────────────────────┼───────────┼──────────────┼────────────┤
-        │ 71649 │ BODYPUMP™           │ Jane F.   │ 11:15:00     │ 12:15:00   │
-        ├───────┼─────────────────────┼───────────┼──────────────┼────────────┤
-        │ 71650 │ ABS, BUTTS & THIGHS │ Jane F.   │ 12:30:00     │ 13:30:00   │
-        ╘═══════╧═════════════════════╧═══════════╧══════════════╧════════════╛
-        ```
-        
-        #### Book a class
-        
-        ```
-        $ pypuregym book hk 155188 $PURE_USERNAME $PURE_PASSWORD
-        ```
-        
-        ## Documentation
-        
-        You can read the documentation here.
-        This project has been tested under Python 3.6+
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: doc
 Provides-Extra: dev
+License-File: LICENSE
+
+[![Documentation Status](https://readthedocs.org/projects/pypuregym/badge/?version=latest)](https://pypuregym.readthedocs.io/en/latest/?badge=latest) [![Build Status](https://travis-ci.com/j-muller/pypuregym.svg?branch=master)](https://travis-ci.com/j-muller/pypuregym) [![codecov](https://codecov.io/gh/j-muller/pypuregym/branch/master/graph/badge.svg)](https://codecov.io/gh/j-muller/pypuregym)
+
+pypuregym
+=================
+
+A Python library to interact with Pure Fitness/Pure Yoga APIs.
+This library helps you to get the schedule of a Pure studio and book classes.
+Currently, the following Pure locations are supported:
+
+* Hong Kong
+* Singapore
+* Shanghai
+
+## Installation
+
+```
+$ pip install pypuregym
+```
+
+## CLI usage
+
+```
+$ pypuregym --help
+Interact with Pure Fitness/Yoga service.
+
+Usage:
+  pypuregym location <gym-type> <region-id>
+  pypuregym schedule <region-id> <location-id> <date>
+  pypuregym book <region-id> <class-id> <username> <password> [--wait-until <wait>] [--retry <retry>]
+
+Options:
+  <gym-type>                  Can be "fitness" or "yoga".
+  <region-id>                 Can be "HK", "CN" or "SG".
+  <location-id>               ID of the studio (given with the "location" command).
+  <date>                      Date to get the schedule for.
+  <class-id>                  Class ID to book.
+  <username>                  Your Pure username/email.
+  <password>                  Your Pure password.
+  --wait-until <wait>         When booking a class, wait until the specified date time before booking.
+  --retry <retry>             Number of time to retry when booking the class.
+```
+
+#### Get Pure locations
+
+```
+$ pypuregym location fitness hk
+╒══════╤═════════════════╤══════════════════════════════╤══════════════╕
+│   ID │ Code            │ Name                         │ District     │
+╞══════╪═════════════════╪══════════════════════════════╪══════════════╡
+│    4 │ LTP             │ Lee Theatre                  │ Causeway Bay │
+├──────┼─────────────────┼──────────────────────────────┼──────────────┤
+│    6 │ LPF             │ Langham Place                │ Mongkok      │
+├──────┼─────────────────┼──────────────────────────────┼──────────────┤
+│    8 │ KIN             │ Kinwick Centre               │ Central      │
+╘══════╧═════════════════╧══════════════════════════════╧══════════════╛
+```
+
+#### Get Pure schedule
+
+```
+$ pypuregym schedule hk 4 2020-01-01
+╒═══════╤═════════════════════╤═══════════╤══════════════╤════════════╕
+│    ID │ Class Name          │ Teacher   │ Start Time   │ End Time   │
+╞═══════╪═════════════════════╪═══════════╪══════════════╪════════════╡
+│ 71647 │ BODYATTACK™         │ John D.   │ 10:00:00     │ 11:00:00   │
+├───────┼─────────────────────┼───────────┼──────────────┼────────────┤
+│ 71648 │ RPM™                │ John D.   │ 11:15:00     │ 12:05:00   │
+├───────┼─────────────────────┼───────────┼──────────────┼────────────┤
+│ 71649 │ BODYPUMP™           │ Jane F.   │ 11:15:00     │ 12:15:00   │
+├───────┼─────────────────────┼───────────┼──────────────┼────────────┤
+│ 71650 │ ABS, BUTTS & THIGHS │ Jane F.   │ 12:30:00     │ 13:30:00   │
+╘═══════╧═════════════════════╧═══════════╧══════════════╧════════════╛
+```
+
+#### Book a class
+
+```
+$ pypuregym book hk 155188 $PURE_USERNAME $PURE_PASSWORD
+```
+
+## Documentation
+
+You can read the documentation here.
+This project has been tested under Python 3.6+
```

### Comparing `pypuregym-1.4.0/setup.py` & `pypuregym-1.6.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     with open(join(dirname(__file__), filename)) as fileobj:
         return fileobj.read()
 
 
 def get_version(package):
     return [
         line for line in read('{}/__init__.py'.format(package)).splitlines()
-        if line.startswith('__version__ = ')][0].split("'")[1]
+        if line.startswith('__version__ = ')][0].split('"')[1]
 
 
 PROJECT_NAME = "pypuregym"
 PACKAGE_NAME = "pypuregym"
 VERSION = get_version(PACKAGE_NAME)
```

