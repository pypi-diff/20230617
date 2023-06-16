# Comparing `tmp/ofscraper-2.4.1.tar.gz` & `tmp/ofscraper-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-2.4.1.tar", max compression
+gzip compressed data, was "ofscraper-2.4.3.tar", max compression
```

## Comparing `ofscraper-2.4.1.tar` & `ofscraper-2.4.3.tar`

### file list

```diff
@@ -1,49 +1,50 @@
--rw-r--r--   0        0        0     1067 2023-06-15 14:23:11.103686 ofscraper-2.4.1/LICENSE
--rw-r--r--   0        0        0     5201 2023-06-15 14:23:11.103686 ofscraper-2.4.1/README.md
--rw-r--r--   0        0        0      607 2023-06-15 14:23:11.111686 ofscraper-2.4.1/ofscraper/__init__.py
--rw-r--r--   0        0        0      999 2023-06-15 14:23:11.111686 ofscraper-2.4.1/ofscraper/__version__.py
--rw-r--r--   0        0        0        1 2023-06-15 14:23:11.111686 ofscraper-2.4.1/ofscraper/api/__init__.py
--rw-r--r--   0        0        0     7066 2023-06-15 14:23:11.111686 ofscraper-2.4.1/ofscraper/api/archive.py
--rw-r--r--   0        0        0     3944 2023-06-15 14:23:11.111686 ofscraper-2.4.1/ofscraper/api/highlights.py
--rw-r--r--   0        0        0     1067 2023-06-15 14:23:11.111686 ofscraper-2.4.1/ofscraper/api/init.py
--rw-r--r--   0        0        0     2343 2023-06-15 14:23:11.111686 ofscraper-2.4.1/ofscraper/api/me.py
--rw-r--r--   0        0        0     6515 2023-06-15 14:23:11.111686 ofscraper-2.4.1/ofscraper/api/messages.py
--rw-r--r--   0        0        0     8462 2023-06-15 14:23:11.111686 ofscraper-2.4.1/ofscraper/api/paid.py
--rw-r--r--   0        0        0     4576 2023-06-15 14:23:11.111686 ofscraper-2.4.1/ofscraper/api/pinned.py
--rw-r--r--   0        0        0    11157 2023-06-15 14:23:11.111686 ofscraper-2.4.1/ofscraper/api/posts.py
--rw-r--r--   0        0        0     3593 2023-06-15 14:23:11.111686 ofscraper-2.4.1/ofscraper/api/profile.py
--rw-r--r--   0        0        0     3047 2023-06-15 14:23:11.111686 ofscraper-2.4.1/ofscraper/api/subscriptions.py
--rw-r--r--   0        0        0     7713 2023-06-15 14:23:11.111686 ofscraper-2.4.1/ofscraper/api/timeline.py
--rw-r--r--   0        0        0    31071 2023-06-15 14:23:11.111686 ofscraper-2.4.1/ofscraper/commands/check.py
--rwxr-xr-x   0        0        0    22507 2023-06-15 14:23:11.111686 ofscraper-2.4.1/ofscraper/commands/scraper.py
--rw-r--r--   0        0        0     5769 2023-06-15 14:23:11.111686 ofscraper-2.4.1/ofscraper/constants.py
--rw-r--r--   0        0        0        1 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/db/__init__.py
--rw-r--r--   0        0        0     8581 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/db/operations.py
--rw-r--r--   0        0        0     3253 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/db/queries.py
--rw-r--r--   0        0        0        1 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/interaction/__init__.py
--rw-r--r--   0        0        0     4121 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/interaction/like.py
--rw-r--r--   0        0        0     1364 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/prompt model.md
--rw-r--r--   0        0        0      463 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/prompts/prompt_strings.py
--rw-r--r--   0        0        0     6754 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/prompts/prompt_validators.py
--rw-r--r--   0        0        0    26253 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/prompts/prompts.py
--rw-r--r--   0        0        0      679 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/start.py
--rw-r--r--   0        0        0        1 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/__init__.py
--rw-r--r--   0        0        0     9162 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/args.py
--rw-r--r--   0        0        0     9035 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/auth.py
--rw-r--r--   0        0        0     6158 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/binaries.py
--rw-r--r--   0        0        0    10680 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/config.py
--rw-r--r--   0        0        0      257 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/console.py
--rw-r--r--   0        0        0      993 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/dates.py
--rw-r--r--   0        0        0    19571 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/download.py
--rw-r--r--   0        0        0      609 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/encoding.py
--rw-r--r--   0        0        0     2865 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/exit.py
--rw-r--r--   0        0        0     3137 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/filters.py
--rw-r--r--   0        0        0     5622 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/logger.py
--rw-r--r--   0        0        0     7654 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/paths.py
--rw-r--r--   0        0        0     3073 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/profiles.py
--rw-r--r--   0        0        0      397 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/semaphoreDelayed.py
--rw-r--r--   0        0        0     1358 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/separate.py
--rw-r--r--   0        0        0      554 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/stdout.py
--rw-r--r--   0        0        0     6042 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/userselector.py
--rw-r--r--   0        0        0     1520 2023-06-15 14:23:54.123770 ofscraper-2.4.1/pyproject.toml
--rw-r--r--   0        0        0     6607 1970-01-01 00:00:00.000000 ofscraper-2.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-16 18:24:54.342140 ofscraper-2.4.3/LICENSE
+-rw-r--r--   0        0        0     5201 2023-06-16 18:24:54.342140 ofscraper-2.4.3/README.md
+-rw-r--r--   0        0        0      607 2023-06-16 18:24:54.346140 ofscraper-2.4.3/ofscraper/__init__.py
+-rw-r--r--   0        0        0      999 2023-06-16 18:24:54.346140 ofscraper-2.4.3/ofscraper/__version__.py
+-rw-r--r--   0        0        0        1 2023-06-16 18:24:54.346140 ofscraper-2.4.3/ofscraper/api/__init__.py
+-rw-r--r--   0        0        0     7066 2023-06-16 18:24:54.346140 ofscraper-2.4.3/ofscraper/api/archive.py
+-rw-r--r--   0        0        0     3944 2023-06-16 18:24:54.346140 ofscraper-2.4.3/ofscraper/api/highlights.py
+-rw-r--r--   0        0        0     1067 2023-06-16 18:24:54.346140 ofscraper-2.4.3/ofscraper/api/init.py
+-rw-r--r--   0        0        0     2343 2023-06-16 18:24:54.346140 ofscraper-2.4.3/ofscraper/api/me.py
+-rw-r--r--   0        0        0     6592 2023-06-16 18:24:54.346140 ofscraper-2.4.3/ofscraper/api/messages.py
+-rw-r--r--   0        0        0     8529 2023-06-16 18:24:54.346140 ofscraper-2.4.3/ofscraper/api/paid.py
+-rw-r--r--   0        0        0     4576 2023-06-16 18:24:54.346140 ofscraper-2.4.3/ofscraper/api/pinned.py
+-rw-r--r--   0        0        0    11162 2023-06-16 18:24:54.346140 ofscraper-2.4.3/ofscraper/api/posts.py
+-rw-r--r--   0        0        0     3593 2023-06-16 18:24:54.346140 ofscraper-2.4.3/ofscraper/api/profile.py
+-rw-r--r--   0        0        0     3047 2023-06-16 18:24:54.346140 ofscraper-2.4.3/ofscraper/api/subscriptions.py
+-rw-r--r--   0        0        0     7712 2023-06-16 18:24:54.346140 ofscraper-2.4.3/ofscraper/api/timeline.py
+-rw-r--r--   0        0        0    31071 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/commands/check.py
+-rwxr-xr-x   0        0        0    14029 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/commands/scraper.py
+-rw-r--r--   0        0        0     5769 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/constants.py
+-rw-r--r--   0        0        0        1 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/db/__init__.py
+-rw-r--r--   0        0        0     8581 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/db/operations.py
+-rw-r--r--   0        0        0     3253 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/db/queries.py
+-rw-r--r--   0        0        0        1 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/interaction/__init__.py
+-rw-r--r--   0        0        0     4768 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/interaction/like.py
+-rw-r--r--   0        0        0     1364 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/prompt model.md
+-rw-r--r--   0        0        0      696 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/prompts/prompt_strings.py
+-rw-r--r--   0        0        0     6754 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/prompts/prompt_validators.py
+-rw-r--r--   0        0        0    27230 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/prompts/prompts.py
+-rw-r--r--   0        0        0      679 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/start.py
+-rw-r--r--   0        0        0        1 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/__init__.py
+-rw-r--r--   0        0        0     9292 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/args.py
+-rw-r--r--   0        0        0     9035 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/auth.py
+-rw-r--r--   0        0        0     6158 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/binaries.py
+-rw-r--r--   0        0        0    10680 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/config.py
+-rw-r--r--   0        0        0      257 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/console.py
+-rw-r--r--   0        0        0      993 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/dates.py
+-rw-r--r--   0        0        0    19690 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/download.py
+-rw-r--r--   0        0        0      609 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/encoding.py
+-rw-r--r--   0        0        0     2865 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/exit.py
+-rw-r--r--   0        0        0     3155 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/filters.py
+-rw-r--r--   0        0        0     5622 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/logger.py
+-rw-r--r--   0        0        0     9870 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/of.py
+-rw-r--r--   0        0        0     7654 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/paths.py
+-rw-r--r--   0        0        0     3073 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/profiles.py
+-rw-r--r--   0        0        0      399 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/semaphoreDelayed.py
+-rw-r--r--   0        0        0     1358 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/separate.py
+-rw-r--r--   0        0        0      554 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/stdout.py
+-rw-r--r--   0        0        0     6042 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/userselector.py
+-rw-r--r--   0        0        0     1520 2023-06-16 18:25:27.978646 ofscraper-2.4.3/pyproject.toml
+-rw-r--r--   0        0        0     6607 1970-01-01 00:00:00.000000 ofscraper-2.4.3/PKG-INFO
```

### Comparing `ofscraper-2.4.1/LICENSE` & `ofscraper-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.1/README.md` & `ofscraper-2.4.3/README.md`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.1/ofscraper/__init__.py` & `ofscraper-2.4.3/ofscraper/__init__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.1/ofscraper/__version__.py` & `ofscraper-2.4.3/ofscraper/__version__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.1/ofscraper/api/archive.py` & `ofscraper-2.4.3/ofscraper/api/archive.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.1/ofscraper/api/highlights.py` & `ofscraper-2.4.3/ofscraper/api/highlights.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.1/ofscraper/api/init.py` & `ofscraper-2.4.3/ofscraper/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.1/ofscraper/api/me.py` & `ofscraper-2.4.3/ofscraper/api/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.1/ofscraper/api/messages.py` & `ofscraper-2.4.3/ofscraper/api/messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 import arrow
 import ofscraper.constants as constants
 import ofscraper.utils.auth as auth
 import ofscraper.utils.paths as paths
 from ..utils import auth
 import ofscraper.utils.console as console
 from ofscraper.utils.semaphoreDelayed import semaphoreDelayed
+import ofscraper.utils.args as args_
+
 
 from diskcache import Cache
 cache = Cache(paths.getcachepath())
 log=logging.getLogger(__package__)
 attempt = contextvars.ContextVar("attempt")
 
 sem = semaphoreDelayed(constants.MAX_SEMAPHORE)
@@ -54,15 +56,15 @@
 
     tasks=[]
     responseArray=[]
     page_count=0
     #require a min num of posts to be returned
     min_posts=50
     with Live(progress_group, refresh_per_second=constants.refreshScreen,console=console.shared_console): 
-        oldmessages=cache.get(f"messages_{model_id}",default=[]) 
+        oldmessages=cache.get(f"messages_{model_id}",default=[]) if not args_.getargs().no_cache else []
         oldmsgset=set(map(lambda x:x.get("id"),oldmessages))
         log.debug(f"[bold]Messages Cache[/bold] {len(oldmessages)} found")
         oldmessages=list(filter(lambda x:x.get("createdAt")!=None,oldmessages))
         postedAtArray=list(map(lambda x:x["id"],sorted(oldmessages,key=lambda x:arrow.get(x["createdAt"]).float_timestamp,reverse=True)))
```

