# Comparing `tmp/pyosrs-0.0.3.tar.gz` & `tmp/pyosrs-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyosrs-0.0.3.tar", max compression
+gzip compressed data, was "pyosrs-0.0.4.tar", max compression
```

## Comparing `pyosrs-0.0.3.tar` & `pyosrs-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     7652 2023-05-01 17:25:50.463786 pyosrs-0.0.3/LICENSE
--rw-r--r--   0        0        0     2466 2023-05-01 17:25:50.463786 pyosrs-0.0.3/README.md
--rw-r--r--   0        0        0        0 2023-05-01 17:25:50.463786 pyosrs-0.0.3/pyosrs/__init__.py
--rw-r--r--   0        0        0     6424 2023-05-01 17:25:50.463786 pyosrs-0.0.3/pyosrs/client.py
--rw-r--r--   0        0        0     4503 2023-05-01 17:25:50.463786 pyosrs-0.0.3/pyosrs/enums.py
--rw-r--r--   0        0        0      410 2023-05-01 17:25:50.463786 pyosrs-0.0.3/pyosrs/exceptions.py
--rw-r--r--   0        0        0     3893 2023-05-01 17:25:50.463786 pyosrs-0.0.3/pyosrs/models.py
--rw-r--r--   0        0        0      901 2023-05-01 17:25:50.463786 pyosrs-0.0.3/pyosrs/utils.py
--rw-r--r--   0        0        0      767 2023-05-01 17:25:50.463786 pyosrs-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3200 1970-01-01 00:00:00.000000 pyosrs-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-06-17 14:31:37.020271 pyosrs-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2473 2023-06-17 14:31:37.020271 pyosrs-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-17 14:31:37.020271 pyosrs-0.0.4/pyosrs/__init__.py
+-rw-r--r--   0        0        0     6151 2023-06-17 14:31:37.020271 pyosrs-0.0.4/pyosrs/client.py
+-rw-r--r--   0        0        0     4762 2023-06-17 14:31:37.020271 pyosrs-0.0.4/pyosrs/enums.py
+-rw-r--r--   0        0        0      410 2023-06-17 14:31:37.020271 pyosrs-0.0.4/pyosrs/exceptions.py
+-rw-r--r--   0        0        0     3959 2023-06-17 14:31:37.020271 pyosrs-0.0.4/pyosrs/models.py
+-rw-r--r--   0        0        0      901 2023-06-17 14:31:37.020271 pyosrs-0.0.4/pyosrs/utils.py
+-rw-r--r--   0        0        0      767 2023-06-17 14:31:37.020271 pyosrs-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3207 1970-01-01 00:00:00.000000 pyosrs-0.0.4/PKG-INFO
```

### Comparing `pyosrs-0.0.3/LICENSE` & `pyosrs-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyosrs-0.0.3/README.md` & `pyosrs-0.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 ### Retrieving Hiscores
 
 To retrieve the hiscore for a player, you can create a Pyosrs instance and use its get_hiscore method. Here's an example:
 
 ```python
 import asyncio
-from pyosrs import Pyosrs
+from pyosrs.client import Pyosrs
 from pyosrs.enums import GAME_MODE
 
 async def main():
     async with Pyosrs() as pyosrs:
         hiscore = await pyosrs.get_hiscore("username")
         # With game mode
         hiscore = await pyosrs.get_hiscore("username", GAME_MODE.MAIN)
```

### Comparing `pyosrs-0.0.3/pyosrs/client.py` & `pyosrs-0.0.4/pyosrs/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import asyncio
-from typing import Tuple, Dict
+from typing import Dict, Tuple
 
 import httpx
 
 from .enums import (
     BOSSES_INDEX,
-    CLUES_INDEX,
     GAME_MODE,
     HISCORE_RESPONSE_LEN,
     MINIGAMES_INDEX,
     SKILLS_INDEX,
 )
 from .exceptions import InvalidAPIResponseException, InvalidUserException
