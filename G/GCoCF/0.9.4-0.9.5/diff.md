# Comparing `tmp/gcocf-0.9.4.tar.gz` & `tmp/gcocf-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcocf-0.9.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gcocf-0.9.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gcocf-0.9.4.tar` & `gcocf-0.9.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      124 2023-06-16 16:22:47.068422 gcocf-0.9.4/.example.envrc
--rw-r--r--   0        0        0      669 2023-06-16 16:22:47.072422 gcocf-0.9.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      644 2023-06-16 16:22:47.072422 gcocf-0.9.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      501 2023-06-16 16:22:47.072422 gcocf-0.9.4/.github/dependabot.yml
--rw-r--r--   0        0        0     1076 2023-06-16 16:22:47.072422 gcocf-0.9.4/.github/pull_request_template.md
--rw-r--r--   0        0        0     1691 2023-06-16 16:22:47.072422 gcocf-0.9.4/.github/workflows/Testing.yml
--rw-r--r--   0        0        0       87 2023-06-16 16:22:47.072422 gcocf-0.9.4/.gitignore
--rw-r--r--   0        0        0     5224 2023-06-16 16:22:47.072422 gcocf-0.9.4/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      203 2023-06-16 16:22:47.072422 gcocf-0.9.4/CONTRIBUTING.md
--rw-r--r--   0        0        0      273 2023-06-16 16:22:47.072422 gcocf-0.9.4/Dockerfile
--rw-r--r--   0        0        0      144 2023-06-16 16:22:47.072422 gcocf-0.9.4/GCoCF/__init__.py
--rwxr-xr-x   0        0        0    10880 2023-06-16 16:22:47.072422 gcocf-0.9.4/GCoCF/__main__.py
--rw-r--r--   0        0        0     2224 2023-06-16 16:22:47.072422 gcocf-0.9.4/GCoCF/api.py
--rw-r--r--   0        0        0     6488 2023-06-16 16:22:47.072422 gcocf-0.9.4/GCoCF/formatters.py
--rw-r--r--   0        0        0     2369 2023-06-16 16:22:47.072422 gcocf-0.9.4/GCoCF/locales/messages.pot
--rw-r--r--   0        0        0    11947 2023-06-16 16:22:47.072422 gcocf-0.9.4/GCoCF/models.py
--rw-r--r--   0        0        0     1009 2023-06-16 16:22:47.072422 gcocf-0.9.4/GCoCF/notifiers.py
--rw-r--r--   0        0        0     1378 2023-06-16 16:22:47.072422 gcocf-0.9.4/GCoCF/utils.py
--rw-r--r--   0        0        0     1070 2023-06-16 16:22:47.072422 gcocf-0.9.4/LICENSE.txt
--rw-r--r--   0        0        0       34 2023-06-16 16:22:47.072422 gcocf-0.9.4/README.md
--rw-r--r--   0        0        0     2495 2023-06-16 16:22:47.072422 gcocf-0.9.4/SECURITY.md
--rw-r--r--   0        0        0    41692 2023-06-16 16:22:47.072422 gcocf-0.9.4/data/full_destruction.json
--rw-r--r--   0        0        0    77643 2023-06-16 16:22:47.072422 gcocf-0.9.4/data/inWar_40.json
--rw-r--r--   0        0        0     1059 2023-06-16 16:22:47.072422 gcocf-0.9.4/data/notInWar.json
--rw-r--r--   0        0        0    24207 2023-06-16 16:22:47.072422 gcocf-0.9.4/data/op_full_destruction.json
--rw-r--r--   0        0        0    98300 2023-06-16 16:22:47.072422 gcocf-0.9.4/data/warEnded_50.json
--rw-r--r--   0        0        0      832 2023-06-16 16:22:47.072422 gcocf-0.9.4/pyproject.toml
--rw-r--r--   0        0        0       54 2023-06-16 16:22:47.072422 gcocf-0.9.4/requirements.txt
--rw-r--r--   0        0        0    11544 2023-06-16 16:22:47.072422 gcocf-0.9.4/test_everything.py
--rw-r--r--   0        0        0      875 1970-01-01 00:00:00.000000 gcocf-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0      124 2023-06-17 07:10:07.058388 gcocf-0.9.5/.example.envrc
+-rw-r--r--   0        0        0      669 2023-06-17 07:10:07.058388 gcocf-0.9.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      644 2023-06-17 07:10:07.058388 gcocf-0.9.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      501 2023-06-17 07:10:07.058388 gcocf-0.9.5/.github/dependabot.yml
+-rw-r--r--   0        0        0     1076 2023-06-17 07:10:07.058388 gcocf-0.9.5/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1691 2023-06-17 07:10:07.058388 gcocf-0.9.5/.github/workflows/Testing.yml
+-rw-r--r--   0        0        0      103 2023-06-17 07:10:07.058388 gcocf-0.9.5/.gitignore
+-rw-r--r--   0        0        0     5224 2023-06-17 07:10:07.058388 gcocf-0.9.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      203 2023-06-17 07:10:07.058388 gcocf-0.9.5/CONTRIBUTING.md
+-rw-r--r--   0        0        0      273 2023-06-17 07:10:07.058388 gcocf-0.9.5/Dockerfile
+-rw-r--r--   0        0        0      144 2023-06-17 07:10:07.058388 gcocf-0.9.5/GCoCF/__init__.py
+-rwxr-xr-x   0        0        0    10649 2023-06-17 07:10:07.058388 gcocf-0.9.5/GCoCF/__main__.py
+-rw-r--r--   0        0        0     2224 2023-06-17 07:10:07.058388 gcocf-0.9.5/GCoCF/api.py
+-rw-r--r--   0        0        0    10419 2023-06-17 07:10:07.058388 gcocf-0.9.5/GCoCF/formatters.py
+-rw-r--r--   0        0        0     2369 2023-06-17 07:10:07.058388 gcocf-0.9.5/GCoCF/locales/messages.pot
+-rw-r--r--   0        0        0    12638 2023-06-17 07:10:07.058388 gcocf-0.9.5/GCoCF/models.py
+-rw-r--r--   0        0        0     1009 2023-06-17 07:10:07.058388 gcocf-0.9.5/GCoCF/notifiers.py
+-rw-r--r--   0        0        0     1378 2023-06-17 07:10:07.058388 gcocf-0.9.5/GCoCF/utils.py
+-rw-r--r--   0        0        0     1070 2023-06-17 07:10:07.058388 gcocf-0.9.5/LICENSE.txt
+-rw-r--r--   0        0        0     1303 2023-06-17 07:10:07.058388 gcocf-0.9.5/README.md
+-rw-r--r--   0        0        0     2495 2023-06-17 07:10:07.058388 gcocf-0.9.5/SECURITY.md
+-rw-r--r--   0        0        0    41692 2023-06-17 07:10:07.058388 gcocf-0.9.5/data/full_destruction.json
+-rw-r--r--   0        0        0    77643 2023-06-17 07:10:07.058388 gcocf-0.9.5/data/inWar_40.json
+-rw-r--r--   0        0        0     1059 2023-06-17 07:10:07.058388 gcocf-0.9.5/data/notInWar.json
+-rw-r--r--   0        0        0    24207 2023-06-17 07:10:07.058388 gcocf-0.9.5/data/op_full_destruction.json
+-rw-r--r--   0        0        0    98300 2023-06-17 07:10:07.062388 gcocf-0.9.5/data/warEnded_50.json
+-rw-r--r--   0        0        0      832 2023-06-17 07:10:07.062388 gcocf-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0       54 2023-06-17 07:10:07.062388 gcocf-0.9.5/requirements.txt
+-rw-r--r--   0        0        0    13950 2023-06-17 07:10:07.062388 gcocf-0.9.5/test_everything.py
+-rw-r--r--   0        0        0     2144 1970-01-01 00:00:00.000000 gcocf-0.9.5/PKG-INFO
```

### Comparing `gcocf-0.9.4/.github/ISSUE_TEMPLATE/bug_report.md` & `gcocf-0.9.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.4/.github/ISSUE_TEMPLATE/feature_request.md` & `gcocf-0.9.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.4/.github/pull_request_template.md` & `gcocf-0.9.5/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.4/.github/workflows/Testing.yml` & `gcocf-0.9.5/.github/workflows/Testing.yml`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.4/CODE_OF_CONDUCT.md` & `gcocf-0.9.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.4/GCoCF/__main__.py` & `gcocf-0.9.5/GCoCF/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python
 """GCoCF - Clash of Clans war moniting for Discord."""
 import os
 import time
+import discord
 import shelve
 import gettext
 import hashlib
 import logging
 
 import click
 
@@ -237,66 +238,64 @@
             self.send(msg)
             self.mark_msg_as_sent(msg_id)
 
     def send(self, msg):
         self.notifier.send(msg)
 
     def start(self):
-        """Send war news to telegram channel."""
+        """Send war news to Discord."""
+
+        last_summary_send_time = 0
+        msg_factory = MessageFactory(None, None, None)
+
         while True:
             try:
+                current_time = time.time()
                 leagueinfo = self.coc_api.get_currentleague(self.clan_tag)
                 if leagueinfo:
                     for previous_wartag in leagueinfo.get_previous_wartags():
                         self.update(wartag=previous_wartag)
                     current_war_tag = leagueinfo.get_current_wartag()
                     next_war_tag = leagueinfo.get_next_wartag()
                     if current_war_tag:
                         self.update(wartag=current_war_tag)
                     if next_war_tag:
                         self.update(wartag=next_war_tag)
                 else:
                     self.update()
+
+                # Send a summary message after each hour passed within the war
+                if current_time - last_summary_send_time >= 3600:
+                    if self.warinfo and self.warinfo.is_in_war():
+                        self.notifier.send(self.msg_factory.create_war_summary_msg())
+                        last_summary_send_time = current_time
+
                 time.sleep(POLL_INTERVAL)
+
             except Exception as err:
-                if '403' in str(err):
-                    # Check whether warlog is public
-                    if not self.coc_api.get_claninfo(self.clan_tag).is_warlog_public:
-                        print('Warlog must be public. Exiting.')
-                        self.notifier.send(_("Warlog must be public boss! ☠️"))
-                elif '500' in str(err):
-                    print('CoC internal server error, retrying.')
-                    # self.notifier.send(
-                    #     'CoC internal server error, retrying in {} seconds.'
-                    #     .format(POLL_INTERVAL * 10), silent=True)
-                    time.sleep(POLL_INTERVAL * 10)
-                    continue
-                elif '502' in str(err):
-                    print('CoC bad gateway, retrying.')
-                    # self.notifier.send(
-                    #     'CoC bad gateway, retrying in {} seconds.'
-                    #     .format(POLL_INTERVAL * 10), silent=True)
-                    time.sleep(POLL_INTERVAL * 10)
-                    continue
-                elif '503' in str(err):
-                    print('CoC maintenance error, retrying.')
-                    self.notifier.send(
-                        'CoC maintenance error, retrying in {} seconds.'
-                        .format(POLL_INTERVAL * 10), silent=True)
-                    time.sleep(POLL_INTERVAL * 10)
-                    continue
-                elif '504' in str(err):
-                    print('504 Gateway Timeout, retrying.')
-                    # self.notifier.send(
-                    #     '504 Gateway Timeout, retrying in {} seconds.'
-                    #     .format(POLL_INTERVAL * 10), silent=True)
-                    time.sleep(POLL_INTERVAL * 10)
-                    continue
+                try:
+                    error_message = None
+                    if '403' in str(err):
+                        # Check whether warlog is public
+                        if not self.coc_api.get_claninfo(self.clan_tag).is_warlog_public:
+                            error_message = _('Warlog must be public boss! ☠️')
+                    elif '500' in str(err):
+                        error_message = _('CoC internal server error, retrying.')
+                    elif '502' in str(err):
+                        error_message = _('CoC bad gateway, retrying.')
+                    elif '503' in str(err):
+                        error_message = _('CoC maintenance error, retrying.')
+                    elif '504' in str(err):
+                        error_message = _('504 Gateway Timeout, retrying.')
+
+                    if error_message:
+                        self.notifier.send(msg_factory.create_error_embed(error_message))
+                    else:
+                        self.notifier.send(msg_factory.create_error_embed(_("☠️ 😵 App is broken boss! Come over and fix me please!")))
 
-                else:
-                    self.notifier.send(
-                        _("☠️ 😵 App is broken boss! Come over and fix me please!"))
+                except Exception as e:
+                    raise Exception(str(e))
                 raise
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `gcocf-0.9.4/GCoCF/api.py` & `gcocf-0.9.5/GCoCF/api.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.4/GCoCF/locales/messages.pot` & `gcocf-0.9.5/GCoCF/locales/messages.pot`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.4/GCoCF/models.py` & `gcocf-0.9.5/GCoCF/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 
 class WarInfo(object):
     def __init__(self, wardata):
         self.data = wardata
         self.clan_members = {}
         self.opponent_members = {}
         self.players = {}
+        self.op_members = {}
         self.ordered_attacks = None
         self._populate()
 
     @property
     def state(self):
         return self.data['state']
 
@@ -123,23 +124,39 @@
             return
         for member in self.data['clan']['members']:
             self.clan_members[member['tag']] = member
             self.players[member['tag']] = member
         for opponent in self.data['opponent']['members']:
             self.opponent_members[opponent['tag']] = opponent
             self.players[opponent['tag']] = opponent
+            self.op_members[opponent['tag']] = opponent
+            
         self.ordered_attacks = self.get_ordered_attacks()
 
     def get_ordered_attacks(self):
         ordered_attacks = {}
         for player in self.players.values():
             for attack in self.get_player_attacks(player):
                 ordered_attacks[attack['order']] = (player, attack)
         return ordered_attacks
 
+    def get_last_attacks(self, max_attacks=5):
+        last_attacks = []
+        ordered_attacks = list(self.ordered_attacks.values())
+
+        for index in range(len(ordered_attacks) - 1, max(len(ordered_attacks) - max_attacks - 1, -1), -1):
+            player, attack = ordered_attacks[index]
+            attacker_tag = player['tag']
+            defender_tag = attack['defenderTag']
+            attacker = self.players[attacker_tag]
+            defender = self.players[defender_tag]
+            last_attacks.append({'attacker': attacker, 'defender': defender})
+
+        return last_attacks
+
     def get_player_attacks(self, player):
         if 'attacks' in player:
             return player['attacks']
         else:
             return []
 
     def get_player_info(self, tag):
```