### Comparing `ofscraper-2.4.1/ofscraper/api/paid.py` & `ofscraper-2.4.3/ofscraper/api/paid.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,23 +92,23 @@
     attempt.set(attempt.get(0) + 1)
     
     await sem.acquire()
     task=job_progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}",visible=True)
     async with httpx.AsyncClient(http2=True, headers=headers, follow_redirects=True) as c:
         auth.add_cookies(c)
         url = constants.purchased_contentEP.format(offset,username)
-        offset += 10
         c.headers.update(auth.create_sign(url, headers))
         r = await c.get(url, timeout=None)
         sem.release()
     if not r.is_error:
         attempt.set(0)
-        if "hasMore" in r.json() and r.json()['hasMore']:
-            tasks.append(asyncio.create_task(scrape_paid(username,offset=offset)))
         media=list(filter(lambda x:isinstance(x,list),r.json().values()))[0]
+        if "hasMore" in r.json() and r.json()['hasMore']:
+            offset += len(media)-3
+            tasks.append(asyncio.create_task(scrape_paid(username,job_progress,offset=offset)))
         job_progress.remove_task(task)
 
     else:
         log.debug(f"[bold]paid request status code:[/bold]{r.status_code}")
         log.debug(f"[bold]paid response:[/bold] {r.content.decode()}")
         log.debug(f"[bold]paid headers:[/bold] {r.headers}")
         job_progress.remove_task(task)