-from .models import Bosses, Clues, Hiscore, Minigame, Minigames, Skill, Skills
+from .models import Bosses, Hiscore, Minigame, Minigames, Skill, Skills
 from .utils import calc_combat_level
 
 
 class Pyosrs:
     def __init__(self):
         self.session = httpx.AsyncClient(
             base_url="https://secure.runescape.com/",
@@ -62,32 +61,28 @@
         try:
             response = await self._get_hiscore(username, game_mode)
         except httpx.HTTPStatusError:
             raise InvalidUserException(username)
 
         skills: Dict[str, Skill] = {}
         minigames: Dict[str, Minigame] = {}
-        clues: Dict[str, Minigame] = {}
         bosses: Dict[str, Minigame] = {}
 
         if len(lines := response.text.splitlines()) != HISCORE_RESPONSE_LEN:
             raise InvalidAPIResponseException
 
         for index, line in enumerate(lines):
             if index in SKILLS_INDEX:
                 rank, level, experience = map(int, line.split(","))
                 skills[SKILLS_INDEX[index][0]] = Skill(
                     rank=rank, level=level, experience=experience
                 )
             elif index in MINIGAMES_INDEX:
                 rank, score = map(int, line.split(","))
                 minigames[MINIGAMES_INDEX[index][0]] = Minigame(rank=rank, score=score)
-            elif index in CLUES_INDEX:
-                rank, score = map(int, line.split(","))
-                clues[CLUES_INDEX[index][0]] = Minigame(rank=rank, score=score)
             else:
                 rank, score = map(int, line.split(","))
                 bosses[BOSSES_INDEX[index][0]] = Minigame(rank=rank, score=score)
 
         combat_level = calc_combat_level(
             defence=skills["defence"].level,
             hitpoints=skills["hitpoints"].level,
@@ -100,15 +95,14 @@
 
         return Hiscore(
             username=username,
             game_mode=game_mode,
             combat_level=combat_level,
             skills=Skills(**skills),
             minigames=Minigames(**minigames),
-            clues=Clues(**clues),
             bosses=Bosses(**bosses),
         )
 
     async def get_game_mode(self, username: str) -> Tuple[GAME_MODE, Hiscore]:
         """
         Determines the game mode of a given username by comparing the experience
         levels across different modes using the hiscore API.
```

### Comparing `pyosrs-0.0.3/pyosrs/enums.py` & `pyosrs-0.0.4/pyosrs/enums.py`

 * *Files 15% similar despite different names*

```diff
@@ -40,86 +40,85 @@
     23: ("construction", "Construction"),
 }
 
 MINIGAMES_INDEX: Final[Dict[int, Tuple[str, str]]] = {
     24: ("league_points", "League Points"),
     25: ("bounty_hunter_hunter", "Bounty Hunter - Hunter"),
     26: ("bounty_hunter_rogue", "Bounty Hunter - Rogue"),
-    34: ("lms", "LMS"),
-    35: ("pvp_arena", "PvP Arena"),
-    36: ("soul_wars", "Soul Wars Zeal"),
-    37: ("rifts_closed", "Rifts Closed"),
-}
-
-CLUES_INDEX: Final[Dict[int, Tuple[str, str]]] = {
-    27: ("all", "All"),
-    28: ("beginner", "Beginner"),
-    29: ("easy", "Easy"),
-    30: ("medium", "Medium"),
-    31: ("hard", "Hard"),
-    32: ("elite", "Elite"),
-    33: ("master", "Master"),
+    27: ("bounty_hunter_hunter_legacy", "Bounty Hunter (Legacy) - Hunter"),
+    28: ("bounty_hunter_rogue_legacy", "Bounty Hunter (Legacy) - Rogue"),
+    29: ("clue_scrolls_all", "Clue Scrolls All"),
+    30: ("clue_scrolls_beginner", "Clue Scrolls Beginner"),
+    31: ("clue_scrolls_easy", "Clue Scrolls Easy"),
+    32: ("clue_scrolls_medium", "Clue Scrolls Medium"),
+    33: ("clue_scrolls_hard", "Clue Scrolls Hard"),
+    34: ("clue_scrolls_elite", "Clue Scrolls Elite"),
+    35: ("clue_scrolls_master", "Clue Scrolls Master"),
+    36: ("lms", "LMS"),
+    37: ("pvp_arena", "PvP Arena"),
+    38: ("soul_wars", "Soul Wars Zeal"),
+    39: ("rifts_closed", "Rifts Closed"),
 }
 
 BOSSES_INDEX: Final[Dict[int, Tuple[str, str]]] = {
-    38: ("abyssal_sire", "Abyssal Sire"),
-    39: ("alchemical_hydra", "Alchemical Hydra"),
-    40: ("artio", "Artio"),
-    41: ("barrows_chests", "Barrows Chests"),
-    42: ("bryophyta", "Bryophyta"),
-    43: ("callisto", "Callisto"),
-    44: ("cal_varion", "Calvarion"),
-    45: ("cerberus", "Cerberus"),
-    46: ("chambers_of_xeric", "Chambers of Xeric"),
-    47: (
+    40: ("abyssal_sire", "Abyssal Sire"),
+    41: ("alchemical_hydra", "Alchemical Hydra"),
+    42: ("artio", "Artio"),
+    43: ("barrows_chests", "Barrows Chests"),
+    44: ("bryophyta", "Bryophyta"),
+    45: ("callisto", "Callisto"),
+    46: ("cal_varion", "Calvarion"),
+    47: ("cerberus", "Cerberus"),
+    48: ("chambers_of_xeric", "Chambers of Xeric"),
+    49: (
         "chambers_of_xeric_challenge_mode",
         "Chambers of Xeric: Challenge Mode",
     ),
-    48: ("chaos_elemental", "Chaos Elemental"),
-    49: ("chaos_fanatic", "Chaos Fanatic"),
-    50: ("commander_zilyana", "Commander Zilyana"),
-    51: ("corporeal_beast", "Corporeal Beast"),
-    52: ("crazy_archaeologist", "Crazy Archaeologist"),
-    53: ("dagannoth_prime", "Dagannoth Prime"),
-    54: ("dagannoth_rex", "Dagannoth Rex"),
-    55: ("dagannoth_supreme", "Dagannoth Supreme"),
-    56: ("deranged_archaeologist", "Deranged Archaeologist"),
-    57: ("general_graardor", "General Graardor"),
-    58: ("giant_mole", "Giant Mole"),
-    59: ("grotesque_guardians", "Grotesque Guardians"),
-    60: ("hespori", "Hespori"),
-    61: ("kalphite_queen", "Kalphite Queen"),
-    62: ("king_black_dragon", "King Black Dragon"),
-    63: ("kraken", "Kraken"),
-    64: ("kree_arra", "Kree'Arra"),
-    65: ("kril_tsutsaroth", "K'ril Tsutsaroth"),
-    66: ("mimic", "Mimic"),
-    67: ("nex", "Nex"),
-    68: ("nightmare", "Nightmare"),
-    69: ("phosanis_nightmare", "Phosani's Nightmare"),
-    70: ("obor", "Obor"),
-    71: ("phantom_muspah", "Phantom Muspah"),
-    72: ("sarachnis", "Sarachnis"),
-    73: ("scorpia", "Scorpia"),
-    74: ("skotizo", "Skotizo"),
-    75: ("spindel", "Spindel"),
-    76: ("tempoross", "Tempoross"),
-    77: ("the_gauntlet", "The Gauntlet"),
-    78: ("the_corrupted_gauntlet", "The Corrupted Gauntlet"),
-    79: ("theatre_of_blood", "Theatre of Blood"),
-    80: ("theatre_of_blood_hard_mode", "Theatre of Blood: Hard Mode"),
-    81: ("thermonuclear_smoke_devil", "Thermonuclear Smoke Devil"),
-    82: ("tombs_of_amascut", "Tombs of Amascut"),
-    83: ("tombs_of_amascut_expert_mode", "Tombs of Amascut: Expert Mode"),
-    84: ("tzkal_zuk", "TzKal-Zuk"),
-    85: ("tztok_jad", "TzTok-Jad"),
-    86: ("venenatis", "Venenatis"),
-    87: ("vet_ion", "Vet'ion"),
-    88: ("vorkath", "Vorkath"),
-    89: ("wintertodt", "Wintertodt"),
-    90: ("zalcano", "Zalcano"),
-    91: ("zulrah", "Zulrah"),
+    50: ("chaos_elemental", "Chaos Elemental"),
+    51: ("chaos_fanatic", "Chaos Fanatic"),
+    52: ("commander_zilyana", "Commander Zilyana"),
+    53: ("corporeal_beast", "Corporeal Beast"),
+    54: ("crazy_archaeologist", "Crazy Archaeologist"),
+    55: ("dagannoth_prime", "Dagannoth Prime"),
+    56: ("dagannoth_rex", "Dagannoth Rex"),
+    57: ("dagannoth_supreme", "Dagannoth Supreme"),
+    58: ("deranged_archaeologist", "Deranged Archaeologist"),
+    59: ("general_graardor", "General Graardor"),
+    60: ("giant_mole", "Giant Mole"),
+    61: ("grotesque_guardians", "Grotesque Guardians"),
+    62: ("hespori", "Hespori"),
+    63: ("kalphite_queen", "Kalphite Queen"),
+    64: ("king_black_dragon", "King Black Dragon"),
+    65: ("kraken", "Kraken"),
+    66: ("kree_arra", "Kree'Arra"),
+    67: ("kril_tsutsaroth", "K'ril Tsutsaroth"),
+    68: ("mimic", "Mimic"),
+    69: ("nex", "Nex"),
+    70: ("nightmare", "Nightmare"),
+    71: ("phosanis_nightmare", "Phosani's Nightmare"),
+    72: ("obor", "Obor"),
+    73: ("phantom_muspah", "Phantom Muspah"),
+    74: ("sarachnis", "Sarachnis"),
+    75: ("scorpia", "Scorpia"),
+    76: ("skotizo", "Skotizo"),
+    77: ("spindel", "Spindel"),
+    78: ("tempoross", "Tempoross"),
+    79: ("the_gauntlet", "The Gauntlet"),
+    80: ("the_corrupted_gauntlet", "The Corrupted Gauntlet"),
+    81: ("theatre_of_blood", "Theatre of Blood"),
+    82: ("theatre_of_blood_hard_mode", "Theatre of Blood: Hard Mode"),
+    83: ("thermonuclear_smoke_devil", "Thermonuclear Smoke Devil"),
+    84: ("tombs_of_amascut", "Tombs of Amascut"),
+    85: ("tombs_of_amascut_expert_mode", "Tombs of Amascut: Expert Mode"),
+    86: ("tzkal_zuk", "TzKal-Zuk"),
+    87: ("tztok_jad", "TzTok-Jad"),
+    88: ("venenatis", "Venenatis"),
+    89: ("vet_ion", "Vet'ion"),
+    90: ("vorkath", "Vorkath"),
+    91: ("wintertodt", "Wintertodt"),
+    92: ("zalcano", "Zalcano"),
+    93: ("zulrah", "Zulrah"),
 }
 
 HISCORE_RESPONSE_LEN: Final[int] = (
-    len(SKILLS_INDEX) + len(MINIGAMES_INDEX) + len(CLUES_INDEX) + len(BOSSES_INDEX)
+    len(SKILLS_INDEX) + len(MINIGAMES_INDEX) + len(BOSSES_INDEX)
 )
```

### Comparing `pyosrs-0.0.3/pyosrs/models.py` & `pyosrs-0.0.4/pyosrs/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,28 +41,27 @@
     construction: Skill = Skill()
 
 
 class Minigames(BaseModel):
     league_points: Minigame = Minigame()
     bounty_hunter_hunter: Minigame = Minigame()
     bounty_hunter_rogue: Minigame = Minigame()
-    lms: Minigame = Minigame()
-    pvp_arena: Minigame = Minigame()
-    soul_wars: Minigame = Minigame()
-    rifts_closed: Minigame = Minigame()
-
-
-class Clues(BaseModel):
+    bounty_hunter_hunter_legacy: Minigame = Minigame()
+    bounty_hunter_rogue_legacy: Minigame = Minigame()
     all: Minigame = Minigame()
     beginner: Minigame = Minigame()
     easy: Minigame = Minigame()
     medium: Minigame = Minigame()
     hard: Minigame = Minigame()
     elite: Minigame = Minigame()
     master: Minigame = Minigame()
+    lms: Minigame = Minigame()
+    pvp_arena: Minigame = Minigame()
+    soul_wars: Minigame = Minigame()
+    rifts_closed: Minigame = Minigame()
 
 
 class Bosses(BaseModel):
     alchemical_hydra: Minigame = Minigame()
     artio: Minigame = Minigame()
     barrows_chests: Minigame = Minigame()
     bryophyta: Minigame = Minigame()
@@ -119,9 +118,8 @@
 
 class Hiscore(BaseModel):
     username: str
     game_mode: GAME_MODE
     combat_level: int
     skills: Skills
     minigames: Minigames
-    clues: Clues
     bosses: Bosses
```

### Comparing `pyosrs-0.0.3/pyosrs/utils.py` & `pyosrs-0.0.4/pyosrs/utils.py`

 * *Files identical despite different names*

### Comparing `pyosrs-0.0.3/pyproject.toml` & `pyosrs-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyosrs"
-version = "0.0.3"
+version = "0.0.4"
 description = "A Python library for Oldschool RuneScape."
 authors = ["Phong Tran"]
 repository = "https://github.com/phongse/pyosrs"
 license = "LGPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `pyosrs-0.0.3/PKG-INFO` & `pyosrs-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyosrs
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python library for Oldschool RuneScape.
 Home-page: https://github.com/phongse/pyosrs
 License: LGPL-3.0-only
 Author: Phong Tran
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -33,15 +33,15 @@
 
 ### Retrieving Hiscores
 
 To retrieve the hiscore for a player, you can create a Pyosrs instance and use its get_hiscore method. Here's an example:
 
 ```python
 import asyncio
-from pyosrs import Pyosrs
+from pyosrs.client import Pyosrs
 from pyosrs.enums import GAME_MODE
 
 async def main():
     async with Pyosrs() as pyosrs:
         hiscore = await pyosrs.get_hiscore("username")
         # With game mode
         hiscore = await pyosrs.get_hiscore("username", GAME_MODE.MAIN)
```

