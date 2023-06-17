# Comparing `tmp/rolimons-2.5.3.tar.gz` & `tmp/rolimons-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rolimons-2.5.3.tar", last modified: Mon Mar 20 16:24:39 2023, max compression
+gzip compressed data, was "rolimons-2.5.4.tar", last modified: Sat Jun 17 16:22:48 2023, max compression
```

## Comparing `rolimons-2.5.3.tar` & `rolimons-2.5.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-20 16:24:39.616509 rolimons-2.5.3/
--rw-rw-rw-   0        0        0      917 2023-03-20 16:24:39.616509 rolimons-2.5.3/PKG-INFO
--rw-rw-rw-   0        0        0      693 2023-03-20 16:24:34.000000 rolimons-2.5.3/README.md
-drwxrwxrwx   0        0        0        0 2023-03-20 16:24:39.590755 rolimons-2.5.3/rolimons/
--rw-rw-rw-   0        0        0      202 2023-03-20 16:23:27.000000 rolimons-2.5.3/rolimons/__init__.py
--rw-rw-rw-   0        0        0      123 2023-03-20 16:23:37.000000 rolimons-2.5.3/rolimons/exceptions.py
--rw-rw-rw-   0        0        0     3822 2023-03-20 16:23:55.000000 rolimons-2.5.3/rolimons/item.py
--rw-rw-rw-   0        0        0     2525 2023-03-20 16:23:51.000000 rolimons-2.5.3/rolimons/player.py
--rw-rw-rw-   0        0        0     2096 2023-03-20 16:24:05.000000 rolimons-2.5.3/rolimons/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-20 16:24:39.613682 rolimons-2.5.3/rolimons.egg-info/
--rw-rw-rw-   0        0        0      917 2023-03-20 16:24:39.000000 rolimons-2.5.3/rolimons.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-03-20 16:24:39.000000 rolimons-2.5.3/rolimons.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-20 16:24:39.000000 rolimons-2.5.3/rolimons.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-03-20 16:24:39.000000 rolimons-2.5.3/rolimons.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-20 16:24:39.000000 rolimons-2.5.3/rolimons.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-20 16:24:39.616509 rolimons-2.5.3/setup.cfg
--rw-rw-rw-   0        0        0      488 2023-03-20 16:23:13.000000 rolimons-2.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 16:22:48.318048 rolimons-2.5.4/
+-rw-rw-rw-   0        0        0      917 2023-06-17 16:22:48.318048 rolimons-2.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0      693 2023-03-20 16:24:34.000000 rolimons-2.5.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 16:22:48.303437 rolimons-2.5.4/rolimons/
+-rw-rw-rw-   0        0        0      202 2023-03-20 16:23:27.000000 rolimons-2.5.4/rolimons/__init__.py
+-rw-rw-rw-   0        0        0      123 2023-03-20 16:23:37.000000 rolimons-2.5.4/rolimons/exceptions.py
+-rw-rw-rw-   0        0        0     5086 2023-06-17 16:21:31.000000 rolimons-2.5.4/rolimons/item.py
+-rw-rw-rw-   0        0        0     2525 2023-03-20 16:23:51.000000 rolimons-2.5.4/rolimons/player.py
+-rw-rw-rw-   0        0        0     2096 2023-06-17 16:19:21.000000 rolimons-2.5.4/rolimons/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-17 16:22:48.316152 rolimons-2.5.4/rolimons.egg-info/
+-rw-rw-rw-   0        0        0      917 2023-06-17 16:22:48.000000 rolimons-2.5.4/rolimons.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-06-17 16:22:48.000000 rolimons-2.5.4/rolimons.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 16:22:48.000000 rolimons-2.5.4/rolimons.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-17 16:22:48.000000 rolimons-2.5.4/rolimons.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-17 16:22:48.000000 rolimons-2.5.4/rolimons.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-17 16:22:48.318936 rolimons-2.5.4/setup.cfg
+-rw-rw-rw-   0        0        0      488 2023-06-17 16:22:41.000000 rolimons-2.5.4/setup.py
```

### Comparing `rolimons-2.5.3/PKG-INFO` & `rolimons-2.5.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rolimons
-Version: 2.5.3
+Version: 2.5.4
 Summary: Rolimons API Wrapper
 Home-page: https://github.com/wa1ker38552/rolimons.py
 Author: walker
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Rolimons
```

### Comparing `rolimons-2.5.3/README.md` & `rolimons-2.5.4/README.md`

 * *Files identical despite different names*

### Comparing `rolimons-2.5.3/rolimons/item.py` & `rolimons-2.5.4/rolimons/item.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import requests
 from bs4 import BeautifulSoup
 from .exceptions import RateLimitError
 from .exceptions import InvalidItemDetails
 
 
 class item:
@@ -51,14 +52,40 @@
 
     def get_ownership_data(self):
         request = requests.get(f'https://www.rolimons.com/item/{self.id}')
         soup = BeautifulSoup(request.text, 'html.parser')
         tags = [tag.get_text() for tag in soup.find_all('div', attrs={'class': 'value-stat-data'})]
         return owner(tags)
 
+    def get_owner_data(self):
+        def index_segment(start, end, data):
+            i = data.index(start)
+            while 1:
+                if data[i:i + len(end)] == end: break
+                i += 1
+            return data[data.index(start):i].replace(start, '').strip()
+
+        request = requests.get(f'https://www.rolimons.com/item/{self.id}').text
+        data = json.loads(index_segment('var all_copies_data                = ', '      var all_copies_data_count ', request)[:-1])
+        return ItemOwners(data)
+
+
+class ItemOwners:
+  def __init__(self, data):
+    self.num_copies: int = int(data['num_copies'])
+    self.owner_ids: list[int] = data['owner_ids']
+    self.owner_names: list[str] = data['owner_names']
+    self.uaids: list[int] = data['uaids']
+    self.updated: list[int] = data['updated']
+    self.owner_membership: list[int] = data['owner_bc_levels']
+
+    self.owners: list[dict] = [{'id': id, 'name': self.owner_names[i], 'uaid': self.uaids[i], 'updated': self.updated[i], 'is_premium': True if self.owner_membership[i] else False} for i, id in enumerate(self.owner_ids)]
+
+  def get_premium_owners(self) -> list[dict]:
+    return [self.owners[i] for i, o in enumerate(self.owner_membership) if o]
 
 class sales:
     def __init__(self, data: list):
         self.average_daily_sales: int = data[0]
         self.rap_after_sale: int = data[1]
         self.original_price: int = data[2]
         self.sellers: int = data[3]
```

### Comparing `rolimons-2.5.3/rolimons/player.py` & `rolimons-2.5.4/rolimons/player.py`

 * *Files identical despite different names*

### Comparing `rolimons-2.5.3/rolimons/utils.py` & `rolimons-2.5.4/rolimons/utils.py`

 * *Files identical despite different names*

### Comparing `rolimons-2.5.3/rolimons.egg-info/PKG-INFO` & `rolimons-2.5.4/rolimons.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rolimons
-Version: 2.5.3
+Version: 2.5.4
 Summary: Rolimons API Wrapper
 Home-page: https://github.com/wa1ker38552/rolimons.py
 Author: walker
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Rolimons
```