@@ -128,15 +128,15 @@
 
     output=[]
     min_posts=100
     global tasks
     tasks=[]
     page_count=0
     with Live(progress_group, refresh_per_second=5,console=console.shared_console):
-        allpaid=cache.get(f"purchased_all",default=[])
+        allpaid=cache.get(f"purchased_all",default=[]) if not args_.getargs().no_cache else []
         log.debug(f"[bold]ALl Paid Cache[/bold] {len(allpaid)} found")
         
       
         if len(allpaid)>min_posts:
             splitArrays=[i for i in range(0, len(allpaid), min_posts)]
             #use the previous split for timesamp
             tasks.append(asyncio.create_task(scrape_all_paid(job_progress,offset=0,count=0,required=0)))
```

### Comparing `ofscraper-2.4.1/ofscraper/api/pinned.py` & `ofscraper-2.4.3/ofscraper/api/pinned.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.1/ofscraper/api/posts.py` & `ofscraper-2.4.3/ofscraper/api/posts.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,15 +324,15 @@
 
     @property
     def count(self):
         return self._count+1
 
     @property
     def filename(self):
-        if not self.url or self.mpd:
+        if not self.url and not self.mpd:
             return None
         elif not self.responsetype=="Profile":
             return  re.sub("\.mpd$","",(self.url or self.mpd).split('.')[-2].split('/')[-1].strip("/,.;!_-@#$%^&*()+\\ "))
         else:
             filename= re.sub("\.mpd$","",(self.url or self.mpd).split('.')[-2].split('/')[-1].strip("/,.;!_-@#$%^&*()+\\ "))
             return f"{filename}_{arrow.get(self.date).format(config.get_date(config.read_config()))}"