### Comparing `gcocf-0.9.4/GCoCF/notifiers.py` & `gcocf-0.9.5/GCoCF/notifiers.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.4/GCoCF/utils.py` & `gcocf-0.9.5/GCoCF/utils.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.4/LICENSE.txt` & `gcocf-0.9.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.4/SECURITY.md` & `gcocf-0.9.5/SECURITY.md`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.4/data/full_destruction.json` & `gcocf-0.9.5/data/full_destruction.json`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.4/data/inWar_40.json` & `gcocf-0.9.5/data/inWar_40.json`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.4/data/notInWar.json` & `gcocf-0.9.5/data/notInWar.json`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.4/data/op_full_destruction.json` & `gcocf-0.9.5/data/op_full_destruction.json`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.4/data/warEnded_50.json` & `gcocf-0.9.5/data/warEnded_50.json`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.4/pyproject.toml` & `gcocf-0.9.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.4/test_everything.py` & `gcocf-0.9.5/test_everything.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 '''GCoCF tests.'''
 import os
 import json
+import discord
 import gettext
 import unittest
-from unittest.mock import MagicMock
+from unittest.mock import MagicMock, patch
+from discord.embeds import Embed
 
 from GCoCF.__main__ import WarMonitor
 from GCoCF.models import WarStats, ClanInfo, WarInfo, WarStats
 from GCoCF.formatters import MessageFactory
 from GCoCF.api import CoCAPI