```

### Comparing `ofscraper-2.4.1/ofscraper/api/profile.py` & `ofscraper-2.4.3/ofscraper/api/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.1/ofscraper/api/subscriptions.py` & `ofscraper-2.4.3/ofscraper/api/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.1/ofscraper/api/timeline.py` & `ofscraper-2.4.3/ofscraper/api/timeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 import time
 import asyncio
-from ofscraper.utils.semaphoreDelayed import semaphoreDelayed
 import logging
 import contextvars
 import math
 import httpx
 from tenacity import retry,stop_after_attempt,wait_random
 from rich.progress import Progress
 from rich.progress import (
@@ -22,18 +21,18 @@
 )
 from rich.panel import Panel
 from rich.console import Group
 from rich.live import Live
 from rich.style import Style
 import arrow
 import ofscraper.constants as constants
+from ofscraper.utils.semaphoreDelayed import semaphoreDelayed
 from ..utils import auth
 from ..utils.paths import getcachepath
 import ofscraper.utils.console as console
-import ofscraper.utils.config as config_
 import ofscraper.utils.args as args_
 
 from diskcache import Cache
 cache = Cache(getcachepath())
 log=logging.getLogger(__package__)
 attempt = contextvars.ContextVar("attempt")
 
@@ -102,15 +101,15 @@
     global tasks
     tasks=[]
     min_posts=50
     responseArray=[]
     page_count=0
     with Live(progress_group, refresh_per_second=5,console=console.shared_console): 
 
-        oldtimeline=cache.get(f"timeline_{model_id}",default=[])
+        oldtimeline=cache.get(f"timeline_{model_id}",default=[]) if not args_.getargs().no_cache else []
         oldtimeset=set(map(lambda x:x.get("id"),oldtimeline))
         log.debug(f"[bold]Timeline Cache[/bold] {len(oldtimeline)} found")
         oldtimeline=list(filter(lambda x:x.get("postedAtPrecise")!=None,oldtimeline))
         postedAtArray=sorted(list(map(lambda x:float(x["postedAtPrecise"]),oldtimeline)))
         filteredArray=list(filter(lambda x:x>=(args_.getargs().after or arrow.get(0)).float_timestamp,postedAtArray))
```

### Comparing `ofscraper-2.4.1/ofscraper/commands/check.py` & `ofscraper-2.4.3/ofscraper/commands/check.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.1/ofscraper/constants.py` & `ofscraper-2.4.3/ofscraper/constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.1/ofscraper/db/operations.py` & `ofscraper-2.4.3/ofscraper/db/operations.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.1/ofscraper/db/queries.py` & `ofscraper-2.4.3/ofscraper/db/queries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.1/ofscraper/interaction/like.py` & `ofscraper-2.4.3/ofscraper/interaction/like.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import random
 import time
 import logging
 from typing import Union
 import asyncio
 import httpx
 
-log=logging.getLogger(__package__)
+from tenacity import retry,stop_after_attempt,wait_random
 
 from rich.progress import Progress
 from rich.progress import (
     Progress,
     MofNCompleteColumn,
     BarColumn,
     TextColumn,
@@ -28,21 +28,38 @@
 from rich.style import Style
 from ..api import timeline
 from ..constants import favoriteEP, postURL
 from ..utils import auth
 import ofscraper.api.archive as archive
 import ofscraper.api.pinned as pinned
 import ofscraper.utils.console as console
+import ofscraper.constants as constants
+from ofscraper.utils.semaphoreDelayed import semaphoreDelayed
+import ofscraper.prompts.prompts as prompts
+
+sem = semaphoreDelayed(1)
+log=logging.getLogger(__package__)
+import ofscraper.utils.args as args_
 
 
 
 def get_posts(headers, model_id):
-    pinned_posts = asyncio.run(pinned.get_pinned_post(headers, model_id))
-    timeline_posts = asyncio.run(timeline.get_timeline_post(headers, model_id))
-    archived_posts = asyncio.run(archive.get_archived_post(headers, model_id))
+    pinned_posts=[]
+    timeline_posts=[]
+    archived_posts=[]
+    args=args_.getargs()
+
+    args.posts = list(map(lambda x:x.capitalize(),(args.posts or prompts.like_areas_prompt())
+    ))
+    if ('Pinned' in args.posts or 'All' in args.posts):
+        pinned_posts = asyncio.run(pinned.get_pinned_post(headers, model_id))
+    if ('Timeline' in args.posts or 'All' in args.posts):
+        timeline_posts = asyncio.run(timeline.get_timeline_post(headers, model_id))
+    if ('Archived' in args.posts or 'All' in args.posts):
+        archived_posts = asyncio.run(archive.get_archived_post(headers, model_id))
     log.debug(f"[bold]Number of Post Found[/bold] {len(pinned_posts) + len(timeline_posts) + len(archived_posts)}")
     return pinned_posts + timeline_posts + archived_posts
 
 
 def filter_for_unfavorited(posts: list) -> list:
     output=list(filter(lambda x:x.get("isFavorite")==False,posts))
     log.debug(f"[bold]Number of unliked post[/bold] {len(output)}")
@@ -61,55 +78,62 @@
 def get_post_ids(posts: list) -> list:
     valid_post=list(filter(lambda x:x.get("isOpened")==True,posts))
     return list(map(lambda x:x.get("id"),valid_post))
    
 
 
 def like(headers, model_id, username, ids: list):
-    _like(headers, model_id, username, ids, True)
+    asyncio.run(_like(headers, model_id, username, ids, True))
 
 
 def unlike(headers, model_id, username, ids: list):
-    _like(headers, model_id, username, ids, False)
+    asyncio.run(_like(headers, model_id, username, ids, False))
+
+
 
 
-def _like(headers, model_id, username, ids: list, like_action: bool):
+async def _like(headers, model_id, username, ids: list, like_action: bool):
     title = "Liking" if like_action else "Unliking"
+    global sem
+    sem.delay=3
     with Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("{task.description}"),BarColumn(),MofNCompleteColumn(),console=console.shared_console) as overall_progress:
+        tasks=[]
         task1=overall_progress.add_task(f"{title} posts...\n",total=len(ids))