-from GCoCF.notifiers import DiscordNotifier
+from GCoCF.notifiers import DiscordNotifier, DummyNotifier
 
 class ClanInfoTestCase(unittest.TestCase):
     def setUp(self):
         self.claninfo = ClanInfo({'location': {'name': 'Iran',
                                                'isCountry': 'true',
                                                'countryCode': 'IR'},
                                   'warWinStreak': 0,
@@ -220,15 +222,44 @@
     def setlocale_en(self):
         self._setlocale('en_US.UTF-8')
 
     def test_format_time_default(self):
         os.environ['LANG'] = 'en'
         os.environ['LANGUAGE'] = 'en'
         timestr = self.msg_factory.format_time('20170603T191148.000Z')
-        self.assertEqual(timestr, 'Sat, 03 Jun 2017 19:11:48')
+        self.assertEqual(timestr, 'Sat, 03 Jun 2017 19.11.48')
+
+class MessageFactorySummaryTest(unittest.TestCase):
+    def setUp(self):
+        self.clan_info = MagicMock()
+        self.warinfo = WarInfo(
+            json.loads(open(os.path.join('data', 'inWar_40.json'), 'r', encoding='utf8').read()))
+        self.msg_factory = MessageFactory(None, self.warinfo, self.clan_info)
+
+    def test_create_war_summary_msg(self):
+        war_summary_msg = self.msg_factory.create_war_summary_msg()
+
+        self.assertIsInstance(war_summary_msg, discord.Embed)
+        self.assertEqual(war_summary_msg.title, "War Summary")
+
+        print("War Summary Message")
+        for field in war_summary_msg.fields:
+            print(f"{field.name}: {field.value}")
+        print()
+
+    def test_create_players_msg(self):
+        players_msg = self.msg_factory.create_players_msg()
+
+        self.assertIsInstance(players_msg, discord.Embed)
+        self.assertEqual(players_msg.title, "Players")
+
+        print("Players Message")
+        for field in players_msg.fields:
+            print(f"{field.name}: {field.value}")
+        print()
 
 class WarMonitorTestCase(unittest.TestCase):
     def setUp(self):
         coc_api = CoCAPI(None)
         self.warinfo = self.get_warinfo()
         our_claninfo = ClanInfo({'location': {'name': 'Iran',
                                               'isCountry': 'true',
@@ -327,10 +358,41 @@
         with self.assertRaises(ValueError):
             self.monitor.is_msg_sent('war_over_msg')
 
     def test_is_war_over_msg_sent(self):
         self.monitor.warinfo = self.warinfo
         self.assertTrue(self.monitor.is_msg_sent('war_over_msg'))
 
+class TestErrorHandling(unittest.TestCase):
+
+    def setUp(self):
+        coc_api = CoCAPI(None)
+        coc_api.get_currentleague = MagicMock()
+        coc_api.get_previousleague = MagicMock()
+        coc_api.get_currentwar = MagicMock()
+        coc_api.get_claninfo = MagicMock()
+
+        webhook_url = None
+        notifier = DummyNotifier()
+        self.monitor = WarMonitor({}, coc_api, '', notifier)
+
+    def test_error_handling(self):
+        # Mock the update method to raise an exception
+        self.monitor.update = MagicMock(side_effect=Exception("Sample error"))
+
+        # Temporarily replace the notifier.send method with a MagicMock
+        original_send = self.monitor.notifier.send
+        self.monitor.notifier.send = MagicMock()
+
+        # Mock the MessageFactory.create_error_embed static method
+        with patch("GCoCF.formatters.MessageFactory.create_error_embed", lambda error_message, title=None: Embed()):
+            try:
+                self.monitor.start()
+            except Exception as e:
+                self.assertEqual(str(e), "Sample error")
+
+        # Check if the notifier.send method was called with an Embed object
+        send_args = self.monitor.notifier.send.call_args[0]
+        self.assertIsInstance(send_args[0], discord.Embed)
 
 if __name__ == '__main__':
-    unittest.main()
+    unittest.main()
```