-        for i in ids:
-            with httpx.Client(http2=True, headers=headers) as c:
-                url = favoriteEP.format(i, model_id)
-
-                auth.add_cookies(c)
-                c.headers.update(auth.create_sign(url, headers))
-
-                retries = 0
-                while retries <= 1:
-                    time.sleep(random.uniform(0.8, 0.9))
-                    retries += 1
-                    try:
-                        r = c.post(url)
-                        if not r.is_error or r.status_code == 400:
-                            log.debug(f"ID: {i} Performed {'like' if like_action==True else 'unlike'} action")
-                            overall_progress.update(task1,advance=1,refresh=True)
-                            break
-                        else:
-                            _handle_err(r, postURL.format(i, username))
-                    except httpx.TransportError as e:
-                        _handle_err(e, postURL.format(i, username))
-        overall_progress.remove_task(task1)
-
-def _handle_err(param: Union[httpx.Response, httpx.TransportError], url: str) -> str:
-    message = 'unable to execute action'
-    status = ''
-    try:
-        if isinstance(param, httpx.Response):
-            json = param.json()
-            if 'error' in json and 'message' in json['error']:
-                message = json['error']['message']
-            status = f'STATUS CODE {param.status_code}: '
-        else:
-            message = str(param)
-    except:
-        pass
-    log.info(f'{status}{message}, post at {url}')
+
+        [tasks.append(asyncio.create_task(_like_request(headers,id,model_id,username)))
+            for id in ids]
+        for count,coro in enumerate(asyncio.as_completed(tasks)):
+                id=await coro
+                log.debug(f"ID: {id} Performed {'like' if like_action==True else 'unlike'} action")
+                if count+1%60==0 and count+1%50==0:
+                    sem.delay=15
+                elif count+1%60==0:
+                    sem.delay=3
+                elif count+1%50==0:
+                    sem.delay=30  
+                 
+                overall_progress.update(task1,advance=1,refresh=True)
+
+        
+        
+
+@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
+async def _like_request(headers,id,model_id,username):
+    async with sem:
+        with httpx.Client(http2=True, headers=headers) as c:
+            url = favoriteEP.format(id, model_id)
+            auth.add_cookies(c)
+            c.headers.update(auth.create_sign(url, headers))
+            r = c.post(url)
+    
+            if not r.is_error or r.status_code == 400:
+                return id
+                     
+            
+            log.debug(f"[bold]timeline request status code:[/bold]{r.status_code}")
+            log.debug(f"[bold]timeline response:[/bold] {r.content.decode()}")
+            log.debug(f"[bold]timeline headers:[/bold] {r.headers}")
+            r.raise_for_status()
+
+
+
+
```

### Comparing `ofscraper-2.4.1/ofscraper/prompt model.md` & `ofscraper-2.4.3/ofscraper/prompt model.md`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.1/ofscraper/prompts/prompt_validators.py` & `ofscraper-2.4.3/ofscraper/prompts/prompt_validators.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.1/ofscraper/prompts/prompts.py` & `ofscraper-2.4.3/ofscraper/prompts/prompts.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,51 @@
 
         }
     ]
     answers = prompt(questions)
     return answers[name]
 
 
+def like_areas_prompt() -> list:
+    name = 'areas'
 
+    questions = [
+        {
+            'type': 'checkbox',
+            'qmark': '[?]',
+            'name': name,
+            'message': 'Which area(s) would you to perform like/unlike actions on',
+             "validate":prompt_validators.emptyListValidator(),
+            'choices': [
+                Choice('Timeline'),
+                Choice('Pinned'),
+                Choice('Archived'),
+            ]
+            ,"instruction":prompt_strings.CHECKLISTINSTRUCTIONS,
+
+        }
+    ]
+    answers = prompt(questions)
+    return answers[name]
+
+def scrape_paid_prompt():
+    questions = [
+        {
+            'type': 'list',
+            'message': "Scrape entire paid page",
+            'choices':[Choice(True,"True"),Choice(False,"False",enabled=True)],
+            'long_instruction': prompt_strings.SCRAPE_PAID,
+            "default":False
+
+        },
+
+    ]
+
+    answer = prompt(questions)
+    return answer[0]
 
 def auth_prompt(auth) -> dict:
     questions = [
         {
             'type': 'input',
             'name': 'sess',
             'message': 'Enter your sess cookie:',
@@ -128,27 +164,27 @@
 def ask_make_auth_prompt() -> bool:
     name = 'make_auth'
 
     questions = [
         {
             'type': 'confirm',
             'name': name,
-            'message': "It doesn't seem you have an `auth.json` file. Would you like to make one?",
+            'message': "You don't seem to have an `auth.json` file. Would you like to make one?",
         }
     ]
 
     answer = prompt(questions)
     return answer[name]
 
 def browser_prompt()->str:
     pythonver=float(f"{sys.version_info[0]}.{sys.version_info[1]}")
     msg="Select how to retrive auth information"
 
     if pythonver<3.9 or pythonver>=3.11:
-        console.print("\nNote: Browser Extractions only works with default Profile\n\n")
+        console.print("\nNote: Browser Extractions only works with default browser profile\n\n")
         questions = [
             {
                 'type': 'list',
                 'message':msg ,
                 'choices':["Enter Each Field Manually","Paste From Cookie Helper", Separator(line="-----------\nBrowser Extractions"),"Chrome","Chromium","Firefox","Opera","Opera GX","Edge","Chromium","Brave","Vivaldi","Safari"],
                 "default":"Enter Each Field Manually",
 
@@ -676,15 +712,15 @@
                                                                 renewal=(args_.getargs().renewal or "Both").capitalize()
 
                                                                 
                                                                 ),
 
                                                                  
         choices=choices,
-        transformer=lambda result:",".join(map(lambda x:x.split(" ")[0],result)),
+        transformer=lambda result:",".join(map(lambda x:x.split(" ")[1],result)),
         multiselect=True,
         validate=prompt_validators.emptyListValidator(),
         prompt='Filter: ',
         marker="\u25c9 ",
         marker_pl="\u25cb ",
         message= "Which models do you want to scrape\n:",
         mandatory=False,
```

### Comparing `ofscraper-2.4.1/ofscraper/start.py` & `ofscraper-2.4.3/ofscraper/start.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.1/ofscraper/utils/args.py` & `ofscraper-2.4.3/ofscraper/utils/args.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,17 @@
     post.add_argument("-sk","--skip-timed",default=None,help="skip promotional or tempory post",action="store_true")
     post.add_argument(
         '-ft', '--filter', help = 'Filter post by provide regex\nNote if you include any uppercase characters the search will be case-sensitive',default=".*",required=False,type = str
     )
     post.add_argument(
         '-sp', '--scrape-paid', help = 'scrape the entire paid page for content. This can take a very long time',default=False,required=False,action="store_true"
     )
+    post.add_argument(
+        '-nc', '--no-cache', help = 'disable cache',default=False,required=False,action="store_true"
+    )
 
      #Filters for accounts
     filters=parser.add_argument_group("filters",description="Filters out usernames based on selected parameters")
     
     filters.add_argument(
         '-at', '--account-type', help = 'Filter Free or paid accounts\npaid and free correspond to your original price, and not the renewal price',default=None,required=False,type = str.lower,choices=["paid","free"]
     )
```

### Comparing `ofscraper-2.4.1/ofscraper/utils/auth.py` & `ofscraper-2.4.3/ofscraper/utils/auth.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.1/ofscraper/utils/binaries.py` & `ofscraper-2.4.3/ofscraper/utils/binaries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.1/ofscraper/utils/config.py` & `ofscraper-2.4.3/ofscraper/utils/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.1/ofscraper/utils/dates.py` & `ofscraper-2.4.3/ofscraper/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.1/ofscraper/utils/download.py` & `ofscraper-2.4.3/ofscraper/utils/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,46 +52,45 @@
 import ofscraper.utils.auth as auth
 import ofscraper.constants as constants
 import ofscraper.utils.dates as dates
 import ofscraper.utils.logger as logger
 import ofscraper.utils.console as console
 import ofscraper.utils.stdout as stdout
 import ofscraper.utils.config as config_
+import ofscraper.utils.args as args_
 
 from diskcache import Cache
 
 cache = Cache(paths.getcachepath())
 attempt = contextvars.ContextVar("attempt")
 log=logging.getLogger(__package__)
 from ofscraper.utils.semaphoreDelayed import semaphoreDelayed
 sem = semaphoreDelayed(config_.get_threads(config_.read_config()))
 
 
-async def process_dicts(username, model_id, medialist,forced=False):
+async def process_dicts(username, model_id, medialist):
     with stdout.lowstdout():
         overall_progress=Progress(  TextColumn("{task.description}"),
         BarColumn(),TaskProgressColumn(),TimeElapsedColumn())
         job_progress=Progress(TextColumn("{task.description}",table_column=Column(ratio=2)),BarColumn(),
         TaskProgressColumn(),TimeRemainingColumn(),TransferSpeedColumn(),TotalFileSizeColumn())
         progress_group = Group(
         overall_progress
         , Panel(Group(job_progress,fit=True)))
         with Live(progress_group, refresh_per_second=constants.refreshScreen,console=console.shared_console):    
-                if not forced:
+                if not args_.getargs().dupe:
                     media_ids = set(operations.get_media_ids(model_id,username))
                     medialist = seperate.separate_by_id(medialist, media_ids)
                     medialist=seperate.seperate_avatars(medialist)
-
                     log.info(f"Skipping previously downloaded\nMedia left for download {len(medialist)}")
                 else:
                     log.info("forcing all downloads")
                 file_size_limit = config_.get_filesize()
                 global sem
-               
-            
+                  
                 aws=[]
                 photo_count = 0
                 video_count = 0
                 audio_count=0
                 skipped = 0
                 total_bytes_downloaded = 0
                 data = 0
@@ -206,15 +205,15 @@
         log.debug(f"Media:{ele.id} Post:{ele.postid} Downloading with protected media downloader")      
         log.debug(f"Media:{ele.id} Post:{ele.postid} Attempting to download media {ele.filename} with {ele.mpd}")
         video = None
         audio = None
         base_url=re.sub("[0-9a-z]*\.mpd$","",ele.mpd,re.IGNORECASE)
         mpd=await ele.parse_mpd
         path_to_file = paths.trunicate(pathlib.Path(path,f'{createfilename(ele,username,model_id,"mp4")}'))
-        temp_path=paths.trunicate(pathlib.Path(path,f"{ele.id}.mkv"))
+        temp_path=paths.trunicate(pathlib.Path(path,f"tem{ele.id or ele.filename}.mkv"))
 
         for period in mpd.periods:
             for adapt_set in filter(lambda x:x.mime_type=="video/mp4",period.adaptation_sets):             
                 kId=None
                 for prot in adapt_set.content_protections:
                     if prot.value==None:
                         kId = prot.pssh[0].pssh 
@@ -288,14 +287,15 @@
     temp_path.unlink(missing_ok=True)
     t=subprocess.run([config_.get_ffmpeg(config_.read_config()),"-i",str(video["path"]),"-i",str(audio["path"]),"-c","copy",str(temp_path)],stdout=subprocess.PIPE,stderr=subprocess.PIPE)
     if t.stderr.decode().find("Output")==-1:
         log.debug(t.stdout.decode())
         log.debug(t.stderr.decode())
     video["path"].unlink(missing_ok=True)
     audio["path"].unlink(missing_ok=True)
+    log.debug(f"Moving intermediate path {temp_path} to {path_to_file}")
     shutil.move(temp_path,path_to_file)
     if ele.postdate:
         newDate=dates.convert_local_time(ele.postdate)
         log.debug(f"Media:{ele.id} Post:{ele.postid} Attempt to set Date to {arrow.get(newDate).format('YYYY-MM-DD HH:mm')}")  
         set_time(path_to_file,newDate )
         log.debug(f"Media:{ele.id} Post:{ele.postid} Date set to {arrow.get(path_to_file.stat().st_mtime).format('YYYY-MM-DD HH:mm')}")  
     if ele.id:
```

### Comparing `ofscraper-2.4.1/ofscraper/utils/encoding.py` & `ofscraper-2.4.3/ofscraper/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.1/ofscraper/utils/exit.py` & `ofscraper-2.4.3/ofscraper/utils/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.1/ofscraper/utils/filters.py` & `ofscraper-2.4.3/ofscraper/utils/filters.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,16 +42,16 @@
     return list(sorted(output,key=lambda x:x.date,reverse=True))
 
 
 
     
 def timeline_array_filter(posts):
     out=[]
-    undated=filter(lambda x:x.get("postedAt")==None,posts)
-    dated=filter(lambda x:x.get("postedAt")!=None,posts)
+    undated=list(filter(lambda x:x.get("postedAt")==None,posts))
+    dated=list(filter(lambda x:x.get("postedAt")!=None,posts))
     dated=sorted(dated,key=lambda x:arrow.get(x.get("postedAt")))
     if args.before:
         dated=list(filter(lambda x:arrow.get(x.get("postedAt"))<=args.before,dated))
     if args.after:
          dated=list(filter(lambda x:arrow.get(x.get("postedAt"))>=args.after,dated))
     out.extend(undated)
     out.extend(dated)
@@ -70,18 +70,18 @@
     else:
         log.info("The settings you picked for the filter are not valid\nNot Filtering")
         log.debug(f"[bold]Combined Media Count Filtered:[/bold] {len(media)}")
     return media
 
 def posts_date_filter(media):
     if args.before:
-        media=filter(lambda x:x.postdate==None or arrow.get(x.postdate)<=args.before,media)
+        media=list(filter(lambda x:x.postdate==None or arrow.get(x.postdate)<=args.before,media))
     if args.after:
-        media=filter(lambda x:x.postdate==None or arrow.get(x.postdate)>=args.after,media)
-    return list(media)
+        media=list(filter(lambda x:x.postdate==None or arrow.get(x.postdate)>=args.after,media))
+    return media
 
 def post_timed_filter(media):
     if args.skip_timed:
         return list(filter(lambda x:not x.expires,media))
     return media
 def post_user_filter(media):
     userfilter=args.filter
```

### Comparing `ofscraper-2.4.1/ofscraper/utils/logger.py` & `ofscraper-2.4.3/ofscraper/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.1/ofscraper/utils/paths.py` & `ofscraper-2.4.3/ofscraper/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.1/ofscraper/utils/profiles.py` & `ofscraper-2.4.3/ofscraper/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.1/ofscraper/utils/separate.py` & `ofscraper-2.4.3/ofscraper/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.1/ofscraper/utils/stdout.py` & `ofscraper-2.4.3/ofscraper/utils/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.1/ofscraper/utils/userselector.py` & `ofscraper-2.4.3/ofscraper/utils/userselector.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.1/pyproject.toml` & `ofscraper-2.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "2.4.1"
+version = "2.4.3"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4"
 httpx = {extras = ["http2"], version = "^0.23.3"}
```

### Comparing `ofscraper-2.4.1/PKG-INFO` & `ofscraper-2.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 2.4.1
+Version: 2.4.3
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >=3.7.0,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

